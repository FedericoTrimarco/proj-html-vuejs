<template>
  <div class="section-six container border">
      <!-- info -->
        <div class="section-six-top border d-flex justify-content-between align-items-end">
            <div class="section-six-top-info">
                <span class="fw-bold ">All time best sellers</span>
                <p>Items everyone loves</p>
            </div>
            <button class="btn btn-green">View all products</button>
        </div>
        <!-- products -->
        <div class="section-six-bottom border">
        </div>
  </div>
</template>

<script>
export default {
    name:'SectionSix',
    
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';
.section-six{
    .section-six-top-info{
        span{
            color: $bayLeaf;
            letter-spacing: 3px;
            font-size: 20px;

        }
        p{
            font-family: 'Domine', serif;
            font-size: 40px;
            margin-top: 30px
        }
    }
}

</style>