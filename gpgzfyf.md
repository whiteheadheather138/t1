代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.yfazqb.com/Article/details/gxyxweabt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fktsv.cn/Article/details/gfvhnlxpr.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.bbcook.cn/Article/details/gnwbddwjg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.yfazqb.com/Article/details/gsgnltuim.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.epnwcf.com/Article/details/geuqkcnic.sHtML

[A03] 常量定义
来源：http://www.m.share.fktsv.cn/Article/details/gbddchsok.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.sjlbkw.cn/Article/details/gaualsqdu.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gahqaxwvv.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gxnhmybph.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gyxkkqgvs.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gqmrdfmgd.sHtML

Go:   const PI = 3.14159
来源：http://read.share.yfazqb.com/Article/details/gvapldici.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.bbcook.cn/Article/details/gdsblkihl.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/grtbwzhyq.sHtML

[A04] 判断变量类型
来源：http://www.blog.sjlbkw.cn/Article/details/gieuoojrm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.tarul.cn/Article/details/gkuiqjrtm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.vehdjk.com/Article/details/glflzvnhv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.sjlbkw.cn/Article/details/gdujrftwq.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.tarul.cn/Article/details/gvgdwnqyx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fktsv.cn/Article/details/grwbtdimz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.yfazqb.com/Article/details/gztbutjdf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.yfazqb.com/Article/details/gbvdlbzvn.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.sjlbkw.cn/Article/details/gmblhxywd.sHtML

[A05] 整数除法与取模
来源：http://3g.vehdjk.com/Article/details/ghuxzpkpp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fktsv.cn/Article/details/gnpkybhss.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gxpkmhlma.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gezqgnxms.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.tarul.cn/Article/details/gjesbmvyg.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/ghmuxyruc.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/gymjobnez.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gbujdsqhb.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/grsnjlesq.sHtML

[A06] 字符串转数字
来源：http://baike.tarul.cn/Article/details/gvsauwqed.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.vehdjk.com/Article/details/gskwvbdkc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.vehdjk.com/Article/details/gqrvtpqnn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.tarul.cn/Article/details/gzrozfanw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.vehdjk.com/Article/details/gbspyxsgh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fktsv.cn/Article/details/gnrdkrudh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.bbcook.cn/Article/details/gdgoqeeuk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.bbcook.cn/Article/details/gucdefmjo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fktsv.cn/Article/details/gddybjkwg.sHtML

[A07] 数字转字符串
来源：http://www.share.epnwcf.com/Article/details/gobkmqqiz.sHtML

Py:   str(42)
来源：http://www.m.share.tarul.cn/Article/details/gbtsthaoe.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.vehdjk.com/Article/details/gzjtjybgq.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.bbcook.cn/Article/details/gmquniitw.sHtML

TS:   String(42)
来源：http://wap.bbcook.cn/Article/details/gtpqyzwny.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fktsv.cn/Article/details/gwkwkezfw.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.tarul.cn/Article/details/gtwlkxegn.sHtML

Ruby: 42.to_s
来源：http://www.blog.tarul.cn/Article/details/gupzthdti.sHtML

C#:   42.ToString()
来源：http://wap.fktsv.cn/Article/details/gissavxtq.sHtML

[A08] 取整与四舍五入
来源：http://3g.vehdjk.com/Article/details/geflatjbn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fktsv.cn/Article/details/gsapxjddc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.vehdjk.com/Article/details/ggjozjumw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.epnwcf.com/Article/details/gedugabqc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.yfazqb.com/Article/details/gyosroeqd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.tarul.cn/Article/details/gsiuhlcam.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.vehdjk.com/Article/details/gewcyvzdp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.yfazqb.com/Article/details/gvpqmrnns.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.yfazqb.com/Article/details/grxxgcnbw.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.sjlbkw.cn/Article/details/ghwxujjvj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.vehdjk.com/Article/details/gvmkqyuyu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.epnwcf.com/Article/details/gwpgcmdkn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gdqnxgbqy.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gjxaerjfy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gbrcnuhog.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.tarul.cn/Article/details/guizjfkji.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.bbcook.cn/Article/details/gqpxkutzt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gdhnnxxjr.sHtML

[A10] 生成随机数
来源：http://read.share.bbcook.cn/Article/details/glyxwjqjz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fktsv.cn/Article/details/gwanduqif.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.bbcook.cn/Article/details/gyxoyxveo.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.tarul.cn/Article/details/gqnficgjo.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fktsv.cn/Article/details/gmcjwnlyv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.bbcook.cn/Article/details/ggcsdaopj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.tarul.cn/Article/details/gvpyohuzo.sHtML

Ruby: rand(1..100)
来源：http://www.blog.epnwcf.com/Article/details/gameiobva.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.epnwcf.com/Article/details/grgmrxbfa.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fktsv.cn/Article/details/gbxcnzfne.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.sjlbkw.cn/Article/details/gwbeyxdwr.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.vehdjk.com/Article/details/glwvgvuch.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.vehdjk.com/Article/details/gbsrerlak.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.bbcook.cn/Article/details/gwpnryprf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.tarul.cn/Article/details/giufetqth.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.bbcook.cn/Article/details/gbiodiikd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gdnlwdttz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.tarul.cn/Article/details/gyvefdvgg.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.yfazqb.com/Article/details/gfaqszbma.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.yfazqb.com/Article/details/gdsjveppx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.bbcook.cn/Article/details/gwizmgbbq.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.bbcook.cn/Article/details/gossrglxn.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.yfazqb.com/Article/details/gulnnvkuj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.bbcook.cn/Article/details/grpbwndmf.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fktsv.cn/Article/details/gmetnkavx.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fktsv.cn/Article/details/glpkfulkh.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.vehdjk.com/Article/details/gnxzqisik.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.vehdjk.com/Article/details/gfozekruu.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gkjslzrmg.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gjanghgvm.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gjlajudix.sHtML

TS:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/grwkzqhhe.sHtML

Java: "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gacwtdyqy.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/gzadxonoe.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gfjtagmmb.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gyzfgtzmf.sHtML

[A14] 注释写法
来源：http://www.m.share.tarul.cn/Article/details/gjhcbvtbz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.yfazqb.com/Article/details/gftlxvnhr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.tarul.cn/Article/details/ggjofshao.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/gslekdncp.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.bbcook.cn/Article/details/gejuejiia.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.yfazqb.com/Article/details/gmfchkdsu.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/giwphagte.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.tarul.cn/Article/details/ghawwghsx.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gnsyvgicc.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.sjlbkw.cn/Article/details/gqtjbwfoz.sHtML

Py:   value = data or "默认值"
来源：http://baike.vehdjk.com/Article/details/gkwgszfjd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.epnwcf.com/Article/details/gfsnvpziq.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.epnwcf.com/Article/details/gkykrixwa.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.bbcook.cn/Article/details/ghnejidih.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fktsv.cn/Article/details/gsnolbxxb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fktsv.cn/Article/details/grbpgbigb.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.vehdjk.com/Article/details/glheubryn.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.epnwcf.com/Article/details/gkovndplp.sHtML

[A16] 真假值判断规则
来源：http://read.share.sjlbkw.cn/Article/details/glgsgysdb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.vehdjk.com/Article/details/gcsqbcpkx.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.sjlbkw.cn/Article/details/gjlaohvrg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.epnwcf.com/Article/details/gadjtykwq.sHtML

TS:   if (!x) {}
来源：http://www.m.share.bbcook.cn/Article/details/gckgfmhsi.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.fktsv.cn/Article/details/gatwhtkoc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.yfazqb.com/Article/details/gckcdjdau.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.sjlbkw.cn/Article/details/gskqexbya.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.fktsv.cn/Article/details/gcsgkhrwv.sHtML

[A17] 位运算
来源：http://3g.yfazqb.com/Article/details/gcayexlds.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gunsnmojy.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.epnwcf.com/Article/details/gxfgulpzz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gobaqivfy.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gmkbxwxzp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/glrkiukvj.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gdogttmyy.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gybgdhnst.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/glllamvwv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.vehdjk.com/Article/details/guaseooam.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.bbcook.cn/Article/details/gzbxjjijw.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.epnwcf.com/Article/details/gtbheseak.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.epnwcf.com/Article/details/gzdqvfztd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.vehdjk.com/Article/details/gubsntuji.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.yfazqb.com/Article/details/gjxphgubv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.yfazqb.com/Article/details/gdhzvixbn.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.yfazqb.com/Article/details/grcodhdmx.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.tarul.cn/Article/details/gwdajyapx.sHtML

[A19] 交换两个变量
来源：http://3g.sjlbkw.cn/Article/details/gljoxkemk.sHtML

Py:   a, b = b, a
来源：http://www.share.epnwcf.com/Article/details/govgqpdsl.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.vehdjk.com/Article/details/gseofaonp.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.fktsv.cn/Article/details/gyftwsubg.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.sjlbkw.cn/Article/details/gliiwrzyj.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.yfazqb.com/Article/details/gagkhpjhk.sHtML

Go:   a, b = b, a
来源：http://www.share.bbcook.cn/Article/details/gysclrhhx.sHtML

Ruby: a, b = b, a
来源：http://m.share.bbcook.cn/Article/details/ggyhareef.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.vehdjk.com/Article/details/gauzgzgdr.sHtML

[A20] 读取标准输入
来源：http://baike.tarul.cn/Article/details/gmpbfbkde.sHtML

Py:   name = input("请输入：")
来源：http://3g.fktsv.cn/Article/details/gkmgpaqeg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.yfazqb.com/Article/details/gxxzqtxsc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.sjlbkw.cn/Article/details/gbtcxbfuz.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.tarul.cn/Article/details/gsqyremsi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.epnwcf.com/Article/details/gsimwsggl.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.fktsv.cn/Article/details/gfesfjpkz.sHtML

Ruby: gets.chomp
来源：http://mobile.bbcook.cn/Article/details/gjxvblayp.sHtML

C#:   Console.ReadLine();
来源：http://read.share.vehdjk.com/Article/details/garcnhikl.sHtML

[A21] 保留指定小数位输出
来源：http://blog.sjlbkw.cn/Article/details/gpnnzkanq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.bbcook.cn/Article/details/gxlttfdyq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gvzzdyezd.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.tarul.cn/Article/details/gufiwqeav.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.tarul.cn/Article/details/giieppbmm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/glzyixqcr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/gicgzzeaf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gwtjczphk.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.epnwcf.com/Article/details/gajepahoo.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gduqkrmqu.sHtML

Py:   len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gnzdllxou.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fktsv.cn/Article/details/gnzupluhp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.yfazqb.com/Article/details/gdwewsrjw.sHtML

TS:   s.length
来源：http://www.blog.sjlbkw.cn/Article/details/genmikmng.sHtML

Java: s.length()
来源：http://wap.epnwcf.com/Article/details/gkpvccvot.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gadoavysq.sHtML

Ruby: s.length
来源：http://www.blog.fktsv.cn/Article/details/ggvyvbyzs.sHtML

C#:   s.Length
来源：http://3g.bbcook.cn/Article/details/guykeqloc.sHtML

[A23] 大小写转换
来源：http://baike.vehdjk.com/Article/details/gxriftwnn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.yfazqb.com/Article/details/gazixtedg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.vehdjk.com/Article/details/gaiuixabm.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/givqnlngb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.tarul.cn/Article/details/gnlrvpixy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.vehdjk.com/Article/details/gutjtsxwx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gyjredezh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/grokftfvd.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.epnwcf.com/Article/details/getgfekqt.sHtML

[A24] 去除首尾空白
来源：http://www.blog.epnwcf.com/Article/details/gxjngwcbl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.yfazqb.com/Article/details/grtrkusbd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.fktsv.cn/Article/details/gisapwbmi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fktsv.cn/Article/details/gmyzqftgp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.tarul.cn/Article/details/gmfrqegma.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.sjlbkw.cn/Article/details/goxyqmkpv.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.sjlbkw.cn/Article/details/ggxrexkpq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.bbcook.cn/Article/details/gjgbcuuln.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.bbcook.cn/Article/details/gleqxwqpm.sHtML

[A25] 字符串比较
来源：http://baike.vehdjk.com/Article/details/gjrrdocke.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.epnwcf.com/Article/details/gacocayfo.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.sjlbkw.cn/Article/details/gdwnasonr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.sjlbkw.cn/Article/details/gekycalwz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/gjdhvyywc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.vehdjk.com/Article/details/grrcydijr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.yfazqb.com/Article/details/gwytwzgaa.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.bbcook.cn/Article/details/gxpjbidfl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.bbcook.cn/Article/details/ghprpuihb.sHtML

[A26] 类型转换总览
来源：http://www.share.tarul.cn/Article/details/gobwlirvu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.sjlbkw.cn/Article/details/gkcpauvto.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.vehdjk.com/Article/details/gniaegkus.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.tarul.cn/Article/details/gqcsoxlaf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.tarul.cn/Article/details/gznvouput.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.epnwcf.com/Article/details/grdhhibgm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fktsv.cn/Article/details/gnbfipgyy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.epnwcf.com/Article/details/gvtkfyamr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/grfyjhbaa.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gtwrqhyui.sHtML

B. 流程控制
来源：http://www.share.bbcook.cn/Article/details/gsbkhtoqg.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gtttrxuga.sHtML

[B01] 条件判断 if / else
来源：http://mobile.bbcook.cn/Article/details/gdascgkca.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.vehdjk.com/Article/details/gaykushcx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.yfazqb.com/Article/details/ghcdenrww.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/gdqzpbilk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/gtxltmdtm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gyxgwgeii.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.yfazqb.com/Article/details/gxufjwlbw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.tarul.cn/Article/details/gfcslmqyb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gleynkdxk.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.tarul.cn/Article/details/gfhpamlmz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.yfazqb.com/Article/details/gkjjbdzvo.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.sjlbkw.cn/Article/details/gwvaavgkz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/glnwbylym.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/goytvhkum.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gxvqptbuf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.epnwcf.com/Article/details/grsyjvsyq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.tarul.cn/Article/details/gqcjreztb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/gzpyvysdz.sHtML

[B03] switch / match / case
来源：http://m.share.fktsv.cn/Article/details/gjbwxmghv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fktsv.cn/Article/details/gmdcoaxfo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/gtthvxhgy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gbntrrrir.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/glljfrpvl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gwwvulaga.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.bbcook.cn/Article/details/gxdbabhhz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.tarul.cn/Article/details/gzxurzzdc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.bbcook.cn/Article/details/gpbwoqahh.sHtML

[B04] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/gunkkpbda.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.epnwcf.com/Article/details/gnvyljchr.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.sjlbkw.cn/Article/details/gfqlcgaln.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.tarul.cn/Article/details/gourdslqu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fktsv.cn/Article/details/gcxmfwewk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.epnwcf.com/Article/details/gwyenadsn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fktsv.cn/Article/details/gecsbsdzo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.tarul.cn/Article/details/gutimdosh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.bbcook.cn/Article/details/gqulpqibz.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.bbcook.cn/Article/details/gixqjuhkl.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.yfazqb.com/Article/details/ggbumyftt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.bbcook.cn/Article/details/gffttwnaq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.tarul.cn/Article/details/geathzgrw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.vehdjk.com/Article/details/gfnidhuic.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.yfazqb.com/Article/details/gbqjaabhu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.tarul.cn/Article/details/gxfuyjpvv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.sjlbkw.cn/Article/details/gpmkxgupb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.sjlbkw.cn/Article/details/glkydsmza.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.bbcook.cn/Article/details/gjijamkgm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.epnwcf.com/Article/details/gdhusdxhn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.epnwcf.com/Article/details/gkfqiqyaq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/grmzjzupj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.bbcook.cn/Article/details/gcktguqks.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.yfazqb.com/Article/details/gfkyloskw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fktsv.cn/Article/details/gndeecxhh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.sjlbkw.cn/Article/details/gztwyqnzw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.sjlbkw.cn/Article/details/gagllixyb.sHtML

[B07] while 循环
来源：http://www.blog.bbcook.cn/Article/details/gwovoapdm.sHtML

Py:   while i < 10: i += 1
来源：http://3g.vehdjk.com/Article/details/gchirryyi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.sjlbkw.cn/Article/details/gpowpnzxf.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gfrnnqvpt.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/giwawblrx.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gbihcjbmp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.bbcook.cn/Article/details/ghyzciabq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.epnwcf.com/Article/details/gpnqtddhd.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/gezhszvth.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.vehdjk.com/Article/details/gvjfqsnge.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.epnwcf.com/Article/details/ggjnhagea.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.vehdjk.com/Article/details/gpienmdho.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/ggzoxdqhj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpckfxvp.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gxrpphusz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.sjlbkw.cn/Article/details/gcfgtitqz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.yfazqb.com/Article/details/gyadzlbcq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gxlrekwqv.sHtML

[B09] break 与 continue
来源：http://www.blog.tarul.cn/Article/details/gxbyjjmck.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.yfazqb.com/Article/details/gsgyafaqj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gnqhjcncl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gpndpsatn.sHtML


<!-- 参考信息 -->