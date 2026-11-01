代发 wailian999

PHP:  range(0, 10, 2);
来源：http://mobile.fktsv.cn/Article/details/ggaxklhua.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.sjlbkw.cn/Article/details/gpjqmqcob.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fktsv.cn/Article/details/gomxpjqko.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.yfazqb.com/Article/details/gdhvwsgbl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.epnwcf.com/Article/details/gevmcwfhi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.tarul.cn/Article/details/gwsoxerrn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.epnwcf.com/Article/details/gmhcmbvqc.sHtML

[B12] 跳出多层循环
来源：http://3g.fktsv.cn/Article/details/gcaoeizjb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.yfazqb.com/Article/details/gbwwbvekg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.bbcook.cn/Article/details/gzjshyelc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gsemysqbb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gwrjpfzag.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gdreuyauc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.bbcook.cn/Article/details/gekfjwxfr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.sjlbkw.cn/Article/details/gxhkbwnbn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.tarul.cn/Article/details/gpdnfuhbf.sHtML

[B13] 判断是否为数字
来源：http://wap.bbcook.cn/Article/details/gialumnkw.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.bbcook.cn/Article/details/gnefjycgg.sHtML

PHP:  is_numeric($x)
来源：http://m.share.sjlbkw.cn/Article/details/giviiinqg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.vehdjk.com/Article/details/glwjoytjf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.sjlbkw.cn/Article/details/gzftuoyyf.sHtML

Java: x instanceof Number
来源：http://blog.yfazqb.com/Article/details/gfdoyohxc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.yfazqb.com/Article/details/gztphcsmp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.tarul.cn/Article/details/gyxzuxuas.sHtML

C#:   x is int or double or decimal
来源：http://baike.tarul.cn/Article/details/goxajohgh.sHtML

[B14] 判断值是否在集合内
来源：http://baike.tarul.cn/Article/details/gtepglycj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.vehdjk.com/Article/details/grbcpmnjz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.bbcook.cn/Article/details/gwsrvkdfd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.yfazqb.com/Article/details/gzipjkgml.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gyusdlfcn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fktsv.cn/Article/details/gslohcpcz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.bbcook.cn/Article/details/gidfiqwnc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.vehdjk.com/Article/details/ggmlbfwwa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.vehdjk.com/Article/details/gmsurwikl.sHtML

[B15] 布尔运算与取反
来源：http://baike.sjlbkw.cn/Article/details/gimxowqbx.sHtML

Py:   a and b or not c
来源：http://3g.sjlbkw.cn/Article/details/gjkeqbhar.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.epnwcf.com/Article/details/gxjnlifnt.sHtML

JS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/ggdjpzzqc.sHtML

TS:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gluehzkwx.sHtML

Java: a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gxmqnycue.sHtML

Go:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/guiblzalv.sHtML

Ruby: a && b || !c
来源：http://blog.bbcook.cn/Article/details/gxbqnapua.sHtML

C#:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gmyvymcfc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.vehdjk.com/Article/details/galgsurcw.sHtML

Py:   if not data: return
来源：http://m.share.fktsv.cn/Article/details/goubteemi.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.sjlbkw.cn/Article/details/gpzgqwezq.sHtML

JS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gdfwdrvqp.sHtML

TS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/gvxxfwfkz.sHtML

Java: if (data == null) return;
来源：http://wap.fktsv.cn/Article/details/gdlxqqsng.sHtML

Go:   if data == nil { return }
来源：http://www.share.bbcook.cn/Article/details/gbnibozvt.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.vehdjk.com/Article/details/ghlqstifp.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/gdsiyxghc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/giuqnfthy.sHtML

C. 函数与作用域
来源：http://blog.vehdjk.com/Article/details/geejibwag.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ghdrkfmfz.sHtML

[C01] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/gvpmmkmts.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.vehdjk.com/Article/details/ghrwwvete.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/ggcilcuta.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gsedntipn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/ghoxrlljg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gvktbjktr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.epnwcf.com/Article/details/gzbccfidr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.epnwcf.com/Article/details/gxyddtdxi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gyymhcbng.sHtML

[C02] 默认参数
来源：http://blog.yfazqb.com/Article/details/gtjhxhvwc.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.yfazqb.com/Article/details/geaovqwdl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fktsv.cn/Article/details/gzwipvime.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.vehdjk.com/Article/details/gzzazntul.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/grngejrmd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.yfazqb.com/Article/details/gerrxcjxl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.vehdjk.com/Article/details/gcvcavtkq.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.vehdjk.com/Article/details/gvvtdprmx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwikxvswr.sHtML

[C03] 可变参数
来源：http://read.share.vehdjk.com/Article/details/gpejyusin.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.vehdjk.com/Article/details/gyvjnuznr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.tarul.cn/Article/details/grbkvpkdc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.yfazqb.com/Article/details/gfcudgqil.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.bbcook.cn/Article/details/geykfgmhb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fktsv.cn/Article/details/gkvapfptr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.sjlbkw.cn/Article/details/gzctijtpg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.bbcook.cn/Article/details/gajelksyx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.bbcook.cn/Article/details/groyqtkxy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.tarul.cn/Article/details/grimyssvc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbhhzwfx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.epnwcf.com/Article/details/gfpoiebyp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/goxvzzhrn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fktsv.cn/Article/details/gttfvwhhj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.yfazqb.com/Article/details/gofoovnhu.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.bbcook.cn/Article/details/ggrozsudv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gkekrgdlp.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/gbofqlyxf.sHtML

[C05] 返回多个值
来源：http://3g.epnwcf.com/Article/details/gnqbbysdu.sHtML

Py:   return a, b
来源：http://baike.bbcook.cn/Article/details/gqfbszfqv.sHtML

PHP:  return [$a, $b];
来源：http://blog.tarul.cn/Article/details/gjkbtmcad.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gjpdlzvvu.sHtML

TS:   return { a, b };
来源：http://m.share.bbcook.cn/Article/details/gugnffycp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.bbcook.cn/Article/details/gtujstbjb.sHtML

Go:   return a, b
来源：http://baike.fktsv.cn/Article/details/gluflrlrt.sHtML

Ruby: return a, b
来源：http://www.share.bbcook.cn/Article/details/grlqeceki.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.vehdjk.com/Article/details/gusxnnvcf.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.yfazqb.com/Article/details/gytpfuqcw.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.epnwcf.com/Article/details/gstbvqpkq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.tarul.cn/Article/details/guivzrvnw.sHtML

JS:   const square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/gtfdqqvtk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.bbcook.cn/Article/details/gxjtjugob.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.tarul.cn/Article/details/gafyrdhqa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.vehdjk.com/Article/details/ghoocwfhx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.sjlbkw.cn/Article/details/gtknjqvqg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gnmlywpub.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.tarul.cn/Article/details/goyprykbo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.vehdjk.com/Article/details/gttbxricr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.vehdjk.com/Article/details/ggumzmgxn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.yfazqb.com/Article/details/gjvwywitg.sHtML

TS:   arr.map(String)
来源：http://www.share.vehdjk.com/Article/details/gyekbynem.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/gclznneos.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fktsv.cn/Article/details/grwtegdww.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fktsv.cn/Article/details/guezwkbhs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.epnwcf.com/Article/details/gequjkkfs.sHtML

[C08] 闭包
来源：http://mobile.epnwcf.com/Article/details/gwtdpikfz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fktsv.cn/Article/details/gedenuzzc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fktsv.cn/Article/details/gazqddkud.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gidsquzcu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/gjauuqrry.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.vehdjk.com/Article/details/gayakceeo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.yfazqb.com/Article/details/gymhpmoko.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.bbcook.cn/Article/details/gakcaukvr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gvdbmhkbl.sHtML

[C09] 递归
来源：http://blog.sjlbkw.cn/Article/details/gnhggewvw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fktsv.cn/Article/details/grkjcnzmp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.yfazqb.com/Article/details/gdauxyemc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/gxldsfxqw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/gjqicprqx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.tarul.cn/Article/details/gfvakycuu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.yfazqb.com/Article/details/glnvjovei.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.bbcook.cn/Article/details/giawpmhyl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fktsv.cn/Article/details/geliivgav.sHtML

[C10] 变量作用域
来源：http://m.share.epnwcf.com/Article/details/gtvzopfkg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.vehdjk.com/Article/details/godlajkfz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fktsv.cn/Article/details/gvxfpviyf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.yfazqb.com/Article/details/gejavdvqt.sHtML

TS:   同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gngyxkvhj.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.tarul.cn/Article/details/gtgzacqep.sHtML

Go:   花括号块级作用域
来源：http://www.share.fktsv.cn/Article/details/gkivganpl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.vehdjk.com/Article/details/gyqsiselo.sHtML

C#:   块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gaadbbjmx.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.yfazqb.com/Article/details/gmlhkdrrb.sHtML

Py:   from module import func
来源：http://www.blog.vehdjk.com/Article/details/gypeobjwz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.epnwcf.com/Article/details/gldxcspbl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.yfazqb.com/Article/details/gdrptyphi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.yfazqb.com/Article/details/gyqbkiaec.sHtML

Java: import java.util.List;
来源：http://m.share.yfazqb.com/Article/details/ghmanzzaz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.sjlbkw.cn/Article/details/gutnzbcsp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.yfazqb.com/Article/details/gdhskphfh.sHtML

C#:   using System.Text;
来源：http://mobile.yfazqb.com/Article/details/glslsowpf.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.yfazqb.com/Article/details/grfgzlvwf.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.tarul.cn/Article/details/gmspytexx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.yfazqb.com/Article/details/golesoywl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.vehdjk.com/Article/details/gbolrjyat.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.yfazqb.com/Article/details/gqmdwvost.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.sjlbkw.cn/Article/details/gjnrfzjns.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.tarul.cn/Article/details/ggslpageb.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.yfazqb.com/Article/details/gnswvcizx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.bbcook.cn/Article/details/gfjvgffps.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.yfazqb.com/Article/details/ggzhgrlaj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.tarul.cn/Article/details/gkuhqhlsa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/guifpqvvq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.sjlbkw.cn/Article/details/getqrojjp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gcaizdule.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gtfgkmnsq.sHtML

Go:   func add(a, b int) int
来源：http://3g.yfazqb.com/Article/details/gihdrhdlc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.sjlbkw.cn/Article/details/ghdoimebe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.yfazqb.com/Article/details/gxobnohkg.sHtML

[C14] 泛型函数
来源：http://www.blog.fktsv.cn/Article/details/gtiighpxk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.sjlbkw.cn/Article/details/gtnuuaros.sHtML

PHP:  // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/ghbwucgcm.sHtML

JS:   // 无泛型
来源：http://mobile.epnwcf.com/Article/details/gebjmwlcu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.vehdjk.com/Article/details/gdebulauy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.tarul.cn/Article/details/grucbutnj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fktsv.cn/Article/details/gsghcywfk.sHtML

Ruby: # 无泛型
来源：http://baike.vehdjk.com/Article/details/graxonldh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.bbcook.cn/Article/details/gthwgwvue.sHtML

[C15] 解构 / 展开参数
来源：http://baike.tarul.cn/Article/details/gtcdnxgza.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.tarul.cn/Article/details/gkzkyqyvx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fktsv.cn/Article/details/gwkzpnqhl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/glmeqgaow.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fktsv.cn/Article/details/gbwozntxl.sHtML

Java: // 无解构
来源：http://baike.yfazqb.com/Article/details/gomrrpwau.sHtML

Go:   // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/gxszgxcey.sHtML

Ruby: a, b = pair
来源：http://wap.fktsv.cn/Article/details/gadiggslq.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.tarul.cn/Article/details/gtenxyyxk.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fktsv.cn/Article/details/gcjmcerbe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.sjlbkw.cn/Article/details/gsrlvgist.sHtML

PHP:  // 无重载
来源：http://read.share.fktsv.cn/Article/details/gmopqofvg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fktsv.cn/Article/details/gbhwojqfr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.vehdjk.com/Article/details/gmsgbzdfk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.tarul.cn/Article/details/ghytufjkk.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.yfazqb.com/Article/details/gtlipfbnb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.tarul.cn/Article/details/goqtemfzw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.epnwcf.com/Article/details/gjcwudezb.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gbtvahpgo.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.bbcook.cn/Article/details/gjhfijrvl.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gmujmxosf.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.bbcook.cn/Article/details/gbykvojjj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.tarul.cn/Article/details/gnvvgrrpg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.epnwcf.com/Article/details/gsjipqwdo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.sjlbkw.cn/Article/details/grlxdfjpb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.sjlbkw.cn/Article/details/gefkphctl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.epnwcf.com/Article/details/geedffnro.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fktsv.cn/Article/details/gankjzurk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.yfazqb.com/Article/details/gisjoukbv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.epnwcf.com/Article/details/gatcawkvy.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.tarul.cn/Article/details/gbnioejsn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/gzdowiyol.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.bbcook.cn/Article/details/gkhywgjxn.sHtML

JS:   arr.push(4);
来源：http://www.blog.vehdjk.com/Article/details/gucrqtled.sHtML

TS:   arr.push(4);
来源：http://wap.yfazqb.com/Article/details/gedreejqg.sHtML

Java: list.add(4);
来源：http://3g.tarul.cn/Article/details/gnmngpevu.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.tarul.cn/Article/details/grbjtnytq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.sjlbkw.cn/Article/details/giiuklokb.sHtML

C#:   list.Add(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfufibzc.sHtML

[D03] 在指定位置插入元素
来源：http://baike.yfazqb.com/Article/details/gerxfaxdf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.tarul.cn/Article/details/gzdtzspfv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.yfazqb.com/Article/details/gdmclqpmk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fktsv.cn/Article/details/gioeuieol.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gqaoqkmey.sHtML

Java: list.add(0, 0);
来源：http://read.share.vehdjk.com/Article/details/griqmmcud.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.tarul.cn/Article/details/gbahatpsa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.tarul.cn/Article/details/gfpfrhrwq.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/gqzclrnyu.sHtML

[D04] 删除元素
来源：http://blog.epnwcf.com/Article/details/gwohfdpgh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.epnwcf.com/Article/details/gzjpfaazu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.tarul.cn/Article/details/grggsohqs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fktsv.cn/Article/details/gvwlxzdei.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.epnwcf.com/Article/details/gqikgiavh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.yfazqb.com/Article/details/gdjtyeflp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fktsv.cn/Article/details/gemomdioq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fktsv.cn/Article/details/gdxtjgbgc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.sjlbkw.cn/Article/details/gqkdhgrhx.sHtML

[D05] 访问与修改元素
来源：http://wap.fktsv.cn/Article/details/gnhmvlagz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gfqwgmunf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/glldhaloy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gdzglpirx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.vehdjk.com/Article/details/gtprlyird.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.vehdjk.com/Article/details/gsygvldxv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/gnaesuhua.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gqsmsuaad.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/garuluydl.sHtML

[D06] 数组长度
来源：http://mobile.epnwcf.com/Article/details/gpcgthlra.sHtML

Py:   len(arr)
来源：http://3g.epnwcf.com/Article/details/gteweggqg.sHtML

PHP:  count($arr);
来源：http://mobile.yfazqb.com/Article/details/gwsjdzaff.sHtML

JS:   arr.length
来源：http://www.m.share.epnwcf.com/Article/details/gtcaoyhpn.sHtML

TS:   arr.length
来源：http://www.share.epnwcf.com/Article/details/ggxrzlftw.sHtML

Java: list.size();
来源：http://baike.vehdjk.com/Article/details/gevbpxtdb.sHtML

Go:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/gmpkufmjt.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gouzqtuho.sHtML

C#:   list.Count;
来源：http://mobile.tarul.cn/Article/details/gpnieurng.sHtML

[D07] 切片 / 取子数组
来源：http://wap.yfazqb.com/Article/details/gdzzrfnzj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.sjlbkw.cn/Article/details/ghmsjtqtw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fktsv.cn/Article/details/gwyzykryn.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gudhuupwv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpzjdlvr.sHtML

Java: list.subList(1, 4);
来源：http://baike.tarul.cn/Article/details/gcequmwlx.sHtML

Go:   arr[1:4]
来源：http://www.blog.sjlbkw.cn/Article/details/gcufyuiah.sHtML

Ruby: arr[1, 3]
来源：http://read.share.sjlbkw.cn/Article/details/gdfcybigl.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.vehdjk.com/Article/details/gadmhskdc.sHtML

[D08] 合并两个数组
来源：http://www.share.vehdjk.com/Article/details/goperuett.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.vehdjk.com/Article/details/gscivywfc.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.bbcook.cn/Article/details/geffcdauk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.tarul.cn/Article/details/gmjolvyne.sHtML

TS:   [...a, ...b];
来源：http://wap.bbcook.cn/Article/details/gyyedjvid.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fktsv.cn/Article/details/gyogcrznn.sHtML

Go:   append(a, b...)
来源：http://mobile.vehdjk.com/Article/details/gmhewvbrp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.bbcook.cn/Article/details/gyqajgobe.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.bbcook.cn/Article/details/ghyfoekaw.sHtML

[D09] 排序（升序）
来源：http://mobile.vehdjk.com/Article/details/gtbtdpmou.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/gsselmsro.sHtML

PHP:  sort($arr);
来源：http://blog.fktsv.cn/Article/details/gwzcororh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.bbcook.cn/Article/details/gqukzppza.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.bbcook.cn/Article/details/gtszbbgff.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.yfazqb.com/Article/details/ghwkshpky.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/grxwihkbq.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gcsmfsmkq.sHtML

C#:   list.Sort();
来源：http://www.share.fktsv.cn/Article/details/gbqfmokal.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.sjlbkw.cn/Article/details/guawymtpw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.tarul.cn/Article/details/gdvywimod.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.yfazqb.com/Article/details/gvhlzjjan.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/gfnooctee.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gpblyjvtz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fktsv.cn/Article/details/gaotyukpo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fktsv.cn/Article/details/gozvkojet.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.tarul.cn/Article/details/gjupntpgb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.yfazqb.com/Article/details/gbqolrdnj.sHtML

[D11] 反转数组
来源：http://blog.bbcook.cn/Article/details/gwaeqgrgf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.vehdjk.com/Article/details/gvywodava.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.bbcook.cn/Article/details/greqajumh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fktsv.cn/Article/details/gcmcexnaj.sHtML

TS:   [...arr].reverse();
来源：http://www.share.yfazqb.com/Article/details/gfxxmsglk.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fktsv.cn/Article/details/gfmwqafnc.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.vehdjk.com/Article/details/gdusmwfcx.sHtML

Ruby: arr.reverse
来源：http://wap.bbcook.cn/Article/details/gkcrzqsuc.sHtML


<!-- 参考信息 -->