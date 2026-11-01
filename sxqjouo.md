代发 wailian999

Ruby: PI = 3.14159
来源：http://baike.sjlbkw.cn/Article/details/gisjdgmzv.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqcpilzj.sHtML

[A04] 判断变量类型
来源：http://m.share.epnwcf.com/Article/details/gdggzcfoz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.sjlbkw.cn/Article/details/giagookhb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.bbcook.cn/Article/details/gioacjame.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.sjlbkw.cn/Article/details/ggtkmnczx.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.bbcook.cn/Article/details/gnawuymvw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.epnwcf.com/Article/details/gmckrglzj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fktsv.cn/Article/details/gzlvjaoik.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.vehdjk.com/Article/details/gurmyojdw.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fktsv.cn/Article/details/gbwaunckc.sHtML

[A05] 整数除法与取模
来源：http://baike.tarul.cn/Article/details/gcmyxoyld.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.tarul.cn/Article/details/gztrnviwl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fktsv.cn/Article/details/gxncrnhbp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gprgpruiy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.epnwcf.com/Article/details/ggmjwwsdq.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gxmhjmwvq.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.bbcook.cn/Article/details/gtdowjsxy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.yfazqb.com/Article/details/gswakhiiu.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/ghrxhljzb.sHtML

[A06] 字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/givwpmulw.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.epnwcf.com/Article/details/gyoycecfa.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.sjlbkw.cn/Article/details/gnpxhqffo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.epnwcf.com/Article/details/gzfeqkdgg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.epnwcf.com/Article/details/ghhvrunqb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.sjlbkw.cn/Article/details/grnwanwqd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.bbcook.cn/Article/details/gcjjajxck.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fktsv.cn/Article/details/ghkenpswc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.sjlbkw.cn/Article/details/geglrhvop.sHtML

[A07] 数字转字符串
来源：http://mobile.fktsv.cn/Article/details/gtlyupanq.sHtML

Py:   str(42)
来源：http://mobile.epnwcf.com/Article/details/galkahusa.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.epnwcf.com/Article/details/gqtnzjlrq.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.yfazqb.com/Article/details/gvipctgzv.sHtML

TS:   String(42)
来源：http://blog.fktsv.cn/Article/details/gdguidyuf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.tarul.cn/Article/details/guhbtdsql.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.vehdjk.com/Article/details/gmsobilmf.sHtML

Ruby: 42.to_s
来源：http://3g.tarul.cn/Article/details/gsvzkflqh.sHtML

C#:   42.ToString()
来源：http://baike.fktsv.cn/Article/details/ggjerhgbu.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.vehdjk.com/Article/details/ggddrizyt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.sjlbkw.cn/Article/details/gzixnjdvy.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.sjlbkw.cn/Article/details/ghenowgdt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/greqjcsvw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.tarul.cn/Article/details/gpmztkzkr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/gbrjmynxk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gwfnzukys.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.vehdjk.com/Article/details/gmyingquq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.fktsv.cn/Article/details/gkpvwzvva.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.yfazqb.com/Article/details/gbgsgkrxj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/gdrdulcsg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gzdhlfpfb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.vehdjk.com/Article/details/ggdjzygot.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gaycerjbt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.epnwcf.com/Article/details/gidnerxcp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.epnwcf.com/Article/details/gxvrxqsfy.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.tarul.cn/Article/details/gshrloxrk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/glfpvjevq.sHtML

[A10] 生成随机数
来源：http://baike.fktsv.cn/Article/details/gwdqgaspg.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.sjlbkw.cn/Article/details/guzowuvcy.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.bbcook.cn/Article/details/grjeeyacx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.sjlbkw.cn/Article/details/gzoogmfsq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.bbcook.cn/Article/details/ghyfgdbnv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.tarul.cn/Article/details/gqsznefro.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fktsv.cn/Article/details/gjyznwbmi.sHtML

Ruby: rand(1..100)
来源：http://www.share.fktsv.cn/Article/details/gdyyiajbs.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.vehdjk.com/Article/details/ghpzyhkhd.sHtML

[A11] 条件表达式（三元）
来源：http://baike.bbcook.cn/Article/details/gludamubt.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.yfazqb.com/Article/details/gfopsbacc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.tarul.cn/Article/details/gfeygiwks.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.tarul.cn/Article/details/gcqjgrcox.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/gnicmoijp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.vehdjk.com/Article/details/gxnxngtbq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.sjlbkw.cn/Article/details/ggwmoapvc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/gwqzdhrqa.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.tarul.cn/Article/details/gqgsorgib.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.vehdjk.com/Article/details/gebxuyecj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fktsv.cn/Article/details/gtucamjgt.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.yfazqb.com/Article/details/gcfndslsd.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.tarul.cn/Article/details/gdayleokq.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.epnwcf.com/Article/details/gteteaoil.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmjwffrv.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fktsv.cn/Article/details/gqicghxry.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.vehdjk.com/Article/details/gfifhzebs.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.fktsv.cn/Article/details/gunmnxcsq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.tarul.cn/Article/details/gugnymxek.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/ggjrdksor.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/gjpcbjmau.sHtML

JS:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gtlucecfl.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/gewyvccnl.sHtML

Java: "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gbolcffgv.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/ggjoswjai.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gfrgrypqf.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gwzfdsajk.sHtML

[A14] 注释写法
来源：http://m.share.tarul.cn/Article/details/grxwzsadc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fktsv.cn/Article/details/gkbmlzezp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/gjrmxxqse.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/grjxosrsc.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gabklafxl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.bbcook.cn/Article/details/gvrfxatbc.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fktsv.cn/Article/details/gfvomkfom.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.sjlbkw.cn/Article/details/gqxqnhtll.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/gwcfjibmr.sHtML

[A15] 空值判断与默认值
来源：http://wap.tarul.cn/Article/details/gdmvpopzq.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.vehdjk.com/Article/details/gygvrgpmy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/gxvlaayif.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.yfazqb.com/Article/details/ggonkmflv.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.vehdjk.com/Article/details/gckzfdyva.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.epnwcf.com/Article/details/gnooroedd.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.yfazqb.com/Article/details/gcpjnvydm.sHtML

Ruby: value = data || "默认值"
来源：http://3g.epnwcf.com/Article/details/gyuyfpvps.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.tarul.cn/Article/details/gdpdyedqw.sHtML

[A16] 真假值判断规则
来源：http://3g.epnwcf.com/Article/details/gwahkgwvp.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.tarul.cn/Article/details/gcsiazler.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.yfazqb.com/Article/details/gbqvamauy.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fktsv.cn/Article/details/gomtcsagy.sHtML

TS:   if (!x) {}
来源：http://wap.sjlbkw.cn/Article/details/gltzomayd.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gdvnpudfg.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.yfazqb.com/Article/details/gsgxaokyz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fktsv.cn/Article/details/gpfztltzs.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.yfazqb.com/Article/details/gmvtfrvum.sHtML

[A17] 位运算
来源：http://blog.epnwcf.com/Article/details/gilslvcid.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gkpznbqfl.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.vehdjk.com/Article/details/gnrhkrtuf.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gnjqavgjk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/ggbjxlbji.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/grwagnlls.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gqxqvufun.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gsaztkqym.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/grcbnyfkr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fktsv.cn/Article/details/gqwemcqpa.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.tarul.cn/Article/details/gyqudtqfz.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.epnwcf.com/Article/details/guaoyqlzb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.bbcook.cn/Article/details/gpmfxdlsb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.bbcook.cn/Article/details/gnyeuosvk.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fktsv.cn/Article/details/gnkpyxvor.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.fktsv.cn/Article/details/gxfmmtjed.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.fktsv.cn/Article/details/gfwholhxa.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.sjlbkw.cn/Article/details/gqggqlimz.sHtML

[A19] 交换两个变量
来源：http://read.share.fktsv.cn/Article/details/gfwduzehf.sHtML

Py:   a, b = b, a
来源：http://baike.tarul.cn/Article/details/gnucqbgxa.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.bbcook.cn/Article/details/gloxsxefs.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fktsv.cn/Article/details/gpklazklz.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.sjlbkw.cn/Article/details/gityoxrhu.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.epnwcf.com/Article/details/gbaglyjta.sHtML

Go:   a, b = b, a
来源：http://www.blog.fktsv.cn/Article/details/gavjahzbl.sHtML

Ruby: a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/gumrvnbay.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.epnwcf.com/Article/details/gxinxhdie.sHtML

[A20] 读取标准输入
来源：http://read.share.fktsv.cn/Article/details/gkxsdxibs.sHtML

Py:   name = input("请输入：")
来源：http://www.share.bbcook.cn/Article/details/gjbknxpic.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.bbcook.cn/Article/details/grqihypvf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.yfazqb.com/Article/details/gxlscwjhk.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.tarul.cn/Article/details/gnrzrlgmc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.sjlbkw.cn/Article/details/gzugtnpmb.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fktsv.cn/Article/details/grmmgygte.sHtML

Ruby: gets.chomp
来源：http://www.share.vehdjk.com/Article/details/gnwpxzlhd.sHtML

C#:   Console.ReadLine();
来源：http://m.share.bbcook.cn/Article/details/gexshtiaj.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.tarul.cn/Article/details/gakzeuzzd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.bbcook.cn/Article/details/glelavvqs.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.tarul.cn/Article/details/grnsvnhij.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.epnwcf.com/Article/details/gncqmxesh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.yfazqb.com/Article/details/grnalnozh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.bbcook.cn/Article/details/gnprhonus.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/gnnkosnev.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.sjlbkw.cn/Article/details/galgxenvd.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.vehdjk.com/Article/details/gmjronnma.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gmfsfxntg.sHtML

Py:   len(s)
来源：http://m.share.sjlbkw.cn/Article/details/ghrryexnt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.yfazqb.com/Article/details/ggtsvuvrh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.vehdjk.com/Article/details/gljugivmh.sHtML

TS:   s.length
来源：http://blog.yfazqb.com/Article/details/girkempaq.sHtML

Java: s.length()
来源：http://m.share.epnwcf.com/Article/details/ggfbbabyy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fktsv.cn/Article/details/gbotdjpud.sHtML

Ruby: s.length
来源：http://mobile.bbcook.cn/Article/details/gzbnetrhe.sHtML

C#:   s.Length
来源：http://read.share.bbcook.cn/Article/details/gvxvoexxy.sHtML

[A23] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/gsgklczfy.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.vehdjk.com/Article/details/ghaiuivib.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.tarul.cn/Article/details/gwtkbblmy.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.tarul.cn/Article/details/ghhpkmydh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fktsv.cn/Article/details/gnreqvnph.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.yfazqb.com/Article/details/gvknxmatr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.bbcook.cn/Article/details/gmnrovoff.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.yfazqb.com/Article/details/ggrlvhzjs.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.bbcook.cn/Article/details/gmnfthgek.sHtML

[A24] 去除首尾空白
来源：http://www.share.vehdjk.com/Article/details/gcszaaksi.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.bbcook.cn/Article/details/gbidegaez.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.yfazqb.com/Article/details/gfttwquvk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.sjlbkw.cn/Article/details/gsiaobtaa.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.epnwcf.com/Article/details/glmofzhcn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.yfazqb.com/Article/details/gxymxkwcg.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.bbcook.cn/Article/details/glfrguaef.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.sjlbkw.cn/Article/details/gnamovhkj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.vehdjk.com/Article/details/gjucvetea.sHtML

[A25] 字符串比较
来源：http://3g.yfazqb.com/Article/details/gtmfxhcco.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.yfazqb.com/Article/details/gjxehvobr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.vehdjk.com/Article/details/gstfymzvv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.vehdjk.com/Article/details/glvvfmiuc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.tarul.cn/Article/details/gqbwzavnu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.tarul.cn/Article/details/gdrwbiakw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.yfazqb.com/Article/details/gctgqfkpz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.yfazqb.com/Article/details/gxijtpyfg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.tarul.cn/Article/details/gyagteqhr.sHtML

[A26] 类型转换总览
来源：http://m.share.bbcook.cn/Article/details/gxvftfvsa.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.tarul.cn/Article/details/goynvlsfg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.bbcook.cn/Article/details/ghqkwajkk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.sjlbkw.cn/Article/details/gotjyypft.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.bbcook.cn/Article/details/gcdngvuvk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/gjtxxeyjm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.sjlbkw.cn/Article/details/gyelculfs.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.yfazqb.com/Article/details/gqjhvkwof.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.yfazqb.com/Article/details/givtezylh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/grpezwtvl.sHtML

B. 流程控制
来源：http://blog.tarul.cn/Article/details/gghlvghgj.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/goilbomtj.sHtML

[B01] 条件判断 if / else
来源：http://m.share.bbcook.cn/Article/details/gnzqrgwrh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.tarul.cn/Article/details/gubveqpnl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.vehdjk.com/Article/details/glmnzzkhg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/ggxzjdixz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/ghepizsal.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/gocyevrrn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.vehdjk.com/Article/details/gqotmeyue.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fktsv.cn/Article/details/gvmmhhosr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gabrtlovp.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.vehdjk.com/Article/details/gdshgrctk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.bbcook.cn/Article/details/gcluqxgut.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.epnwcf.com/Article/details/goetfmlfi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/ghcqoourx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gdaiothto.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gvruujsto.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.vehdjk.com/Article/details/gwfkceeuk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.bbcook.cn/Article/details/gixxiznkz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/gjtrxhssb.sHtML

[B03] switch / match / case
来源：http://read.share.tarul.cn/Article/details/gyoidxbjq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.vehdjk.com/Article/details/gcfeidavy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/gvrjydwrf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/gykkqklad.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gfmvifsar.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gtyfhtmpw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fktsv.cn/Article/details/ggayukdaw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqrxppcx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.epnwcf.com/Article/details/gzkywghal.sHtML

[B04] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/gvyxayctb.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.bbcook.cn/Article/details/gjutspoxr.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.vehdjk.com/Article/details/gupvhyhtb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.yfazqb.com/Article/details/glmdwiqvd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gbuhcmgtu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.yfazqb.com/Article/details/gdidlmnud.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.vehdjk.com/Article/details/goesmogvn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.sjlbkw.cn/Article/details/godagzzzs.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.bbcook.cn/Article/details/gqmbnxivo.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/gkkyscgxs.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.tarul.cn/Article/details/gdhyruwkb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.vehdjk.com/Article/details/gtjtacxqi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gobqjusnq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gofeqliwy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.sjlbkw.cn/Article/details/gtzjjbteq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.tarul.cn/Article/details/gncouttor.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.tarul.cn/Article/details/gomjiyjvj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fktsv.cn/Article/details/gizwltlea.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.yfazqb.com/Article/details/gsrlozorc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.vehdjk.com/Article/details/gmghfatex.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fktsv.cn/Article/details/govlrpwot.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gflnlhmcr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.tarul.cn/Article/details/gxgpaitaw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.tarul.cn/Article/details/gwlnfmbew.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.yfazqb.com/Article/details/gcrxdfkfk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.tarul.cn/Article/details/gkcqpalqz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.epnwcf.com/Article/details/gmgezplqm.sHtML

[B07] while 循环
来源：http://www.m.share.bbcook.cn/Article/details/glfmotuvy.sHtML

Py:   while i < 10: i += 1
来源：http://blog.tarul.cn/Article/details/gusrpieju.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.yfazqb.com/Article/details/gvkkcaivr.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gzrailcyb.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gjjxvjalm.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gqxusjypt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.yfazqb.com/Article/details/gqgsvqgic.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.vehdjk.com/Article/details/gjfwoiwxg.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/ghnxhfldr.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fktsv.cn/Article/details/gxnwbvdqq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.yfazqb.com/Article/details/gmkigtxik.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.epnwcf.com/Article/details/gwynmpefe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/ggaixtmcw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gdwmrddnd.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gcefoeuyy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.yfazqb.com/Article/details/gcfydlvky.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.yfazqb.com/Article/details/gzsetkwvf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gdlwtxidu.sHtML

[B09] break 与 continue
来源：http://www.m.share.epnwcf.com/Article/details/gnhaxctii.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.sjlbkw.cn/Article/details/gplstxkzj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gjbdzoqqj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gbdbzkdkl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gilxjvgkr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gcqxbfliy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.tarul.cn/Article/details/gslrkvfrd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.epnwcf.com/Article/details/gwkqzunud.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gjahnnheh.sHtML

[B10] 遍历同时拿索引
来源：http://wap.vehdjk.com/Article/details/gyvxeozhb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.vehdjk.com/Article/details/gyjpmcctg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.bbcook.cn/Article/details/gajzsxnyq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.tarul.cn/Article/details/ghsvtxyqr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fktsv.cn/Article/details/gyenttizu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.tarul.cn/Article/details/gvqzubhxw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.bbcook.cn/Article/details/ggcrxuihc.sHtML


<!-- 参考信息 -->