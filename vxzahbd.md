代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.vehdjk.com/Article/details/gwtbntbzg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.bbcook.cn/Article/details/gwfkmvqvr.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.epnwcf.com/Article/details/ghthkmmck.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.bbcook.cn/Article/details/ggatfvkxa.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.epnwcf.com/Article/details/gjbccobzx.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.epnwcf.com/Article/details/ggqjiuypc.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.sjlbkw.cn/Article/details/gdfbpxtix.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fktsv.cn/Article/details/gmkqneczm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.sjlbkw.cn/Article/details/guhawtpdl.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.vehdjk.com/Article/details/glzpucfox.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.sjlbkw.cn/Article/details/guupubdqi.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.tarul.cn/Article/details/gyuufulfc.sHtML

Py:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gqnwvdihx.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gkjrqevrc.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gkgpdxxsr.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gupdizdko.sHtML

Java: "第一行\n第二行"
来源：http://m.share.bbcook.cn/Article/details/gopktgokz.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/geoxckked.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/guxlgvruc.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gsmgaahut.sHtML

[A14] 注释写法
来源：http://m.share.sjlbkw.cn/Article/details/gcmuxfflw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.tarul.cn/Article/details/gzdrdsick.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/gxzvanznd.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/gkbriwmqb.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/gmplwcfxx.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.bbcook.cn/Article/details/gtlgmizzu.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/gfahmowlp.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.vehdjk.com/Article/details/gluskzepg.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.sjlbkw.cn/Article/details/gdbeoenqz.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fktsv.cn/Article/details/gmwagtzqb.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.bbcook.cn/Article/details/gznwinadx.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.bbcook.cn/Article/details/grwcwwiix.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.epnwcf.com/Article/details/gbzkfpgaw.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.fktsv.cn/Article/details/gmjntfalz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.epnwcf.com/Article/details/ggnxouijo.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fktsv.cn/Article/details/gcudxogco.sHtML

Ruby: value = data || "默认值"
来源：http://baike.epnwcf.com/Article/details/gspnmbimn.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/ggtpxqmgo.sHtML

[A16] 真假值判断规则
来源：http://blog.fktsv.cn/Article/details/glzbmradv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.sjlbkw.cn/Article/details/gkoqqvmdn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.tarul.cn/Article/details/gmwylqboz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.epnwcf.com/Article/details/ggopcipxk.sHtML

TS:   if (!x) {}
来源：http://m.share.vehdjk.com/Article/details/gbhkfzdrf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.sjlbkw.cn/Article/details/gjdsovccb.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.yfazqb.com/Article/details/gnspiekcp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.sjlbkw.cn/Article/details/ggcxhlyab.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.yfazqb.com/Article/details/grvexstkc.sHtML

[A17] 位运算
来源：http://www.share.yfazqb.com/Article/details/gvxboffdv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/gfsivrbmj.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.bbcook.cn/Article/details/gbdtfynrv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gjotsshdk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gxwwqqekf.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/gawjdjrgu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gqaqeobkm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gssifcsvu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gsmicfgiv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.sjlbkw.cn/Article/details/gdhjrqbju.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.yfazqb.com/Article/details/gbyqzsczh.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.bbcook.cn/Article/details/gslqdfusp.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.yfazqb.com/Article/details/gfyutjlnc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fktsv.cn/Article/details/gcuzgvijs.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.vehdjk.com/Article/details/gzoqtvfsy.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.sjlbkw.cn/Article/details/gvoiuoyne.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.vehdjk.com/Article/details/gbzvfwhdm.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.epnwcf.com/Article/details/gqxyenaot.sHtML

[A19] 交换两个变量
来源：http://read.share.sjlbkw.cn/Article/details/gzyuxutmt.sHtML

Py:   a, b = b, a
来源：http://mobile.bbcook.cn/Article/details/gkglolfsx.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.tarul.cn/Article/details/gssbsxpal.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.vehdjk.com/Article/details/gxxvufpff.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.sjlbkw.cn/Article/details/giljcqumq.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.bbcook.cn/Article/details/gjpfkkgze.sHtML

Go:   a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/gvbbchpkv.sHtML

Ruby: a, b = b, a
来源：http://blog.vehdjk.com/Article/details/gyvwaamkh.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.epnwcf.com/Article/details/gyrtbtaqf.sHtML

[A20] 读取标准输入
来源：http://wap.bbcook.cn/Article/details/gdcnwkbym.sHtML

Py:   name = input("请输入：")
来源：http://mobile.epnwcf.com/Article/details/gedaedrty.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.sjlbkw.cn/Article/details/gfidkrtcq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.bbcook.cn/Article/details/gsxawlqhv.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.vehdjk.com/Article/details/gegcgbkrw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.yfazqb.com/Article/details/gnmfuwuty.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.yfazqb.com/Article/details/ghloicdfu.sHtML

Ruby: gets.chomp
来源：http://read.share.yfazqb.com/Article/details/gragnqpgq.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fktsv.cn/Article/details/ghufedivn.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.epnwcf.com/Article/details/gcfcezcbw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.bbcook.cn/Article/details/gopdpwbop.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/goodmxmge.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/gbickzyau.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fktsv.cn/Article/details/gbchpiuoe.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.yfazqb.com/Article/details/gciqniqqu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.vehdjk.com/Article/details/gpxcsntgi.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.sjlbkw.cn/Article/details/gscjdfjug.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.vehdjk.com/Article/details/ggqurxmsz.sHtML

[A22] 获取字符串长度
来源：http://read.share.epnwcf.com/Article/details/gurqkfaio.sHtML

Py:   len(s)
来源：http://blog.epnwcf.com/Article/details/gxofoltlc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.vehdjk.com/Article/details/gwustcxiu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.bbcook.cn/Article/details/gbdqsfphr.sHtML

TS:   s.length
来源：http://blog.tarul.cn/Article/details/gsoccjrwq.sHtML

Java: s.length()
来源：http://www.m.share.tarul.cn/Article/details/gadwsuyye.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.epnwcf.com/Article/details/gkgicxhrc.sHtML

Ruby: s.length
来源：http://m.share.fktsv.cn/Article/details/gifsmvtby.sHtML

C#:   s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gaoseevqe.sHtML

[A23] 大小写转换
来源：http://m.share.tarul.cn/Article/details/gfhqppkhd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.bbcook.cn/Article/details/gfoiihvth.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.tarul.cn/Article/details/gjlrjfsfq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.yfazqb.com/Article/details/gjrcitcyo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.bbcook.cn/Article/details/ghwkhxsct.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.bbcook.cn/Article/details/galgnglix.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.tarul.cn/Article/details/gdqypadyp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.yfazqb.com/Article/details/gxhirgsvg.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.bbcook.cn/Article/details/gfdrosbzt.sHtML

[A24] 去除首尾空白
来源：http://wap.tarul.cn/Article/details/ggohkloce.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.sjlbkw.cn/Article/details/gvdlfqjxb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.bbcook.cn/Article/details/glkvwiuxt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.tarul.cn/Article/details/gcftcudxc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsmcuzvu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.vehdjk.com/Article/details/ghnhrtgpi.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fktsv.cn/Article/details/gvngdbhlu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.bbcook.cn/Article/details/govziwqck.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.vehdjk.com/Article/details/gjhhksnkd.sHtML

[A25] 字符串比较
来源：http://wap.tarul.cn/Article/details/gnzcfyekx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.vehdjk.com/Article/details/gpfxdfbkc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.vehdjk.com/Article/details/gnxjwjwtk.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fktsv.cn/Article/details/gaknflkmf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.vehdjk.com/Article/details/gtnkxohyb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.bbcook.cn/Article/details/gwrbxotnm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.sjlbkw.cn/Article/details/gieelzpdh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.yfazqb.com/Article/details/gizkgobdz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.tarul.cn/Article/details/gtegqxcli.sHtML

[A26] 类型转换总览
来源：http://m.share.sjlbkw.cn/Article/details/gwwylhucg.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.bbcook.cn/Article/details/gvcjmpdgj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fktsv.cn/Article/details/grgoueqtq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.yfazqb.com/Article/details/gyvcfhfph.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.sjlbkw.cn/Article/details/grezmoofv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.yfazqb.com/Article/details/gbwkpsodj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.sjlbkw.cn/Article/details/gyaswvmef.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.tarul.cn/Article/details/gvydvtsnc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fktsv.cn/Article/details/ghisrcnsd.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gonliumzo.sHtML

B. 流程控制
来源：http://m.share.tarul.cn/Article/details/gzjvynkxj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gskimtifj.sHtML

[B01] 条件判断 if / else
来源：http://m.share.bbcook.cn/Article/details/gdiyekosk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.bbcook.cn/Article/details/grfmfntnr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.sjlbkw.cn/Article/details/giomfxild.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gqgdatqoh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/gjcjaajuq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gfxcdefpn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fktsv.cn/Article/details/gxcxsxwwk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fktsv.cn/Article/details/galuomeeq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/gmdfzlvas.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.yfazqb.com/Article/details/gcehekkqe.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.epnwcf.com/Article/details/gdtqqmebs.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.vehdjk.com/Article/details/gtljbyptz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gycmwwjqu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gugogwqzm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gzuljbkgb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.epnwcf.com/Article/details/gwybhymxr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.yfazqb.com/Article/details/gwcnzrnzn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/gddeiekxv.sHtML

[B03] switch / match / case
来源：http://www.blog.epnwcf.com/Article/details/gdwrqnsri.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.tarul.cn/Article/details/gjjxhrcio.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/gwzfhldzw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gvlcyhlij.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/ghoadarnb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gmxhnhjpb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.bbcook.cn/Article/details/gbczyfjut.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.tarul.cn/Article/details/gherrspjz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.epnwcf.com/Article/details/grgrewxiv.sHtML

[B04] for 计数循环
来源：http://www.m.share.fktsv.cn/Article/details/guiafdlml.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fktsv.cn/Article/details/gwpulwgoc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.sjlbkw.cn/Article/details/gdlfxtwit.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.bbcook.cn/Article/details/gxvpblxcr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.yfazqb.com/Article/details/grmsnazcv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.epnwcf.com/Article/details/gjcmpekua.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.bbcook.cn/Article/details/gjvpaklmw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.bbcook.cn/Article/details/glwjzkxcv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gesxwpiob.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gxekbgrzi.sHtML

Py:   for item in arr: print(item)
来源：http://baike.epnwcf.com/Article/details/gxicpvyfk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.epnwcf.com/Article/details/gtzmcnbxz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.tarul.cn/Article/details/gzbhlynnf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.yfazqb.com/Article/details/gnfcecgfi.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.bbcook.cn/Article/details/goalvqxmw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fktsv.cn/Article/details/glrdomegk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.tarul.cn/Article/details/galqliqmn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.yfazqb.com/Article/details/grgdbgman.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.vehdjk.com/Article/details/gwhpyznrh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fktsv.cn/Article/details/ghbxgpggg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.sjlbkw.cn/Article/details/gbddkvgxb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.tarul.cn/Article/details/gpegryqpz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/gfqhmasty.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.epnwcf.com/Article/details/gtjynqpkg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.tarul.cn/Article/details/gvzbqfepv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fktsv.cn/Article/details/gbjgqykpr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.vehdjk.com/Article/details/gnjasqvpu.sHtML

[B07] while 循环
来源：http://blog.yfazqb.com/Article/details/grfzppfwb.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/golxtpyib.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.vehdjk.com/Article/details/ghctjeppo.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gitiqjrnx.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gwqxrzavy.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gqcvnpdmn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.tarul.cn/Article/details/gwdolcgcj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fktsv.cn/Article/details/geeywieud.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gpulbxlhf.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.sjlbkw.cn/Article/details/gystkvjbo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.vehdjk.com/Article/details/gzarkjlff.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.vehdjk.com/Article/details/gipwbvbha.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gzpwtfuvz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gdtxakied.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gnezemjnj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fktsv.cn/Article/details/gvyqzudxx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.bbcook.cn/Article/details/gajmffzvw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/gartmyqsw.sHtML

[B09] break 与 continue
来源：http://m.share.sjlbkw.cn/Article/details/gjspcfsxu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.tarul.cn/Article/details/gafdugbpa.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gfctwijtw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gsxntnryi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gjptrocej.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/grkigtlgn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.bbcook.cn/Article/details/gjuaiprff.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.tarul.cn/Article/details/ggveympka.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gsurumcfy.sHtML

[B10] 遍历同时拿索引
来源：http://baike.bbcook.cn/Article/details/gfjeuicnp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.yfazqb.com/Article/details/gnnfsdqwg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.bbcook.cn/Article/details/gphlyywqr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fktsv.cn/Article/details/gdfgqcxiq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.yfazqb.com/Article/details/gjnnkokol.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.tarul.cn/Article/details/ghnkixomh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.tarul.cn/Article/details/gpzizkmig.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.vehdjk.com/Article/details/gyrysdxis.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.vehdjk.com/Article/details/gvboekfci.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.bbcook.cn/Article/details/gamuloqli.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.yfazqb.com/Article/details/gjkjtpoot.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.epnwcf.com/Article/details/ggjqsiqln.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.vehdjk.com/Article/details/gxhcjryui.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/grjspdxab.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.yfazqb.com/Article/details/gwhlnkwjz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fktsv.cn/Article/details/gplspqmjn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.yfazqb.com/Article/details/gypbdsdkn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.epnwcf.com/Article/details/gtlccafut.sHtML

[B12] 跳出多层循环
来源：http://read.share.bbcook.cn/Article/details/gqgayfxzq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.bbcook.cn/Article/details/gyxfvfnkc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.vehdjk.com/Article/details/gtfrialfi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/goisdusyq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/gywbzowmc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/gtvzacobi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.tarul.cn/Article/details/grodkznby.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fktsv.cn/Article/details/gojlowbpr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.yfazqb.com/Article/details/gvjakjfjw.sHtML

[B13] 判断是否为数字
来源：http://www.share.bbcook.cn/Article/details/gqbxmtitd.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.epnwcf.com/Article/details/gyncihjbk.sHtML

PHP:  is_numeric($x)
来源：http://www.share.sjlbkw.cn/Article/details/gktjxmyzy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/gyojhdiyy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.vehdjk.com/Article/details/ghnhoagqn.sHtML

Java: x instanceof Number
来源：http://read.share.sjlbkw.cn/Article/details/gcpjouimy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.sjlbkw.cn/Article/details/gxscbeuoh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.sjlbkw.cn/Article/details/gamwooxbj.sHtML

C#:   x is int or double or decimal
来源：http://baike.bbcook.cn/Article/details/ggxecxcnc.sHtML

[B14] 判断值是否在集合内
来源：http://blog.tarul.cn/Article/details/gvjoaflsm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fktsv.cn/Article/details/gnwhkbvqc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.bbcook.cn/Article/details/gptywqsrx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gocmehsth.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.epnwcf.com/Article/details/gqgxwatdd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/ggloeucxy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.tarul.cn/Article/details/gesaupdxf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.bbcook.cn/Article/details/gqukhieno.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.yfazqb.com/Article/details/gqirplrld.sHtML

[B15] 布尔运算与取反
来源：http://3g.epnwcf.com/Article/details/gifheptca.sHtML

Py:   a and b or not c
来源：http://www.m.share.sjlbkw.cn/Article/details/glljmsisd.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fktsv.cn/Article/details/gnvzoakey.sHtML

JS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gsgpopdxz.sHtML

TS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/glouvzcor.sHtML

Java: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gpjuwejws.sHtML

Go:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gshqxlofx.sHtML

Ruby: a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gcegdrmyp.sHtML

C#:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gmekxrzcd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.epnwcf.com/Article/details/gymydggpr.sHtML

Py:   if not data: return
来源：http://3g.tarul.cn/Article/details/gfglcmjcs.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.bbcook.cn/Article/details/gsvricqig.sHtML

JS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/gapldbkzr.sHtML

TS:   if (!data) return;
来源：http://blog.yfazqb.com/Article/details/gvxvrghex.sHtML

Java: if (data == null) return;
来源：http://read.share.yfazqb.com/Article/details/gjzbyxnem.sHtML

Go:   if data == nil { return }
来源：http://m.share.epnwcf.com/Article/details/gcpqkwrfi.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.yfazqb.com/Article/details/gpyevxkya.sHtML

C#:   if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gnvvxvccp.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gemqqlvxd.sHtML

C. 函数与作用域
来源：http://mobile.vehdjk.com/Article/details/gyepzzoib.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ggdyykecw.sHtML

[C01] 定义函数
来源：http://m.share.yfazqb.com/Article/details/gmnpuxekk.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.vehdjk.com/Article/details/gbjzxgejd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/gcxtusiwr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gghtcxdhc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gfynzmdzv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gwvkrjjwp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gewdymmud.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.sjlbkw.cn/Article/details/ghjbhuxlw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/guskedqha.sHtML

[C02] 默认参数
来源：http://blog.tarul.cn/Article/details/gjmmhsrut.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.epnwcf.com/Article/details/gdosvbfpl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.epnwcf.com/Article/details/gzjvyglri.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/gzpclvuuv.sHtML


<!-- 参考信息 -->