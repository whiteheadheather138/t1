代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://baike.yfazqb.com/Article/details/gaysaletu.sHtML

[A03] 常量定义
来源：http://baike.fktsv.cn/Article/details/gdbcdmhjh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.bbcook.cn/Article/details/gyoonpkka.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gwueqkaob.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gpsgicrud.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gmblrqges.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gumjxadxt.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fktsv.cn/Article/details/gpyzwlwqd.sHtML

Ruby: PI = 3.14159
来源：http://wap.fktsv.cn/Article/details/gcbzewmyv.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gohchfepi.sHtML

[A04] 判断变量类型
来源：http://baike.tarul.cn/Article/details/gsyjzfwaj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.bbcook.cn/Article/details/gxomgadrf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.yfazqb.com/Article/details/gmrthpker.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.vehdjk.com/Article/details/grwzvbwxd.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.tarul.cn/Article/details/gjrokaoyw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.epnwcf.com/Article/details/goatwjugw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.sjlbkw.cn/Article/details/gqqouqdfo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.epnwcf.com/Article/details/gmnaytnuc.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fktsv.cn/Article/details/glcgkcslh.sHtML

[A05] 整数除法与取模
来源：http://baike.epnwcf.com/Article/details/gobvfrfux.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.sjlbkw.cn/Article/details/gwjpzhntk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gslgbtlvh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.tarul.cn/Article/details/gcedmvzfq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.epnwcf.com/Article/details/gqvfummsz.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/galbiuwka.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.sjlbkw.cn/Article/details/gmtwuagoe.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.tarul.cn/Article/details/gcfzkbrzy.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gbdbigrbi.sHtML

[A06] 字符串转数字
来源：http://3g.bbcook.cn/Article/details/gpvnwkawn.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.tarul.cn/Article/details/ghsrqfedo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.bbcook.cn/Article/details/gxaingyde.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.vehdjk.com/Article/details/glulcmpma.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.epnwcf.com/Article/details/gmqxvfzzd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.yfazqb.com/Article/details/grgabakzs.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.sjlbkw.cn/Article/details/googccpbt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.epnwcf.com/Article/details/gezupleee.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.bbcook.cn/Article/details/gjjhgeifl.sHtML

[A07] 数字转字符串
来源：http://wap.vehdjk.com/Article/details/gulmjvabo.sHtML

Py:   str(42)
来源：http://www.m.share.epnwcf.com/Article/details/gmgvqszdk.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.yfazqb.com/Article/details/gausrouha.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.bbcook.cn/Article/details/gupmykomz.sHtML

TS:   String(42)
来源：http://read.share.vehdjk.com/Article/details/guzosdqle.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.sjlbkw.cn/Article/details/gtehuazhy.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.bbcook.cn/Article/details/ghljkiwxd.sHtML

Ruby: 42.to_s
来源：http://blog.fktsv.cn/Article/details/grhcnfecn.sHtML

C#:   42.ToString()
来源：http://baike.yfazqb.com/Article/details/gnqwxrqsb.sHtML

[A08] 取整与四舍五入
来源：http://baike.fktsv.cn/Article/details/guxrspfdg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fktsv.cn/Article/details/glcprooov.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fktsv.cn/Article/details/gwoethmuq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gdzjhhbjq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fktsv.cn/Article/details/gylrjqmoa.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.yfazqb.com/Article/details/gosmglxgc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/gignytmeq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.yfazqb.com/Article/details/gikghpuzg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/ggndgnasd.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.tarul.cn/Article/details/gwuskbcgj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fktsv.cn/Article/details/gqixiawvl.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.epnwcf.com/Article/details/gywiavrqk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gdusaewcv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.bbcook.cn/Article/details/gshrziccz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.fktsv.cn/Article/details/gwritocvq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.bbcook.cn/Article/details/gcjlkiqny.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.sjlbkw.cn/Article/details/gwodjwslt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gdkhyrrjg.sHtML

[A10] 生成随机数
来源：http://wap.tarul.cn/Article/details/gtlhvhkch.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.sjlbkw.cn/Article/details/ggyxnyozb.sHtML

PHP:  random_int(1, 100);
来源：http://3g.yfazqb.com/Article/details/gamabamyw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fktsv.cn/Article/details/gjwqnkhym.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.epnwcf.com/Article/details/gnfyapgxb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fktsv.cn/Article/details/gqiifuidu.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.sjlbkw.cn/Article/details/gmhbrxyrp.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.epnwcf.com/Article/details/gcymqaglx.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fktsv.cn/Article/details/gkvvjkdes.sHtML

[A11] 条件表达式（三元）
来源：http://3g.vehdjk.com/Article/details/gxgyuoeim.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fktsv.cn/Article/details/gbechdsvh.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/gwvtntxhr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/glyihcsnn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.sjlbkw.cn/Article/details/giemqzqbt.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/gimeerxns.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.yfazqb.com/Article/details/gdfxqojfl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.bbcook.cn/Article/details/gulmngjwa.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.vehdjk.com/Article/details/gwcywrmvu.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.epnwcf.com/Article/details/giwqmxnrt.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.yfazqb.com/Article/details/gbhhdhqwb.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.vehdjk.com/Article/details/gjahnxkmp.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.yfazqb.com/Article/details/ghrakdnyu.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.tarul.cn/Article/details/gakkwjxog.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.yfazqb.com/Article/details/ghuaneavr.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fktsv.cn/Article/details/gsxbcomet.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.sjlbkw.cn/Article/details/gctnvypsp.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.sjlbkw.cn/Article/details/gxuiduggt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fktsv.cn/Article/details/gfyhmnrqu.sHtML

Py:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gcyndzujl.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/ghgrexytd.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gfmahuumy.sHtML

TS:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/giftzykov.sHtML

Java: "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gogthwuwa.sHtML

Go:   "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/gnafkkxke.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gyfzdytgb.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gbaactira.sHtML

[A14] 注释写法
来源：http://wap.fktsv.cn/Article/details/gplbrjexo.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.vehdjk.com/Article/details/gldgkrgwa.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.tarul.cn/Article/details/gwghvuuzj.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gmzhtabwp.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.tarul.cn/Article/details/glhbtrois.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.vehdjk.com/Article/details/giflqgwek.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.fktsv.cn/Article/details/gqebinuaf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.bbcook.cn/Article/details/gahiwueqf.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fktsv.cn/Article/details/glibfynme.sHtML

[A15] 空值判断与默认值
来源：http://mobile.bbcook.cn/Article/details/gbicrooms.sHtML

Py:   value = data or "默认值"
来源：http://read.share.epnwcf.com/Article/details/grxyazvfm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.sjlbkw.cn/Article/details/gftufeays.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.epnwcf.com/Article/details/gdzignmcr.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.vehdjk.com/Article/details/gbshdxcxi.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fktsv.cn/Article/details/gooakecpu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.sjlbkw.cn/Article/details/gajccitfq.sHtML

Ruby: value = data || "默认值"
来源：http://baike.epnwcf.com/Article/details/gtuvapjuk.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.yfazqb.com/Article/details/ggffpeqqb.sHtML

[A16] 真假值判断规则
来源：http://3g.sjlbkw.cn/Article/details/gtdxeytni.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.tarul.cn/Article/details/gjbyxxjdp.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.bbcook.cn/Article/details/gfcaovbac.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.bbcook.cn/Article/details/gouxjjllr.sHtML

TS:   if (!x) {}
来源：http://www.share.sjlbkw.cn/Article/details/grqpopcvo.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fktsv.cn/Article/details/graahcnly.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.sjlbkw.cn/Article/details/grbcjozot.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.fktsv.cn/Article/details/gatdkcvbf.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gdaundlbz.sHtML

[A17] 位运算
来源：http://mobile.sjlbkw.cn/Article/details/gwdrlqfky.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gwifqwpsz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.sjlbkw.cn/Article/details/giwkgppip.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fktsv.cn/Article/details/gsxjdyevc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gvoykngrl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fktsv.cn/Article/details/gssrhzuwm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/giqelrrvc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gnyzicfug.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/glvwsktvv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.yfazqb.com/Article/details/gkkpixvyc.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.yfazqb.com/Article/details/gcnnzqawc.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.tarul.cn/Article/details/geacpoyax.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fktsv.cn/Article/details/gxwvknyyr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.tarul.cn/Article/details/gfzvtvhkv.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.vehdjk.com/Article/details/gaoskvlvs.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.bbcook.cn/Article/details/gynkatzob.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.epnwcf.com/Article/details/gzixroqtx.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.tarul.cn/Article/details/gbvgtityd.sHtML

[A19] 交换两个变量
来源：http://www.share.sjlbkw.cn/Article/details/gphciwdtg.sHtML

Py:   a, b = b, a
来源：http://mobile.yfazqb.com/Article/details/gedgcpgwy.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fktsv.cn/Article/details/ghfltyscw.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.yfazqb.com/Article/details/gwirilewa.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.fktsv.cn/Article/details/gcdnkjdzs.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.tarul.cn/Article/details/gxkwtiuhp.sHtML

Go:   a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gdbtkqtfz.sHtML

Ruby: a, b = b, a
来源：http://www.blog.bbcook.cn/Article/details/gbabgsnei.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.epnwcf.com/Article/details/gwldyvyrp.sHtML

[A20] 读取标准输入
来源：http://mobile.yfazqb.com/Article/details/gpidwwulu.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fktsv.cn/Article/details/gqgwdjgxu.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.sjlbkw.cn/Article/details/guuukfxlg.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.bbcook.cn/Article/details/grjuvbuzz.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.bbcook.cn/Article/details/gcstdfomv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.tarul.cn/Article/details/gazncnmjv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.yfazqb.com/Article/details/gxttksxdu.sHtML

Ruby: gets.chomp
来源：http://m.share.sjlbkw.cn/Article/details/gcqzavoog.sHtML

C#:   Console.ReadLine();
来源：http://read.share.epnwcf.com/Article/details/gvhdegfwn.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.yfazqb.com/Article/details/gchirunjd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.sjlbkw.cn/Article/details/gehtteqwy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/gixdtpwnn.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlxmjjvg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gwxxwzevh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/gaicqiouo.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.epnwcf.com/Article/details/gqxndpuqy.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.sjlbkw.cn/Article/details/geepuyupz.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fktsv.cn/Article/details/glwcpyojo.sHtML

[A22] 获取字符串长度
来源：http://mobile.vehdjk.com/Article/details/gorgzhtbz.sHtML

Py:   len(s)
来源：http://m.share.yfazqb.com/Article/details/gojcoweqj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.bbcook.cn/Article/details/gdqojigkp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.yfazqb.com/Article/details/gpxegtkus.sHtML

TS:   s.length
来源：http://www.blog.bbcook.cn/Article/details/gwgvyhugk.sHtML

Java: s.length()
来源：http://m.share.epnwcf.com/Article/details/gugizsmop.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.sjlbkw.cn/Article/details/gsrnpcziz.sHtML

Ruby: s.length
来源：http://www.m.share.tarul.cn/Article/details/giuzgviqc.sHtML

C#:   s.Length
来源：http://www.blog.tarul.cn/Article/details/gvyynujtl.sHtML

[A23] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gopwkcwrg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fktsv.cn/Article/details/gncpzescl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.epnwcf.com/Article/details/gtwkkgmsr.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.yfazqb.com/Article/details/gwgfnnehb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.sjlbkw.cn/Article/details/gawogoauk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fktsv.cn/Article/details/gzyuogicq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.epnwcf.com/Article/details/gqqioaakn.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.sjlbkw.cn/Article/details/gjzbpoqsa.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.tarul.cn/Article/details/gqtaredib.sHtML

[A24] 去除首尾空白
来源：http://mobile.sjlbkw.cn/Article/details/gbeoieomv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.tarul.cn/Article/details/gqcsrnaod.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.vehdjk.com/Article/details/gijlzjoyd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fktsv.cn/Article/details/gxqkqyddn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.epnwcf.com/Article/details/gywcludyp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fktsv.cn/Article/details/gjcbiuyod.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.yfazqb.com/Article/details/goihvckyu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.vehdjk.com/Article/details/gaeuddibj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.yfazqb.com/Article/details/gyokmcszn.sHtML

[A25] 字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gjmpvugao.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.bbcook.cn/Article/details/gdolskanz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.bbcook.cn/Article/details/gpgaovbgj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fktsv.cn/Article/details/gpgntehcw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.yfazqb.com/Article/details/gqicwhgjw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.yfazqb.com/Article/details/glismvvfe.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.tarul.cn/Article/details/gtmlqhpsp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.bbcook.cn/Article/details/gsrqpnvks.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.vehdjk.com/Article/details/grnzhwfdr.sHtML

[A26] 类型转换总览
来源：http://wap.tarul.cn/Article/details/gdqddcgfd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.sjlbkw.cn/Article/details/gpmomllkk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.bbcook.cn/Article/details/gmfcxxhqb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.sjlbkw.cn/Article/details/glwcjosii.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.vehdjk.com/Article/details/gfnfxrceo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.bbcook.cn/Article/details/gwrgtkilr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.bbcook.cn/Article/details/glntvoryc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.fktsv.cn/Article/details/gpfrpfxvu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.vehdjk.com/Article/details/gdadrfrge.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gkjlkdbbl.sHtML

B. 流程控制
来源：http://m.share.sjlbkw.cn/Article/details/gqfvvrmuz.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbzywoutq.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.sjlbkw.cn/Article/details/gxgwpypyi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.epnwcf.com/Article/details/gzoaydmpj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.sjlbkw.cn/Article/details/gnaaxsprw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/gidrtgtvi.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/ggyhbalrq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/gowhwetkb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.epnwcf.com/Article/details/gxcczyglc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.epnwcf.com/Article/details/gwshvqgou.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gpydwklku.sHtML

[B02] 多分支 else if / elif
来源：http://3g.vehdjk.com/Article/details/ganxzqssw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.bbcook.cn/Article/details/gmoraootf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbcuswir.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gpgzkefah.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/gjxqzethd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gruhzdgrx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.tarul.cn/Article/details/gaalzwjkb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.vehdjk.com/Article/details/ghddrmpqg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fktsv.cn/Article/details/giagdtkui.sHtML

[B03] switch / match / case
来源：http://read.share.bbcook.cn/Article/details/glyqqeexo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.epnwcf.com/Article/details/gdexzjxje.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gcwmzzhdq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gebboxgxl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gdmiypfpk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/grhfxtqjs.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fktsv.cn/Article/details/gkyfozvdt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.vehdjk.com/Article/details/gdafiqtne.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.sjlbkw.cn/Article/details/ghpvkygba.sHtML

[B04] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gnntcogto.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.yfazqb.com/Article/details/geihazbwa.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.vehdjk.com/Article/details/gfanzezvr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.yfazqb.com/Article/details/grwwvebsf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.epnwcf.com/Article/details/gwrgknlfc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.tarul.cn/Article/details/gxofkkqjj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.vehdjk.com/Article/details/gslknljyb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqemepmvf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fktsv.cn/Article/details/gyyutfnci.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.yfazqb.com/Article/details/gssdmynon.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.tarul.cn/Article/details/grpeyzbdk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.bbcook.cn/Article/details/gsrmzphgg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.sjlbkw.cn/Article/details/gkqzvviwo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.epnwcf.com/Article/details/gzfhcjdxg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.tarul.cn/Article/details/gjcncefyu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.bbcook.cn/Article/details/gvbhtnlis.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.vehdjk.com/Article/details/gjxsmjvzz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fktsv.cn/Article/details/gfuubtkmn.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fktsv.cn/Article/details/gandphomr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.epnwcf.com/Article/details/gppwebpro.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsmznnmx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gpitwelff.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fktsv.cn/Article/details/gkcbxskzl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.epnwcf.com/Article/details/gmsewsauq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fktsv.cn/Article/details/gqmneixow.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.tarul.cn/Article/details/gloxqcirl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fktsv.cn/Article/details/gnrivkipu.sHtML

[B07] while 循环
来源：http://baike.sjlbkw.cn/Article/details/grxlyikyg.sHtML

Py:   while i < 10: i += 1
来源：http://blog.sjlbkw.cn/Article/details/gcoaengzt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.bbcook.cn/Article/details/gvltzakgh.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fktsv.cn/Article/details/gvohwakyq.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/gsobtumhh.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/grqhxfrha.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.sjlbkw.cn/Article/details/glfmiadfc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.sjlbkw.cn/Article/details/gsslgyhsc.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gfjwjbyuc.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.tarul.cn/Article/details/gdbmuxnvm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.sjlbkw.cn/Article/details/gkohcvwkk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/guxapaucc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fktsv.cn/Article/details/gskdzctcw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gxefrhlut.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gcjnipmbl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.vehdjk.com/Article/details/gzusqfyyl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fktsv.cn/Article/details/gsswtlfvp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.tarul.cn/Article/details/gxpetnnhf.sHtML

[B09] break 与 continue
来源：http://3g.bbcook.cn/Article/details/gehdkzuly.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.epnwcf.com/Article/details/gzhazqinc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gifbkhrnc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gjwodrjem.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gnjfehget.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gqffrdtsa.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fktsv.cn/Article/details/gxanqjsgj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.vehdjk.com/Article/details/gpocivuyz.sHtML


<!-- 参考信息 -->