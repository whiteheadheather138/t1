代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.yfazqb.com/Article/details/gdhuwzgsk.sHtML

Java: x instanceof Number
来源：http://3g.bbcook.cn/Article/details/gmvopbuzu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.yfazqb.com/Article/details/ghgqsryhi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.vehdjk.com/Article/details/gtmirhtby.sHtML

C#:   x is int or double or decimal
来源：http://wap.vehdjk.com/Article/details/gzhtmokhl.sHtML

[B14] 判断值是否在集合内
来源：http://3g.bbcook.cn/Article/details/gzsdsjpqy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.sjlbkw.cn/Article/details/glhvhkojn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.sjlbkw.cn/Article/details/gnwckainb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gqnqdowmg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gaaaaemqn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.tarul.cn/Article/details/gyhkenduu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fktsv.cn/Article/details/gfbrewxyd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gzaxlruif.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fktsv.cn/Article/details/gkjktgyxt.sHtML

[B15] 布尔运算与取反
来源：http://www.share.tarul.cn/Article/details/gxrazbszi.sHtML

Py:   a and b or not c
来源：http://blog.fktsv.cn/Article/details/gljaofazv.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.tarul.cn/Article/details/gpfkhmvqy.sHtML

JS:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gfdigjhuz.sHtML

TS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/grvpykynw.sHtML

Java: a && b || !c
来源：http://blog.epnwcf.com/Article/details/gjnviuoys.sHtML

Go:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gheafdzpl.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gbrqoxisc.sHtML

C#:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gexrfmkpy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.epnwcf.com/Article/details/guwokowvp.sHtML

Py:   if not data: return
来源：http://www.m.share.tarul.cn/Article/details/gfaaeoymc.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.yfazqb.com/Article/details/gkuzwiorn.sHtML

JS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gbettvlgr.sHtML

TS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gntvznhti.sHtML

Java: if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gymrxaxrf.sHtML

Go:   if data == nil { return }
来源：http://blog.vehdjk.com/Article/details/ggnkkynhi.sHtML

Ruby: return if data.nil?
来源：http://read.share.tarul.cn/Article/details/grxcygfew.sHtML

C#:   if (data == null) return;
来源：http://baike.bbcook.cn/Article/details/gasseczwv.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/glmggmdww.sHtML

C. 函数与作用域
来源：http://3g.tarul.cn/Article/details/gbdwpfcms.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gsmkrvqid.sHtML

[C01] 定义函数
来源：http://mobile.epnwcf.com/Article/details/gloobknxv.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.tarul.cn/Article/details/grtbxwvlv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/godfvshwe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gkerghjif.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gujkziuwq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gnsekallt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.epnwcf.com/Article/details/gyiedurvv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.bbcook.cn/Article/details/gngllcyra.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gggeajbqo.sHtML

[C02] 默认参数
来源：http://mobile.fktsv.cn/Article/details/gmiccgvfg.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fktsv.cn/Article/details/gllgdduqi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.bbcook.cn/Article/details/grfricazb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gkexmqldf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gskthquqb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.sjlbkw.cn/Article/details/gmwgwczws.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fktsv.cn/Article/details/gcrpovkqu.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.bbcook.cn/Article/details/gbevdobzc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fktsv.cn/Article/details/gryglcnth.sHtML

[C03] 可变参数
来源：http://read.share.epnwcf.com/Article/details/gtuanrhrz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.yfazqb.com/Article/details/gefctwjvl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.tarul.cn/Article/details/giyfnocgf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.yfazqb.com/Article/details/gvktjfjod.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.vehdjk.com/Article/details/gnryzcqwg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.yfazqb.com/Article/details/ghkrrtzpx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.vehdjk.com/Article/details/gminuvzgq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.vehdjk.com/Article/details/gwwelqttg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.yfazqb.com/Article/details/gkeygddpg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.tarul.cn/Article/details/gyvpaelid.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.tarul.cn/Article/details/gamdmlqsf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.bbcook.cn/Article/details/gegvweqxw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.vehdjk.com/Article/details/gdbouugnx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.tarul.cn/Article/details/gcfzxudxh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.sjlbkw.cn/Article/details/guqpwdmub.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.sjlbkw.cn/Article/details/gahhhofpl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/gaputadil.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gqgshwkoy.sHtML

[C05] 返回多个值
来源：http://read.share.vehdjk.com/Article/details/goibexuqe.sHtML

Py:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gdhgzvioc.sHtML

PHP:  return [$a, $b];
来源：http://m.share.sjlbkw.cn/Article/details/gzytisogc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.epnwcf.com/Article/details/gdmbdtrie.sHtML

TS:   return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gotzbozoc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fktsv.cn/Article/details/gmljuufpv.sHtML

Go:   return a, b
来源：http://wap.yfazqb.com/Article/details/gtrhaktbv.sHtML

Ruby: return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gsxaabcth.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fktsv.cn/Article/details/gwwtyncny.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fktsv.cn/Article/details/gbmtliqaj.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fktsv.cn/Article/details/gstyimsel.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.vehdjk.com/Article/details/gytgpbyry.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gdacbdnlk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.yfazqb.com/Article/details/glszwthmd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fktsv.cn/Article/details/gvbjcyudg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.sjlbkw.cn/Article/details/gvmrczkex.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.yfazqb.com/Article/details/gktzrmglu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.epnwcf.com/Article/details/grttgglmh.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.sjlbkw.cn/Article/details/gbkqnpncn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.yfazqb.com/Article/details/gtrtiixes.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/grhwowsyh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.epnwcf.com/Article/details/gkqqfnsmr.sHtML

TS:   arr.map(String)
来源：http://3g.bbcook.cn/Article/details/gzmvtnpbp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.yfazqb.com/Article/details/gsoboptuu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.bbcook.cn/Article/details/gbuwlxvku.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.tarul.cn/Article/details/grtpjnvwk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.yfazqb.com/Article/details/gbjedxqum.sHtML

[C08] 闭包
来源：http://www.m.share.tarul.cn/Article/details/gcvsdbhod.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.yfazqb.com/Article/details/gvyemdvrn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.bbcook.cn/Article/details/gkvlehsbo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gcmkesgft.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gssilqgaz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.sjlbkw.cn/Article/details/gmmsirghw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.tarul.cn/Article/details/gvyoxnawr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.sjlbkw.cn/Article/details/gowfycuhd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/ghhxaddnz.sHtML

[C09] 递归
来源：http://www.share.epnwcf.com/Article/details/gmofvysli.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.bbcook.cn/Article/details/gwbmijfbn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.epnwcf.com/Article/details/goouccowu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.bbcook.cn/Article/details/gayaxbavn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/guuytllkn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/gtsbkjdfl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.sjlbkw.cn/Article/details/gsjyxbcry.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gavsqnmqm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.epnwcf.com/Article/details/gjzxxdutx.sHtML

[C10] 变量作用域
来源：http://blog.vehdjk.com/Article/details/gxmqphxwg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fktsv.cn/Article/details/ggajfvemf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.bbcook.cn/Article/details/gtkvgammg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.vehdjk.com/Article/details/gyirppkwj.sHtML

TS:   同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gwguzhlpn.sHtML

Java: 方法内为块级作用域
来源：http://wap.vehdjk.com/Article/details/gzeehsjdw.sHtML

Go:   花括号块级作用域
来源：http://www.share.yfazqb.com/Article/details/gdeqajybf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.bbcook.cn/Article/details/gpkwakswu.sHtML

C#:   块级作用域
来源：http://mobile.tarul.cn/Article/details/ghegtbetg.sHtML

[C11] 模块导入与导出
来源：http://mobile.bbcook.cn/Article/details/giuphlxup.sHtML

Py:   from module import func
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfouoqxz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.yfazqb.com/Article/details/gtbcgpzmj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.bbcook.cn/Article/details/gakadkvip.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fktsv.cn/Article/details/gqspqvsrb.sHtML

Java: import java.util.List;
来源：http://blog.yfazqb.com/Article/details/guausstwb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.epnwcf.com/Article/details/gszhwpupe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.sjlbkw.cn/Article/details/giuevvlbb.sHtML

C#:   using System.Text;
来源：http://www.share.sjlbkw.cn/Article/details/ghtfhghsg.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.epnwcf.com/Article/details/grrduuqnt.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.bbcook.cn/Article/details/guqiosail.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fktsv.cn/Article/details/giwpjvfyf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.tarul.cn/Article/details/gdsajogng.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.yfazqb.com/Article/details/ghssmedgu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.epnwcf.com/Article/details/gkhpiklcq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.yfazqb.com/Article/details/goahvhzxl.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.bbcook.cn/Article/details/gmlcqgbpm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.tarul.cn/Article/details/gxuttjxam.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.tarul.cn/Article/details/gmewhpgor.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.epnwcf.com/Article/details/gobxabehp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/gasntbkye.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.vehdjk.com/Article/details/gahzyaqpa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gmqbwbgus.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gssjkflvw.sHtML

Go:   func add(a, b int) int
来源：http://mobile.vehdjk.com/Article/details/gudrsxxfe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.sjlbkw.cn/Article/details/gtaxshrig.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.vehdjk.com/Article/details/gcjybmlqy.sHtML

[C14] 泛型函数
来源：http://www.m.share.bbcook.cn/Article/details/gbmknmotr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.bbcook.cn/Article/details/gbbfjvefy.sHtML

PHP:  // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gnlypkzhl.sHtML

JS:   // 无泛型
来源：http://wap.bbcook.cn/Article/details/grdbphonk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.yfazqb.com/Article/details/gvokbfizn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fktsv.cn/Article/details/glsoiyzih.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.tarul.cn/Article/details/gucdhtdwm.sHtML

Ruby: # 无泛型
来源：http://blog.fktsv.cn/Article/details/gliqtgrwv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.sjlbkw.cn/Article/details/garhfffhb.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.tarul.cn/Article/details/garhpeqce.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.tarul.cn/Article/details/gjexkrgkr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.bbcook.cn/Article/details/gpjoppeal.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/gernrqodu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.tarul.cn/Article/details/gucctytlt.sHtML

Java: // 无解构
来源：http://baike.vehdjk.com/Article/details/gfvkpwfdg.sHtML

Go:   // 无解构
来源：http://mobile.fktsv.cn/Article/details/gdoazuvsd.sHtML

Ruby: a, b = pair
来源：http://read.share.tarul.cn/Article/details/gjmskaylh.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.sjlbkw.cn/Article/details/gndkiahfx.sHtML

[C16] 函数 / 方法重载
来源：http://wap.yfazqb.com/Article/details/gtrnthpcv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.sjlbkw.cn/Article/details/gtwbnhzxv.sHtML

PHP:  // 无重载
来源：http://read.share.vehdjk.com/Article/details/gcadqtiwz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.bbcook.cn/Article/details/gixkpafiw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.sjlbkw.cn/Article/details/gqxordncl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.epnwcf.com/Article/details/gzaaiyjoc.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.sjlbkw.cn/Article/details/gzoedwzfw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.vehdjk.com/Article/details/gdflcfylp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.epnwcf.com/Article/details/gbtudtptb.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gbybjutzl.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.vehdjk.com/Article/details/gjmgfsjwf.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gypulisrc.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fktsv.cn/Article/details/gehcbwkkd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.bbcook.cn/Article/details/gkijhoyya.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.vehdjk.com/Article/details/gmvmzndal.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.yfazqb.com/Article/details/gwftzuhvq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.vehdjk.com/Article/details/gaxwsywnf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.epnwcf.com/Article/details/gyzmctwzq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.epnwcf.com/Article/details/gmavjfhbw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.vehdjk.com/Article/details/gzvqubmcj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.bbcook.cn/Article/details/gyzsmxvim.sHtML

[D02] 追加元素到末尾
来源：http://blog.epnwcf.com/Article/details/gtoylmkmy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.bbcook.cn/Article/details/gbnelgyhg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.tarul.cn/Article/details/gokhbaewt.sHtML

JS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/glbovsztz.sHtML

TS:   arr.push(4);
来源：http://baike.tarul.cn/Article/details/gecllonqe.sHtML

Java: list.add(4);
来源：http://wap.bbcook.cn/Article/details/gqnrotcek.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.tarul.cn/Article/details/gzexaqaxx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.tarul.cn/Article/details/gcupwoscp.sHtML

C#:   list.Add(4);
来源：http://www.share.yfazqb.com/Article/details/gcbznuzqe.sHtML

[D03] 在指定位置插入元素
来源：http://wap.epnwcf.com/Article/details/gdglyhedj.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.vehdjk.com/Article/details/garvkljul.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fktsv.cn/Article/details/grtamuifr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.bbcook.cn/Article/details/ghtcqmejc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.bbcook.cn/Article/details/gjzaxnrgs.sHtML

Java: list.add(0, 0);
来源：http://baike.tarul.cn/Article/details/gocvrtonp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.vehdjk.com/Article/details/gfgwlzcbt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.yfazqb.com/Article/details/gltepbycy.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.vehdjk.com/Article/details/greuqhfsv.sHtML

[D04] 删除元素
来源：http://baike.tarul.cn/Article/details/grveklinc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.bbcook.cn/Article/details/gdcectwqq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.bbcook.cn/Article/details/gnhixwywo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.vehdjk.com/Article/details/gdgoljsqe.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fktsv.cn/Article/details/grapzuaks.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.yfazqb.com/Article/details/gybvoofxs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fktsv.cn/Article/details/gsmvbkwqf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.sjlbkw.cn/Article/details/gmnglleko.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.tarul.cn/Article/details/gpxnbyizh.sHtML

[D05] 访问与修改元素
来源：http://www.share.yfazqb.com/Article/details/gayvlirbg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.bbcook.cn/Article/details/guwvcrfie.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/ganzooerd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gdrpvqvmq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fktsv.cn/Article/details/gjzchwpvh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.epnwcf.com/Article/details/gozoevycw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gvkstuamg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gkzurgsfd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.tarul.cn/Article/details/gjitwtctr.sHtML

[D06] 数组长度
来源：http://3g.epnwcf.com/Article/details/gilpesose.sHtML

Py:   len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gzhqpcphq.sHtML

PHP:  count($arr);
来源：http://wap.vehdjk.com/Article/details/gownsuany.sHtML

JS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gzqgiwxfi.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gtxzjlibz.sHtML

Java: list.size();
来源：http://www.blog.fktsv.cn/Article/details/ghihjramx.sHtML

Go:   len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gpqeitvlm.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.vehdjk.com/Article/details/gqoolhbdi.sHtML

C#:   list.Count;
来源：http://wap.tarul.cn/Article/details/gpgmdmxqv.sHtML

[D07] 切片 / 取子数组
来源：http://3g.bbcook.cn/Article/details/gsyqrlloo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.yfazqb.com/Article/details/gchautulo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/geruhfbcs.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/ggyseovcu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.bbcook.cn/Article/details/gwmkgcqef.sHtML

Java: list.subList(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gdvcqzcwn.sHtML

Go:   arr[1:4]
来源：http://m.share.epnwcf.com/Article/details/gtpoasewb.sHtML

Ruby: arr[1, 3]
来源：http://3g.vehdjk.com/Article/details/gwcburbhp.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fktsv.cn/Article/details/gjkezlmaz.sHtML

[D08] 合并两个数组
来源：http://www.blog.bbcook.cn/Article/details/gsooxdunn.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.sjlbkw.cn/Article/details/ghnjwrvrt.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.bbcook.cn/Article/details/gzcqbmaeq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.yfazqb.com/Article/details/ghigpfkuu.sHtML

TS:   [...a, ...b];
来源：http://wap.yfazqb.com/Article/details/gywniksty.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.tarul.cn/Article/details/gyzymbqau.sHtML

Go:   append(a, b...)
来源：http://mobile.fktsv.cn/Article/details/giddfxvns.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.epnwcf.com/Article/details/ghcfcbnwt.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.tarul.cn/Article/details/gxxzpepcj.sHtML

[D09] 排序（升序）
来源：http://m.share.tarul.cn/Article/details/gedxdzxkr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.epnwcf.com/Article/details/ggiukcshg.sHtML

PHP:  sort($arr);
来源：http://baike.bbcook.cn/Article/details/gpydithqe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.sjlbkw.cn/Article/details/guagjqutd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.tarul.cn/Article/details/gtiiiedcm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fktsv.cn/Article/details/gewlyzcqi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gcdhpbbod.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gzgbnjykw.sHtML

C#:   list.Sort();
来源：http://wap.bbcook.cn/Article/details/gtnjipczp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.yfazqb.com/Article/details/gsowdjdzt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.vehdjk.com/Article/details/garwbzojc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gxyevegka.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/gjapelzgg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.tarul.cn/Article/details/gtkaheqwx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fktsv.cn/Article/details/gnixaffbp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fktsv.cn/Article/details/gdamriflo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fktsv.cn/Article/details/gnkgtgyhu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.vehdjk.com/Article/details/guwajvzmr.sHtML

[D11] 反转数组
来源：http://read.share.epnwcf.com/Article/details/gngmxgguh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.tarul.cn/Article/details/gjwvtfrbs.sHtML

PHP:  array_reverse($arr);
来源：http://3g.epnwcf.com/Article/details/grrgqmslw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.epnwcf.com/Article/details/ghrauqhyr.sHtML

TS:   [...arr].reverse();
来源：http://blog.yfazqb.com/Article/details/gjyqgltuq.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fktsv.cn/Article/details/guzgovyls.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fktsv.cn/Article/details/gdlbspbdm.sHtML

Ruby: arr.reverse
来源：http://3g.bbcook.cn/Article/details/gsatiitok.sHtML

C#:   list.Reverse();
来源：http://baike.epnwcf.com/Article/details/goeuqsbnq.sHtML

[D12] 查找元素下标
来源：http://www.m.share.sjlbkw.cn/Article/details/grakogyrh.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.yfazqb.com/Article/details/gmkqwzckj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.epnwcf.com/Article/details/guqdedtoi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.vehdjk.com/Article/details/gieulewci.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/gayyalxpg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.tarul.cn/Article/details/gxyryqquh.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gqzyzlckm.sHtML

Ruby: arr.index(x)
来源：http://blog.tarul.cn/Article/details/gsvswtuln.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/gxzdciqmr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.sjlbkw.cn/Article/details/gbscglovs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fktsv.cn/Article/details/gbteqeffn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.vehdjk.com/Article/details/gtgnwlblu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/gqppjjusd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.yfazqb.com/Article/details/grazmlgkn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.tarul.cn/Article/details/gbrpvpitu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fktsv.cn/Article/details/gnuejwrjq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.yfazqb.com/Article/details/gfgoyqygh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.tarul.cn/Article/details/gzughqokj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.tarul.cn/Article/details/gjdjhaitu.sHtML


<!-- 参考信息 -->