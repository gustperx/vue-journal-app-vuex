<template>
    <div class="entry-title d-flex justify-content-between p2">
        <div>
            <span class="text-success fs-3 fw-bold">15</span>
            <span class="mx-1 fs-3">Julio</span>
            <span class="mx-2 fs-4 fw-light">2021, Jueves</span>
        </div>

        <div>
            <button class="btn btn-danger mx-1 my-1">
                Borrar
                <i class="fa fa-trash-alt"></i>
            </button>
            <button class="btn btn-primary mx-1">
                Subir foto
                <i class="fa fa-upload"></i>
            </button>
        </div>
    </div>

    <div class="d-flex flex-column px-3 h-75">
        <textarea 
            placeholder="¿Qué sucedio hoy?"
        ></textarea>
    </div>

    <FlorinActionButton 
        icon="fa-save"
    />

    <img 
        src="https://www.openenglish.com/blog/es/wp-content/uploads/sites/2/2016/02/geek-en-ingles-blog.jpg" 
        alt="entry-picture"
        class="img-thumbnail"    
    >

</template>

<script>
import { defineAsyncComponent } from 'vue'

export default {
    components: {
        FlorinActionButton: defineAsyncComponent(() => import('../components/FlorinActionButton'))
    }
}
</script>

<style lang="scss" scoped>

textarea {
    font-size: 20px;
    border: none;
    height: 100%;

    &:focus {
        outline: none;
    }
}

img {
    width: 200px;
    position: fixed;
    bottom: 150px;
    right: 20px;
    box-shadow: 0px 6px 10px rgba($color: #000000, $alpha: 0.2);
}

</style>