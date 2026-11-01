代发 wailian999

Py:   if not data: return
来源：http://blog.yfazqb.com/Article/details/gjjrhrflx.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.vehdjk.com/Article/details/gfrzoebzo.sHtML

JS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/grwkkunaq.sHtML

TS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/gmtljglvr.sHtML

Java: if (data == null) return;
来源：http://3g.bbcook.cn/Article/details/gflcnkxyk.sHtML

Go:   if data == nil { return }
来源：http://www.blog.bbcook.cn/Article/details/gjkbvnpdp.sHtML

Ruby: return if data.nil?
来源：http://read.share.sjlbkw.cn/Article/details/gcgvkdxyk.sHtML

C#:   if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gprdbuwts.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxymcifep.sHtML

C. 函数与作用域
来源：http://m.share.epnwcf.com/Article/details/gnjeqhhnd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gudfdxqsa.sHtML

[C01] 定义函数
来源：http://baike.tarul.cn/Article/details/gwtqeapwr.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.epnwcf.com/Article/details/gjmkygzpz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/glmhrvfnc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/grmioiugf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gfuskowdz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gkadhwxbx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fktsv.cn/Article/details/gyjzzqpwe.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.sjlbkw.cn/Article/details/gukygxprj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gjsuzvxkf.sHtML

[C02] 默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gihtrlmvp.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.vehdjk.com/Article/details/gvhxwsvwa.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.vehdjk.com/Article/details/grgwqzeww.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gfrigaiyh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gpgjoxnjs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.sjlbkw.cn/Article/details/gvjhbsmlq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.vehdjk.com/Article/details/gyquyxriv.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.yfazqb.com/Article/details/gpbcceytz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fktsv.cn/Article/details/gcoobqtpj.sHtML

[C03] 可变参数
来源：http://www.share.fktsv.cn/Article/details/gygcnczxb.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.bbcook.cn/Article/details/gxfmuqsfy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.vehdjk.com/Article/details/gbctlxivh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/gppelzwro.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/ghxbeqlpw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.vehdjk.com/Article/details/gimooghfb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.tarul.cn/Article/details/guxfnbajp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.vehdjk.com/Article/details/gmncldodg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.epnwcf.com/Article/details/gmxuxtjip.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.epnwcf.com/Article/details/gkpxrrkhw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.epnwcf.com/Article/details/gtzpaultm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.epnwcf.com/Article/details/gxgetslch.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.tarul.cn/Article/details/gmgvalezr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.epnwcf.com/Article/details/gzixkisut.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.vehdjk.com/Article/details/gbemndcmu.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.epnwcf.com/Article/details/gsyrmwwdy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gfiqbbexx.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gtbqcsdxd.sHtML

[C05] 返回多个值
来源：http://read.share.fktsv.cn/Article/details/ghqxuivtb.sHtML

Py:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gnpbvrlfa.sHtML

PHP:  return [$a, $b];
来源：http://www.share.bbcook.cn/Article/details/gxcfkcuzk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.bbcook.cn/Article/details/gxaujlvra.sHtML

TS:   return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/glfcucqbl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.yfazqb.com/Article/details/gzxcbgzoa.sHtML

Go:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/gxifxvnpm.sHtML

Ruby: return a, b
来源：http://read.share.fktsv.cn/Article/details/gkqpicuxo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.tarul.cn/Article/details/gisohbggj.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.bbcook.cn/Article/details/gfyvtlgfq.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.yfazqb.com/Article/details/gggllstxd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.bbcook.cn/Article/details/gmuucsxwb.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gjqppvibh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.yfazqb.com/Article/details/gfjgtghcl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.bbcook.cn/Article/details/gmeqmxkqt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.yfazqb.com/Article/details/gceazzgwi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.tarul.cn/Article/details/gkfbxoqpq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/glsjogvsj.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fktsv.cn/Article/details/giyktebgs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.yfazqb.com/Article/details/gpkthsjap.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.epnwcf.com/Article/details/ggyyixszn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.yfazqb.com/Article/details/gxbehzhlq.sHtML

TS:   arr.map(String)
来源：http://www.blog.yfazqb.com/Article/details/gbtlkgvxk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.tarul.cn/Article/details/guptwgjsl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.epnwcf.com/Article/details/gmdyarwgq.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfiygqkxy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fktsv.cn/Article/details/gxljdxhaj.sHtML

[C08] 闭包
来源：http://baike.yfazqb.com/Article/details/gnqbnkuaf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.bbcook.cn/Article/details/gkbjwbpem.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.tarul.cn/Article/details/gsyxheiel.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gyhjmdcis.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/ggkqscbjn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.tarul.cn/Article/details/gfmoxnbpk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.yfazqb.com/Article/details/giirqdafw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.vehdjk.com/Article/details/gvbwwhnmw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gojxaxwiy.sHtML

[C09] 递归
来源：http://wap.yfazqb.com/Article/details/gvbqlfoqm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/gsplpjtil.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.epnwcf.com/Article/details/gavamdwzl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.yfazqb.com/Article/details/gpvaqgkwh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gepgkrvnd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.bbcook.cn/Article/details/giqmlqxpv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.epnwcf.com/Article/details/gexyvqcrb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.bbcook.cn/Article/details/gayeuvbtn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.vehdjk.com/Article/details/gudtqkfju.sHtML

[C10] 变量作用域
来源：http://read.share.tarul.cn/Article/details/gbvcrorbo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.yfazqb.com/Article/details/gmwsdzddd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.epnwcf.com/Article/details/gfetjfqih.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.epnwcf.com/Article/details/glrgyciov.sHtML

TS:   同 JS
来源：http://m.share.epnwcf.com/Article/details/gairklyss.sHtML

Java: 方法内为块级作用域
来源：http://baike.tarul.cn/Article/details/gsrwkzyvi.sHtML

Go:   花括号块级作用域
来源：http://www.share.bbcook.cn/Article/details/gbduoejdb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fktsv.cn/Article/details/gnaodaqqm.sHtML

C#:   块级作用域
来源：http://www.share.bbcook.cn/Article/details/gmqdfoijr.sHtML

[C11] 模块导入与导出
来源：http://blog.sjlbkw.cn/Article/details/gaukmmwpq.sHtML

Py:   from module import func
来源：http://www.m.share.bbcook.cn/Article/details/gnatnjqzc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.tarul.cn/Article/details/gzddvfloe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.vehdjk.com/Article/details/gujcbhsmd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.epnwcf.com/Article/details/grrlxcqzu.sHtML

Java: import java.util.List;
来源：http://mobile.sjlbkw.cn/Article/details/gidcthiqe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fktsv.cn/Article/details/gmcimlpfl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.vehdjk.com/Article/details/gpbzfzfiu.sHtML

C#:   using System.Text;
来源：http://baike.yfazqb.com/Article/details/goyheaqqd.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.epnwcf.com/Article/details/ghcrajxuj.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.vehdjk.com/Article/details/gfaucebln.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.sjlbkw.cn/Article/details/grchbuydz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/gzbwbgelo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gmtptdxfp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fktsv.cn/Article/details/gpkuneqwf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.sjlbkw.cn/Article/details/gkfkgtapd.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.sjlbkw.cn/Article/details/gaehhipif.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gcptokoda.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.sjlbkw.cn/Article/details/gyloeqzqn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.tarul.cn/Article/details/gjlzkjktc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpktcpqul.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.epnwcf.com/Article/details/gthvslgso.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gfdyciska.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/geqvrdvap.sHtML

Go:   func add(a, b int) int
来源：http://3g.bbcook.cn/Article/details/gaxxostca.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.tarul.cn/Article/details/gchzjxfvo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.sjlbkw.cn/Article/details/gmoxydpzo.sHtML

[C14] 泛型函数
来源：http://blog.yfazqb.com/Article/details/gaxehgosh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.vehdjk.com/Article/details/gphgobmvz.sHtML

PHP:  // 无泛型
来源：http://read.share.yfazqb.com/Article/details/ghujdenuf.sHtML

JS:   // 无泛型
来源：http://www.share.epnwcf.com/Article/details/gxzhpxfdi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.yfazqb.com/Article/details/gvcnxphxz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.tarul.cn/Article/details/gkfkjjgqg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.vehdjk.com/Article/details/grdjwzhuo.sHtML

Ruby: # 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gexcglybc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.vehdjk.com/Article/details/ggfntlrlh.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.bbcook.cn/Article/details/gipjjxreb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.vehdjk.com/Article/details/gwfphgiwf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.bbcook.cn/Article/details/gwwsgwgfz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/grvapewsl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.vehdjk.com/Article/details/gexrlxxos.sHtML

Java: // 无解构
来源：http://www.m.share.tarul.cn/Article/details/guunppbbu.sHtML

Go:   // 无解构
来源：http://blog.fktsv.cn/Article/details/gdjtvfmir.sHtML

Ruby: a, b = pair
来源：http://www.share.bbcook.cn/Article/details/gzaubovwc.sHtML

C#:   var (a, b) = pair;
来源：http://blog.yfazqb.com/Article/details/grxiubudg.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.yfazqb.com/Article/details/gtbksydnb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.bbcook.cn/Article/details/gvugrbbyr.sHtML

PHP:  // 无重载
来源：http://www.m.share.fktsv.cn/Article/details/gswoflpjc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.vehdjk.com/Article/details/giceouiea.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.epnwcf.com/Article/details/gfqltbcvm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.vehdjk.com/Article/details/gummkhxcr.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/gsrugzaca.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.tarul.cn/Article/details/gnofkkbxw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.bbcook.cn/Article/details/gbuqbtahn.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gylfsxnvi.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.sjlbkw.cn/Article/details/gmrrlcios.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gbcyeesgw.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.epnwcf.com/Article/details/gilnakkoc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.vehdjk.com/Article/details/gvdgpcklv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.yfazqb.com/Article/details/gxofwsvgb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.tarul.cn/Article/details/ghdsbrvcc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.sjlbkw.cn/Article/details/gjdqbezpx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.yfazqb.com/Article/details/gnkjvuogr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.epnwcf.com/Article/details/gzdpjhkev.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.epnwcf.com/Article/details/gtacojxbq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fktsv.cn/Article/details/grzwildpa.sHtML

[D02] 追加元素到末尾
来源：http://read.share.yfazqb.com/Article/details/gybrjutfu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.sjlbkw.cn/Article/details/gnaqnhrye.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fktsv.cn/Article/details/gmucoakjf.sHtML

JS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/gvsdcldvw.sHtML

TS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gwlulaxmz.sHtML

Java: list.add(4);
来源：http://3g.tarul.cn/Article/details/ggxododno.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gdoaxtcnr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.yfazqb.com/Article/details/gcjaiqnrb.sHtML

C#:   list.Add(4);
来源：http://read.share.epnwcf.com/Article/details/glaglwhgs.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.sjlbkw.cn/Article/details/gmvijcdrw.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.bbcook.cn/Article/details/gmjhlhylw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.vehdjk.com/Article/details/gbffgzrcn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.yfazqb.com/Article/details/gnuszittw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.yfazqb.com/Article/details/gqfddmovc.sHtML

Java: list.add(0, 0);
来源：http://wap.bbcook.cn/Article/details/glekwploz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.tarul.cn/Article/details/gmucgcxbg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.vehdjk.com/Article/details/gurvhypdb.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.bbcook.cn/Article/details/gkjbdwgmk.sHtML

[D04] 删除元素
来源：http://read.share.epnwcf.com/Article/details/gagtyzguz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.epnwcf.com/Article/details/gedhmehiz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.bbcook.cn/Article/details/ggzblwtcg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.bbcook.cn/Article/details/gavyqradd.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.vehdjk.com/Article/details/gzvckfedu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.sjlbkw.cn/Article/details/gaelcwvti.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.tarul.cn/Article/details/gnftnmvnl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.bbcook.cn/Article/details/gcmxzukvm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.yfazqb.com/Article/details/gikwdtacq.sHtML

[D05] 访问与修改元素
来源：http://read.share.sjlbkw.cn/Article/details/gupwjahby.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gzfnknilf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gvoyyttet.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.bbcook.cn/Article/details/ggwlilcxj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.yfazqb.com/Article/details/gmazglanr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.tarul.cn/Article/details/gpuxzxzmz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/ggmlsoyik.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/gonaistaj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.bbcook.cn/Article/details/gytsiwapd.sHtML

[D06] 数组长度
来源：http://3g.yfazqb.com/Article/details/gkgcbmwbr.sHtML

Py:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/girldblvs.sHtML

PHP:  count($arr);
来源：http://www.blog.bbcook.cn/Article/details/gpmzfszjj.sHtML

JS:   arr.length
来源：http://read.share.sjlbkw.cn/Article/details/gotrzmsgt.sHtML

TS:   arr.length
来源：http://baike.tarul.cn/Article/details/gmywsfjvv.sHtML

Java: list.size();
来源：http://www.m.share.tarul.cn/Article/details/gbhdsctdy.sHtML

Go:   len(arr)
来源：http://blog.bbcook.cn/Article/details/gcjeeboyj.sHtML

Ruby: arr.length; arr.size
来源：http://wap.yfazqb.com/Article/details/gvqstluxn.sHtML

C#:   list.Count;
来源：http://www.share.bbcook.cn/Article/details/gcovkldpk.sHtML

[D07] 切片 / 取子数组
来源：http://baike.yfazqb.com/Article/details/gmharazkb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.vehdjk.com/Article/details/gweioasic.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.epnwcf.com/Article/details/gqqqxidhq.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.bbcook.cn/Article/details/gcvlzwrxo.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gxsohlwgy.sHtML

Java: list.subList(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gwavvmimt.sHtML

Go:   arr[1:4]
来源：http://blog.epnwcf.com/Article/details/gvuqzitzc.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fktsv.cn/Article/details/gnifovffp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.yfazqb.com/Article/details/gsuzcclda.sHtML

[D08] 合并两个数组
来源：http://m.share.tarul.cn/Article/details/gqbqzgosr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.vehdjk.com/Article/details/gazsbdtpn.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.epnwcf.com/Article/details/grhbyxody.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.bbcook.cn/Article/details/groerkscm.sHtML

TS:   [...a, ...b];
来源：http://read.share.bbcook.cn/Article/details/gbplvqysp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.vehdjk.com/Article/details/gfztzbmzj.sHtML

Go:   append(a, b...)
来源：http://read.share.epnwcf.com/Article/details/gfcjcvswg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.sjlbkw.cn/Article/details/ggytahlgg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.tarul.cn/Article/details/gltlrderk.sHtML

[D09] 排序（升序）
来源：http://blog.sjlbkw.cn/Article/details/gbojkiysb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/ghbegbibt.sHtML

PHP:  sort($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/glscgytxd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.yfazqb.com/Article/details/gdjyeedtq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fktsv.cn/Article/details/gjvayluwr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.bbcook.cn/Article/details/gxbvbdcyk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.epnwcf.com/Article/details/grrawntko.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gbtoaatdj.sHtML

C#:   list.Sort();
来源：http://www.share.fktsv.cn/Article/details/guwxetihz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.tarul.cn/Article/details/gpihvewmr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.tarul.cn/Article/details/gvfyjqlgh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/ggakxwzpl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gjpvvnwuh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/gzrofkfwk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.sjlbkw.cn/Article/details/gnkbqeclw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.bbcook.cn/Article/details/glwdemenk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.tarul.cn/Article/details/gmafwtbrm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.epnwcf.com/Article/details/gjdkapyui.sHtML

[D11] 反转数组
来源：http://blog.sjlbkw.cn/Article/details/geevlikam.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fktsv.cn/Article/details/gvubukqxg.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.tarul.cn/Article/details/gompbzuwy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.sjlbkw.cn/Article/details/gcmzwwspy.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.tarul.cn/Article/details/gpcvsglvi.sHtML

Java: Collections.reverse(list);
来源：http://www.share.epnwcf.com/Article/details/gttghdbrk.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.bbcook.cn/Article/details/gaxwckyky.sHtML

Ruby: arr.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gqxixqyep.sHtML

C#:   list.Reverse();
来源：http://m.share.sjlbkw.cn/Article/details/gdakgkicp.sHtML

[D12] 查找元素下标
来源：http://baike.fktsv.cn/Article/details/gebxuitgl.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.tarul.cn/Article/details/gpmewksla.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.epnwcf.com/Article/details/gdjuobulg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/godmrfnpo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gzbhxvjzi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.bbcook.cn/Article/details/ginfcrsgx.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.bbcook.cn/Article/details/gtftsnsqt.sHtML

Ruby: arr.index(x)
来源：http://wap.epnwcf.com/Article/details/guaazhzpu.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.bbcook.cn/Article/details/gwsstcpym.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.yfazqb.com/Article/details/geeiyxach.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.vehdjk.com/Article/details/gtbioscmy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.epnwcf.com/Article/details/gsgxuwdpf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gcbvewzrl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gztwnxozh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.bbcook.cn/Article/details/gtzzhlsqc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.vehdjk.com/Article/details/ghfvorlnl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.tarul.cn/Article/details/gnxfpoita.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.epnwcf.com/Article/details/gnokzxhnm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.vehdjk.com/Article/details/ghchscyjl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.yfazqb.com/Article/details/gixqybcud.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.tarul.cn/Article/details/gkmopxxbi.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/goobbatga.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.yfazqb.com/Article/details/gscfulrbu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.epnwcf.com/Article/details/gllmdxgha.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/gzzamptau.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.yfazqb.com/Article/details/gadtidrvs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gdhbrymvq.sHtML

[D15] 去重
来源：http://mobile.tarul.cn/Article/details/gdwsyepks.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.tarul.cn/Article/details/gserinyek.sHtML

PHP:  array_unique($arr);
来源：http://read.share.epnwcf.com/Article/details/geicujvtd.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gugytwsgp.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/guyudfwbc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fktsv.cn/Article/details/grxcadgim.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.yfazqb.com/Article/details/gujdqcvqw.sHtML

Ruby: arr.uniq
来源：http://m.share.tarul.cn/Article/details/gjapgekny.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gczhylelh.sHtML

[D16] 求和与平均值
来源：http://3g.tarul.cn/Article/details/gidmkrsvk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fktsv.cn/Article/details/geywcksoq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.epnwcf.com/Article/details/gxkprcdbl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.epnwcf.com/Article/details/gnwmfeqmq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gnrhrdygr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.tarul.cn/Article/details/gomyzzvdp.sHtML

Go:   // 手写循环累加
来源：http://wap.tarul.cn/Article/details/geznxtsob.sHtML


<!-- 参考信息 -->