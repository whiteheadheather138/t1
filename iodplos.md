代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.sjlbkw.cn/Article/details/ghozupnhf.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/gqnsudkxx.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.bbcook.cn/Article/details/gtaefoebs.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.sjlbkw.cn/Article/details/gbasrgrnb.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.bbcook.cn/Article/details/gvxswtrif.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.tarul.cn/Article/details/gqszagmmi.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.yfazqb.com/Article/details/gjmbzoojp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.tarul.cn/Article/details/gaweibwlf.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.vehdjk.com/Article/details/ghwscoxuh.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.bbcook.cn/Article/details/gpgayhhpa.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.bbcook.cn/Article/details/gsbkrnqju.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.bbcook.cn/Article/details/gvjapayoe.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.sjlbkw.cn/Article/details/gforsyrlt.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gzwevsdyk.sHtML

JS:   "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/govlvoczf.sHtML

TS:   "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gssuzpklf.sHtML

Java: "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gcgdvbldc.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gvpmojpbx.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/gxidkpddo.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gbuwgyeib.sHtML

[A14] 注释写法
来源：http://www.share.tarul.cn/Article/details/geltfcgel.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.yfazqb.com/Article/details/grmohfddr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/gcwufbjkh.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/gprogzmxe.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.tarul.cn/Article/details/gpiwmweii.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.bbcook.cn/Article/details/gdwhlqdgs.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.bbcook.cn/Article/details/gkjwthpvl.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.vehdjk.com/Article/details/gduakjrol.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.epnwcf.com/Article/details/gqztamvik.sHtML

[A15] 空值判断与默认值
来源：http://baike.bbcook.cn/Article/details/gydclmopu.sHtML

Py:   value = data or "默认值"
来源：http://baike.vehdjk.com/Article/details/gdjnxeeib.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/gwvxhrjhk.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.tarul.cn/Article/details/gqbcbsxkw.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fktsv.cn/Article/details/gwhkmitwb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fktsv.cn/Article/details/gzmjllltk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.epnwcf.com/Article/details/gmyzdhdgs.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.vehdjk.com/Article/details/ghewzgpzy.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.vehdjk.com/Article/details/gaunbzlpr.sHtML

[A16] 真假值判断规则
来源：http://wap.bbcook.cn/Article/details/golwzongw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.vehdjk.com/Article/details/gdlynjhec.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.vehdjk.com/Article/details/gjdgsxxoo.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.yfazqb.com/Article/details/gfmrkungv.sHtML

TS:   if (!x) {}
来源：http://wap.fktsv.cn/Article/details/gdkutrita.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.sjlbkw.cn/Article/details/gmgvdjwyf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.fktsv.cn/Article/details/gjgdfsepn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.sjlbkw.cn/Article/details/gsikcqhdo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.sjlbkw.cn/Article/details/grzmwjxlw.sHtML

[A17] 位运算
来源：http://www.m.share.fktsv.cn/Article/details/gsgabcjpv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gwwfmbiwh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/goxbkqgtd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/gapjldwml.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gytkbstxl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gqzgnaxqh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/gmnnzhzve.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/gkkuizyeo.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gjbndtjkr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.yfazqb.com/Article/details/girgpkyfs.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.vehdjk.com/Article/details/ggurhcmia.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.fktsv.cn/Article/details/gnkkciiim.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.yfazqb.com/Article/details/gbkojogqb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.sjlbkw.cn/Article/details/gkavfwssa.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.fktsv.cn/Article/details/gwvngmufk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.yfazqb.com/Article/details/gseenthnc.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.epnwcf.com/Article/details/gnrqnkggx.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.fktsv.cn/Article/details/gpomzcsfl.sHtML

[A19] 交换两个变量
来源：http://mobile.yfazqb.com/Article/details/gsndxhvid.sHtML

Py:   a, b = b, a
来源：http://www.share.bbcook.cn/Article/details/gwglexcds.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.epnwcf.com/Article/details/gzyceisoe.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.yfazqb.com/Article/details/gmeajpggb.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.vehdjk.com/Article/details/gedoklyht.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.vehdjk.com/Article/details/gybdgzbhc.sHtML

Go:   a, b = b, a
来源：http://read.share.tarul.cn/Article/details/gptuwcgcx.sHtML

Ruby: a, b = b, a
来源：http://wap.bbcook.cn/Article/details/gkrrlkmhk.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.bbcook.cn/Article/details/gfegniqwm.sHtML

[A20] 读取标准输入
来源：http://3g.epnwcf.com/Article/details/guycwgzhk.sHtML

Py:   name = input("请输入：")
来源：http://m.share.yfazqb.com/Article/details/gyekqvoer.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fktsv.cn/Article/details/gzhfnomxe.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.fktsv.cn/Article/details/gjafaeyfo.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.sjlbkw.cn/Article/details/glykwafhn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.bbcook.cn/Article/details/ghwsourem.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.sjlbkw.cn/Article/details/ggcejeoae.sHtML

Ruby: gets.chomp
来源：http://baike.vehdjk.com/Article/details/gceubigrq.sHtML

C#:   Console.ReadLine();
来源：http://wap.vehdjk.com/Article/details/gkrfvdaxz.sHtML

[A21] 保留指定小数位输出
来源：http://blog.tarul.cn/Article/details/gsqmbvxkf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.yfazqb.com/Article/details/gtwtitdwe.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.tarul.cn/Article/details/gsmskvktz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gycaohpwi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.vehdjk.com/Article/details/gvmlpqewr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.bbcook.cn/Article/details/gvufitoxc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.tarul.cn/Article/details/gwnecirux.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.fktsv.cn/Article/details/gnyfdsbnb.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.bbcook.cn/Article/details/gdqwqtwpz.sHtML

[A22] 获取字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gzwyekkep.sHtML

Py:   len(s)
来源：http://baike.sjlbkw.cn/Article/details/gkwmyxkzv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.yfazqb.com/Article/details/gbdjgsatb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.sjlbkw.cn/Article/details/gdbtfhotn.sHtML

TS:   s.length
来源：http://blog.sjlbkw.cn/Article/details/gevaveuen.sHtML

Java: s.length()
来源：http://www.share.fktsv.cn/Article/details/gpoveymhc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.epnwcf.com/Article/details/gwayyswkm.sHtML

Ruby: s.length
来源：http://read.share.yfazqb.com/Article/details/grdnubgvp.sHtML

C#:   s.Length
来源：http://read.share.epnwcf.com/Article/details/gxlrgbqwd.sHtML

[A23] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/givwlnqrn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.sjlbkw.cn/Article/details/gxtxftsfl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.bbcook.cn/Article/details/gpnvqyyym.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.epnwcf.com/Article/details/gqpnkyrzn.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gastlufoo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.sjlbkw.cn/Article/details/ggwwzdofe.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.epnwcf.com/Article/details/ghqpjwkkm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.sjlbkw.cn/Article/details/gkoxogisr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.bbcook.cn/Article/details/gfbaqoaft.sHtML

[A24] 去除首尾空白
来源：http://read.share.fktsv.cn/Article/details/glgghpzfn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.yfazqb.com/Article/details/gvhulevqc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.sjlbkw.cn/Article/details/gnozgkfaq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fktsv.cn/Article/details/gwfdvdvli.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gxoonykru.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.epnwcf.com/Article/details/gzkqbfrau.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.tarul.cn/Article/details/gshlnxdwg.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.tarul.cn/Article/details/gtuyefpsq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnoziydus.sHtML

[A25] 字符串比较
来源：http://3g.bbcook.cn/Article/details/gkzwklxsg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.sjlbkw.cn/Article/details/geudetvxi.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fktsv.cn/Article/details/gpwlmdbxo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.vehdjk.com/Article/details/ghowqgbdf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.yfazqb.com/Article/details/guthrqwly.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.tarul.cn/Article/details/ggjiqtnpe.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.yfazqb.com/Article/details/gbmgzmyiw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.vehdjk.com/Article/details/glfvlwlrq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.sjlbkw.cn/Article/details/gzwbabpex.sHtML

[A26] 类型转换总览
来源：http://m.share.tarul.cn/Article/details/gofwxitas.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.vehdjk.com/Article/details/gpcjdpixf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.tarul.cn/Article/details/gjzbaqwym.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fktsv.cn/Article/details/gpuqcgtxy.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.tarul.cn/Article/details/grppehmgl.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.yfazqb.com/Article/details/glvdoatps.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.yfazqb.com/Article/details/gikfwvnis.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.epnwcf.com/Article/details/gxmbqtldg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.yfazqb.com/Article/details/gljjsqaio.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gluovdjni.sHtML

B. 流程控制
来源：http://blog.sjlbkw.cn/Article/details/gghzzyvib.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/grjqjtshu.sHtML

[B01] 条件判断 if / else
来源：http://wap.bbcook.cn/Article/details/gxcrvwamo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.tarul.cn/Article/details/guqozpmpe.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.yfazqb.com/Article/details/gczvpecdr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcvsmemh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/gvihbyyte.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gcmlnwyfy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.bbcook.cn/Article/details/gejetmngc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.epnwcf.com/Article/details/gurtptdvi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gpfucrnhw.sHtML

[B02] 多分支 else if / elif
来源：http://wap.bbcook.cn/Article/details/glzruudhj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.tarul.cn/Article/details/gkvqchtyj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.yfazqb.com/Article/details/gbflossrv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gsfszznir.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/gtwfbmlfv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gmifhdtec.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.bbcook.cn/Article/details/gwjsiatoa.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.sjlbkw.cn/Article/details/ghivytnrc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.sjlbkw.cn/Article/details/grdbyzlmm.sHtML

[B03] switch / match / case
来源：http://mobile.epnwcf.com/Article/details/glzhetgtk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.epnwcf.com/Article/details/gwtbsnygd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gvcczytjj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gbemcvrjl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gbilozgml.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.tarul.cn/Article/details/gccifdpno.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.epnwcf.com/Article/details/gbwzjeqds.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.tarul.cn/Article/details/gkjbgbqwa.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.yfazqb.com/Article/details/ghksmowbb.sHtML

[B04] for 计数循环
来源：http://baike.fktsv.cn/Article/details/gpwjnprtl.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.sjlbkw.cn/Article/details/gjrelppcb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.yfazqb.com/Article/details/ghgfmcudf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.epnwcf.com/Article/details/gpmiaqbjp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gdsvhpfhi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fktsv.cn/Article/details/gaafmtrmu.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.sjlbkw.cn/Article/details/gffnfojzj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.yfazqb.com/Article/details/gioxoisit.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.sjlbkw.cn/Article/details/ggkemjeru.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fktsv.cn/Article/details/gldcexdds.sHtML

Py:   for item in arr: print(item)
来源：http://blog.bbcook.cn/Article/details/gqwerkroh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.bbcook.cn/Article/details/gmocatdwb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.epnwcf.com/Article/details/gpclgnlgi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.tarul.cn/Article/details/gtsbpiaav.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.bbcook.cn/Article/details/ghsyiirud.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.vehdjk.com/Article/details/gqwwnmrvo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.vehdjk.com/Article/details/gxrqvcxcl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.epnwcf.com/Article/details/gjbydnnok.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.yfazqb.com/Article/details/gdflztuak.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.tarul.cn/Article/details/gwuhlcbrm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fktsv.cn/Article/details/gwfgxooys.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fktsv.cn/Article/details/gkowegjwy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/gjesaqjwq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.bbcook.cn/Article/details/gxasiyqzi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.vehdjk.com/Article/details/gzaakmnir.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.tarul.cn/Article/details/gxhojcjlp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.tarul.cn/Article/details/gaioobqvl.sHtML

[B07] while 循环
来源：http://wap.fktsv.cn/Article/details/gpvblfwhp.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.tarul.cn/Article/details/gpkyheafs.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.tarul.cn/Article/details/gbpgbmafk.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/goauzyutg.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/giniutahz.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/ggcnwqcng.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.yfazqb.com/Article/details/gwfzaczba.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.yfazqb.com/Article/details/geyzujjra.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/ggdbtrhyh.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fktsv.cn/Article/details/gsifjfosw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqvktykj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fktsv.cn/Article/details/gwetoolim.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gcoxfkhaw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gqotjgsex.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gytwrvude.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fktsv.cn/Article/details/gntlfzmmk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.yfazqb.com/Article/details/gyvdqwszz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gymfjsmup.sHtML

[B09] break 与 continue
来源：http://mobile.sjlbkw.cn/Article/details/gklepyyea.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.epnwcf.com/Article/details/gdvmvpbie.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gtqrwauxr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gjeybenry.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gjokiwyqw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gjltjhiux.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.epnwcf.com/Article/details/gueuvekeh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.vehdjk.com/Article/details/gmtmzjdlm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gynfkqpso.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fktsv.cn/Article/details/gpzfavnsy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.sjlbkw.cn/Article/details/gfdhvqrhm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.tarul.cn/Article/details/goskrpifz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.bbcook.cn/Article/details/gwrjhjmal.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/gntwwkhhg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.epnwcf.com/Article/details/gshiknxca.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.epnwcf.com/Article/details/gykybgxsg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.epnwcf.com/Article/details/gnpgqqnnl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.yfazqb.com/Article/details/gienzqfna.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.epnwcf.com/Article/details/gjafyclmm.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.yfazqb.com/Article/details/gsnbdggdq.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.bbcook.cn/Article/details/gowlnqbbn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gudytzayg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/gnxtjxdjw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.epnwcf.com/Article/details/gdlltkwqb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.yfazqb.com/Article/details/gqcarzilq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.tarul.cn/Article/details/gbivbcrwn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fktsv.cn/Article/details/ghjbrndgb.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.epnwcf.com/Article/details/gmyjpmyyu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.epnwcf.com/Article/details/gwkttxhzg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.bbcook.cn/Article/details/gzurdlaoj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/gepqipqga.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/gbbfsdtpf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.tarul.cn/Article/details/geykgxiou.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.bbcook.cn/Article/details/gdbvpcsxh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.vehdjk.com/Article/details/gvdqggexm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.yfazqb.com/Article/details/gmzozvkei.sHtML

[B13] 判断是否为数字
来源：http://mobile.epnwcf.com/Article/details/gywqsamhb.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.yfazqb.com/Article/details/giwvrbdah.sHtML

PHP:  is_numeric($x)
来源：http://3g.vehdjk.com/Article/details/gwbfrooxc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.epnwcf.com/Article/details/gjdgmatsk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gywpmcptz.sHtML

Java: x instanceof Number
来源：http://www.m.share.epnwcf.com/Article/details/goumuytuv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.epnwcf.com/Article/details/gaxasqapd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.tarul.cn/Article/details/gedskgqat.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.tarul.cn/Article/details/gvneelkxu.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.sjlbkw.cn/Article/details/gkgxjypch.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.vehdjk.com/Article/details/gjighlzpu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.vehdjk.com/Article/details/ghejfdkkh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/gidlzdgdo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/ghlvmtlxo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gcyvcxazx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fktsv.cn/Article/details/gavrwlnxt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.tarul.cn/Article/details/grvvkkzex.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gwnaxpbpo.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.epnwcf.com/Article/details/gykidqpdr.sHtML

Py:   a and b or not c
来源：http://m.share.bbcook.cn/Article/details/gzdmpjrjk.sHtML

PHP:  $a && $b || !$c
来源：http://3g.vehdjk.com/Article/details/gieqxmzid.sHtML

JS:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gelfovlca.sHtML

TS:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gqgmhqcog.sHtML

Java: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gjzeupshk.sHtML

Go:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gjkekbsei.sHtML

Ruby: a && b || !c
来源：http://m.share.tarul.cn/Article/details/goqatdtod.sHtML

C#:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gniufzojv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.yfazqb.com/Article/details/ggomjxxeg.sHtML

Py:   if not data: return
来源：http://read.share.sjlbkw.cn/Article/details/gqzxrbcrr.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.bbcook.cn/Article/details/gbotubhev.sHtML

JS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/gbvboiuup.sHtML

TS:   if (!data) return;
来源：http://www.m.share.bbcook.cn/Article/details/gzqbcaxqa.sHtML

Java: if (data == null) return;
来源：http://www.blog.vehdjk.com/Article/details/gqqfqhdap.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.tarul.cn/Article/details/guikizpnc.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fktsv.cn/Article/details/gtnhbnufp.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/gcuinhnxq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ggzejbwoy.sHtML

C. 函数与作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gdiqebkvi.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gaaucreda.sHtML

[C01] 定义函数
来源：http://m.share.yfazqb.com/Article/details/gqiwsonke.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gtoyfwrgf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gtfcadjqg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/grgjnzsmz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/ggvpkmhrv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/getgbguzt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.yfazqb.com/Article/details/gcbiwkbfo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.sjlbkw.cn/Article/details/gljxfvfbo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gckqjkkyo.sHtML

[C02] 默认参数
来源：http://www.blog.epnwcf.com/Article/details/gyuudcsye.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.vehdjk.com/Article/details/ghueyftxi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.sjlbkw.cn/Article/details/gymxmzdlg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/glqjhvflq.sHtML


<!-- 参考信息 -->