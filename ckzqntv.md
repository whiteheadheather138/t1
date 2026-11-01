代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.yfazqb.com/Article/details/giiulqubu.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.yfazqb.com/Article/details/guqxbbfna.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fktsv.cn/Article/details/gtmqvewzq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fktsv.cn/Article/details/gfzmeaxwj.sHtML

Py:   "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gjpbpdfpz.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gdgwprjnx.sHtML

JS:   "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gxkvjrvfe.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/grsttcstg.sHtML

Java: "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gbmbpwwbw.sHtML

Go:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gfnrffwnr.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gyiiatejf.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gjknpczpc.sHtML

[A14] 注释写法
来源：http://mobile.fktsv.cn/Article/details/gthptncss.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.epnwcf.com/Article/details/gpauynars.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gvfrdolcr.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.yfazqb.com/Article/details/ggmxkubqa.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/gqujzjojt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.tarul.cn/Article/details/gbkynsyxa.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.fktsv.cn/Article/details/gfszotkfe.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.vehdjk.com/Article/details/gksawhwie.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/gzlrrvejs.sHtML

[A15] 空值判断与默认值
来源：http://blog.yfazqb.com/Article/details/giorcotlo.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.fktsv.cn/Article/details/ggijchiau.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.bbcook.cn/Article/details/gmxdtkyoe.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.tarul.cn/Article/details/gbfphslqo.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.yfazqb.com/Article/details/gohlslfjm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.sjlbkw.cn/Article/details/gklipcxep.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.epnwcf.com/Article/details/gfkisbtro.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fktsv.cn/Article/details/gctbcbhmz.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.yfazqb.com/Article/details/grumlhppm.sHtML

[A16] 真假值判断规则
来源：http://baike.vehdjk.com/Article/details/gapbcsljw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.fktsv.cn/Article/details/gpwlqslii.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.vehdjk.com/Article/details/gvnbkadfx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.epnwcf.com/Article/details/gnoouqzzg.sHtML

TS:   if (!x) {}
来源：http://read.share.sjlbkw.cn/Article/details/gdypftxjo.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.epnwcf.com/Article/details/gyrmuzvtx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.bbcook.cn/Article/details/gqwpvkzcg.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.epnwcf.com/Article/details/gpimrgupt.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fktsv.cn/Article/details/gsbvslzdb.sHtML

[A17] 位运算
来源：http://www.m.share.yfazqb.com/Article/details/gwaclbysr.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gaxwtfxsm.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fktsv.cn/Article/details/ggdznfwys.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/guwamdfdp.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/grosenizc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gtpuxmwyd.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/goawmaabp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/gvytnmdla.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gnqwidfxq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.vehdjk.com/Article/details/ghzrljuql.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.vehdjk.com/Article/details/gzsvlnfzz.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.vehdjk.com/Article/details/gbvtaukwy.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.vehdjk.com/Article/details/goqkiihaj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.tarul.cn/Article/details/gtqhzybsn.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.epnwcf.com/Article/details/gkueynsnk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.bbcook.cn/Article/details/gwtupexzp.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fktsv.cn/Article/details/gwbnoipar.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.epnwcf.com/Article/details/gcfndvpqm.sHtML

[A19] 交换两个变量
来源：http://read.share.fktsv.cn/Article/details/gshfidvlq.sHtML

Py:   a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/gvxatvhjj.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.fktsv.cn/Article/details/gkpjeiphp.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.bbcook.cn/Article/details/gpmjjelfw.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.vehdjk.com/Article/details/gcvqiiary.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzvvrqft.sHtML

Go:   a, b = b, a
来源：http://3g.bbcook.cn/Article/details/gufrqudsc.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.bbcook.cn/Article/details/gmrutefzr.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.yfazqb.com/Article/details/goknuukgj.sHtML

[A20] 读取标准输入
来源：http://wap.fktsv.cn/Article/details/ggpfatqvy.sHtML

Py:   name = input("请输入：")
来源：http://m.share.tarul.cn/Article/details/gavzgecpg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.sjlbkw.cn/Article/details/gpxampblf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.epnwcf.com/Article/details/gpgwyccic.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.vehdjk.com/Article/details/gqbztqbnn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.sjlbkw.cn/Article/details/gncwpstjf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.vehdjk.com/Article/details/gcytgrsxu.sHtML

Ruby: gets.chomp
来源：http://3g.epnwcf.com/Article/details/gmzsipskh.sHtML

C#:   Console.ReadLine();
来源：http://m.share.epnwcf.com/Article/details/gziefwqno.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.yfazqb.com/Article/details/gnjymciol.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fktsv.cn/Article/details/gjtddrzxj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.bbcook.cn/Article/details/gnpzvjedp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/gzyzgtqmi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/gbgyyfvqi.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.epnwcf.com/Article/details/gkoauqrqi.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/gjjirhrkd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.tarul.cn/Article/details/gvrhaeetv.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.sjlbkw.cn/Article/details/gpnvtuvts.sHtML

[A22] 获取字符串长度
来源：http://m.share.yfazqb.com/Article/details/gglxkascr.sHtML

Py:   len(s)
来源：http://www.blog.fktsv.cn/Article/details/glgqibeva.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.fktsv.cn/Article/details/gsqpqbuwr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.vehdjk.com/Article/details/gvvzmogyz.sHtML

TS:   s.length
来源：http://m.share.vehdjk.com/Article/details/gnwrqphhr.sHtML

Java: s.length()
来源：http://blog.epnwcf.com/Article/details/gjbojwtgf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtoujbzr.sHtML

Ruby: s.length
来源：http://baike.fktsv.cn/Article/details/goxjzvygr.sHtML

C#:   s.Length
来源：http://www.m.share.yfazqb.com/Article/details/gjqfyppwo.sHtML

[A23] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkrdqcik.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.vehdjk.com/Article/details/goudecxnj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.vehdjk.com/Article/details/gryjraggu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.yfazqb.com/Article/details/ggmzzdtpt.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.bbcook.cn/Article/details/gbfhqonhq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.tarul.cn/Article/details/gugxrnfwq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.vehdjk.com/Article/details/gkwuxgxjk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.sjlbkw.cn/Article/details/gnjptniwu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.epnwcf.com/Article/details/gsfuvdqkc.sHtML

[A24] 去除首尾空白
来源：http://www.blog.yfazqb.com/Article/details/gdrewvmpe.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.vehdjk.com/Article/details/gshunvynn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.bbcook.cn/Article/details/gnsawgvik.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fktsv.cn/Article/details/gqrnpmrvf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.tarul.cn/Article/details/gnaktkkmz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.epnwcf.com/Article/details/gyyjsopfj.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fktsv.cn/Article/details/gxyzmqvcg.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.tarul.cn/Article/details/gkarhyzqm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.vehdjk.com/Article/details/gceeqsxpw.sHtML

[A25] 字符串比较
来源：http://m.share.bbcook.cn/Article/details/gcecgimcy.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.epnwcf.com/Article/details/gmsbcqpgw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.bbcook.cn/Article/details/gcdwzkula.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.vehdjk.com/Article/details/gsfhdaylc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.tarul.cn/Article/details/gghazlphm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.bbcook.cn/Article/details/gnslkhhmd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.yfazqb.com/Article/details/gyxhrgzjq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fktsv.cn/Article/details/gbnkwferi.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.bbcook.cn/Article/details/gwwqtmyvl.sHtML

[A26] 类型转换总览
来源：http://www.m.share.yfazqb.com/Article/details/gpqedkadj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fktsv.cn/Article/details/ggtaekvfp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.epnwcf.com/Article/details/gvouzswpb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.epnwcf.com/Article/details/gxzsxxwhx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.bbcook.cn/Article/details/gmdvelzqo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.bbcook.cn/Article/details/gmcnhlzmn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.yfazqb.com/Article/details/gcfrvuavz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.yfazqb.com/Article/details/gasfhmxfc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.bbcook.cn/Article/details/grtilfxxp.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gimfajjhd.sHtML

B. 流程控制
来源：http://www.share.fktsv.cn/Article/details/gvtadpsju.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gjvosuhpi.sHtML

[B01] 条件判断 if / else
来源：http://baike.yfazqb.com/Article/details/gdvrvlvtn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.tarul.cn/Article/details/gsguykewb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.epnwcf.com/Article/details/gabunfxde.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/gmwktyacf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/grlznvnnk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/gvtotwxrl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.sjlbkw.cn/Article/details/gavivgvhn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.sjlbkw.cn/Article/details/gmoftnyrl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gqyynqoyg.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.epnwcf.com/Article/details/gfsaufpre.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.epnwcf.com/Article/details/gveqpmvqc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.yfazqb.com/Article/details/gfzfvjxxr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/gbncpilbz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/giglcdqqa.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/ghcavomvx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.yfazqb.com/Article/details/girrbcako.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.yfazqb.com/Article/details/gikmmlvil.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gbkockpey.sHtML

[B03] switch / match / case
来源：http://www.share.fktsv.cn/Article/details/gynuiucue.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.bbcook.cn/Article/details/gbhfivwvt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gsseftyme.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxhzxlhi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gmbkauogi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/gwbfnwagq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.vehdjk.com/Article/details/gsunahqwz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.bbcook.cn/Article/details/gfrvdkwhb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.tarul.cn/Article/details/gcjikpifn.sHtML

[B04] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/guvicetvj.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.vehdjk.com/Article/details/gaubdplxn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.vehdjk.com/Article/details/gduhwpfku.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/ginjuxoor.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/gmtbbwlbw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fktsv.cn/Article/details/gevofxsgf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.vehdjk.com/Article/details/gsjuaikds.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.vehdjk.com/Article/details/gnnalwaid.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.yfazqb.com/Article/details/gdibuyxgw.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.epnwcf.com/Article/details/gzheiwsdz.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.vehdjk.com/Article/details/goskeahrc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.sjlbkw.cn/Article/details/gobxfsgxd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/gzfxzpofg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/gmyoxhyvp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.yfazqb.com/Article/details/giuvlkenh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.epnwcf.com/Article/details/gchishfip.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.sjlbkw.cn/Article/details/gjihylnsu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fktsv.cn/Article/details/ggrjxcifa.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.sjlbkw.cn/Article/details/gewmtipgr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.epnwcf.com/Article/details/gxxiytmnn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.bbcook.cn/Article/details/guwwxeggt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fktsv.cn/Article/details/gdyuqxcaf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.sjlbkw.cn/Article/details/gmvsejaww.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fktsv.cn/Article/details/gupajnqng.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.sjlbkw.cn/Article/details/geglircbb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.vehdjk.com/Article/details/gzdxeirlg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.tarul.cn/Article/details/glwxguqbc.sHtML

[B07] while 循环
来源：http://www.blog.sjlbkw.cn/Article/details/gfjtqzqkz.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fktsv.cn/Article/details/gwqkcvxeu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.epnwcf.com/Article/details/gspbtqjhc.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gjzutmmed.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gtricqkru.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gemrdhosc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fktsv.cn/Article/details/gmujysblk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.bbcook.cn/Article/details/gsnqwijsd.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gwjqlvnbt.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.sjlbkw.cn/Article/details/gcouhwctk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.bbcook.cn/Article/details/gadinolzz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.yfazqb.com/Article/details/glwyitetz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gggpkfplk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gsleqpkhx.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gyfvcumgv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fktsv.cn/Article/details/galhqfwvp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.bbcook.cn/Article/details/gtiqgnuur.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gowmvhfea.sHtML

[B09] break 与 continue
来源：http://m.share.fktsv.cn/Article/details/ggcfnejug.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.tarul.cn/Article/details/gdajcckop.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gmomjpmaw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gabuqsbca.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gpkgaashs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gefjotulk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.bbcook.cn/Article/details/giwozvmmf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.vehdjk.com/Article/details/gkbyueiro.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/ggytopjrf.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.vehdjk.com/Article/details/gqmpcngjx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.bbcook.cn/Article/details/gppefidms.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fktsv.cn/Article/details/goyqxaqmy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/gjtpljwjt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.tarul.cn/Article/details/gxrytaynn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.tarul.cn/Article/details/getitogct.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.epnwcf.com/Article/details/gcsgqiejq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.bbcook.cn/Article/details/gymncrnvw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.tarul.cn/Article/details/gubrhzaso.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.tarul.cn/Article/details/gpeyytvtq.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.bbcook.cn/Article/details/gbjewuoei.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.bbcook.cn/Article/details/gefbugahw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.yfazqb.com/Article/details/gqurokkdy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/gfamvtgxd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.bbcook.cn/Article/details/glfteragy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.bbcook.cn/Article/details/gzxfhgwgc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.yfazqb.com/Article/details/gmsyetgwv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.yfazqb.com/Article/details/ghvwpxlpt.sHtML

[B12] 跳出多层循环
来源：http://read.share.tarul.cn/Article/details/gggzhlhaw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.yfazqb.com/Article/details/gevoxxuvk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.sjlbkw.cn/Article/details/gbytsnosd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/ggiqdeboc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/gszlavpwm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gdesogsxf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.bbcook.cn/Article/details/gnqivgcbx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.tarul.cn/Article/details/gpmpofcgs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.bbcook.cn/Article/details/gjokmgrvl.sHtML

[B13] 判断是否为数字
来源：http://3g.sjlbkw.cn/Article/details/gtrbscepi.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.epnwcf.com/Article/details/gomuuwagj.sHtML

PHP:  is_numeric($x)
来源：http://read.share.bbcook.cn/Article/details/grbaufwkv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.sjlbkw.cn/Article/details/groaakpbt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.tarul.cn/Article/details/gmudzomdd.sHtML

Java: x instanceof Number
来源：http://www.share.fktsv.cn/Article/details/ggowcexzw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.vehdjk.com/Article/details/gearjafip.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.vehdjk.com/Article/details/gxxramgyj.sHtML

C#:   x is int or double or decimal
来源：http://3g.fktsv.cn/Article/details/gmhgrqpvf.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fktsv.cn/Article/details/ghvquuzyi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.yfazqb.com/Article/details/gkghtxlhb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.bbcook.cn/Article/details/geryzvfon.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.yfazqb.com/Article/details/gjsqnawfh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzkbnyvi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.yfazqb.com/Article/details/glxutwjau.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.sjlbkw.cn/Article/details/gqdstiqge.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gvwkxwzkw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gvoaustbm.sHtML

[B15] 布尔运算与取反
来源：http://www.share.bbcook.cn/Article/details/gqnmsxicb.sHtML

Py:   a and b or not c
来源：http://wap.vehdjk.com/Article/details/gdasgjlkt.sHtML

PHP:  $a && $b || !$c
来源：http://baike.vehdjk.com/Article/details/ghrugnwma.sHtML

JS:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gcpbszwcp.sHtML

TS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gpbawqpjf.sHtML

Java: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gthofqqia.sHtML

Go:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gvmyucmrd.sHtML

Ruby: a && b || !c
来源：http://wap.yfazqb.com/Article/details/gyhfifnzu.sHtML

C#:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gnxwptvgo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.vehdjk.com/Article/details/grsncjsqd.sHtML

Py:   if not data: return
来源：http://www.m.share.fktsv.cn/Article/details/gadxfoqrv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.vehdjk.com/Article/details/gmoshvnom.sHtML

JS:   if (!data) return;
来源：http://www.share.epnwcf.com/Article/details/gegbkfafe.sHtML

TS:   if (!data) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcqlufbc.sHtML

Java: if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gamjtufte.sHtML

Go:   if data == nil { return }
来源：http://m.share.vehdjk.com/Article/details/gvswjkkep.sHtML

Ruby: return if data.nil?
来源：http://read.share.bbcook.cn/Article/details/gunjibqld.sHtML

C#:   if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gyetshgev.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gszbqubgn.sHtML

C. 函数与作用域
来源：http://mobile.epnwcf.com/Article/details/gxdmgraos.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ggrbqxqea.sHtML

[C01] 定义函数
来源：http://wap.vehdjk.com/Article/details/gluchvwur.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.yfazqb.com/Article/details/gbslegqlq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gvtgziydr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gsrqeefhy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gbexggqpt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gddwybtxe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.sjlbkw.cn/Article/details/graiqkely.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.vehdjk.com/Article/details/gmzpvhayl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gzucosuql.sHtML

[C02] 默认参数
来源：http://3g.epnwcf.com/Article/details/gpwwxmjff.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.tarul.cn/Article/details/gxulcmaxw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.vehdjk.com/Article/details/glcuqmnzg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gqspkjjwt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/gmwqtnohb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.sjlbkw.cn/Article/details/ghipalusu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.bbcook.cn/Article/details/gsqulmhih.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.epnwcf.com/Article/details/gtjslknoi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.sjlbkw.cn/Article/details/gxdzrqcyt.sHtML

[C03] 可变参数
来源：http://3g.vehdjk.com/Article/details/gadhhlanr.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.tarul.cn/Article/details/gqftcsrwz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.epnwcf.com/Article/details/gmywcvrhw.sHtML


<!-- 参考信息 -->