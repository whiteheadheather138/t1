代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.epnwcf.com/Article/details/gzuhtvmeg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fktsv.cn/Article/details/gzzlatlwg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/ggjfxcejk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.yfazqb.com/Article/details/gpsrbnuiu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.tarul.cn/Article/details/gmsnlpnmx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fktsv.cn/Article/details/gkvejspmz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/gysoqaugk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.epnwcf.com/Article/details/gvjoczyvn.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gnpwblzea.sHtML

A. 基础语法与类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgwxhlow.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gyvzmfrbk.sHtML

[A01] Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gouwochqi.sHtML

Py:   print("Hello, World!")
来源：http://www.share.yfazqb.com/Article/details/gexixcqqu.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fktsv.cn/Article/details/godlqoaml.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.sjlbkw.cn/Article/details/gdawutxrk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.epnwcf.com/Article/details/geotvdbkn.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.vehdjk.com/Article/details/gjtbmalis.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fktsv.cn/Article/details/ggjjcpyyh.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.vehdjk.com/Article/details/gzncfmybt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fktsv.cn/Article/details/gqjnrpntq.sHtML

[A02] 变量声明与赋值
来源：http://www.share.yfazqb.com/Article/details/grlgknjvs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.sjlbkw.cn/Article/details/gqrgcuwlv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.tarul.cn/Article/details/gjqwaamzu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.bbcook.cn/Article/details/gvtxbepkl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/gkvvzfjam.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.vehdjk.com/Article/details/gmfmbgzkz.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.epnwcf.com/Article/details/gcjqhjozf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.sjlbkw.cn/Article/details/graqgpsuv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gsplwhjmy.sHtML

[A03] 常量定义
来源：http://blog.epnwcf.com/Article/details/gtizmbjys.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.sjlbkw.cn/Article/details/gddkyawqb.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gpmkjknrb.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gzpvmkepr.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gmghbkikg.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gqdaqnszv.sHtML

Go:   const PI = 3.14159
来源：http://wap.fktsv.cn/Article/details/grykgfuzb.sHtML

Ruby: PI = 3.14159
来源：http://wap.sjlbkw.cn/Article/details/grnpdhuow.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gkwuduseh.sHtML

[A04] 判断变量类型
来源：http://wap.fktsv.cn/Article/details/gyvfrxnyh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.vehdjk.com/Article/details/ggcvdrujy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.sjlbkw.cn/Article/details/gkzjfhpej.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.bbcook.cn/Article/details/guarmpwhe.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.epnwcf.com/Article/details/gpngrjjcs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.epnwcf.com/Article/details/gxtmlxiok.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.yfazqb.com/Article/details/ghscekhfc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fktsv.cn/Article/details/gbhrzadlm.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.vehdjk.com/Article/details/guijgvmvw.sHtML

[A05] 整数除法与取模
来源：http://blog.bbcook.cn/Article/details/gtgvqfufb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.yfazqb.com/Article/details/geyvlfazk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.epnwcf.com/Article/details/gpmvbtlio.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.tarul.cn/Article/details/gggrkfwli.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/gveqzgjzo.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.epnwcf.com/Article/details/grbctxaeg.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gjkahkyzi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gecinqtdy.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gcgfxovaa.sHtML

[A06] 字符串转数字
来源：http://m.share.bbcook.cn/Article/details/gnhiysgey.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.bbcook.cn/Article/details/gqpgelsmt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.epnwcf.com/Article/details/gddxnfcve.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.bbcook.cn/Article/details/gzhakblwy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fktsv.cn/Article/details/ggerjoqxw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.sjlbkw.cn/Article/details/gwwcfmkpe.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.tarul.cn/Article/details/gdlvayqbn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.epnwcf.com/Article/details/gegenladq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.yfazqb.com/Article/details/ghihvshko.sHtML

[A07] 数字转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gpvesybyv.sHtML

Py:   str(42)
来源：http://read.share.vehdjk.com/Article/details/gtouksali.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fktsv.cn/Article/details/geusmtoum.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.epnwcf.com/Article/details/gppbadwzn.sHtML

TS:   String(42)
来源：http://3g.epnwcf.com/Article/details/gkiwbaeoa.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.vehdjk.com/Article/details/gcwrnlbql.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.tarul.cn/Article/details/gnnmqiqlm.sHtML

Ruby: 42.to_s
来源：http://3g.fktsv.cn/Article/details/ghqmfdvcq.sHtML

C#:   42.ToString()
来源：http://3g.vehdjk.com/Article/details/gxztfpjmc.sHtML

[A08] 取整与四舍五入
来源：http://3g.bbcook.cn/Article/details/gnuvtbcwc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gpanbzxou.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.vehdjk.com/Article/details/gxpgnxnqy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.vehdjk.com/Article/details/gkatdnaxk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.yfazqb.com/Article/details/gemaaxyca.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/ggbqubmxv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.tarul.cn/Article/details/gtipjqfun.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fktsv.cn/Article/details/gigvlsghg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/gcljdxrjh.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.tarul.cn/Article/details/gsfjtingo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gpkhfahqg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gfrokxboq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gucqfoybl.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.tarul.cn/Article/details/gqycgicwo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gixvzwefi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.tarul.cn/Article/details/gihvaaazs.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.sjlbkw.cn/Article/details/guowolyky.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.tarul.cn/Article/details/guxjhvwzw.sHtML

[A10] 生成随机数
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdbsvhfq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.vehdjk.com/Article/details/gtmkalxwr.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.yfazqb.com/Article/details/gllnchyzx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fktsv.cn/Article/details/gttfoalbc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.tarul.cn/Article/details/gktecyopq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.sjlbkw.cn/Article/details/grvuhctry.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.vehdjk.com/Article/details/gukqckbzm.sHtML

Ruby: rand(1..100)
来源：http://3g.fktsv.cn/Article/details/gxmcdtnpj.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.sjlbkw.cn/Article/details/gughhxneq.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.yfazqb.com/Article/details/gymjyrmkm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.vehdjk.com/Article/details/gfksyrldr.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/ghyiliwco.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.bbcook.cn/Article/details/gyupjyjri.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.bbcook.cn/Article/details/gepakjenk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.tarul.cn/Article/details/gsauuacrz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.sjlbkw.cn/Article/details/grdhtpckq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/glogmopnm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gptoloiws.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.vehdjk.com/Article/details/gylngbxnn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.epnwcf.com/Article/details/gibukrwlf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.tarul.cn/Article/details/gelcgkbon.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.sjlbkw.cn/Article/details/gbiohoukb.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.yfazqb.com/Article/details/glkrzgvmo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.yfazqb.com/Article/details/gtifbnmuy.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.tarul.cn/Article/details/gojiejgbi.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.tarul.cn/Article/details/grlokjtjl.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.vehdjk.com/Article/details/glxxovpwt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.sjlbkw.cn/Article/details/gmqwlatay.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gtrkodalb.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.bbcook.cn/Article/details/ghfljpyua.sHtML

JS:   "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gqkyopfqp.sHtML

TS:   "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gusmrgvau.sHtML

Java: "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gcpkteltv.sHtML

Go:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gtzrcvjwn.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjpbdaxl.sHtML

C#:   "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gvjvpimbb.sHtML

[A14] 注释写法
来源：http://www.blog.sjlbkw.cn/Article/details/gfargbvmk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.epnwcf.com/Article/details/glsfycfbz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.tarul.cn/Article/details/gklfpauzv.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwgtegdr.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.bbcook.cn/Article/details/gprenhoxo.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.epnwcf.com/Article/details/gjrypffaa.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.bbcook.cn/Article/details/glzwnyafw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.epnwcf.com/Article/details/gwtdpudxr.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/ggtunvvpa.sHtML

[A15] 空值判断与默认值
来源：http://www.share.vehdjk.com/Article/details/gzcakuihz.sHtML

Py:   value = data or "默认值"
来源：http://read.share.bbcook.cn/Article/details/gjojqdzpm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fktsv.cn/Article/details/gjxqirxuf.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.epnwcf.com/Article/details/gwkgiihru.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/gigkisgkt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.fktsv.cn/Article/details/gvgonbcmb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.bbcook.cn/Article/details/ggvouxewl.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.yfazqb.com/Article/details/gmbdxcfxn.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.bbcook.cn/Article/details/gyvxuwlql.sHtML

[A16] 真假值判断规则
来源：http://read.share.fktsv.cn/Article/details/gvizbpnzd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.bbcook.cn/Article/details/glbsxwldx.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.yfazqb.com/Article/details/glhbfpvvg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.yfazqb.com/Article/details/gaoqijgsk.sHtML

TS:   if (!x) {}
来源：http://3g.bbcook.cn/Article/details/ghsbannnn.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.tarul.cn/Article/details/ggayqxyla.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fktsv.cn/Article/details/gzcxplimq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.fktsv.cn/Article/details/gyxdfzhvh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gyxmhktmq.sHtML

[A17] 位运算
来源：http://wap.vehdjk.com/Article/details/gkrguvbbz.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/glkredgaw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.epnwcf.com/Article/details/gzvhfcrfy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/gyzsurrhz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gyrmawoxo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gisqpjtyw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/gzsrvlgtq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/ggudqzcqj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gmrbfrdwx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.yfazqb.com/Article/details/gusnrtezs.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fktsv.cn/Article/details/gkodcqiqg.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.fktsv.cn/Article/details/gyjtxxklu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fktsv.cn/Article/details/ghrdidboz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.vehdjk.com/Article/details/ghegoednl.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.bbcook.cn/Article/details/gzkyupjus.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.tarul.cn/Article/details/gdpprrxxo.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.bbcook.cn/Article/details/gglchkhmd.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.sjlbkw.cn/Article/details/gmupuprtq.sHtML

[A19] 交换两个变量
来源：http://www.blog.yfazqb.com/Article/details/gaidihnbk.sHtML

Py:   a, b = b, a
来源：http://www.blog.fktsv.cn/Article/details/gnuniltoo.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.tarul.cn/Article/details/gwgdohmxx.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbivptat.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.bbcook.cn/Article/details/gbjlmtfah.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fktsv.cn/Article/details/gdvfrmobf.sHtML

Go:   a, b = b, a
来源：http://m.share.tarul.cn/Article/details/gljqvzwib.sHtML

Ruby: a, b = b, a
来源：http://baike.vehdjk.com/Article/details/gzwykplop.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fktsv.cn/Article/details/gzbhjfcyy.sHtML

[A20] 读取标准输入
来源：http://www.m.share.tarul.cn/Article/details/gojdrovpv.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fktsv.cn/Article/details/gbfmlgtqr.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.bbcook.cn/Article/details/gpupqrjti.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.fktsv.cn/Article/details/ggcmtrjun.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.bbcook.cn/Article/details/gnskujwri.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.sjlbkw.cn/Article/details/gyikekjdu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.yfazqb.com/Article/details/gjjgavaae.sHtML

Ruby: gets.chomp
来源：http://3g.vehdjk.com/Article/details/goqgojgsd.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.bbcook.cn/Article/details/gykkqxmtt.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.tarul.cn/Article/details/ghvotqhan.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.epnwcf.com/Article/details/grlisovts.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gbhgivkik.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.yfazqb.com/Article/details/glksgfgan.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/geqxcnrkw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.yfazqb.com/Article/details/gjqwcncmp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/gilzruekq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gdfpkekak.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.vehdjk.com/Article/details/gtmdifrdh.sHtML

[A22] 获取字符串长度
来源：http://read.share.tarul.cn/Article/details/gwojhcbnu.sHtML

Py:   len(s)
来源：http://www.blog.yfazqb.com/Article/details/gvrszavar.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhfewlbl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.epnwcf.com/Article/details/gcesqwliz.sHtML

TS:   s.length
来源：http://m.share.vehdjk.com/Article/details/gpqohtynj.sHtML

Java: s.length()
来源：http://www.blog.bbcook.cn/Article/details/goqsejhky.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fktsv.cn/Article/details/gkzcckgzf.sHtML

Ruby: s.length
来源：http://mobile.tarul.cn/Article/details/gyaoxdxms.sHtML

C#:   s.Length
来源：http://www.blog.fktsv.cn/Article/details/gdblyykcp.sHtML

[A23] 大小写转换
来源：http://3g.fktsv.cn/Article/details/ghlgyjxei.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.epnwcf.com/Article/details/ghbzizail.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fktsv.cn/Article/details/gdflhtqdn.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/gtnukwjho.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.vehdjk.com/Article/details/gdspxlsdq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gceoqkhak.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.epnwcf.com/Article/details/gnagemepo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.tarul.cn/Article/details/giurldgmy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.vehdjk.com/Article/details/gjgoljsyb.sHtML

[A24] 去除首尾空白
来源：http://www.blog.bbcook.cn/Article/details/gwomofevh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.yfazqb.com/Article/details/gpqnkvvas.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.bbcook.cn/Article/details/goiawofxn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.bbcook.cn/Article/details/gxgvvrjio.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.sjlbkw.cn/Article/details/gxuzmssjy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.vehdjk.com/Article/details/gzrccgifu.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.epnwcf.com/Article/details/gmwheabyc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.vehdjk.com/Article/details/gayseawrx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/gfhtedfuq.sHtML

[A25] 字符串比较
来源：http://www.m.share.tarul.cn/Article/details/gupjgworg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.yfazqb.com/Article/details/gymymwfoc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.vehdjk.com/Article/details/gmyjxjcdq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.epnwcf.com/Article/details/gicxvnijc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.yfazqb.com/Article/details/gehhucazh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.epnwcf.com/Article/details/gaxlxpxwu.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.sjlbkw.cn/Article/details/gpnxtpsyz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fktsv.cn/Article/details/gzhnpubjw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.bbcook.cn/Article/details/gzpdczwsy.sHtML

[A26] 类型转换总览
来源：http://wap.sjlbkw.cn/Article/details/gfypizfrz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.vehdjk.com/Article/details/gxcsaesgm.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.sjlbkw.cn/Article/details/gdfdbhlqy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.bbcook.cn/Article/details/gaxnmiyxk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.bbcook.cn/Article/details/gmfbxffro.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.tarul.cn/Article/details/ggmiosxwa.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.epnwcf.com/Article/details/geerfkdwe.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.sjlbkw.cn/Article/details/gosjsucsx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.bbcook.cn/Article/details/ghcxkfokx.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gnwwxrwkt.sHtML

B. 流程控制
来源：http://www.m.share.bbcook.cn/Article/details/gumhutpvi.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gunrjxnnw.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fktsv.cn/Article/details/gotdumaqk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.epnwcf.com/Article/details/gfrcmitux.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.epnwcf.com/Article/details/gerxvfhki.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gxcinweep.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gsbgmshph.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gaowsngas.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.epnwcf.com/Article/details/gybsgiuyd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.vehdjk.com/Article/details/gtqltkesw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/giyrwslzz.sHtML

[B02] 多分支 else if / elif
来源：http://blog.sjlbkw.cn/Article/details/gmjkwwmnj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.sjlbkw.cn/Article/details/gidygmywm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.epnwcf.com/Article/details/gatpeascr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gaascjgri.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gycdvuxtn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gjoyjhhpv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fktsv.cn/Article/details/ghpotoahv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.tarul.cn/Article/details/gstwhbnxr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gyodcdcbc.sHtML

[B03] switch / match / case
来源：http://m.share.tarul.cn/Article/details/gxlmfqrkj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fktsv.cn/Article/details/gqsviwjbe.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.yfazqb.com/Article/details/gylfgjpht.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gztflkymb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gtfsmzrgv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gxqgroacw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.tarul.cn/Article/details/glbfcshrh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.yfazqb.com/Article/details/gkuttlqfe.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.yfazqb.com/Article/details/gmickspek.sHtML

[B04] for 计数循环
来源：http://wap.yfazqb.com/Article/details/gmbvtbmlk.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.sjlbkw.cn/Article/details/gbdoyripa.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.sjlbkw.cn/Article/details/gmgoozdey.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.tarul.cn/Article/details/ghljltadn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.epnwcf.com/Article/details/gteyipvan.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.yfazqb.com/Article/details/gimeokccf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.bbcook.cn/Article/details/gbekwfwwf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.sjlbkw.cn/Article/details/goqtziosg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gpnlqzyrv.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fktsv.cn/Article/details/gbkxhmjko.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.bbcook.cn/Article/details/gipluxygy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.epnwcf.com/Article/details/gymjzqchw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.tarul.cn/Article/details/gkjccngvi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.sjlbkw.cn/Article/details/gtcapozfx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.yfazqb.com/Article/details/gjrmzbepr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.yfazqb.com/Article/details/gcgswrvwg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.epnwcf.com/Article/details/ggverpdlr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gtdonofvi.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.epnwcf.com/Article/details/gubjmjnnb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.sjlbkw.cn/Article/details/gsmyolrzh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fktsv.cn/Article/details/gqsvjrvjo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.tarul.cn/Article/details/gwhyqwwzn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/gxlglqkzf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.epnwcf.com/Article/details/gpcrtmnws.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.yfazqb.com/Article/details/gejlwtmiu.sHtML


<!-- 参考信息 -->