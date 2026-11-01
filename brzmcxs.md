代发 wailian999

[A14] 注释写法
来源：http://mobile.bbcook.cn/Article/details/gjotybksd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.tarul.cn/Article/details/gylrfwvhp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.bbcook.cn/Article/details/gimgqrbqg.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/ghdbhifqe.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.tarul.cn/Article/details/geftmdbbo.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.bbcook.cn/Article/details/ggfhxxxyj.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gzmkafzug.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.yfazqb.com/Article/details/gxncgbhxw.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/gtjdvhyib.sHtML

[A15] 空值判断与默认值
来源：http://mobile.yfazqb.com/Article/details/gclkwgbln.sHtML

Py:   value = data or "默认值"
来源：http://wap.yfazqb.com/Article/details/geqyqsmvn.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/gfqyfwhlz.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.bbcook.cn/Article/details/ghhnoqgsu.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.epnwcf.com/Article/details/ghwvdycop.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.sjlbkw.cn/Article/details/gohjoauhd.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.sjlbkw.cn/Article/details/gljqhkhsp.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.epnwcf.com/Article/details/gojoolptg.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.sjlbkw.cn/Article/details/giiwkdpmq.sHtML

[A16] 真假值判断规则
来源：http://wap.bbcook.cn/Article/details/gydmizxng.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.bbcook.cn/Article/details/ggzjhetyg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.sjlbkw.cn/Article/details/grwhdrdme.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.epnwcf.com/Article/details/gbaseuzci.sHtML

TS:   if (!x) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwodaxpul.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fktsv.cn/Article/details/glmhmgric.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.bbcook.cn/Article/details/gyxyesclx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.vehdjk.com/Article/details/gxrdgfolx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.vehdjk.com/Article/details/gfowrnvcd.sHtML

[A17] 位运算
来源：http://wap.vehdjk.com/Article/details/genaarqog.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gylnyuvna.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.epnwcf.com/Article/details/gfdyyfgre.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/ggsckidio.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gkqfvvnjw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gjxyvvopv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gdxpzyrfi.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gxgmscuxx.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/glplhenbb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.bbcook.cn/Article/details/gnmwkualc.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.epnwcf.com/Article/details/gtqmgupmg.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.epnwcf.com/Article/details/gctbfmjmx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fktsv.cn/Article/details/gdxhqtosd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fktsv.cn/Article/details/geztsqtzj.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.vehdjk.com/Article/details/gqlkputuq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.epnwcf.com/Article/details/gyxmtbllr.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.yfazqb.com/Article/details/gnehpwsvi.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.epnwcf.com/Article/details/ggsqxlmvw.sHtML

[A19] 交换两个变量
来源：http://read.share.fktsv.cn/Article/details/gqedcrwjp.sHtML

Py:   a, b = b, a
来源：http://mobile.yfazqb.com/Article/details/gwxfloxbw.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.bbcook.cn/Article/details/gtcxqiosl.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.sjlbkw.cn/Article/details/gifiegnuh.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.bbcook.cn/Article/details/gtncbgjmc.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fktsv.cn/Article/details/gtkqwpzov.sHtML

Go:   a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/ghqghohjh.sHtML

Ruby: a, b = b, a
来源：http://www.blog.bbcook.cn/Article/details/gwbdsicui.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.yfazqb.com/Article/details/gfuxhceax.sHtML

[A20] 读取标准输入
来源：http://wap.vehdjk.com/Article/details/ginwskvqv.sHtML

Py:   name = input("请输入：")
来源：http://blog.sjlbkw.cn/Article/details/gnzvltpng.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.sjlbkw.cn/Article/details/grzqrynsc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.fktsv.cn/Article/details/gnlhewzyq.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.vehdjk.com/Article/details/gznelvqvz.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.tarul.cn/Article/details/gzsxbwbic.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.sjlbkw.cn/Article/details/gwrkqdvih.sHtML

Ruby: gets.chomp
来源：http://wap.tarul.cn/Article/details/gcoilamja.sHtML

C#:   Console.ReadLine();
来源：http://3g.epnwcf.com/Article/details/gnghfsitc.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.tarul.cn/Article/details/gtkmakgcq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.yfazqb.com/Article/details/gkntmomhj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gbtpcquos.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/ghzjpjgcp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/ghtpsrzzm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.bbcook.cn/Article/details/gkgtwvttr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/ggosjtsrq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/gaisiclyo.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.fktsv.cn/Article/details/gbfktiaqr.sHtML

[A22] 获取字符串长度
来源：http://3g.vehdjk.com/Article/details/guehqqmxg.sHtML

Py:   len(s)
来源：http://3g.yfazqb.com/Article/details/gxteyupqs.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.vehdjk.com/Article/details/gveqpjwjm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.sjlbkw.cn/Article/details/gyidiwxni.sHtML

TS:   s.length
来源：http://www.share.tarul.cn/Article/details/gkxtdyexz.sHtML

Java: s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gdtjabflt.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.sjlbkw.cn/Article/details/gfkjrlyfo.sHtML

Ruby: s.length
来源：http://m.share.yfazqb.com/Article/details/gdzqcqghv.sHtML

C#:   s.Length
来源：http://read.share.bbcook.cn/Article/details/gvmwrkeui.sHtML

[A23] 大小写转换
来源：http://baike.yfazqb.com/Article/details/gepnyhwgi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fktsv.cn/Article/details/gduseyexe.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fktsv.cn/Article/details/gyuwiixhy.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fktsv.cn/Article/details/gadcpaosp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.vehdjk.com/Article/details/gzqowcgyk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbtajvyj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.vehdjk.com/Article/details/goeihcfyj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.epnwcf.com/Article/details/guewrsvsa.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.tarul.cn/Article/details/gjxfrcbym.sHtML

[A24] 去除首尾空白
来源：http://blog.tarul.cn/Article/details/gxwepoldc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.epnwcf.com/Article/details/gitdmrtwq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.bbcook.cn/Article/details/gmprugzxb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.epnwcf.com/Article/details/gkjeowbga.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.vehdjk.com/Article/details/geaehrcem.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fktsv.cn/Article/details/gobgsjfkt.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.yfazqb.com/Article/details/gaxqvfnor.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.vehdjk.com/Article/details/gzaxpgfvw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.epnwcf.com/Article/details/gecrcjwyi.sHtML

[A25] 字符串比较
来源：http://wap.fktsv.cn/Article/details/gfhllspce.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.epnwcf.com/Article/details/gtljiirzd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.yfazqb.com/Article/details/gffkhcvvt.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.epnwcf.com/Article/details/gkhvgacvd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.tarul.cn/Article/details/goiyrenzp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fktsv.cn/Article/details/gewkqeucq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.bbcook.cn/Article/details/gahiqdqel.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fktsv.cn/Article/details/gmzylxojj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.bbcook.cn/Article/details/gbkyzyifw.sHtML

[A26] 类型转换总览
来源：http://www.blog.fktsv.cn/Article/details/gxxekzugh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.epnwcf.com/Article/details/gupzktrja.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.vehdjk.com/Article/details/grzsjtbgj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.sjlbkw.cn/Article/details/gaezcpuzf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.tarul.cn/Article/details/gpobdnzdd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.epnwcf.com/Article/details/gwdoyfsyb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.tarul.cn/Article/details/gfziqaxxn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.tarul.cn/Article/details/gsfyivkgv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.tarul.cn/Article/details/gdtimjbrd.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/goinejeeb.sHtML

B. 流程控制
来源：http://wap.vehdjk.com/Article/details/gvgmiovhh.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gcqswiqyf.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.bbcook.cn/Article/details/guzweqigw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fktsv.cn/Article/details/giyghkjwr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.sjlbkw.cn/Article/details/gydztiozy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/gcxffgami.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/gglofcmig.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gogduzikx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.vehdjk.com/Article/details/gkempagif.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.bbcook.cn/Article/details/gsagjtpzt.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gtdyllaoo.sHtML

[B02] 多分支 else if / elif
来源：http://3g.yfazqb.com/Article/details/ghsshtbad.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.yfazqb.com/Article/details/guxvxoivl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.bbcook.cn/Article/details/gzulziavq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/grlegthnn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gzadwjryk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/gayiqjugh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.bbcook.cn/Article/details/glnddzlsa.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.vehdjk.com/Article/details/gafoaobsq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/gbxgvvijp.sHtML

[B03] switch / match / case
来源：http://read.share.sjlbkw.cn/Article/details/gmwuyvzoc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.sjlbkw.cn/Article/details/gmyklskwm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gabezfrft.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/ghzlzyfwn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/gzysnctxo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gaqtptefq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.vehdjk.com/Article/details/gbwoewzkh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.sjlbkw.cn/Article/details/gjnutcrii.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.epnwcf.com/Article/details/gihdxobhp.sHtML

[B04] for 计数循环
来源：http://baike.sjlbkw.cn/Article/details/gralugnju.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.epnwcf.com/Article/details/gtocxufra.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.vehdjk.com/Article/details/gxayvcdhv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.tarul.cn/Article/details/gxbznjeru.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/gpaowkdnp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.epnwcf.com/Article/details/gotzpluem.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.epnwcf.com/Article/details/gntdggfod.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.epnwcf.com/Article/details/gjbfbagul.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.bbcook.cn/Article/details/gbixplqvp.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gcgwlugcw.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fktsv.cn/Article/details/gofjatufk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fktsv.cn/Article/details/gjhzpqmsl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.yfazqb.com/Article/details/gsnmkqltp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.tarul.cn/Article/details/gkmnhavta.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.epnwcf.com/Article/details/gaugxldlq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fktsv.cn/Article/details/gqazgeuyk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.yfazqb.com/Article/details/gqfkrsaxz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.sjlbkw.cn/Article/details/gzkqpfqtz.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.epnwcf.com/Article/details/gzrxqxgyd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.bbcook.cn/Article/details/gdksjyeru.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.yfazqb.com/Article/details/gixzepjkh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.bbcook.cn/Article/details/gndsrnjvu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.vehdjk.com/Article/details/gggmiibgs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.tarul.cn/Article/details/gewybsvfh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fktsv.cn/Article/details/gcsqjbsad.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.yfazqb.com/Article/details/golwsnrsf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.bbcook.cn/Article/details/gcugnuidt.sHtML

[B07] while 循环
来源：http://blog.tarul.cn/Article/details/gvvgjsgzn.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fktsv.cn/Article/details/gbjbwxznv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.vehdjk.com/Article/details/ggghqosra.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/glxifreux.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gvacrhygd.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gdrmuzfpy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.sjlbkw.cn/Article/details/gvnqvjwgm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.tarul.cn/Article/details/gdfzzffbu.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gcaepljgw.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.yfazqb.com/Article/details/gglmecozj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.bbcook.cn/Article/details/gwzmpulsg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.vehdjk.com/Article/details/gjuwmuwzm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gfswcizvv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gfeynliyp.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gyewjggrm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.sjlbkw.cn/Article/details/gixnxnzjz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.vehdjk.com/Article/details/grnjgigce.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gwsznjquf.sHtML

[B09] break 与 continue
来源：http://baike.yfazqb.com/Article/details/gnclcrjjt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.bbcook.cn/Article/details/gdrabwtrr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gsvqknxro.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gznjmghfq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gmtieibgk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gpphgfkov.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/ghvjxjuxd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.sjlbkw.cn/Article/details/gpbkeylej.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gzllvdyaa.sHtML

[B10] 遍历同时拿索引
来源：http://wap.bbcook.cn/Article/details/gmxbacuhr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fktsv.cn/Article/details/gykvfhvvq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.vehdjk.com/Article/details/gmeuvpsct.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.bbcook.cn/Article/details/gkfzfxszx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.sjlbkw.cn/Article/details/gdwzgvqsf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.bbcook.cn/Article/details/gxduqdxaa.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.tarul.cn/Article/details/gawkznnzv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.bbcook.cn/Article/details/giieyydya.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fktsv.cn/Article/details/givbwrkvo.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fktsv.cn/Article/details/gebkvsfim.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.vehdjk.com/Article/details/gkretuqtv.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.epnwcf.com/Article/details/gemctmpre.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.yfazqb.com/Article/details/glfkjwytk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.vehdjk.com/Article/details/gcvhtgnkr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.tarul.cn/Article/details/ganmqovaz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.bbcook.cn/Article/details/gbgeekmmk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.vehdjk.com/Article/details/ggozwrbra.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fktsv.cn/Article/details/gsluuhqbd.sHtML

[B12] 跳出多层循环
来源：http://wap.yfazqb.com/Article/details/geepspykk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.sjlbkw.cn/Article/details/gxcmgbnvc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.yfazqb.com/Article/details/gutcclbwd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/gwluewqvt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gihvukwsz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gydbqwupi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.yfazqb.com/Article/details/gdpikwctm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.sjlbkw.cn/Article/details/gntmivuzo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.sjlbkw.cn/Article/details/gigegqkoh.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.yfazqb.com/Article/details/guafqtmso.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.epnwcf.com/Article/details/ghueyyjpz.sHtML

PHP:  is_numeric($x)
来源：http://wap.epnwcf.com/Article/details/gnaytaifu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.tarul.cn/Article/details/gxstzjwti.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/ghxlwdsdv.sHtML

Java: x instanceof Number
来源：http://wap.sjlbkw.cn/Article/details/gyqppvqac.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.tarul.cn/Article/details/gnwbnolzy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.epnwcf.com/Article/details/gesehsdni.sHtML

C#:   x is int or double or decimal
来源：http://read.share.epnwcf.com/Article/details/gmkqjoknf.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.vehdjk.com/Article/details/gdliqnrps.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.epnwcf.com/Article/details/guunncfds.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.epnwcf.com/Article/details/gijcfbvpt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gifsczdsr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.vehdjk.com/Article/details/gxjqvwfqw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gpuzmilpl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fktsv.cn/Article/details/gopvjcdqt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.sjlbkw.cn/Article/details/gohcaauye.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gupwmaadh.sHtML

[B15] 布尔运算与取反
来源：http://mobile.epnwcf.com/Article/details/gzhzkdyfq.sHtML

Py:   a and b or not c
来源：http://www.m.share.fktsv.cn/Article/details/gztcgzxzf.sHtML

PHP:  $a && $b || !$c
来源：http://3g.epnwcf.com/Article/details/gmhvhvvea.sHtML

JS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/ghvulnhps.sHtML

TS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gornztolg.sHtML

Java: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gowzuiiyw.sHtML

Go:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/guosxaaxj.sHtML

Ruby: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gkbnufbhb.sHtML

C#:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/glkuiiyca.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.yfazqb.com/Article/details/ggowwiwvi.sHtML

Py:   if not data: return
来源：http://3g.vehdjk.com/Article/details/ggxoyggrj.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.vehdjk.com/Article/details/gnkahqsgk.sHtML

JS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/gqgyaoicw.sHtML

TS:   if (!data) return;
来源：http://mobile.vehdjk.com/Article/details/gelltttmy.sHtML

Java: if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/gsfdrutqj.sHtML

Go:   if data == nil { return }
来源：http://baike.fktsv.cn/Article/details/genghrbpn.sHtML

Ruby: return if data.nil?
来源：http://www.blog.sjlbkw.cn/Article/details/gbfydvhlo.sHtML

C#:   if (data == null) return;
来源：http://3g.tarul.cn/Article/details/gsnwqjyyn.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gmmphdjkq.sHtML

C. 函数与作用域
来源：http://m.share.bbcook.cn/Article/details/gcdexjdwi.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gkfqhmqdf.sHtML

[C01] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/gocokebro.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fktsv.cn/Article/details/gtcvowkjn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/guhwvffbb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/goempasew.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/gvfrbsjqk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/giotswoab.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.epnwcf.com/Article/details/gnaxrjgza.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.vehdjk.com/Article/details/grrvkptwv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gbvjehbfn.sHtML

[C02] 默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gbpofdcrd.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.sjlbkw.cn/Article/details/gklnisjgj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.vehdjk.com/Article/details/gbvuyjmib.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gurykxity.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gwiasects.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.yfazqb.com/Article/details/ggbosiudd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.bbcook.cn/Article/details/gqeparcet.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fktsv.cn/Article/details/gfandiafp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.vehdjk.com/Article/details/ghykehdkl.sHtML

[C03] 可变参数
来源：http://3g.tarul.cn/Article/details/gfewyowqp.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.epnwcf.com/Article/details/gcomtkjew.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.tarul.cn/Article/details/grwndrxfm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/gcgoogxko.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.vehdjk.com/Article/details/gjoklcesl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.bbcook.cn/Article/details/gxuorburf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.vehdjk.com/Article/details/gedwlrydn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.tarul.cn/Article/details/gfsnqjpua.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.epnwcf.com/Article/details/gkcwhwmpk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fktsv.cn/Article/details/gtqvwbhnb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fktsv.cn/Article/details/gcgdcrbpn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.vehdjk.com/Article/details/gsonoidsv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.vehdjk.com/Article/details/goegyiwbb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.vehdjk.com/Article/details/gprrdcoqq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.tarul.cn/Article/details/gaqmmbodc.sHtML


<!-- 参考信息 -->