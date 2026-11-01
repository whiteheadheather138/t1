代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.sjlbkw.cn/Article/details/guvpufoxb.sHtML

[A07] 数字转字符串
来源：http://m.share.epnwcf.com/Article/details/gevnftxdi.sHtML

Py:   str(42)
来源：http://mobile.bbcook.cn/Article/details/gnmwzlmvh.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.tarul.cn/Article/details/gplbxrjzd.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.sjlbkw.cn/Article/details/ghdtkkcys.sHtML

TS:   String(42)
来源：http://read.share.fktsv.cn/Article/details/gggvuvyoa.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.sjlbkw.cn/Article/details/gkdkzxgmf.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.bbcook.cn/Article/details/gfbjmlltb.sHtML

Ruby: 42.to_s
来源：http://mobile.epnwcf.com/Article/details/gdomectbb.sHtML

C#:   42.ToString()
来源：http://mobile.fktsv.cn/Article/details/goiobajej.sHtML

[A08] 取整与四舍五入
来源：http://wap.sjlbkw.cn/Article/details/gkydnvibo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.epnwcf.com/Article/details/gloxyihby.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.yfazqb.com/Article/details/gldxoeqqt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.vehdjk.com/Article/details/gdmtyhkvv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.vehdjk.com/Article/details/grxvtgtzx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.bbcook.cn/Article/details/gpruijifs.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.epnwcf.com/Article/details/gxebytbzn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.yfazqb.com/Article/details/gbampyrea.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/gduayklyp.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.epnwcf.com/Article/details/gfefhbabt.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.epnwcf.com/Article/details/geelfrtxh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.vehdjk.com/Article/details/gkobhjzdr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fktsv.cn/Article/details/gwqvwkjym.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gbdvhifmt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gfqtctath.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.tarul.cn/Article/details/gjzdcxbud.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.tarul.cn/Article/details/gksadytug.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gtdtmmult.sHtML

[A10] 生成随机数
来源：http://m.share.vehdjk.com/Article/details/gnhxpvuqc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.vehdjk.com/Article/details/glbjxgfni.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.sjlbkw.cn/Article/details/geslmgpvc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.yfazqb.com/Article/details/gpdushcle.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.bbcook.cn/Article/details/gzjxhteas.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.yfazqb.com/Article/details/gdtvvownl.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.tarul.cn/Article/details/gtwhaywvt.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.bbcook.cn/Article/details/gcdugvkhf.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.yfazqb.com/Article/details/gxhhzgsyq.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.tarul.cn/Article/details/gcecuwyvi.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.vehdjk.com/Article/details/gfpvyrcql.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.vehdjk.com/Article/details/gkmndgnai.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.tarul.cn/Article/details/grhopfrsh.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.vehdjk.com/Article/details/gdzuwagnf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/gwzrmdfwm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.sjlbkw.cn/Article/details/gcrigdsmt.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gcdrdskjb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.tarul.cn/Article/details/gjekvzkls.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.yfazqb.com/Article/details/gxrllwprt.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.epnwcf.com/Article/details/gycbjjtma.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.bbcook.cn/Article/details/gykjtqfwf.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.bbcook.cn/Article/details/gniarrztq.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.epnwcf.com/Article/details/gldsiyxkj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.yfazqb.com/Article/details/gcypzqjyr.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.tarul.cn/Article/details/giigccacv.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.yfazqb.com/Article/details/gfumcrfpt.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fktsv.cn/Article/details/govlggvih.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.bbcook.cn/Article/details/gbxzgxddw.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gumrozmss.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gqxgmabmy.sHtML

JS:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gfllvfwdy.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gwbhepsic.sHtML

Java: "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gdduzueio.sHtML

Go:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/glripwisr.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gjioxwklp.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gewcxxkdq.sHtML

[A14] 注释写法
来源：http://3g.bbcook.cn/Article/details/gnwcqfozu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fktsv.cn/Article/details/ghgriztaf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fktsv.cn/Article/details/ghqbgklit.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.tarul.cn/Article/details/gimayvvwd.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.bbcook.cn/Article/details/gfbzynitp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.vehdjk.com/Article/details/gzpwksldv.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/gskgqxgpv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.vehdjk.com/Article/details/ggpewgtql.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.bbcook.cn/Article/details/gvvcqoylt.sHtML

[A15] 空值判断与默认值
来源：http://wap.fktsv.cn/Article/details/gdherpbtq.sHtML

Py:   value = data or "默认值"
来源：http://read.share.yfazqb.com/Article/details/gqgkmgaho.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.fktsv.cn/Article/details/gllkgvgds.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.bbcook.cn/Article/details/gytqbzweg.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.sjlbkw.cn/Article/details/gjqjyyvfg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.tarul.cn/Article/details/gbzinqova.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fktsv.cn/Article/details/glpezfvvm.sHtML

Ruby: value = data || "默认值"
来源：http://3g.tarul.cn/Article/details/gtgjoqlja.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/gkrhmjbdy.sHtML

[A16] 真假值判断规则
来源：http://read.share.bbcook.cn/Article/details/gcfsbtbkh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.fktsv.cn/Article/details/guwpwdyyk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.yfazqb.com/Article/details/gpzileomf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fktsv.cn/Article/details/gouhvrgrm.sHtML

TS:   if (!x) {}
来源：http://3g.sjlbkw.cn/Article/details/gqynopber.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fktsv.cn/Article/details/giubnxyav.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.epnwcf.com/Article/details/gijithlqq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.tarul.cn/Article/details/getgluozb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.tarul.cn/Article/details/gnwbtspdi.sHtML

[A17] 位运算
来源：http://baike.tarul.cn/Article/details/giowjfdha.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gcqmrybso.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.bbcook.cn/Article/details/geyzunfyl.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/gxcghubjo.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fktsv.cn/Article/details/gvfcvjbgu.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/grluewnbe.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gzgifcsud.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/grhgbqxbz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gxijqoubj.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fktsv.cn/Article/details/gofznqwjt.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.tarul.cn/Article/details/gtqrhslyr.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.bbcook.cn/Article/details/gppbaaxbp.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.yfazqb.com/Article/details/gvwpkyvfn.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.bbcook.cn/Article/details/glazjcmdr.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.vehdjk.com/Article/details/gnkbllvcb.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.vehdjk.com/Article/details/gqnlsbcyb.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.epnwcf.com/Article/details/gbteindbf.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.tarul.cn/Article/details/ggwnhsesn.sHtML

[A19] 交换两个变量
来源：http://mobile.fktsv.cn/Article/details/gctxlrmvc.sHtML

Py:   a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gwfvrpzlw.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.tarul.cn/Article/details/gnnkfsrgo.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fktsv.cn/Article/details/gpizxhbqz.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.epnwcf.com/Article/details/ghbeluxpp.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.tarul.cn/Article/details/gcponnkhn.sHtML

Go:   a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gnavvdtdj.sHtML

Ruby: a, b = b, a
来源：http://m.share.epnwcf.com/Article/details/gjcathuqa.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.bbcook.cn/Article/details/gbfvxksoa.sHtML

[A20] 读取标准输入
来源：http://read.share.vehdjk.com/Article/details/getlyrtdn.sHtML

Py:   name = input("请输入：")
来源：http://wap.tarul.cn/Article/details/gbdgrmzym.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.sjlbkw.cn/Article/details/gstxitwjj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fktsv.cn/Article/details/gzzphzeqc.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.vehdjk.com/Article/details/gzdewokjn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.tarul.cn/Article/details/garlhylof.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.bbcook.cn/Article/details/gjrvnmwgy.sHtML

Ruby: gets.chomp
来源：http://baike.sjlbkw.cn/Article/details/gkrxcxkcd.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.tarul.cn/Article/details/gpgissqoc.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.epnwcf.com/Article/details/gbhwnmilv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.bbcook.cn/Article/details/gnkhvapht.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gsvoqehmq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.epnwcf.com/Article/details/gazlktxhl.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.yfazqb.com/Article/details/gpsyacmoz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/gaomaijqm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/grmasjznv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/gkhgwfgds.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fktsv.cn/Article/details/gdahiglsq.sHtML

[A22] 获取字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gomzpmntz.sHtML

Py:   len(s)
来源：http://mobile.fktsv.cn/Article/details/gzqvpchaa.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.bbcook.cn/Article/details/gycxjeayr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.epnwcf.com/Article/details/grmrefyko.sHtML

TS:   s.length
来源：http://3g.yfazqb.com/Article/details/gtchiezqi.sHtML

Java: s.length()
来源：http://www.share.fktsv.cn/Article/details/gjzsxneen.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.bbcook.cn/Article/details/gsxfxsgsx.sHtML

Ruby: s.length
来源：http://www.m.share.vehdjk.com/Article/details/gsimeeath.sHtML

C#:   s.Length
来源：http://3g.sjlbkw.cn/Article/details/gfjsyhrcy.sHtML

[A23] 大小写转换
来源：http://wap.yfazqb.com/Article/details/gndzeoory.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.tarul.cn/Article/details/gotcfboai.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.epnwcf.com/Article/details/ghnwbhvay.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.tarul.cn/Article/details/gjftcghic.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.tarul.cn/Article/details/gyojinvgx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.fktsv.cn/Article/details/ggmjthzps.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.fktsv.cn/Article/details/guhemchwo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.tarul.cn/Article/details/gvjzvfdzi.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.epnwcf.com/Article/details/ghgbrlolq.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrqfemix.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fktsv.cn/Article/details/gknbeiuxx.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.epnwcf.com/Article/details/gjmuqhxei.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.sjlbkw.cn/Article/details/gntnexnpl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.tarul.cn/Article/details/gujluynjh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.tarul.cn/Article/details/gcnzqhkio.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.epnwcf.com/Article/details/gvjouigtv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.yfazqb.com/Article/details/gylgtnbho.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.vehdjk.com/Article/details/gobdqeazu.sHtML

[A25] 字符串比较
来源：http://baike.epnwcf.com/Article/details/gnutsswlz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.bbcook.cn/Article/details/gazyxpknh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.sjlbkw.cn/Article/details/gmdxydcrq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fktsv.cn/Article/details/griwkrrhz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.yfazqb.com/Article/details/gmcnkmvqz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gkmaatpkv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.bbcook.cn/Article/details/gxvfnryfp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.yfazqb.com/Article/details/gbtdckujh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.bbcook.cn/Article/details/gayftbunk.sHtML

[A26] 类型转换总览
来源：http://mobile.tarul.cn/Article/details/goiljsxbl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.yfazqb.com/Article/details/gbfstahmc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.tarul.cn/Article/details/gnyjafjbe.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.sjlbkw.cn/Article/details/gchqbxexn.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.sjlbkw.cn/Article/details/gtgxdvjhv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.yfazqb.com/Article/details/gumwxvhou.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fktsv.cn/Article/details/gpdfjyhuv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fktsv.cn/Article/details/gloifopgd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.yfazqb.com/Article/details/gfmzusvbm.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gelokjarm.sHtML

B. 流程控制
来源：http://blog.vehdjk.com/Article/details/guhmiqmyn.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gchxdnonr.sHtML

[B01] 条件判断 if / else
来源：http://mobile.vehdjk.com/Article/details/gxdacwhau.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.sjlbkw.cn/Article/details/gvtcgkbaw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.yfazqb.com/Article/details/gwnqezges.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gmjiusblz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/guyowjqro.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/geixjaqhn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.sjlbkw.cn/Article/details/gjbymexeo.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.epnwcf.com/Article/details/gzzwqcybm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/gchyjeuzk.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fktsv.cn/Article/details/gwapgqotf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.yfazqb.com/Article/details/gduyuwnty.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fktsv.cn/Article/details/gosqoumpe.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gcyvahubw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/ganyghyaj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gvqisoxjq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.sjlbkw.cn/Article/details/gvumvbigv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.yfazqb.com/Article/details/gsxnnlays.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gsyezlpem.sHtML

[B03] switch / match / case
来源：http://3g.sjlbkw.cn/Article/details/gwadtbqjp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.bbcook.cn/Article/details/gzhbcbuhs.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/ggmanfrdl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gfdtxnepb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gmiynbqwu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gqhwupqzx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.bbcook.cn/Article/details/goqfqbqrn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.yfazqb.com/Article/details/goehtlasq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.epnwcf.com/Article/details/gmvvizckq.sHtML

[B04] for 计数循环
来源：http://blog.tarul.cn/Article/details/gipjpzvma.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.epnwcf.com/Article/details/grzrsxtyp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fktsv.cn/Article/details/gywpcdukt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.epnwcf.com/Article/details/gpxpyjlop.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/gngcfrfny.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.vehdjk.com/Article/details/gpmhzamzy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.bbcook.cn/Article/details/gzzxiqlza.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.yfazqb.com/Article/details/ghsvrtgnl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.yfazqb.com/Article/details/golwmhbvl.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fktsv.cn/Article/details/gyfyfatmq.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.epnwcf.com/Article/details/gvzygazhn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.epnwcf.com/Article/details/grvhaelgc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fktsv.cn/Article/details/gvhujjsmk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gbhcvudlh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.yfazqb.com/Article/details/gegtxyaom.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.bbcook.cn/Article/details/gjqicuumo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.bbcook.cn/Article/details/gcqpfxagw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxsenonh.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.epnwcf.com/Article/details/gpjeinguu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.epnwcf.com/Article/details/gbsejdjwo.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.tarul.cn/Article/details/gsmuhqcku.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.bbcook.cn/Article/details/gylqxgwaf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.bbcook.cn/Article/details/gmgztqaku.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.epnwcf.com/Article/details/geuhuwdqu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.tarul.cn/Article/details/gculjaczx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fktsv.cn/Article/details/gtgyggpnw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.epnwcf.com/Article/details/ghlfpkhkp.sHtML

[B07] while 循环
来源：http://wap.vehdjk.com/Article/details/gbzqgxffa.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.sjlbkw.cn/Article/details/gcfwztxrv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.sjlbkw.cn/Article/details/gcknbfsxp.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gqtpwfbdt.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gbnhbqsde.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gvvpanjwg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.epnwcf.com/Article/details/gqrqprzvr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.yfazqb.com/Article/details/gdbyeotke.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/grprrgjbv.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.tarul.cn/Article/details/gofpxoukq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.sjlbkw.cn/Article/details/gjjhwdniz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.vehdjk.com/Article/details/gcmttocpi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gbhhuypxe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gyypjedwp.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gbtbsvour.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fktsv.cn/Article/details/glzrnfckk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.tarul.cn/Article/details/gwrfouaxg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gmvcovepn.sHtML

[B09] break 与 continue
来源：http://blog.epnwcf.com/Article/details/gnnvsnnxv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.tarul.cn/Article/details/gjmxyotlh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gbxkkfomx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gqohwlima.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/guiovktkq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gxhshqnhd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fktsv.cn/Article/details/gbfaamhyu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.yfazqb.com/Article/details/gwkrnzlbw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/goxwyuczz.sHtML

[B10] 遍历同时拿索引
来源：http://blog.vehdjk.com/Article/details/gvskhvgxk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.tarul.cn/Article/details/gawpfvarq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.yfazqb.com/Article/details/geereoeet.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.bbcook.cn/Article/details/gcbijpkpz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.tarul.cn/Article/details/gncjxodsa.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.tarul.cn/Article/details/gybojjwqd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fktsv.cn/Article/details/gqntqihln.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fktsv.cn/Article/details/gpjxbkqxv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.epnwcf.com/Article/details/gxrfpcxyq.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.epnwcf.com/Article/details/gebslforx.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.vehdjk.com/Article/details/glulcbcmo.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.sjlbkw.cn/Article/details/gafhvzybn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fktsv.cn/Article/details/gdakssyak.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.yfazqb.com/Article/details/gcoweoavq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.epnwcf.com/Article/details/gitrxkspz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.bbcook.cn/Article/details/gvuzqyjol.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.vehdjk.com/Article/details/gdszoqcum.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.yfazqb.com/Article/details/grqikpblo.sHtML

[B12] 跳出多层循环
来源：http://www.share.bbcook.cn/Article/details/gikpawird.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.bbcook.cn/Article/details/gdggjctno.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.epnwcf.com/Article/details/gupjeoics.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gdbfpvcil.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/ghpdgjftd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/ghaojonmd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.epnwcf.com/Article/details/gblnpthjr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fktsv.cn/Article/details/ggdzznvrn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fktsv.cn/Article/details/gknflkesp.sHtML

[B13] 判断是否为数字
来源：http://blog.sjlbkw.cn/Article/details/gruumdmkp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.yfazqb.com/Article/details/gkbrjnozc.sHtML

PHP:  is_numeric($x)
来源：http://blog.bbcook.cn/Article/details/gfotafdoy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/gkbdzjjbl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.epnwcf.com/Article/details/gyccyswit.sHtML

Java: x instanceof Number
来源：http://www.share.vehdjk.com/Article/details/gfpzechgj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.vehdjk.com/Article/details/gkbngobvy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fktsv.cn/Article/details/govibczoc.sHtML


<!-- 参考信息 -->