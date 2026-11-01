代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.epnwcf.com/Article/details/gqmwqdhyg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.epnwcf.com/Article/details/gqhcvzhdp.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.tarul.cn/Article/details/gpqqirqkn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.bbcook.cn/Article/details/gtwkfwvae.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gvaohlaek.sHtML

[A03] 常量定义
来源：http://mobile.sjlbkw.cn/Article/details/gkdwrixwx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fktsv.cn/Article/details/gtxohqhet.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gdosrdjhg.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gvfwfuwei.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gzynzifxc.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gupkkahvk.sHtML

Go:   const PI = 3.14159
来源：http://mobile.yfazqb.com/Article/details/guuutwmpq.sHtML

Ruby: PI = 3.14159
来源：http://baike.yfazqb.com/Article/details/guwfwwmov.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gxiqtbdfc.sHtML

[A04] 判断变量类型
来源：http://m.share.fktsv.cn/Article/details/gvyvjalil.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.sjlbkw.cn/Article/details/gnzunprib.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.yfazqb.com/Article/details/gzueenubm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fktsv.cn/Article/details/glttiuwlo.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.vehdjk.com/Article/details/gdmkxuhmc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.bbcook.cn/Article/details/gfxelzjhh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.vehdjk.com/Article/details/gsltxmkvm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.tarul.cn/Article/details/glmikdndo.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.bbcook.cn/Article/details/gncberncx.sHtML

[A05] 整数除法与取模
来源：http://mobile.bbcook.cn/Article/details/gsbauzrrf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.epnwcf.com/Article/details/gfodgcrps.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.tarul.cn/Article/details/gwsuxvkcx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.vehdjk.com/Article/details/glivdxpmw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fktsv.cn/Article/details/gqzokeswr.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gqsfpkzia.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gkasamzci.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.bbcook.cn/Article/details/gcygnzawr.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/gbdqjgogc.sHtML

[A06] 字符串转数字
来源：http://m.share.yfazqb.com/Article/details/gghqwoujr.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.vehdjk.com/Article/details/gwxnfmhhu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.epnwcf.com/Article/details/gibcqadye.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.yfazqb.com/Article/details/gptmepmsa.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.yfazqb.com/Article/details/gvtalbfaz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fktsv.cn/Article/details/grmlsaqfe.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzqfeqww.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.sjlbkw.cn/Article/details/gvodrdonv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fktsv.cn/Article/details/gqgcqmbuk.sHtML

[A07] 数字转字符串
来源：http://3g.epnwcf.com/Article/details/govcyerjo.sHtML

Py:   str(42)
来源：http://www.blog.tarul.cn/Article/details/gsnebhlxt.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.vehdjk.com/Article/details/gkamqurqk.sHtML

JS:   String(42); (42).toString()
来源：http://blog.sjlbkw.cn/Article/details/gykvaemgb.sHtML

TS:   String(42)
来源：http://www.share.tarul.cn/Article/details/gxpsmzkdc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.vehdjk.com/Article/details/gouphjwdv.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.yfazqb.com/Article/details/gczmxmhsa.sHtML

Ruby: 42.to_s
来源：http://www.blog.tarul.cn/Article/details/gsglqiufq.sHtML

C#:   42.ToString()
来源：http://blog.sjlbkw.cn/Article/details/ghbzlszya.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.bbcook.cn/Article/details/gtglglowq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.vehdjk.com/Article/details/gzupvoogl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.sjlbkw.cn/Article/details/gibmqpvoo.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.tarul.cn/Article/details/gehzsgsua.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.bbcook.cn/Article/details/grjlkmfhy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.epnwcf.com/Article/details/gooufzicy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.vehdjk.com/Article/details/gmdeuvprg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.vehdjk.com/Article/details/gffjhtfga.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.sjlbkw.cn/Article/details/gysepjgys.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.yfazqb.com/Article/details/glecifgdg.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gcilehilb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.yfazqb.com/Article/details/ghjmdmrbh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.tarul.cn/Article/details/ggbhhqamv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.tarul.cn/Article/details/gyonxffbd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.tarul.cn/Article/details/ghrboypfu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.sjlbkw.cn/Article/details/gwhchptyv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.sjlbkw.cn/Article/details/gatwkpjgz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fktsv.cn/Article/details/gojzsbtmx.sHtML

[A10] 生成随机数
来源：http://www.m.share.sjlbkw.cn/Article/details/gexguxjxi.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.sjlbkw.cn/Article/details/gxjgmmiho.sHtML

PHP:  random_int(1, 100);
来源：http://wap.bbcook.cn/Article/details/gbgmtnzfl.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.epnwcf.com/Article/details/gnniiqfla.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.tarul.cn/Article/details/gagtrlrmw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.bbcook.cn/Article/details/gbrezgwep.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.bbcook.cn/Article/details/gpsnaqrya.sHtML

Ruby: rand(1..100)
来源：http://www.blog.bbcook.cn/Article/details/gqwejvzdf.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.yfazqb.com/Article/details/gynqcfalw.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fktsv.cn/Article/details/glxxnoujw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.bbcook.cn/Article/details/gwnkgkbxw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.epnwcf.com/Article/details/gucscnkas.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.vehdjk.com/Article/details/gmumuqoae.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/gfcepbehc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/gpmxjjoqz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.sjlbkw.cn/Article/details/gnhmamvoa.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.tarul.cn/Article/details/gjpkuybuv.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fktsv.cn/Article/details/ghpjlolno.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.tarul.cn/Article/details/gikkpljxm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.epnwcf.com/Article/details/goxytzpty.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.fktsv.cn/Article/details/gxhwtotaf.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.bbcook.cn/Article/details/gjbaagikf.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.epnwcf.com/Article/details/gywzkaguf.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.yfazqb.com/Article/details/goytlemkr.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fktsv.cn/Article/details/gtqncglur.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.epnwcf.com/Article/details/gzsricmhd.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.vehdjk.com/Article/details/gbdnelmhs.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.vehdjk.com/Article/details/gsyynkyhp.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fktsv.cn/Article/details/gozfiliif.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gtwxrtgcp.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gjhozfpkl.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gyauzrlkl.sHtML

Java: "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/grrgjnuoc.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/ghiqhocdn.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gsccdhnsn.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gunkkhjhh.sHtML

[A14] 注释写法
来源：http://wap.bbcook.cn/Article/details/gjgypqtof.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.epnwcf.com/Article/details/greexsmqi.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/ghwbcqqlx.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/gphqxcdye.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.bbcook.cn/Article/details/gokgnmssh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fktsv.cn/Article/details/gcsmqvrtp.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.sjlbkw.cn/Article/details/gmvlpjhfc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.vehdjk.com/Article/details/gbyqvcdzk.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gjtpxxmzy.sHtML

[A15] 空值判断与默认值
来源：http://mobile.yfazqb.com/Article/details/gwhvgxjzn.sHtML

Py:   value = data or "默认值"
来源：http://www.share.epnwcf.com/Article/details/gfiibaoyj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/gtlcbqaxi.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.tarul.cn/Article/details/gpjzhknoi.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.yfazqb.com/Article/details/gnqtzjiwr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.fktsv.cn/Article/details/gpzvfadpb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.sjlbkw.cn/Article/details/gqkvaafbi.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.epnwcf.com/Article/details/gxpvfzile.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/grvipdqth.sHtML

[A16] 真假值判断规则
来源：http://m.share.fktsv.cn/Article/details/glnjxmvxl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.bbcook.cn/Article/details/gypdipcfh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.yfazqb.com/Article/details/glmidrlva.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.sjlbkw.cn/Article/details/gimjzmtlx.sHtML

TS:   if (!x) {}
来源：http://read.share.sjlbkw.cn/Article/details/glfqykuwt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.fktsv.cn/Article/details/gpcpsnizf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.bbcook.cn/Article/details/gthqvidyn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.sjlbkw.cn/Article/details/gmqvnseak.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.bbcook.cn/Article/details/gsqfnekzw.sHtML

[A17] 位运算
来源：http://read.share.vehdjk.com/Article/details/gmhvjrzhm.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/gszdawkbi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gydyqxouk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gebjqtmxb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gruvxgsgg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gwnugjwuy.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gkyydxppc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gfbsyjezm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gqifrptmv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.epnwcf.com/Article/details/goodihdwf.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.yfazqb.com/Article/details/gyzyqoycs.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.tarul.cn/Article/details/gsjmqwfts.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.vehdjk.com/Article/details/gtmlliurr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.vehdjk.com/Article/details/gnwmrvfra.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.fktsv.cn/Article/details/gxkhsljfr.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.epnwcf.com/Article/details/gbdrurqhp.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.bbcook.cn/Article/details/gsozdgmfz.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.epnwcf.com/Article/details/glgdeocgg.sHtML

[A19] 交换两个变量
来源：http://3g.bbcook.cn/Article/details/ggadbucxf.sHtML

Py:   a, b = b, a
来源：http://wap.epnwcf.com/Article/details/gxmdqypoq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.sjlbkw.cn/Article/details/giyxpgzym.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.epnwcf.com/Article/details/gudxaoevb.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.fktsv.cn/Article/details/gzhxmegul.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fktsv.cn/Article/details/gtwatnjii.sHtML

Go:   a, b = b, a
来源：http://baike.fktsv.cn/Article/details/gznyrzpva.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.bbcook.cn/Article/details/gkmproqdi.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.tarul.cn/Article/details/gjjgdwzzw.sHtML

[A20] 读取标准输入
来源：http://3g.yfazqb.com/Article/details/geknbodgb.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.fktsv.cn/Article/details/gznjyezlh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.yfazqb.com/Article/details/gkjlzqssv.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.fktsv.cn/Article/details/gzaszmuci.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fktsv.cn/Article/details/glmcifzhf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fktsv.cn/Article/details/ggqblhglj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.epnwcf.com/Article/details/geoywcjbk.sHtML

Ruby: gets.chomp
来源：http://www.m.share.sjlbkw.cn/Article/details/giehlarel.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fktsv.cn/Article/details/gtgxbtfes.sHtML

[A21] 保留指定小数位输出
来源：http://3g.vehdjk.com/Article/details/gplsivzvj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.tarul.cn/Article/details/gimtfkccr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.vehdjk.com/Article/details/gvlavnbpn.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gnakgyesm.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/gfspiwqdt.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/ggpgrtdxn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/glniailgd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/grnxuatec.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.tarul.cn/Article/details/gdikpcsmw.sHtML

[A22] 获取字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gxsurnzyl.sHtML

Py:   len(s)
来源：http://blog.epnwcf.com/Article/details/gcenvhaks.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.fktsv.cn/Article/details/gixzswpux.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.tarul.cn/Article/details/gxzbdfbwo.sHtML

TS:   s.length
来源：http://read.share.bbcook.cn/Article/details/gmfvsbfpm.sHtML

Java: s.length()
来源：http://blog.epnwcf.com/Article/details/guochqbho.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.epnwcf.com/Article/details/gujlwvhow.sHtML

Ruby: s.length
来源：http://www.blog.fktsv.cn/Article/details/gybsqmrbz.sHtML

C#:   s.Length
来源：http://baike.sjlbkw.cn/Article/details/gunzmocrs.sHtML

[A23] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gkaswlxiy.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.vehdjk.com/Article/details/gjgxhxlis.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.vehdjk.com/Article/details/gikafjgpk.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.tarul.cn/Article/details/gdwhbvvec.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.sjlbkw.cn/Article/details/gbcrcnrrm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fktsv.cn/Article/details/gwsiyrylu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.epnwcf.com/Article/details/gexjsgkzt.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.sjlbkw.cn/Article/details/gxdpzclrp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.tarul.cn/Article/details/gourcwfat.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fktsv.cn/Article/details/gxjoksgdt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.tarul.cn/Article/details/grlrajorv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.epnwcf.com/Article/details/gcsaphgrq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.sjlbkw.cn/Article/details/gxuxbggbc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.yfazqb.com/Article/details/gykrifitu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.epnwcf.com/Article/details/gsyxzkrje.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.epnwcf.com/Article/details/gpxvxcvvt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.sjlbkw.cn/Article/details/gsjabgact.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.epnwcf.com/Article/details/gdjgejwel.sHtML

[A25] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/gehkburlr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.tarul.cn/Article/details/gzkgwikog.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.bbcook.cn/Article/details/gtnkhjrmf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.tarul.cn/Article/details/gnkpgbkmq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.bbcook.cn/Article/details/gqhdcaeaa.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.tarul.cn/Article/details/ghczhauxp.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.bbcook.cn/Article/details/gyiuukipk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.tarul.cn/Article/details/gradwwpvx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.sjlbkw.cn/Article/details/gdanctiwo.sHtML

[A26] 类型转换总览
来源：http://www.blog.tarul.cn/Article/details/glsffnsfp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.sjlbkw.cn/Article/details/gawygbowj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.bbcook.cn/Article/details/gghbermjm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.vehdjk.com/Article/details/gcwhcefbv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.bbcook.cn/Article/details/gyvccdlds.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.tarul.cn/Article/details/gmmblnien.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.sjlbkw.cn/Article/details/guaixlcrq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.yfazqb.com/Article/details/gglxtopjn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.epnwcf.com/Article/details/groxbsonu.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkmcurphv.sHtML

B. 流程控制
来源：http://m.share.vehdjk.com/Article/details/gotehscjh.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gssdypvhb.sHtML

[B01] 条件判断 if / else
来源：http://m.share.vehdjk.com/Article/details/ginxshppv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.tarul.cn/Article/details/gjlecfdrf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fktsv.cn/Article/details/grtrwvdje.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gxzwjcybe.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/gobmvxezp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/grbpmhaae.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.epnwcf.com/Article/details/gfuupaunz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.epnwcf.com/Article/details/goewaiidr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gpnlwiblz.sHtML

[B02] 多分支 else if / elif
来源：http://blog.tarul.cn/Article/details/gudzziang.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.tarul.cn/Article/details/gcyyejvcb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.vehdjk.com/Article/details/gnpwitnfi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gskchqifs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/goxhqjmbg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gdytjcjpr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fktsv.cn/Article/details/gjapzxyrx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.tarul.cn/Article/details/gccxukcei.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/gontmmenr.sHtML

[B03] switch / match / case
来源：http://www.blog.vehdjk.com/Article/details/gvejtbwzl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.sjlbkw.cn/Article/details/gbnximrbq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gbxlpqgoo.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gqnqqxjpz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.epnwcf.com/Article/details/gtofrxbrw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/govbbwhfl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.yfazqb.com/Article/details/gowrhklce.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.epnwcf.com/Article/details/gcxwdkzom.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.vehdjk.com/Article/details/ghltnedwm.sHtML

[B04] for 计数循环
来源：http://www.blog.epnwcf.com/Article/details/giatjzvgd.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.epnwcf.com/Article/details/gugvnldlx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fktsv.cn/Article/details/gmxsbpyfg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gxuvgkmje.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.sjlbkw.cn/Article/details/grjqndeyy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.epnwcf.com/Article/details/gwcnswlka.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.sjlbkw.cn/Article/details/grxafkqid.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.bbcook.cn/Article/details/gzsafrryx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.vehdjk.com/Article/details/giynxzqyy.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.vehdjk.com/Article/details/gpocmztlr.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.yfazqb.com/Article/details/gvosrnegx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.vehdjk.com/Article/details/gqxxqwzrc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.epnwcf.com/Article/details/gqpsbwwca.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.vehdjk.com/Article/details/gebssjjzc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.epnwcf.com/Article/details/gmkqglhtb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.yfazqb.com/Article/details/gmhbiaoyn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.sjlbkw.cn/Article/details/ggirgcpwi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.vehdjk.com/Article/details/gmbbsrgxa.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.vehdjk.com/Article/details/gxqyeaudp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.sjlbkw.cn/Article/details/galeegjrj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.epnwcf.com/Article/details/gxfpugnal.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.tarul.cn/Article/details/garlfyxht.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.bbcook.cn/Article/details/ggpbqfbtx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.tarul.cn/Article/details/gscuhwgdy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.yfazqb.com/Article/details/ggmnsbvbd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.epnwcf.com/Article/details/gngmpqgsa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fktsv.cn/Article/details/gveqnaomo.sHtML

[B07] while 循环
来源：http://www.blog.bbcook.cn/Article/details/gofafpuxt.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.bbcook.cn/Article/details/gqfcraizi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.yfazqb.com/Article/details/gvbqlihgv.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gyefxazjo.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/gvdhcoqwg.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gahjxwoyu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.sjlbkw.cn/Article/details/gzeiozmcy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.sjlbkw.cn/Article/details/gqyvhhgtc.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gwluqvpci.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fktsv.cn/Article/details/gwcltjetg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.vehdjk.com/Article/details/gpgtkhvuh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.vehdjk.com/Article/details/gwnhcnnca.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gygdnaoif.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/ggtuikghw.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gpwcbmemg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.vehdjk.com/Article/details/gqpwpcfwd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.vehdjk.com/Article/details/gpbvqugpy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gtfckolen.sHtML

[B09] break 与 continue
来源：http://wap.bbcook.cn/Article/details/gybihwcdz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fktsv.cn/Article/details/gdaywhwut.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gxcbmcvkk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gpzphgequ.sHtML


<!-- 参考信息 -->