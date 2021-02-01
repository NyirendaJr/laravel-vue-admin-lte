<template>
       <div class="card card-info card-outline">
            <div class="card-header">
            <h3 class="card-title">
                <i class="fas fa-edit"></i>
                Toasts Examples <small>built in AdminLTE</small>
            </h3>
            </div>
            <div class="card-body">
            <br />
            <button type="button" class="btn btn-success" @click="openDefaultToast()">
                Launch Success Toast
            </button>
            </div>
        </div>
      </div>
</template>

<script>
export default {
    data() {
        return {

        }
    },
    methods: {
        openDefaultToast() {
            console.log('Before opening the toast..');
            $(document).Toasts('create', {
                class: 'bg-success',
                title: 'Toast Title',
                subtitle: 'Subtitle',
                body: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr.'
            })
        },
    }
}
</script>