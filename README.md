var btn3 = document.getElementById('btn3');
var clipboard3 = new Clipboard(btn3, {
    text: function() {
        return '333-JS里指定复制的内容';
    }
});
clipboard3.on('success', function(e) {//复制成功执行的回调，可选
    console.log(e);
});
clipboard3.on('error', function(e) {//复制失败执行的回调，可选
    console.log(e);
});
