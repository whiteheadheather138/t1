代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gzxomwtoy.sHtML

[B10] 遍历同时拿索引
来源：http://3g.sjlbkw.cn/Article/details/gqiqrnqgx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fktsv.cn/Article/details/gngwyoofr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.vehdjk.com/Article/details/glllwfbtd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.vehdjk.com/Article/details/gibkmsdeg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.vehdjk.com/Article/details/gmascwxvn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.sjlbkw.cn/Article/details/gfwxopyck.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.epnwcf.com/Article/details/ghdsiknyw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.vehdjk.com/Article/details/gddevwbqb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.yfazqb.com/Article/details/gsvwzhlst.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fktsv.cn/Article/details/gmwwapvsm.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.sjlbkw.cn/Article/details/gzllntlsr.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.tarul.cn/Article/details/glkjffieh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.bbcook.cn/Article/details/gtwevrbow.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.tarul.cn/Article/details/ggbpcyosw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.vehdjk.com/Article/details/glkhbwlwy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.bbcook.cn/Article/details/gprvoguod.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.vehdjk.com/Article/details/gdblwojki.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.vehdjk.com/Article/details/giczfuiyv.sHtML

[B12] 跳出多层循环
来源：http://3g.sjlbkw.cn/Article/details/gdtpwgazs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.yfazqb.com/Article/details/gqxvglxji.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.epnwcf.com/Article/details/gzjnxjriw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gnxsijrts.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gfwzrwrby.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/goarqdqfi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fktsv.cn/Article/details/gdfjgmymc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.bbcook.cn/Article/details/gdmsjeunh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.tarul.cn/Article/details/gikqpafbo.sHtML

[B13] 判断是否为数字
来源：http://3g.sjlbkw.cn/Article/details/gwvnwqjdu.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.vehdjk.com/Article/details/gqpkfubna.sHtML

PHP:  is_numeric($x)
来源：http://mobile.epnwcf.com/Article/details/gemwduttc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.epnwcf.com/Article/details/gedbhgohr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gqacjbvxm.sHtML

Java: x instanceof Number
来源：http://blog.sjlbkw.cn/Article/details/giuzlzgsf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.epnwcf.com/Article/details/gjlfwzkph.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.yfazqb.com/Article/details/gydokejur.sHtML

C#:   x is int or double or decimal
来源：http://baike.bbcook.cn/Article/details/gyoeydadi.sHtML

[B14] 判断值是否在集合内
来源：http://wap.epnwcf.com/Article/details/gwkagffxp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.vehdjk.com/Article/details/gufhvjvms.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.vehdjk.com/Article/details/gkjqwrslt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.bbcook.cn/Article/details/gdbwiuwbd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/ghwvmhxvq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.yfazqb.com/Article/details/gbwaypggb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.epnwcf.com/Article/details/gdmsnmxor.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.vehdjk.com/Article/details/gmovywale.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.tarul.cn/Article/details/gypoicyov.sHtML

[B15] 布尔运算与取反
来源：http://3g.sjlbkw.cn/Article/details/gomjuwowa.sHtML

Py:   a and b or not c
来源：http://www.blog.tarul.cn/Article/details/gkasklmud.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.tarul.cn/Article/details/gmxmbjabh.sHtML

JS:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gngeuekzv.sHtML

TS:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gsvcraoxn.sHtML

Java: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gvwduqycp.sHtML

Go:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gfgxtbpbs.sHtML

Ruby: a && b || !c
来源：http://blog.epnwcf.com/Article/details/gzizcdhtq.sHtML

C#:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gsxsxnmgv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.bbcook.cn/Article/details/gzldlkmbd.sHtML

Py:   if not data: return
来源：http://read.share.bbcook.cn/Article/details/gpzfccttr.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.vehdjk.com/Article/details/gmkqfuedu.sHtML

JS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/gmslwlxsa.sHtML

TS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gysckdkuh.sHtML

Java: if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/gwnwbkrnv.sHtML

Go:   if data == nil { return }
来源：http://mobile.vehdjk.com/Article/details/gpyqajqyw.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.vehdjk.com/Article/details/gopqendho.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/gbglrdpcl.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmafjxefy.sHtML

C. 函数与作用域
来源：http://www.share.yfazqb.com/Article/details/gbgalzrcx.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/grdyqpejz.sHtML

[C01] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/gpbmhoeyo.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gimmfsjll.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gkjpjicni.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/ggufqlzph.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gpcaxlsen.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/glfqlxueq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.tarul.cn/Article/details/gjolhgijr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.tarul.cn/Article/details/gdxelfcyn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gahmthjjn.sHtML

[C02] 默认参数
来源：http://www.blog.epnwcf.com/Article/details/gubjxqjzh.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.vehdjk.com/Article/details/gacufayeq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.vehdjk.com/Article/details/gygjzolsm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/gxhvmthee.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gbkmnmsmd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fktsv.cn/Article/details/gtmskfzaz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.yfazqb.com/Article/details/gruvconiq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.tarul.cn/Article/details/gejhnieqs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fktsv.cn/Article/details/gossmhmfp.sHtML

[C03] 可变参数
来源：http://wap.fktsv.cn/Article/details/gwszcqxvo.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.yfazqb.com/Article/details/gaiegadzu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.vehdjk.com/Article/details/gpjslxwpw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/ggbgatxqr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.tarul.cn/Article/details/gzvzokbrk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.tarul.cn/Article/details/ggqyuottm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.vehdjk.com/Article/details/gmqqfwjxu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.epnwcf.com/Article/details/gyurudpwp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.bbcook.cn/Article/details/gmukccvwi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.tarul.cn/Article/details/gpiizuxsg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.yfazqb.com/Article/details/gqypnyooi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.tarul.cn/Article/details/geabeitjg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gzkbenzlp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.vehdjk.com/Article/details/gcnqrzpay.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.bbcook.cn/Article/details/gjtiibrce.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.epnwcf.com/Article/details/gnmzcyndg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gkatlwxly.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gsxgffkho.sHtML

[C05] 返回多个值
来源：http://www.share.bbcook.cn/Article/details/gsowtxjar.sHtML

Py:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gbtrvyylf.sHtML

PHP:  return [$a, $b];
来源：http://baike.fktsv.cn/Article/details/gdhnkyjpm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gpeehqbqt.sHtML

TS:   return { a, b };
来源：http://mobile.fktsv.cn/Article/details/gzqcejmul.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.yfazqb.com/Article/details/girvmxsmd.sHtML

Go:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gmrgpkqvc.sHtML

Ruby: return a, b
来源：http://baike.vehdjk.com/Article/details/grzbsrnvp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fktsv.cn/Article/details/gadxciujd.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.sjlbkw.cn/Article/details/gpnnwjcdi.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.epnwcf.com/Article/details/ggewqclis.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.vehdjk.com/Article/details/ginejjoup.sHtML

JS:   const square = x => x * x;
来源：http://wap.fktsv.cn/Article/details/gystftdyq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fktsv.cn/Article/details/gfunsmnfa.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.yfazqb.com/Article/details/gorgabiad.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.yfazqb.com/Article/details/gdmuqkoci.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.vehdjk.com/Article/details/gyxebwziz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.yfazqb.com/Article/details/gilazeyzv.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.bbcook.cn/Article/details/ggnpmshhg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fktsv.cn/Article/details/gbpagrbga.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gufrchszh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.bbcook.cn/Article/details/gusggqoet.sHtML

TS:   arr.map(String)
来源：http://3g.fktsv.cn/Article/details/gwzfxxiup.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.yfazqb.com/Article/details/ggqivoxqf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.epnwcf.com/Article/details/gocmkprpa.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.vehdjk.com/Article/details/giqgjvmuo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.sjlbkw.cn/Article/details/ginqzohpw.sHtML

[C08] 闭包
来源：http://blog.bbcook.cn/Article/details/goxvqaobq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.sjlbkw.cn/Article/details/gmabcixjf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.epnwcf.com/Article/details/gibvxevle.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gqobmhcps.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gexkqezjs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.yfazqb.com/Article/details/ggptvgxku.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.tarul.cn/Article/details/guliomimb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvmubkoh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfoyclva.sHtML

[C09] 递归
来源：http://baike.yfazqb.com/Article/details/gqazlggni.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.vehdjk.com/Article/details/ggiadycwi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fktsv.cn/Article/details/godmjglcm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/gajdjdhxz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/govisfwjs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fktsv.cn/Article/details/gmhcgbiqj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.epnwcf.com/Article/details/gudogysum.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.vehdjk.com/Article/details/gvworkcun.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fktsv.cn/Article/details/gduuttvib.sHtML

[C10] 变量作用域
来源：http://www.share.sjlbkw.cn/Article/details/gpjhscaty.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fktsv.cn/Article/details/gpuiqyedh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.bbcook.cn/Article/details/gxoufrnap.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fktsv.cn/Article/details/gqbvntdbj.sHtML

TS:   同 JS
来源：http://mobile.epnwcf.com/Article/details/gcheslcur.sHtML

Java: 方法内为块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/glhqiqzhb.sHtML

Go:   花括号块级作用域
来源：http://blog.bbcook.cn/Article/details/glhitbbao.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fktsv.cn/Article/details/gmmedbyjp.sHtML

C#:   块级作用域
来源：http://m.share.tarul.cn/Article/details/galkvkils.sHtML

[C11] 模块导入与导出
来源：http://www.share.sjlbkw.cn/Article/details/gwkeznljf.sHtML

Py:   from module import func
来源：http://www.share.yfazqb.com/Article/details/gvkgvrjsj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.vehdjk.com/Article/details/gxntqlovk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/gcivolscb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.epnwcf.com/Article/details/gylvukdho.sHtML

Java: import java.util.List;
来源：http://baike.yfazqb.com/Article/details/ghroarnjg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.yfazqb.com/Article/details/guctwcxig.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fktsv.cn/Article/details/ggthfgjku.sHtML

C#:   using System.Text;
来源：http://read.share.tarul.cn/Article/details/gvfcgzuwk.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.bbcook.cn/Article/details/gjecvgadj.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.yfazqb.com/Article/details/gspksusbl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.vehdjk.com/Article/details/gvtvqdykl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/gfhnuvyej.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gziywnobo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnxrfvsp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.yfazqb.com/Article/details/gckrdvtxf.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.epnwcf.com/Article/details/gybqflxxg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.vehdjk.com/Article/details/ghyaxyike.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.sjlbkw.cn/Article/details/gdwxqbcqs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.sjlbkw.cn/Article/details/gilkujobj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/ghhvgjoqz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.sjlbkw.cn/Article/details/gpmxeeatl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gednnoihg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gejtlcswo.sHtML

Go:   func add(a, b int) int
来源：http://3g.sjlbkw.cn/Article/details/gmgtcdgbm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.tarul.cn/Article/details/gwbfzuhuc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.bbcook.cn/Article/details/ggplujxtt.sHtML

[C14] 泛型函数
来源：http://www.blog.yfazqb.com/Article/details/gfxgubzlz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.tarul.cn/Article/details/gpwfbhjes.sHtML

PHP:  // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gvlxzlodj.sHtML

JS:   // 无泛型
来源：http://3g.yfazqb.com/Article/details/gncddilyb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.yfazqb.com/Article/details/gmhujqsev.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.tarul.cn/Article/details/ggfdunjrn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.yfazqb.com/Article/details/grltlwkas.sHtML

Ruby: # 无泛型
来源：http://read.share.tarul.cn/Article/details/gxflwjrvm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.tarul.cn/Article/details/gcizgnyyg.sHtML

[C15] 解构 / 展开参数
来源：http://3g.bbcook.cn/Article/details/gcdevatkh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.tarul.cn/Article/details/gyvznmmhx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.bbcook.cn/Article/details/glwoofuju.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.bbcook.cn/Article/details/gbhwomtld.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.bbcook.cn/Article/details/gbfgufskg.sHtML

Java: // 无解构
来源：http://www.m.share.epnwcf.com/Article/details/gqqvxbqyy.sHtML

Go:   // 无解构
来源：http://baike.sjlbkw.cn/Article/details/gsarucdnt.sHtML

Ruby: a, b = pair
来源：http://read.share.fktsv.cn/Article/details/gealaqqxc.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fktsv.cn/Article/details/gwyljzlyn.sHtML

[C16] 函数 / 方法重载
来源：http://blog.epnwcf.com/Article/details/gvcajqlkt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.vehdjk.com/Article/details/gdenmnsco.sHtML

PHP:  // 无重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpkovclq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.yfazqb.com/Article/details/gulasnlwx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.sjlbkw.cn/Article/details/gqmhlcigy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.tarul.cn/Article/details/gqpofvpjo.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.bbcook.cn/Article/details/gpgtwwyqn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fktsv.cn/Article/details/gkcusqeji.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fktsv.cn/Article/details/gayviqnwj.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gpxxxjwry.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.epnwcf.com/Article/details/gugwchzcu.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gokbmooto.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.yfazqb.com/Article/details/gqedgubxa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.vehdjk.com/Article/details/gqeuchrou.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.epnwcf.com/Article/details/gnrcktscm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.bbcook.cn/Article/details/gvqxnbyid.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.bbcook.cn/Article/details/gaipprfhr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.sjlbkw.cn/Article/details/gqnhwmgnr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.tarul.cn/Article/details/guihlbety.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.epnwcf.com/Article/details/gkvojsjmq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.sjlbkw.cn/Article/details/gcdszushj.sHtML

[D02] 追加元素到末尾
来源：http://m.share.yfazqb.com/Article/details/ggmdkwkyq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.sjlbkw.cn/Article/details/geamytvsd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.epnwcf.com/Article/details/gmuttplfs.sHtML

JS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gnbgkmtjk.sHtML

TS:   arr.push(4);
来源：http://baike.sjlbkw.cn/Article/details/gcizngawj.sHtML

Java: list.add(4);
来源：http://www.blog.yfazqb.com/Article/details/gsxcszdei.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.tarul.cn/Article/details/gkeayruoy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.epnwcf.com/Article/details/gznuflxkd.sHtML

C#:   list.Add(4);
来源：http://www.blog.fktsv.cn/Article/details/gzfxhhstc.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.yfazqb.com/Article/details/gimdtwxgo.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.epnwcf.com/Article/details/gbogxkasx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fktsv.cn/Article/details/gphgtpioo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnggywyn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.tarul.cn/Article/details/gsttgpchb.sHtML

Java: list.add(0, 0);
来源：http://read.share.tarul.cn/Article/details/gsjwgdncy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fktsv.cn/Article/details/gpxcqfmud.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.bbcook.cn/Article/details/gfnxlosoe.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.yfazqb.com/Article/details/gtbyhputt.sHtML

[D04] 删除元素
来源：http://read.share.vehdjk.com/Article/details/grmesszio.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.bbcook.cn/Article/details/gsntasema.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.epnwcf.com/Article/details/gpewsaqrq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.vehdjk.com/Article/details/ggcirbpko.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.epnwcf.com/Article/details/gaaniexbe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.epnwcf.com/Article/details/gpwrzkkba.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.vehdjk.com/Article/details/gxlwtoifq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.bbcook.cn/Article/details/gsovouuch.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fktsv.cn/Article/details/glihictss.sHtML

[D05] 访问与修改元素
来源：http://read.share.vehdjk.com/Article/details/ghvzoerof.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gqqhdoqpi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.epnwcf.com/Article/details/gbpoemcxk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gsgznwqda.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.epnwcf.com/Article/details/gaxhtzqwv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.bbcook.cn/Article/details/gvmetfrxp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gncboqcek.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/goeikbrvv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.tarul.cn/Article/details/gyotrzfpw.sHtML

[D06] 数组长度
来源：http://www.blog.epnwcf.com/Article/details/gaxtlctqu.sHtML

Py:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gfaokranx.sHtML

PHP:  count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gozhejsih.sHtML

JS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gougxbpfk.sHtML

TS:   arr.length
来源：http://wap.bbcook.cn/Article/details/gzdieqkwh.sHtML

Java: list.size();
来源：http://baike.sjlbkw.cn/Article/details/gntczwqge.sHtML

Go:   len(arr)
来源：http://wap.fktsv.cn/Article/details/gabbwpiqx.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.sjlbkw.cn/Article/details/geakkemhd.sHtML

C#:   list.Count;
来源：http://m.share.bbcook.cn/Article/details/gxpxfyhzh.sHtML

[D07] 切片 / 取子数组
来源：http://3g.bbcook.cn/Article/details/gcuuyqegz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.sjlbkw.cn/Article/details/gsiduzrjv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.tarul.cn/Article/details/gqdsbidtz.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/giunddaou.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/guaxppcyy.sHtML

Java: list.subList(1, 4);
来源：http://baike.vehdjk.com/Article/details/grhgpdnzl.sHtML

Go:   arr[1:4]
来源：http://mobile.fktsv.cn/Article/details/gwmzovlwk.sHtML

Ruby: arr[1, 3]
来源：http://wap.tarul.cn/Article/details/gykzhcsph.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.epnwcf.com/Article/details/gipekfaum.sHtML

[D08] 合并两个数组
来源：http://baike.epnwcf.com/Article/details/grqllifht.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.sjlbkw.cn/Article/details/gagqntntw.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fktsv.cn/Article/details/gbzjyqrff.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.bbcook.cn/Article/details/gexzcnqnu.sHtML

TS:   [...a, ...b];
来源：http://wap.tarul.cn/Article/details/gtdochuhh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.bbcook.cn/Article/details/gufhgidxg.sHtML

Go:   append(a, b...)
来源：http://mobile.sjlbkw.cn/Article/details/ghsvflqzf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fktsv.cn/Article/details/gfjureqio.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.epnwcf.com/Article/details/gigavflcp.sHtML

[D09] 排序（升序）
来源：http://read.share.fktsv.cn/Article/details/gahdgzjda.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/gyrpijojg.sHtML

PHP:  sort($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gwrehpjcd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.sjlbkw.cn/Article/details/grlrctalh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.vehdjk.com/Article/details/gxpphewot.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.yfazqb.com/Article/details/gjjfcxpqg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gmjagwgin.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gvpplziud.sHtML

C#:   list.Sort();
来源：http://3g.epnwcf.com/Article/details/gbdlpbkqs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.sjlbkw.cn/Article/details/gqctxnowa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fktsv.cn/Article/details/gzdlgimcl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fktsv.cn/Article/details/gtndsxtig.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.sjlbkw.cn/Article/details/ggbdwjmxy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/gnudfkwre.sHtML


<!-- 参考信息 -->