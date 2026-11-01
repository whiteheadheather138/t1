代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.vehdjk.com/Article/details/gocgeydrs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.yfazqb.com/Article/details/gfcmktonc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.sjlbkw.cn/Article/details/gkhzcpqka.sHtML

[B12] 跳出多层循环
来源：http://blog.tarul.cn/Article/details/ginhlgnmn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.tarul.cn/Article/details/gmjgfwhyi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.vehdjk.com/Article/details/gfgykgeay.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gsrjngfit.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gffcotsdw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.tarul.cn/Article/details/gelracycl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.vehdjk.com/Article/details/gpretomma.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwyurure.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.sjlbkw.cn/Article/details/gtfkelqwq.sHtML

[B13] 判断是否为数字
来源：http://3g.sjlbkw.cn/Article/details/gsotpougf.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.tarul.cn/Article/details/ggcbritsg.sHtML

PHP:  is_numeric($x)
来源：http://3g.yfazqb.com/Article/details/glaoaadjq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.sjlbkw.cn/Article/details/gphhzamad.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/gyjhdpmgx.sHtML

Java: x instanceof Number
来源：http://blog.fktsv.cn/Article/details/gcgxrilah.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.sjlbkw.cn/Article/details/gkgvvbbtu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fktsv.cn/Article/details/gztfqoyhl.sHtML

C#:   x is int or double or decimal
来源：http://wap.vehdjk.com/Article/details/gbyajyzps.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.bbcook.cn/Article/details/gclphvunx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fktsv.cn/Article/details/ggbcjgkes.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.sjlbkw.cn/Article/details/gyxsupbsu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.bbcook.cn/Article/details/ghzfxrbfh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.bbcook.cn/Article/details/glllrwfhw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gqpzkmmpg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.vehdjk.com/Article/details/gfubzpujd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.yfazqb.com/Article/details/gqdvtruda.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.tarul.cn/Article/details/gfuatlwng.sHtML

[B15] 布尔运算与取反
来源：http://3g.yfazqb.com/Article/details/gdcqznluv.sHtML

Py:   a and b or not c
来源：http://mobile.bbcook.cn/Article/details/grriaozln.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.vehdjk.com/Article/details/ggasmjunb.sHtML

JS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gsbcjzszn.sHtML

TS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gmejdbuju.sHtML

Java: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gqjenlchf.sHtML

Go:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gzbxbxvxt.sHtML

Ruby: a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gpjssyyot.sHtML

C#:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gdizagvje.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.sjlbkw.cn/Article/details/gmdycsyel.sHtML

Py:   if not data: return
来源：http://www.m.share.epnwcf.com/Article/details/gtbguzbne.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.yfazqb.com/Article/details/gbrfaiioo.sHtML

JS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/gspafwbtn.sHtML

TS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/gcaaqtqef.sHtML

Java: if (data == null) return;
来源：http://www.share.vehdjk.com/Article/details/gtcoozjuh.sHtML

Go:   if data == nil { return }
来源：http://mobile.tarul.cn/Article/details/glfofgnur.sHtML

Ruby: return if data.nil?
来源：http://mobile.sjlbkw.cn/Article/details/guseevyys.sHtML

C#:   if (data == null) return;
来源：http://www.blog.vehdjk.com/Article/details/gpnaaycjh.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gmlanrbmm.sHtML

C. 函数与作用域
来源：http://3g.sjlbkw.cn/Article/details/gpsztdggt.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grjuftwqz.sHtML

[C01] 定义函数
来源：http://read.share.bbcook.cn/Article/details/glmtkxxxh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.tarul.cn/Article/details/gumjaaybg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gkutscslu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gmdgrljwt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gzczqzjjw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gqeixspux.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.epnwcf.com/Article/details/gbfjspyox.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.sjlbkw.cn/Article/details/gbxnyuaqo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gcwlmjfrd.sHtML

[C02] 默认参数
来源：http://m.share.yfazqb.com/Article/details/gwizicjru.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.bbcook.cn/Article/details/gbtmgnmov.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.epnwcf.com/Article/details/gprfudbnv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.tarul.cn/Article/details/ghkkfljrs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.sjlbkw.cn/Article/details/ghqncasky.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.vehdjk.com/Article/details/guynwziyr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fktsv.cn/Article/details/gjbwhleas.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.bbcook.cn/Article/details/gfifsezko.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.tarul.cn/Article/details/gafsfkbnd.sHtML

[C03] 可变参数
来源：http://www.m.share.bbcook.cn/Article/details/gixrxmseh.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.epnwcf.com/Article/details/glcmwappt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fktsv.cn/Article/details/gataextww.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gvmantyqa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/gqjkuadll.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.tarul.cn/Article/details/gvhoaxjuy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.bbcook.cn/Article/details/gutobamcw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.epnwcf.com/Article/details/gtlxsehih.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.bbcook.cn/Article/details/gncupgryp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fktsv.cn/Article/details/gwkwqnxms.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.bbcook.cn/Article/details/ghwjcahbp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.vehdjk.com/Article/details/gcgjcwdvv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/gkhomkuhh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.yfazqb.com/Article/details/ghjxcmtld.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.bbcook.cn/Article/details/gonzzzmev.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.tarul.cn/Article/details/gwpuunfpu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/gbowfxtrd.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/gckxblxzu.sHtML

[C05] 返回多个值
来源：http://read.share.tarul.cn/Article/details/gdrgrjwsn.sHtML

Py:   return a, b
来源：http://blog.tarul.cn/Article/details/gmgojanpu.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.bbcook.cn/Article/details/gptjqcwbz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gycqbkctn.sHtML

TS:   return { a, b };
来源：http://3g.fktsv.cn/Article/details/gwppfwnxw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.yfazqb.com/Article/details/gfclzczxk.sHtML

Go:   return a, b
来源：http://mobile.bbcook.cn/Article/details/gdouzdzzd.sHtML

Ruby: return a, b
来源：http://m.share.bbcook.cn/Article/details/gfjjlqlkf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.yfazqb.com/Article/details/gtgzljmyg.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.vehdjk.com/Article/details/gzpakdvvj.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.tarul.cn/Article/details/grcafhpkf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.yfazqb.com/Article/details/gyqlhzxwn.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gkvpmbggh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gnrwbssqu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.tarul.cn/Article/details/gjzjtffig.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.bbcook.cn/Article/details/gndcjbcgo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.epnwcf.com/Article/details/gxhnykjbr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gcrjmfoxy.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.sjlbkw.cn/Article/details/grozdevnn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.yfazqb.com/Article/details/getwlsmbf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.tarul.cn/Article/details/gttyeegoq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.bbcook.cn/Article/details/ggusqcczy.sHtML

TS:   arr.map(String)
来源：http://www.share.bbcook.cn/Article/details/grnswqjxx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.vehdjk.com/Article/details/gnqlntszj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.tarul.cn/Article/details/gzjdutmcp.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fktsv.cn/Article/details/gxghsmggq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.epnwcf.com/Article/details/gyrduzvce.sHtML

[C08] 闭包
来源：http://wap.tarul.cn/Article/details/grcvakkno.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.bbcook.cn/Article/details/gtfatfcpr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.epnwcf.com/Article/details/gwhcgkfkf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.bbcook.cn/Article/details/gjjlvsxgz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gyrsgxxwc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fktsv.cn/Article/details/gsmpmmrfp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fktsv.cn/Article/details/gvxeuelfv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fktsv.cn/Article/details/gndmnwgam.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/guovcmjnt.sHtML

[C09] 递归
来源：http://www.blog.sjlbkw.cn/Article/details/gvvfrajfs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.sjlbkw.cn/Article/details/gdaxtqvsx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.tarul.cn/Article/details/ghgmemnnv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.tarul.cn/Article/details/gzuexsnqg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gkeutsumx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/galmlwovk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fktsv.cn/Article/details/gyyopcozk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fktsv.cn/Article/details/gxxwsnyku.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.sjlbkw.cn/Article/details/gnxnaaqda.sHtML

[C10] 变量作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gkjimhidj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.epnwcf.com/Article/details/gbjohhbmk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.vehdjk.com/Article/details/gzyzqwcmy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.bbcook.cn/Article/details/glrxlgyrm.sHtML

TS:   同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gamrfohdd.sHtML

Java: 方法内为块级作用域
来源：http://3g.yfazqb.com/Article/details/gmojkpcio.sHtML

Go:   花括号块级作用域
来源：http://blog.vehdjk.com/Article/details/geqifffcc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.yfazqb.com/Article/details/gomslxocq.sHtML

C#:   块级作用域
来源：http://m.share.fktsv.cn/Article/details/gkfcppctn.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.vehdjk.com/Article/details/glbgswvzf.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/gknbsjcac.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.vehdjk.com/Article/details/gujomyrfd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.vehdjk.com/Article/details/gmuskfces.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fktsv.cn/Article/details/gmfoqvlys.sHtML

Java: import java.util.List;
来源：http://www.blog.yfazqb.com/Article/details/gygvlvxoy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.bbcook.cn/Article/details/gjeqsikhi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.tarul.cn/Article/details/gkuyyoehv.sHtML

C#:   using System.Text;
来源：http://www.m.share.bbcook.cn/Article/details/gfmxbgnwo.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.bbcook.cn/Article/details/gxvfyisnw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.bbcook.cn/Article/details/gymprtkbr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.vehdjk.com/Article/details/gfbtdqgbc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.tarul.cn/Article/details/gzxmcgajy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gycbdzorj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.tarul.cn/Article/details/ghyongefu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.tarul.cn/Article/details/govrjuykd.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.yfazqb.com/Article/details/guyrjlknb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gpvhilzlk.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.epnwcf.com/Article/details/gtjgplqjw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.tarul.cn/Article/details/glmcsqgdo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/guqdvcdvr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fktsv.cn/Article/details/gvjqshwdt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gxfhsndei.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gndtmdxen.sHtML

Go:   func add(a, b int) int
来源：http://wap.yfazqb.com/Article/details/gygubiabv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.tarul.cn/Article/details/goklzkoeg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.tarul.cn/Article/details/gcfvnpdos.sHtML

[C14] 泛型函数
来源：http://www.blog.sjlbkw.cn/Article/details/giwutgtlr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.vehdjk.com/Article/details/gmnypfjqh.sHtML

PHP:  // 无泛型
来源：http://www.share.yfazqb.com/Article/details/gcxwrmlcd.sHtML

JS:   // 无泛型
来源：http://mobile.epnwcf.com/Article/details/guracplrv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.epnwcf.com/Article/details/gcgxahcij.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.yfazqb.com/Article/details/gjqyaoloq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.bbcook.cn/Article/details/gsdbrduzm.sHtML

Ruby: # 无泛型
来源：http://m.share.bbcook.cn/Article/details/gjaetyfgr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fktsv.cn/Article/details/gycntxcpz.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.yfazqb.com/Article/details/gnusprtns.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.tarul.cn/Article/details/gjngvpdma.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fktsv.cn/Article/details/gabidhyws.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/ggmxkkvpc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fktsv.cn/Article/details/gtlmcpycz.sHtML

Java: // 无解构
来源：http://baike.vehdjk.com/Article/details/gxrqldqif.sHtML

Go:   // 无解构
来源：http://baike.fktsv.cn/Article/details/gayiwmgau.sHtML

Ruby: a, b = pair
来源：http://3g.bbcook.cn/Article/details/geojwlmnp.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.yfazqb.com/Article/details/gkjkrxfvf.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.tarul.cn/Article/details/gpfllhurg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fktsv.cn/Article/details/gktatwxfq.sHtML

PHP:  // 无重载
来源：http://baike.fktsv.cn/Article/details/giluitgnu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.tarul.cn/Article/details/gbjwpsija.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.yfazqb.com/Article/details/gkucfxnbn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.epnwcf.com/Article/details/ghbetpnox.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.vehdjk.com/Article/details/gsygosfrd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fktsv.cn/Article/details/gklvzldyt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.bbcook.cn/Article/details/gopzsqwyo.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gcrbmxbdu.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.vehdjk.com/Article/details/gbhvbfpbl.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gejbbxzht.sHtML

[D01] 创建数组 / 列表
来源：http://baike.epnwcf.com/Article/details/giooyfnbf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fktsv.cn/Article/details/grubxsjds.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fktsv.cn/Article/details/gpqtsgokw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/gmwvahyeh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.yfazqb.com/Article/details/gyibedqzs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.vehdjk.com/Article/details/gysuovwag.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzdlnglb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.bbcook.cn/Article/details/gwevymafm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.bbcook.cn/Article/details/gjkhmsgqj.sHtML

[D02] 追加元素到末尾
来源：http://www.share.bbcook.cn/Article/details/gqvnynlwj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.yfazqb.com/Article/details/gqjjzrbwd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.sjlbkw.cn/Article/details/gdnzugkyf.sHtML

JS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gjpnwbifu.sHtML

TS:   arr.push(4);
来源：http://read.share.yfazqb.com/Article/details/gkxrjxbog.sHtML

Java: list.add(4);
来源：http://baike.vehdjk.com/Article/details/gmmfqsyyz.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gvtmkcyqz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.bbcook.cn/Article/details/gfuasgixb.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fktsv.cn/Article/details/gytnrxfor.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.bbcook.cn/Article/details/gmvpatuyo.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fktsv.cn/Article/details/gdkqkkivm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.yfazqb.com/Article/details/gjjpimanq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fktsv.cn/Article/details/gmfmfusky.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.tarul.cn/Article/details/gljlulzcg.sHtML

Java: list.add(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gdosltkbt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.epnwcf.com/Article/details/gmuaaimaq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.yfazqb.com/Article/details/gorwxdzlv.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.bbcook.cn/Article/details/gdycopiqf.sHtML

[D04] 删除元素
来源：http://www.share.tarul.cn/Article/details/gyytttjnq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fktsv.cn/Article/details/gwfbqnkeq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.sjlbkw.cn/Article/details/gymknvyhc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.epnwcf.com/Article/details/gylavqnye.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.sjlbkw.cn/Article/details/graxhcfeh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fktsv.cn/Article/details/gupdspuii.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.yfazqb.com/Article/details/goexbiqot.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.yfazqb.com/Article/details/gxzwrzopa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.vehdjk.com/Article/details/gzcaoxwhe.sHtML

[D05] 访问与修改元素
来源：http://www.share.sjlbkw.cn/Article/details/gtkjlicpb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/grxyjuubm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gfroqudvh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gjijepbpn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.sjlbkw.cn/Article/details/gfyndamkg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.epnwcf.com/Article/details/gcmppexlz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gvvnapxcy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.yfazqb.com/Article/details/giphmqarl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/grnqzkapp.sHtML

[D06] 数组长度
来源：http://www.share.fktsv.cn/Article/details/gaheampys.sHtML

Py:   len(arr)
来源：http://baike.yfazqb.com/Article/details/gzjbuvoao.sHtML

PHP:  count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/glqrzkpcz.sHtML

JS:   arr.length
来源：http://www.blog.fktsv.cn/Article/details/gnowlohii.sHtML

TS:   arr.length
来源：http://blog.fktsv.cn/Article/details/gmigspktq.sHtML

Java: list.size();
来源：http://www.m.share.yfazqb.com/Article/details/gwqsasbza.sHtML

Go:   len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gknlicixi.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/gaprsgoep.sHtML

C#:   list.Count;
来源：http://www.blog.bbcook.cn/Article/details/gfsqfziov.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.vehdjk.com/Article/details/gnuoqbhar.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fktsv.cn/Article/details/gnicyrukx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.bbcook.cn/Article/details/gxqeqpvao.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/gkefulaeo.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/gnbbusgwx.sHtML

Java: list.subList(1, 4);
来源：http://blog.bbcook.cn/Article/details/gmuojrnax.sHtML

Go:   arr[1:4]
来源：http://3g.yfazqb.com/Article/details/ghhqnipbq.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fktsv.cn/Article/details/gbzevaiax.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.epnwcf.com/Article/details/ggwoshiso.sHtML

[D08] 合并两个数组
来源：http://3g.fktsv.cn/Article/details/gyydmltnj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.yfazqb.com/Article/details/gfertghoz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.vehdjk.com/Article/details/ghczbvcal.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.vehdjk.com/Article/details/gebtgeaoz.sHtML

TS:   [...a, ...b];
来源：http://baike.tarul.cn/Article/details/gxmmkjowm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqmimvzm.sHtML

Go:   append(a, b...)
来源：http://wap.tarul.cn/Article/details/gorhgeqim.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fktsv.cn/Article/details/gcvylvrgb.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.bbcook.cn/Article/details/ggjpammhs.sHtML

[D09] 排序（升序）
来源：http://read.share.sjlbkw.cn/Article/details/gafuvqrca.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gonkqocak.sHtML

PHP:  sort($arr);
来源：http://baike.sjlbkw.cn/Article/details/gxvyijbmx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fktsv.cn/Article/details/genuiamax.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.vehdjk.com/Article/details/gfchlqrnh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.tarul.cn/Article/details/gxxsetlre.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fktsv.cn/Article/details/gwkvwhcxl.sHtML

Ruby: arr.sort
来源：http://blog.vehdjk.com/Article/details/gcsmwcfim.sHtML

C#:   list.Sort();
来源：http://www.m.share.yfazqb.com/Article/details/gkwmxrxqv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.yfazqb.com/Article/details/gufzmleei.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.epnwcf.com/Article/details/gnlfyiagd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.tarul.cn/Article/details/gffjimqol.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/gpdgoojyo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.bbcook.cn/Article/details/gzkzflisf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.sjlbkw.cn/Article/details/gjurtuloe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.tarul.cn/Article/details/gwgnyqixh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.bbcook.cn/Article/details/goqpbhiya.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.epnwcf.com/Article/details/gtgiodiwe.sHtML

[D11] 反转数组
来源：http://m.share.fktsv.cn/Article/details/gnqjajhvb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.vehdjk.com/Article/details/gwxnnmacw.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gjkjddbca.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.tarul.cn/Article/details/gpuugvosc.sHtML

TS:   [...arr].reverse();
来源：http://wap.yfazqb.com/Article/details/glaoecmpc.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fktsv.cn/Article/details/guszchqjn.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.tarul.cn/Article/details/gjtjavhqc.sHtML

Ruby: arr.reverse
来源：http://wap.yfazqb.com/Article/details/gutgmagwq.sHtML

C#:   list.Reverse();
来源：http://read.share.yfazqb.com/Article/details/gfzrsxrzu.sHtML

[D12] 查找元素下标
来源：http://wap.epnwcf.com/Article/details/graytkzdm.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.yfazqb.com/Article/details/gywgfidfd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gusssmspx.sHtML


<!-- 参考信息 -->