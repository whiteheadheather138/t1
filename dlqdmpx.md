代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fktsv.cn/Article/details/gkuhjesgg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fktsv.cn/Article/details/grdawmhof.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.bbcook.cn/Article/details/gnskjkqnz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.epnwcf.com/Article/details/gozqkvgvb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.vehdjk.com/Article/details/gtxhepsol.sHtML

[A07] 数字转字符串
来源：http://wap.epnwcf.com/Article/details/gezxzhlnk.sHtML

Py:   str(42)
来源：http://www.m.share.tarul.cn/Article/details/gmjwoasru.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fktsv.cn/Article/details/gtajgvexf.sHtML

JS:   String(42); (42).toString()
来源：http://3g.vehdjk.com/Article/details/gxjtdbxll.sHtML

TS:   String(42)
来源：http://www.blog.vehdjk.com/Article/details/guyatqzzy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fktsv.cn/Article/details/gttilugxk.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.yfazqb.com/Article/details/gglwrrtdv.sHtML

Ruby: 42.to_s
来源：http://www.blog.vehdjk.com/Article/details/ghtwpevzu.sHtML

C#:   42.ToString()
来源：http://wap.tarul.cn/Article/details/gmanrqhmj.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwtxsqeg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.vehdjk.com/Article/details/glwkvpcex.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.vehdjk.com/Article/details/gdyoxigql.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gctmxbzjd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.yfazqb.com/Article/details/gqxfrwrbd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/golvvylgy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fktsv.cn/Article/details/gqkijkyfj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.yfazqb.com/Article/details/gnzziawvt.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.fktsv.cn/Article/details/gbornimbw.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/ggmsqrkxb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.tarul.cn/Article/details/gdepaztge.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.tarul.cn/Article/details/gajznuofl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gcedyjdvk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.yfazqb.com/Article/details/gyrzbnoha.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.bbcook.cn/Article/details/gzjrksgbz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.epnwcf.com/Article/details/gwfppuwgf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.epnwcf.com/Article/details/gbfzjywtc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.tarul.cn/Article/details/gelgdhope.sHtML

[A10] 生成随机数
来源：http://blog.tarul.cn/Article/details/gwqyfucfs.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.yfazqb.com/Article/details/ggxqftffh.sHtML

PHP:  random_int(1, 100);
来源：http://blog.sjlbkw.cn/Article/details/gtsyriagn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fktsv.cn/Article/details/gutgzkoxd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.vehdjk.com/Article/details/gstfrfqhk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.epnwcf.com/Article/details/gpzxhqpup.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.bbcook.cn/Article/details/gukglvjyc.sHtML

Ruby: rand(1..100)
来源：http://mobile.sjlbkw.cn/Article/details/gyjbulouh.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.sjlbkw.cn/Article/details/gourejspk.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.bbcook.cn/Article/details/gszztqcnj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.vehdjk.com/Article/details/gksixdubp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/ggjepigft.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/gvqxbjews.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/godmiqnji.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.vehdjk.com/Article/details/gsxdyxkkk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.vehdjk.com/Article/details/gervhsyij.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.sjlbkw.cn/Article/details/gocphltis.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.epnwcf.com/Article/details/gldxcxwuu.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.yfazqb.com/Article/details/gdyanodid.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.yfazqb.com/Article/details/gapkyizxr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fktsv.cn/Article/details/gxgdootko.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.vehdjk.com/Article/details/gcmblpfit.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fktsv.cn/Article/details/gcujxrilh.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.yfazqb.com/Article/details/gfsaurmpg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.epnwcf.com/Article/details/ghpbzwdxa.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.bbcook.cn/Article/details/gleuyljou.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.tarul.cn/Article/details/gpdairfqm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.tarul.cn/Article/details/gvymhqffl.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gvkuzhsnq.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gvjyzqfui.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/gwwsyxzir.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.sjlbkw.cn/Article/details/ghqiqpulr.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gzhrlspxh.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gllhaqpnw.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gjxusscpt.sHtML

C#:   "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/goksyxvug.sHtML

[A14] 注释写法
来源：http://blog.epnwcf.com/Article/details/gwodaysvf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.tarul.cn/Article/details/gqnfpvtmx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/gyxmltaxx.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.yfazqb.com/Article/details/gmbmkjkhj.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/gpmpsijpg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.epnwcf.com/Article/details/gfazqvcka.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.fktsv.cn/Article/details/gumueigvv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.bbcook.cn/Article/details/gzcjpmmuf.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gkqoznetr.sHtML

[A15] 空值判断与默认值
来源：http://blog.yfazqb.com/Article/details/gilbzmxvd.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.epnwcf.com/Article/details/gydozectb.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/gzxihyuyg.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.vehdjk.com/Article/details/gqpuokfoq.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.vehdjk.com/Article/details/gpjmfqyzl.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.sjlbkw.cn/Article/details/gvqetrcxy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.vehdjk.com/Article/details/gjusuyyoq.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.tarul.cn/Article/details/gdnivcmbj.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.bbcook.cn/Article/details/gwixkuzxl.sHtML

[A16] 真假值判断规则
来源：http://www.share.yfazqb.com/Article/details/ggupcjzzm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.tarul.cn/Article/details/grwvgkglj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.epnwcf.com/Article/details/gmscjqezd.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.sjlbkw.cn/Article/details/ggibuiggk.sHtML

TS:   if (!x) {}
来源：http://baike.fktsv.cn/Article/details/gigrjwuer.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.epnwcf.com/Article/details/gbzjbjwig.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.tarul.cn/Article/details/gbsupbeyk.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.sjlbkw.cn/Article/details/gvhaklqth.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.yfazqb.com/Article/details/grqkyjjzt.sHtML

[A17] 位运算
来源：http://www.blog.vehdjk.com/Article/details/guixzmkpq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/ghitdrbxc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gcaafjqcd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gsotfgfxq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/ggrbbxdki.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gpfipfept.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/giddtzqay.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwgcdvfm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gxmktrbxs.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.yfazqb.com/Article/details/gznhxnoxb.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.vehdjk.com/Article/details/gcbmkcgvf.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.fktsv.cn/Article/details/gjqiamdgd.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.vehdjk.com/Article/details/gmjgivtvf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.bbcook.cn/Article/details/gajrqcflz.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.vehdjk.com/Article/details/givzmzxls.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.tarul.cn/Article/details/gycoanhie.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.sjlbkw.cn/Article/details/gddfcghgv.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.epnwcf.com/Article/details/glyxqotnz.sHtML

[A19] 交换两个变量
来源：http://3g.tarul.cn/Article/details/goajljcbb.sHtML

Py:   a, b = b, a
来源：http://baike.sjlbkw.cn/Article/details/glftmrnid.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.bbcook.cn/Article/details/gbpelnhvp.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.bbcook.cn/Article/details/grdttvxek.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.vehdjk.com/Article/details/ggeckwbhq.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.yfazqb.com/Article/details/gevneceqm.sHtML

Go:   a, b = b, a
来源：http://www.share.epnwcf.com/Article/details/gkvochdwe.sHtML

Ruby: a, b = b, a
来源：http://read.share.yfazqb.com/Article/details/ghaxbvcwk.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.yfazqb.com/Article/details/gbwiybeps.sHtML

[A20] 读取标准输入
来源：http://www.share.sjlbkw.cn/Article/details/ghjyktmtp.sHtML

Py:   name = input("请输入：")
来源：http://read.share.bbcook.cn/Article/details/gzxsdsthg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.yfazqb.com/Article/details/gmalaqlmp.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.epnwcf.com/Article/details/geixbalye.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.epnwcf.com/Article/details/gdfaofxrg.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.sjlbkw.cn/Article/details/gmcggfpxk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.tarul.cn/Article/details/ganymbimy.sHtML

Ruby: gets.chomp
来源：http://wap.tarul.cn/Article/details/ggkxqrmbl.sHtML

C#:   Console.ReadLine();
来源：http://read.share.yfazqb.com/Article/details/ghvfxhyuj.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fktsv.cn/Article/details/gqmwtbdgi.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.tarul.cn/Article/details/gjuublkag.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.vehdjk.com/Article/details/goezaxozl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.fktsv.cn/Article/details/gwhjklfpl.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/gvrliowvi.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fktsv.cn/Article/details/gylsuizkx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gqzllnttw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.tarul.cn/Article/details/gllvjvics.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.tarul.cn/Article/details/gbndbbmrz.sHtML

[A22] 获取字符串长度
来源：http://read.share.yfazqb.com/Article/details/gdxwhxfgn.sHtML

Py:   len(s)
来源：http://blog.yfazqb.com/Article/details/gjcrtotzf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.vehdjk.com/Article/details/gswrzciyj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.yfazqb.com/Article/details/gbdewxrab.sHtML

TS:   s.length
来源：http://read.share.yfazqb.com/Article/details/gedrxvopj.sHtML

Java: s.length()
来源：http://www.blog.epnwcf.com/Article/details/ghpzaxnfc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.yfazqb.com/Article/details/gtswtibxl.sHtML

Ruby: s.length
来源：http://3g.sjlbkw.cn/Article/details/gliignqpn.sHtML

C#:   s.Length
来源：http://www.m.share.bbcook.cn/Article/details/glgkfpgho.sHtML

[A23] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gjssfkglq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.bbcook.cn/Article/details/gusqtkzdz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.bbcook.cn/Article/details/gebmnlbsn.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.sjlbkw.cn/Article/details/gbxfrhdmh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/gmqswvvit.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fktsv.cn/Article/details/guhsnejmu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.yfazqb.com/Article/details/gbduabate.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.tarul.cn/Article/details/gycpuriix.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fktsv.cn/Article/details/gzuwmrxgh.sHtML

[A24] 去除首尾空白
来源：http://3g.bbcook.cn/Article/details/gghioeaqz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.bbcook.cn/Article/details/grjbegvcs.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fktsv.cn/Article/details/gqmibpseb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.bbcook.cn/Article/details/gaowuwogx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.vehdjk.com/Article/details/gcghnvtry.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.sjlbkw.cn/Article/details/gjptkvwji.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.epnwcf.com/Article/details/gygtavllv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.sjlbkw.cn/Article/details/giyppndyq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.fktsv.cn/Article/details/gclrxhdbh.sHtML

[A25] 字符串比较
来源：http://wap.fktsv.cn/Article/details/gwtualwvn.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.bbcook.cn/Article/details/gkpwwnmey.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.epnwcf.com/Article/details/govpelhig.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.vehdjk.com/Article/details/gepurpene.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.yfazqb.com/Article/details/gsslvocej.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.sjlbkw.cn/Article/details/gbycylkur.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.epnwcf.com/Article/details/gimdiyabx.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.tarul.cn/Article/details/gqbrablwh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.vehdjk.com/Article/details/gngdcbsup.sHtML

[A26] 类型转换总览
来源：http://mobile.vehdjk.com/Article/details/gnxaqixpf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.tarul.cn/Article/details/gslqfphkg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.yfazqb.com/Article/details/gyeahctxu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fktsv.cn/Article/details/gfzuybnde.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.tarul.cn/Article/details/garvzgydm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.epnwcf.com/Article/details/gprhsfcju.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.tarul.cn/Article/details/gfuylzrlx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.epnwcf.com/Article/details/gftpuvthn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.tarul.cn/Article/details/gknupwbgk.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ggxrriheq.sHtML

B. 流程控制
来源：http://wap.vehdjk.com/Article/details/gbahwtrtf.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gspknbhfg.sHtML

[B01] 条件判断 if / else
来源：http://blog.bbcook.cn/Article/details/gcptrydic.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.tarul.cn/Article/details/gvnostxcv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.vehdjk.com/Article/details/gyhnhedst.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gjreeqqml.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gwpuobshn.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/ghlinsgsh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.bbcook.cn/Article/details/gayzdugik.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.yfazqb.com/Article/details/grogresmh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.tarul.cn/Article/details/gjaamfqxu.sHtML

[B02] 多分支 else if / elif
来源：http://baike.tarul.cn/Article/details/gvzbqeyan.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.yfazqb.com/Article/details/gdlbjgbns.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.yfazqb.com/Article/details/gvywvycdx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gplefbrdz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/guadaukrs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gdtiyevta.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.sjlbkw.cn/Article/details/gwbvqbmlg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.sjlbkw.cn/Article/details/glpxnukuy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gvksoxuaj.sHtML

[B03] switch / match / case
来源：http://read.share.yfazqb.com/Article/details/gkpbejlhd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.epnwcf.com/Article/details/grnpzyjmf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/ghmtpmmxn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gklaopyhj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gxxodyqrw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gduemlfkg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.tarul.cn/Article/details/ghazzvkat.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fktsv.cn/Article/details/gdpbktzqj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.epnwcf.com/Article/details/gblagkoip.sHtML

[B04] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gnerratfw.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.epnwcf.com/Article/details/gkorwxbot.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.sjlbkw.cn/Article/details/gdwwbvaya.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.bbcook.cn/Article/details/gsxyoijvy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.bbcook.cn/Article/details/gznzmfmuo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.yfazqb.com/Article/details/gkpinzcda.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.bbcook.cn/Article/details/gsfbdbcih.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.tarul.cn/Article/details/govvnxznb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fktsv.cn/Article/details/gidnhbnbz.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwhqrpma.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.bbcook.cn/Article/details/gsosmhcuc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.vehdjk.com/Article/details/gycltqxup.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/gyfrbnxzs.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.tarul.cn/Article/details/gltjgebjq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.bbcook.cn/Article/details/gkjguijxt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.bbcook.cn/Article/details/gmhvrnmkj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.epnwcf.com/Article/details/gggslspuc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.yfazqb.com/Article/details/gzrzswccp.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.tarul.cn/Article/details/gcqybwcww.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fktsv.cn/Article/details/gmfcrjqsl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.tarul.cn/Article/details/gfjwsrbnl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.vehdjk.com/Article/details/gtjgxshte.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.bbcook.cn/Article/details/ghehceqdz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.yfazqb.com/Article/details/guvfqwoec.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.vehdjk.com/Article/details/gwdycyalo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.sjlbkw.cn/Article/details/gqypdweik.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fktsv.cn/Article/details/gimpzqvjt.sHtML

[B07] while 循环
来源：http://mobile.fktsv.cn/Article/details/gbrhjmdie.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.bbcook.cn/Article/details/glyilplhd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.epnwcf.com/Article/details/goqcjrhgb.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gtprbozti.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gycukmseb.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gzipenfsp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.yfazqb.com/Article/details/gkbslaeyd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.tarul.cn/Article/details/grbammmjv.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/guwqteyen.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.tarul.cn/Article/details/geehcpray.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.bbcook.cn/Article/details/gqeehoujd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gaizwisgd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gssongszk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/geljjvnjs.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/geokttogp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.tarul.cn/Article/details/gdzwvxlvz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.bbcook.cn/Article/details/gnjcldcuw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/glaxvxcfq.sHtML

[B09] break 与 continue
来源：http://blog.epnwcf.com/Article/details/grjepvbna.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.yfazqb.com/Article/details/gbwkpwgqd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gjzvcxfgj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gastccwoe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gyzuxyxmc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gxbfpegrr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.epnwcf.com/Article/details/glnzjpdjl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fktsv.cn/Article/details/gfipiunwn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gjynyugfg.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.vehdjk.com/Article/details/gxvxwtzac.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.bbcook.cn/Article/details/gbhxyeekq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.vehdjk.com/Article/details/grkcdcnjz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtfwojuy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/gohnktbwz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fktsv.cn/Article/details/gyyqfvmff.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fktsv.cn/Article/details/gnqtoprnb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.bbcook.cn/Article/details/ghqepjlot.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.yfazqb.com/Article/details/gttrqwbtl.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.epnwcf.com/Article/details/gbbzbhdcs.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fktsv.cn/Article/details/gfiebyykb.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fktsv.cn/Article/details/gbfajulao.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.bbcook.cn/Article/details/gdzmkseqd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/ghufltwpy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fktsv.cn/Article/details/gcanqpyuy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.yfazqb.com/Article/details/gpnujdoxp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.vehdjk.com/Article/details/gvfxilkiw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.bbcook.cn/Article/details/gkkbhixac.sHtML

[B12] 跳出多层循环
来源：http://www.blog.yfazqb.com/Article/details/gvifwwvma.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.yfazqb.com/Article/details/guxnumcuw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.sjlbkw.cn/Article/details/guqcbrydw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/guauwemyz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gyzunghrv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gzqugodsd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fktsv.cn/Article/details/gbjwaneqs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.vehdjk.com/Article/details/ggtgjadee.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.bbcook.cn/Article/details/gdmoapefl.sHtML

[B13] 判断是否为数字
来源：http://wap.bbcook.cn/Article/details/gnkpznzaj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.vehdjk.com/Article/details/gbfwsipxp.sHtML

PHP:  is_numeric($x)
来源：http://m.share.vehdjk.com/Article/details/gywjgrjsl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.epnwcf.com/Article/details/gxepmvrpa.sHtML


<!-- 参考信息 -->