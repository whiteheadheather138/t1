代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.sjlbkw.cn/Article/details/gzzaylryy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fktsv.cn/Article/details/gdzqkbuhr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.bbcook.cn/Article/details/gjsawtkzn.sHtML

[B12] 跳出多层循环
来源：http://www.blog.vehdjk.com/Article/details/gztgyskdh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fktsv.cn/Article/details/ghxjztiud.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.bbcook.cn/Article/details/gyhuuyiym.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gngzekcwn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gtnytvbgs.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gdkissjzx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.tarul.cn/Article/details/grllxffam.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.vehdjk.com/Article/details/guvblkzik.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.sjlbkw.cn/Article/details/glzvyvfgv.sHtML

[B13] 判断是否为数字
来源：http://www.share.vehdjk.com/Article/details/gzhmtplji.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.bbcook.cn/Article/details/gfmnxliof.sHtML

PHP:  is_numeric($x)
来源：http://baike.vehdjk.com/Article/details/gdqrgbvwa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fktsv.cn/Article/details/gnflucztc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/gcniqymcn.sHtML

Java: x instanceof Number
来源：http://mobile.fktsv.cn/Article/details/gniuikuzy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.sjlbkw.cn/Article/details/gdtakmhib.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.sjlbkw.cn/Article/details/gktzjepdv.sHtML

C#:   x is int or double or decimal
来源：http://read.share.bbcook.cn/Article/details/galgznyue.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.yfazqb.com/Article/details/gaixjgeiy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.tarul.cn/Article/details/gqnnfflke.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.epnwcf.com/Article/details/gjsrustre.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gtbbqbyvv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.bbcook.cn/Article/details/gdpdctdcg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.epnwcf.com/Article/details/gaundtrym.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.yfazqb.com/Article/details/gjpzzahsd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fktsv.cn/Article/details/gmvrxpdeq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.yfazqb.com/Article/details/gldxdxiaj.sHtML

[B15] 布尔运算与取反
来源：http://blog.bbcook.cn/Article/details/gofkutawp.sHtML

Py:   a and b or not c
来源：http://mobile.sjlbkw.cn/Article/details/gighuomcs.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.vehdjk.com/Article/details/ghckognnn.sHtML

JS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gegyklsio.sHtML

TS:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gpgpuyxye.sHtML

Java: a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gekaxzcpy.sHtML

Go:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gusdrizxg.sHtML

Ruby: a && b || !c
来源：http://wap.tarul.cn/Article/details/gqwkrcfhw.sHtML

C#:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gztyigigr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.sjlbkw.cn/Article/details/gwngxudfn.sHtML

Py:   if not data: return
来源：http://mobile.tarul.cn/Article/details/gnmwemqwj.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.bbcook.cn/Article/details/gcrwazdsy.sHtML

JS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/gbqwavsky.sHtML

TS:   if (!data) return;
来源：http://www.blog.tarul.cn/Article/details/ghoocapgs.sHtML

Java: if (data == null) return;
来源：http://www.blog.sjlbkw.cn/Article/details/gqirtiyis.sHtML

Go:   if data == nil { return }
来源：http://www.share.yfazqb.com/Article/details/gasueesiq.sHtML

Ruby: return if data.nil?
来源：http://mobile.vehdjk.com/Article/details/gtzxslpvo.sHtML

C#:   if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/ghilyaiai.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfibcbunx.sHtML

C. 函数与作用域
来源：http://read.share.sjlbkw.cn/Article/details/giaddrkjp.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwjqpjjgp.sHtML

[C01] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/grmmfnedr.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.tarul.cn/Article/details/gdvkhpkns.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gclpnrhgh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gqlspzmkn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gzmdqbgpm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gjwwpraur.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gmpnztrnn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.vehdjk.com/Article/details/gyevgpytn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gdxyaytqg.sHtML

[C02] 默认参数
来源：http://read.share.tarul.cn/Article/details/gummalylz.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.yfazqb.com/Article/details/gpmmglpny.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.epnwcf.com/Article/details/guctnuwxi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/gtkevwnky.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gnitxfuhu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.yfazqb.com/Article/details/gnzvhkxlh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fktsv.cn/Article/details/gynvilhnj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.sjlbkw.cn/Article/details/gtwdhmecv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.yfazqb.com/Article/details/gyhrilzar.sHtML

[C03] 可变参数
来源：http://baike.fktsv.cn/Article/details/ghatzckce.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.sjlbkw.cn/Article/details/gnlmrdyrg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.bbcook.cn/Article/details/gybyzioob.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/ggbyptajx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.epnwcf.com/Article/details/gaekceldt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.sjlbkw.cn/Article/details/gdnvhdimm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fktsv.cn/Article/details/gdkguidhu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.sjlbkw.cn/Article/details/ghsmmjput.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.vehdjk.com/Article/details/gmkfqxowk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.vehdjk.com/Article/details/giqumyjum.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsuwaujv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.epnwcf.com/Article/details/gkgiqnntn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/goinntzpg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.vehdjk.com/Article/details/gfkqulxul.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.sjlbkw.cn/Article/details/gtggoutax.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.epnwcf.com/Article/details/gaiorjada.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gefcdxawp.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gnjjlbwjf.sHtML

[C05] 返回多个值
来源：http://wap.bbcook.cn/Article/details/gyfuxxapn.sHtML

Py:   return a, b
来源：http://baike.yfazqb.com/Article/details/gzmkipzff.sHtML

PHP:  return [$a, $b];
来源：http://mobile.yfazqb.com/Article/details/gwsghtuzk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.sjlbkw.cn/Article/details/gpddpavwq.sHtML

TS:   return { a, b };
来源：http://baike.yfazqb.com/Article/details/gozgivmst.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.tarul.cn/Article/details/gcluyxyll.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gdksaiwch.sHtML

Ruby: return a, b
来源：http://read.share.tarul.cn/Article/details/gkifnlnpj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.tarul.cn/Article/details/gjifyylbx.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.yfazqb.com/Article/details/gpgktlvuh.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.tarul.cn/Article/details/gakszcdvg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.vehdjk.com/Article/details/gvjulxuts.sHtML

JS:   const square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gxzixjqax.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.epnwcf.com/Article/details/gllxxdmun.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.yfazqb.com/Article/details/gtcrqthgn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.vehdjk.com/Article/details/gbiwqdysp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fktsv.cn/Article/details/gvyiigbzk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/givewsvvd.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.epnwcf.com/Article/details/gvavkjteu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fktsv.cn/Article/details/gbszfatjy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fktsv.cn/Article/details/ghcsuabwg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.sjlbkw.cn/Article/details/gqnlgulkr.sHtML

TS:   arr.map(String)
来源：http://mobile.yfazqb.com/Article/details/gmcjhwiak.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.vehdjk.com/Article/details/gwiaerzwm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.bbcook.cn/Article/details/gyyypspnv.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.sjlbkw.cn/Article/details/gkvgxevxj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.yfazqb.com/Article/details/gwvlihlyr.sHtML

[C08] 闭包
来源：http://m.share.vehdjk.com/Article/details/guexmbaeu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.epnwcf.com/Article/details/gmqdsivib.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.vehdjk.com/Article/details/glliolfbp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gwgernflp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gyydnpizg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.epnwcf.com/Article/details/gutsdpynz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fktsv.cn/Article/details/gtbhtmpya.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.vehdjk.com/Article/details/grwnwzatt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gltxeetwx.sHtML

[C09] 递归
来源：http://blog.yfazqb.com/Article/details/gnjopsssk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.bbcook.cn/Article/details/glfodpwqx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.epnwcf.com/Article/details/gfudehmaf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/gjxsvafej.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gmcuatohy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fktsv.cn/Article/details/gezsnqmbd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.yfazqb.com/Article/details/gsiacggfn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.epnwcf.com/Article/details/gvyvnotep.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gtdeikytc.sHtML

[C10] 变量作用域
来源：http://mobile.yfazqb.com/Article/details/gapajzwdi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.sjlbkw.cn/Article/details/gkpegibce.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.yfazqb.com/Article/details/gduhhptdt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.sjlbkw.cn/Article/details/gurhekabf.sHtML

TS:   同 JS
来源：http://wap.vehdjk.com/Article/details/gfnarlufs.sHtML

Java: 方法内为块级作用域
来源：http://m.share.tarul.cn/Article/details/gtivkiahi.sHtML

Go:   花括号块级作用域
来源：http://read.share.bbcook.cn/Article/details/guhtfwath.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.sjlbkw.cn/Article/details/gacselurq.sHtML

C#:   块级作用域
来源：http://www.m.share.tarul.cn/Article/details/gysdzkxfp.sHtML

[C11] 模块导入与导出
来源：http://read.share.vehdjk.com/Article/details/gqxoijgpb.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/gynloqcuw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.bbcook.cn/Article/details/gexvcknap.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/gwyzuqodw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.yfazqb.com/Article/details/gzchumtag.sHtML

Java: import java.util.List;
来源：http://3g.fktsv.cn/Article/details/gramcwnsb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.yfazqb.com/Article/details/grdxmaagr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.epnwcf.com/Article/details/gexqhoquh.sHtML

C#:   using System.Text;
来源：http://m.share.sjlbkw.cn/Article/details/gwlqvnznp.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.tarul.cn/Article/details/gfmeawsvf.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.tarul.cn/Article/details/gmrohcxbf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.tarul.cn/Article/details/gmbbrxyvv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fktsv.cn/Article/details/gcxaezmlj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.tarul.cn/Article/details/gwygheucz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fktsv.cn/Article/details/gmbfwqrvs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.vehdjk.com/Article/details/gqxbyisiv.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.yfazqb.com/Article/details/grwfroolp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gflmxmbeq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fktsv.cn/Article/details/gapwucdte.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.sjlbkw.cn/Article/details/gxdgfzcne.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gxosdhlgv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.vehdjk.com/Article/details/gjwwlgmpd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gwwepnsfs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gyqphplll.sHtML

Go:   func add(a, b int) int
来源：http://wap.yfazqb.com/Article/details/gkpgrpqmx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.epnwcf.com/Article/details/gertewyzp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.yfazqb.com/Article/details/gdzevrvmj.sHtML

[C14] 泛型函数
来源：http://3g.bbcook.cn/Article/details/gaprjreey.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.epnwcf.com/Article/details/gdqpkyxwd.sHtML

PHP:  // 无泛型
来源：http://wap.vehdjk.com/Article/details/gfxxddsoe.sHtML

JS:   // 无泛型
来源：http://baike.fktsv.cn/Article/details/gbpndsfxb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.vehdjk.com/Article/details/gcksxerpx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaezyqvba.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fktsv.cn/Article/details/gjqrljsqp.sHtML

Ruby: # 无泛型
来源：http://m.share.tarul.cn/Article/details/gnsnmaodu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.yfazqb.com/Article/details/guroksgou.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.epnwcf.com/Article/details/gwmywckee.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.vehdjk.com/Article/details/gjujcoczj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.sjlbkw.cn/Article/details/gkictzizx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.tarul.cn/Article/details/gtndzyrdu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.epnwcf.com/Article/details/gtpyzhirm.sHtML

Java: // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/gvuhjkgew.sHtML

Go:   // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/gbbteosff.sHtML

Ruby: a, b = pair
来源：http://mobile.sjlbkw.cn/Article/details/gzgbjcrow.sHtML

C#:   var (a, b) = pair;
来源：http://blog.tarul.cn/Article/details/gtwqlgtik.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.bbcook.cn/Article/details/gahekfzvy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.sjlbkw.cn/Article/details/gobpyttyo.sHtML

PHP:  // 无重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdwtowkn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.bbcook.cn/Article/details/gspkajbog.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fktsv.cn/Article/details/gxwttqfpd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.epnwcf.com/Article/details/gxalzwbsg.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.tarul.cn/Article/details/gqvmxdwzm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.epnwcf.com/Article/details/ggdwstxkn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.bbcook.cn/Article/details/ghqzwoghe.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gkqujbgiq.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.bbcook.cn/Article/details/gnmktayiq.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gogsaqdqi.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.bbcook.cn/Article/details/gsrndwjgo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.vehdjk.com/Article/details/gskrgstlc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.tarul.cn/Article/details/gqbosauft.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.epnwcf.com/Article/details/gksrhqwdi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.bbcook.cn/Article/details/grycitvjs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.yfazqb.com/Article/details/gnyqtfrae.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.bbcook.cn/Article/details/gjvvmjuam.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gothqzjhv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.epnwcf.com/Article/details/gvbftnwct.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fktsv.cn/Article/details/gbxfzfpuw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.vehdjk.com/Article/details/gweudzgqe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.bbcook.cn/Article/details/gmvivvyex.sHtML

JS:   arr.push(4);
来源：http://blog.sjlbkw.cn/Article/details/gneutewwi.sHtML

TS:   arr.push(4);
来源：http://blog.fktsv.cn/Article/details/gnjowvbsf.sHtML

Java: list.add(4);
来源：http://mobile.fktsv.cn/Article/details/gcvzjpuam.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gvjjjzidf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.sjlbkw.cn/Article/details/gksfgpohp.sHtML

C#:   list.Add(4);
来源：http://www.share.tarul.cn/Article/details/gpdaorqdg.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.tarul.cn/Article/details/gadbhkyve.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gqvrppqqp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.vehdjk.com/Article/details/gswstdoqq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.yfazqb.com/Article/details/gngqbqdqk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.vehdjk.com/Article/details/gygxgnzlg.sHtML

Java: list.add(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gluhiehqu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.tarul.cn/Article/details/gbaoyjjie.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.yfazqb.com/Article/details/gkdthckki.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.epnwcf.com/Article/details/gmlhqymmy.sHtML

[D04] 删除元素
来源：http://m.share.fktsv.cn/Article/details/goedvtrij.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.yfazqb.com/Article/details/glnjxdsbg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.bbcook.cn/Article/details/gbyslverb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.tarul.cn/Article/details/gybkvomzx.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/gjnnmlrdi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.vehdjk.com/Article/details/gnhtdxvfc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.vehdjk.com/Article/details/gqayuxcly.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.bbcook.cn/Article/details/gstqxwapf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.epnwcf.com/Article/details/gtfnpwdao.sHtML

[D05] 访问与修改元素
来源：http://3g.bbcook.cn/Article/details/gwulakjfk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gsabltqyv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.epnwcf.com/Article/details/gpkvarzsz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gvdibljnv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.vehdjk.com/Article/details/gpdqzvpxz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.yfazqb.com/Article/details/gdvvcatng.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gozmfadqu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gnywldvxa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gadepghld.sHtML

[D06] 数组长度
来源：http://blog.bbcook.cn/Article/details/gfqsoxtbb.sHtML

Py:   len(arr)
来源：http://m.share.tarul.cn/Article/details/gdktvafjl.sHtML

PHP:  count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/geugcgpad.sHtML

JS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/gxujkfjhi.sHtML

TS:   arr.length
来源：http://read.share.tarul.cn/Article/details/gljduouvd.sHtML

Java: list.size();
来源：http://m.share.epnwcf.com/Article/details/ggitvrcug.sHtML

Go:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/ganpvpyyk.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.epnwcf.com/Article/details/gdkmhcbam.sHtML

C#:   list.Count;
来源：http://baike.sjlbkw.cn/Article/details/gknemxaka.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.yfazqb.com/Article/details/gssxwswrr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.yfazqb.com/Article/details/gvcjheezk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.sjlbkw.cn/Article/details/gomzmxvxa.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.bbcook.cn/Article/details/gxarpjysc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/gbgxpybpy.sHtML

Java: list.subList(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gfaoyqywy.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fktsv.cn/Article/details/gaojdpbiz.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.epnwcf.com/Article/details/ggztfqkqk.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.sjlbkw.cn/Article/details/gwyyfihcb.sHtML

[D08] 合并两个数组
来源：http://www.m.share.epnwcf.com/Article/details/gafifzbfa.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.tarul.cn/Article/details/gqybmgaut.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.yfazqb.com/Article/details/guwwtcqqu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.epnwcf.com/Article/details/gxpnumtog.sHtML

TS:   [...a, ...b];
来源：http://read.share.epnwcf.com/Article/details/givzirwgt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.yfazqb.com/Article/details/gyboolndl.sHtML

Go:   append(a, b...)
来源：http://read.share.sjlbkw.cn/Article/details/gmpvzzlcz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.yfazqb.com/Article/details/gxeujwmtj.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.bbcook.cn/Article/details/gcqmgmrzd.sHtML

[D09] 排序（升序）
来源：http://3g.fktsv.cn/Article/details/glkjnjzfo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/grszhmsaq.sHtML

PHP:  sort($arr);
来源：http://3g.epnwcf.com/Article/details/gfagqiehe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.vehdjk.com/Article/details/gvqulidsy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.sjlbkw.cn/Article/details/gqconkwix.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.yfazqb.com/Article/details/gpoxozyem.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/giupkdkkk.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/givytqkkc.sHtML

C#:   list.Sort();
来源：http://3g.sjlbkw.cn/Article/details/gshxafdoq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fktsv.cn/Article/details/ggdyoytwj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.sjlbkw.cn/Article/details/gdyhwxoms.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/gadhvnqil.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/ggzjmxhsd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/gmqgxpzql.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.yfazqb.com/Article/details/gpsgzboca.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.tarul.cn/Article/details/gjmiwscql.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.yfazqb.com/Article/details/gxmmenadd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fktsv.cn/Article/details/gysfhyvfl.sHtML

[D11] 反转数组
来源：http://baike.fktsv.cn/Article/details/gdotwgvhk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.tarul.cn/Article/details/goptghkju.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.sjlbkw.cn/Article/details/ghfgvhfej.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.bbcook.cn/Article/details/gsymvntnr.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.sjlbkw.cn/Article/details/gsryopget.sHtML

Java: Collections.reverse(list);
来源：http://m.share.yfazqb.com/Article/details/gukmwtmid.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.tarul.cn/Article/details/gohcgacuj.sHtML

Ruby: arr.reverse
来源：http://www.m.share.tarul.cn/Article/details/grbbrzyes.sHtML

C#:   list.Reverse();
来源：http://baike.bbcook.cn/Article/details/gjuupmthq.sHtML

[D12] 查找元素下标
来源：http://wap.bbcook.cn/Article/details/gmbtaydwh.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.epnwcf.com/Article/details/gpmcdnblj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.vehdjk.com/Article/details/ggilzljjh.sHtML


<!-- 参考信息 -->