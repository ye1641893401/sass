<style>
@import "./style/_index.sass"

%border{
  content:'';
  position:absolute;
  box-sizing:border-box;
  width:100%;
  height:100%;
  top:0;
  left:0;
}

%border-top {
  &::before{
    @extend %border;
    @include retina-border(top)
  }
}
</style>




