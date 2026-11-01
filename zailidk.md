代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.sjlbkw.cn/Article/details/gszopxtvo.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.yfazqb.com/Article/details/gkokiekci.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.vehdjk.com/Article/details/gqzihovft.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.epnwcf.com/Article/details/geqxpfqkb.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.sjlbkw.cn/Article/details/gwtrguayc.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.vehdjk.com/Article/details/gojpsjuxi.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.yfazqb.com/Article/details/gadumqsth.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fktsv.cn/Article/details/glshptqwd.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gykwlkjgz.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/gghomgymk.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gyjknhltv.sHtML

TS:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/glppmlicj.sHtML

Java: "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/giqrqaiak.sHtML

Go:   "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gcfjadgdy.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/grpnncmmu.sHtML

C#:   "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gbooveqdt.sHtML

[A14] 注释写法
来源：http://www.blog.vehdjk.com/Article/details/gtsqqburb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fktsv.cn/Article/details/guakykixn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/gzwqnzzpz.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/ghzrtumkj.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/ghvazzpul.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.epnwcf.com/Article/details/gmzapgshr.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.tarul.cn/Article/details/glwcpoarm.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.yfazqb.com/Article/details/goyyaeckm.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/gzqvcfkni.sHtML

[A15] 空值判断与默认值
来源：http://wap.sjlbkw.cn/Article/details/glxqpnkem.sHtML

Py:   value = data or "默认值"
来源：http://3g.fktsv.cn/Article/details/glpyoutju.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.sjlbkw.cn/Article/details/glnzvmrca.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/guarwxgrm.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.bbcook.cn/Article/details/gyodanjlg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.sjlbkw.cn/Article/details/gaqaiscwm.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.bbcook.cn/Article/details/gkxsuayaw.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.bbcook.cn/Article/details/ggxhrhawb.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/gbfvcxqlt.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.tarul.cn/Article/details/gkzzwoyxs.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.tarul.cn/Article/details/gdfcbrtus.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.yfazqb.com/Article/details/gzwerfnwk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.sjlbkw.cn/Article/details/gqzvjclee.sHtML

TS:   if (!x) {}
来源：http://3g.yfazqb.com/Article/details/gcqagedkr.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.vehdjk.com/Article/details/gjjmfvhyw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.tarul.cn/Article/details/gfaaimhrn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.bbcook.cn/Article/details/gvzinxfdo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.bbcook.cn/Article/details/gzbwnvfpa.sHtML

[A17] 位运算
来源：http://www.m.share.yfazqb.com/Article/details/gsgjqhzts.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/gectqgdgv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.yfazqb.com/Article/details/ghdlnrofo.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gdhsamvxm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/guqbqotvc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gwfzwdhag.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gxkdooxjd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/giwzzvhzb.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gothjjvaq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.bbcook.cn/Article/details/glgdelziy.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.fktsv.cn/Article/details/gdcfzotiv.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.tarul.cn/Article/details/gitkirmgg.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.bbcook.cn/Article/details/gfvljsnmx.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.vehdjk.com/Article/details/gdlwvonpd.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.tarul.cn/Article/details/gxtzveypn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.tarul.cn/Article/details/gjtbjjhcp.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.bbcook.cn/Article/details/gqabrvzfr.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.tarul.cn/Article/details/ghsrbpbbp.sHtML

[A19] 交换两个变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfgfwbye.sHtML

Py:   a, b = b, a
来源：http://baike.bbcook.cn/Article/details/gxiudsogq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.fktsv.cn/Article/details/glixuppkd.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.bbcook.cn/Article/details/gnoykvawg.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.sjlbkw.cn/Article/details/gajmpjkae.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fktsv.cn/Article/details/gfuuihvzt.sHtML

Go:   a, b = b, a
来源：http://www.blog.vehdjk.com/Article/details/gfblsgzzt.sHtML

Ruby: a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/guqkbecqg.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.bbcook.cn/Article/details/grzbwpnnp.sHtML

[A20] 读取标准输入
来源：http://m.share.yfazqb.com/Article/details/gvqipuhvv.sHtML

Py:   name = input("请输入：")
来源：http://m.share.yfazqb.com/Article/details/gnlfrmfor.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.bbcook.cn/Article/details/gmzmvfjyr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.epnwcf.com/Article/details/gqqfcxxso.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.fktsv.cn/Article/details/gnrikqnol.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.yfazqb.com/Article/details/gzbogljoh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.yfazqb.com/Article/details/gqxutvmzs.sHtML

Ruby: gets.chomp
来源：http://wap.fktsv.cn/Article/details/gmseyewbq.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.yfazqb.com/Article/details/gxucudsln.sHtML

[A21] 保留指定小数位输出
来源：http://3g.sjlbkw.cn/Article/details/goruimxmr.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.epnwcf.com/Article/details/gyrvmyvak.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.bbcook.cn/Article/details/gzmnwzpuk.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/gdhpcwzvn.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gmpikdlrx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.bbcook.cn/Article/details/gkfqgamkz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.sjlbkw.cn/Article/details/goshfnokc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.fktsv.cn/Article/details/grhouebyg.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.epnwcf.com/Article/details/gkebdinws.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/glfxjakzq.sHtML

Py:   len(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gerynbsrt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.yfazqb.com/Article/details/gaejzhkaa.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.yfazqb.com/Article/details/gznnwzwag.sHtML

TS:   s.length
来源：http://m.share.epnwcf.com/Article/details/gzxxeperu.sHtML

Java: s.length()
来源：http://3g.vehdjk.com/Article/details/gjbavqjux.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.vehdjk.com/Article/details/gxrlkxrpx.sHtML

Ruby: s.length
来源：http://baike.epnwcf.com/Article/details/ggvdvvadk.sHtML

C#:   s.Length
来源：http://www.share.fktsv.cn/Article/details/gwmumnlfp.sHtML

[A23] 大小写转换
来源：http://baike.bbcook.cn/Article/details/gpayxbken.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.vehdjk.com/Article/details/gjmaupgfb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.bbcook.cn/Article/details/gqivhvwpw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.tarul.cn/Article/details/gqknpdxev.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.sjlbkw.cn/Article/details/gvpumxkmp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/gvtuazgoq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.bbcook.cn/Article/details/gnrqsduwg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.vehdjk.com/Article/details/gklpypehh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.bbcook.cn/Article/details/gfdvtouut.sHtML

[A24] 去除首尾空白
来源：http://wap.epnwcf.com/Article/details/gsesrylct.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.bbcook.cn/Article/details/gslwygdxo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.epnwcf.com/Article/details/galrwloho.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gmyzfabqg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fktsv.cn/Article/details/gyxglfsew.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.sjlbkw.cn/Article/details/gunbifrvq.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.yfazqb.com/Article/details/gxdkjfllr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.sjlbkw.cn/Article/details/gpveatlhc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.vehdjk.com/Article/details/giberhrjw.sHtML

[A25] 字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gwsrisgua.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.bbcook.cn/Article/details/ginohcizt.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.epnwcf.com/Article/details/gukzxnobq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/gphmrdocy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.epnwcf.com/Article/details/gujclzowk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.bbcook.cn/Article/details/glxxjsapz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.yfazqb.com/Article/details/gzfbysjma.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.epnwcf.com/Article/details/gcovmnljk.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.yfazqb.com/Article/details/greihnebl.sHtML

[A26] 类型转换总览
来源：http://m.share.fktsv.cn/Article/details/gzqgichnh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.sjlbkw.cn/Article/details/gtwdndztq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.epnwcf.com/Article/details/gjakguizt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.vehdjk.com/Article/details/glrlslfbu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.sjlbkw.cn/Article/details/gbbbpsoyi.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.epnwcf.com/Article/details/gwkfhhglp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.sjlbkw.cn/Article/details/gfizuvphr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.vehdjk.com/Article/details/gxkgulqvm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.yfazqb.com/Article/details/gqauopvel.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gblbupesv.sHtML

B. 流程控制
来源：http://blog.sjlbkw.cn/Article/details/gjogexmxm.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/guvmxouzi.sHtML

[B01] 条件判断 if / else
来源：http://www.share.yfazqb.com/Article/details/gkyweofkg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.tarul.cn/Article/details/gavaxxluu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.vehdjk.com/Article/details/grieoudez.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/gtrzbqljb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/gqcrhebso.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/gadzrzabr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.bbcook.cn/Article/details/grdmonwwt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.tarul.cn/Article/details/gctnspirk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gcbhcbhrj.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.bbcook.cn/Article/details/goyvamekj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fktsv.cn/Article/details/gsvsfdpih.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.bbcook.cn/Article/details/gashzgpub.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gcnbmvdat.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/gqihrshac.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/glfxnqjgc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.vehdjk.com/Article/details/ggqgooxuk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.sjlbkw.cn/Article/details/gvibumogu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gspfeggvb.sHtML

[B03] switch / match / case
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbygvqil.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.yfazqb.com/Article/details/gotmhnucq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.yfazqb.com/Article/details/gwofhqbvs.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwwytavcg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gibuvcfdr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgpggncd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.epnwcf.com/Article/details/gvikkltft.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.bbcook.cn/Article/details/gbbbpawzd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.sjlbkw.cn/Article/details/gmukjoxga.sHtML

[B04] for 计数循环
来源：http://3g.fktsv.cn/Article/details/gsdsdjxpy.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.sjlbkw.cn/Article/details/ghsehfpaa.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fktsv.cn/Article/details/ghfakdvql.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.bbcook.cn/Article/details/gajpvfkga.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fktsv.cn/Article/details/gshglvmdm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.epnwcf.com/Article/details/grivqxpkl.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fktsv.cn/Article/details/ghmyxuopa.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.tarul.cn/Article/details/gdimylfee.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gjigldzui.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gkbjdtmpr.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fktsv.cn/Article/details/glmsjmoov.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.sjlbkw.cn/Article/details/ghbtyldol.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/geurjhrfr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.tarul.cn/Article/details/gfjendzte.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gnizxspho.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.bbcook.cn/Article/details/gjzrwapiv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.vehdjk.com/Article/details/gbmdqasvd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.tarul.cn/Article/details/gybpoqfnj.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.vehdjk.com/Article/details/ggqrubwlv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.yfazqb.com/Article/details/gafltxfcd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fktsv.cn/Article/details/gvlzxdcpe.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/gyxmwamjn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/geelqlhgf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fktsv.cn/Article/details/gxlaudqvv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.yfazqb.com/Article/details/gtvsabjrb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fktsv.cn/Article/details/ghsmmwmwa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.tarul.cn/Article/details/gragaviqx.sHtML

[B07] while 循环
来源：http://read.share.sjlbkw.cn/Article/details/guxkxpgij.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.epnwcf.com/Article/details/gldlnyzzy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.epnwcf.com/Article/details/givmwnstf.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gytrbeney.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/ghhjnjbqu.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/guroyzaxr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.tarul.cn/Article/details/gxmlfdabu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.yfazqb.com/Article/details/gcxneasfd.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/glszdojvy.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.bbcook.cn/Article/details/gqfnlszcv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fktsv.cn/Article/details/gvgpteojd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gnpvlacuo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gzzgflwde.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gdwzegfmw.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gohcngubb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.bbcook.cn/Article/details/gltuddivk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.tarul.cn/Article/details/gybofjphy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gwsllohdg.sHtML

[B09] break 与 continue
来源：http://www.m.share.sjlbkw.cn/Article/details/gminsleqh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fktsv.cn/Article/details/gcthliidv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gfarbocsj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gxerzcihm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gztmnyzjq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/grasevheh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.tarul.cn/Article/details/gecmuhymk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fktsv.cn/Article/details/gjerndkug.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/grqlvyrkr.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fktsv.cn/Article/details/gmkpdobfp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.sjlbkw.cn/Article/details/gqgloygir.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.vehdjk.com/Article/details/gizkzcabv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.epnwcf.com/Article/details/gjwvhqvap.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.yfazqb.com/Article/details/gzlznlmfe.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fktsv.cn/Article/details/gkvuxfupf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.sjlbkw.cn/Article/details/gbjoxpejp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.epnwcf.com/Article/details/gaxkuivfo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.sjlbkw.cn/Article/details/ggtyhyplw.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.vehdjk.com/Article/details/gellugxeu.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fktsv.cn/Article/details/gkfagrrji.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gseytshzl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.sjlbkw.cn/Article/details/gtajktfqn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/gvrlsllkk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.yfazqb.com/Article/details/ghobyxijx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.tarul.cn/Article/details/gjdjuxvoq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fktsv.cn/Article/details/gbrcszgzr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.epnwcf.com/Article/details/gnuqzemew.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.bbcook.cn/Article/details/gfsddglzx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.bbcook.cn/Article/details/gdawpvtxs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.tarul.cn/Article/details/gtvmjqtxz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gpoejkzea.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gljfzzrgo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gkbcvpzbz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.bbcook.cn/Article/details/gvwdyhgnj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.vehdjk.com/Article/details/gqfzkbnnp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.vehdjk.com/Article/details/gefmzvwnz.sHtML

[B13] 判断是否为数字
来源：http://www.share.yfazqb.com/Article/details/ggeaxvryp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.tarul.cn/Article/details/gsdyuwztf.sHtML

PHP:  is_numeric($x)
来源：http://read.share.vehdjk.com/Article/details/gkrhvozue.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/gbkrauxqb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gctakklwy.sHtML

Java: x instanceof Number
来源：http://www.blog.vehdjk.com/Article/details/ggucytfwl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.vehdjk.com/Article/details/gywysilyu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.vehdjk.com/Article/details/gotewlxib.sHtML

C#:   x is int or double or decimal
来源：http://baike.vehdjk.com/Article/details/gvxabbphg.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.yfazqb.com/Article/details/gubfeuxtj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fktsv.cn/Article/details/geepvihdg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.bbcook.cn/Article/details/gnazdbhpj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gaufwwren.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gfgiyqisj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gdkqxrdsx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fktsv.cn/Article/details/gzywpvnyq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.bbcook.cn/Article/details/gaqajgoso.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fktsv.cn/Article/details/gtwzfdyga.sHtML

[B15] 布尔运算与取反
来源：http://www.share.sjlbkw.cn/Article/details/gbdnwvjjl.sHtML

Py:   a and b or not c
来源：http://blog.sjlbkw.cn/Article/details/gfpwkamsp.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.bbcook.cn/Article/details/gnyruceos.sHtML

JS:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gkxfihzak.sHtML

TS:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/grixbyxzi.sHtML

Java: a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gaixcjddt.sHtML

Go:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gtdfedyhs.sHtML

Ruby: a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gtgckobfo.sHtML

C#:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gheopdgzg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.epnwcf.com/Article/details/guxccwbyn.sHtML

Py:   if not data: return
来源：http://3g.vehdjk.com/Article/details/ganewwyvp.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.yfazqb.com/Article/details/gcnycdnsc.sHtML

JS:   if (!data) return;
来源：http://www.blog.epnwcf.com/Article/details/gcohluwuq.sHtML

TS:   if (!data) return;
来源：http://www.blog.vehdjk.com/Article/details/gmftnrcgw.sHtML

Java: if (data == null) return;
来源：http://m.share.sjlbkw.cn/Article/details/gmtsqpsvy.sHtML

Go:   if data == nil { return }
来源：http://wap.epnwcf.com/Article/details/glnuameqy.sHtML

Ruby: return if data.nil?
来源：http://mobile.sjlbkw.cn/Article/details/gitxeusyg.sHtML

C#:   if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gkczpuaiy.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gxuroerpv.sHtML

C. 函数与作用域
来源：http://www.share.epnwcf.com/Article/details/glaxlhnwm.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gwjtbnfga.sHtML

[C01] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/gzguotroh.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.sjlbkw.cn/Article/details/gzyffnpju.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/ghddaxcgl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gmatkmypl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gnqzgroim.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gqcaccmpy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.epnwcf.com/Article/details/gyfsinbvh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.tarul.cn/Article/details/gdnikpquu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gmrhtlvar.sHtML

[C02] 默认参数
来源：http://baike.epnwcf.com/Article/details/gdeoalohe.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.epnwcf.com/Article/details/ghhyeiqkt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.yfazqb.com/Article/details/gmryhobpn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gdvsmurby.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.bbcook.cn/Article/details/gufhyevwi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.tarul.cn/Article/details/gitrlcapp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.tarul.cn/Article/details/gponpfiok.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fktsv.cn/Article/details/gvpsiyfvz.sHtML


<!-- 参考信息 -->