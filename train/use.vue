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

$font('N1')

map-get($fonts,"N1")

@mixin when($state){
  @at-root{
    &.#{'is-'+$state}{
      @content;
    }
  }
}

</style>




