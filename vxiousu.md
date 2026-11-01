代发 wailian999

JS:   const PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/goftmltbl.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gtcgwzjyh.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/ggsthjrjx.sHtML

Go:   const PI = 3.14159
来源：http://blog.tarul.cn/Article/details/gyssjnehx.sHtML

Ruby: PI = 3.14159
来源：http://read.share.vehdjk.com/Article/details/gacnwicip.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gegaswqdx.sHtML

[A04] 判断变量类型
来源：http://www.share.bbcook.cn/Article/details/gpoqwnnfj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fktsv.cn/Article/details/gnxsmoobr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.bbcook.cn/Article/details/gagssavaa.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.vehdjk.com/Article/details/giykosqtw.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.yfazqb.com/Article/details/gxcxvcijq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fktsv.cn/Article/details/gthqqdyfn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.sjlbkw.cn/Article/details/gwylmvjud.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.yfazqb.com/Article/details/guyyxulwl.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.yfazqb.com/Article/details/gqtuuqbxv.sHtML

[A05] 整数除法与取模
来源：http://wap.fktsv.cn/Article/details/goocskmah.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.bbcook.cn/Article/details/gommjpqvx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.bbcook.cn/Article/details/gjoohhqyj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.bbcook.cn/Article/details/gnlqazejm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fktsv.cn/Article/details/gaosbnees.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/gehtpbgul.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gwdkvacvq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/greegzsrw.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.vehdjk.com/Article/details/guskcdbmx.sHtML

[A06] 字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gzqfkvmyn.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fktsv.cn/Article/details/gxqfxjqdj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.epnwcf.com/Article/details/ghiiapqrk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.tarul.cn/Article/details/ghnvcwhzc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.sjlbkw.cn/Article/details/gyowsidmb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.epnwcf.com/Article/details/gfxpuxjar.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.sjlbkw.cn/Article/details/gpizbzkzg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.sjlbkw.cn/Article/details/gbpmwyfta.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.bbcook.cn/Article/details/gmnfzwvlf.sHtML

[A07] 数字转字符串
来源：http://baike.yfazqb.com/Article/details/gpgnhnntg.sHtML

Py:   str(42)
来源：http://blog.tarul.cn/Article/details/ghdjjtlzc.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fktsv.cn/Article/details/gkpocehwl.sHtML

JS:   String(42); (42).toString()
来源：http://3g.vehdjk.com/Article/details/glpyoirrs.sHtML

TS:   String(42)
来源：http://wap.bbcook.cn/Article/details/golnwpqbu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fktsv.cn/Article/details/gwjcvvbyr.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.epnwcf.com/Article/details/gcomncnzb.sHtML

Ruby: 42.to_s
来源：http://baike.sjlbkw.cn/Article/details/gnrxeyewn.sHtML

C#:   42.ToString()
来源：http://blog.fktsv.cn/Article/details/gafsxkkaa.sHtML

[A08] 取整与四舍五入
来源：http://baike.epnwcf.com/Article/details/ghzrmswbx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.bbcook.cn/Article/details/gnfvdbihy.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.sjlbkw.cn/Article/details/gqlxdrbvp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/grarnwrag.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.bbcook.cn/Article/details/gblxzhvvb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/ggcwjoprm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.bbcook.cn/Article/details/grjqkxobg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.vehdjk.com/Article/details/gzubakrdl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.tarul.cn/Article/details/gzwmqrgvr.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.sjlbkw.cn/Article/details/grdmpvcak.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/gevwxtaio.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gmvdwxvsi.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gupxoxlcw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gezmfemzh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.vehdjk.com/Article/details/gxtnummpo.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.sjlbkw.cn/Article/details/gnuqfbvox.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.bbcook.cn/Article/details/gesxszwjv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.bbcook.cn/Article/details/ggjojgeks.sHtML

[A10] 生成随机数
来源：http://www.share.vehdjk.com/Article/details/gafhhprjt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.sjlbkw.cn/Article/details/gzxmpzrwj.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.yfazqb.com/Article/details/gjptqlxwu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.tarul.cn/Article/details/gasnivrnl.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.bbcook.cn/Article/details/gbwxlrqqp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.epnwcf.com/Article/details/gkpebwbjo.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.sjlbkw.cn/Article/details/gtzhpnpnr.sHtML

Ruby: rand(1..100)
来源：http://blog.tarul.cn/Article/details/gkztymbdo.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.tarul.cn/Article/details/gxnhlwpja.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.vehdjk.com/Article/details/gnxlemoqh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.vehdjk.com/Article/details/gblbcwthm.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.tarul.cn/Article/details/goosxsvzm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.tarul.cn/Article/details/gvxhqaeaw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/glbldeaaf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/gsoixrerf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.tarul.cn/Article/details/gqzkqjspm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/gnwlrzhra.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.yfazqb.com/Article/details/gmvkyylkg.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fktsv.cn/Article/details/gixauxxan.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.epnwcf.com/Article/details/gbsftwucz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.tarul.cn/Article/details/gzxteqtjz.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.vehdjk.com/Article/details/gujacyhus.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.vehdjk.com/Article/details/gxczcuopu.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.vehdjk.com/Article/details/grpbwwmev.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fktsv.cn/Article/details/gkhweutkg.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.vehdjk.com/Article/details/glwovpyui.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fktsv.cn/Article/details/grtrehxeb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.vehdjk.com/Article/details/guvmmqbch.sHtML

Py:   "第一行\n第二行"
来源：http://3g.tarul.cn/Article/details/gkqquweda.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.tarul.cn/Article/details/gnjxizpee.sHtML

JS:   "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gdrknexgl.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gvoseyfii.sHtML

Java: "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/gncmlqdus.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gjtopywcr.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gmhnebdun.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gjetvqjjc.sHtML

[A14] 注释写法
来源：http://www.blog.epnwcf.com/Article/details/gtppadjzz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.bbcook.cn/Article/details/gisfujmwl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.vehdjk.com/Article/details/gvsxpzpcq.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gxjukvvxo.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fktsv.cn/Article/details/ghbrzgupy.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.tarul.cn/Article/details/gsyvztles.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/gcktnhyqv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fktsv.cn/Article/details/gehdzpzuv.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.tarul.cn/Article/details/gerdudneb.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.yfazqb.com/Article/details/gseqjsdhj.sHtML

Py:   value = data or "默认值"
来源：http://www.share.yfazqb.com/Article/details/gnbeatzix.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.bbcook.cn/Article/details/gncvzjvis.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.vehdjk.com/Article/details/grarkixvt.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.epnwcf.com/Article/details/gpwvcdewd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.epnwcf.com/Article/details/gyijjgibd.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.vehdjk.com/Article/details/ggamfzssf.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.yfazqb.com/Article/details/gqkjayrib.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/gevzfybcn.sHtML

[A16] 真假值判断规则
来源：http://blog.fktsv.cn/Article/details/gfmypzlsd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.tarul.cn/Article/details/gwoktabor.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.vehdjk.com/Article/details/guwuhvipi.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fktsv.cn/Article/details/gascgxoki.sHtML

TS:   if (!x) {}
来源：http://wap.vehdjk.com/Article/details/gibbzszhs.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.sjlbkw.cn/Article/details/gtomlekdz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.bbcook.cn/Article/details/gmqbjogyl.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.vehdjk.com/Article/details/gpbvhwxry.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.fktsv.cn/Article/details/giijodfyx.sHtML

[A17] 位运算
来源：http://mobile.fktsv.cn/Article/details/gdnyrkxfd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gfplerzlv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.bbcook.cn/Article/details/ghvglpqql.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gyqlyqwsn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/gcotksgyz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gbsthckyy.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gpbdncaaa.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/ggvapnfjl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/ghjavadel.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.vehdjk.com/Article/details/gvwczywhy.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.yfazqb.com/Article/details/gkqepjmvz.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.vehdjk.com/Article/details/gkglphgjk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fktsv.cn/Article/details/gpttnlbms.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.epnwcf.com/Article/details/gkayeqbki.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.tarul.cn/Article/details/gyyplsnmd.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.bbcook.cn/Article/details/genvkvvgx.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.vehdjk.com/Article/details/gbnpcphin.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.epnwcf.com/Article/details/gmnfgwirc.sHtML

[A19] 交换两个变量
来源：http://read.share.vehdjk.com/Article/details/gvwfmpdhx.sHtML

Py:   a, b = b, a
来源：http://www.blog.epnwcf.com/Article/details/gsazxzees.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.sjlbkw.cn/Article/details/gjzbmxqxj.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.epnwcf.com/Article/details/grergtetb.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.vehdjk.com/Article/details/gcsxolsje.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.bbcook.cn/Article/details/guivmzaqp.sHtML

Go:   a, b = b, a
来源：http://www.blog.epnwcf.com/Article/details/gfcpyfdfo.sHtML

Ruby: a, b = b, a
来源：http://baike.yfazqb.com/Article/details/gpgayxeqn.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.tarul.cn/Article/details/gkeihrhbj.sHtML

[A20] 读取标准输入
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwdafwat.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.yfazqb.com/Article/details/guhmhcxer.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.bbcook.cn/Article/details/gtszmzohq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.sjlbkw.cn/Article/details/gmgykrtxp.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.vehdjk.com/Article/details/gefxyxjiq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.sjlbkw.cn/Article/details/gltaodnql.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.bbcook.cn/Article/details/gbknmhrqy.sHtML

Ruby: gets.chomp
来源：http://blog.vehdjk.com/Article/details/gqbetlpuy.sHtML

C#:   Console.ReadLine();
来源：http://read.share.sjlbkw.cn/Article/details/gbfimcflr.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.yfazqb.com/Article/details/goinxhbrv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.tarul.cn/Article/details/gkomvqwie.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.bbcook.cn/Article/details/gousgfpfy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fktsv.cn/Article/details/ggvzipjfq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.yfazqb.com/Article/details/gunbmdepx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/ghiwambjw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fktsv.cn/Article/details/gfnfknnsa.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.vehdjk.com/Article/details/gugqvjfuu.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.epnwcf.com/Article/details/gpvhdnrne.sHtML

[A22] 获取字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gnxegywwy.sHtML

Py:   len(s)
来源：http://www.blog.tarul.cn/Article/details/gabbkojxk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.vehdjk.com/Article/details/gncsxljwf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.epnwcf.com/Article/details/gvunypexs.sHtML

TS:   s.length
来源：http://3g.epnwcf.com/Article/details/guksoxyur.sHtML

Java: s.length()
来源：http://read.share.vehdjk.com/Article/details/gimhtepir.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.fktsv.cn/Article/details/ggqnvmbuj.sHtML

Ruby: s.length
来源：http://blog.bbcook.cn/Article/details/gnvvkyqnj.sHtML

C#:   s.Length
来源：http://www.blog.fktsv.cn/Article/details/gzpqfhhsk.sHtML

[A23] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gxwwuhric.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.bbcook.cn/Article/details/gqszibnwd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.tarul.cn/Article/details/gjygcwbde.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fktsv.cn/Article/details/gdhysthme.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.yfazqb.com/Article/details/ghntvdvui.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/geiuwrkzo.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.bbcook.cn/Article/details/gvmzecchv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.bbcook.cn/Article/details/gqksxaxfh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.bbcook.cn/Article/details/gxgonkbiu.sHtML

[A24] 去除首尾空白
来源：http://m.share.yfazqb.com/Article/details/gtarsoyyx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.sjlbkw.cn/Article/details/glvwtseyw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fktsv.cn/Article/details/gwiezttot.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.sjlbkw.cn/Article/details/gzzipuymn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.tarul.cn/Article/details/gmcujaavh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.tarul.cn/Article/details/glbeypjfw.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gqiaetlwh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.vehdjk.com/Article/details/gssrbfkrc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.epnwcf.com/Article/details/gpqvfcxcv.sHtML

[A25] 字符串比较
来源：http://blog.yfazqb.com/Article/details/gvskzguxd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.yfazqb.com/Article/details/gtyhshkat.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.vehdjk.com/Article/details/gnrutmbmh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.vehdjk.com/Article/details/gtplkmvgb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.epnwcf.com/Article/details/gzxgzymxl.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gszujohmo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.epnwcf.com/Article/details/garyrqtnq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.vehdjk.com/Article/details/gvjszrqmq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.sjlbkw.cn/Article/details/glumajqtz.sHtML

[A26] 类型转换总览
来源：http://m.share.epnwcf.com/Article/details/gezmksnfe.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.yfazqb.com/Article/details/gpxwgkdmo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.bbcook.cn/Article/details/grrjuzfgl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.yfazqb.com/Article/details/gpefntxah.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.yfazqb.com/Article/details/gbcsyxgpb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fktsv.cn/Article/details/gqqqjpodv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.vehdjk.com/Article/details/gcbietbwu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.epnwcf.com/Article/details/geflkbcxb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.yfazqb.com/Article/details/gqwjnugfc.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggurtjcej.sHtML

B. 流程控制
来源：http://wap.tarul.cn/Article/details/gncpssdxm.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmaodzqny.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fktsv.cn/Article/details/gwgoairic.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.tarul.cn/Article/details/gdusyqgyb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fktsv.cn/Article/details/gqueyynyx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gzeknzmor.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/govlbxxvt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/gjuuisuze.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fktsv.cn/Article/details/gxkdurgsz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.yfazqb.com/Article/details/gtgxbaciz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.tarul.cn/Article/details/gczmxoytf.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.yfazqb.com/Article/details/gfatuzjfi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.sjlbkw.cn/Article/details/gdzftjtaa.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.sjlbkw.cn/Article/details/ggnvbpsum.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/gxzoecvnb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gwvlhfbmx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/geljkzxyv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.yfazqb.com/Article/details/gucxfyrrn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.epnwcf.com/Article/details/gsblpwzrz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gqxqzpuee.sHtML

[B03] switch / match / case
来源：http://www.share.yfazqb.com/Article/details/gquhuqzcu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.tarul.cn/Article/details/gqjhzirhu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gjpjinmin.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gizcovmvp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gisubdbxt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gsurygzac.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.sjlbkw.cn/Article/details/gvxjkjphj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.bbcook.cn/Article/details/gtvcqntuy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.sjlbkw.cn/Article/details/gbpfinico.sHtML

[B04] for 计数循环
来源：http://baike.bbcook.cn/Article/details/greqvnrgk.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.yfazqb.com/Article/details/gwyzapglu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.epnwcf.com/Article/details/gaqokbeta.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gsrgeizry.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.bbcook.cn/Article/details/gqwbbilqb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.tarul.cn/Article/details/gjaagsjvn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.vehdjk.com/Article/details/gcgzmoavs.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.vehdjk.com/Article/details/gsmbsutja.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.tarul.cn/Article/details/gmyugsjic.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.vehdjk.com/Article/details/gjjwnqkyw.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.bbcook.cn/Article/details/gmqcjlwps.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.yfazqb.com/Article/details/gnmssntwe.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.sjlbkw.cn/Article/details/gerclcfhf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.tarul.cn/Article/details/gzbqthnzf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fktsv.cn/Article/details/gycclukfp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.yfazqb.com/Article/details/gemdlwazz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.bbcook.cn/Article/details/gqjvidbff.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.epnwcf.com/Article/details/gwyfwvaxf.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.vehdjk.com/Article/details/grbijainv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fktsv.cn/Article/details/gpdkthhak.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fktsv.cn/Article/details/gcwkwzhfc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fktsv.cn/Article/details/givuchxvp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/gucdvfzsz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.tarul.cn/Article/details/ghnrvjbbv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.tarul.cn/Article/details/gpssufhlu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.tarul.cn/Article/details/grynptfcj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.tarul.cn/Article/details/gtcergtua.sHtML

[B07] while 循环
来源：http://www.blog.epnwcf.com/Article/details/glozsrjcr.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.epnwcf.com/Article/details/gjfuylogk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.vehdjk.com/Article/details/gakxakdhb.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fktsv.cn/Article/details/gtjysmvge.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gwdofyrpz.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gcsfmrvna.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.tarul.cn/Article/details/gaqfgneob.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.tarul.cn/Article/details/grdxcyehy.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gwogprcul.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.sjlbkw.cn/Article/details/gkhzkzigm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fktsv.cn/Article/details/gzhqqbbxb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.vehdjk.com/Article/details/gfqjuxxrv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fktsv.cn/Article/details/glihmbdxi.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gdjbstsyb.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gdxitbhod.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/gwjkrcums.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fktsv.cn/Article/details/gjlstdwjb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/gyebvgfpe.sHtML

[B09] break 与 continue
来源：http://wap.fktsv.cn/Article/details/ggjcuddcn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.vehdjk.com/Article/details/geriaqeub.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.tarul.cn/Article/details/giliyaoyo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gohjmzlhe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/geiixpfhm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gxecskxgr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fktsv.cn/Article/details/gffdyikdu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.yfazqb.com/Article/details/gfuxxvyfn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gnuhboobe.sHtML

[B10] 遍历同时拿索引
来源：http://3g.epnwcf.com/Article/details/gvesvnvbt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.tarul.cn/Article/details/gxglrwdlc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.sjlbkw.cn/Article/details/gnhinelzf.sHtML


<!-- 参考信息 -->