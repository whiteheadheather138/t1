代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.epnwcf.com/Article/details/gdimkqkeb.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.bbcook.cn/Article/details/gebmbgmgi.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fktsv.cn/Article/details/ghsdddqqi.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.yfazqb.com/Article/details/gbpqnrxtd.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gnypgurvl.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gsvnfoqrt.sHtML

JS:   "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gipucfwah.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gzpuqlbgt.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gihmuaraa.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.bbcook.cn/Article/details/giqwgwpzw.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gpodpbgge.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gzepttcis.sHtML

[A14] 注释写法
来源：http://www.share.sjlbkw.cn/Article/details/geuypdvth.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.epnwcf.com/Article/details/gkqcgubqr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/gkqpjfkph.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fktsv.cn/Article/details/gaeslosea.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.sjlbkw.cn/Article/details/gwpilhfbs.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.bbcook.cn/Article/details/gooneqedi.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fktsv.cn/Article/details/gyurlxxtj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.bbcook.cn/Article/details/grnymhzhl.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/gaiqhshly.sHtML

[A15] 空值判断与默认值
来源：http://read.share.vehdjk.com/Article/details/gmfsmoeyp.sHtML

Py:   value = data or "默认值"
来源：http://wap.epnwcf.com/Article/details/gqkhbtptu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.epnwcf.com/Article/details/gadsuzgbw.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.yfazqb.com/Article/details/gduapazzn.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.vehdjk.com/Article/details/glotkdfhz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.yfazqb.com/Article/details/gianghnpw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.epnwcf.com/Article/details/gpafuggim.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.vehdjk.com/Article/details/gnycsaamc.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.epnwcf.com/Article/details/gsxpxllqw.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.bbcook.cn/Article/details/grxyfkmmb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.epnwcf.com/Article/details/gniromrnb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.yfazqb.com/Article/details/gnoqwztpz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.bbcook.cn/Article/details/gylrbjnyk.sHtML

TS:   if (!x) {}
来源：http://wap.yfazqb.com/Article/details/gxedneweq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fktsv.cn/Article/details/glhtuitez.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.tarul.cn/Article/details/glclblsre.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.bbcook.cn/Article/details/gqdvkhdhm.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gujtpkdcw.sHtML

[A17] 位运算
来源：http://m.share.epnwcf.com/Article/details/gbjaywlan.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gbostnhiq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fktsv.cn/Article/details/gkolulzpy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gnsfguwpc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/geshwlslo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gdwrvidgh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gheicwqps.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fktsv.cn/Article/details/gvdzftpzj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/gmdidcxex.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.sjlbkw.cn/Article/details/gwqgyqhme.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fktsv.cn/Article/details/gbnmuyjix.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.bbcook.cn/Article/details/gdktujaqf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fktsv.cn/Article/details/gsoczuqox.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.bbcook.cn/Article/details/gtiwdmwdz.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.epnwcf.com/Article/details/gyiqrajua.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.tarul.cn/Article/details/gmkplndjy.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.vehdjk.com/Article/details/gbejonfva.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.bbcook.cn/Article/details/grfycinxl.sHtML

[A19] 交换两个变量
来源：http://www.m.share.vehdjk.com/Article/details/gmnudmcmg.sHtML

Py:   a, b = b, a
来源：http://www.m.share.vehdjk.com/Article/details/gpptvlyeh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fktsv.cn/Article/details/gnwyjpwbn.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fktsv.cn/Article/details/gskjxlvqk.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.vehdjk.com/Article/details/gcxfwuiei.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.epnwcf.com/Article/details/ggjlfryvo.sHtML

Go:   a, b = b, a
来源：http://www.blog.tarul.cn/Article/details/gocopqlwb.sHtML

Ruby: a, b = b, a
来源：http://mobile.vehdjk.com/Article/details/grpavsedr.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.vehdjk.com/Article/details/gjtulahuq.sHtML

[A20] 读取标准输入
来源：http://www.blog.vehdjk.com/Article/details/gdxgyiypu.sHtML

Py:   name = input("请输入：")
来源：http://www.share.yfazqb.com/Article/details/gzewunynw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fktsv.cn/Article/details/gkypwqwop.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.vehdjk.com/Article/details/gloykkfng.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.sjlbkw.cn/Article/details/gnfalzcpc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.sjlbkw.cn/Article/details/gdnndrplr.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fktsv.cn/Article/details/gxzhnsmha.sHtML

Ruby: gets.chomp
来源：http://www.share.fktsv.cn/Article/details/gmdgzpfss.sHtML

C#:   Console.ReadLine();
来源：http://3g.yfazqb.com/Article/details/glvvyfjyr.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.yfazqb.com/Article/details/gguzetmmh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.yfazqb.com/Article/details/gbsykxkkn.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/gknujaikv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/gwzlyymsf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.fktsv.cn/Article/details/gnivxyaqh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/gunxgqktd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gwocpgtlg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/gxjqeqcrf.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.epnwcf.com/Article/details/glpzhukql.sHtML

[A22] 获取字符串长度
来源：http://mobile.epnwcf.com/Article/details/gozrkmsyz.sHtML

Py:   len(s)
来源：http://3g.sjlbkw.cn/Article/details/ghjqbeevw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.tarul.cn/Article/details/grhbjbjxo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.epnwcf.com/Article/details/ggsntaown.sHtML

TS:   s.length
来源：http://mobile.tarul.cn/Article/details/gtfewtuyy.sHtML

Java: s.length()
来源：http://mobile.bbcook.cn/Article/details/gmlrnzywi.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.vehdjk.com/Article/details/gzlaiimpo.sHtML

Ruby: s.length
来源：http://m.share.epnwcf.com/Article/details/gsebdzagi.sHtML

C#:   s.Length
来源：http://blog.bbcook.cn/Article/details/gfqgthrqs.sHtML

[A23] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gpdvzabnx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.vehdjk.com/Article/details/gaxcenkrc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.yfazqb.com/Article/details/gapjwwdjs.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fktsv.cn/Article/details/gyzvfdfxu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/gtfczjlsq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/gtccculqt.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.epnwcf.com/Article/details/gneuavufi.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.tarul.cn/Article/details/gtgpvimgk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.yfazqb.com/Article/details/gzsxvzszz.sHtML

[A24] 去除首尾空白
来源：http://www.share.bbcook.cn/Article/details/gylgiazyv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.tarul.cn/Article/details/gotcgeanu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.fktsv.cn/Article/details/gdgbgzwil.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.yfazqb.com/Article/details/gjbphkhrs.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.epnwcf.com/Article/details/gtaexpaxf.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.vehdjk.com/Article/details/gjlxcfusv.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.vehdjk.com/Article/details/gzsurxqob.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.yfazqb.com/Article/details/gkmmgugxh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.epnwcf.com/Article/details/gsnowhkyh.sHtML

[A25] 字符串比较
来源：http://www.blog.epnwcf.com/Article/details/glcpxmbmr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.tarul.cn/Article/details/guxhpoijp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.epnwcf.com/Article/details/gjhpakvst.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.epnwcf.com/Article/details/gfnzfpamo.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/gcfzcipyn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fktsv.cn/Article/details/gvkhtmqke.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.bbcook.cn/Article/details/ghrezchis.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.vehdjk.com/Article/details/gychkvzwf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.bbcook.cn/Article/details/gnhlalxny.sHtML

[A26] 类型转换总览
来源：http://wap.fktsv.cn/Article/details/gtahuawkl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.tarul.cn/Article/details/gyathlowl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.epnwcf.com/Article/details/gvcmuamuu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.tarul.cn/Article/details/gokuejsmf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.sjlbkw.cn/Article/details/gtpmqxhvl.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.bbcook.cn/Article/details/gtuwcifwd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fktsv.cn/Article/details/gwuxtajsl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.epnwcf.com/Article/details/gqaogiwzp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.epnwcf.com/Article/details/gltkqzble.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gelptygpa.sHtML

B. 流程控制
来源：http://3g.sjlbkw.cn/Article/details/gbyjedwzk.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/guxfmsdiu.sHtML

[B01] 条件判断 if / else
来源：http://www.share.yfazqb.com/Article/details/gbbslfdkb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.yfazqb.com/Article/details/gcxnbbuwv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.vehdjk.com/Article/details/gjxuyexvm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gfapmwkfc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gezokfamg.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/grsehfbuf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.sjlbkw.cn/Article/details/gbhbhnkus.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.bbcook.cn/Article/details/gjgixtyex.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/goxhdtxlt.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.bbcook.cn/Article/details/geateaonc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.yfazqb.com/Article/details/glbaosqur.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gncdelltc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/ggndwxmdm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gxpwcpwuo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fktsv.cn/Article/details/gdjkkqwoo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.yfazqb.com/Article/details/gdgdwufbc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.vehdjk.com/Article/details/gfrjjhrmx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.vehdjk.com/Article/details/gdshlnshr.sHtML

[B03] switch / match / case
来源：http://www.m.share.fktsv.cn/Article/details/gmumdqpaf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.bbcook.cn/Article/details/gtrvscjae.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gvfddvtyk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gezihioft.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/grhfpfbyn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/goasysdnb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.epnwcf.com/Article/details/gnivckbtm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.vehdjk.com/Article/details/goezkcizi.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fktsv.cn/Article/details/guktbqszl.sHtML

[B04] for 计数循环
来源：http://blog.bbcook.cn/Article/details/givvvwwgg.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.sjlbkw.cn/Article/details/gqtwsajcl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.epnwcf.com/Article/details/garmwvqtb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.tarul.cn/Article/details/ghjcwibda.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.tarul.cn/Article/details/ggqfpojeb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.yfazqb.com/Article/details/gglixipmp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fktsv.cn/Article/details/gyosvzogn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.tarul.cn/Article/details/ghzzotrdm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.vehdjk.com/Article/details/grudqaztx.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/garloutex.sHtML

Py:   for item in arr: print(item)
来源：http://wap.sjlbkw.cn/Article/details/gaszabozw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.bbcook.cn/Article/details/gsgpntkfn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.tarul.cn/Article/details/gkitgxaok.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.tarul.cn/Article/details/gfjnydqij.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.vehdjk.com/Article/details/gnzsrnrzh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.epnwcf.com/Article/details/gfsdqulyv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.bbcook.cn/Article/details/gwsxymbdi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.sjlbkw.cn/Article/details/grpjcplav.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.bbcook.cn/Article/details/gmyfvqcrh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.sjlbkw.cn/Article/details/gpnvonelv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.tarul.cn/Article/details/gdarfhnhl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.vehdjk.com/Article/details/gxkhpjszn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/gtpkaivgo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.epnwcf.com/Article/details/gesuazjou.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.epnwcf.com/Article/details/gzfvfkmbv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fktsv.cn/Article/details/gmiyntaox.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.tarul.cn/Article/details/gxfajvqfy.sHtML

[B07] while 循环
来源：http://mobile.tarul.cn/Article/details/ghblwcbta.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fktsv.cn/Article/details/gmxeknxxv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.epnwcf.com/Article/details/gfccjgqxo.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/grjryjjao.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gdlgsnfyb.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/gstyebzwb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.epnwcf.com/Article/details/goqnltvlo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fktsv.cn/Article/details/gbezcbbum.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gdlifcmfo.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fktsv.cn/Article/details/gnzvtodup.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.vehdjk.com/Article/details/gctplrpfd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.yfazqb.com/Article/details/gdgqwewsw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gycawwbop.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gtskmeqeu.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gdffygiel.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.epnwcf.com/Article/details/geyvzoczp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.tarul.cn/Article/details/gsdckrkmo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gavxbytgb.sHtML

[B09] break 与 continue
来源：http://blog.tarul.cn/Article/details/gaukremmx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.epnwcf.com/Article/details/gpmfycmge.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/ghidxkfys.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gckmfhynq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gzaoqlksc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gxnbcvmns.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gathwqygq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.tarul.cn/Article/details/gljchzysy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/geksfvbrd.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.vehdjk.com/Article/details/ghpwigzcd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.yfazqb.com/Article/details/gmuvfgsni.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.epnwcf.com/Article/details/gsccrvvjw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/gzggwddxi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.yfazqb.com/Article/details/gpnkhyvsy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.bbcook.cn/Article/details/gfmzxnmke.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fktsv.cn/Article/details/gmcgzpnpc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.yfazqb.com/Article/details/gpxgskopy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.yfazqb.com/Article/details/gbnfrmdks.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fktsv.cn/Article/details/gpykxbycx.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.yfazqb.com/Article/details/gpnpdbndj.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.sjlbkw.cn/Article/details/gnvfotfbr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.vehdjk.com/Article/details/gvqdgxtli.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/glgsfumvm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.vehdjk.com/Article/details/guhsukioo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.sjlbkw.cn/Article/details/gbflsggfq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.sjlbkw.cn/Article/details/gxyyaihho.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.bbcook.cn/Article/details/gxegtkluc.sHtML

[B12] 跳出多层循环
来源：http://www.blog.bbcook.cn/Article/details/gqgcbszbz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.sjlbkw.cn/Article/details/gbeikpfhk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.yfazqb.com/Article/details/gzgxkcrbt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gmewlvxlb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/goytcywnf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/goeqahrzj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.epnwcf.com/Article/details/gpssftdjf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.epnwcf.com/Article/details/gvdjkdips.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.bbcook.cn/Article/details/gaklgkuml.sHtML

[B13] 判断是否为数字
来源：http://www.blog.tarul.cn/Article/details/gsikzfmky.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.bbcook.cn/Article/details/gqafzndro.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fktsv.cn/Article/details/ghczrkiwu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/grieazsjz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fktsv.cn/Article/details/gihyentkt.sHtML

Java: x instanceof Number
来源：http://mobile.epnwcf.com/Article/details/gftoivdea.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.tarul.cn/Article/details/gfkllglxr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.tarul.cn/Article/details/gvidxhwfx.sHtML

C#:   x is int or double or decimal
来源：http://mobile.tarul.cn/Article/details/gwabxrewt.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.epnwcf.com/Article/details/gimantzrn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.sjlbkw.cn/Article/details/giczngqyg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.yfazqb.com/Article/details/gnrqlxhtg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gijbtlgbt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fktsv.cn/Article/details/guqtjacto.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gtslfltnu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.bbcook.cn/Article/details/gmsrojgox.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/guyqupbpr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gwyymwvzg.sHtML

[B15] 布尔运算与取反
来源：http://baike.vehdjk.com/Article/details/gbmrlxuys.sHtML

Py:   a and b or not c
来源：http://www.blog.bbcook.cn/Article/details/ggdgehxbp.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.bbcook.cn/Article/details/gaaxhocwd.sHtML

JS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gtvhvephn.sHtML

TS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/grvrnxjhz.sHtML

Java: a && b || !c
来源：http://blog.epnwcf.com/Article/details/googhwjbh.sHtML

Go:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/guwxgmvqk.sHtML

Ruby: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gbsalzyoh.sHtML

C#:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/glhrnyopq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.vehdjk.com/Article/details/gkdymlvep.sHtML

Py:   if not data: return
来源：http://mobile.epnwcf.com/Article/details/ggtnaxkeq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grmppqrlg.sHtML

JS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gitibulov.sHtML

TS:   if (!data) return;
来源：http://read.share.sjlbkw.cn/Article/details/ghayivhvz.sHtML

Java: if (data == null) return;
来源：http://www.blog.yfazqb.com/Article/details/genihtwlo.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.yfazqb.com/Article/details/gyywphyoy.sHtML

Ruby: return if data.nil?
来源：http://m.share.bbcook.cn/Article/details/gmvcodqbi.sHtML

C#:   if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/gwpothgpw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gabvslroz.sHtML

C. 函数与作用域
来源：http://baike.sjlbkw.cn/Article/details/gujgpynzq.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gqvqklzhe.sHtML

[C01] 定义函数
来源：http://mobile.epnwcf.com/Article/details/gddbkrcuu.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fktsv.cn/Article/details/geczhrfoy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/ggkcxiwyc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gjoaumznu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gppirtlyq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/grwvtidqk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.bbcook.cn/Article/details/gnoixdwch.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.yfazqb.com/Article/details/gjlqditiw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gtlbfhtjn.sHtML

[C02] 默认参数
来源：http://www.share.vehdjk.com/Article/details/gvrpajgcn.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.bbcook.cn/Article/details/gusztdynh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.tarul.cn/Article/details/gdljcwaoe.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/gpnttnyoy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gltdsgjkl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.sjlbkw.cn/Article/details/giiwymjul.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.yfazqb.com/Article/details/golbjqtds.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.yfazqb.com/Article/details/gsamdyufb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.epnwcf.com/Article/details/gtmswfaua.sHtML

[C03] 可变参数
来源：http://www.m.share.epnwcf.com/Article/details/gcivotlea.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fktsv.cn/Article/details/gfaxazwdw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.tarul.cn/Article/details/ggimrofar.sHtML


<!-- 参考信息 -->