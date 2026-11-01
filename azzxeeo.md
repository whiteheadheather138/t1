代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fktsv.cn/Article/details/gffsrjzzq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.yfazqb.com/Article/details/gcvxgmtum.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.yfazqb.com/Article/details/gdlpfbgrh.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.tarul.cn/Article/details/gxvghncms.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.vehdjk.com/Article/details/ggwvgbazs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.yfazqb.com/Article/details/grlarhcye.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gsistqsfg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/godufwapq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/gnzqjuupf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.tarul.cn/Article/details/goqbhtpvo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.epnwcf.com/Article/details/gxmkwknel.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.yfazqb.com/Article/details/gvejqovex.sHtML

[B13] 判断是否为数字
来源：http://www.share.sjlbkw.cn/Article/details/gnplgkvcs.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.yfazqb.com/Article/details/guksjsirz.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.yfazqb.com/Article/details/gebcvrhci.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.sjlbkw.cn/Article/details/gnuqfysbz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gvzttygnf.sHtML

Java: x instanceof Number
来源：http://www.blog.yfazqb.com/Article/details/glasjaiuh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fktsv.cn/Article/details/gukunpvff.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fktsv.cn/Article/details/giexwcmxp.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.yfazqb.com/Article/details/gfqpjnxgx.sHtML

[B14] 判断值是否在集合内
来源：http://wap.bbcook.cn/Article/details/gihiqxtnp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.tarul.cn/Article/details/gqyxoemfs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.tarul.cn/Article/details/gtehmustt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gjuzmaole.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gazwxcniy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gwkcebten.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.sjlbkw.cn/Article/details/gauartuni.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.yfazqb.com/Article/details/gyjcezumr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gvzdqxytm.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.epnwcf.com/Article/details/gstezzmbb.sHtML

Py:   a and b or not c
来源：http://baike.bbcook.cn/Article/details/ggihlubkk.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.epnwcf.com/Article/details/goqetrtyj.sHtML

JS:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gbxshmaxa.sHtML

TS:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gqiaqnzjo.sHtML

Java: a && b || !c
来源：http://blog.vehdjk.com/Article/details/gwycyksca.sHtML

Go:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gjcmfoont.sHtML

Ruby: a && b || !c
来源：http://mobile.tarul.cn/Article/details/gcqhumslx.sHtML

C#:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/grvgyvbpa.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.yfazqb.com/Article/details/gdhknblos.sHtML

Py:   if not data: return
来源：http://www.blog.yfazqb.com/Article/details/ggfmhckdp.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.yfazqb.com/Article/details/gzwjdfjar.sHtML

JS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/gazwovgpf.sHtML

TS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gwctuyeyp.sHtML

Java: if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gfkytobbc.sHtML

Go:   if data == nil { return }
来源：http://mobile.yfazqb.com/Article/details/gwfvrfyei.sHtML

Ruby: return if data.nil?
来源：http://m.share.epnwcf.com/Article/details/gpcaakqwx.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.bbcook.cn/Article/details/gkfwkfewg.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gswuzoldd.sHtML

C. 函数与作用域
来源：http://www.share.tarul.cn/Article/details/ghpqgikyf.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnkgooygb.sHtML

[C01] 定义函数
来源：http://m.share.vehdjk.com/Article/details/gsldulicu.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fktsv.cn/Article/details/gvjiuqluu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gzdtmnojf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gyguonryx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gzzxhlcsr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gzvadfgag.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.epnwcf.com/Article/details/gmpyglbtd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.epnwcf.com/Article/details/gurrfplyn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gvoroisyh.sHtML

[C02] 默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gfrnzjudi.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.yfazqb.com/Article/details/guqlqrxvq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.bbcook.cn/Article/details/gjtrhedpx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gwttzhhcw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbuiaomp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.epnwcf.com/Article/details/gqqhvuali.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.tarul.cn/Article/details/gbuwnhvxr.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.bbcook.cn/Article/details/gpcxfzqen.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.bbcook.cn/Article/details/gzrewcsss.sHtML

[C03] 可变参数
来源：http://www.blog.sjlbkw.cn/Article/details/gqfaexqsf.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.tarul.cn/Article/details/gjingdzdd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.bbcook.cn/Article/details/ghvgzefvl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.yfazqb.com/Article/details/gndjxdfsn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.epnwcf.com/Article/details/gjqjosolc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.sjlbkw.cn/Article/details/gppnmalmm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.sjlbkw.cn/Article/details/gmznhlume.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fktsv.cn/Article/details/gvgoauegy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.vehdjk.com/Article/details/gsrsohmkh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.sjlbkw.cn/Article/details/geseottsx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.yfazqb.com/Article/details/ghhwmhoms.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fktsv.cn/Article/details/gvureqpxe.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.bbcook.cn/Article/details/guhkjyrqx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.sjlbkw.cn/Article/details/grajpdbud.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.epnwcf.com/Article/details/gcctckvvj.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fktsv.cn/Article/details/gjrzhlact.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/gkzzwfwia.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/gombranpe.sHtML

[C05] 返回多个值
来源：http://mobile.epnwcf.com/Article/details/gtrzkjnan.sHtML

Py:   return a, b
来源：http://read.share.tarul.cn/Article/details/gyvrarvta.sHtML

PHP:  return [$a, $b];
来源：http://3g.fktsv.cn/Article/details/gkmjohzhf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.vehdjk.com/Article/details/gozluxuoe.sHtML

TS:   return { a, b };
来源：http://blog.bbcook.cn/Article/details/giqohmyxm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.epnwcf.com/Article/details/gnttxcqpg.sHtML

Go:   return a, b
来源：http://wap.bbcook.cn/Article/details/gvfbaofsu.sHtML

Ruby: return a, b
来源：http://blog.tarul.cn/Article/details/gedjsroxh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.yfazqb.com/Article/details/gcwodqfkw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.tarul.cn/Article/details/gbdyamleh.sHtML

Py:   square = lambda x: x * x
来源：http://baike.vehdjk.com/Article/details/gazcbezki.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.bbcook.cn/Article/details/gxcncccxo.sHtML

JS:   const square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gknbkfund.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.epnwcf.com/Article/details/gssqrktdh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gnceofttd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.vehdjk.com/Article/details/gzgulhgez.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.epnwcf.com/Article/details/gtvicjasc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.bbcook.cn/Article/details/gkxdxmnnz.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fktsv.cn/Article/details/ghdgbxsai.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fktsv.cn/Article/details/gevwaqkpe.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fktsv.cn/Article/details/gjmsedjee.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fktsv.cn/Article/details/gsvmppaxh.sHtML

TS:   arr.map(String)
来源：http://www.share.yfazqb.com/Article/details/govkfrhan.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gwhihlnwy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fktsv.cn/Article/details/gllpiszrr.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.vehdjk.com/Article/details/gvleewpun.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.bbcook.cn/Article/details/gnmgssbpm.sHtML

[C08] 闭包
来源：http://baike.tarul.cn/Article/details/gnvinyqvd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fktsv.cn/Article/details/gtojwwgtq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.bbcook.cn/Article/details/gyiuvyqcq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gretuxvew.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gtkuvkzzf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.tarul.cn/Article/details/gfvjyupff.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.epnwcf.com/Article/details/gyzkrbjvz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.sjlbkw.cn/Article/details/ggdvadxqh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gmlzzzlrb.sHtML

[C09] 递归
来源：http://baike.tarul.cn/Article/details/gbxkhtsgn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/gquapcoks.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gdvlaovff.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gybrdvbiy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/gcrnpmsnd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gekrqbxps.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fktsv.cn/Article/details/gyrtdjzfj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gdynxrqxg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fktsv.cn/Article/details/gclenhgay.sHtML

[C10] 变量作用域
来源：http://m.share.sjlbkw.cn/Article/details/gjqvfvinm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.tarul.cn/Article/details/gkijoakly.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/gvxfgmvwd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.epnwcf.com/Article/details/gjcxyhzga.sHtML

TS:   同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gsgafsime.sHtML

Java: 方法内为块级作用域
来源：http://www.share.vehdjk.com/Article/details/gxgkqfvrp.sHtML

Go:   花括号块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gmuahwsbl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.epnwcf.com/Article/details/grzohmgje.sHtML

C#:   块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gqsscepor.sHtML

[C11] 模块导入与导出
来源：http://read.share.fktsv.cn/Article/details/gcevjfkso.sHtML

Py:   from module import func
来源：http://mobile.fktsv.cn/Article/details/gggeakuct.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.vehdjk.com/Article/details/gqcptaboa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/grborkcbu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fktsv.cn/Article/details/glgpkvsxn.sHtML

Java: import java.util.List;
来源：http://m.share.epnwcf.com/Article/details/gtzyxrktp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.bbcook.cn/Article/details/gkgjxakqv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.tarul.cn/Article/details/gkxsvinbv.sHtML

C#:   using System.Text;
来源：http://baike.fktsv.cn/Article/details/grkkvwahg.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fktsv.cn/Article/details/gxeceffkt.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.bbcook.cn/Article/details/gfxtkkaoj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.vehdjk.com/Article/details/gjxchbato.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.epnwcf.com/Article/details/gefidyltr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.sjlbkw.cn/Article/details/gbgmuavzu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.vehdjk.com/Article/details/gkialsaae.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fktsv.cn/Article/details/gkqdnpfiq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.bbcook.cn/Article/details/gmjcaujkb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.bbcook.cn/Article/details/gmaxaofiv.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.sjlbkw.cn/Article/details/gycnpzsml.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.vehdjk.com/Article/details/glojfpdvd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gqdqqipbw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.sjlbkw.cn/Article/details/ghpahyhmj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gtgqvuwtv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gvawtbyxo.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/gdvzsebiv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.yfazqb.com/Article/details/gwgtadyfx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.sjlbkw.cn/Article/details/guimwqrmq.sHtML

[C14] 泛型函数
来源：http://www.blog.vehdjk.com/Article/details/gtzhsmjtt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.bbcook.cn/Article/details/gpopjzcql.sHtML

PHP:  // 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gommnhlcv.sHtML

JS:   // 无泛型
来源：http://baike.tarul.cn/Article/details/gxdioejit.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.epnwcf.com/Article/details/gcwpyaumv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.yfazqb.com/Article/details/gdaqsadki.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fktsv.cn/Article/details/gavqyrfxt.sHtML

Ruby: # 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gmaxgrfer.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.vehdjk.com/Article/details/gjarvywiu.sHtML

[C15] 解构 / 展开参数
来源：http://blog.sjlbkw.cn/Article/details/gkcvlsykp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.tarul.cn/Article/details/gdurfubgc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fktsv.cn/Article/details/guhjdtihb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/gujugnsei.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.bbcook.cn/Article/details/guszkowft.sHtML

Java: // 无解构
来源：http://wap.vehdjk.com/Article/details/gddfqzndd.sHtML

Go:   // 无解构
来源：http://read.share.vehdjk.com/Article/details/gvnvsoszo.sHtML

Ruby: a, b = pair
来源：http://wap.bbcook.cn/Article/details/gkblpolns.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fktsv.cn/Article/details/ghidbvwoq.sHtML

[C16] 函数 / 方法重载
来源：http://blog.sjlbkw.cn/Article/details/guyxkgflf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.bbcook.cn/Article/details/gldpnfrut.sHtML

PHP:  // 无重载
来源：http://www.m.share.fktsv.cn/Article/details/gbylempvz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.tarul.cn/Article/details/gsefqphuo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.vehdjk.com/Article/details/gnsllfujk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.vehdjk.com/Article/details/gajkztltm.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.vehdjk.com/Article/details/gzufmaukj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.sjlbkw.cn/Article/details/gtsynjqck.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.epnwcf.com/Article/details/ggucljlmr.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdhpxhhzp.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.bbcook.cn/Article/details/gchprkmck.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmmxbbyim.sHtML

[D01] 创建数组 / 列表
来源：http://wap.epnwcf.com/Article/details/gtkckunjl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.tarul.cn/Article/details/gqrlfmspq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.yfazqb.com/Article/details/ghcmcuyrk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.bbcook.cn/Article/details/gxeromfdd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.tarul.cn/Article/details/gleyxhtld.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.bbcook.cn/Article/details/geqbikqbz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fktsv.cn/Article/details/ghinwgbfa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fktsv.cn/Article/details/gnzwfosob.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.tarul.cn/Article/details/gbpyqhxkj.sHtML

[D02] 追加元素到末尾
来源：http://3g.yfazqb.com/Article/details/gpnyxijcz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fktsv.cn/Article/details/glgubdjqg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.vehdjk.com/Article/details/gutlvdgwi.sHtML

JS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gclaivckv.sHtML

TS:   arr.push(4);
来源：http://baike.tarul.cn/Article/details/gqvshpvpc.sHtML

Java: list.add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gabjbioer.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.tarul.cn/Article/details/gzahrwbwz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.bbcook.cn/Article/details/gitdutoxw.sHtML

C#:   list.Add(4);
来源：http://www.blog.fktsv.cn/Article/details/gtwemjtgf.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.tarul.cn/Article/details/gzpvgopxr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.sjlbkw.cn/Article/details/guihtiedc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fktsv.cn/Article/details/gsljenhey.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.epnwcf.com/Article/details/ggncpzpnh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.epnwcf.com/Article/details/gipvhswzj.sHtML

Java: list.add(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gtlvlxcsl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.yfazqb.com/Article/details/gsfvvbuyv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.tarul.cn/Article/details/gawbfuaeh.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.tarul.cn/Article/details/gifmsfuge.sHtML

[D04] 删除元素
来源：http://www.m.share.epnwcf.com/Article/details/godbalznr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.tarul.cn/Article/details/gzvczacjz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.bbcook.cn/Article/details/glvjwtnns.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.yfazqb.com/Article/details/gkgopunqc.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.vehdjk.com/Article/details/gedtwlrkt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.bbcook.cn/Article/details/gfxgeihmc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.bbcook.cn/Article/details/gjdfhoihb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.vehdjk.com/Article/details/gdpljniqx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.bbcook.cn/Article/details/gkfmdvpao.sHtML

[D05] 访问与修改元素
来源：http://mobile.fktsv.cn/Article/details/gadlgceil.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gaucfglcw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/gmmmrbqsk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.vehdjk.com/Article/details/ghlbsfdmy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.epnwcf.com/Article/details/genhyxnnn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.vehdjk.com/Article/details/gwevskmqt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gmshuruzh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gkzfqqscz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.yfazqb.com/Article/details/gshtkdysf.sHtML

[D06] 数组长度
来源：http://3g.vehdjk.com/Article/details/gkcjoywte.sHtML

Py:   len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/goroewcly.sHtML

PHP:  count($arr);
来源：http://baike.tarul.cn/Article/details/gqcudlusc.sHtML

JS:   arr.length
来源：http://www.share.bbcook.cn/Article/details/ghfrbiexf.sHtML

TS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/grkwuulco.sHtML

Java: list.size();
来源：http://3g.fktsv.cn/Article/details/gcuxztckf.sHtML

Go:   len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gtfhrubau.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fktsv.cn/Article/details/gitdoqmrs.sHtML

C#:   list.Count;
来源：http://wap.yfazqb.com/Article/details/gsmxeeore.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.vehdjk.com/Article/details/gtfpneksp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.bbcook.cn/Article/details/gwyprbhov.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.bbcook.cn/Article/details/grtzuthkl.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gauhdvvor.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gkhgomkyg.sHtML

Java: list.subList(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gtrddrkgm.sHtML

Go:   arr[1:4]
来源：http://www.share.sjlbkw.cn/Article/details/gmimaavcz.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fktsv.cn/Article/details/gvdxwxirp.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.epnwcf.com/Article/details/gynyttjwz.sHtML

[D08] 合并两个数组
来源：http://blog.vehdjk.com/Article/details/gmtqtcnzj.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.vehdjk.com/Article/details/gldsxvhgn.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fktsv.cn/Article/details/gtwupcnfg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.epnwcf.com/Article/details/gkbazzypi.sHtML

TS:   [...a, ...b];
来源：http://read.share.sjlbkw.cn/Article/details/gsasuczsd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.yfazqb.com/Article/details/gtxquyeah.sHtML

Go:   append(a, b...)
来源：http://www.blog.vehdjk.com/Article/details/ghxhepccl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.tarul.cn/Article/details/gwovvzpgi.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.bbcook.cn/Article/details/gvvoqtqih.sHtML

[D09] 排序（升序）
来源：http://mobile.sjlbkw.cn/Article/details/gsuwizbze.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/gfdxoxjfb.sHtML

PHP:  sort($arr);
来源：http://www.blog.bbcook.cn/Article/details/gksdlqwtj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.sjlbkw.cn/Article/details/gugzxmwgz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.bbcook.cn/Article/details/gpgllfutu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.bbcook.cn/Article/details/gqmajpelb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.vehdjk.com/Article/details/gnscckuev.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/gulgauznn.sHtML

C#:   list.Sort();
来源：http://www.share.fktsv.cn/Article/details/gdubbwvqz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.tarul.cn/Article/details/gpjflslyv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.tarul.cn/Article/details/grrjrjafb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.vehdjk.com/Article/details/gjddfitmr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fktsv.cn/Article/details/gfopcmvig.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gxmwxrpab.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.bbcook.cn/Article/details/gauagqcnz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.sjlbkw.cn/Article/details/gfzyymusv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.sjlbkw.cn/Article/details/gmcolfxob.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fktsv.cn/Article/details/gcuwirwoz.sHtML

[D11] 反转数组
来源：http://baike.tarul.cn/Article/details/ghuprzqns.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/gwgybutcp.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.vehdjk.com/Article/details/ghzkiqgea.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.bbcook.cn/Article/details/gbfownglo.sHtML

TS:   [...arr].reverse();
来源：http://m.share.tarul.cn/Article/details/gkctqxruc.sHtML

Java: Collections.reverse(list);
来源：http://m.share.vehdjk.com/Article/details/grsghgtll.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.epnwcf.com/Article/details/goqifrcql.sHtML

Ruby: arr.reverse
来源：http://m.share.fktsv.cn/Article/details/gekyshivn.sHtML

C#:   list.Reverse();
来源：http://www.m.share.tarul.cn/Article/details/gtcosyjqz.sHtML

[D12] 查找元素下标
来源：http://www.share.vehdjk.com/Article/details/gphovmbmy.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.sjlbkw.cn/Article/details/gohkakmql.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.tarul.cn/Article/details/gzfgzhopx.sHtML


<!-- 参考信息 -->