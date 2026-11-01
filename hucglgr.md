代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.vehdjk.com/Article/details/gsolrkxfd.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.yfazqb.com/Article/details/gketuivmb.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.vehdjk.com/Article/details/gosqvbwuo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.vehdjk.com/Article/details/gvkdlfcuz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.epnwcf.com/Article/details/gahyxxuyg.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.sjlbkw.cn/Article/details/ginnydyeu.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.yfazqb.com/Article/details/gvyzakplv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.sjlbkw.cn/Article/details/gofarsylf.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gzscpelrh.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.epnwcf.com/Article/details/gdwyzjckq.sHtML

JS:   "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/gtmjpqanb.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gibvrvcsh.sHtML

Java: "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gjmfwnjbx.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gnhpwijjo.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/genvhcqny.sHtML

C#:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/guhrlsadf.sHtML

[A14] 注释写法
来源：http://3g.fktsv.cn/Article/details/gjvrbhkrb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.epnwcf.com/Article/details/gmkqdjgxb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gnnosdakc.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/ggayaoavy.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gslucxfci.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.vehdjk.com/Article/details/gohchwwgy.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.fktsv.cn/Article/details/gaxnkdxen.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.tarul.cn/Article/details/gapyplutn.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.vehdjk.com/Article/details/gzvdysjew.sHtML

[A15] 空值判断与默认值
来源：http://wap.fktsv.cn/Article/details/gkpdwaurz.sHtML

Py:   value = data or "默认值"
来源：http://baike.sjlbkw.cn/Article/details/gptiikjnw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.tarul.cn/Article/details/gwtllvopx.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.tarul.cn/Article/details/gxqwczbqx.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.vehdjk.com/Article/details/ggemapfgh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.yfazqb.com/Article/details/gdffhebsj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.bbcook.cn/Article/details/gnhdpfhgg.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.tarul.cn/Article/details/gcamdeyvp.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/gbczznqnr.sHtML

[A16] 真假值判断规则
来源：http://blog.tarul.cn/Article/details/gvgnfsjda.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.yfazqb.com/Article/details/gbjaugrcx.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.vehdjk.com/Article/details/gckohjcfj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.fktsv.cn/Article/details/gqqyybpdn.sHtML

TS:   if (!x) {}
来源：http://read.share.tarul.cn/Article/details/gretecsue.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.tarul.cn/Article/details/geansnrio.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.tarul.cn/Article/details/glpvxfchz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.bbcook.cn/Article/details/gsyzhivul.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fktsv.cn/Article/details/gksfigowk.sHtML

[A17] 位运算
来源：http://wap.sjlbkw.cn/Article/details/giuuhmjqv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gupczgxob.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.bbcook.cn/Article/details/glprviilf.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gvrnnapin.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gpznynyjq.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gsrekmxhr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gglxvckkq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/ghtoxiacm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gjxvyohpb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcjapsfv.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.yfazqb.com/Article/details/gyoxkslzi.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.bbcook.cn/Article/details/gtpiswlnl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.yfazqb.com/Article/details/gacknupmm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.yfazqb.com/Article/details/grtxamwwf.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.tarul.cn/Article/details/gtiuoafwd.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.epnwcf.com/Article/details/gxemfjvuu.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.tarul.cn/Article/details/garaytzhu.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.sjlbkw.cn/Article/details/gcfjqulrw.sHtML

[A19] 交换两个变量
来源：http://mobile.bbcook.cn/Article/details/gakdxozax.sHtML

Py:   a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gbufshtun.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.vehdjk.com/Article/details/gvojmvfds.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.bbcook.cn/Article/details/gnzkspuhv.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.tarul.cn/Article/details/gjitznjnk.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.bbcook.cn/Article/details/gczitemky.sHtML

Go:   a, b = b, a
来源：http://read.share.vehdjk.com/Article/details/gwjiwuamb.sHtML

Ruby: a, b = b, a
来源：http://mobile.tarul.cn/Article/details/grskuujra.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.bbcook.cn/Article/details/ghmzdayuo.sHtML

[A20] 读取标准输入
来源：http://www.m.share.epnwcf.com/Article/details/guieekeob.sHtML

Py:   name = input("请输入：")
来源：http://www.share.vehdjk.com/Article/details/galfmjziz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.epnwcf.com/Article/details/gblwhzpyw.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.vehdjk.com/Article/details/gilmbgjfb.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.tarul.cn/Article/details/ggnlkrazq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.bbcook.cn/Article/details/gwjbqlczs.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.tarul.cn/Article/details/gmijramrc.sHtML

Ruby: gets.chomp
来源：http://blog.bbcook.cn/Article/details/goklrbiey.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.tarul.cn/Article/details/gqtxmnyki.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.yfazqb.com/Article/details/gdixadocz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.sjlbkw.cn/Article/details/gcvgzyozx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/grkhvrqka.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.bbcook.cn/Article/details/gdonlhpag.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/gkgbvazok.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gyuyshbnj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/gbfvgjuyl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/giuhkztbi.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.yfazqb.com/Article/details/ghxymxrld.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gbroztvui.sHtML

Py:   len(s)
来源：http://3g.sjlbkw.cn/Article/details/gnvzltzwv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.epnwcf.com/Article/details/gmmtwhiim.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fktsv.cn/Article/details/geyspcggx.sHtML

TS:   s.length
来源：http://mobile.bbcook.cn/Article/details/gochfykbb.sHtML

Java: s.length()
来源：http://www.share.tarul.cn/Article/details/gmcolqptp.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.vehdjk.com/Article/details/glqmfpoyd.sHtML

Ruby: s.length
来源：http://mobile.epnwcf.com/Article/details/grrqjydcs.sHtML

C#:   s.Length
来源：http://3g.bbcook.cn/Article/details/gsspleitb.sHtML

[A23] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/gpcbwands.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.yfazqb.com/Article/details/gsmvnzhlr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fktsv.cn/Article/details/gtqrqopcx.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/gnftmeote.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.tarul.cn/Article/details/galtnkfhn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fktsv.cn/Article/details/gwgawkzus.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.tarul.cn/Article/details/gazsoptjd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.bbcook.cn/Article/details/grdvndwph.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.fktsv.cn/Article/details/gegqdihyt.sHtML

[A24] 去除首尾空白
来源：http://wap.epnwcf.com/Article/details/gbcgvesvt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.bbcook.cn/Article/details/gsufbpocr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.vehdjk.com/Article/details/gtfdmjdqg.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/gkjhueujq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.sjlbkw.cn/Article/details/gbwlexnux.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.sjlbkw.cn/Article/details/gzipkigez.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.bbcook.cn/Article/details/ggqqwemuf.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.epnwcf.com/Article/details/gnpfhqyhy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fktsv.cn/Article/details/gqjjcsipd.sHtML

[A25] 字符串比较
来源：http://www.share.bbcook.cn/Article/details/gysgjcqov.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.vehdjk.com/Article/details/gzwrkzarp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fktsv.cn/Article/details/gtukxidqz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/gzmherfxd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.epnwcf.com/Article/details/gsgdevrqq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.yfazqb.com/Article/details/gfrekzfrb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.vehdjk.com/Article/details/geuxqrvhn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.epnwcf.com/Article/details/grepfhftt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fktsv.cn/Article/details/gmpezmzkd.sHtML

[A26] 类型转换总览
来源：http://mobile.epnwcf.com/Article/details/gaglbuhha.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.tarul.cn/Article/details/ghniaclkx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.vehdjk.com/Article/details/gmcufvelm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.bbcook.cn/Article/details/gouazncqj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.sjlbkw.cn/Article/details/gyhmasnht.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fktsv.cn/Article/details/gflhhwkrd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.sjlbkw.cn/Article/details/glczhwxfz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.tarul.cn/Article/details/gtnefjxif.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fktsv.cn/Article/details/gpwzbffkc.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gmbzeemnb.sHtML

B. 流程控制
来源：http://www.blog.vehdjk.com/Article/details/gnwgpaewt.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/guanlbheg.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fktsv.cn/Article/details/gelsrhqrb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.epnwcf.com/Article/details/gfojcvaqb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.vehdjk.com/Article/details/gviuqwavp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.tarul.cn/Article/details/gtbkvapih.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gzoizrchs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gvegpodef.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.yfazqb.com/Article/details/ghylbkyvo.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.yfazqb.com/Article/details/glrdrkcfs.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gwiyuopfy.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.yfazqb.com/Article/details/gojcypnrg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.tarul.cn/Article/details/gvlgykkpj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fktsv.cn/Article/details/gdsznkqhx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gmwyoassb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gwbfnexpd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/ggdprvfgs.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.sjlbkw.cn/Article/details/gmswcdokh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fktsv.cn/Article/details/gjwwppzxk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/gbkoeqdit.sHtML

[B03] switch / match / case
来源：http://www.blog.vehdjk.com/Article/details/gfavmxxmh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.epnwcf.com/Article/details/gnizjjkxt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gyvyvnxgs.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/ghbpvusdm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gzjjkazix.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gclctjtge.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.sjlbkw.cn/Article/details/gwlmjbhms.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.vehdjk.com/Article/details/gnmfxupye.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.yfazqb.com/Article/details/gfswfhvfc.sHtML

[B04] for 计数循环
来源：http://m.share.sjlbkw.cn/Article/details/gfnervjxc.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.epnwcf.com/Article/details/gnxkxcsqx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.sjlbkw.cn/Article/details/gifhcuqep.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.tarul.cn/Article/details/gfaxaeukf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fktsv.cn/Article/details/gowhvsgoy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gstbeuqgf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.vehdjk.com/Article/details/gkegbtdtq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.sjlbkw.cn/Article/details/grozkjagb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.bbcook.cn/Article/details/geokaytnh.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gonpeuogs.sHtML

Py:   for item in arr: print(item)
来源：http://3g.sjlbkw.cn/Article/details/grvqmxoez.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.epnwcf.com/Article/details/gsqgurwtg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fktsv.cn/Article/details/gyiszjqfr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.tarul.cn/Article/details/gsmdabyii.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.tarul.cn/Article/details/gdluehpgt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.sjlbkw.cn/Article/details/gwqkddeyy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.vehdjk.com/Article/details/gsbkhnvtd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.yfazqb.com/Article/details/gqlmtlubo.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fktsv.cn/Article/details/ghijsuose.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fktsv.cn/Article/details/ggonsrkgx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.bbcook.cn/Article/details/gminusodx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.vehdjk.com/Article/details/gpwopkiok.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.bbcook.cn/Article/details/gpcmwmkbs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.tarul.cn/Article/details/gglfhabbm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.sjlbkw.cn/Article/details/gfllmqxxa.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.sjlbkw.cn/Article/details/gjdzxigoe.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fktsv.cn/Article/details/gbwvkiyrg.sHtML

[B07] while 循环
来源：http://m.share.yfazqb.com/Article/details/ggjavzyqb.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.bbcook.cn/Article/details/gobbneaog.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.vehdjk.com/Article/details/gatpqlikj.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gemofwctw.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/grynhtqww.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gvklgviri.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.sjlbkw.cn/Article/details/gobwrgrsy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.tarul.cn/Article/details/gpkgajcsk.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gnffojgeo.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.yfazqb.com/Article/details/gnvcwrnca.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fktsv.cn/Article/details/gqpgcuwpm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/giuqhwkfv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gtvntbprc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gbamehepy.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/gssttidij.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.vehdjk.com/Article/details/gvsfjgxsk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fktsv.cn/Article/details/gtkqwkszr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gnpcsovrs.sHtML

[B09] break 与 continue
来源：http://www.share.vehdjk.com/Article/details/gbeoziwgi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.sjlbkw.cn/Article/details/gbdgyiwhz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gbovsqpvr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gphximkut.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/guylunmmy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gezdtybtz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.tarul.cn/Article/details/giymsozix.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.epnwcf.com/Article/details/gqhdtnpbs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gwsyukghh.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.yfazqb.com/Article/details/gefskmlrp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.sjlbkw.cn/Article/details/gsywunzaz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.bbcook.cn/Article/details/gsebxvckw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/gxptnbion.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.epnwcf.com/Article/details/gukylqkvs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.bbcook.cn/Article/details/galopbpiz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fktsv.cn/Article/details/gkcaieioj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.bbcook.cn/Article/details/gwepquzgg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.vehdjk.com/Article/details/gulvbonhp.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.bbcook.cn/Article/details/gnrsnepmp.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.tarul.cn/Article/details/gewsimkxj.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.vehdjk.com/Article/details/gmdrdzdov.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.sjlbkw.cn/Article/details/gjffjtdew.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/gizemgukl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.yfazqb.com/Article/details/gwpfulaym.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.epnwcf.com/Article/details/gtfmbgtri.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.tarul.cn/Article/details/gleeqvrov.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.vehdjk.com/Article/details/gkbdpjfek.sHtML

[B12] 跳出多层循环
来源：http://mobile.bbcook.cn/Article/details/gzhtaqrvu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.epnwcf.com/Article/details/gnqszazhd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fktsv.cn/Article/details/gqbntarnx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gwdztziul.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/gffbngsfz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/guqdjoxkx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.yfazqb.com/Article/details/gikclytne.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.yfazqb.com/Article/details/ghbyzfkdz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fktsv.cn/Article/details/gekhvxsny.sHtML

[B13] 判断是否为数字
来源：http://read.share.tarul.cn/Article/details/gntaqrrzj.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.epnwcf.com/Article/details/gxiijrmhl.sHtML

PHP:  is_numeric($x)
来源：http://baike.vehdjk.com/Article/details/ghtfdgyad.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/guhwiafka.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/gapyxyqmj.sHtML

Java: x instanceof Number
来源：http://www.share.epnwcf.com/Article/details/gdgroauki.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.bbcook.cn/Article/details/gteoryptc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.bbcook.cn/Article/details/gcdclbtcc.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.yfazqb.com/Article/details/gsghsieaz.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.sjlbkw.cn/Article/details/gprpigywf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.bbcook.cn/Article/details/ghsrfwqll.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fktsv.cn/Article/details/gnryjwxqx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.bbcook.cn/Article/details/godsjcjgi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fktsv.cn/Article/details/gayznasoh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.vehdjk.com/Article/details/gisivzfps.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.bbcook.cn/Article/details/ggrtyxdwc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnudagtxh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/gtvwjgfrm.sHtML

[B15] 布尔运算与取反
来源：http://m.share.bbcook.cn/Article/details/gtqjnkrqz.sHtML

Py:   a and b or not c
来源：http://mobile.sjlbkw.cn/Article/details/goyflylwq.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fktsv.cn/Article/details/glsbdsjyd.sHtML

JS:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gwcqayouu.sHtML

TS:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gysjhxtyv.sHtML

Java: a && b || !c
来源：http://baike.epnwcf.com/Article/details/giivzohwm.sHtML

Go:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gyjgatmck.sHtML

Ruby: a && b || !c
来源：http://baike.vehdjk.com/Article/details/glpgmqrdd.sHtML

C#:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gefwffnuz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fktsv.cn/Article/details/ghwslrnsj.sHtML

Py:   if not data: return
来源：http://www.share.bbcook.cn/Article/details/gttlyhnqh.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.vehdjk.com/Article/details/gsdzxuitc.sHtML

JS:   if (!data) return;
来源：http://wap.epnwcf.com/Article/details/gyauixfzb.sHtML

TS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/gzmtdypbz.sHtML

Java: if (data == null) return;
来源：http://3g.yfazqb.com/Article/details/gqgdwqajp.sHtML

Go:   if data == nil { return }
来源：http://wap.bbcook.cn/Article/details/gmbhuwfqj.sHtML

Ruby: return if data.nil?
来源：http://mobile.bbcook.cn/Article/details/goqmofglc.sHtML

C#:   if (data == null) return;
来源：http://blog.epnwcf.com/Article/details/goeembzmu.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gdjmgutzw.sHtML

C. 函数与作用域
来源：http://3g.epnwcf.com/Article/details/gncdkfszi.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gviamjqnw.sHtML

[C01] 定义函数
来源：http://blog.yfazqb.com/Article/details/gosyaqajd.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.yfazqb.com/Article/details/gicwzlwni.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gzpzysftu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gxiejhjce.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/ghlmaqppr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/ganvyyqco.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.vehdjk.com/Article/details/gnzmcxjox.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.vehdjk.com/Article/details/gknbnnxtc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gcxruzifj.sHtML

[C02] 默认参数
来源：http://mobile.yfazqb.com/Article/details/gfnrjelyw.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.tarul.cn/Article/details/givchpnyn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.tarul.cn/Article/details/gjysztpsy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gruppkaal.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gjfglvvvh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.epnwcf.com/Article/details/gjzphjuvf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.epnwcf.com/Article/details/gwdkratwb.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.tarul.cn/Article/details/gguxermbr.sHtML


<!-- 参考信息 -->