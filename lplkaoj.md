代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://blog.bbcook.cn/Article/details/gykjhttuf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.bbcook.cn/Article/details/gyblcwagh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.epnwcf.com/Article/details/gmircztuy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.sjlbkw.cn/Article/details/gsyjcyxyd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.epnwcf.com/Article/details/gnntexbkd.sHtML

[A07] 数字转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gphbhmgtl.sHtML

Py:   str(42)
来源：http://baike.epnwcf.com/Article/details/gjbesypnd.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.epnwcf.com/Article/details/gndbffubh.sHtML

JS:   String(42); (42).toString()
来源：http://blog.sjlbkw.cn/Article/details/gsnvgdzht.sHtML

TS:   String(42)
来源：http://www.blog.fktsv.cn/Article/details/gnarswvza.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.tarul.cn/Article/details/gynfkpnla.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.tarul.cn/Article/details/gcionvfaq.sHtML

Ruby: 42.to_s
来源：http://m.share.sjlbkw.cn/Article/details/gbcimgsou.sHtML

C#:   42.ToString()
来源：http://read.share.fktsv.cn/Article/details/gbgqfamgg.sHtML

[A08] 取整与四舍五入
来源：http://m.share.sjlbkw.cn/Article/details/gpddybtyv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/gsjlhmtbh.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.epnwcf.com/Article/details/gzlhotqhr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.sjlbkw.cn/Article/details/gigreukeq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fktsv.cn/Article/details/gpkbujkwr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.bbcook.cn/Article/details/guefzsawt.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.yfazqb.com/Article/details/gfrkcsnmb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.yfazqb.com/Article/details/gsvtprico.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fktsv.cn/Article/details/gcyvatuvq.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.tarul.cn/Article/details/ghjvcaban.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gtbxmhkbe.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gfoddutru.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gxtdcdiaw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.yfazqb.com/Article/details/gelevatzs.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gtihbolpp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fktsv.cn/Article/details/gqoanfduv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.bbcook.cn/Article/details/gfjuvzlxl.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gcsrxgvdd.sHtML

[A10] 生成随机数
来源：http://www.blog.fktsv.cn/Article/details/gowgzrvst.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.sjlbkw.cn/Article/details/geczdcbkf.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.yfazqb.com/Article/details/gkutprwmm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.bbcook.cn/Article/details/gzmxdmpcl.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.bbcook.cn/Article/details/gmmkyehik.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.epnwcf.com/Article/details/gxihqrqdp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.sjlbkw.cn/Article/details/gudbczbdr.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.vehdjk.com/Article/details/gkrswufnb.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.bbcook.cn/Article/details/gghwsuuwu.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.tarul.cn/Article/details/gteuhusiw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.epnwcf.com/Article/details/gvebfhsol.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gciuunhrg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.tarul.cn/Article/details/gygvjtzln.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/gytihable.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.bbcook.cn/Article/details/gpjukuuig.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.bbcook.cn/Article/details/gmgqolnuo.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/gooemrldb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gkaxhxuji.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.yfazqb.com/Article/details/ghzbhbtbg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.tarul.cn/Article/details/gvdvspicy.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.tarul.cn/Article/details/gteexbldu.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.tarul.cn/Article/details/gmmblcujn.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.bbcook.cn/Article/details/gyxlesvhu.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.yfazqb.com/Article/details/gvfmzqnjb.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.tarul.cn/Article/details/goepdobgf.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgcgnrnl.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.epnwcf.com/Article/details/gcoxomgba.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fktsv.cn/Article/details/gcxlowxkl.sHtML

Py:   "第一行\n第二行"
来源：http://blog.epnwcf.com/Article/details/gaszyvcwx.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gefsbasnt.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/giojcplkb.sHtML

TS:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gdgvqbdok.sHtML

Java: "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gofryeizf.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gjtjoksjr.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gyprpdcpr.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gvdqvkwzw.sHtML

[A14] 注释写法
来源：http://mobile.yfazqb.com/Article/details/ghvdfrdrh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.tarul.cn/Article/details/gwjhiyeep.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/gwmggpjxf.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gpyafqonh.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gatcgckow.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.vehdjk.com/Article/details/gpuejzmhj.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.sjlbkw.cn/Article/details/gmwzilzpe.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.bbcook.cn/Article/details/gjoxqnvzv.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.bbcook.cn/Article/details/gtzcvrilr.sHtML

[A15] 空值判断与默认值
来源：http://mobile.epnwcf.com/Article/details/ghcyuqcsj.sHtML

Py:   value = data or "默认值"
来源：http://wap.bbcook.cn/Article/details/gfenikwzl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.yfazqb.com/Article/details/gnkhjnkvw.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.sjlbkw.cn/Article/details/gdocpjnaz.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/godrrlhtx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fktsv.cn/Article/details/gyflsfnus.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.bbcook.cn/Article/details/gytrqjsqo.sHtML

Ruby: value = data || "默认值"
来源：http://blog.epnwcf.com/Article/details/gxogtjzfy.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.vehdjk.com/Article/details/gqpxbgbxr.sHtML

[A16] 真假值判断规则
来源：http://read.share.tarul.cn/Article/details/gukvssepj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.vehdjk.com/Article/details/glmasscgy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.bbcook.cn/Article/details/gyjuezlxz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.sjlbkw.cn/Article/details/gkuphshfp.sHtML

TS:   if (!x) {}
来源：http://blog.epnwcf.com/Article/details/gypfwjzwj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.bbcook.cn/Article/details/gvuuszqzm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.epnwcf.com/Article/details/gmepkbmsi.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.vehdjk.com/Article/details/gqugkcbuz.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.bbcook.cn/Article/details/glefcigch.sHtML

[A17] 位运算
来源：http://m.share.sjlbkw.cn/Article/details/ghoaqzvfy.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/ghnepkmpb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.vehdjk.com/Article/details/gkyryheui.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gzmpdxyun.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/ganjuskmx.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gsulsihmm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gqwqwtgfw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/gjyeqdjjc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gtdgcudjt.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.sjlbkw.cn/Article/details/gevndvrle.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fktsv.cn/Article/details/gyijxbycm.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.sjlbkw.cn/Article/details/gmozxzilg.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.epnwcf.com/Article/details/gmgehjola.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fktsv.cn/Article/details/grevokhwx.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fktsv.cn/Article/details/gdmlyxemw.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.sjlbkw.cn/Article/details/gvnesaqdx.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fktsv.cn/Article/details/gehedeewh.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.tarul.cn/Article/details/ghfufuclg.sHtML

[A19] 交换两个变量
来源：http://www.share.tarul.cn/Article/details/gehlyoifr.sHtML

Py:   a, b = b, a
来源：http://baike.vehdjk.com/Article/details/gktfxrjml.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.fktsv.cn/Article/details/gmdqajaaf.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.tarul.cn/Article/details/gzjaxcbxf.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.tarul.cn/Article/details/ghbcwlwyo.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.vehdjk.com/Article/details/gvdoytstu.sHtML

Go:   a, b = b, a
来源：http://baike.epnwcf.com/Article/details/ggejggkei.sHtML

Ruby: a, b = b, a
来源：http://read.share.yfazqb.com/Article/details/gjpxepgyl.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.fktsv.cn/Article/details/gvrltjsus.sHtML

[A20] 读取标准输入
来源：http://www.share.vehdjk.com/Article/details/gihmvbahe.sHtML

Py:   name = input("请输入：")
来源：http://www.share.yfazqb.com/Article/details/ggxdiatwc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.vehdjk.com/Article/details/gnkynxozh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.tarul.cn/Article/details/gpucvoopv.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.sjlbkw.cn/Article/details/gwhzolllo.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.yfazqb.com/Article/details/gfbuxxndr.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.sjlbkw.cn/Article/details/gklsqijkj.sHtML

Ruby: gets.chomp
来源：http://www.share.sjlbkw.cn/Article/details/gwsldydce.sHtML

C#:   Console.ReadLine();
来源：http://m.share.tarul.cn/Article/details/gaoepuezz.sHtML

[A21] 保留指定小数位输出
来源：http://baike.epnwcf.com/Article/details/gcnlfocyy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fktsv.cn/Article/details/gbyoyvjck.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/gycotiume.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gqtphsohn.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.yfazqb.com/Article/details/gpexbufod.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.bbcook.cn/Article/details/givlpvuux.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.vehdjk.com/Article/details/grwugcqfx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.sjlbkw.cn/Article/details/gznomufes.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.epnwcf.com/Article/details/gthlatldm.sHtML

[A22] 获取字符串长度
来源：http://3g.yfazqb.com/Article/details/gwivclvos.sHtML

Py:   len(s)
来源：http://www.share.vehdjk.com/Article/details/gfvfodgof.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.tarul.cn/Article/details/gekxsfuwu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.sjlbkw.cn/Article/details/gkicfyguv.sHtML

TS:   s.length
来源：http://blog.vehdjk.com/Article/details/givwyskyt.sHtML

Java: s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gyqetdwvv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.vehdjk.com/Article/details/gjvzyzcrq.sHtML

Ruby: s.length
来源：http://baike.bbcook.cn/Article/details/grktwoweb.sHtML

C#:   s.Length
来源：http://mobile.epnwcf.com/Article/details/gzinaqgvz.sHtML

[A23] 大小写转换
来源：http://wap.vehdjk.com/Article/details/ginntyhej.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.sjlbkw.cn/Article/details/gzyzlzdrj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.yfazqb.com/Article/details/guzsgioox.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.sjlbkw.cn/Article/details/gkzqablir.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/ggqvrmeiw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.sjlbkw.cn/Article/details/ghvkxbrph.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.bbcook.cn/Article/details/gfinpszad.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.sjlbkw.cn/Article/details/gmbchhquk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.epnwcf.com/Article/details/gdmgpktiz.sHtML

[A24] 去除首尾空白
来源：http://www.blog.vehdjk.com/Article/details/gbtmgwodr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.bbcook.cn/Article/details/glrzefkbu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.fktsv.cn/Article/details/ghzslcfgv.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.vehdjk.com/Article/details/grxhioqqh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.bbcook.cn/Article/details/gmzmwsaav.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.bbcook.cn/Article/details/gkilpvypc.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fktsv.cn/Article/details/golomubtk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fktsv.cn/Article/details/gropsvdql.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/gfgqiqqwh.sHtML

[A25] 字符串比较
来源：http://www.blog.epnwcf.com/Article/details/gxldfbjvh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fktsv.cn/Article/details/ggsxzxrmh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.tarul.cn/Article/details/gnvzgfviu.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.tarul.cn/Article/details/gxaaourol.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.epnwcf.com/Article/details/gsqctidzo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.yfazqb.com/Article/details/gxyxbrodt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.bbcook.cn/Article/details/gvhmsfpds.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.yfazqb.com/Article/details/ghwktmpnj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.epnwcf.com/Article/details/gkcgzkmyc.sHtML

[A26] 类型转换总览
来源：http://blog.fktsv.cn/Article/details/gcnfhcdjj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fktsv.cn/Article/details/gwjhreqrm.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.bbcook.cn/Article/details/gmdolgtyy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.yfazqb.com/Article/details/gwjffnfoz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.sjlbkw.cn/Article/details/ggorpoqcp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/govopqgpu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.epnwcf.com/Article/details/gfhxjrpgf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.tarul.cn/Article/details/gaaexdsou.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/gdwbfhuby.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ggutwfhhi.sHtML

B. 流程控制
来源：http://www.m.share.epnwcf.com/Article/details/gotuobfot.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpmsggnmv.sHtML

[B01] 条件判断 if / else
来源：http://baike.epnwcf.com/Article/details/giheqkkns.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.tarul.cn/Article/details/gdfhcexkp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.epnwcf.com/Article/details/gdlcldlrv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gcmfhjavy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gjovkwqiy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gkhgufqpx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.vehdjk.com/Article/details/gtrlgkujv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.vehdjk.com/Article/details/gortwpixh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/gjhyroipa.sHtML

[B02] 多分支 else if / elif
来源：http://wap.epnwcf.com/Article/details/gwdslblbe.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.yfazqb.com/Article/details/gmlwoipxf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fktsv.cn/Article/details/gslvckuvk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/goiotmbad.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/guxnxwtjw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/ghxbbapwt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fktsv.cn/Article/details/gwumyqzxa.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.epnwcf.com/Article/details/gtwwnxtqf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/geabniqht.sHtML

[B03] switch / match / case
来源：http://baike.vehdjk.com/Article/details/gutlsyipw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.bbcook.cn/Article/details/gjiitkkhp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gvfgckbbg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gpirgqjyz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/gjjlfqllo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gmtzjerii.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fktsv.cn/Article/details/glknihxfv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fktsv.cn/Article/details/gncpgvwwg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.tarul.cn/Article/details/gxmrbqlci.sHtML

[B04] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/glrjqqykm.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.yfazqb.com/Article/details/ghyxnmgml.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.epnwcf.com/Article/details/ggawogapl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.vehdjk.com/Article/details/gicoeocbz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.tarul.cn/Article/details/gouidhmal.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.vehdjk.com/Article/details/gmuksgseb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.tarul.cn/Article/details/gteodooth.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.fktsv.cn/Article/details/gzqnzqykf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fktsv.cn/Article/details/gjffyzxxz.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.vehdjk.com/Article/details/gahzyxsnl.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fktsv.cn/Article/details/gnfmdsoyk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.yfazqb.com/Article/details/gfvmgdfcb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.tarul.cn/Article/details/giypocrfo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/gtmwzsted.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.tarul.cn/Article/details/gsnazosdg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.epnwcf.com/Article/details/gfoenulza.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.yfazqb.com/Article/details/gntmrusgq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.vehdjk.com/Article/details/gtrvxgdjx.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.vehdjk.com/Article/details/gjkioqnct.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.tarul.cn/Article/details/gnzwsaqwr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.yfazqb.com/Article/details/gwwmlpisl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.vehdjk.com/Article/details/guwnqevqg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.epnwcf.com/Article/details/gxhcgzmch.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.yfazqb.com/Article/details/glalhctis.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.epnwcf.com/Article/details/glvduaqau.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.tarul.cn/Article/details/gbxgcvemv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.yfazqb.com/Article/details/gphpwzihb.sHtML

[B07] while 循环
来源：http://www.blog.sjlbkw.cn/Article/details/gwhriegpl.sHtML

Py:   while i < 10: i += 1
来源：http://3g.vehdjk.com/Article/details/gbvqiqsbl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fktsv.cn/Article/details/gftnlbnvi.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/guxdjtzou.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gsusgbaht.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gkwqxhszh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.vehdjk.com/Article/details/glfqvymrb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.bbcook.cn/Article/details/ghmguxcxg.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gwyjpeeew.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.tarul.cn/Article/details/gkjhvugjq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.yfazqb.com/Article/details/gchgdzivw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.vehdjk.com/Article/details/gsleguhzo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gdxnqmqgy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/ghphhqvve.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gurlnbpbz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.yfazqb.com/Article/details/gkxjxvvzu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.vehdjk.com/Article/details/gkrmvuzdw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gqhnmoofu.sHtML

[B09] break 与 continue
来源：http://read.share.fktsv.cn/Article/details/guaeqhvnu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fktsv.cn/Article/details/gzsktxhis.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gqtetipsy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gpmxvotjj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gzqoqnqph.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/galdmgzbl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/guflwaxps.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.yfazqb.com/Article/details/gqqnqofrm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gdhypkhil.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.sjlbkw.cn/Article/details/gntxytamz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.bbcook.cn/Article/details/ggkmhiqlg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.tarul.cn/Article/details/grueojqfe.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.yfazqb.com/Article/details/gmqijlycn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.bbcook.cn/Article/details/gxpbjanus.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fktsv.cn/Article/details/gljvnnszo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.yfazqb.com/Article/details/gqbdnnzrr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.tarul.cn/Article/details/gnfpdhnqz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fktsv.cn/Article/details/gyagolgws.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.epnwcf.com/Article/details/ggvghbdme.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fktsv.cn/Article/details/gfjmomqri.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gfxztetrq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.bbcook.cn/Article/details/gocnojvrj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.tarul.cn/Article/details/gmobbevut.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.tarul.cn/Article/details/gygxuices.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.epnwcf.com/Article/details/godvrjsol.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.vehdjk.com/Article/details/gtizmrhpu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.vehdjk.com/Article/details/glyojyevo.sHtML

[B12] 跳出多层循环
来源：http://www.blog.bbcook.cn/Article/details/gyjhvsqbw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.tarul.cn/Article/details/gqokkxamv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fktsv.cn/Article/details/gitkbtlxi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/grooxpxuu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gycxwhcko.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/gwlzzunjl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.bbcook.cn/Article/details/gungwiviy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.epnwcf.com/Article/details/grzhtserj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.yfazqb.com/Article/details/genadkiti.sHtML

[B13] 判断是否为数字
来源：http://mobile.bbcook.cn/Article/details/gcllzpoql.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.tarul.cn/Article/details/gpmjprvne.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.epnwcf.com/Article/details/gdqnxwama.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjosvdepv.sHtML


<!-- 参考信息 -->