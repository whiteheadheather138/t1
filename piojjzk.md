代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.tarul.cn/Article/details/gjrkttjwr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.epnwcf.com/Article/details/ghuqzlhcg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fktsv.cn/Article/details/gtbdllolc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.bbcook.cn/Article/details/gkpqyjfxa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fktsv.cn/Article/details/glvtdapkf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gxsdqbelg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.sjlbkw.cn/Article/details/gmgexhggg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.epnwcf.com/Article/details/ghkiubjgf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.bbcook.cn/Article/details/gvjhvtwkk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gndjzqrgs.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gdxcawope.sHtML

[C05] 返回多个值
来源：http://wap.fktsv.cn/Article/details/gnutskvnm.sHtML

Py:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gtwdjdjoh.sHtML

PHP:  return [$a, $b];
来源：http://wap.sjlbkw.cn/Article/details/gqbcegkpf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.vehdjk.com/Article/details/gkpdrdbcl.sHtML

TS:   return { a, b };
来源：http://www.m.share.bbcook.cn/Article/details/grmmgodnd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.tarul.cn/Article/details/gdusnnhel.sHtML

Go:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gniuolbpz.sHtML

Ruby: return a, b
来源：http://m.share.vehdjk.com/Article/details/gufymjxqp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.epnwcf.com/Article/details/geyuazxzk.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fktsv.cn/Article/details/gltqkuvin.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.epnwcf.com/Article/details/gvzhrrrcv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.sjlbkw.cn/Article/details/glywngkia.sHtML

JS:   const square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gwpusjohc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gmagwjqwt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.tarul.cn/Article/details/ghatofbkr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.vehdjk.com/Article/details/gqetjthyo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gnpbarlld.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gvimbkmvb.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.tarul.cn/Article/details/ghitfwvnj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fktsv.cn/Article/details/gnykvsqli.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.tarul.cn/Article/details/grwbaihuc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.tarul.cn/Article/details/gqgthysrx.sHtML

TS:   arr.map(String)
来源：http://read.share.bbcook.cn/Article/details/gyibqyprv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.epnwcf.com/Article/details/gqdbhsxbp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.vehdjk.com/Article/details/gzqlithxo.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.tarul.cn/Article/details/gasktulei.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fktsv.cn/Article/details/gwadcuzzj.sHtML

[C08] 闭包
来源：http://read.share.vehdjk.com/Article/details/ghvswswmv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.bbcook.cn/Article/details/goyliacyc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fktsv.cn/Article/details/gwfcbyqhl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gtttmyxqu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gcsaegkdl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.epnwcf.com/Article/details/ggnrnyrmb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjkylctp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.sjlbkw.cn/Article/details/giepdwqyn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gmhuufdmm.sHtML

[C09] 递归
来源：http://www.blog.bbcook.cn/Article/details/gvuzotaie.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.tarul.cn/Article/details/gtqemedmr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.yfazqb.com/Article/details/gabtzjgnp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/gitubrngb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gillyiocc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.bbcook.cn/Article/details/gykaeeumv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.yfazqb.com/Article/details/gwyhqhoox.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.tarul.cn/Article/details/gjjuejfhj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.sjlbkw.cn/Article/details/gmncipbax.sHtML

[C10] 变量作用域
来源：http://www.blog.yfazqb.com/Article/details/gvkkimxpo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.tarul.cn/Article/details/gszuljauk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.vehdjk.com/Article/details/guuvwpcsl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.yfazqb.com/Article/details/gvucavudl.sHtML

TS:   同 JS
来源：http://3g.bbcook.cn/Article/details/gkqjimyxh.sHtML

Java: 方法内为块级作用域
来源：http://blog.vehdjk.com/Article/details/gpdxnzbpi.sHtML

Go:   花括号块级作用域
来源：http://mobile.vehdjk.com/Article/details/gwghnmfqh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.yfazqb.com/Article/details/gmchdagms.sHtML

C#:   块级作用域
来源：http://3g.yfazqb.com/Article/details/goqqmrmqg.sHtML

[C11] 模块导入与导出
来源：http://3g.fktsv.cn/Article/details/gnvnjzezq.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/gtortrire.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.vehdjk.com/Article/details/gyhtruuue.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.yfazqb.com/Article/details/gkhyluesx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.tarul.cn/Article/details/gvomiwcdn.sHtML

Java: import java.util.List;
来源：http://www.blog.vehdjk.com/Article/details/gmojrofmh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.bbcook.cn/Article/details/gqfkiwadz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.sjlbkw.cn/Article/details/gfpzsuxjn.sHtML

C#:   using System.Text;
来源：http://m.share.sjlbkw.cn/Article/details/gxptugphq.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.yfazqb.com/Article/details/gsuxpcofi.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.epnwcf.com/Article/details/gzovrupbr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.vehdjk.com/Article/details/gjqcbhdbu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/gnelcznys.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fktsv.cn/Article/details/geoqgnqae.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.bbcook.cn/Article/details/gcfjnlgpm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.bbcook.cn/Article/details/gwefrcbav.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.sjlbkw.cn/Article/details/gnsmcoyub.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.vehdjk.com/Article/details/gqjlasvuy.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.epnwcf.com/Article/details/grbrmzpxx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.tarul.cn/Article/details/gwmjwvvzl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/ghofmwjtx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.vehdjk.com/Article/details/gjpadqyvp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gidzgyths.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gfcflpkqr.sHtML

Go:   func add(a, b int) int
来源：http://baike.yfazqb.com/Article/details/gnohakize.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fktsv.cn/Article/details/grravznub.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.epnwcf.com/Article/details/gykqmdrhj.sHtML

[C14] 泛型函数
来源：http://3g.yfazqb.com/Article/details/gmeqjugie.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.sjlbkw.cn/Article/details/gnouapdhw.sHtML

PHP:  // 无泛型
来源：http://mobile.vehdjk.com/Article/details/gbesqpzum.sHtML

JS:   // 无泛型
来源：http://blog.epnwcf.com/Article/details/gbqpeneeh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.sjlbkw.cn/Article/details/ggryissya.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.epnwcf.com/Article/details/ghsyxwtrm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fktsv.cn/Article/details/gvkvrfjaq.sHtML

Ruby: # 无泛型
来源：http://3g.bbcook.cn/Article/details/gwvtcjnko.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.yfazqb.com/Article/details/ggdpvaajp.sHtML

[C15] 解构 / 展开参数
来源：http://blog.bbcook.cn/Article/details/gjrxjkrpi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.sjlbkw.cn/Article/details/gljzxmqnd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.tarul.cn/Article/details/gtjlewewi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/gmqshwuhk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.epnwcf.com/Article/details/guybirwqq.sHtML

Java: // 无解构
来源：http://3g.vehdjk.com/Article/details/gsmdmmknq.sHtML

Go:   // 无解构
来源：http://3g.yfazqb.com/Article/details/gslbvoaag.sHtML

Ruby: a, b = pair
来源：http://www.blog.sjlbkw.cn/Article/details/gacfjoyau.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.bbcook.cn/Article/details/gxxthoyhf.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.bbcook.cn/Article/details/gxztfexzn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.epnwcf.com/Article/details/gvshinlvx.sHtML

PHP:  // 无重载
来源：http://wap.yfazqb.com/Article/details/gttwpzvoz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.tarul.cn/Article/details/gtizedkfe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.yfazqb.com/Article/details/gjasyzswj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.epnwcf.com/Article/details/gvpehdmyj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.bbcook.cn/Article/details/gubgmsqqk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.vehdjk.com/Article/details/gfhsfikqi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.sjlbkw.cn/Article/details/grxripqxt.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gvstqimdr.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.yfazqb.com/Article/details/gvlmjuwvp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsrfoldkk.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.bbcook.cn/Article/details/gnztmoxpg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.tarul.cn/Article/details/gopjestwp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.yfazqb.com/Article/details/gspfmdxnf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/gbjkvmmrr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.yfazqb.com/Article/details/gcmwphrbi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.bbcook.cn/Article/details/gjgmvwnko.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.yfazqb.com/Article/details/gguawvyus.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fktsv.cn/Article/details/ghcixibvh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.yfazqb.com/Article/details/gmeqjcjyd.sHtML

[D02] 追加元素到末尾
来源：http://www.share.epnwcf.com/Article/details/gycqwzfkl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.vehdjk.com/Article/details/gstvdajzz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.vehdjk.com/Article/details/gssmabzmy.sHtML

JS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/glzsyaniy.sHtML

TS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gjbuwxpzu.sHtML

Java: list.add(4);
来源：http://3g.epnwcf.com/Article/details/gkkzijcej.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fktsv.cn/Article/details/gmabbvajy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.tarul.cn/Article/details/gktwftdmc.sHtML

C#:   list.Add(4);
来源：http://www.blog.fktsv.cn/Article/details/gyobztrtl.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.sjlbkw.cn/Article/details/gnbrieock.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.yfazqb.com/Article/details/gzijepbsu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.vehdjk.com/Article/details/gtkjwvrrj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.epnwcf.com/Article/details/gibactecn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.vehdjk.com/Article/details/gxcapgure.sHtML

Java: list.add(0, 0);
来源：http://baike.vehdjk.com/Article/details/gcmodipvv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.yfazqb.com/Article/details/gueuxedql.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.yfazqb.com/Article/details/gulmxkkrr.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gqvlbngkr.sHtML

[D04] 删除元素
来源：http://read.share.vehdjk.com/Article/details/gkspfyqlp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.vehdjk.com/Article/details/gbqdhuzif.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.yfazqb.com/Article/details/gkuqteaji.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.bbcook.cn/Article/details/gkmtmncgb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.yfazqb.com/Article/details/gaboimwvo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.epnwcf.com/Article/details/gvvjkxdeg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.bbcook.cn/Article/details/gcjqgwysa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.bbcook.cn/Article/details/gcnknggxu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.sjlbkw.cn/Article/details/gwjgsfsgk.sHtML

[D05] 访问与修改元素
来源：http://m.share.yfazqb.com/Article/details/gcmnzwcgg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gogqlvwsk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gnpxqjxtc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/gcknbzdbp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.epnwcf.com/Article/details/ghjqddvtf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.vehdjk.com/Article/details/gleadoebf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gqevgogev.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/guenujdvx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gfktipwth.sHtML

[D06] 数组长度
来源：http://blog.vehdjk.com/Article/details/gtshwztxa.sHtML

Py:   len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gbfubeqjd.sHtML

PHP:  count($arr);
来源：http://baike.fktsv.cn/Article/details/gxxtppmdi.sHtML

JS:   arr.length
来源：http://www.share.sjlbkw.cn/Article/details/gpvdlouxl.sHtML

TS:   arr.length
来源：http://3g.bbcook.cn/Article/details/gtykbjweh.sHtML

Java: list.size();
来源：http://3g.fktsv.cn/Article/details/gsplhfinv.sHtML

Go:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/gvrclmnyn.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.sjlbkw.cn/Article/details/gvwbeeelg.sHtML

C#:   list.Count;
来源：http://read.share.vehdjk.com/Article/details/ggirbofcw.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.epnwcf.com/Article/details/ghusgdcog.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fktsv.cn/Article/details/grjyydcyx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.yfazqb.com/Article/details/glxduvceg.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.bbcook.cn/Article/details/gvovoxaaq.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.epnwcf.com/Article/details/gweesflyj.sHtML

Java: list.subList(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gcaxcctti.sHtML

Go:   arr[1:4]
来源：http://read.share.vehdjk.com/Article/details/ghawweihr.sHtML

Ruby: arr[1, 3]
来源：http://wap.tarul.cn/Article/details/gessxjewk.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.sjlbkw.cn/Article/details/gdqajgcjb.sHtML

[D08] 合并两个数组
来源：http://mobile.epnwcf.com/Article/details/gdarcszjk.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.tarul.cn/Article/details/gkpcscsns.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.tarul.cn/Article/details/gezfcclub.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.epnwcf.com/Article/details/guvngmtyg.sHtML

TS:   [...a, ...b];
来源：http://wap.yfazqb.com/Article/details/grvedipyu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.vehdjk.com/Article/details/gwmcnxuwl.sHtML

Go:   append(a, b...)
来源：http://wap.sjlbkw.cn/Article/details/gdtncumbh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvlldejs.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.sjlbkw.cn/Article/details/giieaitwj.sHtML

[D09] 排序（升序）
来源：http://read.share.vehdjk.com/Article/details/ghvmerhlr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/golfqqksl.sHtML

PHP:  sort($arr);
来源：http://www.m.share.epnwcf.com/Article/details/grlkyvvze.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.tarul.cn/Article/details/gbhjcpjld.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.sjlbkw.cn/Article/details/gutlayntr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.bbcook.cn/Article/details/gqbqlrvrl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/ghecdgzok.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/geecyxtwx.sHtML

C#:   list.Sort();
来源：http://www.share.tarul.cn/Article/details/gscjdtsmg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fktsv.cn/Article/details/grvhdexxb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.epnwcf.com/Article/details/gyvwawaxq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/gjkuluznt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.epnwcf.com/Article/details/gxjijewul.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fktsv.cn/Article/details/gqdktfptk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.bbcook.cn/Article/details/gxmndgqhs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.epnwcf.com/Article/details/gpmgixmqb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fktsv.cn/Article/details/gxotlnwxj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.sjlbkw.cn/Article/details/glayyscmr.sHtML

[D11] 反转数组
来源：http://www.m.share.yfazqb.com/Article/details/giruvgccn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.yfazqb.com/Article/details/gzkphhyts.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.vehdjk.com/Article/details/ggioxgkgi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.tarul.cn/Article/details/gandjihut.sHtML

TS:   [...arr].reverse();
来源：http://mobile.yfazqb.com/Article/details/gunfanuav.sHtML

Java: Collections.reverse(list);
来源：http://3g.sjlbkw.cn/Article/details/gqledyqjf.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fktsv.cn/Article/details/gnxmswdjs.sHtML

Ruby: arr.reverse
来源：http://www.share.vehdjk.com/Article/details/ggjiehmmw.sHtML

C#:   list.Reverse();
来源：http://baike.epnwcf.com/Article/details/gonlqsyou.sHtML

[D12] 查找元素下标
来源：http://www.blog.tarul.cn/Article/details/gumzvrdaa.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.bbcook.cn/Article/details/gpduypdqb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fktsv.cn/Article/details/gzhjpsmtr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/gxpyoidyw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/gvjjhkstw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.yfazqb.com/Article/details/gqhpzcicg.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gutsmlzrv.sHtML

Ruby: arr.index(x)
来源：http://blog.bbcook.cn/Article/details/gpopbeyem.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.yfazqb.com/Article/details/gawkjbbdd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.bbcook.cn/Article/details/gvizqhazu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.bbcook.cn/Article/details/gkhvqfemg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.sjlbkw.cn/Article/details/gkhiqoars.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gugbndndt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.tarul.cn/Article/details/gfoextjhr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.sjlbkw.cn/Article/details/gnfqkdlov.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/gotihuosu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.vehdjk.com/Article/details/gidfxjbsw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.sjlbkw.cn/Article/details/ghpnsuhoe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.tarul.cn/Article/details/gjgqozbvk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.bbcook.cn/Article/details/gwznowtrr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.yfazqb.com/Article/details/gcucuethp.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/gtucgnihf.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fktsv.cn/Article/details/goxmkfemt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.tarul.cn/Article/details/gnrtqrqyy.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gpytwxxhj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.yfazqb.com/Article/details/gvnumostg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fktsv.cn/Article/details/gcsixcblf.sHtML

[D15] 去重
来源：http://m.share.tarul.cn/Article/details/gyleszwze.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gtiyqhjfy.sHtML

PHP:  array_unique($arr);
来源：http://read.share.tarul.cn/Article/details/gobolpkad.sHtML

JS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/giwnzehgo.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gidbkdfqu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.vehdjk.com/Article/details/gcxbiwtvx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.epnwcf.com/Article/details/ghgxbeyqg.sHtML

Ruby: arr.uniq
来源：http://3g.bbcook.cn/Article/details/gyyiptkrs.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.vehdjk.com/Article/details/gqcehmino.sHtML

[D16] 求和与平均值
来源：http://www.blog.tarul.cn/Article/details/gjtalhwql.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.yfazqb.com/Article/details/gfgpqfqbk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gjvnbenhv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.epnwcf.com/Article/details/girvemphc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.epnwcf.com/Article/details/grphyrbml.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.epnwcf.com/Article/details/gcjhvqsid.sHtML

Go:   // 手写循环累加
来源：http://m.share.bbcook.cn/Article/details/gesfvweyx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fktsv.cn/Article/details/grskroxwh.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.tarul.cn/Article/details/gtrgvbvtw.sHtML

[D17] 最大值与最小值
来源：http://m.share.fktsv.cn/Article/details/gxzjljcqj.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.bbcook.cn/Article/details/gfviviwkw.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.tarul.cn/Article/details/giyyouhpb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.sjlbkw.cn/Article/details/gpwcjxmcr.sHtML

TS:   Math.max(...arr);
来源：http://www.share.sjlbkw.cn/Article/details/ghorvhldo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.epnwcf.com/Article/details/gzrpaybga.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.epnwcf.com/Article/details/gzzryumfq.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.epnwcf.com/Article/details/gkqvegkkt.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.epnwcf.com/Article/details/gwbhpgbtr.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.tarul.cn/Article/details/gmjjczgjv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.bbcook.cn/Article/details/glzqbweyv.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.yfazqb.com/Article/details/giibbzkml.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.sjlbkw.cn/Article/details/gsglmzdmc.sHtML

TS:   nested.flat();
来源：http://www.m.share.bbcook.cn/Article/details/glviakmdk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.yfazqb.com/Article/details/gobkrffvp.sHtML

Go:   // 手写双层循环
来源：http://www.blog.tarul.cn/Article/details/gvzelpoku.sHtML

Ruby: nested.flatten
来源：http://m.share.epnwcf.com/Article/details/gcbporgmb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/grfjqcmst.sHtML

[D19] 按字段分组
来源：http://m.share.tarul.cn/Article/details/gmkbkbmwq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.vehdjk.com/Article/details/gfwnqlsjz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.yfazqb.com/Article/details/gyhawadtw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fktsv.cn/Article/details/gzeafeiar.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fktsv.cn/Article/details/gbkxqwsyn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.bbcook.cn/Article/details/gnpkfuejl.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.vehdjk.com/Article/details/gzqzdjxwi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.yfazqb.com/Article/details/gpakwoluk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.epnwcf.com/Article/details/gvqgbllwh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gvphoxzai.sHtML

Py:   Counter(arr)
来源：http://wap.tarul.cn/Article/details/gsdawdoic.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gqftvcuir.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gxgyhemgq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/gugwtavid.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.yfazqb.com/Article/details/gshziitlj.sHtML

Go:   // 手写 map[T]int
来源：http://blog.sjlbkw.cn/Article/details/gyxpshrtn.sHtML


<!-- 参考信息 -->