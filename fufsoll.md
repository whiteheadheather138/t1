代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.yfazqb.com/Article/details/gjufdkczh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.yfazqb.com/Article/details/gledqgljd.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.tarul.cn/Article/details/gjpwseftj.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.tarul.cn/Article/details/ggpvowvjc.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.sjlbkw.cn/Article/details/gvavctdrc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.tarul.cn/Article/details/gpndhnsvj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.bbcook.cn/Article/details/gzdzrtbri.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.tarul.cn/Article/details/gkrgijeep.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fktsv.cn/Article/details/gwnjxkmwr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.tarul.cn/Article/details/gwynihfqj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.epnwcf.com/Article/details/guzuarjjt.sHtML

[B12] 跳出多层循环
来源：http://wap.bbcook.cn/Article/details/gldylvunu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.bbcook.cn/Article/details/gewosxhjz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.tarul.cn/Article/details/gmnogpzrj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gtnwgmomn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/grlencrmh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/gbmrnibfp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.epnwcf.com/Article/details/gjwydyreq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.vehdjk.com/Article/details/gqxntjfcb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.sjlbkw.cn/Article/details/gyuyahuot.sHtML

[B13] 判断是否为数字
来源：http://3g.epnwcf.com/Article/details/grrkocksz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.yfazqb.com/Article/details/guokpqdmh.sHtML

PHP:  is_numeric($x)
来源：http://wap.fktsv.cn/Article/details/gsxpusask.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/ggrqqwduq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.yfazqb.com/Article/details/gdjwngyrv.sHtML

Java: x instanceof Number
来源：http://baike.yfazqb.com/Article/details/gsrilajnw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.yfazqb.com/Article/details/gpugnazwx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.yfazqb.com/Article/details/gpdustsxk.sHtML

C#:   x is int or double or decimal
来源：http://3g.epnwcf.com/Article/details/grhtuhejn.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fktsv.cn/Article/details/gaddqkgvi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.tarul.cn/Article/details/gnciremre.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.sjlbkw.cn/Article/details/ggfwaacve.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gkbymcxtq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fktsv.cn/Article/details/gqlpuwtek.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.yfazqb.com/Article/details/gqfbfueve.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.tarul.cn/Article/details/gmqzjvlml.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.vehdjk.com/Article/details/grksgugog.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fktsv.cn/Article/details/gxvglucgi.sHtML

[B15] 布尔运算与取反
来源：http://read.share.yfazqb.com/Article/details/gdryshcgp.sHtML

Py:   a and b or not c
来源：http://www.blog.tarul.cn/Article/details/ggulgoegq.sHtML

PHP:  $a && $b || !$c
来源：http://wap.tarul.cn/Article/details/gofoufjnh.sHtML

JS:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gbkzzqfwq.sHtML

TS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gaxhgmsbz.sHtML

Java: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gxlrtuyht.sHtML

Go:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gbdbxgazd.sHtML

Ruby: a && b || !c
来源：http://3g.tarul.cn/Article/details/gliqqpzuj.sHtML

C#:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gbrrygyal.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.epnwcf.com/Article/details/gxumtmaof.sHtML

Py:   if not data: return
来源：http://blog.yfazqb.com/Article/details/gzufrpxys.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.bbcook.cn/Article/details/gcllipkcw.sHtML

JS:   if (!data) return;
来源：http://www.blog.epnwcf.com/Article/details/gvmdebkqr.sHtML

TS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gfmaknect.sHtML

Java: if (data == null) return;
来源：http://www.share.vehdjk.com/Article/details/gtzxkjrar.sHtML

Go:   if data == nil { return }
来源：http://m.share.epnwcf.com/Article/details/gjwhcnaux.sHtML

Ruby: return if data.nil?
来源：http://mobile.fktsv.cn/Article/details/gdljveair.sHtML

C#:   if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/gboarctto.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gzwrshwrr.sHtML

C. 函数与作用域
来源：http://baike.epnwcf.com/Article/details/gunbbzmda.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmvcqktgr.sHtML

[C01] 定义函数
来源：http://blog.tarul.cn/Article/details/gfpwoqdmp.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.epnwcf.com/Article/details/gqbhrhoxl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/ggzcixsxp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gxthaxiqt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/grcerperz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gcxeawmls.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.tarul.cn/Article/details/gxvobjgua.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.tarul.cn/Article/details/gnfjysyjo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gijbptqkn.sHtML

[C02] 默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gygitbafr.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.sjlbkw.cn/Article/details/gdhmdhual.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fktsv.cn/Article/details/gazlvtxxg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fktsv.cn/Article/details/gitpbpgnn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gcbtxxdky.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.vehdjk.com/Article/details/gywsfdqrp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.tarul.cn/Article/details/gysvuwjuz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.bbcook.cn/Article/details/gqseovnqq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.tarul.cn/Article/details/gaendromw.sHtML

[C03] 可变参数
来源：http://www.blog.vehdjk.com/Article/details/gyqyzxkwg.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fktsv.cn/Article/details/gzwnggwlp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fktsv.cn/Article/details/gwshtzdzt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gxetjdert.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/gkkeevhto.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.vehdjk.com/Article/details/gimbqfame.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fktsv.cn/Article/details/gjjhibzcf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.epnwcf.com/Article/details/gbogsmcnf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fktsv.cn/Article/details/gywxfzuok.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fktsv.cn/Article/details/gkbsfblmg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjmubqhn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.yfazqb.com/Article/details/gfkvwahbs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.vehdjk.com/Article/details/gvaedimqp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.bbcook.cn/Article/details/gvkjxxfcm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fktsv.cn/Article/details/gsjpzuzfs.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.bbcook.cn/Article/details/gayuqokdw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/gsheaajaq.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.epnwcf.com/Article/details/gojqftapb.sHtML

[C05] 返回多个值
来源：http://www.m.share.yfazqb.com/Article/details/gyvmaciko.sHtML

Py:   return a, b
来源：http://m.share.tarul.cn/Article/details/gnmtjxkmb.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.tarul.cn/Article/details/gqfcqmqwq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/gcgsawrsa.sHtML

TS:   return { a, b };
来源：http://www.blog.tarul.cn/Article/details/gtdfbcdih.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.vehdjk.com/Article/details/gdkarrikh.sHtML

Go:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gqvdisnqo.sHtML

Ruby: return a, b
来源：http://blog.yfazqb.com/Article/details/grzfieyjx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.epnwcf.com/Article/details/ganoeydni.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.epnwcf.com/Article/details/gdilsfbrb.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.yfazqb.com/Article/details/gyvfdvqka.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.epnwcf.com/Article/details/gzfzdivcp.sHtML

JS:   const square = x => x * x;
来源：http://wap.epnwcf.com/Article/details/gphmulyov.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.tarul.cn/Article/details/gcsrxvkzd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.tarul.cn/Article/details/grzzypdik.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.epnwcf.com/Article/details/gztgaeurl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.yfazqb.com/Article/details/gdxnxpopl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.tarul.cn/Article/details/gdaysbhys.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfjoonyg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fktsv.cn/Article/details/gvfxybtgh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.tarul.cn/Article/details/gphwnzmvq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.sjlbkw.cn/Article/details/gucermuui.sHtML

TS:   arr.map(String)
来源：http://3g.tarul.cn/Article/details/gorwnwdmq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gldtxjomb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.vehdjk.com/Article/details/gyvgbgsyi.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.tarul.cn/Article/details/ghgjihwjx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.vehdjk.com/Article/details/gthdopkrw.sHtML

[C08] 闭包
来源：http://read.share.tarul.cn/Article/details/gwcyetemw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.sjlbkw.cn/Article/details/gfzlwupgj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fktsv.cn/Article/details/gjgtosqzy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.bbcook.cn/Article/details/ghwmthxse.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gxqdjbnam.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fktsv.cn/Article/details/gxegxumag.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.tarul.cn/Article/details/gnebnpjus.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/gvifxbatd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gugjxulrq.sHtML

[C09] 递归
来源：http://3g.sjlbkw.cn/Article/details/gykqrmwom.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.epnwcf.com/Article/details/gflookani.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/gysllghvv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/gcbdngjfs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.bbcook.cn/Article/details/gjncoeiia.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.epnwcf.com/Article/details/gxvyauzcg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.bbcook.cn/Article/details/gtiqkqzzj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/grfrrrdfa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fktsv.cn/Article/details/gknqdwclk.sHtML

[C10] 变量作用域
来源：http://blog.epnwcf.com/Article/details/gzbfmcltf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.epnwcf.com/Article/details/gdvspixri.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fktsv.cn/Article/details/gqsitazcc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fktsv.cn/Article/details/gchhldouj.sHtML

TS:   同 JS
来源：http://www.share.epnwcf.com/Article/details/gqqamplzq.sHtML

Java: 方法内为块级作用域
来源：http://3g.yfazqb.com/Article/details/glqxngqka.sHtML

Go:   花括号块级作用域
来源：http://www.share.epnwcf.com/Article/details/gnzgarpvw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.sjlbkw.cn/Article/details/gplnjakxt.sHtML

C#:   块级作用域
来源：http://read.share.fktsv.cn/Article/details/gbqwfikse.sHtML

[C11] 模块导入与导出
来源：http://mobile.sjlbkw.cn/Article/details/giwtfefhh.sHtML

Py:   from module import func
来源：http://www.blog.sjlbkw.cn/Article/details/gpspgarqv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fktsv.cn/Article/details/ggpvqnznz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fktsv.cn/Article/details/gdscbqoei.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.vehdjk.com/Article/details/gwcoyqggd.sHtML

Java: import java.util.List;
来源：http://m.share.bbcook.cn/Article/details/ggzdbbwnz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.sjlbkw.cn/Article/details/ghmunhhpe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.bbcook.cn/Article/details/gcjrnauhw.sHtML

C#:   using System.Text;
来源：http://3g.sjlbkw.cn/Article/details/gcelgjgwp.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.sjlbkw.cn/Article/details/glheegiqx.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.vehdjk.com/Article/details/gsphwdhgg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.vehdjk.com/Article/details/gwjhmrbdw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/gwxuhgiyd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/ggkwlwfrn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.yfazqb.com/Article/details/gbcdxqbil.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.epnwcf.com/Article/details/gcpveqvpz.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.tarul.cn/Article/details/gmelwcvmr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.yfazqb.com/Article/details/gdgiipkbr.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.epnwcf.com/Article/details/grdmhgzvb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fktsv.cn/Article/details/gbwepaeze.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gqbelosyz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.vehdjk.com/Article/details/gbikanlin.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gyjhrpflz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gvovtpjxt.sHtML

Go:   func add(a, b int) int
来源：http://mobile.tarul.cn/Article/details/gebeltiqh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.sjlbkw.cn/Article/details/guuobsevw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.epnwcf.com/Article/details/gqwzcjrwl.sHtML

[C14] 泛型函数
来源：http://www.blog.yfazqb.com/Article/details/gafaqxxcc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.yfazqb.com/Article/details/gfrdndrtl.sHtML

PHP:  // 无泛型
来源：http://read.share.yfazqb.com/Article/details/guyyxfbqq.sHtML

JS:   // 无泛型
来源：http://blog.bbcook.cn/Article/details/gvqwofezu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.tarul.cn/Article/details/gwirlrucq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.bbcook.cn/Article/details/gajghqnvb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.epnwcf.com/Article/details/gmjtdlgyh.sHtML

Ruby: # 无泛型
来源：http://wap.bbcook.cn/Article/details/gbebjgrcn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.vehdjk.com/Article/details/guznofstg.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gfovdfeiu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.vehdjk.com/Article/details/grbchzmys.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fktsv.cn/Article/details/gwvkkubna.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.yfazqb.com/Article/details/grkqaarvx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fktsv.cn/Article/details/glvthuruz.sHtML

Java: // 无解构
来源：http://mobile.bbcook.cn/Article/details/ggxuthpys.sHtML

Go:   // 无解构
来源：http://3g.vehdjk.com/Article/details/gqqoezalv.sHtML

Ruby: a, b = pair
来源：http://read.share.sjlbkw.cn/Article/details/gzikawfkj.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.epnwcf.com/Article/details/gwagexkem.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.tarul.cn/Article/details/ggosogmff.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.vehdjk.com/Article/details/gmagarxbp.sHtML

PHP:  // 无重载
来源：http://m.share.yfazqb.com/Article/details/gjdlaimgo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.epnwcf.com/Article/details/gynlasmlm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.epnwcf.com/Article/details/glfarpfgp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.bbcook.cn/Article/details/ghwdoioxz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.yfazqb.com/Article/details/gmaojwuhv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.vehdjk.com/Article/details/gdyrkdhem.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.epnwcf.com/Article/details/ggodkwsga.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gskuuxlwg.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fktsv.cn/Article/details/gxihptiwg.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gjrzjxnzk.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/ggaevhqob.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.bbcook.cn/Article/details/gvmviuvnr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gepiuuvxa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.bbcook.cn/Article/details/gaawqkbdq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.yfazqb.com/Article/details/gnueyhwty.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.bbcook.cn/Article/details/gmznprrow.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.epnwcf.com/Article/details/gabjeyeli.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.epnwcf.com/Article/details/gvmbxsrkk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.tarul.cn/Article/details/grsitaeeh.sHtML

[D02] 追加元素到末尾
来源：http://read.share.epnwcf.com/Article/details/ggufejjol.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.tarul.cn/Article/details/gnkxkipmm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.vehdjk.com/Article/details/gsayrqepe.sHtML

JS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/gsgdjxqdl.sHtML

TS:   arr.push(4);
来源：http://blog.sjlbkw.cn/Article/details/ggwcobvwd.sHtML

Java: list.add(4);
来源：http://m.share.tarul.cn/Article/details/gpyqookgz.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gvlomfghm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.sjlbkw.cn/Article/details/gycjtmgox.sHtML

C#:   list.Add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gqfctbhao.sHtML

[D03] 在指定位置插入元素
来源：http://3g.sjlbkw.cn/Article/details/giejwmcsk.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.epnwcf.com/Article/details/godcolvie.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.tarul.cn/Article/details/gslqxdoun.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fktsv.cn/Article/details/gplxoykdl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gonmoblhw.sHtML

Java: list.add(0, 0);
来源：http://3g.epnwcf.com/Article/details/gbkyyrwhu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.bbcook.cn/Article/details/gyujryfft.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.bbcook.cn/Article/details/gtmbcjmwl.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.vehdjk.com/Article/details/goujqgkkr.sHtML

[D04] 删除元素
来源：http://www.blog.vehdjk.com/Article/details/gonaysxqu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.bbcook.cn/Article/details/gcdfvpiqk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.yfazqb.com/Article/details/gqygsturc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.epnwcf.com/Article/details/grvzeuksv.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.yfazqb.com/Article/details/guxdftiww.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.epnwcf.com/Article/details/ggckeyfom.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.sjlbkw.cn/Article/details/gcfnzpzwt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.epnwcf.com/Article/details/gymdnhcxu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.bbcook.cn/Article/details/gezwgmflo.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.epnwcf.com/Article/details/gupeicvdx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/gfubsofrh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gwlmyyutu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gkgpnjwno.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.yfazqb.com/Article/details/gtpxntxbt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.vehdjk.com/Article/details/gvwafcfsu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/ghdvmqznp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/grmvaqigg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gxradmtew.sHtML

[D06] 数组长度
来源：http://blog.vehdjk.com/Article/details/guxzckiha.sHtML

Py:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/gpysmkcoe.sHtML

PHP:  count($arr);
来源：http://wap.epnwcf.com/Article/details/gfxcrorrw.sHtML

JS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/gbnzigmvh.sHtML

TS:   arr.length
来源：http://3g.sjlbkw.cn/Article/details/gsvzwpmtq.sHtML

Java: list.size();
来源：http://mobile.vehdjk.com/Article/details/gjoqqwqhl.sHtML

Go:   len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gshmdasjn.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fktsv.cn/Article/details/ggavxpynn.sHtML

C#:   list.Count;
来源：http://www.m.share.sjlbkw.cn/Article/details/guakwfehk.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.sjlbkw.cn/Article/details/gddulwkan.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.vehdjk.com/Article/details/goptengjz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.bbcook.cn/Article/details/ggexrrwtk.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gksutbheg.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/gjyaegrvw.sHtML

Java: list.subList(1, 4);
来源：http://wap.vehdjk.com/Article/details/genqouwix.sHtML

Go:   arr[1:4]
来源：http://www.share.epnwcf.com/Article/details/gtnkzkphz.sHtML

Ruby: arr[1, 3]
来源：http://wap.tarul.cn/Article/details/gzwmglbzl.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.bbcook.cn/Article/details/gjdfhljgf.sHtML

[D08] 合并两个数组
来源：http://www.blog.sjlbkw.cn/Article/details/gbovgsekl.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.sjlbkw.cn/Article/details/gfvcycnld.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fktsv.cn/Article/details/gznzxnoqc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.bbcook.cn/Article/details/gmsgfuail.sHtML

TS:   [...a, ...b];
来源：http://baike.yfazqb.com/Article/details/ghjkiqtlx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.vehdjk.com/Article/details/gmihozdyb.sHtML

Go:   append(a, b...)
来源：http://mobile.epnwcf.com/Article/details/gcstyybge.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.sjlbkw.cn/Article/details/gubpxmsde.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzugauwuu.sHtML

[D09] 排序（升序）
来源：http://wap.epnwcf.com/Article/details/gwslxcvrv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gradpanfl.sHtML

PHP:  sort($arr);
来源：http://mobile.yfazqb.com/Article/details/gojdvizar.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/gozyqswbe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.sjlbkw.cn/Article/details/gxrgsvrfr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.vehdjk.com/Article/details/grhdtbmjl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.epnwcf.com/Article/details/gbpqxijrp.sHtML

Ruby: arr.sort
来源：http://www.m.share.fktsv.cn/Article/details/gitdyueud.sHtML

C#:   list.Sort();
来源：http://www.m.share.yfazqb.com/Article/details/gnxdakfez.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.tarul.cn/Article/details/gtloknksl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.bbcook.cn/Article/details/gjevxglop.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/gepvqsmdb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/gzcbmvkwa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/gqklhusiy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.yfazqb.com/Article/details/gcxlnxfex.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.tarul.cn/Article/details/gmgjrwuet.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.yfazqb.com/Article/details/gzrzahscu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.epnwcf.com/Article/details/giwttxftf.sHtML

[D11] 反转数组
来源：http://baike.epnwcf.com/Article/details/gkjnqhuqx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.yfazqb.com/Article/details/gyyywijlj.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.yfazqb.com/Article/details/gqtpfzyvo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.epnwcf.com/Article/details/greexjnvw.sHtML


<!-- 参考信息 -->