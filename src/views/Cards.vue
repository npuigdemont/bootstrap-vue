<template>
    <div class="m-5">
        <b-button pill class="m-2" variant="outline-primary">Text</b-button>
        <b-button pill class="m-2" variant="outline-secondary">Text</b-button>
        <b-button pill class="m-2" variant="outline-success">Text</b-button>
    

    <b-row class="mt-3">
        <b-col cols="12" md="4" class="m-3">
            <b-card
              title="Card Title"
               img-src="https://picsum.photos/600/300/?image=25"
                img-alt="Image"
                 img-top
                   tag="article"
                  style="max-width: 20rem;"
                 >
        <p>
    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laudantium et iste ipsam magni neque soluta quia. Iure maxime temporibus nisi pariatur, odit possimus quos porro labore, assumenda quo unde totam.
        </p>
            <b-button class="m-2" href="#" variant="outline-info">Text</b-button>
            </b-card>
        </b-col>

         <b-col cols="12" md="4" class="m-3">
            <b-card
              title="Card Title"
               img-src="https://picsum.photos/600/300/?image=25"
                img-alt="Image"
                 img-top
                   tag="article"
                  style="max-width: 20rem;"
                 >
        <p>
    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laudantium et iste ipsam magni neque soluta quia. Iure maxime temporibus nisi pariatur, odit possimus quos porro labore, assumenda quo unde totam.
        </p>
            <b-button class="m-2" href="#" variant="outline-info">Text</b-button>
            </b-card>
        </b-col>
    </b-row>
    </div>
</template>

<script>
export default {
    name: 'Cards'
}
</script>