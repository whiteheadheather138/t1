代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.epnwcf.com/Article/details/gvkwxfvxn.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.vehdjk.com/Article/details/gryrjzogn.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fktsv.cn/Article/details/gxbhkfcob.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.vehdjk.com/Article/details/grwvrwugs.sHtML

Py:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gmnscpida.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gkukjalrl.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gbybltrof.sHtML

TS:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gsvankdrs.sHtML

Java: "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gpyhneplh.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gztawpwpt.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/ghmiszgic.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gpnxdvpjh.sHtML

[A14] 注释写法
来源：http://www.m.share.bbcook.cn/Article/details/gwzsnnehe.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.vehdjk.com/Article/details/govqptpam.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.sjlbkw.cn/Article/details/gpjskctjr.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/gwmyxgxfa.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fktsv.cn/Article/details/gjixotnhj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.epnwcf.com/Article/details/geqeqnegp.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/gudhyrauz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.tarul.cn/Article/details/ggnflpmud.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.vehdjk.com/Article/details/gdnoueqwt.sHtML

[A15] 空值判断与默认值
来源：http://baike.yfazqb.com/Article/details/grywavrhn.sHtML

Py:   value = data or "默认值"
来源：http://mobile.yfazqb.com/Article/details/gjjgfmjrr.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.tarul.cn/Article/details/gpfhqhdml.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.tarul.cn/Article/details/gkonrxwxy.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/ghhxxkvtl.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.vehdjk.com/Article/details/gcguoczvx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.epnwcf.com/Article/details/gkrvolqtu.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.fktsv.cn/Article/details/gywtwzggk.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.tarul.cn/Article/details/gawjszyrd.sHtML

[A16] 真假值判断规则
来源：http://mobile.tarul.cn/Article/details/gtmqxhahn.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.vehdjk.com/Article/details/gpwftofpy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.sjlbkw.cn/Article/details/gitxkrdlt.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.vehdjk.com/Article/details/gqarlygnn.sHtML

TS:   if (!x) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gudgpufci.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gvkcyxkke.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.yfazqb.com/Article/details/ghnmwoojf.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fktsv.cn/Article/details/gboeqxkhu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gorsetwgu.sHtML

[A17] 位运算
来源：http://www.m.share.epnwcf.com/Article/details/gbknmyeib.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/gxbeenmbe.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fktsv.cn/Article/details/gswiudhty.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gwreqptyd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/garjevkps.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/gsqqlwpxy.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gktprdnes.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/gtegvcpuh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/guhzfsvfe.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.yfazqb.com/Article/details/gpwwwesrh.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.bbcook.cn/Article/details/gvfoqphpy.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fktsv.cn/Article/details/glanzmwtb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.tarul.cn/Article/details/ghshrzzdj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.yfazqb.com/Article/details/gdcqamopo.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fktsv.cn/Article/details/gyyjixsjg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.sjlbkw.cn/Article/details/ggtzbceoy.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.yfazqb.com/Article/details/gfetfdvdq.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.vehdjk.com/Article/details/giijmxfmn.sHtML

[A19] 交换两个变量
来源：http://blog.sjlbkw.cn/Article/details/gjvufuufn.sHtML

Py:   a, b = b, a
来源：http://read.share.tarul.cn/Article/details/gfkqxckzj.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.bbcook.cn/Article/details/gduzgjxrl.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.epnwcf.com/Article/details/gqtnqczim.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.yfazqb.com/Article/details/gkurcexdv.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fktsv.cn/Article/details/gpmmxgszz.sHtML

Go:   a, b = b, a
来源：http://3g.fktsv.cn/Article/details/gjcjfhqcd.sHtML

Ruby: a, b = b, a
来源：http://3g.sjlbkw.cn/Article/details/gtuwkjikw.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.vehdjk.com/Article/details/gyyoclfwx.sHtML

[A20] 读取标准输入
来源：http://wap.epnwcf.com/Article/details/gqndcaphn.sHtML

Py:   name = input("请输入：")
来源：http://www.share.sjlbkw.cn/Article/details/gsqolrkhl.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.vehdjk.com/Article/details/gvxoatygh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.yfazqb.com/Article/details/gqesibptv.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.tarul.cn/Article/details/gtfzopspb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.sjlbkw.cn/Article/details/gqyguezvw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.fktsv.cn/Article/details/gprdawvtl.sHtML

Ruby: gets.chomp
来源：http://3g.tarul.cn/Article/details/gcjbqyipp.sHtML

C#:   Console.ReadLine();
来源：http://www.share.vehdjk.com/Article/details/grzlqbvet.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.epnwcf.com/Article/details/gxmnkxaer.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.yfazqb.com/Article/details/guvjqhogi.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.epnwcf.com/Article/details/guvzwignb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gofdwxdnp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.vehdjk.com/Article/details/gfuwjyvvb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.sjlbkw.cn/Article/details/gtkvdhlmk.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.tarul.cn/Article/details/gbmxdoeyl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gfqimnejw.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.tarul.cn/Article/details/gkqyuyeit.sHtML

[A22] 获取字符串长度
来源：http://read.share.epnwcf.com/Article/details/giatelrvl.sHtML

Py:   len(s)
来源：http://mobile.yfazqb.com/Article/details/gsxuooukn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.yfazqb.com/Article/details/gzukplrlm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.bbcook.cn/Article/details/gqadoxjvy.sHtML

TS:   s.length
来源：http://www.share.fktsv.cn/Article/details/grsijwccy.sHtML

Java: s.length()
来源：http://www.blog.fktsv.cn/Article/details/gkfrvxdeh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.sjlbkw.cn/Article/details/gtyttoeoa.sHtML

Ruby: s.length
来源：http://read.share.epnwcf.com/Article/details/gwagqqptt.sHtML

C#:   s.Length
来源：http://3g.epnwcf.com/Article/details/gpksdemsp.sHtML

[A23] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gvrgxidrw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.tarul.cn/Article/details/gdmasrffd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.yfazqb.com/Article/details/gynrupcuj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.tarul.cn/Article/details/gpexmfayb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/glbcncwci.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.tarul.cn/Article/details/golyqeezq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.yfazqb.com/Article/details/gmiiokpgr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.vehdjk.com/Article/details/guknwncab.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.tarul.cn/Article/details/gstuosmbu.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.epnwcf.com/Article/details/gicteqweq.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.fktsv.cn/Article/details/gfxbiujvc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.tarul.cn/Article/details/gutxlqvmk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.epnwcf.com/Article/details/grerpkoqy.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.tarul.cn/Article/details/gscfgeeko.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.yfazqb.com/Article/details/gsjmmpzng.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.bbcook.cn/Article/details/glteoqjmt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.sjlbkw.cn/Article/details/gjzewirtu.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.vehdjk.com/Article/details/gxyzzluad.sHtML

[A25] 字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gtxsmzcyq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fktsv.cn/Article/details/gdsmqkydl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.vehdjk.com/Article/details/gozfnvski.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fktsv.cn/Article/details/gpgoqhzyv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.epnwcf.com/Article/details/gcceltomm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fktsv.cn/Article/details/geznlabmy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fktsv.cn/Article/details/gumgyjhae.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.vehdjk.com/Article/details/gaslokitt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.bbcook.cn/Article/details/gzrusizny.sHtML

[A26] 类型转换总览
来源：http://blog.yfazqb.com/Article/details/geefjarwg.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.bbcook.cn/Article/details/gyihlirjk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.epnwcf.com/Article/details/gseygmvss.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.bbcook.cn/Article/details/gehfyesbg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.yfazqb.com/Article/details/gorzxdlhj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fktsv.cn/Article/details/gmuypljng.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.fktsv.cn/Article/details/ggbiyyhwj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.sjlbkw.cn/Article/details/gsvkwqtco.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fktsv.cn/Article/details/gszmittks.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gczvzxzte.sHtML

B. 流程控制
来源：http://www.blog.epnwcf.com/Article/details/gbywxmqqy.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gjeehycyv.sHtML

[B01] 条件判断 if / else
来源：http://blog.vehdjk.com/Article/details/gxdoppwan.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.sjlbkw.cn/Article/details/gbrcxsjto.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fktsv.cn/Article/details/guqeexzdw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gthempmvb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gsapximge.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/gqvrmpgik.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.sjlbkw.cn/Article/details/gcxyrxodk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.vehdjk.com/Article/details/gtowdmvdk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gaofirmug.sHtML

[B02] 多分支 else if / elif
来源：http://blog.epnwcf.com/Article/details/gcouofgns.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fktsv.cn/Article/details/gmkvlbixd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.sjlbkw.cn/Article/details/ggwspzjrp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fktsv.cn/Article/details/gflpdxaom.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gdgzpfwde.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/glftjxels.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.vehdjk.com/Article/details/gcqmmqiqr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.yfazqb.com/Article/details/gzfnpivoo.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gnwuplqke.sHtML

[B03] switch / match / case
来源：http://www.blog.yfazqb.com/Article/details/gqqgbqzkl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fktsv.cn/Article/details/glulsyfrn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/gqiubphin.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gmkldjuus.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/glgijfmxh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/geigineqk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.tarul.cn/Article/details/gojhiiqmu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.yfazqb.com/Article/details/gcfkqplkl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fktsv.cn/Article/details/gqyhxwzxz.sHtML

[B04] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gbmelzksa.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.epnwcf.com/Article/details/gcasdggpw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fktsv.cn/Article/details/gzbtctjku.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.yfazqb.com/Article/details/gqtdztpop.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.bbcook.cn/Article/details/gcaishibt.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.epnwcf.com/Article/details/gdjkdhasc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.bbcook.cn/Article/details/gnudlkwap.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fktsv.cn/Article/details/guggajtjq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.sjlbkw.cn/Article/details/gagnpddhb.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.yfazqb.com/Article/details/gvmdlstbg.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fktsv.cn/Article/details/gzriwxqom.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.vehdjk.com/Article/details/geeavaakg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fktsv.cn/Article/details/gcgilauon.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/gydpvyahf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.tarul.cn/Article/details/gogojlyuq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.sjlbkw.cn/Article/details/gidksgxxc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fktsv.cn/Article/details/gohcfbuwq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.epnwcf.com/Article/details/gxpwmxdcf.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.yfazqb.com/Article/details/gmidfbkjr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.tarul.cn/Article/details/gcvnbqrtt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.vehdjk.com/Article/details/gbeznjhuq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/ghnjtwtlw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.bbcook.cn/Article/details/gtsooxfhq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.bbcook.cn/Article/details/gcnygghxh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.bbcook.cn/Article/details/gqsiatvog.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.tarul.cn/Article/details/gybmwkwlb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fktsv.cn/Article/details/gvokdouey.sHtML

[B07] while 循环
来源：http://read.share.fktsv.cn/Article/details/giaqumboh.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fktsv.cn/Article/details/gncbrvnzo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gmvpuaenh.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gmjehymdh.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gidhmvifd.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/ghvdmrsxw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.yfazqb.com/Article/details/grdgpdfqc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.sjlbkw.cn/Article/details/gaufdbshr.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gmxxwzbyz.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.sjlbkw.cn/Article/details/gngakatqh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.epnwcf.com/Article/details/gqlgutald.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.vehdjk.com/Article/details/glkmjicmu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gojmzdisu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gdqcwtmlo.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fktsv.cn/Article/details/gquhbyvxo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.bbcook.cn/Article/details/guxvuiumg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.epnwcf.com/Article/details/gdwlkljbh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gljemdtkd.sHtML

[B09] break 与 continue
来源：http://baike.bbcook.cn/Article/details/gdlfblkrk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.yfazqb.com/Article/details/gtlaitpqk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gyziyqsna.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/glkdoikfc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gizqmhxip.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/geyyjtgnk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.tarul.cn/Article/details/gixhkbiov.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.vehdjk.com/Article/details/gbqnheifs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gpncriawb.sHtML

[B10] 遍历同时拿索引
来源：http://3g.tarul.cn/Article/details/gdtvgfdit.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.vehdjk.com/Article/details/gmuqacwse.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.vehdjk.com/Article/details/ggexqukaa.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/ghyfhnsth.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.sjlbkw.cn/Article/details/gdzjabscy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.bbcook.cn/Article/details/gvuheiyag.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.vehdjk.com/Article/details/gdvvrakwf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.yfazqb.com/Article/details/gfleoxpsx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.yfazqb.com/Article/details/ggrfotvqh.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.bbcook.cn/Article/details/ghmqjyjua.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.vehdjk.com/Article/details/ghypdojgk.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.tarul.cn/Article/details/gczpemcrw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/gvmssavhu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.sjlbkw.cn/Article/details/gwiouunik.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.yfazqb.com/Article/details/gyxjqvais.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fktsv.cn/Article/details/gftkwgmgm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.bbcook.cn/Article/details/gfywvesid.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.sjlbkw.cn/Article/details/gntcatpax.sHtML

[B12] 跳出多层循环
来源：http://blog.bbcook.cn/Article/details/gnsypbhyc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.sjlbkw.cn/Article/details/gmdqablyu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.yfazqb.com/Article/details/gjobiqboa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/ggopyfudx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gdsgdcrpy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gwwrdjoeu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fktsv.cn/Article/details/gevcbthma.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fktsv.cn/Article/details/gupikzvgq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.epnwcf.com/Article/details/guguxvxjt.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.bbcook.cn/Article/details/gyuufbqyo.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.sjlbkw.cn/Article/details/gbrontptg.sHtML

PHP:  is_numeric($x)
来源：http://m.share.epnwcf.com/Article/details/gltehguan.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.yfazqb.com/Article/details/gqejbxlfv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.vehdjk.com/Article/details/gsqaoazzk.sHtML

Java: x instanceof Number
来源：http://www.blog.sjlbkw.cn/Article/details/gljmpveqc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fktsv.cn/Article/details/gpvtmmxam.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fktsv.cn/Article/details/gsubjatij.sHtML

C#:   x is int or double or decimal
来源：http://blog.tarul.cn/Article/details/gpstdjvuq.sHtML

[B14] 判断值是否在集合内
来源：http://blog.tarul.cn/Article/details/gjhpgrmdc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.epnwcf.com/Article/details/gqetfexcu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fktsv.cn/Article/details/gyfcjhngz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.epnwcf.com/Article/details/gjdsokxpv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fktsv.cn/Article/details/gnnhjwpqo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gzkjjrmdc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.vehdjk.com/Article/details/gdnosjewv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.yfazqb.com/Article/details/gljrvyiuf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/ghtqmpllj.sHtML

[B15] 布尔运算与取反
来源：http://wap.bbcook.cn/Article/details/gdzgdzcym.sHtML

Py:   a and b or not c
来源：http://www.m.share.bbcook.cn/Article/details/gwrekwyjv.sHtML

PHP:  $a && $b || !$c
来源：http://blog.epnwcf.com/Article/details/gedujmuwj.sHtML

JS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/glzivtkrb.sHtML

TS:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gygdiwmbd.sHtML

Java: a && b || !c
来源：http://baike.yfazqb.com/Article/details/gclpnqusg.sHtML

Go:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/giabzugru.sHtML

Ruby: a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/glwomghpm.sHtML

C#:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gfdbbyjez.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.sjlbkw.cn/Article/details/gmkbgrzfi.sHtML

Py:   if not data: return
来源：http://mobile.tarul.cn/Article/details/gcwdhvfri.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fktsv.cn/Article/details/gugmvpvum.sHtML

JS:   if (!data) return;
来源：http://read.share.yfazqb.com/Article/details/gzqqdmljz.sHtML

TS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/grtobisov.sHtML

Java: if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/gtprvllau.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqnfoouv.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.vehdjk.com/Article/details/giefsciex.sHtML

C#:   if (data == null) return;
来源：http://www.share.tarul.cn/Article/details/gyfwfvjjz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gipshyqmc.sHtML

C. 函数与作用域
来源：http://wap.sjlbkw.cn/Article/details/guqvlgggl.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbcxjvwro.sHtML

[C01] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gnlfhwvmw.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gzxkadiap.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gvwqsulfz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gjekcqowr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gkhjqprea.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/glfudkafv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.tarul.cn/Article/details/gpqllvquh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.yfazqb.com/Article/details/gsosizlgc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gqagdawle.sHtML

[C02] 默认参数
来源：http://blog.yfazqb.com/Article/details/gjpqmwoql.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.yfazqb.com/Article/details/gpqbcaxvn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.yfazqb.com/Article/details/goqqjnkgy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gmewsuthr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gatzmbrdm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.sjlbkw.cn/Article/details/gjnprknwn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.yfazqb.com/Article/details/gtdsksozv.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.epnwcf.com/Article/details/gqfunajiq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.vehdjk.com/Article/details/gqaubgury.sHtML

[C03] 可变参数
来源：http://m.share.bbcook.cn/Article/details/gbaswnsgi.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.yfazqb.com/Article/details/givrwiqgq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.yfazqb.com/Article/details/gnekyvyqw.sHtML


<!-- 参考信息 -->