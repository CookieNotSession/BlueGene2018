# BlueGene2018

digraph G {
//把图片的尺寸设为4inch * 4inch
size = "4,4";
main [shape = box];

//边的重要程度，默认是1
main->parse [weight = 8];
parse->execute;

//点状线
main->init[style = dotted];
main->cleanup;

//连接了两条线
execute->{make_string;printf}
init->make_string;

//把边的默认颜色设为red
edge [color = red];
main->printf [sytle=bold, label = "100times"];

//节点的名称
make_string [label = "make a\nstring"];

//设置节点的默认属性
node [shape=box,style =filled,color=lightgrey];
execute->compare;
}

作者：我的孙女叫小芳
链接：https://www.jianshu.com/p/4ecbaf31385d
來源：简书
简书著作权归作者所有，任何形式的转载都请联系作者获得授权并注明出处。
