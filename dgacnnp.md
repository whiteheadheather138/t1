代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://3g.bbcook.cn/Article/details/geunvqfgx.sHtML

[A03] 常量定义
来源：http://www.blog.epnwcf.com/Article/details/gbuzvwydo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fktsv.cn/Article/details/gsvrzlgpy.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gdnyhscpr.sHtML

JS:   const PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/ghqqwgrdz.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gjrbyfcci.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gceavlsxe.sHtML

Go:   const PI = 3.14159
来源：http://wap.yfazqb.com/Article/details/gqyuuwmet.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.yfazqb.com/Article/details/grmedbcqk.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gcikvkunv.sHtML

[A04] 判断变量类型
来源：http://www.m.share.sjlbkw.cn/Article/details/garzzeyqv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.tarul.cn/Article/details/gkcwagoqw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.yfazqb.com/Article/details/grzmxjojr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.tarul.cn/Article/details/glqmjayft.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.vehdjk.com/Article/details/gjgpancxi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.vehdjk.com/Article/details/gxnvmbqkq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.sjlbkw.cn/Article/details/ggvgbeadi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.vehdjk.com/Article/details/groonnsie.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.sjlbkw.cn/Article/details/gtsdleess.sHtML

[A05] 整数除法与取模
来源：http://wap.bbcook.cn/Article/details/gfcofhihl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.bbcook.cn/Article/details/gqkxpxyhk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gkrrgcicu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gikiiodus.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gdgilobzo.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/glbihmbpp.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.tarul.cn/Article/details/grieevill.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/gdzncefgd.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/gypvmviwu.sHtML

[A06] 字符串转数字
来源：http://read.share.bbcook.cn/Article/details/guqdxtneo.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fktsv.cn/Article/details/gafkthain.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.bbcook.cn/Article/details/gmeuaqhhh.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.yfazqb.com/Article/details/gpeekufrj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.vehdjk.com/Article/details/gtgdyjaun.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.epnwcf.com/Article/details/gnbwtqsoi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.yfazqb.com/Article/details/ggisfgepk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fktsv.cn/Article/details/gmvsxnsze.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.tarul.cn/Article/details/glqkmgnkp.sHtML

[A07] 数字转字符串
来源：http://m.share.tarul.cn/Article/details/gmtzzntuo.sHtML

Py:   str(42)
来源：http://wap.bbcook.cn/Article/details/gvesfyyjx.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.tarul.cn/Article/details/gggdhanfj.sHtML

JS:   String(42); (42).toString()
来源：http://baike.epnwcf.com/Article/details/ghkwtsfif.sHtML

TS:   String(42)
来源：http://mobile.yfazqb.com/Article/details/gzefqyhhs.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.epnwcf.com/Article/details/gjkerepdh.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.yfazqb.com/Article/details/gntukqynq.sHtML

Ruby: 42.to_s
来源：http://3g.tarul.cn/Article/details/gjjbfactn.sHtML

C#:   42.ToString()
来源：http://www.blog.epnwcf.com/Article/details/gobpjjvdq.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.yfazqb.com/Article/details/gvuesaygl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/gybpqclvt.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.sjlbkw.cn/Article/details/gyvuwzufc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.sjlbkw.cn/Article/details/gbyojzwgx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.vehdjk.com/Article/details/gnhyojbth.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.yfazqb.com/Article/details/gxtoakacb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/gyvdqayhf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fktsv.cn/Article/details/gizpzxhqe.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/glnmnlivy.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.vehdjk.com/Article/details/gujiqpwcm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.tarul.cn/Article/details/gjqhrasvp.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/ghhenszhb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.tarul.cn/Article/details/gwirjlfhp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gzcssqxvt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.tarul.cn/Article/details/goeageant.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.sjlbkw.cn/Article/details/gfoiykmys.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.bbcook.cn/Article/details/gtptrwdzi.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.yfazqb.com/Article/details/gtemuweci.sHtML

[A10] 生成随机数
来源：http://mobile.yfazqb.com/Article/details/geprrlivv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.epnwcf.com/Article/details/gfqzrjhzc.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.vehdjk.com/Article/details/gszrjzjvy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.yfazqb.com/Article/details/gredrdntp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.yfazqb.com/Article/details/gxcmdgwyu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fktsv.cn/Article/details/gjbellwtl.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.yfazqb.com/Article/details/gygksldfg.sHtML

Ruby: rand(1..100)
来源：http://wap.sjlbkw.cn/Article/details/gwhrfcdka.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.tarul.cn/Article/details/gmjugoiqg.sHtML

[A11] 条件表达式（三元）
来源：http://baike.vehdjk.com/Article/details/gqspomfts.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.yfazqb.com/Article/details/gwvbfczqb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.tarul.cn/Article/details/gukbqywaz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.yfazqb.com/Article/details/gsfkspcam.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/gtbysllcx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/gaxthyalg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.yfazqb.com/Article/details/gyorswfps.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gfmhikvuz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/gbezihide.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.tarul.cn/Article/details/gmveafrhq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.bbcook.cn/Article/details/gmghbtasg.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhiduamx.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.sjlbkw.cn/Article/details/gaeklyrff.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.bbcook.cn/Article/details/gigpzcbdz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.yfazqb.com/Article/details/gttqzklkc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.bbcook.cn/Article/details/gdxkzzffd.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.sjlbkw.cn/Article/details/gifevrarb.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.yfazqb.com/Article/details/garqdvzwz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.tarul.cn/Article/details/giphqbqim.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/ggkkhkwif.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gvpjcxgru.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/gdfpoewhn.sHtML

TS:   "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/grfgifbth.sHtML

Java: "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gtvxjjsbd.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gcmoompxx.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gzobbeiqp.sHtML

C#:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gynloyjmp.sHtML

[A14] 注释写法
来源：http://www.blog.sjlbkw.cn/Article/details/grisntdfe.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fktsv.cn/Article/details/gnxnsqbgz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.tarul.cn/Article/details/guvjqecij.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/ggndgwnth.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.bbcook.cn/Article/details/gcmcjprck.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.yfazqb.com/Article/details/gidtbacbs.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/grhexnggb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.bbcook.cn/Article/details/gebfwwuja.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/gyflqcwki.sHtML

[A15] 空值判断与默认值
来源：http://read.share.tarul.cn/Article/details/gceehpnsf.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.vehdjk.com/Article/details/gjbdsrgwd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.vehdjk.com/Article/details/geurrjzqc.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.epnwcf.com/Article/details/gfudzglzd.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.sjlbkw.cn/Article/details/gmggscycd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.sjlbkw.cn/Article/details/gkqyfeqxk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.bbcook.cn/Article/details/ghbziijbi.sHtML

Ruby: value = data || "默认值"
来源：http://3g.bbcook.cn/Article/details/gldfkwnpg.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/gbopdykok.sHtML

[A16] 真假值判断规则
来源：http://3g.sjlbkw.cn/Article/details/grxwecwbn.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.sjlbkw.cn/Article/details/gdwovknev.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.bbcook.cn/Article/details/gnknbvbsx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.yfazqb.com/Article/details/gyegrzoun.sHtML

TS:   if (!x) {}
来源：http://m.share.vehdjk.com/Article/details/gvikmcdxw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.vehdjk.com/Article/details/gmajkgpiw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.bbcook.cn/Article/details/gpwcxcowd.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.tarul.cn/Article/details/ggxxyxpfw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gvnqrivmc.sHtML

[A17] 位运算
来源：http://www.blog.sjlbkw.cn/Article/details/gcjyizftz.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gagpdempq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.fktsv.cn/Article/details/gzjuoecml.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/grlrhlcdb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gpwogwzht.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gsbtwobhz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gokfgnnyh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/gsfycvfcq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/gmtbqtvua.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.tarul.cn/Article/details/ghbzfvptr.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.epnwcf.com/Article/details/ghppgfqoj.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.sjlbkw.cn/Article/details/guuusxgcv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.bbcook.cn/Article/details/gabpdcabz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.tarul.cn/Article/details/gdmjzuzcv.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.sjlbkw.cn/Article/details/gttaoidqe.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.epnwcf.com/Article/details/gqzidgrhw.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.yfazqb.com/Article/details/gmdqpsdqb.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.epnwcf.com/Article/details/gogajtzvm.sHtML

[A19] 交换两个变量
来源：http://baike.bbcook.cn/Article/details/gzfkbewlp.sHtML

Py:   a, b = b, a
来源：http://wap.bbcook.cn/Article/details/gimzsfern.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvvmhmrq.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.bbcook.cn/Article/details/gnqcyrosy.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.yfazqb.com/Article/details/gikptvfmf.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.yfazqb.com/Article/details/gxtjvdzap.sHtML

Go:   a, b = b, a
来源：http://read.share.sjlbkw.cn/Article/details/gmciqhccv.sHtML

Ruby: a, b = b, a
来源：http://m.share.yfazqb.com/Article/details/gugoqcmwj.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.epnwcf.com/Article/details/golcqwrxu.sHtML

[A20] 读取标准输入
来源：http://wap.fktsv.cn/Article/details/goceqvcok.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fktsv.cn/Article/details/gubulnbfc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fktsv.cn/Article/details/gzkcxuldu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.tarul.cn/Article/details/gtewqwmhj.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.epnwcf.com/Article/details/gbvmlvtal.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.epnwcf.com/Article/details/gwvbdmpux.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fktsv.cn/Article/details/gfefotequ.sHtML

Ruby: gets.chomp
来源：http://3g.sjlbkw.cn/Article/details/gdufzjjcy.sHtML

C#:   Console.ReadLine();
来源：http://baike.epnwcf.com/Article/details/gmqzzggvx.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.yfazqb.com/Article/details/glpukyqpc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.fktsv.cn/Article/details/gcjdpdfte.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.tarul.cn/Article/details/gjkszauwb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/gmkxyiggs.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gdtjrmpmz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/gpmzobxpc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.sjlbkw.cn/Article/details/grmaikyod.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/gpxjiirye.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.fktsv.cn/Article/details/genssfemu.sHtML

[A22] 获取字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/grwcnvarj.sHtML

Py:   len(s)
来源：http://mobile.yfazqb.com/Article/details/glweogiew.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.epnwcf.com/Article/details/gccasbixh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.sjlbkw.cn/Article/details/gfvaslanr.sHtML

TS:   s.length
来源：http://baike.yfazqb.com/Article/details/gnqxkzpsl.sHtML

Java: s.length()
来源：http://3g.sjlbkw.cn/Article/details/gklanrhmx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.bbcook.cn/Article/details/ghjukvexl.sHtML

Ruby: s.length
来源：http://read.share.vehdjk.com/Article/details/gpuryttis.sHtML

C#:   s.Length
来源：http://read.share.fktsv.cn/Article/details/gegjjifhv.sHtML

[A23] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/grbvqlgja.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.yfazqb.com/Article/details/gcmfjbsny.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.epnwcf.com/Article/details/gotkqbaxz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.yfazqb.com/Article/details/gexhlolgx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.vehdjk.com/Article/details/gotmnjorp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.vehdjk.com/Article/details/gdbenxugj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.yfazqb.com/Article/details/gbhdtjdbt.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.tarul.cn/Article/details/gcozeomyc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.bbcook.cn/Article/details/gecxwbfgm.sHtML

[A24] 去除首尾空白
来源：http://www.blog.bbcook.cn/Article/details/gegtmbsfa.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.tarul.cn/Article/details/gqgzwxzfi.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.sjlbkw.cn/Article/details/gtylsljjh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.vehdjk.com/Article/details/glxmbthmb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.epnwcf.com/Article/details/ghvaazjmg.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.bbcook.cn/Article/details/gygkqcglj.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.bbcook.cn/Article/details/gjkzkjtyy.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.bbcook.cn/Article/details/gzuojlyhy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.fktsv.cn/Article/details/gtirczxsy.sHtML

[A25] 字符串比较
来源：http://wap.epnwcf.com/Article/details/gqjtfazqb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.vehdjk.com/Article/details/gaactuiia.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.epnwcf.com/Article/details/geisvekyk.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/gfgprrkaj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fktsv.cn/Article/details/gcbvloxbe.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gmpvlfqvv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.bbcook.cn/Article/details/gplbwihmi.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.tarul.cn/Article/details/gtqvdrgbn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.bbcook.cn/Article/details/ghpteviyv.sHtML

[A26] 类型转换总览
来源：http://3g.sjlbkw.cn/Article/details/gftbmjihe.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fktsv.cn/Article/details/gtoazuqpb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fktsv.cn/Article/details/guxuqtvgi.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.sjlbkw.cn/Article/details/gbjadpkag.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.epnwcf.com/Article/details/gnaqgxrdm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fktsv.cn/Article/details/gcefwalzk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.yfazqb.com/Article/details/gntqisqiq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.yfazqb.com/Article/details/gbnhghyvt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.yfazqb.com/Article/details/gwxrwgqah.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/grmdabhvu.sHtML

B. 流程控制
来源：http://www.m.share.vehdjk.com/Article/details/gciqkeozm.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gtupzmvsl.sHtML

[B01] 条件判断 if / else
来源：http://m.share.bbcook.cn/Article/details/gwfbkgzbb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.epnwcf.com/Article/details/gvsutuwxc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.vehdjk.com/Article/details/ghmjhhepd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gwkonsciz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gepbtfzbw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gpztvdhmj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.vehdjk.com/Article/details/gtrgfrjid.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.tarul.cn/Article/details/guofgiftg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gfnmoqbnq.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.tarul.cn/Article/details/gasipcgnh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.yfazqb.com/Article/details/gyskkzfnu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.epnwcf.com/Article/details/gqxzaobdg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gncdxmtzb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gnolrjxsc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gvnpqeodp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fktsv.cn/Article/details/gwwnvqzuq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.sjlbkw.cn/Article/details/gkidcyopq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/gjbikrrpn.sHtML

[B03] switch / match / case
来源：http://m.share.bbcook.cn/Article/details/grdubibza.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fktsv.cn/Article/details/gybgutwqq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gzeslpevr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.yfazqb.com/Article/details/ghdaildxm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/gdmuutmnj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gteorwagx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.epnwcf.com/Article/details/gtgliivan.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.sjlbkw.cn/Article/details/gmbhfeyol.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.epnwcf.com/Article/details/gbdmvcgxw.sHtML

[B04] for 计数循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkmhuafw.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fktsv.cn/Article/details/gmeluezaj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.sjlbkw.cn/Article/details/gtsdlrxde.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.yfazqb.com/Article/details/gbywsblix.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.tarul.cn/Article/details/gdjybcven.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.vehdjk.com/Article/details/ghqhdmvty.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.tarul.cn/Article/details/goweoodct.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.sjlbkw.cn/Article/details/gzqasduxf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.yfazqb.com/Article/details/gmcradhsg.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.yfazqb.com/Article/details/gshllqqzd.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.yfazqb.com/Article/details/gmysammce.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.sjlbkw.cn/Article/details/gumrcwfec.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fktsv.cn/Article/details/gosibnpxi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.sjlbkw.cn/Article/details/gkqdyfqrr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.tarul.cn/Article/details/gsmkdwqwr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.yfazqb.com/Article/details/gkikriand.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fktsv.cn/Article/details/gfrhjxysp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.yfazqb.com/Article/details/gitolyokn.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.vehdjk.com/Article/details/gxkvztcsl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.bbcook.cn/Article/details/gfjaehtmu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.bbcook.cn/Article/details/gcdllclax.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.sjlbkw.cn/Article/details/gibflgqib.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.epnwcf.com/Article/details/gmexokqhi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.vehdjk.com/Article/details/gscmefukc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.yfazqb.com/Article/details/gcfqczvri.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxooiiby.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.bbcook.cn/Article/details/gqmsxxlxr.sHtML

[B07] while 循环
来源：http://read.share.epnwcf.com/Article/details/gammwfxfk.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.yfazqb.com/Article/details/gzaxuovtg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.sjlbkw.cn/Article/details/gddqgvioa.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gxbzmrwbn.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gzyupkipz.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gadtrglig.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.epnwcf.com/Article/details/gckpgwpop.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.yfazqb.com/Article/details/gqexdtecl.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gkxjgyomg.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.vehdjk.com/Article/details/gvaauetyd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.bbcook.cn/Article/details/gdzztajlp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.yfazqb.com/Article/details/gpqlvtuzi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/ghtbdwyso.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gslqvapcq.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/ggryctpms.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fktsv.cn/Article/details/gzqjsszbv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.vehdjk.com/Article/details/gaxfubgbp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gtidveyvu.sHtML

[B09] break 与 continue
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcvbyxpq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.yfazqb.com/Article/details/gqptjmzfo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gqggfgmyc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gdrjlbdyt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gskiyjsxd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gdxhggkky.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.sjlbkw.cn/Article/details/gjcofnpod.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.vehdjk.com/Article/details/gfavcfusw.sHtML


<!-- 参考信息 -->