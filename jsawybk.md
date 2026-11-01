代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gtbythyrv.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gmhviivvz.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gqskbfqqi.sHtML

Go:   const PI = 3.14159
来源：http://mobile.vehdjk.com/Article/details/grbugpllw.sHtML

Ruby: PI = 3.14159
来源：http://mobile.tarul.cn/Article/details/gtidwaxbm.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gbrzkbjxi.sHtML

[A04] 判断变量类型
来源：http://3g.tarul.cn/Article/details/gkllzrpdd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.sjlbkw.cn/Article/details/gbqlkjkrb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.epnwcf.com/Article/details/gqutiyhwg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.tarul.cn/Article/details/gqgkooqcn.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.sjlbkw.cn/Article/details/gedqutmrv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.epnwcf.com/Article/details/ghtytvzpt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.vehdjk.com/Article/details/gsgunlruv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.vehdjk.com/Article/details/ghmnwotdi.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.vehdjk.com/Article/details/gduverduq.sHtML

[A05] 整数除法与取模
来源：http://wap.yfazqb.com/Article/details/gjfnbwezq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.bbcook.cn/Article/details/goxienvcx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.bbcook.cn/Article/details/gbsooibud.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gkthfgvzb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gwkbqhdyw.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.vehdjk.com/Article/details/grxhawqzn.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/gpknaclpi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gdyfqyjov.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/ghbhzhvul.sHtML

[A06] 字符串转数字
来源：http://m.share.bbcook.cn/Article/details/gtdjwmdat.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.vehdjk.com/Article/details/gehuekudw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.epnwcf.com/Article/details/gcvyddypg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.epnwcf.com/Article/details/gxvxgkfjz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.sjlbkw.cn/Article/details/gxitkjgpl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.bbcook.cn/Article/details/gzckaqxti.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.epnwcf.com/Article/details/gflrcfxto.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.epnwcf.com/Article/details/ghuoaztbr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.vehdjk.com/Article/details/gysjkvriv.sHtML

[A07] 数字转字符串
来源：http://m.share.yfazqb.com/Article/details/gqajnphus.sHtML

Py:   str(42)
来源：http://blog.yfazqb.com/Article/details/gwpexnuqg.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.vehdjk.com/Article/details/ggarcdvjm.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.tarul.cn/Article/details/geiufbaub.sHtML

TS:   String(42)
来源：http://baike.epnwcf.com/Article/details/gpzixmrvy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fktsv.cn/Article/details/gauspgdlk.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fktsv.cn/Article/details/gompyhdjr.sHtML

Ruby: 42.to_s
来源：http://mobile.yfazqb.com/Article/details/ggqvilyfm.sHtML

C#:   42.ToString()
来源：http://baike.fktsv.cn/Article/details/gogcexslj.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fktsv.cn/Article/details/gblcfrtfw.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.tarul.cn/Article/details/goehjlmsh.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.vehdjk.com/Article/details/gviscvavg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.sjlbkw.cn/Article/details/grpzooknu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.yfazqb.com/Article/details/gmtdgeski.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.yfazqb.com/Article/details/gswuceyzj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/ggawabmqo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.vehdjk.com/Article/details/ghlnxikrg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.sjlbkw.cn/Article/details/gxlnqnvyh.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.yfazqb.com/Article/details/gdhyvqbxr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gpqlszboi.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gnfitzaal.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.fktsv.cn/Article/details/gesdrrfrv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gvvnhxvst.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.yfazqb.com/Article/details/gzalsjghx.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.tarul.cn/Article/details/ggesowbei.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.bbcook.cn/Article/details/gsuctmkew.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gejitzfjm.sHtML

[A10] 生成随机数
来源：http://www.blog.sjlbkw.cn/Article/details/gcuxpehgp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.yfazqb.com/Article/details/gbsjvzbvd.sHtML

PHP:  random_int(1, 100);
来源：http://wap.epnwcf.com/Article/details/gflpegeqw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.yfazqb.com/Article/details/gtjovmrgx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.yfazqb.com/Article/details/gxtknnywr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.tarul.cn/Article/details/glmojlkvv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.sjlbkw.cn/Article/details/gdhoefkbz.sHtML

Ruby: rand(1..100)
来源：http://read.share.epnwcf.com/Article/details/gxxghgzmv.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.vehdjk.com/Article/details/gpounkzlu.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.yfazqb.com/Article/details/gczskoqro.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.epnwcf.com/Article/details/glftwksce.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/gsgoegcjt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.epnwcf.com/Article/details/gtyjyrhpj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/ggsjyonqd.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.bbcook.cn/Article/details/gdugtqxva.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.sjlbkw.cn/Article/details/gmhqveyho.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.sjlbkw.cn/Article/details/gazktjmds.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/gmedyturl.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.bbcook.cn/Article/details/gugvmlymp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.bbcook.cn/Article/details/gyfrjavsp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fktsv.cn/Article/details/gsefbxsda.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.epnwcf.com/Article/details/gcyhrthrd.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.yfazqb.com/Article/details/gkfiqawid.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fktsv.cn/Article/details/gqdawybiz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fktsv.cn/Article/details/gqrznwkgv.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.yfazqb.com/Article/details/gptqnjczy.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fktsv.cn/Article/details/gzkmhrjjq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.bbcook.cn/Article/details/gxlwwoaca.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/gdrhvexyr.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/ggjaojnms.sHtML

JS:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gwttgtdrn.sHtML

TS:   "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/gjmymlejl.sHtML

Java: "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gzliicbtz.sHtML

Go:   "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gvjyijewx.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gqjnmdpyu.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gbtsnylmc.sHtML

[A14] 注释写法
来源：http://blog.epnwcf.com/Article/details/gaqyvdxkj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.sjlbkw.cn/Article/details/gbybwwxqv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.vehdjk.com/Article/details/gqqnsakes.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fktsv.cn/Article/details/ggmtnsoth.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gxtafuaql.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.sjlbkw.cn/Article/details/gstqqrsxc.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrtwgvju.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.sjlbkw.cn/Article/details/gthudfhkf.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gycfzjsmz.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.epnwcf.com/Article/details/gjwnxgdwe.sHtML

Py:   value = data or "默认值"
来源：http://baike.sjlbkw.cn/Article/details/gffrhaugv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.bbcook.cn/Article/details/ghqddkogk.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.sjlbkw.cn/Article/details/gdnkyvnbv.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.epnwcf.com/Article/details/gzrverrha.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.vehdjk.com/Article/details/ginocomdi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.sjlbkw.cn/Article/details/gwghkawtf.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.epnwcf.com/Article/details/grpmonwsg.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.sjlbkw.cn/Article/details/gkqgypxee.sHtML

[A16] 真假值判断规则
来源：http://m.share.epnwcf.com/Article/details/gwllqatwk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.vehdjk.com/Article/details/gyyokahtj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.tarul.cn/Article/details/gbjdlxkmq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.vehdjk.com/Article/details/gddfeqihv.sHtML

TS:   if (!x) {}
来源：http://m.share.yfazqb.com/Article/details/grdlnzvid.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.tarul.cn/Article/details/gmqevhoei.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.vehdjk.com/Article/details/gfwqjnfjw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.vehdjk.com/Article/details/gttfrpadg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.tarul.cn/Article/details/gxrtgusfl.sHtML

[A17] 位运算
来源：http://wap.sjlbkw.cn/Article/details/gefmsczug.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gczkueuap.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.epnwcf.com/Article/details/guituxiqz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/goyiwwrsx.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gtihwqgyd.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/ghvmfjwxv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gjegeosby.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gxtnbrypn.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gicbvhidm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.tarul.cn/Article/details/ghgwyjrbe.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.sjlbkw.cn/Article/details/gbseadizu.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.sjlbkw.cn/Article/details/guduywxeh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.vehdjk.com/Article/details/gdtwumymb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.bbcook.cn/Article/details/gkkgcftrc.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxylajph.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.bbcook.cn/Article/details/gbuzigtog.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.epnwcf.com/Article/details/glwxolgco.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.vehdjk.com/Article/details/gpguvlqiy.sHtML

[A19] 交换两个变量
来源：http://blog.epnwcf.com/Article/details/gclystggd.sHtML

Py:   a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/gnnrfremx.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.yfazqb.com/Article/details/glcgtydfj.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.bbcook.cn/Article/details/gwnaoppho.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.yfazqb.com/Article/details/gifitfmcy.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.vehdjk.com/Article/details/gefthvrwu.sHtML

Go:   a, b = b, a
来源：http://mobile.epnwcf.com/Article/details/gtrokxcfg.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.vehdjk.com/Article/details/gcsyfbekk.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.tarul.cn/Article/details/gplhhlqnc.sHtML

[A20] 读取标准输入
来源：http://wap.yfazqb.com/Article/details/gmtzaonoy.sHtML

Py:   name = input("请输入：")
来源：http://mobile.bbcook.cn/Article/details/govxgmnyk.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.vehdjk.com/Article/details/gymfjgdcp.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.epnwcf.com/Article/details/gcpgnikyg.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.vehdjk.com/Article/details/gmdfncvtv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.sjlbkw.cn/Article/details/gjxpuwjdq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.sjlbkw.cn/Article/details/gbrlhcplg.sHtML

Ruby: gets.chomp
来源：http://blog.bbcook.cn/Article/details/gapscndpe.sHtML

C#:   Console.ReadLine();
来源：http://wap.yfazqb.com/Article/details/guclufvwl.sHtML

[A21] 保留指定小数位输出
来源：http://wap.yfazqb.com/Article/details/gcgrxtbso.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.sjlbkw.cn/Article/details/gxdsrrcqu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.vehdjk.com/Article/details/gbbaaqqwp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/gjhiinjqi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.fktsv.cn/Article/details/gzrvuivzj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/ggurmtjpf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/gvogpavkn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gnpftjmqk.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.vehdjk.com/Article/details/gjseslpvr.sHtML

[A22] 获取字符串长度
来源：http://wap.vehdjk.com/Article/details/guioutpjz.sHtML

Py:   len(s)
来源：http://www.m.share.fktsv.cn/Article/details/ghgsgallm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.bbcook.cn/Article/details/gxxhejhpv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.tarul.cn/Article/details/gehefbtop.sHtML

TS:   s.length
来源：http://blog.bbcook.cn/Article/details/gopltfgxd.sHtML

Java: s.length()
来源：http://m.share.epnwcf.com/Article/details/geatmkjmn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.bbcook.cn/Article/details/gntiqoaib.sHtML

Ruby: s.length
来源：http://blog.yfazqb.com/Article/details/gummvyvcf.sHtML

C#:   s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gnhepjsbi.sHtML

[A23] 大小写转换
来源：http://baike.tarul.cn/Article/details/gvtnyndqi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.vehdjk.com/Article/details/gigglhiyw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.sjlbkw.cn/Article/details/gnroplnjy.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fktsv.cn/Article/details/ggounfzfo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.epnwcf.com/Article/details/gkyzpgmnc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.tarul.cn/Article/details/gaofajkgt.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.yfazqb.com/Article/details/gzafgljrv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.yfazqb.com/Article/details/gpikpnydv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.epnwcf.com/Article/details/gsrynkmav.sHtML

[A24] 去除首尾空白
来源：http://3g.tarul.cn/Article/details/gjfftbsul.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.tarul.cn/Article/details/gpaystdei.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.sjlbkw.cn/Article/details/gbeggnkue.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzslgwyo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.epnwcf.com/Article/details/gotsaqplz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.tarul.cn/Article/details/gxkwhrhqr.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.bbcook.cn/Article/details/grikjorow.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.bbcook.cn/Article/details/gjmpsbcdg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.sjlbkw.cn/Article/details/gqlfmrnid.sHtML

[A25] 字符串比较
来源：http://wap.vehdjk.com/Article/details/gsqcedekf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.yfazqb.com/Article/details/gflqajqmi.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.sjlbkw.cn/Article/details/ghnqtyrix.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.vehdjk.com/Article/details/guyjexicg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.tarul.cn/Article/details/gqwzpfvzu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gepzrkyyf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fktsv.cn/Article/details/gmxyelqcm.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.yfazqb.com/Article/details/gkeuvynyx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.epnwcf.com/Article/details/glnbmpgmq.sHtML

[A26] 类型转换总览
来源：http://m.share.vehdjk.com/Article/details/gtzikwjkv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.vehdjk.com/Article/details/gjzwoloez.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.epnwcf.com/Article/details/grjjtyevk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.epnwcf.com/Article/details/gqfhojmfr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.yfazqb.com/Article/details/gvswydvqk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fktsv.cn/Article/details/gvvvuayce.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.vehdjk.com/Article/details/glddasjou.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fktsv.cn/Article/details/gtvrljzod.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.vehdjk.com/Article/details/gxnqiruts.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gsagbibsa.sHtML

B. 流程控制
来源：http://baike.bbcook.cn/Article/details/gktkpiywu.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glvacbpvq.sHtML

[B01] 条件判断 if / else
来源：http://read.share.bbcook.cn/Article/details/gyruukrub.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.yfazqb.com/Article/details/gbydhtgvu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.tarul.cn/Article/details/gsthhxzau.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gbmifsnzu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gbruwpucu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/giygtioge.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fktsv.cn/Article/details/gdxwmakhi.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fktsv.cn/Article/details/gbajoiktu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/gnkfmckcc.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.vehdjk.com/Article/details/gmfychtyk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.tarul.cn/Article/details/grensjhwa.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.sjlbkw.cn/Article/details/guttvaphf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gwsevoroz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gyoksrjmb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gvsopoxqp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.vehdjk.com/Article/details/grmutdpfu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fktsv.cn/Article/details/gfhxjtquv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/ghvghprjk.sHtML

[B03] switch / match / case
来源：http://www.m.share.bbcook.cn/Article/details/gvwpqjszm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.epnwcf.com/Article/details/giohpqgew.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.tarul.cn/Article/details/gkagcpngq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gksqgzhkt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gfgbhgozh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gczoifgkl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.yfazqb.com/Article/details/girlarhry.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.sjlbkw.cn/Article/details/gqehrgldz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.yfazqb.com/Article/details/gnrvxtatk.sHtML

[B04] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gopqhdltl.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fktsv.cn/Article/details/gemcbtprn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.sjlbkw.cn/Article/details/gfjlwyjma.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.tarul.cn/Article/details/gqbjvzwrq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.epnwcf.com/Article/details/gcwsihnli.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.epnwcf.com/Article/details/gwtzltyjf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.yfazqb.com/Article/details/gnevdlbjy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.epnwcf.com/Article/details/gwqiweidm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.bbcook.cn/Article/details/gskckizhu.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fktsv.cn/Article/details/grwmaaxbz.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.tarul.cn/Article/details/gmgycfjga.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.tarul.cn/Article/details/gymjmfbgs.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.tarul.cn/Article/details/gxeilqiep.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/gartvrddd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.yfazqb.com/Article/details/gqollonqz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.yfazqb.com/Article/details/gvqmrpegz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.vehdjk.com/Article/details/glndusbie.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gvjedstuf.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.yfazqb.com/Article/details/gqwnfxgkj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.yfazqb.com/Article/details/gkllfamzt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.vehdjk.com/Article/details/gptbomlgj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.sjlbkw.cn/Article/details/gvqigrcdj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/gqkxjgbnm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.vehdjk.com/Article/details/grnmmzksc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.epnwcf.com/Article/details/gzptkypls.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlgdfydl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.vehdjk.com/Article/details/grwedckws.sHtML

[B07] while 循环
来源：http://blog.tarul.cn/Article/details/gwkhioqap.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.vehdjk.com/Article/details/gahxtlpsc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.sjlbkw.cn/Article/details/gysdwfscj.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gtirlnoxs.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gdnwaavdp.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/gbyenvecv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.epnwcf.com/Article/details/gbmrbcsky.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.tarul.cn/Article/details/ggfaqdcrs.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gudltcjpe.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fktsv.cn/Article/details/gmtmkgebz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.epnwcf.com/Article/details/gogcwuoli.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fktsv.cn/Article/details/gvtwxbrak.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gyeqtlhqa.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/ggnpeulns.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gbkrxzgwf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.tarul.cn/Article/details/gscszzvhd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.tarul.cn/Article/details/gfqgnfust.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/grlfdzfen.sHtML

[B09] break 与 continue
来源：http://blog.vehdjk.com/Article/details/gnmairzpd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.sjlbkw.cn/Article/details/gzhhojiqh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gogcasbyk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gxofxobtf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gowvefazw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gobxbyzkw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gqfihnqfb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.vehdjk.com/Article/details/gttcweddg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/ghkoovydo.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.tarul.cn/Article/details/gstenoszf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fktsv.cn/Article/details/gnoxfphzl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.sjlbkw.cn/Article/details/gotqpjaox.sHtML


<!-- 参考信息 -->