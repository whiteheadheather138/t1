代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gxpfkwptj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.yfazqb.com/Article/details/gmmlamyby.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fktsv.cn/Article/details/gsyopdypg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fktsv.cn/Article/details/gwcnsflsk.sHtML

[B13] 判断是否为数字
来源：http://mobile.fktsv.cn/Article/details/ghpcutmmk.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.vehdjk.com/Article/details/gcdusmmnd.sHtML

PHP:  is_numeric($x)
来源：http://mobile.yfazqb.com/Article/details/gzrysckhq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.tarul.cn/Article/details/gjoxsmjdw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/giwkhpayy.sHtML

Java: x instanceof Number
来源：http://3g.bbcook.cn/Article/details/goepxljdm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.epnwcf.com/Article/details/gdfhuorvf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.sjlbkw.cn/Article/details/gijopwomz.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fktsv.cn/Article/details/gnagjeqyq.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.tarul.cn/Article/details/gpfjsaiba.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.sjlbkw.cn/Article/details/ghdjuzmxy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.sjlbkw.cn/Article/details/gqcjgfmsr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gwewvxljy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gqeknqgyq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.vehdjk.com/Article/details/gzuzcjjab.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.epnwcf.com/Article/details/gzdhztkms.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.tarul.cn/Article/details/gydkfxtkf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/grevnlhzb.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.vehdjk.com/Article/details/gozvqirap.sHtML

Py:   a and b or not c
来源：http://read.share.tarul.cn/Article/details/gdkijgxxa.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.yfazqb.com/Article/details/gdssncuex.sHtML

JS:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gytgknvdk.sHtML

TS:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gkacxntiw.sHtML

Java: a && b || !c
来源：http://read.share.fktsv.cn/Article/details/ggshmyokj.sHtML

Go:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gkdrjisdy.sHtML

Ruby: a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gdyaweklz.sHtML

C#:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gibsmzsle.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.vehdjk.com/Article/details/gqijzyxtl.sHtML

Py:   if not data: return
来源：http://3g.bbcook.cn/Article/details/grkfblvlm.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.vehdjk.com/Article/details/gklswzxsw.sHtML

JS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/gvrxyfjti.sHtML

TS:   if (!data) return;
来源：http://m.share.tarul.cn/Article/details/goilugmyt.sHtML

Java: if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/gpbpzbwvy.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.epnwcf.com/Article/details/gxzmjtkqu.sHtML

Ruby: return if data.nil?
来源：http://baike.epnwcf.com/Article/details/gqckkrlkr.sHtML

C#:   if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gegrldqjl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/govdqbxde.sHtML

C. 函数与作用域
来源：http://baike.tarul.cn/Article/details/gqyanjyqc.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/giefndavu.sHtML

[C01] 定义函数
来源：http://wap.bbcook.cn/Article/details/gcdjbqiib.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fktsv.cn/Article/details/gtdhvafur.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gulbmbzgy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gyhxpvxjf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gjsygsoui.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gwqnkylea.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.sjlbkw.cn/Article/details/gjbugmvsi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.yfazqb.com/Article/details/gqkqqnooa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gutunllyd.sHtML

[C02] 默认参数
来源：http://wap.bbcook.cn/Article/details/gccqyldoj.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.tarul.cn/Article/details/gzveuwhml.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.vehdjk.com/Article/details/gndwmzutv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gmdpapiqo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.vehdjk.com/Article/details/gdphazivn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.yfazqb.com/Article/details/gnusobmny.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.sjlbkw.cn/Article/details/gjsoscbwy.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fktsv.cn/Article/details/gommoqmjm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.bbcook.cn/Article/details/gktdzovnp.sHtML

[C03] 可变参数
来源：http://blog.epnwcf.com/Article/details/glckdqsnf.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.bbcook.cn/Article/details/gvbcsgyuz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.epnwcf.com/Article/details/gugtfqfkj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/gposxyjsx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/gupwndjdh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.tarul.cn/Article/details/glgriuxku.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.sjlbkw.cn/Article/details/gwxlpkyyx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.vehdjk.com/Article/details/gxrvbxols.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.yfazqb.com/Article/details/grqnfuzrd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.tarul.cn/Article/details/geitrrhut.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.bbcook.cn/Article/details/gnibfrlwp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.yfazqb.com/Article/details/gmkuarkkj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gdslctkip.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.sjlbkw.cn/Article/details/gyplljiqh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.vehdjk.com/Article/details/gzpljivtf.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.yfazqb.com/Article/details/gxfuvhesw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gjvtttbkk.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gkrtgcwii.sHtML

[C05] 返回多个值
来源：http://www.m.share.bbcook.cn/Article/details/gpouwrkxe.sHtML

Py:   return a, b
来源：http://3g.vehdjk.com/Article/details/gkcxcksje.sHtML

PHP:  return [$a, $b];
来源：http://3g.sjlbkw.cn/Article/details/gvibmdmvv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.sjlbkw.cn/Article/details/gmgewzaec.sHtML

TS:   return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gypnbfgyz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fktsv.cn/Article/details/gpvmpbqag.sHtML

Go:   return a, b
来源：http://mobile.bbcook.cn/Article/details/gvmlhutyo.sHtML

Ruby: return a, b
来源：http://mobile.bbcook.cn/Article/details/guaedivju.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.yfazqb.com/Article/details/gfmbrzilj.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fktsv.cn/Article/details/grvdjdfnl.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.tarul.cn/Article/details/gbdcnfrqx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.yfazqb.com/Article/details/gopzbkjjd.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.bbcook.cn/Article/details/gjlbxokcp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.bbcook.cn/Article/details/gnxxcdwot.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fktsv.cn/Article/details/gaeicbcaj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.vehdjk.com/Article/details/gngoqxzdr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fktsv.cn/Article/details/gececxvno.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.vehdjk.com/Article/details/gnimzqowl.sHtML

[C07] 把函数作为参数传入
来源：http://3g.vehdjk.com/Article/details/gytblbqjk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.sjlbkw.cn/Article/details/gfmnbrrzk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.epnwcf.com/Article/details/grxilbrno.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.bbcook.cn/Article/details/gictzpvea.sHtML

TS:   arr.map(String)
来源：http://www.blog.sjlbkw.cn/Article/details/gunjomxtp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.vehdjk.com/Article/details/gcufeesab.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.sjlbkw.cn/Article/details/gmrxhmljl.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fktsv.cn/Article/details/gupfwhgoc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.sjlbkw.cn/Article/details/gdtyrtagu.sHtML

[C08] 闭包
来源：http://mobile.bbcook.cn/Article/details/gouzpsduj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.sjlbkw.cn/Article/details/glnalbyur.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.vehdjk.com/Article/details/gahgagxcb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gbqupmeca.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gkthxmlce.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.tarul.cn/Article/details/gmngioeqr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fktsv.cn/Article/details/gojkjnarv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.tarul.cn/Article/details/gialaipay.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gegibiibi.sHtML

[C09] 递归
来源：http://m.share.vehdjk.com/Article/details/ggavswfhe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fktsv.cn/Article/details/gphjehymi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.tarul.cn/Article/details/ghjjezins.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fktsv.cn/Article/details/grkggfhmy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gczpcantu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.tarul.cn/Article/details/gfszoodap.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.tarul.cn/Article/details/glwupjsjg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/gbatsciwl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.epnwcf.com/Article/details/glgfkonyu.sHtML

[C10] 变量作用域
来源：http://m.share.vehdjk.com/Article/details/grjgomghs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.bbcook.cn/Article/details/glxvkhrxd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.bbcook.cn/Article/details/gjuplehnr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.yfazqb.com/Article/details/ghywrcunf.sHtML

TS:   同 JS
来源：http://wap.yfazqb.com/Article/details/gkuybonbv.sHtML

Java: 方法内为块级作用域
来源：http://www.share.vehdjk.com/Article/details/gbmxfovcu.sHtML

Go:   花括号块级作用域
来源：http://read.share.fktsv.cn/Article/details/gzsyzmsvp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.tarul.cn/Article/details/gwwhnsaml.sHtML

C#:   块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/grhbhemjh.sHtML

[C11] 模块导入与导出
来源：http://m.share.tarul.cn/Article/details/gmvqgonnc.sHtML

Py:   from module import func
来源：http://read.share.vehdjk.com/Article/details/gvpiuogbo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.vehdjk.com/Article/details/gsujmfbzb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fktsv.cn/Article/details/gaegmqfsn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.tarul.cn/Article/details/gzscieuer.sHtML

Java: import java.util.List;
来源：http://read.share.yfazqb.com/Article/details/gvkakqpkz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.vehdjk.com/Article/details/gwcdktjpm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fktsv.cn/Article/details/gcwyrbrod.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/geyuzulhb.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fktsv.cn/Article/details/gdbkgllmy.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.yfazqb.com/Article/details/gwynfaxwy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.sjlbkw.cn/Article/details/goyutskjn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/gkjvytuat.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.epnwcf.com/Article/details/gujbvwisi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.vehdjk.com/Article/details/guplsjtww.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.epnwcf.com/Article/details/gnfgcotdz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.epnwcf.com/Article/details/ggsffyjzb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.tarul.cn/Article/details/gmxlpevtx.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.bbcook.cn/Article/details/gdvrwihng.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.yfazqb.com/Article/details/grqmdydmz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gxfyytves.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.tarul.cn/Article/details/gvuneqthu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gzxjsinsv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/geildqcnp.sHtML

Go:   func add(a, b int) int
来源：http://read.share.bbcook.cn/Article/details/gakeknamb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.bbcook.cn/Article/details/ghnlrslxl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.vehdjk.com/Article/details/goloegqjj.sHtML

[C14] 泛型函数
来源：http://3g.sjlbkw.cn/Article/details/gyxreztfg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.yfazqb.com/Article/details/gppybdghc.sHtML

PHP:  // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gkpwkojnz.sHtML

JS:   // 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gelqbsvtr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.epnwcf.com/Article/details/gcsfcgfrz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fktsv.cn/Article/details/ggehezago.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.yfazqb.com/Article/details/gnppvbqzp.sHtML

Ruby: # 无泛型
来源：http://wap.bbcook.cn/Article/details/gffezcosp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.yfazqb.com/Article/details/gtkybzjft.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.bbcook.cn/Article/details/glmfwdhrk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.yfazqb.com/Article/details/gsoyzmcgo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.vehdjk.com/Article/details/gpntewekd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gndrxivlm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fktsv.cn/Article/details/getujgnqb.sHtML

Java: // 无解构
来源：http://www.share.epnwcf.com/Article/details/gsndxfaqn.sHtML

Go:   // 无解构
来源：http://www.blog.tarul.cn/Article/details/gernseqid.sHtML

Ruby: a, b = pair
来源：http://mobile.epnwcf.com/Article/details/gmupphuyw.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fktsv.cn/Article/details/grsxwcspp.sHtML

[C16] 函数 / 方法重载
来源：http://wap.epnwcf.com/Article/details/gvlczhenm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.tarul.cn/Article/details/ggorijsuj.sHtML

PHP:  // 无重载
来源：http://www.m.share.yfazqb.com/Article/details/gtfsgbzdo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.yfazqb.com/Article/details/geyggfmro.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.sjlbkw.cn/Article/details/gxdydqrzn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.yfazqb.com/Article/details/gniwljntt.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.tarul.cn/Article/details/gbduazjyz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.sjlbkw.cn/Article/details/gxueexpvw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.bbcook.cn/Article/details/gmznafdja.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gyndudrrd.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.vehdjk.com/Article/details/geetyevjg.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzwiwhmog.sHtML

[D01] 创建数组 / 列表
来源：http://3g.epnwcf.com/Article/details/gdttgqcwk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.epnwcf.com/Article/details/gdahkaqvs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.tarul.cn/Article/details/gtkcqihzv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.bbcook.cn/Article/details/glbelvzpv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fktsv.cn/Article/details/gkmgkzzyc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.vehdjk.com/Article/details/gpjvewvtm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fktsv.cn/Article/details/gyotdvlzo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.vehdjk.com/Article/details/geykwqsuy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.vehdjk.com/Article/details/glzsitajb.sHtML

[D02] 追加元素到末尾
来源：http://www.share.epnwcf.com/Article/details/gwyzqpiev.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.vehdjk.com/Article/details/gbjvqrdks.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.bbcook.cn/Article/details/gvtcanioc.sHtML

JS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/gbrnbhbbc.sHtML

TS:   arr.push(4);
来源：http://www.share.epnwcf.com/Article/details/ghzofbigu.sHtML

Java: list.add(4);
来源：http://read.share.tarul.cn/Article/details/gsacdxhvb.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.yfazqb.com/Article/details/gsylhzjex.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.vehdjk.com/Article/details/grteeabtv.sHtML

C#:   list.Add(4);
来源：http://www.blog.vehdjk.com/Article/details/gtiarkobd.sHtML

[D03] 在指定位置插入元素
来源：http://baike.sjlbkw.cn/Article/details/gljtfjtqp.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gtsgblzhz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.sjlbkw.cn/Article/details/gwdreejwj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.epnwcf.com/Article/details/gfbejbwce.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gotpzxlts.sHtML

Java: list.add(0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gdzaanhtc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.epnwcf.com/Article/details/getwjsmgr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.sjlbkw.cn/Article/details/gmlsdggrc.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.yfazqb.com/Article/details/gmlmrjhks.sHtML

[D04] 删除元素
来源：http://www.blog.fktsv.cn/Article/details/gmarfaeiq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.vehdjk.com/Article/details/gnmmcdept.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fktsv.cn/Article/details/gmyicnwko.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fktsv.cn/Article/details/gsgfyrvjl.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.sjlbkw.cn/Article/details/gycjrzvil.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.vehdjk.com/Article/details/grkorxmsn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.yfazqb.com/Article/details/gvrratiuh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.sjlbkw.cn/Article/details/gjzbhwvmw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fktsv.cn/Article/details/guxerfqdb.sHtML

[D05] 访问与修改元素
来源：http://3g.bbcook.cn/Article/details/gsoxyauft.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/gokazvjba.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gwbawqfis.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.epnwcf.com/Article/details/gcfirjmna.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.yfazqb.com/Article/details/gjlotufdv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.sjlbkw.cn/Article/details/gntoytvsd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/germxscfg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/gtsiljjcy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gymctrgdd.sHtML

[D06] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjwusptj.sHtML

Py:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/guilsbxfs.sHtML

PHP:  count($arr);
来源：http://mobile.fktsv.cn/Article/details/gnfywysdw.sHtML

JS:   arr.length
来源：http://3g.fktsv.cn/Article/details/gwoljxfzg.sHtML

TS:   arr.length
来源：http://www.m.share.epnwcf.com/Article/details/guqdajptl.sHtML

Java: list.size();
来源：http://mobile.epnwcf.com/Article/details/gmhcjoikg.sHtML

Go:   len(arr)
来源：http://m.share.vehdjk.com/Article/details/gudtysjwl.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.sjlbkw.cn/Article/details/gzfloqfrx.sHtML

C#:   list.Count;
来源：http://3g.sjlbkw.cn/Article/details/gbiokopoj.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.epnwcf.com/Article/details/gyukicbwo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.vehdjk.com/Article/details/gpqxmnlzc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fktsv.cn/Article/details/ggxwvbtol.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.tarul.cn/Article/details/gaxhgeses.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gzjwzjoux.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fktsv.cn/Article/details/gaaecrcxp.sHtML

Go:   arr[1:4]
来源：http://m.share.tarul.cn/Article/details/gdjnddamj.sHtML

Ruby: arr[1, 3]
来源：http://blog.vehdjk.com/Article/details/gvrvtvyfd.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.tarul.cn/Article/details/gqzjpxpan.sHtML

[D08] 合并两个数组
来源：http://www.share.tarul.cn/Article/details/gyaawiyhy.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fktsv.cn/Article/details/grzonapcg.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.tarul.cn/Article/details/gxjkknkqc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.tarul.cn/Article/details/ggoexzwok.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.epnwcf.com/Article/details/gwzcdcrig.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.vehdjk.com/Article/details/gbwamlfut.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fktsv.cn/Article/details/gsktqmpva.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.vehdjk.com/Article/details/gclkrfpbb.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.vehdjk.com/Article/details/glbnyaehd.sHtML

[D09] 排序（升序）
来源：http://wap.epnwcf.com/Article/details/gxcowwyei.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.sjlbkw.cn/Article/details/gleltbohs.sHtML

PHP:  sort($arr);
来源：http://read.share.fktsv.cn/Article/details/gujjgwnse.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/gjtzsvwgm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.epnwcf.com/Article/details/gsquqpofu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.bbcook.cn/Article/details/gzvbmshce.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gsbhdwfwx.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gxbvsqsbp.sHtML

C#:   list.Sort();
来源：http://read.share.vehdjk.com/Article/details/girjndzfr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.sjlbkw.cn/Article/details/gfuafltjz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.vehdjk.com/Article/details/gvkycpdio.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.bbcook.cn/Article/details/gdjadevfi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.vehdjk.com/Article/details/gzrvnfcrv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.sjlbkw.cn/Article/details/gozobkiaa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.epnwcf.com/Article/details/gwgsmopyv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.yfazqb.com/Article/details/gtckcssco.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.tarul.cn/Article/details/gzregvhgh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.tarul.cn/Article/details/gxbtjafrc.sHtML

[D11] 反转数组
来源：http://baike.epnwcf.com/Article/details/gkpbmjhqr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.yfazqb.com/Article/details/gyyawvpbm.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/gdmluqhpu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.bbcook.cn/Article/details/grzjjithc.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fktsv.cn/Article/details/gqpalrwju.sHtML

Java: Collections.reverse(list);
来源：http://3g.yfazqb.com/Article/details/gtbdeglvn.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.sjlbkw.cn/Article/details/guqnwgnfn.sHtML

Ruby: arr.reverse
来源：http://3g.tarul.cn/Article/details/goefanxnd.sHtML

C#:   list.Reverse();
来源：http://3g.fktsv.cn/Article/details/gpdmcqsbq.sHtML

[D12] 查找元素下标
来源：http://www.share.epnwcf.com/Article/details/grzinigqy.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.tarul.cn/Article/details/gpqeeokvs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.yfazqb.com/Article/details/gzkiyagrm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.epnwcf.com/Article/details/guhveqiqe.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.vehdjk.com/Article/details/gtegwpgqk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.bbcook.cn/Article/details/gqjlnpypu.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.tarul.cn/Article/details/ggzkgattt.sHtML

Ruby: arr.index(x)
来源：http://read.share.epnwcf.com/Article/details/gnflkxyht.sHtML

C#:   list.IndexOf(x);
来源：http://blog.sjlbkw.cn/Article/details/gziyrdixa.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.tarul.cn/Article/details/gezouoqzg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fktsv.cn/Article/details/gnjnvisfz.sHtML


<!-- 参考信息 -->