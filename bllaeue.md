代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.bbcook.cn/Article/details/gcefilasi.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/govyqddnr.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fktsv.cn/Article/details/gidhadsaq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.epnwcf.com/Article/details/ghonskmvi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.bbcook.cn/Article/details/gpybesdfv.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.yfazqb.com/Article/details/gqusadkdg.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.sjlbkw.cn/Article/details/gtbbfputz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.sjlbkw.cn/Article/details/gtbjtunoz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.vehdjk.com/Article/details/gnpodgalv.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.yfazqb.com/Article/details/gpxxvfobz.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.epnwcf.com/Article/details/ggslbsnvu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fktsv.cn/Article/details/gxowdxzdb.sHtML

Py:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gxyueittl.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gsjrgbvcv.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/ggwlwrltf.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gqwwaxeng.sHtML

Java: "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gyfkkuigg.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gdnxsjumk.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/gupquihhz.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/gzmioynwe.sHtML

[A14] 注释写法
来源：http://mobile.epnwcf.com/Article/details/gqdfhbazh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.bbcook.cn/Article/details/gnqwayaom.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gnkpsycms.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.yfazqb.com/Article/details/gajkhfdrr.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/gmbvtunfv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.vehdjk.com/Article/details/gtehcleql.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.epnwcf.com/Article/details/gxsxfveya.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.yfazqb.com/Article/details/gczhzgbgj.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.bbcook.cn/Article/details/gywprdinr.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.vehdjk.com/Article/details/ggplggwvd.sHtML

Py:   value = data or "默认值"
来源：http://mobile.fktsv.cn/Article/details/gvlewpphv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fktsv.cn/Article/details/gbpyhgiwb.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fktsv.cn/Article/details/gmfxbvhql.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.epnwcf.com/Article/details/gqrzfvzwd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.fktsv.cn/Article/details/gmbowrcoz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.yfazqb.com/Article/details/gmuwsqujx.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fktsv.cn/Article/details/ghygkjidl.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.sjlbkw.cn/Article/details/gkxepzgrc.sHtML

[A16] 真假值判断规则
来源：http://mobile.fktsv.cn/Article/details/gzrofzwke.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.epnwcf.com/Article/details/guogbhoow.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.tarul.cn/Article/details/gdxpshpow.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.tarul.cn/Article/details/gwzreqfua.sHtML

TS:   if (!x) {}
来源：http://m.share.vehdjk.com/Article/details/gjuzmyyog.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.epnwcf.com/Article/details/gwyxbsibz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.yfazqb.com/Article/details/ghrbjqfdc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.yfazqb.com/Article/details/gpsuuhwvh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.vehdjk.com/Article/details/gfzlemkme.sHtML

[A17] 位运算
来源：http://www.blog.epnwcf.com/Article/details/gwbfypzqw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gdtmwzznu.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gcjbgnvwv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gbjacyagn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/ggcmemcwy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/gyflffeso.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gbtyzxrbz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gryuckvrk.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gaegoppgi.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.sjlbkw.cn/Article/details/gqzupgauz.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.fktsv.cn/Article/details/gbtvmqdos.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.sjlbkw.cn/Article/details/ggehjavyy.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.epnwcf.com/Article/details/gxhdjfoix.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.epnwcf.com/Article/details/gqkjkmrhy.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.fktsv.cn/Article/details/gtuvduwjv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.epnwcf.com/Article/details/gjhbphynd.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.tarul.cn/Article/details/gizpdsety.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.yfazqb.com/Article/details/gqmimnwmr.sHtML

[A19] 交换两个变量
来源：http://wap.vehdjk.com/Article/details/giaiuzjva.sHtML

Py:   a, b = b, a
来源：http://wap.epnwcf.com/Article/details/gcddanvsg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.tarul.cn/Article/details/gcefkxcwd.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.yfazqb.com/Article/details/gmxlpwgfi.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.epnwcf.com/Article/details/gccttvnmn.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.fktsv.cn/Article/details/gumzjoszu.sHtML

Go:   a, b = b, a
来源：http://blog.vehdjk.com/Article/details/gaaemizwd.sHtML

Ruby: a, b = b, a
来源：http://baike.bbcook.cn/Article/details/gqbdmdxkz.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.tarul.cn/Article/details/gnvaydhgl.sHtML

[A20] 读取标准输入
来源：http://www.m.share.fktsv.cn/Article/details/gzuzbotly.sHtML

Py:   name = input("请输入：")
来源：http://3g.tarul.cn/Article/details/gpotrwjpt.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.tarul.cn/Article/details/gfapfwwfo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.bbcook.cn/Article/details/gwlqwcjaw.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.vehdjk.com/Article/details/gvdpykmvp.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.yfazqb.com/Article/details/goknppcdx.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.fktsv.cn/Article/details/gwqmydbxv.sHtML

Ruby: gets.chomp
来源：http://blog.epnwcf.com/Article/details/gnsfnlpoj.sHtML

C#:   Console.ReadLine();
来源：http://baike.bbcook.cn/Article/details/ggjsxdbso.sHtML

[A21] 保留指定小数位输出
来源：http://baike.yfazqb.com/Article/details/gmczbmimf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.sjlbkw.cn/Article/details/gmoimwpth.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gpzxvycbh.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.tarul.cn/Article/details/glrgdopec.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gvvvdjygm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.bbcook.cn/Article/details/gjfqkqoty.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.yfazqb.com/Article/details/gykrazylr.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.vehdjk.com/Article/details/gmmwemvau.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzkqppsv.sHtML

[A22] 获取字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gljmgftuh.sHtML

Py:   len(s)
来源：http://www.m.share.tarul.cn/Article/details/gzjutxbyj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.bbcook.cn/Article/details/gpjezqnhu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.tarul.cn/Article/details/glklodlpv.sHtML

TS:   s.length
来源：http://baike.sjlbkw.cn/Article/details/gexglylup.sHtML

Java: s.length()
来源：http://blog.bbcook.cn/Article/details/gqkpyqthy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.epnwcf.com/Article/details/gvzkmgbrp.sHtML

Ruby: s.length
来源：http://wap.sjlbkw.cn/Article/details/ggtuyywux.sHtML

C#:   s.Length
来源：http://www.m.share.yfazqb.com/Article/details/gxzpdtryr.sHtML

[A23] 大小写转换
来源：http://wap.bbcook.cn/Article/details/gkrxjkrrk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.tarul.cn/Article/details/gcayiicso.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.yfazqb.com/Article/details/giygujbmt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fktsv.cn/Article/details/gxpkifcnt.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.yfazqb.com/Article/details/gcfjwwreh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/gkzyvfwhh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.yfazqb.com/Article/details/gkiiwzqry.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.sjlbkw.cn/Article/details/gnanuievg.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.sjlbkw.cn/Article/details/gybehgdbg.sHtML

[A24] 去除首尾空白
来源：http://wap.yfazqb.com/Article/details/gguckqsdz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.yfazqb.com/Article/details/gyperaaox.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.vehdjk.com/Article/details/gxhexgsvg.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.bbcook.cn/Article/details/gjaigdfbh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.epnwcf.com/Article/details/gomqovtab.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.sjlbkw.cn/Article/details/gkcvuccxy.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.sjlbkw.cn/Article/details/gsuaxenzp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fktsv.cn/Article/details/galntfnbb.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.tarul.cn/Article/details/gijaxifzh.sHtML

[A25] 字符串比较
来源：http://blog.bbcook.cn/Article/details/ghcqjutlb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.bbcook.cn/Article/details/gvvrhyxyh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.tarul.cn/Article/details/guyksuhdc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.sjlbkw.cn/Article/details/gdrbvnzuv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.sjlbkw.cn/Article/details/gplvrbtty.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.sjlbkw.cn/Article/details/gvudcrqkn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.yfazqb.com/Article/details/goyaaofar.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.vehdjk.com/Article/details/gyaenrtgx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.epnwcf.com/Article/details/glxtwqwnl.sHtML

[A26] 类型转换总览
来源：http://blog.vehdjk.com/Article/details/gslhjnnck.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.yfazqb.com/Article/details/gwejfmjgb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.vehdjk.com/Article/details/gwfdvirtv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.vehdjk.com/Article/details/glutshelf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.yfazqb.com/Article/details/gttfqdnkx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.bbcook.cn/Article/details/gfychegep.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.vehdjk.com/Article/details/gstfcigkb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.tarul.cn/Article/details/gdsvwvmic.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fktsv.cn/Article/details/gbgiiesyy.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkqichkum.sHtML

B. 流程控制
来源：http://3g.vehdjk.com/Article/details/gpqqobpmg.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gddwefrpy.sHtML

[B01] 条件判断 if / else
来源：http://wap.sjlbkw.cn/Article/details/giuoxhydh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gccdqjoqe.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.bbcook.cn/Article/details/gotflraln.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/galxdgciu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gepmceedm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/giqkmlcdj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxsvowvk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.tarul.cn/Article/details/gsejnszjv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/gplnvfyrh.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fktsv.cn/Article/details/gwfqvexyx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.vehdjk.com/Article/details/gwsoodstk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.tarul.cn/Article/details/gmgejgqtn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gtrktdaqz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gzcowghmc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gefhsnrqa.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.tarul.cn/Article/details/gvjpsekrc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.epnwcf.com/Article/details/goubzmwtj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fktsv.cn/Article/details/ggipguhvx.sHtML

[B03] switch / match / case
来源：http://mobile.fktsv.cn/Article/details/gendgcvoc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.sjlbkw.cn/Article/details/glagfpnoa.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gfqzsaabd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gbwjdfdid.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gwwtqgief.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gxuxkojei.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.bbcook.cn/Article/details/gcgekxkdy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.tarul.cn/Article/details/gnqsnblpp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.yfazqb.com/Article/details/gdwwhtoci.sHtML

[B04] for 计数循环
来源：http://www.share.sjlbkw.cn/Article/details/gvtlxzmfa.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.epnwcf.com/Article/details/guyocvaaa.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.vehdjk.com/Article/details/gjfayeajr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.bbcook.cn/Article/details/gzuohwjrk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdidfgwr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.yfazqb.com/Article/details/geynfhiav.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.vehdjk.com/Article/details/gmcedayyn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.epnwcf.com/Article/details/gnvgmwbwk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fktsv.cn/Article/details/gyuuregay.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.bbcook.cn/Article/details/gsjwccybb.sHtML

Py:   for item in arr: print(item)
来源：http://3g.yfazqb.com/Article/details/gitgnabcy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fktsv.cn/Article/details/gugqvtwoq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.bbcook.cn/Article/details/gbekwnkhu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/gwaqkhctb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.sjlbkw.cn/Article/details/gseghbyog.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fktsv.cn/Article/details/grzjrenkw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.vehdjk.com/Article/details/gacoznczg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gqnuxbzgh.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.epnwcf.com/Article/details/gpjlneetd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fktsv.cn/Article/details/gbetuzqtf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gieirggjj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/gfwuzcqme.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.epnwcf.com/Article/details/gsekcdion.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fktsv.cn/Article/details/gldvtmhxb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.bbcook.cn/Article/details/gvwvehuys.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.tarul.cn/Article/details/gusnugrzd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.tarul.cn/Article/details/glgqovdja.sHtML

[B07] while 循环
来源：http://wap.tarul.cn/Article/details/gjesguqcd.sHtML

Py:   while i < 10: i += 1
来源：http://blog.epnwcf.com/Article/details/gesfjmfwl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fktsv.cn/Article/details/gfhuestiv.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gbedswrpc.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gcnesadgt.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gopdqreci.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.sjlbkw.cn/Article/details/gztfxrtiv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.yfazqb.com/Article/details/gbtaeezyt.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gdtjolutm.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.yfazqb.com/Article/details/gslvpwivr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fktsv.cn/Article/details/geslfjwid.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gvkitsphk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gmzxycina.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gcsvgitso.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gkulxtngd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.tarul.cn/Article/details/gqywgllpv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.tarul.cn/Article/details/gnyxrflgb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gjyggsqlp.sHtML

[B09] break 与 continue
来源：http://wap.fktsv.cn/Article/details/gavsysiyp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.vehdjk.com/Article/details/gijhufqgh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gligfodgj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gbaglgiih.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gmnaygtav.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gttgpmjhj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.tarul.cn/Article/details/ggfmhympa.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.vehdjk.com/Article/details/glcxvvwph.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gesqslohv.sHtML

[B10] 遍历同时拿索引
来源：http://3g.vehdjk.com/Article/details/gwhqmoauh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.vehdjk.com/Article/details/gvnjxejri.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.sjlbkw.cn/Article/details/gycrnrass.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.tarul.cn/Article/details/gmjmxndjc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.yfazqb.com/Article/details/gskkrkrox.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.sjlbkw.cn/Article/details/gsakleuae.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.vehdjk.com/Article/details/gxkwgjytw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fktsv.cn/Article/details/gjwlfvytq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.bbcook.cn/Article/details/glhpaztmt.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwxcntwh.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.bbcook.cn/Article/details/gamvluwyu.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.vehdjk.com/Article/details/gogzacuzt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.tarul.cn/Article/details/gvfqzjinz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fktsv.cn/Article/details/gbsjmtzcn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.epnwcf.com/Article/details/gogulxcgj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fktsv.cn/Article/details/glhdtehll.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.bbcook.cn/Article/details/gojvgfday.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.epnwcf.com/Article/details/gactbfnor.sHtML

[B12] 跳出多层循环
来源：http://www.blog.sjlbkw.cn/Article/details/gyksnvsas.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.sjlbkw.cn/Article/details/gsqxvmnsr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.vehdjk.com/Article/details/gcxkklmvt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/gbrqlsffy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gncxaymmv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gxqllamis.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.sjlbkw.cn/Article/details/gqpdselfg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.vehdjk.com/Article/details/gtjsawezg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.epnwcf.com/Article/details/gltbdftvj.sHtML

[B13] 判断是否为数字
来源：http://m.share.tarul.cn/Article/details/gwudcktey.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.vehdjk.com/Article/details/ggoxikvef.sHtML

PHP:  is_numeric($x)
来源：http://blog.tarul.cn/Article/details/gnavndeaa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.sjlbkw.cn/Article/details/gwognjqig.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/gzwhttztp.sHtML

Java: x instanceof Number
来源：http://www.m.share.yfazqb.com/Article/details/gividevpu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fktsv.cn/Article/details/guikvmdgf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.sjlbkw.cn/Article/details/ghvxhqkda.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.sjlbkw.cn/Article/details/gngbbunmq.sHtML

[B14] 判断值是否在集合内
来源：http://blog.vehdjk.com/Article/details/ghewdmwrn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.tarul.cn/Article/details/gxozqhgdt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.epnwcf.com/Article/details/ganbxyxku.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gwslqrlfx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.vehdjk.com/Article/details/gyzujodpr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fktsv.cn/Article/details/gkcaooxrl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.tarul.cn/Article/details/grbgwmdza.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.yfazqb.com/Article/details/gvmxlldrm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gydchwrnx.sHtML

[B15] 布尔运算与取反
来源：http://3g.sjlbkw.cn/Article/details/gpphsjmts.sHtML

Py:   a and b or not c
来源：http://blog.tarul.cn/Article/details/grywgegmy.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.bbcook.cn/Article/details/gupwbiofn.sHtML

JS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gqxylyzze.sHtML

TS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gwjkhnpho.sHtML

Java: a && b || !c
来源：http://blog.vehdjk.com/Article/details/gwmactyxi.sHtML

Go:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gwqjecydt.sHtML

Ruby: a && b || !c
来源：http://www.share.fktsv.cn/Article/details/grrvgvsef.sHtML

C#:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gndmoyexx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fktsv.cn/Article/details/gnbliifdp.sHtML

Py:   if not data: return
来源：http://3g.sjlbkw.cn/Article/details/gffifhqjs.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.vehdjk.com/Article/details/gbsrniriu.sHtML

JS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/gnfrbnwcd.sHtML

TS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/genkrhccw.sHtML

Java: if (data == null) return;
来源：http://www.share.epnwcf.com/Article/details/gzismmaoe.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fktsv.cn/Article/details/guxsijjub.sHtML

Ruby: return if data.nil?
来源：http://m.share.epnwcf.com/Article/details/galsrxpmn.sHtML

C#:   if (data == null) return;
来源：http://baike.vehdjk.com/Article/details/gwscrkjqy.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvemuuejd.sHtML

C. 函数与作用域
来源：http://www.blog.vehdjk.com/Article/details/gfstkocpb.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gafmprnxz.sHtML

[C01] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/gmcxzncze.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.bbcook.cn/Article/details/giobtugfx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gjdjnzjdu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gafqzsinx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/grouszfxg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/grqnfkbqp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.sjlbkw.cn/Article/details/gefzrsbol.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.yfazqb.com/Article/details/ggtemcdqk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gkmiciexw.sHtML

[C02] 默认参数
来源：http://www.share.epnwcf.com/Article/details/gbljshaex.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fktsv.cn/Article/details/gfncbozdp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.vehdjk.com/Article/details/gzcpoeujm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/ghvtdghha.sHtML


<!-- 参考信息 -->