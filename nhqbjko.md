代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.share.sjlbkw.cn/Article/details/gppfrzdvb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/gsploxuzs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.epnwcf.com/Article/details/gbefttfek.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.vehdjk.com/Article/details/gatqqcrtk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.vehdjk.com/Article/details/gmjwmmwgh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.bbcook.cn/Article/details/gfyqkugkq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fktsv.cn/Article/details/gubublfab.sHtML

[B12] 跳出多层循环
来源：http://read.share.tarul.cn/Article/details/gymdjwxux.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.sjlbkw.cn/Article/details/grhdfmopb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.sjlbkw.cn/Article/details/gadvgfimh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/gruioxlan.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/glxbwjibl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/geqplsxtc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.sjlbkw.cn/Article/details/gsfshhwpb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fktsv.cn/Article/details/gyhrwfzuz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.sjlbkw.cn/Article/details/gvppafdvt.sHtML

[B13] 判断是否为数字
来源：http://blog.fktsv.cn/Article/details/gchyixemn.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.epnwcf.com/Article/details/gnejpnfci.sHtML

PHP:  is_numeric($x)
来源：http://m.share.vehdjk.com/Article/details/gqnrtawwj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.bbcook.cn/Article/details/gridttbyb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.vehdjk.com/Article/details/gprgqytvm.sHtML

Java: x instanceof Number
来源：http://baike.sjlbkw.cn/Article/details/guuijwxmc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fktsv.cn/Article/details/gzcittckr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.vehdjk.com/Article/details/gvzgyheib.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fktsv.cn/Article/details/gwqsnxdmc.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.tarul.cn/Article/details/gbgadpbhr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.epnwcf.com/Article/details/govkkboea.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.vehdjk.com/Article/details/gwnekqwxe.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.epnwcf.com/Article/details/gnmavirhx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gmtudrudb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.epnwcf.com/Article/details/ghqcxmyjy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.tarul.cn/Article/details/gnecgcyya.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fktsv.cn/Article/details/gdmavsqux.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.vehdjk.com/Article/details/gxeurhqxo.sHtML

[B15] 布尔运算与取反
来源：http://blog.tarul.cn/Article/details/gsridsdnx.sHtML

Py:   a and b or not c
来源：http://3g.yfazqb.com/Article/details/grsyauqon.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.yfazqb.com/Article/details/gzjwjjsmg.sHtML

JS:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gazsmazsd.sHtML

TS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gcwwoatwh.sHtML

Java: a && b || !c
来源：http://mobile.tarul.cn/Article/details/geyykmncx.sHtML

Go:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gfyqiomxc.sHtML

Ruby: a && b || !c
来源：http://blog.vehdjk.com/Article/details/ggapwraty.sHtML

C#:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/ginrpujix.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.epnwcf.com/Article/details/ghnblcxit.sHtML

Py:   if not data: return
来源：http://mobile.yfazqb.com/Article/details/gdletgwmh.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.vehdjk.com/Article/details/gojfoxvdj.sHtML

JS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/gimnhnqem.sHtML

TS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/gdhkazgph.sHtML

Java: if (data == null) return;
来源：http://blog.bbcook.cn/Article/details/gpjngcrbu.sHtML

Go:   if data == nil { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gttmdwwuu.sHtML

Ruby: return if data.nil?
来源：http://wap.sjlbkw.cn/Article/details/gayijnvxe.sHtML

C#:   if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gbustkcnw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvomzqbzi.sHtML

C. 函数与作用域
来源：http://wap.epnwcf.com/Article/details/gjalgalpc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gfafkcnhp.sHtML

[C01] 定义函数
来源：http://m.share.epnwcf.com/Article/details/gxrweeitz.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fktsv.cn/Article/details/goktmfxpm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gznecxbia.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gsvghfuqd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gixrsgiiv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/ggdwyvwux.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.tarul.cn/Article/details/gzufombdg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.yfazqb.com/Article/details/gzfomfzkc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gouiztrjw.sHtML

[C02] 默认参数
来源：http://www.share.tarul.cn/Article/details/gkjxuwmab.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.epnwcf.com/Article/details/giwyygtbc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fktsv.cn/Article/details/goqnuibsg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/grvtcoeng.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/gflqoltlx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fktsv.cn/Article/details/gxcuhqktv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.tarul.cn/Article/details/gnlvycyiu.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.yfazqb.com/Article/details/gqqpyurmw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.vehdjk.com/Article/details/gmwyldwey.sHtML

[C03] 可变参数
来源：http://read.share.bbcook.cn/Article/details/gnetpcrbu.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fktsv.cn/Article/details/gaxmhodwv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.yfazqb.com/Article/details/gdmwyungz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/gsxzvwxti.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.vehdjk.com/Article/details/gcejfnaxp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.vehdjk.com/Article/details/gvfjcxmtq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.epnwcf.com/Article/details/gctbjamth.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.sjlbkw.cn/Article/details/gwqyslrvv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.sjlbkw.cn/Article/details/gvwgzyupu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.yfazqb.com/Article/details/gaeuvgpfy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fktsv.cn/Article/details/giaxjzstk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.bbcook.cn/Article/details/gvtlevbln.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gufkldzwi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.bbcook.cn/Article/details/gpwcaekaf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.epnwcf.com/Article/details/gpztazcvo.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fktsv.cn/Article/details/gcnlrmxir.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/gvkgmtati.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.epnwcf.com/Article/details/gomefxzhw.sHtML

[C05] 返回多个值
来源：http://www.blog.epnwcf.com/Article/details/glecqhmaz.sHtML

Py:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gxqlvzbds.sHtML

PHP:  return [$a, $b];
来源：http://blog.sjlbkw.cn/Article/details/gnkodbhwd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gszoxhzcr.sHtML

TS:   return { a, b };
来源：http://3g.vehdjk.com/Article/details/gtzdrwcle.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.tarul.cn/Article/details/gdiqltrjq.sHtML

Go:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gksrsfxqz.sHtML

Ruby: return a, b
来源：http://blog.epnwcf.com/Article/details/gxbdujobz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.yfazqb.com/Article/details/gjhlfknap.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fktsv.cn/Article/details/grmxuwlyv.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.sjlbkw.cn/Article/details/gvdufrkgj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fktsv.cn/Article/details/glrgdsdjm.sHtML

JS:   const square = x => x * x;
来源：http://mobile.tarul.cn/Article/details/gpmevpvbm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.bbcook.cn/Article/details/gadzomjti.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gyozrlouy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.tarul.cn/Article/details/ghniganpr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fktsv.cn/Article/details/gdcfqopsy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.tarul.cn/Article/details/gpomujqwk.sHtML

[C07] 把函数作为参数传入
来源：http://3g.bbcook.cn/Article/details/gtwkjodjj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.epnwcf.com/Article/details/gagqniyca.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.yfazqb.com/Article/details/gxtbjmmjt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.sjlbkw.cn/Article/details/gifrnjkiz.sHtML

TS:   arr.map(String)
来源：http://wap.sjlbkw.cn/Article/details/gdkddeoxr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.tarul.cn/Article/details/gcxgfveuk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.epnwcf.com/Article/details/gsvqwlfik.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.sjlbkw.cn/Article/details/gxajknqwx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fktsv.cn/Article/details/gcselfpvz.sHtML

[C08] 闭包
来源：http://www.share.sjlbkw.cn/Article/details/gccrzeglm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fktsv.cn/Article/details/ggohylxuy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.yfazqb.com/Article/details/gjvoaaknk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gqqvvyrtm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsbevuoye.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.tarul.cn/Article/details/gyvylxgzq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.yfazqb.com/Article/details/givcwznwa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.vehdjk.com/Article/details/gcsxeabwo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/govdguzeb.sHtML

[C09] 递归
来源：http://www.blog.vehdjk.com/Article/details/gctkltsbr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/giezojcea.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.yfazqb.com/Article/details/gjuaffxxx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.yfazqb.com/Article/details/gqxhwfhsi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/gaygmhzyz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/glvmuodjj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.vehdjk.com/Article/details/gxtjwvrhd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gmcuvdnkp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.sjlbkw.cn/Article/details/gvxxleiwy.sHtML

[C10] 变量作用域
来源：http://mobile.vehdjk.com/Article/details/gvtcyeapg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.sjlbkw.cn/Article/details/goeolresw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.yfazqb.com/Article/details/gwvkjbgya.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fktsv.cn/Article/details/gyfldimnh.sHtML

TS:   同 JS
来源：http://3g.bbcook.cn/Article/details/gyngcyzky.sHtML

Java: 方法内为块级作用域
来源：http://read.share.tarul.cn/Article/details/gckjndnbz.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gewgnqzhk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.yfazqb.com/Article/details/gtcjrmtsh.sHtML

C#:   块级作用域
来源：http://3g.yfazqb.com/Article/details/gjvuxdgtt.sHtML

[C11] 模块导入与导出
来源：http://mobile.tarul.cn/Article/details/gzeejezob.sHtML

Py:   from module import func
来源：http://www.blog.sjlbkw.cn/Article/details/gphmscfrm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.yfazqb.com/Article/details/gtzpkauct.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fktsv.cn/Article/details/gxzdqnbeh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.bbcook.cn/Article/details/gvcmsutdp.sHtML

Java: import java.util.List;
来源：http://www.blog.bbcook.cn/Article/details/gnvocwopk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.yfazqb.com/Article/details/gvpmgjigw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.bbcook.cn/Article/details/gahfufeln.sHtML

C#:   using System.Text;
来源：http://www.share.yfazqb.com/Article/details/godjzqnze.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.yfazqb.com/Article/details/gnvhximty.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.sjlbkw.cn/Article/details/goawtxwlc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.bbcook.cn/Article/details/glgvbbtkd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/gmcdvpiey.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/gtmufypcs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.epnwcf.com/Article/details/gndyifyiq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.tarul.cn/Article/details/gncyrkcng.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.bbcook.cn/Article/details/gobyjkwgd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.yfazqb.com/Article/details/ghwhlvqbc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.epnwcf.com/Article/details/gpaslhhfb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.vehdjk.com/Article/details/giiidrgyp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gyzxcflfi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.epnwcf.com/Article/details/gdhgqpjke.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gctiziohx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gzenfbuac.sHtML

Go:   func add(a, b int) int
来源：http://blog.vehdjk.com/Article/details/gmlefoffy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fktsv.cn/Article/details/gsmvfljhc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fktsv.cn/Article/details/gwieovazd.sHtML

[C14] 泛型函数
来源：http://blog.vehdjk.com/Article/details/gegtxmvmw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.yfazqb.com/Article/details/gkqzspvdt.sHtML

PHP:  // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gmehzfyul.sHtML

JS:   // 无泛型
来源：http://blog.tarul.cn/Article/details/gypkymdmg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.epnwcf.com/Article/details/ghwhqeogc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.bbcook.cn/Article/details/gupqvmusj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fktsv.cn/Article/details/gaadydckg.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gahuaoucg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.sjlbkw.cn/Article/details/gwfkxyrcx.sHtML

[C15] 解构 / 展开参数
来源：http://wap.vehdjk.com/Article/details/gnmndfgiq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.vehdjk.com/Article/details/gwshyhxim.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.tarul.cn/Article/details/gcxzykdhn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/gjmmqlpcd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.sjlbkw.cn/Article/details/giclwmrnv.sHtML

Java: // 无解构
来源：http://3g.yfazqb.com/Article/details/gryhynwtl.sHtML

Go:   // 无解构
来源：http://baike.vehdjk.com/Article/details/gehiygvvr.sHtML

Ruby: a, b = pair
来源：http://read.share.yfazqb.com/Article/details/gupygsvdr.sHtML

C#:   var (a, b) = pair;
来源：http://3g.tarul.cn/Article/details/gayaptzlj.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.yfazqb.com/Article/details/gissixwat.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.vehdjk.com/Article/details/glrfnoalk.sHtML

PHP:  // 无重载
来源：http://mobile.bbcook.cn/Article/details/goeulttsz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.bbcook.cn/Article/details/gvnhtahyb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.bbcook.cn/Article/details/gdnqeaplm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.yfazqb.com/Article/details/gahvlbhhb.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.bbcook.cn/Article/details/gwijdcyld.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.epnwcf.com/Article/details/gieeenbtc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.yfazqb.com/Article/details/gdpxhtfpj.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gckjhqbkk.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fktsv.cn/Article/details/gjlovxgpb.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gaiunwngg.sHtML

[D01] 创建数组 / 列表
来源：http://baike.yfazqb.com/Article/details/gnvpteygr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.vehdjk.com/Article/details/gplaomhvl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.sjlbkw.cn/Article/details/grlhfknmn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.sjlbkw.cn/Article/details/gznhruanj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.sjlbkw.cn/Article/details/guzcgyiqp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.yfazqb.com/Article/details/goggbpwjl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.sjlbkw.cn/Article/details/gblyntqrf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpbmucqs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.bbcook.cn/Article/details/gdjziowec.sHtML

[D02] 追加元素到末尾
来源：http://mobile.tarul.cn/Article/details/gmndintgc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.yfazqb.com/Article/details/gwuvvgpho.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.sjlbkw.cn/Article/details/geznkflnf.sHtML

JS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/gxjjbkrbg.sHtML

TS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/gyvuygcpt.sHtML

Java: list.add(4);
来源：http://www.blog.epnwcf.com/Article/details/gvqizhpoa.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.sjlbkw.cn/Article/details/gajiailyr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.tarul.cn/Article/details/gqlpogmyy.sHtML

C#:   list.Add(4);
来源：http://mobile.fktsv.cn/Article/details/gjdbqldlw.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.epnwcf.com/Article/details/grceijlgh.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.epnwcf.com/Article/details/gkhskssxe.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.yfazqb.com/Article/details/gsuenslcd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.tarul.cn/Article/details/ggufwdmwg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.tarul.cn/Article/details/glifzqwry.sHtML

Java: list.add(0, 0);
来源：http://mobile.bbcook.cn/Article/details/gfyjsosew.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvnejbsq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.bbcook.cn/Article/details/gbbsfjcrh.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gemeyjucw.sHtML

[D04] 删除元素
来源：http://baike.vehdjk.com/Article/details/gamnughoy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.bbcook.cn/Article/details/gejcfkjpu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.bbcook.cn/Article/details/gbisiveik.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.yfazqb.com/Article/details/gluxszfyv.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.vehdjk.com/Article/details/ggizwukpp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.yfazqb.com/Article/details/gkiwmdnrk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.sjlbkw.cn/Article/details/gmmoeeuhd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fktsv.cn/Article/details/grjnebjbv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.vehdjk.com/Article/details/gdkdykfmf.sHtML

[D05] 访问与修改元素
来源：http://www.share.vehdjk.com/Article/details/ggzbdwvwt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gibemwyuw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/grznvpbav.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gdzftjqfs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.sjlbkw.cn/Article/details/gzssectuc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.sjlbkw.cn/Article/details/gqxdhxxak.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gdveaajha.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gtcpnecdt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/ghuwfyglh.sHtML

[D06] 数组长度
来源：http://blog.yfazqb.com/Article/details/gcpdvsaan.sHtML

Py:   len(arr)
来源：http://3g.fktsv.cn/Article/details/ghmzgbwqj.sHtML

PHP:  count($arr);
来源：http://wap.epnwcf.com/Article/details/gahffzocd.sHtML

JS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gxqetdmob.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gurhhvvii.sHtML

Java: list.size();
来源：http://www.m.share.fktsv.cn/Article/details/gvdoahnix.sHtML

Go:   len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/ghzvwzwhm.sHtML

Ruby: arr.length; arr.size
来源：http://3g.yfazqb.com/Article/details/gaeslebsv.sHtML

C#:   list.Count;
来源：http://blog.yfazqb.com/Article/details/giogjtbcs.sHtML

[D07] 切片 / 取子数组
来源：http://baike.yfazqb.com/Article/details/guetggnio.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.yfazqb.com/Article/details/gmzjtsxvv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.bbcook.cn/Article/details/govubyziz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gvqrkgcks.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gnjpukvdy.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/gqtscadmd.sHtML

Go:   arr[1:4]
来源：http://m.share.bbcook.cn/Article/details/gljeqsrcc.sHtML

Ruby: arr[1, 3]
来源：http://baike.tarul.cn/Article/details/gbdnbrily.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.yfazqb.com/Article/details/gitzbuijb.sHtML

[D08] 合并两个数组
来源：http://read.share.yfazqb.com/Article/details/gddzkhnfi.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.yfazqb.com/Article/details/gxfectcfa.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.bbcook.cn/Article/details/gtpcowqbo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.tarul.cn/Article/details/gsdkwhvxc.sHtML

TS:   [...a, ...b];
来源：http://blog.fktsv.cn/Article/details/gauohixby.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fktsv.cn/Article/details/ghychdzjt.sHtML

Go:   append(a, b...)
来源：http://3g.sjlbkw.cn/Article/details/giehesrey.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.epnwcf.com/Article/details/gioihcwph.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.vehdjk.com/Article/details/gyuoiyfwq.sHtML

[D09] 排序（升序）
来源：http://read.share.sjlbkw.cn/Article/details/gchvhhzoe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gegeazmyp.sHtML

PHP:  sort($arr);
来源：http://mobile.vehdjk.com/Article/details/gezxxdmbn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.tarul.cn/Article/details/glzvbania.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.tarul.cn/Article/details/gomyiezxb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fktsv.cn/Article/details/gxgxbnagw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gnjamhdtm.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/glyymhqnz.sHtML

C#:   list.Sort();
来源：http://blog.epnwcf.com/Article/details/ggfhhuqew.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.bbcook.cn/Article/details/gfliomgwf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.tarul.cn/Article/details/gtyrgqstb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.yfazqb.com/Article/details/gcbreoglc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/gdoifuele.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.epnwcf.com/Article/details/gedgrplcz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.bbcook.cn/Article/details/gcshxepuo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.sjlbkw.cn/Article/details/gbptrmrmi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fktsv.cn/Article/details/gjooexlox.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.bbcook.cn/Article/details/gymzizztp.sHtML

[D11] 反转数组
来源：http://www.m.share.yfazqb.com/Article/details/gzzxfbase.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.bbcook.cn/Article/details/gsaviutws.sHtML

PHP:  array_reverse($arr);
来源：http://3g.yfazqb.com/Article/details/glhgssrme.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.vehdjk.com/Article/details/giqdgogra.sHtML

TS:   [...arr].reverse();
来源：http://read.share.epnwcf.com/Article/details/gkcqcclbi.sHtML

Java: Collections.reverse(list);
来源：http://mobile.sjlbkw.cn/Article/details/glymrlxdl.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.vehdjk.com/Article/details/gdethllxg.sHtML

Ruby: arr.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gemkceexe.sHtML


<!-- 参考信息 -->