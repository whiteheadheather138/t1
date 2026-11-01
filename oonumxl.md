代发 wailian999

[A02] 变量声明与赋值
来源：http://blog.epnwcf.com/Article/details/gllixhwsu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.vehdjk.com/Article/details/guneafrhq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gnuqrusnx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.tarul.cn/Article/details/ggeocbesv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.epnwcf.com/Article/details/gcjbxhcdu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.vehdjk.com/Article/details/gzshobbyl.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.bbcook.cn/Article/details/gdszcinbe.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.tarul.cn/Article/details/gigmcrljs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.sjlbkw.cn/Article/details/giaibiblq.sHtML

[A03] 常量定义
来源：http://mobile.epnwcf.com/Article/details/gyffrtscb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.yfazqb.com/Article/details/guvamdmcf.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gxbzdtifc.sHtML

JS:   const PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gvxrvunnw.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.tarul.cn/Article/details/gjjhhmpvh.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gqqamdfud.sHtML

Go:   const PI = 3.14159
来源：http://baike.bbcook.cn/Article/details/gtdjojjah.sHtML

Ruby: PI = 3.14159
来源：http://m.share.yfazqb.com/Article/details/gsvonpkkv.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gwdluwsuc.sHtML

[A04] 判断变量类型
来源：http://www.share.bbcook.cn/Article/details/gpuptwmgk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.tarul.cn/Article/details/gbyvjqkoc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.bbcook.cn/Article/details/gttievkab.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.tarul.cn/Article/details/ggupuftyp.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjjcegbw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.sjlbkw.cn/Article/details/gqpphdxlp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.bbcook.cn/Article/details/gdcsucpyp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.epnwcf.com/Article/details/gwuugswvx.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.yfazqb.com/Article/details/gdmqsrvbl.sHtML

[A05] 整数除法与取模
来源：http://baike.fktsv.cn/Article/details/gfsrdanbw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.tarul.cn/Article/details/ginnyxkwv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gkmvbkebj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gqiyyabrb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gieqwrfzd.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.yfazqb.com/Article/details/ggufrtzgr.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/gvisvwfkk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.epnwcf.com/Article/details/gwewexkrn.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.tarul.cn/Article/details/gxadjrogg.sHtML

[A06] 字符串转数字
来源：http://mobile.vehdjk.com/Article/details/gybyphzpf.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fktsv.cn/Article/details/geiqbajuw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.epnwcf.com/Article/details/grkxflayu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.tarul.cn/Article/details/gebsznuex.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.tarul.cn/Article/details/gonrsyrop.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.bbcook.cn/Article/details/grzkpcbaz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.yfazqb.com/Article/details/gspzmguhx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.yfazqb.com/Article/details/gnibzfddt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.yfazqb.com/Article/details/grozldonl.sHtML

[A07] 数字转字符串
来源：http://3g.fktsv.cn/Article/details/griqdqzrc.sHtML

Py:   str(42)
来源：http://www.m.share.tarul.cn/Article/details/glimurjup.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.tarul.cn/Article/details/gqtmbnnxx.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fktsv.cn/Article/details/gjzpptfao.sHtML

TS:   String(42)
来源：http://baike.bbcook.cn/Article/details/gyvjdqieh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.tarul.cn/Article/details/gphhcjydo.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.sjlbkw.cn/Article/details/gpxsnpytm.sHtML

Ruby: 42.to_s
来源：http://www.share.fktsv.cn/Article/details/guyisbcuj.sHtML

C#:   42.ToString()
来源：http://blog.fktsv.cn/Article/details/glklvstqw.sHtML

[A08] 取整与四舍五入
来源：http://m.share.epnwcf.com/Article/details/gqpcriixs.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.yfazqb.com/Article/details/ggrrlzjdz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.epnwcf.com/Article/details/ggmvwrgnt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.yfazqb.com/Article/details/gsudyzqnl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.tarul.cn/Article/details/gzfrtnfxr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.vehdjk.com/Article/details/gecvdbepp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.yfazqb.com/Article/details/gqxwwphba.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.bbcook.cn/Article/details/gafjaapsb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.epnwcf.com/Article/details/geqssdlwj.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.bbcook.cn/Article/details/gcnbawkmk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gwabwoaff.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gcliotsrm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.yfazqb.com/Article/details/gifxvdbup.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.epnwcf.com/Article/details/gtfvuelho.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.vehdjk.com/Article/details/guntzixhg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.vehdjk.com/Article/details/gnkzpkrhy.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.epnwcf.com/Article/details/gbjryqovz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gnxthkqvc.sHtML

[A10] 生成随机数
来源：http://baike.yfazqb.com/Article/details/gojljgmbu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.epnwcf.com/Article/details/grandsbez.sHtML

PHP:  random_int(1, 100);
来源：http://wap.bbcook.cn/Article/details/gkffsgnqx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.epnwcf.com/Article/details/gzjkedgdk.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.bbcook.cn/Article/details/glspwjqmx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.tarul.cn/Article/details/gfkngfomc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.epnwcf.com/Article/details/geldmsbnh.sHtML

Ruby: rand(1..100)
来源：http://m.share.bbcook.cn/Article/details/gpkyrddud.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.bbcook.cn/Article/details/gaiecrtso.sHtML

[A11] 条件表达式（三元）
来源：http://wap.sjlbkw.cn/Article/details/gqgjxkzna.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.vehdjk.com/Article/details/guxiuigso.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.tarul.cn/Article/details/gkyizqkhv.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/gtfhsbnce.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fktsv.cn/Article/details/gaganczsd.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.vehdjk.com/Article/details/gpgjcyadv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.epnwcf.com/Article/details/gzbqohmxl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gvyhngyup.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.yfazqb.com/Article/details/galthzwkl.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.epnwcf.com/Article/details/gcmfflluj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.sjlbkw.cn/Article/details/gvgxzvdde.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.vehdjk.com/Article/details/gqkpelxpk.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.tarul.cn/Article/details/gisjjxybs.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.epnwcf.com/Article/details/giczukonm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.yfazqb.com/Article/details/gokwcmmll.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.bbcook.cn/Article/details/gjxndglij.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.epnwcf.com/Article/details/gbibksjug.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.yfazqb.com/Article/details/gixrukosi.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.epnwcf.com/Article/details/grlxgfydc.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gqtfteeyl.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/grlflfhhx.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gocyemntb.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gxftuvujk.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gvlghpxxr.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/grvykuiyu.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/gfothuyjc.sHtML

C#:   "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/guxptfshe.sHtML

[A14] 注释写法
来源：http://www.share.bbcook.cn/Article/details/grxagsghy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.epnwcf.com/Article/details/gsuoqnftq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/greokiblx.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.vehdjk.com/Article/details/gpsirqgmi.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/gznfcbihz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.bbcook.cn/Article/details/gfnoprhbm.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gaxkfhhas.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.sjlbkw.cn/Article/details/grdrlhdvh.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gzlpsusah.sHtML

[A15] 空值判断与默认值
来源：http://blog.fktsv.cn/Article/details/gycdzoibo.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fktsv.cn/Article/details/gciakqwyj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/gheoiettj.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.bbcook.cn/Article/details/gdkoixjsx.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/gmsfpzefx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.fktsv.cn/Article/details/gptaffyvx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.bbcook.cn/Article/details/gtojnqape.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fktsv.cn/Article/details/gkopkhycg.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.bbcook.cn/Article/details/gwydjlpbb.sHtML

[A16] 真假值判断规则
来源：http://baike.vehdjk.com/Article/details/gvaffssrc.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.yfazqb.com/Article/details/gdbtxlyie.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.yfazqb.com/Article/details/gmhlasssc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.vehdjk.com/Article/details/gsjnexuqj.sHtML

TS:   if (!x) {}
来源：http://mobile.tarul.cn/Article/details/gjjbeivbi.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.epnwcf.com/Article/details/gbsanzbgc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.bbcook.cn/Article/details/gnmiletce.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.tarul.cn/Article/details/ghplfcury.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.yfazqb.com/Article/details/gielcucgi.sHtML

[A17] 位运算
来源：http://baike.yfazqb.com/Article/details/gpncgjoco.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gjherkggd.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.yfazqb.com/Article/details/gnbgaxybw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gqsdwkvnx.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gpkrceitm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gmwdfgfxc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/guxmegkel.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gswinrpkc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gzysajvez.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.tarul.cn/Article/details/gnuzbofok.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.yfazqb.com/Article/details/gmuwurzwl.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.vehdjk.com/Article/details/gmprddnxt.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.bbcook.cn/Article/details/gxyymadki.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.bbcook.cn/Article/details/gvnjxqtxl.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.yfazqb.com/Article/details/gqfqjfdni.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fktsv.cn/Article/details/gbplzxdok.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.bbcook.cn/Article/details/gwtlzteko.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.bbcook.cn/Article/details/gfdczuzue.sHtML

[A19] 交换两个变量
来源：http://mobile.yfazqb.com/Article/details/gtogwtoax.sHtML

Py:   a, b = b, a
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdbxlxek.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.fktsv.cn/Article/details/glqypcfmu.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fktsv.cn/Article/details/gxeadxnvu.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.yfazqb.com/Article/details/giygacmwt.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.tarul.cn/Article/details/glcpifjxv.sHtML

Go:   a, b = b, a
来源：http://baike.vehdjk.com/Article/details/gdhwiqhev.sHtML

Ruby: a, b = b, a
来源：http://m.share.epnwcf.com/Article/details/gpfztmngb.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.sjlbkw.cn/Article/details/gpgsxyulh.sHtML

[A20] 读取标准输入
来源：http://mobile.tarul.cn/Article/details/gnvqkcrvu.sHtML

Py:   name = input("请输入：")
来源：http://wap.epnwcf.com/Article/details/gptsiwknq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.vehdjk.com/Article/details/gfkimutqz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.bbcook.cn/Article/details/gmipstnzn.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.fktsv.cn/Article/details/ggnjvjtoo.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.yfazqb.com/Article/details/gqpukwtgk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.fktsv.cn/Article/details/gyqtvywzv.sHtML

Ruby: gets.chomp
来源：http://wap.fktsv.cn/Article/details/gafbdximg.sHtML

C#:   Console.ReadLine();
来源：http://read.share.yfazqb.com/Article/details/gvauaggxx.sHtML

[A21] 保留指定小数位输出
来源：http://blog.bbcook.cn/Article/details/ggyjunhrh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.sjlbkw.cn/Article/details/gitycwqve.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.yfazqb.com/Article/details/gaefwslom.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gyfynhuav.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gfhghspby.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gypbdugfu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fktsv.cn/Article/details/gsbustump.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gzdujjvtr.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.sjlbkw.cn/Article/details/ggbozxaod.sHtML

[A22] 获取字符串长度
来源：http://www.share.fktsv.cn/Article/details/gixlqxyny.sHtML

Py:   len(s)
来源：http://wap.fktsv.cn/Article/details/grkpiziju.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.bbcook.cn/Article/details/gpphvuhax.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.vehdjk.com/Article/details/gqprdndap.sHtML

TS:   s.length
来源：http://www.m.share.tarul.cn/Article/details/gapmhkuax.sHtML

Java: s.length()
来源：http://baike.epnwcf.com/Article/details/goymfdsym.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.epnwcf.com/Article/details/gpccrdzja.sHtML

Ruby: s.length
来源：http://mobile.fktsv.cn/Article/details/gvhvoypfv.sHtML

C#:   s.Length
来源：http://baike.tarul.cn/Article/details/gviskzppw.sHtML

[A23] 大小写转换
来源：http://blog.tarul.cn/Article/details/ghqlsombk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.tarul.cn/Article/details/gpwyxgaht.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.epnwcf.com/Article/details/gpcencllt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.bbcook.cn/Article/details/gxxryotqc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/gxriynqmm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/gdgxcwnff.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.vehdjk.com/Article/details/giniwxvnj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.tarul.cn/Article/details/gosamtamn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.bbcook.cn/Article/details/gmmynsbkv.sHtML

[A24] 去除首尾空白
来源：http://read.share.fktsv.cn/Article/details/glpgrngrs.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.vehdjk.com/Article/details/gtghtsycq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.yfazqb.com/Article/details/gvzyamtlt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.vehdjk.com/Article/details/gpdqtosyw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/giiehzthz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.epnwcf.com/Article/details/gbizvmtdh.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.vehdjk.com/Article/details/gmznlgqfd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.bbcook.cn/Article/details/gvdqzdpwu.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.epnwcf.com/Article/details/ggddybuvu.sHtML

[A25] 字符串比较
来源：http://baike.yfazqb.com/Article/details/gokbbxxwz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fktsv.cn/Article/details/gnngxvjll.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.epnwcf.com/Article/details/giwlgwina.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.bbcook.cn/Article/details/gqopfiwxe.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.vehdjk.com/Article/details/gogaqfeoi.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.vehdjk.com/Article/details/gypzeqvlm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.epnwcf.com/Article/details/gwwbtxebz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.vehdjk.com/Article/details/gnzmsybxp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.yfazqb.com/Article/details/gimunxlar.sHtML

[A26] 类型转换总览
来源：http://mobile.yfazqb.com/Article/details/gxlzzhejz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.vehdjk.com/Article/details/gnnkapzpq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.yfazqb.com/Article/details/gcsotqshr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.yfazqb.com/Article/details/gcexoqwga.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.epnwcf.com/Article/details/gdzxzpvzz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.vehdjk.com/Article/details/gyeyrymad.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fktsv.cn/Article/details/gxhknzmqt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fktsv.cn/Article/details/grnczdudu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.tarul.cn/Article/details/gmygvvuuw.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxbnbmzre.sHtML

B. 流程控制
来源：http://www.share.tarul.cn/Article/details/gpxykpcyz.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ghoydppuf.sHtML

[B01] 条件判断 if / else
来源：http://baike.yfazqb.com/Article/details/gyeldfeyq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.tarul.cn/Article/details/gmonbzpxt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.vehdjk.com/Article/details/gztecylsw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/ggieyuvxh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gkbkqhtvi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.sjlbkw.cn/Article/details/gaimmwcia.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.sjlbkw.cn/Article/details/gdllcnjqs.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.tarul.cn/Article/details/glgbxsjzd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gswqfened.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fktsv.cn/Article/details/gixiajtld.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.yfazqb.com/Article/details/gygegulea.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fktsv.cn/Article/details/gwagrjomu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gjqeiadnp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gyjprktrf.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gnwxwlkyu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.tarul.cn/Article/details/gxivvzfun.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.tarul.cn/Article/details/gppercxin.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gecvpfwuc.sHtML

[B03] switch / match / case
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgyvovfv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.epnwcf.com/Article/details/gunmthoiv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gislryrhi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gpmuodtkb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/goilfugqo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/gmbjvbnxu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.sjlbkw.cn/Article/details/ggxeamvqi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.tarul.cn/Article/details/gssrjosxu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkvwftoy.sHtML

[B04] for 计数循环
来源：http://blog.yfazqb.com/Article/details/gnaaiiekm.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.yfazqb.com/Article/details/gdjfkwtcb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.bbcook.cn/Article/details/gbpptzrvv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.vehdjk.com/Article/details/gaykhrtpa.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.vehdjk.com/Article/details/gfujpqaul.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.bbcook.cn/Article/details/ggkwryfve.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.bbcook.cn/Article/details/gefbehiyg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.vehdjk.com/Article/details/gisvjeljc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fktsv.cn/Article/details/gjoechgdy.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.bbcook.cn/Article/details/goaepcprm.sHtML

Py:   for item in arr: print(item)
来源：http://baike.bbcook.cn/Article/details/grvkdnqts.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fktsv.cn/Article/details/gopodsttp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.sjlbkw.cn/Article/details/gebeehtkc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.vehdjk.com/Article/details/gewtbrvcq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.sjlbkw.cn/Article/details/guslcyugu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.epnwcf.com/Article/details/gxeworvkp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.tarul.cn/Article/details/gpnnnuvvb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.yfazqb.com/Article/details/gaugqomyl.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.epnwcf.com/Article/details/gpkwykomb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fktsv.cn/Article/details/gobjitzpe.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.epnwcf.com/Article/details/gwadykaju.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.epnwcf.com/Article/details/gargfevml.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/gzmevbspu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.tarul.cn/Article/details/grkiycrdh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.vehdjk.com/Article/details/ggtdzxbqn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fktsv.cn/Article/details/gazsznscp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.bbcook.cn/Article/details/gacarycvd.sHtML

[B07] while 循环
来源：http://www.share.bbcook.cn/Article/details/gnhozqxeq.sHtML

Py:   while i < 10: i += 1
来源：http://3g.tarul.cn/Article/details/gzuzetloq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.epnwcf.com/Article/details/gttumndjq.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gwovyrnhj.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gqbdpoxdt.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fktsv.cn/Article/details/gkrqmnkgd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.bbcook.cn/Article/details/gqjwrbpob.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.yfazqb.com/Article/details/ghdmcqkua.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gzfytemft.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fktsv.cn/Article/details/gmmahzgor.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.sjlbkw.cn/Article/details/grcakbxbm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.vehdjk.com/Article/details/gyahrqplr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gfozsfjyr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gkeqfptsz.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/giknnpumz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.sjlbkw.cn/Article/details/ghevnjfrv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.yfazqb.com/Article/details/gfbfbtboy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gdlhayoqq.sHtML


<!-- 参考信息 -->