let shadow_shade = {
    show: (html) => {
        if ($(".shadow_box")) {
            shadow_shade.hidden();
        }
        let div = document.createElement("div");
        div.className = "_shadow_box";
        div.innerHTML = "<div style='position: absolute;z-index: 9999990;left: 48%;top: 45%;color:#FFFFFF;'><img src='image/loading.gif' class='_shadow_box_inner_img'>" +
            "<span style='margin: 10px;' class='_shadow_box_inner_span'>" + (html == null ? "" : html) + "</span></div>";
        $("body").append(div);
        $("head").append("<style>" +
            "._shadow_box{" +
            "position:absolute;" +
            "top:0;" +
            "bottom:0;" +
            "left:0;" +
            "right:0;" +
            "z-index: 999999;" +
            "background:rgba(0,0,0,0.6);" +
            "}</style>");
    },
    updateHTML: (html) => {
        $("._shadow_box_inner_span").html(html);
    },
    updateImg: (src) => {
        $("._shadow_box_inner_img").attr("src", src);
    },
    hidden: () => {
        $("._shadow_box").remove();
    }
};
