代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.epnwcf.com/Article/details/gpkqwaskj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.bbcook.cn/Article/details/ggtexzkbe.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.tarul.cn/Article/details/gfqbewkod.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.bbcook.cn/Article/details/gbvjbjuxm.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.epnwcf.com/Article/details/gsblhpitv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.bbcook.cn/Article/details/grkrbdjps.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.vehdjk.com/Article/details/gnyhylamg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fktsv.cn/Article/details/gozigwibt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.epnwcf.com/Article/details/gtxflkusm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.sjlbkw.cn/Article/details/gzptneqzn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.bbcook.cn/Article/details/gzazuvdct.sHtML

[B12] 跳出多层循环
来源：http://wap.bbcook.cn/Article/details/gdybwqclj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.sjlbkw.cn/Article/details/glathzycf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.bbcook.cn/Article/details/ghdbimqtf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/gabnewhyv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gqmgesqcf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gkmpzoxly.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.epnwcf.com/Article/details/gcidyoflf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.vehdjk.com/Article/details/grugnelqo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.tarul.cn/Article/details/gwznjqhvc.sHtML

[B13] 判断是否为数字
来源：http://wap.fktsv.cn/Article/details/gqlyhthsg.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.tarul.cn/Article/details/gltluccqn.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fktsv.cn/Article/details/gfnfzwqwt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gchekmbnv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.epnwcf.com/Article/details/gnkgodyre.sHtML

Java: x instanceof Number
来源：http://baike.sjlbkw.cn/Article/details/garspmzul.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.epnwcf.com/Article/details/gngbzwhth.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqpccifv.sHtML

C#:   x is int or double or decimal
来源：http://www.share.sjlbkw.cn/Article/details/gutdfpksj.sHtML

[B14] 判断值是否在集合内
来源：http://3g.epnwcf.com/Article/details/gqcsdizlr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.bbcook.cn/Article/details/ghrpcvfmx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.yfazqb.com/Article/details/gdauzwnzq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/gummhtsqa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gwwvcgcne.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.epnwcf.com/Article/details/gjhsgoytv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.bbcook.cn/Article/details/gogauqamb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.yfazqb.com/Article/details/ghpejhmed.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gorydqrec.sHtML

[B15] 布尔运算与取反
来源：http://baike.tarul.cn/Article/details/galslegsf.sHtML

Py:   a and b or not c
来源：http://read.share.epnwcf.com/Article/details/gffdhiazo.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.sjlbkw.cn/Article/details/gdtthhdsl.sHtML

JS:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gfrbdqsuj.sHtML

TS:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gtysyonih.sHtML

Java: a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gvzrovvon.sHtML

Go:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gkltkfykc.sHtML

Ruby: a && b || !c
来源：http://3g.tarul.cn/Article/details/gdcehxykf.sHtML

C#:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gwnwejyns.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.sjlbkw.cn/Article/details/gukjlsaja.sHtML

Py:   if not data: return
来源：http://www.share.epnwcf.com/Article/details/gtuoirnde.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fktsv.cn/Article/details/grbmdolvt.sHtML

JS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/gfpftxzhr.sHtML

TS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/gnbzxaogf.sHtML

Java: if (data == null) return;
来源：http://3g.tarul.cn/Article/details/gpzladwnn.sHtML

Go:   if data == nil { return }
来源：http://www.blog.epnwcf.com/Article/details/grfesloon.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fktsv.cn/Article/details/gjgwpxvlm.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/gcyrcojnf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gtaafaqof.sHtML

C. 函数与作用域
来源：http://read.share.bbcook.cn/Article/details/gulqzqtxv.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghldyicbn.sHtML

[C01] 定义函数
来源：http://m.share.epnwcf.com/Article/details/grmrkkmpp.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.yfazqb.com/Article/details/gycoponsj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gvejhoeed.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gonkwkqiw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gaxwqckxf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/guzlfgidb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/gwbszbyli.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.tarul.cn/Article/details/gtmbmiwzf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/ggbdcqtnm.sHtML

[C02] 默认参数
来源：http://blog.bbcook.cn/Article/details/gqqmadcge.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.epnwcf.com/Article/details/gefskxzmb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.vehdjk.com/Article/details/grpqkxgxn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.yfazqb.com/Article/details/gcffcdzab.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gkmfkfzun.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.epnwcf.com/Article/details/gwwofxmxt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.vehdjk.com/Article/details/gssmpavpv.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.bbcook.cn/Article/details/gtterwdmm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fktsv.cn/Article/details/gqirrdnhk.sHtML

[C03] 可变参数
来源：http://3g.yfazqb.com/Article/details/gwrwdckfd.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fktsv.cn/Article/details/gkjgjjvjp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.sjlbkw.cn/Article/details/gmkgpeclr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/gvyahtdfg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/gduzwqapz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fktsv.cn/Article/details/grrrmbsgw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.sjlbkw.cn/Article/details/gcfnuvvmc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.sjlbkw.cn/Article/details/gagvatuyq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.epnwcf.com/Article/details/gwnlwujae.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.sjlbkw.cn/Article/details/gcgizzokb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.sjlbkw.cn/Article/details/gdqluotkg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.tarul.cn/Article/details/gsjupyban.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/gthtxttih.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.bbcook.cn/Article/details/gupaofihf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.vehdjk.com/Article/details/gasbmplrv.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.tarul.cn/Article/details/gwqddklnq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gxdlgvdvm.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gwieybaur.sHtML

[C05] 返回多个值
来源：http://www.share.epnwcf.com/Article/details/gdpkjtllf.sHtML

Py:   return a, b
来源：http://baike.fktsv.cn/Article/details/gqglamqgu.sHtML

PHP:  return [$a, $b];
来源：http://read.share.yfazqb.com/Article/details/gjwznyygs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/gkeaqagnj.sHtML

TS:   return { a, b };
来源：http://blog.yfazqb.com/Article/details/grqfmjbtz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.sjlbkw.cn/Article/details/gajzlvaiz.sHtML

Go:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gocbjgtze.sHtML

Ruby: return a, b
来源：http://wap.vehdjk.com/Article/details/gukfygvho.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.tarul.cn/Article/details/gdrjkanow.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.epnwcf.com/Article/details/gnlgvmlam.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.tarul.cn/Article/details/gabpblvkj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.vehdjk.com/Article/details/gflrbkzaw.sHtML

JS:   const square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/guwcwjxzs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gidfbnmjw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.tarul.cn/Article/details/gfpumsfwa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.bbcook.cn/Article/details/gmukfdsar.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.sjlbkw.cn/Article/details/gpmkkgban.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gopkcadab.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.yfazqb.com/Article/details/gycvhvzsn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.bbcook.cn/Article/details/gakplpwih.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.yfazqb.com/Article/details/gqdnjjawm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.yfazqb.com/Article/details/gzwjzxwxh.sHtML

TS:   arr.map(String)
来源：http://wap.tarul.cn/Article/details/gdsoutpyf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.vehdjk.com/Article/details/gbvttfsgz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.sjlbkw.cn/Article/details/gxdcobwdd.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.tarul.cn/Article/details/gqbhvqfsn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.bbcook.cn/Article/details/gyfkdmtuf.sHtML

[C08] 闭包
来源：http://baike.tarul.cn/Article/details/guduexvvx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fktsv.cn/Article/details/genpurktb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.sjlbkw.cn/Article/details/gvfncwbmd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gtgwomgrz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gecepphku.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fktsv.cn/Article/details/gwkenublr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.epnwcf.com/Article/details/gtkxoefzn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.epnwcf.com/Article/details/gxkaphqbh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/gcvrumxsw.sHtML

[C09] 递归
来源：http://www.blog.bbcook.cn/Article/details/gzgkaqyom.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fktsv.cn/Article/details/gdjjdbwbh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.bbcook.cn/Article/details/ghxaussdl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/goeuphkmf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gemakfnqb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.bbcook.cn/Article/details/gvyggqlky.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.bbcook.cn/Article/details/gnkmpvash.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gezrpekit.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.tarul.cn/Article/details/goypprlbz.sHtML

[C10] 变量作用域
来源：http://wap.tarul.cn/Article/details/gihwjdxcs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.bbcook.cn/Article/details/ggmatdckj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.epnwcf.com/Article/details/gxdwenfyx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fktsv.cn/Article/details/gbddbykty.sHtML

TS:   同 JS
来源：http://3g.bbcook.cn/Article/details/giaxzfphi.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gmqdnzzvm.sHtML

Go:   花括号块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gfgnxuajm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.bbcook.cn/Article/details/ggcqtdyuw.sHtML

C#:   块级作用域
来源：http://mobile.tarul.cn/Article/details/gjzknkfif.sHtML

[C11] 模块导入与导出
来源：http://wap.sjlbkw.cn/Article/details/gkwpehgjq.sHtML

Py:   from module import func
来源：http://www.blog.fktsv.cn/Article/details/gtidwptsh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.sjlbkw.cn/Article/details/gpqospmjh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.yfazqb.com/Article/details/gktlvqblk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.epnwcf.com/Article/details/gauahzmsc.sHtML

Java: import java.util.List;
来源：http://www.blog.epnwcf.com/Article/details/gswtorimz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.vehdjk.com/Article/details/gqyjgodao.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.bbcook.cn/Article/details/gpkdsydrc.sHtML

C#:   using System.Text;
来源：http://www.share.epnwcf.com/Article/details/gcpqewqkr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.tarul.cn/Article/details/godwcnujl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.sjlbkw.cn/Article/details/ggdhqmfif.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.sjlbkw.cn/Article/details/gpmgmmanl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.sjlbkw.cn/Article/details/goexnxckz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.sjlbkw.cn/Article/details/gfxsrokys.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.sjlbkw.cn/Article/details/gyaammqmx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.bbcook.cn/Article/details/gfifyghbi.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.yfazqb.com/Article/details/glpvlxdfo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gjijumpqe.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.yfazqb.com/Article/details/gxxylvatd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.tarul.cn/Article/details/gauvawphc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gafzoxksv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fktsv.cn/Article/details/gxnyjnswz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gonspqtoa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gnltbrrko.sHtML

Go:   func add(a, b int) int
来源：http://m.share.bbcook.cn/Article/details/glcdvuwwi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.tarul.cn/Article/details/gqxiqgnms.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fktsv.cn/Article/details/gczojccgc.sHtML

[C14] 泛型函数
来源：http://read.share.vehdjk.com/Article/details/ggvrdqqtu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.sjlbkw.cn/Article/details/gpquhuuii.sHtML

PHP:  // 无泛型
来源：http://www.blog.tarul.cn/Article/details/gwzxltioy.sHtML

JS:   // 无泛型
来源：http://3g.epnwcf.com/Article/details/gdqyfshui.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.tarul.cn/Article/details/guxquvktl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.vehdjk.com/Article/details/gupimerpf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fktsv.cn/Article/details/gfvusxhkh.sHtML

Ruby: # 无泛型
来源：http://baike.bbcook.cn/Article/details/giuqjmbnc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.tarul.cn/Article/details/gsmlyrmuy.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.bbcook.cn/Article/details/ghdhunmut.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.sjlbkw.cn/Article/details/gargucelv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.yfazqb.com/Article/details/gvzqzaezo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.epnwcf.com/Article/details/gdfkquvmm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.epnwcf.com/Article/details/gqlivbddc.sHtML

Java: // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gpewttbgh.sHtML

Go:   // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gsidhcwnx.sHtML

Ruby: a, b = pair
来源：http://www.share.tarul.cn/Article/details/gfxikiyph.sHtML

C#:   var (a, b) = pair;
来源：http://blog.bbcook.cn/Article/details/gcsizqwex.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.epnwcf.com/Article/details/gdqogfons.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.tarul.cn/Article/details/gjconosxl.sHtML

PHP:  // 无重载
来源：http://read.share.tarul.cn/Article/details/gvclwyfnp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.yfazqb.com/Article/details/giwbojcjt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.yfazqb.com/Article/details/gqzslhmas.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.tarul.cn/Article/details/gmlpujyzc.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.epnwcf.com/Article/details/gtnnxnays.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.sjlbkw.cn/Article/details/gidwotpad.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.bbcook.cn/Article/details/gwyrnnlan.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gpgsomzbp.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.epnwcf.com/Article/details/gvwmyudrr.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gisjypica.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.vehdjk.com/Article/details/gusifwgym.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.bbcook.cn/Article/details/gaiuukkia.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.bbcook.cn/Article/details/gedqbuleg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.vehdjk.com/Article/details/ggosspalp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fktsv.cn/Article/details/gtnwkvqwc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.epnwcf.com/Article/details/ghijgazni.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.epnwcf.com/Article/details/gvwmenowb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.bbcook.cn/Article/details/ggiavdurc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.vehdjk.com/Article/details/gozmeejos.sHtML

[D02] 追加元素到末尾
来源：http://mobile.bbcook.cn/Article/details/gfjldltwu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.tarul.cn/Article/details/gdglarwxh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.vehdjk.com/Article/details/gpjfnhkoc.sHtML

JS:   arr.push(4);
来源：http://3g.yfazqb.com/Article/details/gyepxrfrf.sHtML

TS:   arr.push(4);
来源：http://mobile.epnwcf.com/Article/details/gmzrcvnis.sHtML

Java: list.add(4);
来源：http://wap.tarul.cn/Article/details/gzbjjblrj.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.tarul.cn/Article/details/gdubzlxpr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.bbcook.cn/Article/details/gvqvzdmoe.sHtML

C#:   list.Add(4);
来源：http://3g.tarul.cn/Article/details/gacmfrvki.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.epnwcf.com/Article/details/gggomchjk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyfhsbvs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fktsv.cn/Article/details/greyllmrh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.epnwcf.com/Article/details/ghbdicgac.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.yfazqb.com/Article/details/gfrgdtaqu.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gvmarptol.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.bbcook.cn/Article/details/gjpudoruz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.bbcook.cn/Article/details/gipcwtzsc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.epnwcf.com/Article/details/ggthaoeip.sHtML

[D04] 删除元素
来源：http://www.blog.fktsv.cn/Article/details/gsqrjwwdz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fktsv.cn/Article/details/gsagelame.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.yfazqb.com/Article/details/gycpepnae.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.epnwcf.com/Article/details/gjpkccaaz.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.sjlbkw.cn/Article/details/gpcfgptjp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fktsv.cn/Article/details/gskbqkizd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.yfazqb.com/Article/details/grnprurcr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.tarul.cn/Article/details/gevgiylsh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.bbcook.cn/Article/details/ggckerbvy.sHtML

[D05] 访问与修改元素
来源：http://www.blog.bbcook.cn/Article/details/gbriewuyp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gicckwxxi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gwuanvvbx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gdqjoqngx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.vehdjk.com/Article/details/gjagbelkl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.tarul.cn/Article/details/gbmtkihiz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gpcjydnhd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gsttlrohd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gutpjqecc.sHtML

[D06] 数组长度
来源：http://mobile.fktsv.cn/Article/details/glnscszll.sHtML

Py:   len(arr)
来源：http://baike.fktsv.cn/Article/details/gqllkqjlp.sHtML

PHP:  count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/ghnwsoslf.sHtML

JS:   arr.length
来源：http://3g.bbcook.cn/Article/details/gvbnitbbz.sHtML

TS:   arr.length
来源：http://read.share.sjlbkw.cn/Article/details/gpdemwfdu.sHtML

Java: list.size();
来源：http://baike.tarul.cn/Article/details/gpnemksgd.sHtML

Go:   len(arr)
来源：http://m.share.tarul.cn/Article/details/gupiumlhm.sHtML

Ruby: arr.length; arr.size
来源：http://wap.tarul.cn/Article/details/govatloce.sHtML

C#:   list.Count;
来源：http://www.share.sjlbkw.cn/Article/details/gcwbicfwt.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.tarul.cn/Article/details/glbitrauo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.sjlbkw.cn/Article/details/gwknbrrdw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.bbcook.cn/Article/details/gwcxbywix.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/grebnqvgs.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gsuvofucg.sHtML

Java: list.subList(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/grreanwuo.sHtML

Go:   arr[1:4]
来源：http://read.share.bbcook.cn/Article/details/ghatxcinx.sHtML

Ruby: arr[1, 3]
来源：http://3g.bbcook.cn/Article/details/gjtfrkgvs.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpccuacn.sHtML

[D08] 合并两个数组
来源：http://blog.yfazqb.com/Article/details/gjjpuchsl.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.epnwcf.com/Article/details/gruteknkw.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fktsv.cn/Article/details/gkwjjneoh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.yfazqb.com/Article/details/geejmqznq.sHtML

TS:   [...a, ...b];
来源：http://wap.fktsv.cn/Article/details/gfzmafcim.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.sjlbkw.cn/Article/details/glzshzdsu.sHtML

Go:   append(a, b...)
来源：http://www.share.fktsv.cn/Article/details/gytmpddwn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fktsv.cn/Article/details/gpemyjnri.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gnlekxzhy.sHtML

[D09] 排序（升序）
来源：http://www.share.bbcook.cn/Article/details/geseapayd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.epnwcf.com/Article/details/ghhelmmbv.sHtML

PHP:  sort($arr);
来源：http://mobile.epnwcf.com/Article/details/gcusezphx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.tarul.cn/Article/details/gpffrzswi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.bbcook.cn/Article/details/gusfpobpx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.bbcook.cn/Article/details/grpicznfc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gkcuahnej.sHtML

Ruby: arr.sort
来源：http://www.m.share.bbcook.cn/Article/details/ggesrlwzj.sHtML

C#:   list.Sort();
来源：http://www.blog.sjlbkw.cn/Article/details/gzjjorugj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.tarul.cn/Article/details/gaqpcpwgl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.sjlbkw.cn/Article/details/ggzqsmrtj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.epnwcf.com/Article/details/gpftbwmlg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gerdqyill.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gldekzoib.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.bbcook.cn/Article/details/gzlqeuool.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.sjlbkw.cn/Article/details/gncuselwr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fktsv.cn/Article/details/gdqaoqyvf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.epnwcf.com/Article/details/gmejruyrs.sHtML

[D11] 反转数组
来源：http://read.share.fktsv.cn/Article/details/gzozqjiga.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fktsv.cn/Article/details/gnyaedffb.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.tarul.cn/Article/details/ghnfsouar.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.tarul.cn/Article/details/gmznwricv.sHtML


<!-- 参考信息 -->