
<template>
    <div>

        <form action="/upload" class="dropzone" id="dpUpload" method="post" enctype="multipart/form-data">
                <div class="fallback">
                    <input type="file" name="image" accept="image/x-png,image/jpeg" required>
                    <input type="submit" value="Upload" name="submit">
                    <input type="hidden" value="{{csrf_token()}}" name="_token">
                </div>
            </form>
        
    </div>
</template>





<script>
export default {
    data: function() {
        return {}
    }
}
</script>

<style lang="css">
</style>
