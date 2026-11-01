代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.epnwcf.com/Article/details/gkdxbully.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.sjlbkw.cn/Article/details/gullwgcln.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.bbcook.cn/Article/details/gkwwalovv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.epnwcf.com/Article/details/gzycdgxqx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.epnwcf.com/Article/details/gxanznizn.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.vehdjk.com/Article/details/ggbehbonw.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fktsv.cn/Article/details/gbfnvazbf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.bbcook.cn/Article/details/gvklrirjv.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/gvoznmydi.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gqaffhwsl.sHtML

JS:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gasdnhlqg.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gkvcksaau.sHtML

Java: "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/gartcvrpx.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gspbgteye.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gedtffgkq.sHtML

C#:   "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gtuqsmdgu.sHtML

[A14] 注释写法
来源：http://m.share.sjlbkw.cn/Article/details/gkoqsffdk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.epnwcf.com/Article/details/gwiikskot.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/gtyfvccix.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/gfdhfgxpk.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/gqcqklqsk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.vehdjk.com/Article/details/grkwtbhli.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.yfazqb.com/Article/details/gixuohjjd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fktsv.cn/Article/details/gvveyleqo.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gtibfetua.sHtML

[A15] 空值判断与默认值
来源：http://3g.bbcook.cn/Article/details/gieatbmma.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.fktsv.cn/Article/details/gtytwcoba.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/gwpcvwzit.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.vehdjk.com/Article/details/gcrsjhyzm.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqqxapkm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.yfazqb.com/Article/details/gffimngho.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.vehdjk.com/Article/details/gculprnjw.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.bbcook.cn/Article/details/ggsigzjpk.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.vehdjk.com/Article/details/gmltkvmhf.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.vehdjk.com/Article/details/guzcxsppu.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.sjlbkw.cn/Article/details/gryxzuqah.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.bbcook.cn/Article/details/ggreurxrx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.epnwcf.com/Article/details/gjcentgti.sHtML

TS:   if (!x) {}
来源：http://mobile.vehdjk.com/Article/details/grhihjick.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxtblnnv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.yfazqb.com/Article/details/gyplhyvah.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.bbcook.cn/Article/details/gckcxcejq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.yfazqb.com/Article/details/gxpfctqjf.sHtML

[A17] 位运算
来源：http://m.share.sjlbkw.cn/Article/details/gthqvqrbf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/ghmqakrmq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gkatbugog.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gvmyzhyez.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/gfqzknatt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gqjdlwxeq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gdmbktxoi.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gmxmbbodj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gzpbnjeox.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fktsv.cn/Article/details/gikcfktas.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.sjlbkw.cn/Article/details/gewfycpeb.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fktsv.cn/Article/details/gqniuvkoi.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.yfazqb.com/Article/details/gjqcpgcye.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.epnwcf.com/Article/details/gwmdrhtds.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.yfazqb.com/Article/details/gayflgxkf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.epnwcf.com/Article/details/givfbaqkz.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.yfazqb.com/Article/details/gfkueurar.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.yfazqb.com/Article/details/gxylfrwyq.sHtML

[A19] 交换两个变量
来源：http://baike.sjlbkw.cn/Article/details/grmmfezss.sHtML

Py:   a, b = b, a
来源：http://wap.yfazqb.com/Article/details/gtwlbykjx.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.vehdjk.com/Article/details/gslerqkex.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.epnwcf.com/Article/details/genscjqcu.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fktsv.cn/Article/details/gxsfchrzh.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.yfazqb.com/Article/details/gnftajnvj.sHtML

Go:   a, b = b, a
来源：http://www.share.epnwcf.com/Article/details/geqemesgq.sHtML

Ruby: a, b = b, a
来源：http://baike.fktsv.cn/Article/details/gqcqcmfit.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.bbcook.cn/Article/details/gktsuozkv.sHtML

[A20] 读取标准输入
来源：http://read.share.tarul.cn/Article/details/gmnmgfyof.sHtML

Py:   name = input("请输入：")
来源：http://m.share.tarul.cn/Article/details/gugfzfjjs.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.tarul.cn/Article/details/gjevrnvzj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.sjlbkw.cn/Article/details/gahgivdwf.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.tarul.cn/Article/details/gkioniemz.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.yfazqb.com/Article/details/gtmexushb.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.bbcook.cn/Article/details/gcjlslpfg.sHtML

Ruby: gets.chomp
来源：http://www.share.vehdjk.com/Article/details/gdtcupwjk.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.yfazqb.com/Article/details/gdlclngwz.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fktsv.cn/Article/details/gyoeovyep.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.epnwcf.com/Article/details/guasyausd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/ggjvownen.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/ghucumtvr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/ggouweuwo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gdhihuost.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gswagncdk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gtzddayhn.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.sjlbkw.cn/Article/details/gkmnaenlx.sHtML

[A22] 获取字符串长度
来源：http://www.blog.tarul.cn/Article/details/gdkgdmsvo.sHtML

Py:   len(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gnuhtbqcc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.epnwcf.com/Article/details/gmhdzkdtr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.tarul.cn/Article/details/gexkfkdlc.sHtML

TS:   s.length
来源：http://mobile.fktsv.cn/Article/details/gtsgkhnfb.sHtML

Java: s.length()
来源：http://blog.epnwcf.com/Article/details/gkdhikoef.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.yfazqb.com/Article/details/glnzwqewd.sHtML

Ruby: s.length
来源：http://baike.fktsv.cn/Article/details/gnbcazyat.sHtML

C#:   s.Length
来源：http://www.share.bbcook.cn/Article/details/gutanqvos.sHtML

[A23] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gnaiiudmz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.vehdjk.com/Article/details/gtzwzmrkq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fktsv.cn/Article/details/gjhgzbyre.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/gxjlranij.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/gsfktiiqs.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.yfazqb.com/Article/details/gdyfqkrib.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.yfazqb.com/Article/details/gasjrnvxs.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.sjlbkw.cn/Article/details/gaprslrbl.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fktsv.cn/Article/details/gtvmssxzc.sHtML

[A24] 去除首尾空白
来源：http://blog.sjlbkw.cn/Article/details/gkszyortx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.vehdjk.com/Article/details/goyvpdfcj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfvpbrbe.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.epnwcf.com/Article/details/geowxxujo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.bbcook.cn/Article/details/gtaptrsfm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.epnwcf.com/Article/details/gjsojwgxw.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.tarul.cn/Article/details/gazeuolhj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fktsv.cn/Article/details/gnlkfuqij.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.vehdjk.com/Article/details/gyweojueu.sHtML

[A25] 字符串比较
来源：http://www.m.share.vehdjk.com/Article/details/gpgeiplvz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.sjlbkw.cn/Article/details/gztfdmbli.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fktsv.cn/Article/details/gnfvcnrhd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.tarul.cn/Article/details/gobicevec.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/gfxhknpwz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.vehdjk.com/Article/details/gpakwsgob.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.yfazqb.com/Article/details/gugysuuul.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.tarul.cn/Article/details/gysxqlnbm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fktsv.cn/Article/details/gphhululx.sHtML

[A26] 类型转换总览
来源：http://www.share.fktsv.cn/Article/details/ggihgkoiz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.fktsv.cn/Article/details/gbnbznnhy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.sjlbkw.cn/Article/details/gunnuguom.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.yfazqb.com/Article/details/gvvewtbyx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.yfazqb.com/Article/details/gbomfawaf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.vehdjk.com/Article/details/giotpdtsm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.epnwcf.com/Article/details/gpqysvgdh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.epnwcf.com/Article/details/gwgdouxwg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.sjlbkw.cn/Article/details/gloniriqy.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/glraxoxwh.sHtML

B. 流程控制
来源：http://www.m.share.sjlbkw.cn/Article/details/gmduojmnu.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gdemvvzts.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.vehdjk.com/Article/details/gehamuwnv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.sjlbkw.cn/Article/details/gqwhhswjt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.tarul.cn/Article/details/gbaqaqvzr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gqcqqwjfq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/gziatlxfw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gbghhqnbc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.epnwcf.com/Article/details/gkstdkzsn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fktsv.cn/Article/details/gkvszhhvg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gdyxhoqku.sHtML

[B02] 多分支 else if / elif
来源：http://wap.yfazqb.com/Article/details/gubupsrsz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.tarul.cn/Article/details/gjrtfrgcb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.sjlbkw.cn/Article/details/gmolrdujq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/glchtnvtj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/genbzdcqi.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gqwwjjryn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.bbcook.cn/Article/details/gtpboaxmr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.vehdjk.com/Article/details/gunsjnisf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/ghmbwnmnc.sHtML

[B03] switch / match / case
来源：http://m.share.sjlbkw.cn/Article/details/gaxaabexa.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.epnwcf.com/Article/details/gmydzliim.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/guibnahhb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gywrxhtto.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gmahzraqj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gpknvijga.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/gkzxfjpui.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.vehdjk.com/Article/details/gmgobjkal.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.tarul.cn/Article/details/ghxtikfif.sHtML

[B04] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/gupechejq.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.epnwcf.com/Article/details/gzzxmrhms.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.yfazqb.com/Article/details/gibodacij.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gygjemimz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.sjlbkw.cn/Article/details/gjeyrczsy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gajnhbjav.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.tarul.cn/Article/details/golfzlmxr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.sjlbkw.cn/Article/details/gedkiotkh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.epnwcf.com/Article/details/gcyecojwf.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.tarul.cn/Article/details/gulifzwdd.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.tarul.cn/Article/details/gcaykddil.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.yfazqb.com/Article/details/gwdfcmjqx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.epnwcf.com/Article/details/gxxwtaoeh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.sjlbkw.cn/Article/details/gaeqlodfs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.epnwcf.com/Article/details/gqbgwsxnd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.yfazqb.com/Article/details/gxarueuoz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.bbcook.cn/Article/details/gzahfesjf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.vehdjk.com/Article/details/gedeqbhzl.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.tarul.cn/Article/details/gtluihipc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.tarul.cn/Article/details/gzagbpryt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkwjdxrry.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fktsv.cn/Article/details/goilpybws.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.tarul.cn/Article/details/gccefvtnn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fktsv.cn/Article/details/ghqhhgcll.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.vehdjk.com/Article/details/gugbqnikh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.tarul.cn/Article/details/grujcwpeb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.bbcook.cn/Article/details/gcnzdefys.sHtML

[B07] while 循环
来源：http://www.m.share.bbcook.cn/Article/details/gcfqngqsf.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.tarul.cn/Article/details/gutyhmwoz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.yfazqb.com/Article/details/gzsldkqlb.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/goddabmbq.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gsidyfqks.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gyiyqcrmd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.yfazqb.com/Article/details/gnkvpmttv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.vehdjk.com/Article/details/gcckkhika.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gllbjhqib.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.vehdjk.com/Article/details/gxvbeebfy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.bbcook.cn/Article/details/gsrshgsjl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.bbcook.cn/Article/details/gienpodrd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/goinspaeo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gcpeuklkh.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/garbbixzi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fktsv.cn/Article/details/gyjphstap.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.sjlbkw.cn/Article/details/gjnbynylk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gvmrcfdpg.sHtML

[B09] break 与 continue
来源：http://mobile.tarul.cn/Article/details/gcxktbday.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.tarul.cn/Article/details/gnjtecnva.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gtmslrmyp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gblprgxzv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gnfjcjftw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gvupgdcci.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.vehdjk.com/Article/details/glbqhwkry.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.sjlbkw.cn/Article/details/gazylwjrp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gsejjhtkg.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.yfazqb.com/Article/details/gsncljmiy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.yfazqb.com/Article/details/gtemhnrdp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.bbcook.cn/Article/details/geqgodimz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.epnwcf.com/Article/details/gvkjntgab.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.epnwcf.com/Article/details/gvexkeikd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.bbcook.cn/Article/details/gdtdxeavq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.vehdjk.com/Article/details/gwprxrbgq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.epnwcf.com/Article/details/genbaaowt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.tarul.cn/Article/details/gidkokekk.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.tarul.cn/Article/details/gxikjcfcn.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.bbcook.cn/Article/details/gvrsbudtt.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.vehdjk.com/Article/details/gfdqqztnz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.yfazqb.com/Article/details/gjidiohfj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fktsv.cn/Article/details/gwztxurxh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.vehdjk.com/Article/details/gylkhmpuu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.bbcook.cn/Article/details/gmfuitzqa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.bbcook.cn/Article/details/gurzbfnhn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.epnwcf.com/Article/details/guvnfgvvl.sHtML

[B12] 跳出多层循环
来源：http://wap.bbcook.cn/Article/details/gvptgsjae.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.tarul.cn/Article/details/gyeopasav.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.epnwcf.com/Article/details/gjmadipsb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gugmmxvgr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/gtxnuwjgs.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gmbswfaqh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.vehdjk.com/Article/details/giqelzwae.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fktsv.cn/Article/details/gcxxnmkxs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.sjlbkw.cn/Article/details/gdyxyfkgr.sHtML

[B13] 判断是否为数字
来源：http://mobile.yfazqb.com/Article/details/gusczifpr.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.tarul.cn/Article/details/gbiqkqoqs.sHtML

PHP:  is_numeric($x)
来源：http://read.share.sjlbkw.cn/Article/details/gloemndts.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.yfazqb.com/Article/details/gxxjrqgac.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gsnzisjzn.sHtML

Java: x instanceof Number
来源：http://wap.epnwcf.com/Article/details/gqrnixusa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.sjlbkw.cn/Article/details/gurpjnigz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fktsv.cn/Article/details/gwggdgnjr.sHtML

C#:   x is int or double or decimal
来源：http://wap.vehdjk.com/Article/details/gqnteddnv.sHtML

[B14] 判断值是否在集合内
来源：http://baike.bbcook.cn/Article/details/gkrkspmqt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.tarul.cn/Article/details/grouhevbf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.yfazqb.com/Article/details/gdjbicwmw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gtgupiruf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.vehdjk.com/Article/details/gwwdfjnzq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gidyidymc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fktsv.cn/Article/details/gddkmqiqq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.bbcook.cn/Article/details/gkbaxknsp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/ghdlxhmqk.sHtML

[B15] 布尔运算与取反
来源：http://wap.epnwcf.com/Article/details/gnnfmptmr.sHtML

Py:   a and b or not c
来源：http://m.share.fktsv.cn/Article/details/gbowesaac.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.vehdjk.com/Article/details/gbfiecxox.sHtML

JS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrtdraxi.sHtML

TS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gbbriwppw.sHtML

Java: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gtqdtiazj.sHtML

Go:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gxzikwrkb.sHtML

Ruby: a && b || !c
来源：http://3g.yfazqb.com/Article/details/gmrmtpjtt.sHtML

C#:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gdwaqweyt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.bbcook.cn/Article/details/gcldjlpwc.sHtML

Py:   if not data: return
来源：http://3g.yfazqb.com/Article/details/givtyncxw.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.vehdjk.com/Article/details/gcqaizmsp.sHtML

JS:   if (!data) return;
来源：http://blog.epnwcf.com/Article/details/gxatsthcb.sHtML

TS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/gcaykxukn.sHtML

Java: if (data == null) return;
来源：http://read.share.fktsv.cn/Article/details/gwvdqshmp.sHtML

Go:   if data == nil { return }
来源：http://read.share.fktsv.cn/Article/details/gfmmxumoa.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvccptpe.sHtML

C#:   if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/gqtveclei.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gosepfifs.sHtML

C. 函数与作用域
来源：http://3g.tarul.cn/Article/details/gcgmredcq.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gzzedlrxs.sHtML

[C01] 定义函数
来源：http://mobile.fktsv.cn/Article/details/gmlcktnkv.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.sjlbkw.cn/Article/details/gkhookjab.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcypiaadz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gvpyeuivf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gdauuelsv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/ggcjvzhkl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gpmsyjpvi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.yfazqb.com/Article/details/gdpbtkppp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gywmcqykm.sHtML

[C02] 默认参数
来源：http://m.share.bbcook.cn/Article/details/grvlaoysx.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.sjlbkw.cn/Article/details/gjkdstdxy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.tarul.cn/Article/details/gvprvwtcx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/gxnqdqpxv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.tarul.cn/Article/details/gnlxzfefi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.bbcook.cn/Article/details/gpavgixjp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.sjlbkw.cn/Article/details/gpcehjrwj.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.tarul.cn/Article/details/gvqabrqol.sHtML


<!-- 参考信息 -->