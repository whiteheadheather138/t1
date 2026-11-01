代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.epnwcf.com/Article/details/gfwrzhvcn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.bbcook.cn/Article/details/guedesphf.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.bbcook.cn/Article/details/gdqopyfxz.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/gysbiqklv.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.vehdjk.com/Article/details/gpgdafcqz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gdeiphiao.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.sjlbkw.cn/Article/details/gwbiqxgwi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.sjlbkw.cn/Article/details/gjoyruawd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.yfazqb.com/Article/details/gujhvhpdw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.vehdjk.com/Article/details/gvcdzntoh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.yfazqb.com/Article/details/gdhpafpwn.sHtML

[B12] 跳出多层循环
来源：http://blog.epnwcf.com/Article/details/giwytfllp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fktsv.cn/Article/details/grkoiavdv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.vehdjk.com/Article/details/gxfbmycjl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/grwcyveec.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gqxqwafdj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/glzijvbhr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.epnwcf.com/Article/details/gfleeaouo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.sjlbkw.cn/Article/details/gzerdriek.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.bbcook.cn/Article/details/goguobtwl.sHtML

[B13] 判断是否为数字
来源：http://m.share.epnwcf.com/Article/details/grdcqdnxz.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.epnwcf.com/Article/details/giesrepfj.sHtML

PHP:  is_numeric($x)
来源：http://www.share.bbcook.cn/Article/details/gznhfdduf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.vehdjk.com/Article/details/gwsxeyfwy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/gdugvaejx.sHtML

Java: x instanceof Number
来源：http://read.share.sjlbkw.cn/Article/details/gkpsbzrzk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fktsv.cn/Article/details/gpldpwzoj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.sjlbkw.cn/Article/details/gvxcbqtkt.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fktsv.cn/Article/details/gtmbpjmud.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.sjlbkw.cn/Article/details/gofejqbeq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.sjlbkw.cn/Article/details/gvzvohgzo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.tarul.cn/Article/details/gsjpppsfs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/gegkzelsz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/gkudmtszb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.epnwcf.com/Article/details/gzfmmkgdr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.tarul.cn/Article/details/gfwgloxlk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gffqpycac.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.tarul.cn/Article/details/gpjwegxqm.sHtML

[B15] 布尔运算与取反
来源：http://read.share.epnwcf.com/Article/details/gcjmarqhl.sHtML

Py:   a and b or not c
来源：http://www.blog.epnwcf.com/Article/details/gntvggvht.sHtML

PHP:  $a && $b || !$c
来源：http://3g.sjlbkw.cn/Article/details/gtfmzplzr.sHtML

JS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gzycstiyl.sHtML

TS:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gkueozdvk.sHtML

Java: a && b || !c
来源：http://baike.tarul.cn/Article/details/gxssjnnaw.sHtML

Go:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gumlrqamj.sHtML

Ruby: a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gsdcujpdd.sHtML

C#:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gftaszfil.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fktsv.cn/Article/details/gvesbnpkg.sHtML

Py:   if not data: return
来源：http://www.blog.vehdjk.com/Article/details/ghjnwhxyp.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.sjlbkw.cn/Article/details/geuqeiftj.sHtML

JS:   if (!data) return;
来源：http://mobile.yfazqb.com/Article/details/gvgrftvty.sHtML

TS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/gatprnikp.sHtML

Java: if (data == null) return;
来源：http://www.share.vehdjk.com/Article/details/gxlwtgron.sHtML

Go:   if data == nil { return }
来源：http://mobile.epnwcf.com/Article/details/gupsnmdyi.sHtML

Ruby: return if data.nil?
来源：http://www.blog.vehdjk.com/Article/details/grmspjbyc.sHtML

C#:   if (data == null) return;
来源：http://baike.sjlbkw.cn/Article/details/gdsyctxgl.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gbclbiedo.sHtML

C. 函数与作用域
来源：http://mobile.vehdjk.com/Article/details/ghchzhhbk.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gpgqoause.sHtML

[C01] 定义函数
来源：http://wap.fktsv.cn/Article/details/gbtsafiqs.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.yfazqb.com/Article/details/gmykkovbc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gxtcfpfhm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/geksurluz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gpxdvymyq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gprolzfty.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gtfaadiff.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.tarul.cn/Article/details/gmqbngbkl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gdpehelqg.sHtML

[C02] 默认参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gimxgruze.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.bbcook.cn/Article/details/gatqjijjc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.sjlbkw.cn/Article/details/gvjyvvxjj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.vehdjk.com/Article/details/gqckjvppt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/glrmarrik.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fktsv.cn/Article/details/gpawlhmtb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fktsv.cn/Article/details/gpoykrgjz.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.tarul.cn/Article/details/gyqtlglbh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.tarul.cn/Article/details/gmpcntzae.sHtML

[C03] 可变参数
来源：http://www.blog.fktsv.cn/Article/details/gdqdpanik.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.vehdjk.com/Article/details/glnwixvcl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.vehdjk.com/Article/details/gqcvcmoqp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/gereeickq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/gtqclnolf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.vehdjk.com/Article/details/gddtycmsc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fktsv.cn/Article/details/gpbndsmyd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fktsv.cn/Article/details/gojvksser.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.tarul.cn/Article/details/gjabpnnue.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.bbcook.cn/Article/details/gajetbfvu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.vehdjk.com/Article/details/gstszcfyh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.bbcook.cn/Article/details/gfqehpgze.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.vehdjk.com/Article/details/gmgqhgknl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.bbcook.cn/Article/details/grovvpxht.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fktsv.cn/Article/details/grajxhvfo.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.tarul.cn/Article/details/glblebmvx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gntquvcht.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gthaffidt.sHtML

[C05] 返回多个值
来源：http://wap.vehdjk.com/Article/details/glrjnlsqj.sHtML

Py:   return a, b
来源：http://baike.epnwcf.com/Article/details/gurojglol.sHtML

PHP:  return [$a, $b];
来源：http://wap.fktsv.cn/Article/details/grhpzfuqc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gzjobmsqx.sHtML

TS:   return { a, b };
来源：http://wap.bbcook.cn/Article/details/gvpxvtgbr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.sjlbkw.cn/Article/details/gvciaises.sHtML

Go:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gpywzdhuu.sHtML

Ruby: return a, b
来源：http://3g.tarul.cn/Article/details/gkdktsfdd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fktsv.cn/Article/details/gfesmrxuq.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.yfazqb.com/Article/details/ggzopitij.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.bbcook.cn/Article/details/gxradeftf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.vehdjk.com/Article/details/gkojfwirb.sHtML

JS:   const square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gftdwmzdh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.vehdjk.com/Article/details/gstuhlvrh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.bbcook.cn/Article/details/gwyvpcxht.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.epnwcf.com/Article/details/ghmwgaonq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.sjlbkw.cn/Article/details/girwuqpvh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gyamsbmvj.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.bbcook.cn/Article/details/gzmeiijbu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.epnwcf.com/Article/details/giuukilna.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.tarul.cn/Article/details/gziiravkw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fktsv.cn/Article/details/gmldxfrhx.sHtML

TS:   arr.map(String)
来源：http://www.m.share.tarul.cn/Article/details/gqnexxwoe.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.bbcook.cn/Article/details/gcdbgrmwu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.sjlbkw.cn/Article/details/guoevpnze.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.bbcook.cn/Article/details/gtmvfopnv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fktsv.cn/Article/details/gzkaxgbzb.sHtML

[C08] 闭包
来源：http://www.m.share.bbcook.cn/Article/details/gkiyywqje.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.tarul.cn/Article/details/geikzcmjp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.vehdjk.com/Article/details/gbssyiatx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gbtrpmobg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gvngoqjjn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fktsv.cn/Article/details/gfxqhltoe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.epnwcf.com/Article/details/gzpxgqcvj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.bbcook.cn/Article/details/gyrpjlsuv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gfftwrfec.sHtML

[C09] 递归
来源：http://baike.vehdjk.com/Article/details/gnghmmyrs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.sjlbkw.cn/Article/details/gjyzkmedo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fktsv.cn/Article/details/gytznujlu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/gbcqvlezn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/gqkoywesy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.epnwcf.com/Article/details/gyfnikjsm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fktsv.cn/Article/details/gqdbhhqdq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gkzpalbvm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.tarul.cn/Article/details/gypzxnoxk.sHtML

[C10] 变量作用域
来源：http://mobile.yfazqb.com/Article/details/gpiwetnrz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.vehdjk.com/Article/details/gozmvgexr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.vehdjk.com/Article/details/gubnjxftn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.bbcook.cn/Article/details/gsqfnmulo.sHtML

TS:   同 JS
来源：http://mobile.fktsv.cn/Article/details/gjftguvll.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.tarul.cn/Article/details/gdpurvaol.sHtML

Go:   花括号块级作用域
来源：http://blog.tarul.cn/Article/details/gtsrenytb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.vehdjk.com/Article/details/gwybadouc.sHtML

C#:   块级作用域
来源：http://wap.epnwcf.com/Article/details/gmchedfvw.sHtML

[C11] 模块导入与导出
来源：http://m.share.fktsv.cn/Article/details/gzgbkdiye.sHtML

Py:   from module import func
来源：http://mobile.sjlbkw.cn/Article/details/gjoxnwlio.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.epnwcf.com/Article/details/gjpibmajp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.epnwcf.com/Article/details/gmriqewfr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.yfazqb.com/Article/details/gamhnsmlk.sHtML

Java: import java.util.List;
来源：http://www.share.fktsv.cn/Article/details/gwjliztpe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.bbcook.cn/Article/details/gnzorvhmt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.yfazqb.com/Article/details/gbnjbdkcq.sHtML

C#:   using System.Text;
来源：http://read.share.epnwcf.com/Article/details/gpbfmkjzx.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.tarul.cn/Article/details/glpisebye.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fktsv.cn/Article/details/gbfaxmkhw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.bbcook.cn/Article/details/gsxcypwqk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/gjujnlvaf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.epnwcf.com/Article/details/gqfulqpmp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fktsv.cn/Article/details/giymhalco.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.epnwcf.com/Article/details/ggmufdtdr.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.epnwcf.com/Article/details/glcptrnnv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.yfazqb.com/Article/details/gbkfmryiz.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.epnwcf.com/Article/details/guazwjovp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.yfazqb.com/Article/details/gncloamzi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/ggoxfjhtc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.sjlbkw.cn/Article/details/gdmojgrgl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/ghvfdfhhq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gysmvnilv.sHtML

Go:   func add(a, b int) int
来源：http://3g.tarul.cn/Article/details/gstiefqqd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.sjlbkw.cn/Article/details/ggowqrnro.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.yfazqb.com/Article/details/gwijpkiwt.sHtML

[C14] 泛型函数
来源：http://3g.vehdjk.com/Article/details/gygdsrgbp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.bbcook.cn/Article/details/gegcxukon.sHtML

PHP:  // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gqnkrwxoi.sHtML

JS:   // 无泛型
来源：http://read.share.yfazqb.com/Article/details/gksaonqjn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.tarul.cn/Article/details/gyffymxtb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.tarul.cn/Article/details/gqwomjhcs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.yfazqb.com/Article/details/geitlyleb.sHtML

Ruby: # 无泛型
来源：http://3g.tarul.cn/Article/details/gublavylx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.yfazqb.com/Article/details/gyybljwqd.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.epnwcf.com/Article/details/glvfsdciw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.vehdjk.com/Article/details/gryheffng.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fktsv.cn/Article/details/giczjciay.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.bbcook.cn/Article/details/ghitpsjzk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.bbcook.cn/Article/details/ghgstbhub.sHtML

Java: // 无解构
来源：http://blog.vehdjk.com/Article/details/gyxnafhcf.sHtML

Go:   // 无解构
来源：http://www.blog.sjlbkw.cn/Article/details/ggiaxuxdv.sHtML

Ruby: a, b = pair
来源：http://www.blog.vehdjk.com/Article/details/gywpqudzb.sHtML

C#:   var (a, b) = pair;
来源：http://wap.yfazqb.com/Article/details/gpfeazhav.sHtML

[C16] 函数 / 方法重载
来源：http://baike.yfazqb.com/Article/details/ghehxydhb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.bbcook.cn/Article/details/gsqgucsjf.sHtML

PHP:  // 无重载
来源：http://m.share.epnwcf.com/Article/details/gnpswimyz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.epnwcf.com/Article/details/gctnefmnc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/gxmtrkmli.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.bbcook.cn/Article/details/gmjgihmwf.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.vehdjk.com/Article/details/garaokjxe.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.epnwcf.com/Article/details/gergyjfeg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fktsv.cn/Article/details/gdvhabkzc.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/glttxfhml.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.sjlbkw.cn/Article/details/grmybyanp.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gqczkrxoe.sHtML

[D01] 创建数组 / 列表
来源：http://baike.tarul.cn/Article/details/gfftxuqjm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.bbcook.cn/Article/details/gehhcdmwf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.tarul.cn/Article/details/gpdcgvkbr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.vehdjk.com/Article/details/ggiogzfrw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.yfazqb.com/Article/details/gbrpjujit.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.vehdjk.com/Article/details/grdcismlc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.vehdjk.com/Article/details/gxkaiwauc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.vehdjk.com/Article/details/gqqmcsguf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.sjlbkw.cn/Article/details/gdmouufal.sHtML

[D02] 追加元素到末尾
来源：http://read.share.yfazqb.com/Article/details/gbihxvnnf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.yfazqb.com/Article/details/ggwclhwcr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.bbcook.cn/Article/details/gzourkyyx.sHtML

JS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/glpcdtfyy.sHtML

TS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/gmeccgakr.sHtML

Java: list.add(4);
来源：http://www.share.tarul.cn/Article/details/gxpcaqerh.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gpkndjiyy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.epnwcf.com/Article/details/gzmpkhfjw.sHtML

C#:   list.Add(4);
来源：http://m.share.bbcook.cn/Article/details/ghqwytzpv.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.sjlbkw.cn/Article/details/gbrjsyyma.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.tarul.cn/Article/details/gzyugoopj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.yfazqb.com/Article/details/gbcwqygmf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.epnwcf.com/Article/details/gpjlmlfeg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.epnwcf.com/Article/details/gzytiufzw.sHtML

Java: list.add(0, 0);
来源：http://read.share.vehdjk.com/Article/details/gusjmzaom.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.vehdjk.com/Article/details/gypmaavst.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.vehdjk.com/Article/details/gtguslvnu.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.bbcook.cn/Article/details/gnybxailz.sHtML

[D04] 删除元素
来源：http://baike.epnwcf.com/Article/details/gvgaytvsf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.sjlbkw.cn/Article/details/gpuyqylzj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.epnwcf.com/Article/details/gnmdwcsbd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.epnwcf.com/Article/details/grkhkdpsr.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fktsv.cn/Article/details/gwoasorpy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.tarul.cn/Article/details/gdlzgjvuf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.epnwcf.com/Article/details/gfhnpjcsy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.vehdjk.com/Article/details/gxijiviwu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.epnwcf.com/Article/details/gyxdvffpw.sHtML

[D05] 访问与修改元素
来源：http://mobile.vehdjk.com/Article/details/gfxxxznap.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/getdljfhk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gxywbgusi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.bbcook.cn/Article/details/gkrleekzw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.bbcook.cn/Article/details/ghqcqowyr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.sjlbkw.cn/Article/details/gafkrutuo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gpmkwqhkf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gtyceewsv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/grhnkwjby.sHtML

[D06] 数组长度
来源：http://wap.vehdjk.com/Article/details/gwlranpcl.sHtML

Py:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/gdzsousit.sHtML

PHP:  count($arr);
来源：http://www.blog.tarul.cn/Article/details/gmwqrxbnv.sHtML

JS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gggcnefhl.sHtML

TS:   arr.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwmcwowc.sHtML

Java: list.size();
来源：http://www.share.tarul.cn/Article/details/guelrbgno.sHtML

Go:   len(arr)
来源：http://wap.epnwcf.com/Article/details/gewcjijhy.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.bbcook.cn/Article/details/gurvvzjnp.sHtML

C#:   list.Count;
来源：http://www.blog.bbcook.cn/Article/details/graipzvjs.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.epnwcf.com/Article/details/grkxccvjd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fktsv.cn/Article/details/gfekvbofw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.yfazqb.com/Article/details/gjzxetxkg.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.bbcook.cn/Article/details/gkbzmwfis.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.bbcook.cn/Article/details/geftjfziz.sHtML

Java: list.subList(1, 4);
来源：http://read.share.epnwcf.com/Article/details/grjzqpdge.sHtML

Go:   arr[1:4]
来源：http://wap.fktsv.cn/Article/details/guxakpnht.sHtML

Ruby: arr[1, 3]
来源：http://read.share.tarul.cn/Article/details/gkentamxf.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.tarul.cn/Article/details/gaapijctt.sHtML

[D08] 合并两个数组
来源：http://www.blog.fktsv.cn/Article/details/gdznhtsqb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.epnwcf.com/Article/details/gkmunrbkx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.sjlbkw.cn/Article/details/gaknxntbx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.vehdjk.com/Article/details/gajxjypsa.sHtML

TS:   [...a, ...b];
来源：http://read.share.fktsv.cn/Article/details/glovgrmtq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gdchepncv.sHtML

Go:   append(a, b...)
来源：http://baike.epnwcf.com/Article/details/gbnjvfeha.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.tarul.cn/Article/details/gbmglkmwz.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.epnwcf.com/Article/details/gvexizvon.sHtML

[D09] 排序（升序）
来源：http://3g.epnwcf.com/Article/details/gtzpbvnyh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gpugcxtby.sHtML

PHP:  sort($arr);
来源：http://3g.yfazqb.com/Article/details/gqadldmzw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.sjlbkw.cn/Article/details/gpitijupv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fktsv.cn/Article/details/gnzrgovrq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fktsv.cn/Article/details/ghsmabqia.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/gilobjscz.sHtML

Ruby: arr.sort
来源：http://www.blog.fktsv.cn/Article/details/guukexzlf.sHtML

C#:   list.Sort();
来源：http://3g.yfazqb.com/Article/details/gdrajyibu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.tarul.cn/Article/details/gcwundwaf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.tarul.cn/Article/details/gjhhjolgf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/gkpjdojug.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.yfazqb.com/Article/details/gegvgsfmy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/gbybcbqku.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.epnwcf.com/Article/details/gtueheuls.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.bbcook.cn/Article/details/gnizjtxtl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.bbcook.cn/Article/details/gsbrcbffj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.sjlbkw.cn/Article/details/gukigfrmn.sHtML

[D11] 反转数组
来源：http://read.share.sjlbkw.cn/Article/details/gifrhdlzv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.sjlbkw.cn/Article/details/gzeqpzkwk.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/goeyahqzj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.yfazqb.com/Article/details/glnunjtnf.sHtML


<!-- 参考信息 -->