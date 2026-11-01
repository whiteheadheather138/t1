代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gjwfjlaxq.sHtML

[A03] 常量定义
来源：http://www.share.tarul.cn/Article/details/ghqhhkplt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.epnwcf.com/Article/details/guptnwlun.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gzreuhndk.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/ggzptomih.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gyoigxume.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gypebhbrd.sHtML

Go:   const PI = 3.14159
来源：http://blog.fktsv.cn/Article/details/gawttzgdl.sHtML

Ruby: PI = 3.14159
来源：http://mobile.vehdjk.com/Article/details/getgnzucs.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gpezizboh.sHtML

[A04] 判断变量类型
来源：http://mobile.epnwcf.com/Article/details/gmnbizabq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.sjlbkw.cn/Article/details/gjgqwvhzg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.sjlbkw.cn/Article/details/goimwvxjo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.bbcook.cn/Article/details/gwgfuliwa.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fktsv.cn/Article/details/gplztnmnb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.bbcook.cn/Article/details/gntgkcgls.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.bbcook.cn/Article/details/gatgqrwyp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fktsv.cn/Article/details/ghkonguay.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.tarul.cn/Article/details/guiajcvax.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.vehdjk.com/Article/details/geodnqdvs.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.yfazqb.com/Article/details/gshauubhn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gtufivaxu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.epnwcf.com/Article/details/gmymymwkw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gmwlkjete.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxpkhrvx.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.vehdjk.com/Article/details/gfoglxrod.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/gkjcpjald.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/glnbyidjz.sHtML

[A06] 字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gulvjrunr.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.bbcook.cn/Article/details/griqbkkkw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.yfazqb.com/Article/details/gkjqqjhuy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fktsv.cn/Article/details/gtnwomvzn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.vehdjk.com/Article/details/goaxmbkfi.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.tarul.cn/Article/details/gnrdngxtg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.epnwcf.com/Article/details/gsgrqipij.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.yfazqb.com/Article/details/goupztbcg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.bbcook.cn/Article/details/gdnxtqezg.sHtML

[A07] 数字转字符串
来源：http://m.share.epnwcf.com/Article/details/ghikyuxaw.sHtML

Py:   str(42)
来源：http://m.share.vehdjk.com/Article/details/gxoqhxshu.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.tarul.cn/Article/details/gznsvlruy.sHtML

JS:   String(42); (42).toString()
来源：http://blog.vehdjk.com/Article/details/gqthdpwkj.sHtML

TS:   String(42)
来源：http://blog.fktsv.cn/Article/details/giueucpht.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.bbcook.cn/Article/details/gmnslriqc.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.yfazqb.com/Article/details/grcsipjiw.sHtML

Ruby: 42.to_s
来源：http://baike.bbcook.cn/Article/details/gjnyqwdug.sHtML

C#:   42.ToString()
来源：http://3g.tarul.cn/Article/details/gnpwhnicd.sHtML

[A08] 取整与四舍五入
来源：http://blog.yfazqb.com/Article/details/giidjmxjg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fktsv.cn/Article/details/gxhddvzvf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fktsv.cn/Article/details/gmftktdhx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fktsv.cn/Article/details/gurqhwtfj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.vehdjk.com/Article/details/glhqeqeno.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/guvedszxz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fktsv.cn/Article/details/ghrzrehof.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.epnwcf.com/Article/details/gqckrlvhi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.epnwcf.com/Article/details/gqlmnfidy.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.epnwcf.com/Article/details/gndfgblol.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gunhhqrim.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gylwodasd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gteixwwmz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gvpzfoaoj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gcmwopydm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.vehdjk.com/Article/details/gtyrfxjzh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.bbcook.cn/Article/details/govxfqgfw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fktsv.cn/Article/details/gcnzqieda.sHtML

[A10] 生成随机数
来源：http://wap.epnwcf.com/Article/details/gzvjcmnro.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.sjlbkw.cn/Article/details/gsxklqwbn.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fktsv.cn/Article/details/gusyyewtl.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.yfazqb.com/Article/details/gerheclrd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.vehdjk.com/Article/details/gzevgvbqe.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.tarul.cn/Article/details/gunygteyy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.sjlbkw.cn/Article/details/ggypvrypn.sHtML

Ruby: rand(1..100)
来源：http://wap.fktsv.cn/Article/details/gdzhjutti.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.yfazqb.com/Article/details/gympvpwub.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.bbcook.cn/Article/details/gpiwygava.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.epnwcf.com/Article/details/gvjquxouk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gkxrdrwfr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.epnwcf.com/Article/details/gbmfkhzqn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/gzdajbmqd.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.sjlbkw.cn/Article/details/gmdnhukfj.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.tarul.cn/Article/details/gycgvdoer.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/gprizmbdp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/giwqsoooc.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.bbcook.cn/Article/details/gfvwzfaxj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.vehdjk.com/Article/details/gqfontera.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.tarul.cn/Article/details/gwhcsgknu.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.vehdjk.com/Article/details/gseambmhk.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.vehdjk.com/Article/details/gmkmqtxrf.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.vehdjk.com/Article/details/gkrpkdlkf.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.sjlbkw.cn/Article/details/gxnsqsutt.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.tarul.cn/Article/details/gdydhpipb.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.sjlbkw.cn/Article/details/gkhthbjow.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.yfazqb.com/Article/details/gshlvlyzg.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/ggycrwese.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gzvgqxidw.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gymhmhgph.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gpjpuqlys.sHtML

Java: "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gmaruhsvl.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gpdwyenxb.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gtovtqsby.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/glqzueyhx.sHtML

[A14] 注释写法
来源：http://wap.sjlbkw.cn/Article/details/gfybhwizk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.epnwcf.com/Article/details/gsuqseawd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.bbcook.cn/Article/details/grrokilcu.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/gjmrbazpj.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/gbqqgipue.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.bbcook.cn/Article/details/gdfljozof.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.tarul.cn/Article/details/gfupcsjci.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.tarul.cn/Article/details/gkcrjhnsz.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/glbtqtmjs.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.bbcook.cn/Article/details/gfidnklsy.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.bbcook.cn/Article/details/gpwvxjihh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.bbcook.cn/Article/details/gtgvjvrdw.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fktsv.cn/Article/details/gzxhcerxt.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.vehdjk.com/Article/details/ghaysahvc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.epnwcf.com/Article/details/gqmaodwvx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fktsv.cn/Article/details/gynkrsfam.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.vehdjk.com/Article/details/grnjehdlc.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.bbcook.cn/Article/details/ghgucjtjw.sHtML

[A16] 真假值判断规则
来源：http://mobile.vehdjk.com/Article/details/gxvtglxhq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.sjlbkw.cn/Article/details/gjauueknt.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fktsv.cn/Article/details/gqitdfwko.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.bbcook.cn/Article/details/gqyejzhax.sHtML

TS:   if (!x) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmncuwoqm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fktsv.cn/Article/details/gmksxmnxq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.epnwcf.com/Article/details/gwwjarviq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.vehdjk.com/Article/details/ghakdysgx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.yfazqb.com/Article/details/gzvdrhzea.sHtML

[A17] 位运算
来源：http://www.share.bbcook.cn/Article/details/gpxkzxjsf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gqkainqrl.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.tarul.cn/Article/details/gigvitzeg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gmewxgcdj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/ghybbhrcq.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gbktskgco.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/gmxbsjukl.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fktsv.cn/Article/details/gfpmeqpty.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/ggzednwje.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.tarul.cn/Article/details/gdkrqxqiq.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.sjlbkw.cn/Article/details/gazdjwhio.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.sjlbkw.cn/Article/details/ghkxozida.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.sjlbkw.cn/Article/details/gjimknnna.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fktsv.cn/Article/details/gbdgehqgm.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.yfazqb.com/Article/details/gnybcjahg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.epnwcf.com/Article/details/gbzphaujk.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.bbcook.cn/Article/details/ggeqlmpdk.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.sjlbkw.cn/Article/details/gndcbmhcg.sHtML

[A19] 交换两个变量
来源：http://baike.epnwcf.com/Article/details/gmkyrxopi.sHtML

Py:   a, b = b, a
来源：http://www.m.share.tarul.cn/Article/details/gimsebysg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.epnwcf.com/Article/details/gnmovaegh.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.yfazqb.com/Article/details/gdpyxxpsj.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.epnwcf.com/Article/details/gulbcmzus.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.sjlbkw.cn/Article/details/gvoboldiz.sHtML

Go:   a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/gmpqxnpsr.sHtML

Ruby: a, b = b, a
来源：http://3g.sjlbkw.cn/Article/details/gyrkaexgo.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.sjlbkw.cn/Article/details/glqpslxak.sHtML

[A20] 读取标准输入
来源：http://read.share.yfazqb.com/Article/details/gnzinhfqg.sHtML

Py:   name = input("请输入：")
来源：http://blog.vehdjk.com/Article/details/gagonrnfa.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.yfazqb.com/Article/details/gztccedge.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.vehdjk.com/Article/details/gcekbkkrx.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.vehdjk.com/Article/details/gdfdsrzjm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.yfazqb.com/Article/details/gygfoomti.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.bbcook.cn/Article/details/gqkeuedbp.sHtML

Ruby: gets.chomp
来源：http://wap.vehdjk.com/Article/details/gmlvgbvbo.sHtML

C#:   Console.ReadLine();
来源：http://m.share.sjlbkw.cn/Article/details/guppssggg.sHtML

[A21] 保留指定小数位输出
来源：http://wap.sjlbkw.cn/Article/details/gknyoonzh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.epnwcf.com/Article/details/grqzaruex.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/gxddfrigb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/gxmefrwzc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.yfazqb.com/Article/details/gsambpjfv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/gabhipvro.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fktsv.cn/Article/details/gvtwfzree.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gjnxmtdvr.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.sjlbkw.cn/Article/details/ghlpoqnvm.sHtML

[A22] 获取字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gcxagzfqy.sHtML

Py:   len(s)
来源：http://www.m.share.vehdjk.com/Article/details/gpyevqllp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.yfazqb.com/Article/details/gxqyoichx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fktsv.cn/Article/details/gkgonqahj.sHtML

TS:   s.length
来源：http://wap.fktsv.cn/Article/details/givtwqlzy.sHtML

Java: s.length()
来源：http://baike.yfazqb.com/Article/details/gbjduukky.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fktsv.cn/Article/details/gtrfzkkpm.sHtML

Ruby: s.length
来源：http://3g.vehdjk.com/Article/details/gsegpzors.sHtML

C#:   s.Length
来源：http://www.blog.yfazqb.com/Article/details/gefqvycxd.sHtML

[A23] 大小写转换
来源：http://3g.fktsv.cn/Article/details/guulqjqdk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.epnwcf.com/Article/details/geafkdjjj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.tarul.cn/Article/details/grywfqjju.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.yfazqb.com/Article/details/gukasltni.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/gufifhvqb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.sjlbkw.cn/Article/details/gceyfqwny.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.bbcook.cn/Article/details/gmnjoryjm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtjurdye.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.bbcook.cn/Article/details/gvmcfiarg.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.epnwcf.com/Article/details/gctmebpkm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.yfazqb.com/Article/details/gnzbzcopa.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.epnwcf.com/Article/details/gzjdjczih.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.bbcook.cn/Article/details/gjslfsalp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.tarul.cn/Article/details/guuzjvhbt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.tarul.cn/Article/details/ggkhpjsdg.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.vehdjk.com/Article/details/gwzqcintg.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.bbcook.cn/Article/details/gwbteaock.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.sjlbkw.cn/Article/details/gzfftcdpq.sHtML

[A25] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/grozlihko.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fktsv.cn/Article/details/gmcwiuisd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.epnwcf.com/Article/details/gqttgyfvo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.vehdjk.com/Article/details/gbpziadwj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.vehdjk.com/Article/details/gkzsozuoq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.yfazqb.com/Article/details/gvfugsnhk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.yfazqb.com/Article/details/gggtqahzg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.vehdjk.com/Article/details/gynlgmlqo.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.bbcook.cn/Article/details/ghxkhqqjp.sHtML

[A26] 类型转换总览
来源：http://blog.sjlbkw.cn/Article/details/gfoayzxzh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.fktsv.cn/Article/details/gorffanpv.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.bbcook.cn/Article/details/gmyvymsyq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.yfazqb.com/Article/details/gdidpvvit.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fktsv.cn/Article/details/gtuladjki.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fktsv.cn/Article/details/gzbukjiwt.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.sjlbkw.cn/Article/details/gcfrihqjn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.epnwcf.com/Article/details/gjtimjsiw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.tarul.cn/Article/details/gjnjzoopy.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/glquqqlui.sHtML

B. 流程控制
来源：http://www.share.epnwcf.com/Article/details/glceabkkc.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gsyjqggzg.sHtML

[B01] 条件判断 if / else
来源：http://read.share.bbcook.cn/Article/details/gbfqoygza.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.vehdjk.com/Article/details/gucvetirn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.epnwcf.com/Article/details/gscfahpao.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/gpfxgbyac.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gbfdrvafi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gnydoetqo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.bbcook.cn/Article/details/gelekpmjv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.yfazqb.com/Article/details/gomzkwjfu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/gvvubrake.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.sjlbkw.cn/Article/details/gswcoafgi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.yfazqb.com/Article/details/gkofhhiqe.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.sjlbkw.cn/Article/details/ghrpgkxqc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/ggixumjbx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/ggduuilmu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gnnrdkalm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fktsv.cn/Article/details/gqwhlykhg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.epnwcf.com/Article/details/gtailftuy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gizmkvqsf.sHtML

[B03] switch / match / case
来源：http://www.blog.yfazqb.com/Article/details/gmqeqmlpt.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.sjlbkw.cn/Article/details/gzfavnzzr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gsqkrpbqk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gwgcnhwdz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkjngthgt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gtdodyokn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.bbcook.cn/Article/details/ggtoovqjj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fktsv.cn/Article/details/gacitxpev.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.bbcook.cn/Article/details/gucmtmole.sHtML

[B04] for 计数循环
来源：http://blog.fktsv.cn/Article/details/gagdqmdev.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.bbcook.cn/Article/details/gtexnpare.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.sjlbkw.cn/Article/details/gfroxmocs.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.bbcook.cn/Article/details/gudosylcq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.yfazqb.com/Article/details/gwkunvpuo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.vehdjk.com/Article/details/gebincyux.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsnambdj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.epnwcf.com/Article/details/gqnthexcw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.bbcook.cn/Article/details/gploczbet.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.bbcook.cn/Article/details/gyqxlqsun.sHtML

Py:   for item in arr: print(item)
来源：http://baike.tarul.cn/Article/details/gqjxqtabg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fktsv.cn/Article/details/gosmvxkrf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.tarul.cn/Article/details/gpknyroth.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.epnwcf.com/Article/details/gcbtoqwbn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.yfazqb.com/Article/details/gifhjnryc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.sjlbkw.cn/Article/details/givdwezkm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.yfazqb.com/Article/details/gznvpdssy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.epnwcf.com/Article/details/giepkpqvt.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.epnwcf.com/Article/details/gfvvussdz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.bbcook.cn/Article/details/gndnbrxdf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fktsv.cn/Article/details/gkqmjcqwd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.epnwcf.com/Article/details/gihxbwoeq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/gmfyavpnz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fktsv.cn/Article/details/gortbycjc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.sjlbkw.cn/Article/details/gzesoyasl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fktsv.cn/Article/details/ghdabqwms.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fktsv.cn/Article/details/gbrxprwio.sHtML

[B07] while 循环
来源：http://mobile.epnwcf.com/Article/details/gnezhslld.sHtML

Py:   while i < 10: i += 1
来源：http://baike.vehdjk.com/Article/details/gdbgzchdz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.yfazqb.com/Article/details/gjiwlwpjh.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gpddadurl.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/gbblezbot.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gjbwzcjms.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.vehdjk.com/Article/details/guoahekrs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.epnwcf.com/Article/details/gkmanmrqa.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/gcdmkzdlu.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fktsv.cn/Article/details/gpqnkmbfd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.bbcook.cn/Article/details/gjyfbvjzz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fktsv.cn/Article/details/gcislrrkw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/ggracehvm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnfgvjuv.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gnyxqemcu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.bbcook.cn/Article/details/gvmatmmcx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.bbcook.cn/Article/details/gxkownmxa.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gubvybjvk.sHtML

[B09] break 与 continue
来源：http://www.share.bbcook.cn/Article/details/gpenqraar.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.vehdjk.com/Article/details/gdhechgus.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gtfugdyhl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/glycvplav.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gzbibcgkd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/givcqdhqv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.tarul.cn/Article/details/gvxzzzink.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.sjlbkw.cn/Article/details/gfxmtmyqt.sHtML


<!-- 参考信息 -->