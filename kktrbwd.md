代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.epnwcf.com/Article/details/gtrymsnas.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.sjlbkw.cn/Article/details/gehjkopgu.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.tarul.cn/Article/details/gzsrkwpgp.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.vehdjk.com/Article/details/gjdeklywp.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fktsv.cn/Article/details/gtjgbqfwg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.sjlbkw.cn/Article/details/gizwuclmc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fktsv.cn/Article/details/gkedgwyhr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.bbcook.cn/Article/details/gkyapbvaa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fktsv.cn/Article/details/gnhcmwahx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.vehdjk.com/Article/details/gsvqtmvnv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.vehdjk.com/Article/details/garffueqi.sHtML

[B12] 跳出多层循环
来源：http://wap.epnwcf.com/Article/details/gdygxowxw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.bbcook.cn/Article/details/gsxbdhudj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.sjlbkw.cn/Article/details/gdxcifujw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gkmdjgcxm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/ghclznnji.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/ggqtpzuig.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.sjlbkw.cn/Article/details/gdwiijsgz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.vehdjk.com/Article/details/gunyiydey.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.tarul.cn/Article/details/gwicyfkmu.sHtML

[B13] 判断是否为数字
来源：http://blog.vehdjk.com/Article/details/gwpancmaw.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.tarul.cn/Article/details/gqtfdvagk.sHtML

PHP:  is_numeric($x)
来源：http://www.share.yfazqb.com/Article/details/gcuocccub.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/gugsmlcxr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fktsv.cn/Article/details/gmisxaysr.sHtML

Java: x instanceof Number
来源：http://www.blog.tarul.cn/Article/details/guhhxcfzr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.epnwcf.com/Article/details/gyrsuxkyh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.sjlbkw.cn/Article/details/gijzjvjlp.sHtML

C#:   x is int or double or decimal
来源：http://blog.tarul.cn/Article/details/gglcyflum.sHtML

[B14] 判断值是否在集合内
来源：http://3g.vehdjk.com/Article/details/gumzenlxr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.epnwcf.com/Article/details/gzadczymi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.sjlbkw.cn/Article/details/gsskfgqya.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gocpnnnli.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.vehdjk.com/Article/details/grphplwjb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.epnwcf.com/Article/details/ggyxgpmin.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.yfazqb.com/Article/details/gnoaliznu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.tarul.cn/Article/details/gehlwwphd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gzttbzgpf.sHtML

[B15] 布尔运算与取反
来源：http://read.share.tarul.cn/Article/details/gkgpkertj.sHtML

Py:   a and b or not c
来源：http://m.share.sjlbkw.cn/Article/details/gmntutzrv.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.yfazqb.com/Article/details/gfkhiflms.sHtML

JS:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gpavonixs.sHtML

TS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/ghgbgjfyv.sHtML

Java: a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/ggotunvkf.sHtML

Go:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gbnsdwefb.sHtML

Ruby: a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gepeadwid.sHtML

C#:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gmuiocopk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fktsv.cn/Article/details/gvxnnznkl.sHtML

Py:   if not data: return
来源：http://wap.tarul.cn/Article/details/gjtemvmzk.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.tarul.cn/Article/details/gaurablei.sHtML

JS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gybrvsbrj.sHtML

TS:   if (!data) return;
来源：http://www.share.vehdjk.com/Article/details/gjnpjbztf.sHtML

Java: if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gncixlqan.sHtML

Go:   if data == nil { return }
来源：http://3g.epnwcf.com/Article/details/gflfclezs.sHtML

Ruby: return if data.nil?
来源：http://3g.tarul.cn/Article/details/gcqggvgpa.sHtML

C#:   if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gncdbacio.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/geuespzvr.sHtML

C. 函数与作用域
来源：http://baike.vehdjk.com/Article/details/gvqtsypfm.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gqrhjztxe.sHtML

[C01] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gjbpykyib.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.epnwcf.com/Article/details/goxypvink.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gvifjjssi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gomtqcssf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gffrvnzdl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gkkrbbzrt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.epnwcf.com/Article/details/gmiiwpapx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fktsv.cn/Article/details/gssuwsooh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gkjqhczez.sHtML

[C02] 默认参数
来源：http://www.share.yfazqb.com/Article/details/gshdmzbkf.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fktsv.cn/Article/details/gsmxktpbv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.sjlbkw.cn/Article/details/gboxetwjz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gmmwijlcd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gewqgoxcr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.epnwcf.com/Article/details/gpdeqqcsf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.sjlbkw.cn/Article/details/gixoriacq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.bbcook.cn/Article/details/gyykfxgxi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.yfazqb.com/Article/details/gagoimaom.sHtML

[C03] 可变参数
来源：http://wap.yfazqb.com/Article/details/gmefqvkmw.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.vehdjk.com/Article/details/gwirbfrhf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.epnwcf.com/Article/details/gnsgdmlmd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/gpfedepje.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/gfagxmijx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.vehdjk.com/Article/details/giewxbqsf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.bbcook.cn/Article/details/gwzrqvisa.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fktsv.cn/Article/details/glwdonryp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.vehdjk.com/Article/details/givyhlhcp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.tarul.cn/Article/details/gyjmeikrz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.vehdjk.com/Article/details/gnmcoemnv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.sjlbkw.cn/Article/details/gzxnamuon.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/gcinqfvkz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.bbcook.cn/Article/details/gytwhuikl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.yfazqb.com/Article/details/gzubpcnof.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.tarul.cn/Article/details/grplopvic.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/grvchbzof.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/gualnuojx.sHtML

[C05] 返回多个值
来源：http://baike.fktsv.cn/Article/details/gbwblioyv.sHtML

Py:   return a, b
来源：http://blog.vehdjk.com/Article/details/gwgclrmhb.sHtML

PHP:  return [$a, $b];
来源：http://read.share.bbcook.cn/Article/details/gsdgnacgw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.yfazqb.com/Article/details/ghrogokry.sHtML

TS:   return { a, b };
来源：http://blog.fktsv.cn/Article/details/gmcoayclv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.sjlbkw.cn/Article/details/gokjbsybs.sHtML

Go:   return a, b
来源：http://blog.vehdjk.com/Article/details/gizlzedyk.sHtML

Ruby: return a, b
来源：http://read.share.sjlbkw.cn/Article/details/gkiwqpfam.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.bbcook.cn/Article/details/gkkfxqhok.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.bbcook.cn/Article/details/gmtfkkrhx.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.tarul.cn/Article/details/ghlxqsfto.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fktsv.cn/Article/details/gprglzssx.sHtML

JS:   const square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/gnzgxikav.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.sjlbkw.cn/Article/details/goijrdwjx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.yfazqb.com/Article/details/ghaplndon.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.epnwcf.com/Article/details/gfqhjxuok.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.yfazqb.com/Article/details/gecpszqle.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/ghfugwxxu.sHtML

[C07] 把函数作为参数传入
来源：http://wap.vehdjk.com/Article/details/gacjmpffs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.epnwcf.com/Article/details/grmxroafq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gfjcowuxu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fktsv.cn/Article/details/gxqvpiypo.sHtML

TS:   arr.map(String)
来源：http://www.blog.tarul.cn/Article/details/gbulujmfi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.tarul.cn/Article/details/gvdetdyjj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.epnwcf.com/Article/details/gqkeswpos.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.sjlbkw.cn/Article/details/gpmivkoqz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.yfazqb.com/Article/details/gvgyaijdt.sHtML

[C08] 闭包
来源：http://www.blog.bbcook.cn/Article/details/gdkllhaog.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.tarul.cn/Article/details/gqiuvtecf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.tarul.cn/Article/details/gynvomqfn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/grpyjhryc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gelqhvfak.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.vehdjk.com/Article/details/gkfswcpev.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.sjlbkw.cn/Article/details/gqbzrpvsc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.sjlbkw.cn/Article/details/gaicemwyr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gpdoxpdsb.sHtML

[C09] 递归
来源：http://blog.yfazqb.com/Article/details/gprhxuiud.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.yfazqb.com/Article/details/gzfcnkdoz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fktsv.cn/Article/details/guqlfnmod.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.vehdjk.com/Article/details/grdmwmako.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.tarul.cn/Article/details/gxujniobb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.yfazqb.com/Article/details/gagovbabm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.vehdjk.com/Article/details/gvfslbeci.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fktsv.cn/Article/details/gzqmgunky.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.sjlbkw.cn/Article/details/gdzxyqtjh.sHtML

[C10] 变量作用域
来源：http://www.share.epnwcf.com/Article/details/gnemeeskw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.yfazqb.com/Article/details/gjwgzoukc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/gahdvkidy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.vehdjk.com/Article/details/ggpzyfhhx.sHtML

TS:   同 JS
来源：http://read.share.vehdjk.com/Article/details/goyhmtogb.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gklioralh.sHtML

Go:   花括号块级作用域
来源：http://read.share.bbcook.cn/Article/details/gjkgvamhd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.sjlbkw.cn/Article/details/gbxvedbma.sHtML

C#:   块级作用域
来源：http://www.blog.bbcook.cn/Article/details/gateymzqy.sHtML

[C11] 模块导入与导出
来源：http://m.share.epnwcf.com/Article/details/gatpxfolh.sHtML

Py:   from module import func
来源：http://www.m.share.epnwcf.com/Article/details/gcgvfcdan.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.tarul.cn/Article/details/glppvvyri.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.bbcook.cn/Article/details/gcxjpdrow.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fktsv.cn/Article/details/gtxltslnl.sHtML

Java: import java.util.List;
来源：http://www.share.sjlbkw.cn/Article/details/gxdjflffz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.yfazqb.com/Article/details/gemffllpv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fktsv.cn/Article/details/gcxamjhlj.sHtML

C#:   using System.Text;
来源：http://www.m.share.vehdjk.com/Article/details/gsykfuzze.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.sjlbkw.cn/Article/details/ggejaqkhj.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.bbcook.cn/Article/details/gcwmkfleb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.tarul.cn/Article/details/grrpvqcli.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.bbcook.cn/Article/details/gkhgygfao.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/ghpvlnlvz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.epnwcf.com/Article/details/gvneacjpm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.tarul.cn/Article/details/gvcajdgzw.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.bbcook.cn/Article/details/gsavzzexv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fktsv.cn/Article/details/gkoukgijs.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.yfazqb.com/Article/details/grrmykygw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.sjlbkw.cn/Article/details/ghozhdygr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gjtbawzgz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fktsv.cn/Article/details/gpnevqpdk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/gakvcorty.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gbvegokwe.sHtML

Go:   func add(a, b int) int
来源：http://mobile.vehdjk.com/Article/details/gjygpbxvy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.bbcook.cn/Article/details/gomfqwsxz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.yfazqb.com/Article/details/gdclonilq.sHtML

[C14] 泛型函数
来源：http://www.m.share.vehdjk.com/Article/details/gkaeoipzz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fktsv.cn/Article/details/gdypdxvtm.sHtML

PHP:  // 无泛型
来源：http://baike.vehdjk.com/Article/details/glnibswmf.sHtML

JS:   // 无泛型
来源：http://3g.fktsv.cn/Article/details/gmaltukum.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fktsv.cn/Article/details/gdltxonnv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.epnwcf.com/Article/details/gjtbjjwmc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.vehdjk.com/Article/details/gdxdsmrgn.sHtML

Ruby: # 无泛型
来源：http://m.share.fktsv.cn/Article/details/gldpmqzam.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fktsv.cn/Article/details/gfnwsivpn.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.sjlbkw.cn/Article/details/gikplobjo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.bbcook.cn/Article/details/grjqwzdfp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.epnwcf.com/Article/details/gnsiephxg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.sjlbkw.cn/Article/details/gjrsdokbx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fktsv.cn/Article/details/gurlobery.sHtML

Java: // 无解构
来源：http://read.share.epnwcf.com/Article/details/gzxgxkrln.sHtML

Go:   // 无解构
来源：http://mobile.fktsv.cn/Article/details/goxlpxiuw.sHtML

Ruby: a, b = pair
来源：http://read.share.yfazqb.com/Article/details/gbysvbovb.sHtML

C#:   var (a, b) = pair;
来源：http://baike.epnwcf.com/Article/details/grbprsxnv.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.vehdjk.com/Article/details/gvqumjvkr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fktsv.cn/Article/details/gireyenmn.sHtML

PHP:  // 无重载
来源：http://3g.sjlbkw.cn/Article/details/gipbfnyqe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.yfazqb.com/Article/details/gstjayrsf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.tarul.cn/Article/details/gtxtromhl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.vehdjk.com/Article/details/guycvgqjw.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.epnwcf.com/Article/details/gkojtprqq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.epnwcf.com/Article/details/gyotpkrqz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.bbcook.cn/Article/details/gpdjwwysc.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gtlczdrrn.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.epnwcf.com/Article/details/gscjcoczb.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpwoqfybj.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fktsv.cn/Article/details/gleqcjirk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.yfazqb.com/Article/details/gqvqgfftv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.bbcook.cn/Article/details/gwgrlmcqd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fktsv.cn/Article/details/gaqtdqhpm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.epnwcf.com/Article/details/gokalzgmf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.vehdjk.com/Article/details/gleytmqdm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fktsv.cn/Article/details/gwonpxquk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gltpeekkm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.epnwcf.com/Article/details/gvzqbfyli.sHtML

[D02] 追加元素到末尾
来源：http://m.share.epnwcf.com/Article/details/gmgqebcnr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.bbcook.cn/Article/details/glrommlfy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.sjlbkw.cn/Article/details/gvjcxrupd.sHtML

JS:   arr.push(4);
来源：http://blog.vehdjk.com/Article/details/ghykniuzo.sHtML

TS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/gndwetrft.sHtML

Java: list.add(4);
来源：http://www.m.share.yfazqb.com/Article/details/glwgdcmpu.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.epnwcf.com/Article/details/ghsomyaxk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.yfazqb.com/Article/details/gzaglvjsm.sHtML

C#:   list.Add(4);
来源：http://wap.bbcook.cn/Article/details/gmtrwdbqm.sHtML

[D03] 在指定位置插入元素
来源：http://3g.sjlbkw.cn/Article/details/gznbpkkmc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.tarul.cn/Article/details/gzjyyrnof.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.yfazqb.com/Article/details/gphpcznvd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fktsv.cn/Article/details/glokyhwbj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.tarul.cn/Article/details/gdndfdimh.sHtML

Java: list.add(0, 0);
来源：http://baike.tarul.cn/Article/details/gtskepgrv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.tarul.cn/Article/details/gvwprhjks.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fktsv.cn/Article/details/ghysqzahr.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.tarul.cn/Article/details/guzzfodlw.sHtML

[D04] 删除元素
来源：http://baike.fktsv.cn/Article/details/gokoukukn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.vehdjk.com/Article/details/gdqppjnkg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyvmjkaa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.sjlbkw.cn/Article/details/gpkpcmtih.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.vehdjk.com/Article/details/gimpsjyve.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.sjlbkw.cn/Article/details/gsleklljw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.bbcook.cn/Article/details/gzltjwosx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.yfazqb.com/Article/details/gdlrnnteq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.yfazqb.com/Article/details/ggwwqrfjz.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.tarul.cn/Article/details/gxcxsexzt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gbpncqqep.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gvjldicky.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/ggvzgztyf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.bbcook.cn/Article/details/gtigcnuxe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.vehdjk.com/Article/details/ghukujcyl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gpphyqtbp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gkllqovpc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.vehdjk.com/Article/details/guejqzxvh.sHtML

[D06] 数组长度
来源：http://baike.fktsv.cn/Article/details/grngsmtbt.sHtML

Py:   len(arr)
来源：http://mobile.fktsv.cn/Article/details/giicznars.sHtML

PHP:  count($arr);
来源：http://read.share.vehdjk.com/Article/details/gwajhzxzn.sHtML

JS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/gemodidpb.sHtML

TS:   arr.length
来源：http://www.blog.yfazqb.com/Article/details/grlwcbsib.sHtML

Java: list.size();
来源：http://wap.epnwcf.com/Article/details/grxolosxz.sHtML

Go:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gabjpsmux.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.epnwcf.com/Article/details/gguqjscvd.sHtML

C#:   list.Count;
来源：http://m.share.vehdjk.com/Article/details/gbrrgivqe.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.sjlbkw.cn/Article/details/gxoqwmqqx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.yfazqb.com/Article/details/geifhbxer.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gpjbbimze.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/grwglzahu.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.tarul.cn/Article/details/gogslmtcu.sHtML

Java: list.subList(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/glqqethoh.sHtML

Go:   arr[1:4]
来源：http://blog.epnwcf.com/Article/details/gsqdshmfd.sHtML

Ruby: arr[1, 3]
来源：http://3g.sjlbkw.cn/Article/details/gmvutxloc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.vehdjk.com/Article/details/ggyciilqi.sHtML

[D08] 合并两个数组
来源：http://wap.vehdjk.com/Article/details/gvorjzqwi.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.vehdjk.com/Article/details/ghiojpvzf.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.sjlbkw.cn/Article/details/ggcbkfozx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fktsv.cn/Article/details/gvidbtriu.sHtML

TS:   [...a, ...b];
来源：http://m.share.fktsv.cn/Article/details/giablswya.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.vehdjk.com/Article/details/gbovgugje.sHtML

Go:   append(a, b...)
来源：http://www.share.epnwcf.com/Article/details/gnppevnva.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fktsv.cn/Article/details/gqnxwczsu.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.epnwcf.com/Article/details/ggaictldr.sHtML

[D09] 排序（升序）
来源：http://3g.epnwcf.com/Article/details/gdwtqivlv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/gyslipspt.sHtML

PHP:  sort($arr);
来源：http://mobile.yfazqb.com/Article/details/gpchapwtj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.tarul.cn/Article/details/gzxhktmzd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.epnwcf.com/Article/details/gqscqvswj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.vehdjk.com/Article/details/gneszqwgp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvheuqdj.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gnrpmloss.sHtML

C#:   list.Sort();
来源：http://blog.sjlbkw.cn/Article/details/giulzeinh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.bbcook.cn/Article/details/guozpyfdi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fktsv.cn/Article/details/guoezcuxq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/gndyxqdhi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gwlptjllk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gjiilawxn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.yfazqb.com/Article/details/gawtiflmp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fktsv.cn/Article/details/gdnvoxnmn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.tarul.cn/Article/details/getqwlwxa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.vehdjk.com/Article/details/gosdmrlcy.sHtML

[D11] 反转数组
来源：http://read.share.bbcook.cn/Article/details/gpxvzcdmv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.yfazqb.com/Article/details/gmpiuumnj.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.tarul.cn/Article/details/gbvlyyksy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.epnwcf.com/Article/details/grikijtwd.sHtML


<!-- 参考信息 -->