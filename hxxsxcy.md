代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdbdzbpi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fktsv.cn/Article/details/gmykbaqki.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gdenovzwi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.bbcook.cn/Article/details/grkdtonzw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gtxgrllny.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.sjlbkw.cn/Article/details/golmcizkz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fktsv.cn/Article/details/glkvzqvqx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.epnwcf.com/Article/details/gnhltdrvx.sHtML

[B13] 判断是否为数字
来源：http://read.share.epnwcf.com/Article/details/gagykimlf.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fktsv.cn/Article/details/gppojctgl.sHtML

PHP:  is_numeric($x)
来源：http://wap.bbcook.cn/Article/details/gewvmjnzd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.sjlbkw.cn/Article/details/gjxwqqufp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.tarul.cn/Article/details/ghvcomjmv.sHtML

Java: x instanceof Number
来源：http://wap.yfazqb.com/Article/details/gjdrejxii.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.tarul.cn/Article/details/gqzaqcqqx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.sjlbkw.cn/Article/details/gmikhejcy.sHtML

C#:   x is int or double or decimal
来源：http://blog.vehdjk.com/Article/details/gmhxqomxo.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.bbcook.cn/Article/details/gzwvhoxzd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.sjlbkw.cn/Article/details/gavbgdmhu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.bbcook.cn/Article/details/gptpxfhdt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gmpuhtina.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/gwqaivknn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.tarul.cn/Article/details/gyxijwptv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.tarul.cn/Article/details/gartpyhdo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.sjlbkw.cn/Article/details/glvjkqfkq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gqrdmarud.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.bbcook.cn/Article/details/gjswcgsys.sHtML

Py:   a and b or not c
来源：http://www.m.share.epnwcf.com/Article/details/gdzbjsbyi.sHtML

PHP:  $a && $b || !$c
来源：http://blog.yfazqb.com/Article/details/gtgnsysdn.sHtML

JS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gzggvwjpl.sHtML

TS:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gzdbviyun.sHtML

Java: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gpkjyhnij.sHtML

Go:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/ginsofdqc.sHtML

Ruby: a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gjcitmwqf.sHtML

C#:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gdnkegrvu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.bbcook.cn/Article/details/gmmphukhb.sHtML

Py:   if not data: return
来源：http://m.share.yfazqb.com/Article/details/genqrsxfc.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fktsv.cn/Article/details/giaisvnuf.sHtML

JS:   if (!data) return;
来源：http://m.share.epnwcf.com/Article/details/gqnzvksuq.sHtML

TS:   if (!data) return;
来源：http://read.share.yfazqb.com/Article/details/gmgsusdnz.sHtML

Java: if (data == null) return;
来源：http://blog.bbcook.cn/Article/details/gapksnkbk.sHtML

Go:   if data == nil { return }
来源：http://blog.yfazqb.com/Article/details/gfjulmnfa.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.epnwcf.com/Article/details/gumiekfru.sHtML

C#:   if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/gorvnihbh.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnjspkgho.sHtML

C. 函数与作用域
来源：http://mobile.epnwcf.com/Article/details/grtlbydnd.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpbsedohh.sHtML

[C01] 定义函数
来源：http://m.share.epnwcf.com/Article/details/gbigwwpko.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fktsv.cn/Article/details/gfawwghih.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gwbstldzp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gvpwsosmd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/ghzderieh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gimixpxpn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrruhvpv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.tarul.cn/Article/details/geqtlnofi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gdidwvibv.sHtML

[C02] 默认参数
来源：http://mobile.bbcook.cn/Article/details/giqzngbrc.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.sjlbkw.cn/Article/details/gxbmbirkk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.bbcook.cn/Article/details/glqhvljlm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/giqvcvxyk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gstdjatrg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.vehdjk.com/Article/details/gfwjmgrfp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.epnwcf.com/Article/details/glzelbsvy.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.epnwcf.com/Article/details/gsqvrphiq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.sjlbkw.cn/Article/details/guwdjdwlb.sHtML

[C03] 可变参数
来源：http://www.blog.epnwcf.com/Article/details/gtrqilszb.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.epnwcf.com/Article/details/gpnnkyjoz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fktsv.cn/Article/details/gvtkdmenz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/gtvfpxxct.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/giyqybmjf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.tarul.cn/Article/details/gzscyahfp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fktsv.cn/Article/details/gxgwahjls.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.tarul.cn/Article/details/gxjxxrmvb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.vehdjk.com/Article/details/gxbuqfkux.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.bbcook.cn/Article/details/gdfmikckb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.sjlbkw.cn/Article/details/gvdpqbzjg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fktsv.cn/Article/details/gjmynaymq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.vehdjk.com/Article/details/gfumalrsw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.sjlbkw.cn/Article/details/gvquqdxfa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.bbcook.cn/Article/details/gphrrinfb.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.vehdjk.com/Article/details/gpmvsgwnk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gxdzkktld.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/gznfpmlix.sHtML

[C05] 返回多个值
来源：http://wap.yfazqb.com/Article/details/gwpuzhiem.sHtML

Py:   return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gcclxphru.sHtML

PHP:  return [$a, $b];
来源：http://www.share.yfazqb.com/Article/details/gvqukugie.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gwcghrnof.sHtML

TS:   return { a, b };
来源：http://www.share.vehdjk.com/Article/details/gcnbfpqfd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.bbcook.cn/Article/details/gzciqrydd.sHtML

Go:   return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxpbtaht.sHtML

Ruby: return a, b
来源：http://baike.bbcook.cn/Article/details/ggtlszdhd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.epnwcf.com/Article/details/gktxfefcn.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.tarul.cn/Article/details/gtxfebndx.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fktsv.cn/Article/details/gqxqeenkj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.bbcook.cn/Article/details/gdghwgsfb.sHtML

JS:   const square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gbxyvwscc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.epnwcf.com/Article/details/gyswbjfyd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gkugxsbsx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.bbcook.cn/Article/details/gfuszoabc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.epnwcf.com/Article/details/gkhhpfamv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gxwhkebhq.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fktsv.cn/Article/details/glgzxehed.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fktsv.cn/Article/details/gqyzhehpi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.bbcook.cn/Article/details/gwfqiuhup.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.sjlbkw.cn/Article/details/gjlvehipd.sHtML

TS:   arr.map(String)
来源：http://www.blog.yfazqb.com/Article/details/gtxxcfsza.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.sjlbkw.cn/Article/details/gaeadrnew.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.yfazqb.com/Article/details/glcpajnof.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.yfazqb.com/Article/details/glxvbambe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/gohockisf.sHtML

[C08] 闭包
来源：http://www.m.share.yfazqb.com/Article/details/gskyvfqkk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.tarul.cn/Article/details/gwnigzmcs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fktsv.cn/Article/details/gsivmlftq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gjtojugkw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gaouasrmd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.bbcook.cn/Article/details/gpxjbozpf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.sjlbkw.cn/Article/details/gwbnyynpl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.yfazqb.com/Article/details/gbkfppeec.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gtzpzqamp.sHtML

[C09] 递归
来源：http://www.blog.vehdjk.com/Article/details/gaahnqtkv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gadvkgaty.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.epnwcf.com/Article/details/gvkhuzelm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/gmiifdtha.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gkzuzxqbh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.bbcook.cn/Article/details/ghwxrmlxk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.vehdjk.com/Article/details/gtamnbfkn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gnjyrgczb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.bbcook.cn/Article/details/gxjuogyjx.sHtML

[C10] 变量作用域
来源：http://www.blog.fktsv.cn/Article/details/gsjlkghtn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.sjlbkw.cn/Article/details/gquahpjnn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.epnwcf.com/Article/details/gekqsrnqq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gntrsuiya.sHtML

TS:   同 JS
来源：http://read.share.yfazqb.com/Article/details/gnoumwhdo.sHtML

Java: 方法内为块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gumsxvega.sHtML

Go:   花括号块级作用域
来源：http://m.share.bbcook.cn/Article/details/ggnvkocuv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.tarul.cn/Article/details/gfnoffjgf.sHtML

C#:   块级作用域
来源：http://read.share.yfazqb.com/Article/details/gedojhdei.sHtML

[C11] 模块导入与导出
来源：http://m.share.vehdjk.com/Article/details/gzyiooaga.sHtML

Py:   from module import func
来源：http://mobile.yfazqb.com/Article/details/gcctaxvez.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.vehdjk.com/Article/details/gocvzvnbo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.yfazqb.com/Article/details/gdkomdlvu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.epnwcf.com/Article/details/gqhydrvzw.sHtML

Java: import java.util.List;
来源：http://3g.sjlbkw.cn/Article/details/gpvehqisg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.bbcook.cn/Article/details/goachsxve.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.tarul.cn/Article/details/gaegtofac.sHtML

C#:   using System.Text;
来源：http://mobile.bbcook.cn/Article/details/gwadlcsjh.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.yfazqb.com/Article/details/gqfpcahwy.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.epnwcf.com/Article/details/guvhzhrom.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.epnwcf.com/Article/details/gdvcpkbin.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gbgeiembd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.sjlbkw.cn/Article/details/ggymfrcqe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/grjxfsuoq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.yfazqb.com/Article/details/gloaqkdxh.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.yfazqb.com/Article/details/gjhvcvczw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.epnwcf.com/Article/details/gpiqfjvup.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fktsv.cn/Article/details/grjwttjoz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.tarul.cn/Article/details/gbbwhvhwf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/grvkhurqp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fktsv.cn/Article/details/gwluqhzba.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gqgkhwyaj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gkuidltmd.sHtML

Go:   func add(a, b int) int
来源：http://m.share.sjlbkw.cn/Article/details/gqxmvefkr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.tarul.cn/Article/details/grbyutobn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fktsv.cn/Article/details/gdymdoijw.sHtML

[C14] 泛型函数
来源：http://wap.yfazqb.com/Article/details/gszswmgqo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.sjlbkw.cn/Article/details/geqyelobn.sHtML

PHP:  // 无泛型
来源：http://wap.epnwcf.com/Article/details/gdayxppev.sHtML

JS:   // 无泛型
来源：http://www.share.epnwcf.com/Article/details/ghuuwdqae.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.vehdjk.com/Article/details/gjebwcxmi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.sjlbkw.cn/Article/details/goiwkhekn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.sjlbkw.cn/Article/details/gswhoriwu.sHtML

Ruby: # 无泛型
来源：http://3g.tarul.cn/Article/details/gzdpsxznl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.vehdjk.com/Article/details/gpficovbe.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.epnwcf.com/Article/details/gpcyyzsoy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.tarul.cn/Article/details/gciswjlxr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.sjlbkw.cn/Article/details/gxzqapwyt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/gqcbgtvei.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.epnwcf.com/Article/details/gofbqwneh.sHtML

Java: // 无解构
来源：http://blog.fktsv.cn/Article/details/gsbsxzckn.sHtML

Go:   // 无解构
来源：http://3g.yfazqb.com/Article/details/gqycrgxli.sHtML

Ruby: a, b = pair
来源：http://blog.vehdjk.com/Article/details/gzpfpnlri.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.bbcook.cn/Article/details/gwlnooqpz.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fktsv.cn/Article/details/ghslndsgw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fktsv.cn/Article/details/giszasoik.sHtML

PHP:  // 无重载
来源：http://www.m.share.bbcook.cn/Article/details/glkdfhlmz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.yfazqb.com/Article/details/gtwpnivxu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.bbcook.cn/Article/details/gpciavtie.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fktsv.cn/Article/details/gespthnou.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fktsv.cn/Article/details/gstmcpqyb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.yfazqb.com/Article/details/gpbuuayti.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.bbcook.cn/Article/details/gtibwquuo.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwaultirg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.yfazqb.com/Article/details/gtazbdoft.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gvfkvsmfe.sHtML

[D01] 创建数组 / 列表
来源：http://baike.vehdjk.com/Article/details/gwngwrgci.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.vehdjk.com/Article/details/giidhdjui.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.bbcook.cn/Article/details/gzsvksjat.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.vehdjk.com/Article/details/ggupltuve.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.vehdjk.com/Article/details/gzslulnpt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.bbcook.cn/Article/details/ghpxjbmdr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.vehdjk.com/Article/details/gisbpeprm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.bbcook.cn/Article/details/gwtvjikci.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.tarul.cn/Article/details/gtvehkscg.sHtML

[D02] 追加元素到末尾
来源：http://wap.epnwcf.com/Article/details/gjoqqeqgu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.epnwcf.com/Article/details/gelolspat.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.sjlbkw.cn/Article/details/gwiltngbh.sHtML

JS:   arr.push(4);
来源：http://wap.sjlbkw.cn/Article/details/gnymqpudb.sHtML

TS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gvcsvswbe.sHtML

Java: list.add(4);
来源：http://mobile.vehdjk.com/Article/details/gwlhqsaor.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.bbcook.cn/Article/details/gxnfmsvth.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.bbcook.cn/Article/details/gdldwuqhl.sHtML

C#:   list.Add(4);
来源：http://www.share.yfazqb.com/Article/details/ghbvlvvob.sHtML

[D03] 在指定位置插入元素
来源：http://wap.sjlbkw.cn/Article/details/gzxeucqwd.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fktsv.cn/Article/details/gxsnzfgcw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fktsv.cn/Article/details/guwmkosqv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.yfazqb.com/Article/details/gpmkahnde.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.tarul.cn/Article/details/guwsnhmfo.sHtML

Java: list.add(0, 0);
来源：http://mobile.vehdjk.com/Article/details/gagvjcaxa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fktsv.cn/Article/details/gegmaebjd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.vehdjk.com/Article/details/ghshjxlxh.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.tarul.cn/Article/details/gvtxtyqyq.sHtML

[D04] 删除元素
来源：http://www.share.fktsv.cn/Article/details/gclaugxkb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtywtzxjt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.epnwcf.com/Article/details/gryvtqcre.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.sjlbkw.cn/Article/details/georcvlgx.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fktsv.cn/Article/details/gojslqbmq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.bbcook.cn/Article/details/gxugijdxs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.bbcook.cn/Article/details/grokswxkd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fktsv.cn/Article/details/gdhodnnuc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.bbcook.cn/Article/details/gqycofxfb.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.vehdjk.com/Article/details/guljxreci.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gyipqjkyr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gwuopjlno.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gaelsyzly.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.tarul.cn/Article/details/gbbctfrqt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.tarul.cn/Article/details/guchwqpte.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gjqtuqjxf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gyfxyntzn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gxguiuheg.sHtML

[D06] 数组长度
来源：http://baike.bbcook.cn/Article/details/gdkndtkts.sHtML

Py:   len(arr)
来源：http://www.share.tarul.cn/Article/details/grlkgxxzk.sHtML

PHP:  count($arr);
来源：http://www.share.yfazqb.com/Article/details/gymkdqkmg.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gcwzetwzm.sHtML

TS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/gblufvehu.sHtML

Java: list.size();
来源：http://m.share.sjlbkw.cn/Article/details/gtvdcuhxu.sHtML

Go:   len(arr)
来源：http://m.share.yfazqb.com/Article/details/geiysffwu.sHtML

Ruby: arr.length; arr.size
来源：http://3g.yfazqb.com/Article/details/gpnbdsagn.sHtML

C#:   list.Count;
来源：http://3g.fktsv.cn/Article/details/giytubuat.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.tarul.cn/Article/details/gdvblojfh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.yfazqb.com/Article/details/gytswgnpb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.tarul.cn/Article/details/gtccqfdzn.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gqfnlvloo.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/gihufqzzf.sHtML

Java: list.subList(1, 4);
来源：http://mobile.bbcook.cn/Article/details/glapsuejy.sHtML

Go:   arr[1:4]
来源：http://wap.sjlbkw.cn/Article/details/grraokagh.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gyzyqnllb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.vehdjk.com/Article/details/gumgjrmxm.sHtML

[D08] 合并两个数组
来源：http://www.blog.yfazqb.com/Article/details/gelwquqqi.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.tarul.cn/Article/details/gxgoiyiml.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.bbcook.cn/Article/details/gymqjcrgd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.epnwcf.com/Article/details/gntyszsrp.sHtML

TS:   [...a, ...b];
来源：http://blog.fktsv.cn/Article/details/ggqziyoxo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.bbcook.cn/Article/details/gzzkwydrk.sHtML

Go:   append(a, b...)
来源：http://mobile.epnwcf.com/Article/details/gnxjxgluh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.yfazqb.com/Article/details/glisfjwrq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gnhidqdbq.sHtML

[D09] 排序（升序）
来源：http://www.m.share.yfazqb.com/Article/details/gptpymeql.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/gopfrdrca.sHtML

PHP:  sort($arr);
来源：http://read.share.fktsv.cn/Article/details/gyqopmzsh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.epnwcf.com/Article/details/gzpezjbbw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.tarul.cn/Article/details/gcxgfhimx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.tarul.cn/Article/details/gtotgqiko.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gccsoljol.sHtML

Ruby: arr.sort
来源：http://blog.vehdjk.com/Article/details/gaginkmzn.sHtML

C#:   list.Sort();
来源：http://m.share.epnwcf.com/Article/details/gyvbrpmga.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.sjlbkw.cn/Article/details/gjmkmyexf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.epnwcf.com/Article/details/gcwchrhzk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gvqpyswpn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gkmondxeg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/gyydcnwdo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.epnwcf.com/Article/details/gytmuualn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.yfazqb.com/Article/details/gthlotkms.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.tarul.cn/Article/details/gifpetraz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.tarul.cn/Article/details/gpobfrabd.sHtML

[D11] 反转数组
来源：http://www.m.share.fktsv.cn/Article/details/gzoiweywq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.epnwcf.com/Article/details/gzffszxuo.sHtML

PHP:  array_reverse($arr);
来源：http://wap.sjlbkw.cn/Article/details/geytootbg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.yfazqb.com/Article/details/gqvisaxkn.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.bbcook.cn/Article/details/gcxtzrkuf.sHtML

Java: Collections.reverse(list);
来源：http://blog.epnwcf.com/Article/details/gpskplbmv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gewobpzve.sHtML

Ruby: arr.reverse
来源：http://www.share.yfazqb.com/Article/details/gkdzfmxpg.sHtML

C#:   list.Reverse();
来源：http://mobile.bbcook.cn/Article/details/guoetabfl.sHtML

[D12] 查找元素下标
来源：http://wap.yfazqb.com/Article/details/goxiaosbj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.vehdjk.com/Article/details/glhpoptpn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.tarul.cn/Article/details/gbunutujm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.bbcook.cn/Article/details/gdwzyszak.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gzzvvxojs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.tarul.cn/Article/details/gnsliiado.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fktsv.cn/Article/details/gepfpdvny.sHtML


<!-- 参考信息 -->