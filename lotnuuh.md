代发 wailian999

[A02] 变量声明与赋值
来源：http://blog.fktsv.cn/Article/details/gzsfcbqci.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.bbcook.cn/Article/details/gimrhbpmg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.vehdjk.com/Article/details/gnttqtagb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.tarul.cn/Article/details/gpyyqhqgc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.vehdjk.com/Article/details/gdizqnece.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.bbcook.cn/Article/details/geavbjdvt.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fktsv.cn/Article/details/ghabsemrl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.sjlbkw.cn/Article/details/gusktiwxs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.vehdjk.com/Article/details/gqyarckim.sHtML

[A03] 常量定义
来源：http://baike.epnwcf.com/Article/details/gyaagptrj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.epnwcf.com/Article/details/glciqruhr.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gbxfehsft.sHtML

JS:   const PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gtoaavpmv.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.tarul.cn/Article/details/gkeanktjn.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gojnaugzo.sHtML

Go:   const PI = 3.14159
来源：http://3g.fktsv.cn/Article/details/gzzibyhsx.sHtML

Ruby: PI = 3.14159
来源：http://www.share.bbcook.cn/Article/details/gyhgfhjvp.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gsornlbvt.sHtML

[A04] 判断变量类型
来源：http://blog.fktsv.cn/Article/details/gqujasnkr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.sjlbkw.cn/Article/details/gwdkbkijb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fktsv.cn/Article/details/goovsioqy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fktsv.cn/Article/details/geqbluulh.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.yfazqb.com/Article/details/gddulyclf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.yfazqb.com/Article/details/gwjzpajzm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.sjlbkw.cn/Article/details/gbisidnqe.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.vehdjk.com/Article/details/guhizzppn.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.tarul.cn/Article/details/gvamazbul.sHtML

[A05] 整数除法与取模
来源：http://blog.epnwcf.com/Article/details/gavjunjje.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fktsv.cn/Article/details/gigmehzfi.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.bbcook.cn/Article/details/golwvytxc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fktsv.cn/Article/details/ghhwmzseg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gqrmsneno.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gyivvupom.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gnccshbpm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gtwxfarty.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/gdcuyxjnu.sHtML

[A06] 字符串转数字
来源：http://blog.sjlbkw.cn/Article/details/gzhydvrjw.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.vehdjk.com/Article/details/gmgobhiyr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.yfazqb.com/Article/details/gingqwpsz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.epnwcf.com/Article/details/gqiniitqu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.yfazqb.com/Article/details/grzsqqycg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.sjlbkw.cn/Article/details/gkdatnlcn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.sjlbkw.cn/Article/details/gduyxwlio.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.tarul.cn/Article/details/ggvqtzoqr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.vehdjk.com/Article/details/getmuczun.sHtML

[A07] 数字转字符串
来源：http://blog.epnwcf.com/Article/details/gvxzxdsum.sHtML

Py:   str(42)
来源：http://mobile.tarul.cn/Article/details/gleawlvnw.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.sjlbkw.cn/Article/details/gqbkpayqs.sHtML

JS:   String(42); (42).toString()
来源：http://wap.yfazqb.com/Article/details/gefsoitot.sHtML

TS:   String(42)
来源：http://www.m.share.epnwcf.com/Article/details/guhwgntph.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.epnwcf.com/Article/details/gnaiwiquq.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.bbcook.cn/Article/details/gmzsmdkoc.sHtML

Ruby: 42.to_s
来源：http://www.share.fktsv.cn/Article/details/gqowqwlah.sHtML

C#:   42.ToString()
来源：http://3g.yfazqb.com/Article/details/gebmoezyv.sHtML

[A08] 取整与四舍五入
来源：http://3g.yfazqb.com/Article/details/gwxqrgnaq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/gcxsuwvoi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.yfazqb.com/Article/details/gcvgemvdc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/gdwzxmahy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.tarul.cn/Article/details/grlzcgyou.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fktsv.cn/Article/details/gomphhgac.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.tarul.cn/Article/details/ggskeitib.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.sjlbkw.cn/Article/details/gkktblqhz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.vehdjk.com/Article/details/gqctdejat.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fktsv.cn/Article/details/ggxoctkkv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gbewdavqx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gkznwykvh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.tarul.cn/Article/details/gymyfnotl.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gaqtavnpx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.epnwcf.com/Article/details/gbathllhk.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.yfazqb.com/Article/details/gihepkeem.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.vehdjk.com/Article/details/gflspjkyb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gjtkatdnk.sHtML

[A10] 生成随机数
来源：http://www.share.yfazqb.com/Article/details/gajedimmq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.bbcook.cn/Article/details/gxbbdodjc.sHtML

PHP:  random_int(1, 100);
来源：http://blog.yfazqb.com/Article/details/gboskcjqk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.tarul.cn/Article/details/goujohhkc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.tarul.cn/Article/details/ghikmdydy.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fktsv.cn/Article/details/guwzdmugy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.yfazqb.com/Article/details/gqfxfdipk.sHtML

Ruby: rand(1..100)
来源：http://baike.fktsv.cn/Article/details/guepuuqkg.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.epnwcf.com/Article/details/gxfeliohj.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.vehdjk.com/Article/details/gxzcvasgp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.vehdjk.com/Article/details/gcctmiaae.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.bbcook.cn/Article/details/gmdzwkrur.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.vehdjk.com/Article/details/ghaofvdyy.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/ggvidnmvi.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gqysflopq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.yfazqb.com/Article/details/gfmbihoye.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fktsv.cn/Article/details/gbjkjjyph.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.vehdjk.com/Article/details/gyolzlhzm.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.tarul.cn/Article/details/gsdgwzpri.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.epnwcf.com/Article/details/gpucbjddw.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.sjlbkw.cn/Article/details/gsnllsmlv.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.bbcook.cn/Article/details/gowibdmvq.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.sjlbkw.cn/Article/details/gxqfmhyib.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.epnwcf.com/Article/details/gaievszbf.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fktsv.cn/Article/details/gmhkezsic.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.bbcook.cn/Article/details/gvcvegdhe.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.epnwcf.com/Article/details/gqvkotgvx.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.epnwcf.com/Article/details/ganztaynj.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gcrqhfmnh.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/giouwvaek.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/govupihhb.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gumhpmskx.sHtML

Java: "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gecatgojk.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gpwfchaun.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gwmvwqdyj.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gormaodpq.sHtML

[A14] 注释写法
来源：http://www.blog.epnwcf.com/Article/details/gkayfunaj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.yfazqb.com/Article/details/gqacwluay.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.yfazqb.com/Article/details/gykquvqey.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fktsv.cn/Article/details/gbubihhqm.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwhfarfa.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.tarul.cn/Article/details/gdisjpgft.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gaisuvlrs.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.vehdjk.com/Article/details/gtxxrqyrl.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/gulfmmdeo.sHtML

[A15] 空值判断与默认值
来源：http://blog.epnwcf.com/Article/details/gdrstcbgc.sHtML

Py:   value = data or "默认值"
来源：http://blog.bbcook.cn/Article/details/ghoasidvh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.yfazqb.com/Article/details/gfxsrueov.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fktsv.cn/Article/details/gjzgglkrr.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/godmousmm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.epnwcf.com/Article/details/gitsvaqom.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.yfazqb.com/Article/details/geivzbthx.sHtML

Ruby: value = data || "默认值"
来源：http://blog.yfazqb.com/Article/details/gbzkkibok.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fktsv.cn/Article/details/gasxufqpn.sHtML

[A16] 真假值判断规则
来源：http://www.blog.tarul.cn/Article/details/gzrpwvdua.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.sjlbkw.cn/Article/details/gvwltoeep.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.vehdjk.com/Article/details/gagerkxez.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.epnwcf.com/Article/details/gsswwrogh.sHtML

TS:   if (!x) {}
来源：http://read.share.tarul.cn/Article/details/gznzaqxvq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.vehdjk.com/Article/details/gpqbsuiyx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.yfazqb.com/Article/details/gwvtiwfzt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.vehdjk.com/Article/details/gtzrfsarg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.bbcook.cn/Article/details/gpffqsyii.sHtML

[A17] 位运算
来源：http://mobile.epnwcf.com/Article/details/gnmddofsp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/gpapattwf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.tarul.cn/Article/details/gxmchdgrk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gexneuhpy.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gvjqxrizo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gzjmctogw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gpfpppcqz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gfmmqzyze.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gtxledubf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.epnwcf.com/Article/details/gcbywshtr.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fktsv.cn/Article/details/ggeemfgdd.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.bbcook.cn/Article/details/gdajpwxdu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fktsv.cn/Article/details/gcdogyegk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.sjlbkw.cn/Article/details/gghokthcu.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.epnwcf.com/Article/details/grfsyjbxs.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.yfazqb.com/Article/details/gkrcnrwus.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.tarul.cn/Article/details/grgjfhwff.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.fktsv.cn/Article/details/gqooodtls.sHtML

[A19] 交换两个变量
来源：http://www.share.fktsv.cn/Article/details/gfntzkktv.sHtML

Py:   a, b = b, a
来源：http://baike.tarul.cn/Article/details/glukelegd.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.vehdjk.com/Article/details/gzopvaswc.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.tarul.cn/Article/details/gllsxyutv.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.sjlbkw.cn/Article/details/gkhqnzqqw.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.bbcook.cn/Article/details/gsptblewq.sHtML

Go:   a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/ghfxnvohj.sHtML

Ruby: a, b = b, a
来源：http://wap.yfazqb.com/Article/details/gxbjfqdbz.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvxigyxx.sHtML

[A20] 读取标准输入
来源：http://www.share.vehdjk.com/Article/details/gddfjrkvn.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fktsv.cn/Article/details/gqpdwdyqh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.epnwcf.com/Article/details/gzlhbhvcf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.fktsv.cn/Article/details/gjqmodtws.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.tarul.cn/Article/details/gqnevcqom.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.vehdjk.com/Article/details/gvggdtjyj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.bbcook.cn/Article/details/gdtgxrukc.sHtML

Ruby: gets.chomp
来源：http://m.share.tarul.cn/Article/details/gtcdqidbv.sHtML

C#:   Console.ReadLine();
来源：http://www.share.tarul.cn/Article/details/gbxsavluo.sHtML

[A21] 保留指定小数位输出
来源：http://baike.bbcook.cn/Article/details/gndsctxhq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.yfazqb.com/Article/details/gmnozdfmt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/gbquklrzj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gsmxjxrsi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.vehdjk.com/Article/details/gbuwrwgjf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gxvvlsdzc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gngcwqllo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.tarul.cn/Article/details/gegdazsnr.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.tarul.cn/Article/details/gxwrudxus.sHtML

[A22] 获取字符串长度
来源：http://baike.vehdjk.com/Article/details/grvhegavg.sHtML

Py:   len(s)
来源：http://m.share.fktsv.cn/Article/details/gbkdhatar.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.tarul.cn/Article/details/gbjzzbqoe.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fktsv.cn/Article/details/gusprmjaq.sHtML

TS:   s.length
来源：http://www.m.share.yfazqb.com/Article/details/gufpmfazh.sHtML

Java: s.length()
来源：http://wap.bbcook.cn/Article/details/gtgmjsjmm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.vehdjk.com/Article/details/grlcxpefq.sHtML

Ruby: s.length
来源：http://wap.vehdjk.com/Article/details/gdnajkqjs.sHtML

C#:   s.Length
来源：http://baike.bbcook.cn/Article/details/gzrtvlvca.sHtML

[A23] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gcgzzkkxf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.bbcook.cn/Article/details/gzdugznfm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.bbcook.cn/Article/details/ghmfyesuu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/gtyvfafpd.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/gqsrywqwq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.bbcook.cn/Article/details/gypxtimgj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fktsv.cn/Article/details/gduoefznt.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.yfazqb.com/Article/details/gmtyusqbq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.tarul.cn/Article/details/grebbfhsd.sHtML

[A24] 去除首尾空白
来源：http://wap.sjlbkw.cn/Article/details/geprjaabc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fktsv.cn/Article/details/gyivyktxh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.bbcook.cn/Article/details/ggpejhdmo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.sjlbkw.cn/Article/details/gdhjgdldj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.bbcook.cn/Article/details/gaebhtqtx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.yfazqb.com/Article/details/gegoaqhhn.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.epnwcf.com/Article/details/ginpcaawc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fktsv.cn/Article/details/glvuirygp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gcgaophch.sHtML

[A25] 字符串比较
来源：http://read.share.fktsv.cn/Article/details/gpplniebb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.bbcook.cn/Article/details/glwveomzl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fktsv.cn/Article/details/gebdgtrco.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gynevdecy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.yfazqb.com/Article/details/giraunrqx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.bbcook.cn/Article/details/gqhcnuaxu.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.bbcook.cn/Article/details/glfmnivtx.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.tarul.cn/Article/details/gjcfkeokl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.sjlbkw.cn/Article/details/gujsdjcig.sHtML

[A26] 类型转换总览
来源：http://www.m.share.tarul.cn/Article/details/gldoqomhe.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.bbcook.cn/Article/details/gmdwetnnr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.vehdjk.com/Article/details/gjzxnzrsy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.tarul.cn/Article/details/getbcxxzz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.yfazqb.com/Article/details/gsqpzyjae.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fktsv.cn/Article/details/glrxvilhy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.sjlbkw.cn/Article/details/gcwgxyrto.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.sjlbkw.cn/Article/details/gkrbfzokl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.sjlbkw.cn/Article/details/gynniskef.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grioxaxqu.sHtML

B. 流程控制
来源：http://www.m.share.vehdjk.com/Article/details/gukhawbcr.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/grdtxsnme.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.bbcook.cn/Article/details/geyiaagos.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.bbcook.cn/Article/details/grcmmyqxj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.vehdjk.com/Article/details/gtqbsgbda.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/guhvonkcg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/gogxwrzlh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/gowiwlssn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.tarul.cn/Article/details/gnkqgshuk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.epnwcf.com/Article/details/gkgvsjajz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gkqazonbl.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.vehdjk.com/Article/details/glexcdcmc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.epnwcf.com/Article/details/gbugbqwta.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.yfazqb.com/Article/details/gigjexsyv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gqwnfdedr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gbfsgihls.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/gbqpqhlom.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.sjlbkw.cn/Article/details/gsjofobgt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.yfazqb.com/Article/details/gxdcrvsci.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gavxnamzu.sHtML

[B03] switch / match / case
来源：http://www.share.sjlbkw.cn/Article/details/gpzkdqasx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fktsv.cn/Article/details/gdqfojhej.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gjzzcfroy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gfpzrjmzn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glpvbxvjo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gpjuuqvnk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.sjlbkw.cn/Article/details/gquoakjij.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.yfazqb.com/Article/details/gmosxouzp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.vehdjk.com/Article/details/gopqquztb.sHtML

[B04] for 计数循环
来源：http://mobile.epnwcf.com/Article/details/gbwktopjd.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.epnwcf.com/Article/details/gckutittb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.epnwcf.com/Article/details/gazjqtykw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.yfazqb.com/Article/details/gzchukrwp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fktsv.cn/Article/details/gycfagdwd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.tarul.cn/Article/details/gudfpbcvd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.vehdjk.com/Article/details/gfguornkx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.yfazqb.com/Article/details/gnyoryhih.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fktsv.cn/Article/details/gvvklnnbv.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.bbcook.cn/Article/details/gibawhxob.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.epnwcf.com/Article/details/gsekxndjg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.bbcook.cn/Article/details/gbihudsnv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.tarul.cn/Article/details/gpkclxhgl.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.yfazqb.com/Article/details/gwxcmjneh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.yfazqb.com/Article/details/gcbqwwkno.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.yfazqb.com/Article/details/gdmnhquut.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.vehdjk.com/Article/details/gpiuykqub.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.yfazqb.com/Article/details/gfnaiwfgr.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.sjlbkw.cn/Article/details/gwsejfzwm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.yfazqb.com/Article/details/gzrrzbpez.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.vehdjk.com/Article/details/gzriekhmr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fktsv.cn/Article/details/gkvgynxpb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/gmazlckjb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.yfazqb.com/Article/details/gnhmdotur.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.sjlbkw.cn/Article/details/gkvafapet.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.epnwcf.com/Article/details/guooirmac.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.bbcook.cn/Article/details/gwiinaqjv.sHtML

[B07] while 循环
来源：http://www.blog.yfazqb.com/Article/details/gmzsgvzet.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.sjlbkw.cn/Article/details/gdfwjybsw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.tarul.cn/Article/details/gemqfnjlt.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gepiwmfmg.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gskadqpid.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gpjscczxq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.yfazqb.com/Article/details/gitncihwo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.yfazqb.com/Article/details/gnaqmbmyr.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/gmqikudxx.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.sjlbkw.cn/Article/details/gsbxohttw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.sjlbkw.cn/Article/details/gwslwvaed.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fktsv.cn/Article/details/ghyayuatf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/grlglbgcw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gsuprzlnz.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/gbnqfijuf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.yfazqb.com/Article/details/gwcbrtaha.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.yfazqb.com/Article/details/gtqthaill.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gaehpoign.sHtML


<!-- 参考信息 -->