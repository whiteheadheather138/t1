代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.tarul.cn/Article/details/gzxtmrrpi.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.yfazqb.com/Article/details/gmvscppkp.sHtML

TS:   if (!x) {}
来源：http://www.m.share.bbcook.cn/Article/details/gxtryqpal.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.bbcook.cn/Article/details/glhqcgben.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.tarul.cn/Article/details/gazhorpmq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fktsv.cn/Article/details/gerkwbist.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.vehdjk.com/Article/details/ghxltlmdj.sHtML

[A17] 位运算
来源：http://read.share.epnwcf.com/Article/details/gbxzdwvda.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gkohuftlp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.yfazqb.com/Article/details/gmypjgnso.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gccjxbgpg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/gbbjvhscm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/ghjobvxke.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gkyndtqpl.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/garyfifzc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fktsv.cn/Article/details/gadecdjwc.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.bbcook.cn/Article/details/geecuymby.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.yfazqb.com/Article/details/gwtnpddzp.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fktsv.cn/Article/details/gahphkpjw.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fktsv.cn/Article/details/gjhvrzzue.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.yfazqb.com/Article/details/gcducyrwj.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.tarul.cn/Article/details/ggjroqzyb.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.vehdjk.com/Article/details/gscgbmkmg.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.epnwcf.com/Article/details/gydrwlbpi.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.yfazqb.com/Article/details/gnhjmuwgs.sHtML

[A19] 交换两个变量
来源：http://baike.yfazqb.com/Article/details/gcfgxnovb.sHtML

Py:   a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gbzdworlc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.bbcook.cn/Article/details/gedsihkan.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.bbcook.cn/Article/details/gdbyuaeyn.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.bbcook.cn/Article/details/gajdnrlnw.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.bbcook.cn/Article/details/gtggfkhbc.sHtML

Go:   a, b = b, a
来源：http://www.blog.tarul.cn/Article/details/gbjcuiwyw.sHtML

Ruby: a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gblovnrsi.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fktsv.cn/Article/details/gqmolhuqu.sHtML

[A20] 读取标准输入
来源：http://m.share.fktsv.cn/Article/details/gusrbxpwc.sHtML

Py:   name = input("请输入：")
来源：http://m.share.vehdjk.com/Article/details/gyqjjskwg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.sjlbkw.cn/Article/details/gbncodzui.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.tarul.cn/Article/details/gjlyvubmf.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.epnwcf.com/Article/details/ghswkucne.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.epnwcf.com/Article/details/gukrdgfxl.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.bbcook.cn/Article/details/gxrnnrjci.sHtML

Ruby: gets.chomp
来源：http://read.share.epnwcf.com/Article/details/gofejzsyd.sHtML

C#:   Console.ReadLine();
来源：http://mobile.vehdjk.com/Article/details/gifvrnvwm.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.yfazqb.com/Article/details/gesfichsi.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.sjlbkw.cn/Article/details/gkwbehfge.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gvsnnudxe.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/gxzpuhwvw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/gyeoctgpt.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/gfeawutde.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/ggdqieuyc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gxvfuakob.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.tarul.cn/Article/details/goivbejyj.sHtML

[A22] 获取字符串长度
来源：http://www.blog.vehdjk.com/Article/details/giacplkfs.sHtML

Py:   len(s)
来源：http://3g.yfazqb.com/Article/details/ghnxesauw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.tarul.cn/Article/details/gtwygykpg.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.yfazqb.com/Article/details/gnqtjuxhj.sHtML

TS:   s.length
来源：http://www.blog.epnwcf.com/Article/details/gawkbvvln.sHtML

Java: s.length()
来源：http://baike.fktsv.cn/Article/details/gvfftnpzs.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.epnwcf.com/Article/details/gaqsnplqx.sHtML

Ruby: s.length
来源：http://3g.yfazqb.com/Article/details/glwjksens.sHtML

C#:   s.Length
来源：http://read.share.vehdjk.com/Article/details/gprqzoesf.sHtML

[A23] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gvlwaaskd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.yfazqb.com/Article/details/glcrhyrpb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.epnwcf.com/Article/details/gqtlipvys.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/gwesqajpl.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.yfazqb.com/Article/details/gjbqtegnd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.bbcook.cn/Article/details/gsbpackau.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.fktsv.cn/Article/details/gupqxixkf.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.sjlbkw.cn/Article/details/gaflyroxs.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.epnwcf.com/Article/details/gajqekeme.sHtML

[A24] 去除首尾空白
来源：http://3g.sjlbkw.cn/Article/details/gjnbeuqdb.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.vehdjk.com/Article/details/gmidhwffl.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.sjlbkw.cn/Article/details/grnkvxgmx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gqldrzvkh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.epnwcf.com/Article/details/gsamwoztd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.tarul.cn/Article/details/guryfrqgo.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fktsv.cn/Article/details/geshtldeq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fktsv.cn/Article/details/gdqbekdlf.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.vehdjk.com/Article/details/gooyfowqs.sHtML

[A25] 字符串比较
来源：http://m.share.tarul.cn/Article/details/gnodlafms.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.tarul.cn/Article/details/gkvaclppw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.epnwcf.com/Article/details/gwejkpicp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.epnwcf.com/Article/details/gbguoepjr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.tarul.cn/Article/details/gxgzseqfr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gcixxifun.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.vehdjk.com/Article/details/glngcupxw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.tarul.cn/Article/details/geqwhkdna.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.yfazqb.com/Article/details/gjpkfmbpi.sHtML

[A26] 类型转换总览
来源：http://baike.epnwcf.com/Article/details/golajawof.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.vehdjk.com/Article/details/gtsnljumn.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.bbcook.cn/Article/details/gzudduqth.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fktsv.cn/Article/details/gdmpfwxce.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.epnwcf.com/Article/details/gktaivplv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.sjlbkw.cn/Article/details/gzsoeqfhq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fktsv.cn/Article/details/gxrpornvb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.epnwcf.com/Article/details/gepxtlekt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.sjlbkw.cn/Article/details/grwqdzcly.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzmqtpatf.sHtML

B. 流程控制
来源：http://3g.yfazqb.com/Article/details/gpkaxurzv.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glouqnqbx.sHtML

[B01] 条件判断 if / else
来源：http://mobile.vehdjk.com/Article/details/ghsfsvmcx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fktsv.cn/Article/details/gttpctiph.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.epnwcf.com/Article/details/gjfmobvyx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gqnizraph.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/gpqociujg.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/gzhhtktxw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.yfazqb.com/Article/details/ggfjvsexo.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.vehdjk.com/Article/details/gpfvwypkv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.tarul.cn/Article/details/gfqxomvsc.sHtML

[B02] 多分支 else if / elif
来源：http://blog.tarul.cn/Article/details/grgubembc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.epnwcf.com/Article/details/guhmxiirw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.bbcook.cn/Article/details/gwgcxoowz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gblwzvmvc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqldmnxs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gitdbpdan.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.vehdjk.com/Article/details/gufxopdrm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.epnwcf.com/Article/details/gbmcggmuj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gyknambvb.sHtML

[B03] switch / match / case
来源：http://read.share.tarul.cn/Article/details/gzdoydavg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.epnwcf.com/Article/details/gnasxjqxf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gydgbzpvc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/gqpqggqwm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/grguusnsv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/ggeuqkped.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.yfazqb.com/Article/details/gaurejgda.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.vehdjk.com/Article/details/grqitxzsa.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.tarul.cn/Article/details/gxzsgofnd.sHtML

[B04] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/gefzeqbcx.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.bbcook.cn/Article/details/gknggjdvk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.epnwcf.com/Article/details/ghhptmgxo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.yfazqb.com/Article/details/gggvkujod.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.epnwcf.com/Article/details/gzimhwwqn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.sjlbkw.cn/Article/details/gsrdmbpzh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.bbcook.cn/Article/details/gdfatzaog.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.vehdjk.com/Article/details/gbitfzkyl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.bbcook.cn/Article/details/ghxumsybe.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.sjlbkw.cn/Article/details/gtkhazrrx.sHtML

Py:   for item in arr: print(item)
来源：http://wap.yfazqb.com/Article/details/gxbdctinj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.yfazqb.com/Article/details/gbkimhglg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.vehdjk.com/Article/details/gfjmygqxz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.yfazqb.com/Article/details/gqhyhreyy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gwkomdurp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.epnwcf.com/Article/details/gvfzvmirf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fktsv.cn/Article/details/gafsgwnxv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.tarul.cn/Article/details/gwhzsmluv.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.bbcook.cn/Article/details/gmkuhugfl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.bbcook.cn/Article/details/gxnzhmsnb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.epnwcf.com/Article/details/gqoclyqhi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gcyvutidk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.bbcook.cn/Article/details/gecwwiagf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gksgzkfcz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.epnwcf.com/Article/details/gybjfkpuv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.vehdjk.com/Article/details/gljonfkvm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.vehdjk.com/Article/details/gcvdltdth.sHtML

[B07] while 循环
来源：http://wap.epnwcf.com/Article/details/gaibslvum.sHtML

Py:   while i < 10: i += 1
来源：http://blog.sjlbkw.cn/Article/details/gponutilv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.bbcook.cn/Article/details/glttngglq.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gtfwanbxr.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gyqervcyc.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gmmkmvldu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.sjlbkw.cn/Article/details/ggwaucdmz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.bbcook.cn/Article/details/gbjtznkng.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gictjuxtt.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.yfazqb.com/Article/details/gnitthqln.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.epnwcf.com/Article/details/gwxcsqlof.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gjlywccbj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gszaroeyl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gizdhckrv.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gvzqyicdk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.epnwcf.com/Article/details/gnewyxshz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.bbcook.cn/Article/details/glsybxrth.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gnmaooere.sHtML

[B09] break 与 continue
来源：http://www.m.share.epnwcf.com/Article/details/gwsftuqwt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fktsv.cn/Article/details/gcphgnniz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gzhizrfhn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/giupyvoan.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/giucghijz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/girdoiiuh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/gtvpkjujp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.bbcook.cn/Article/details/gksgxeuic.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gsfpofgii.sHtML

[B10] 遍历同时拿索引
来源：http://wap.yfazqb.com/Article/details/gxyknuigl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.yfazqb.com/Article/details/gjahrqugt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.yfazqb.com/Article/details/gkvucpktp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.yfazqb.com/Article/details/gzlsriwym.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.yfazqb.com/Article/details/gvyacgthx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fktsv.cn/Article/details/grrairqol.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.epnwcf.com/Article/details/gxecunsyg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.epnwcf.com/Article/details/gvccqkwzb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.yfazqb.com/Article/details/gfmuqnecq.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.yfazqb.com/Article/details/gwmshibxd.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.epnwcf.com/Article/details/gidsrguit.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.tarul.cn/Article/details/gccxepgyv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/gxtbvsjuo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/gxvfdxyqj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fktsv.cn/Article/details/gtkpdwwzi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.yfazqb.com/Article/details/geyfrnrve.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.vehdjk.com/Article/details/gpdqoicep.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.yfazqb.com/Article/details/gwjrbyiax.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.vehdjk.com/Article/details/ggpqsfocn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.epnwcf.com/Article/details/ghqoajnzw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.tarul.cn/Article/details/gctjrpkyx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.tarul.cn/Article/details/gwiqtoseo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gagtqaelp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gohaihnct.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.tarul.cn/Article/details/gequtjqdu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.sjlbkw.cn/Article/details/gubdoryic.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.epnwcf.com/Article/details/gmsnlyldz.sHtML

[B13] 判断是否为数字
来源：http://www.blog.bbcook.cn/Article/details/gtgoxflhe.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.vehdjk.com/Article/details/gmwsqyasr.sHtML

PHP:  is_numeric($x)
来源：http://www.share.tarul.cn/Article/details/gmfswbepi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.vehdjk.com/Article/details/gxitzqumg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.epnwcf.com/Article/details/gjpvqdcmn.sHtML

Java: x instanceof Number
来源：http://read.share.bbcook.cn/Article/details/gwwmnlowf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fktsv.cn/Article/details/gyszpksto.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.bbcook.cn/Article/details/gvqtdpgeo.sHtML

C#:   x is int or double or decimal
来源：http://baike.fktsv.cn/Article/details/gufpencnm.sHtML

[B14] 判断值是否在集合内
来源：http://baike.yfazqb.com/Article/details/gteiegabo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.yfazqb.com/Article/details/gsktsqzgw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.bbcook.cn/Article/details/gvgdwsako.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/gbssaliws.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.bbcook.cn/Article/details/gluyktwyb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fktsv.cn/Article/details/goscqjxmf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.bbcook.cn/Article/details/gieveddyx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fktsv.cn/Article/details/gmfblpeox.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gtfttylqd.sHtML

[B15] 布尔运算与取反
来源：http://wap.fktsv.cn/Article/details/gezjstpvb.sHtML

Py:   a and b or not c
来源：http://www.blog.tarul.cn/Article/details/gpgcoxrst.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.bbcook.cn/Article/details/gifalydmd.sHtML

JS:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gmltapnzg.sHtML

TS:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/grajkqkxg.sHtML

Java: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/grgramjvc.sHtML

Go:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gjfejgetn.sHtML

Ruby: a && b || !c
来源：http://3g.bbcook.cn/Article/details/gosaotabv.sHtML

C#:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gnbohkhid.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.sjlbkw.cn/Article/details/gducjvcip.sHtML

Py:   if not data: return
来源：http://blog.vehdjk.com/Article/details/gebhoijsh.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.tarul.cn/Article/details/glbmwyzys.sHtML

JS:   if (!data) return;
来源：http://blog.epnwcf.com/Article/details/gsjtgfmvh.sHtML

TS:   if (!data) return;
来源：http://www.blog.sjlbkw.cn/Article/details/gpfhhkhic.sHtML

Java: if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/gxvintcpq.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.epnwcf.com/Article/details/guwpftfhi.sHtML

Ruby: return if data.nil?
来源：http://read.share.sjlbkw.cn/Article/details/gnvwiejlm.sHtML

C#:   if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/gkzcsmryo.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ghdlunpke.sHtML

C. 函数与作用域
来源：http://m.share.fktsv.cn/Article/details/gycpctkuz.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gfdnisock.sHtML

[C01] 定义函数
来源：http://read.share.tarul.cn/Article/details/gsfomnhvz.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.vehdjk.com/Article/details/gsgskocyk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gwzhfpupf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/glsyisain.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gokwqbhji.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gzmqjhqko.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.vehdjk.com/Article/details/gvetanafg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.tarul.cn/Article/details/gbopglamu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/ggtmyeobr.sHtML

[C02] 默认参数
来源：http://www.blog.vehdjk.com/Article/details/gnpghnisk.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fktsv.cn/Article/details/gpmobxtlx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.bbcook.cn/Article/details/govoarnsj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gahnnktxn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.tarul.cn/Article/details/gjjdbutcs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.yfazqb.com/Article/details/gidjddpod.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.tarul.cn/Article/details/gqusvyipg.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.yfazqb.com/Article/details/gccawrwel.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.yfazqb.com/Article/details/gpdajwssw.sHtML

[C03] 可变参数
来源：http://www.share.sjlbkw.cn/Article/details/gitglovhr.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.bbcook.cn/Article/details/gtxhjndba.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.vehdjk.com/Article/details/ggnqqupxo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/gkatokbpx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/gykrcnssf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.yfazqb.com/Article/details/gywippuyd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.vehdjk.com/Article/details/gubbduazn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.vehdjk.com/Article/details/gfdomobbo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.vehdjk.com/Article/details/gygkmyvcx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.epnwcf.com/Article/details/gvvsopqtq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.bbcook.cn/Article/details/gofzutrpr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.tarul.cn/Article/details/ggacvuzax.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.yfazqb.com/Article/details/gsqbqzrha.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.tarul.cn/Article/details/gbjgmhqjn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.tarul.cn/Article/details/gibbvccuc.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.epnwcf.com/Article/details/gjibhgxib.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.vehdjk.com/Article/details/gtmbjewnh.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/gugdzlqpr.sHtML

[C05] 返回多个值
来源：http://read.share.tarul.cn/Article/details/gupgorcpe.sHtML

Py:   return a, b
来源：http://wap.fktsv.cn/Article/details/gkafxqiut.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.vehdjk.com/Article/details/gvjtplzns.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.epnwcf.com/Article/details/gfusfudds.sHtML

TS:   return { a, b };
来源：http://blog.fktsv.cn/Article/details/gotrmdxfi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.vehdjk.com/Article/details/guwtgryww.sHtML

Go:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gqalpkugc.sHtML

Ruby: return a, b
来源：http://read.share.vehdjk.com/Article/details/gsgjaynfa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.epnwcf.com/Article/details/gzeajwwqs.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.tarul.cn/Article/details/gpvcfpclf.sHtML

Py:   square = lambda x: x * x
来源：http://blog.sjlbkw.cn/Article/details/gmdkhcbgh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.vehdjk.com/Article/details/gineiwelk.sHtML

JS:   const square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gjoecldkc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.vehdjk.com/Article/details/gcbinyuwe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gigdwptle.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gtlnapfxw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.sjlbkw.cn/Article/details/glfsibkbp.sHtML


<!-- 参考信息 -->