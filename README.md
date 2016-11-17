# Use

- Create folder: uploads/drive in forlder public of Laravel, then chmod 777 it!

JS:
{!! Html::script('global/plugins/laravel.tinymce/tinymce.min.js') !!}

Javascript:

    if (typeof tinymce != 'undefined'){
        tinymce.init({
            selector:'textarea.tinymce',
            theme: "modern",
            menubar : true,
            height: 300,
            plugins: [
                "advlist autolink link image lists charmap print preview hr anchor pagebreak",
                "searchreplace wordcount visualblocks visualchars insertdatetime media nonbreaking",
                "table contextmenu directionality emoticons paste textcolor responsivefilemanager code fullscreen"
     ],
        toolbar1: "fullscreen | undo redo | bold italic underline | alignleft aligncenter alignright alignjustify | bullist numlist outdent indent" +
        " |" +
        " styleselect  | removeformat",
            toolbar2: "link unlink anchor | responsivefilemanager filemanager image media | forecolor backcolor  | print preview code",
            image_advtab: true ,
            external_filemanager_path:"/global/plugins/laravel.tinymce/plugins/filemanager/",
            filemanager_title:"Responsive Filemanager" ,
            external_plugins: { "filemanager" : "/global/plugins/laravel.tinymce/plugins/filemanager/plugin.min.js"}
        });
    }
