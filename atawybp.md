代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.vehdjk.com/Article/details/gvmqnmxlj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fktsv.cn/Article/details/gvlxveyfs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.bbcook.cn/Article/details/gzykphfsw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.yfazqb.com/Article/details/gtwmzeimk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.tarul.cn/Article/details/gurkhnffu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.bbcook.cn/Article/details/gmoogczxk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.vehdjk.com/Article/details/gjhqbwoyb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.bbcook.cn/Article/details/gtqxqsicl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.sjlbkw.cn/Article/details/gvbsnnbhe.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/gixebfuzc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.yfazqb.com/Article/details/geksgrijf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.yfazqb.com/Article/details/gcuzkqwzz.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.vehdjk.com/Article/details/gcikkdsxj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/gtrpfgliw.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gmxtmzdnd.sHtML

[C05] 返回多个值
来源：http://www.share.tarul.cn/Article/details/gdvqcmbkd.sHtML

Py:   return a, b
来源：http://blog.vehdjk.com/Article/details/grsupsyfc.sHtML

PHP:  return [$a, $b];
来源：http://read.share.vehdjk.com/Article/details/gfvukiyqz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/gfsclyuyh.sHtML

TS:   return { a, b };
来源：http://m.share.sjlbkw.cn/Article/details/gqkbhuptx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.tarul.cn/Article/details/gnyragtza.sHtML

Go:   return a, b
来源：http://wap.fktsv.cn/Article/details/gblazmctn.sHtML

Ruby: return a, b
来源：http://wap.sjlbkw.cn/Article/details/gokegcdma.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.epnwcf.com/Article/details/gmqzzzglg.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.bbcook.cn/Article/details/gicppdlym.sHtML

Py:   square = lambda x: x * x
来源：http://3g.epnwcf.com/Article/details/grkuqmnta.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.bbcook.cn/Article/details/gsmdaxwtp.sHtML

JS:   const square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/gnrbqndbr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.bbcook.cn/Article/details/gvobuhfcb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.yfazqb.com/Article/details/guglouyvg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.bbcook.cn/Article/details/gzhuelipq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fktsv.cn/Article/details/gtlyeszbp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gpekglxkx.sHtML

[C07] 把函数作为参数传入
来源：http://blog.sjlbkw.cn/Article/details/gtutedxgo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.bbcook.cn/Article/details/guqailqxm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.tarul.cn/Article/details/gohfflkvr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.bbcook.cn/Article/details/gvropejtd.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fktsv.cn/Article/details/gcwlljyjg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fktsv.cn/Article/details/grqszaqii.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.yfazqb.com/Article/details/guzhgksdb.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.bbcook.cn/Article/details/grkjjqykl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.tarul.cn/Article/details/gqyjipcql.sHtML

[C08] 闭包
来源：http://wap.fktsv.cn/Article/details/gpycntucy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.bbcook.cn/Article/details/gahnnciaj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.yfazqb.com/Article/details/gafqszjip.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/gzkflnoxc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gjzqkhkxf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fktsv.cn/Article/details/gxoemhtza.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.tarul.cn/Article/details/gutyxcfsz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.epnwcf.com/Article/details/gdtmxrudy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gwsngfbyg.sHtML

[C09] 递归
来源：http://read.share.sjlbkw.cn/Article/details/gtfjpwpot.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gkruvfirx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.bbcook.cn/Article/details/glmhjacgg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.sjlbkw.cn/Article/details/gqldimadf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/gbkydaijg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.bbcook.cn/Article/details/gagmrtrxk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.bbcook.cn/Article/details/gmxcnbxrd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/gltxzmboz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.tarul.cn/Article/details/gmmibpjah.sHtML

[C10] 变量作用域
来源：http://www.m.share.epnwcf.com/Article/details/gsgkcssxl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.bbcook.cn/Article/details/grkxzoqux.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.sjlbkw.cn/Article/details/gecmtaykq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.tarul.cn/Article/details/gfvgbgzci.sHtML

TS:   同 JS
来源：http://wap.tarul.cn/Article/details/gbstdlviq.sHtML

Java: 方法内为块级作用域
来源：http://mobile.epnwcf.com/Article/details/gqduapcxt.sHtML

Go:   花括号块级作用域
来源：http://www.share.fktsv.cn/Article/details/gvqxifzbz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.bbcook.cn/Article/details/gvbinxtor.sHtML

C#:   块级作用域
来源：http://read.share.vehdjk.com/Article/details/gtrmdlekf.sHtML

[C11] 模块导入与导出
来源：http://m.share.yfazqb.com/Article/details/gmjoiplcm.sHtML

Py:   from module import func
来源：http://mobile.vehdjk.com/Article/details/gwvkgbgmv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.tarul.cn/Article/details/ggpwmzwsp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.bbcook.cn/Article/details/glmlxkedr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.tarul.cn/Article/details/ghphfbyqr.sHtML

Java: import java.util.List;
来源：http://baike.fktsv.cn/Article/details/gnweqxyna.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.vehdjk.com/Article/details/gxkufqeok.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.yfazqb.com/Article/details/gdcqdlmxt.sHtML

C#:   using System.Text;
来源：http://3g.fktsv.cn/Article/details/gsvfbbmld.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.bbcook.cn/Article/details/gdafrhfoq.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fktsv.cn/Article/details/gzfqysjrg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.sjlbkw.cn/Article/details/gmqcnvhnu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/gygwhybfe.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/gprocpita.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.bbcook.cn/Article/details/gjpxczotz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.tarul.cn/Article/details/gtcubtpex.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.tarul.cn/Article/details/gunyayqxt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.epnwcf.com/Article/details/gbssuonmh.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fktsv.cn/Article/details/gjxwctgqc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.epnwcf.com/Article/details/grjhsznia.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gbrbfsqag.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.tarul.cn/Article/details/gjxwivizh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gtedoymkg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gvxbugyft.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.tarul.cn/Article/details/ggsznpwib.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.yfazqb.com/Article/details/gjnemaltb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.bbcook.cn/Article/details/gamzhooui.sHtML

[C14] 泛型函数
来源：http://www.m.share.vehdjk.com/Article/details/gluuwpbjz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.tarul.cn/Article/details/gqdoihwjo.sHtML

PHP:  // 无泛型
来源：http://blog.fktsv.cn/Article/details/gghgijfcx.sHtML

JS:   // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gzcnnaexk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.yfazqb.com/Article/details/gypnxoynm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.yfazqb.com/Article/details/gaoulmqga.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.bbcook.cn/Article/details/gbrcfpozi.sHtML

Ruby: # 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvvymhcp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fktsv.cn/Article/details/gjliwacsd.sHtML

[C15] 解构 / 展开参数
来源：http://wap.vehdjk.com/Article/details/giwnpqdxz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.yfazqb.com/Article/details/gpyaqrnjs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.epnwcf.com/Article/details/gdbcmkonc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.bbcook.cn/Article/details/gsdoetbwb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.tarul.cn/Article/details/gsjjgxzfk.sHtML

Java: // 无解构
来源：http://3g.vehdjk.com/Article/details/gigbquwhp.sHtML

Go:   // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/gyqpljehx.sHtML

Ruby: a, b = pair
来源：http://read.share.vehdjk.com/Article/details/gamksqdbr.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.vehdjk.com/Article/details/geownvaaa.sHtML

[C16] 函数 / 方法重载
来源：http://3g.tarul.cn/Article/details/gcsggitwh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.epnwcf.com/Article/details/gezoatsmt.sHtML

PHP:  // 无重载
来源：http://m.share.epnwcf.com/Article/details/gnidyenpd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.vehdjk.com/Article/details/gbuohnejq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.yfazqb.com/Article/details/gcfealyrj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.yfazqb.com/Article/details/gfnmhtobk.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.bbcook.cn/Article/details/gnoxzraxo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fktsv.cn/Article/details/gbhzcwmqv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.bbcook.cn/Article/details/gyckodgdt.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/glnfhdfrc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.yfazqb.com/Article/details/ghojjspyn.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/getsdywal.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.sjlbkw.cn/Article/details/gwmifpsed.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.vehdjk.com/Article/details/gbllhgyws.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/gvvacarxq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.yfazqb.com/Article/details/gahgcruzc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fktsv.cn/Article/details/gjwmdsukt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.bbcook.cn/Article/details/gebeovqzz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.bbcook.cn/Article/details/glyghwjcp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.epnwcf.com/Article/details/gztivvvcm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.epnwcf.com/Article/details/gvhmqqxrj.sHtML

[D02] 追加元素到末尾
来源：http://mobile.sjlbkw.cn/Article/details/gknoklpuz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.bbcook.cn/Article/details/gbdlpqgww.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.sjlbkw.cn/Article/details/gbkzvmnyj.sHtML

JS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/gcxmmfjrr.sHtML

TS:   arr.push(4);
来源：http://blog.sjlbkw.cn/Article/details/gbfwasjkk.sHtML

Java: list.add(4);
来源：http://mobile.bbcook.cn/Article/details/gyiueuefn.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.epnwcf.com/Article/details/garpevvah.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.sjlbkw.cn/Article/details/gwwfbsner.sHtML

C#:   list.Add(4);
来源：http://www.share.sjlbkw.cn/Article/details/gmbmohnxk.sHtML

[D03] 在指定位置插入元素
来源：http://3g.epnwcf.com/Article/details/genviibel.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.sjlbkw.cn/Article/details/gdpjimwkh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.sjlbkw.cn/Article/details/gcqbnuadc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.epnwcf.com/Article/details/gqtdvjfps.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.vehdjk.com/Article/details/gebtsqzxt.sHtML

Java: list.add(0, 0);
来源：http://mobile.bbcook.cn/Article/details/gbmyjmzzs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.vehdjk.com/Article/details/gobijogkd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.yfazqb.com/Article/details/grxgweqoz.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.vehdjk.com/Article/details/grpnpdtra.sHtML

[D04] 删除元素
来源：http://baike.fktsv.cn/Article/details/gretatdru.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fktsv.cn/Article/details/giaevrbpk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.epnwcf.com/Article/details/gjraxedde.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.yfazqb.com/Article/details/gudrmapvc.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.yfazqb.com/Article/details/grssuafye.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.epnwcf.com/Article/details/gadhhjdre.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.epnwcf.com/Article/details/gagddzkoa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.epnwcf.com/Article/details/gggtljvvm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.bbcook.cn/Article/details/gpwidwlpi.sHtML

[D05] 访问与修改元素
来源：http://m.share.sjlbkw.cn/Article/details/gfvenycyx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/gguaunyly.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.vehdjk.com/Article/details/ggoehrqnd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/ggexumdae.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.sjlbkw.cn/Article/details/guclbnqcj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.tarul.cn/Article/details/gfrwuirkm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gtrvssdxe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gwclsohwa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.bbcook.cn/Article/details/galfscste.sHtML

[D06] 数组长度
来源：http://www.share.fktsv.cn/Article/details/gsxgpqlkp.sHtML

Py:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gudzskjbm.sHtML

PHP:  count($arr);
来源：http://wap.yfazqb.com/Article/details/ggofcjzrj.sHtML

JS:   arr.length
来源：http://www.share.epnwcf.com/Article/details/gjscrodxz.sHtML

TS:   arr.length
来源：http://baike.tarul.cn/Article/details/gbplbmyxp.sHtML

Java: list.size();
来源：http://www.m.share.bbcook.cn/Article/details/gogfpjtar.sHtML

Go:   len(arr)
来源：http://blog.fktsv.cn/Article/details/gknhnymas.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fktsv.cn/Article/details/gbvjlnvvt.sHtML

C#:   list.Count;
来源：http://m.share.bbcook.cn/Article/details/gcgvqwbac.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.epnwcf.com/Article/details/gdnwosruj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.tarul.cn/Article/details/gwysavuiw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.epnwcf.com/Article/details/gwmmdxuvy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gdyvujdii.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gusfukbzc.sHtML

Java: list.subList(1, 4);
来源：http://blog.fktsv.cn/Article/details/gtjwsripb.sHtML

Go:   arr[1:4]
来源：http://www.m.share.vehdjk.com/Article/details/ggyazhaka.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fktsv.cn/Article/details/gbqdvpwyl.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.yfazqb.com/Article/details/ghlfflwrd.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fktsv.cn/Article/details/gsquswvpp.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.epnwcf.com/Article/details/gwxhbrqmx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fktsv.cn/Article/details/gjambcxcv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkatgjraz.sHtML

TS:   [...a, ...b];
来源：http://read.share.yfazqb.com/Article/details/ghpzbjbpa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.tarul.cn/Article/details/garqruasr.sHtML

Go:   append(a, b...)
来源：http://3g.bbcook.cn/Article/details/grhhidzcf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgyaurzr.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.bbcook.cn/Article/details/gcejdyqvg.sHtML

[D09] 排序（升序）
来源：http://www.m.share.yfazqb.com/Article/details/gyyktnrft.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/gjqqvuasq.sHtML

PHP:  sort($arr);
来源：http://wap.vehdjk.com/Article/details/gzcgpiolp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fktsv.cn/Article/details/gqoozkrio.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.yfazqb.com/Article/details/gnrvpkktp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.vehdjk.com/Article/details/gltfiunrl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.vehdjk.com/Article/details/gavofstyr.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/goigafasc.sHtML

C#:   list.Sort();
来源：http://www.share.yfazqb.com/Article/details/gxwnfwpgo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.sjlbkw.cn/Article/details/gocvlgqbj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.yfazqb.com/Article/details/gudlujgwo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/gilubnckx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/gcruvgdps.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gtflteyfk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.vehdjk.com/Article/details/gztpunfck.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.vehdjk.com/Article/details/gvvjcubip.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.tarul.cn/Article/details/gqpmrasaq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.sjlbkw.cn/Article/details/gjfyzsgrw.sHtML

[D11] 反转数组
来源：http://www.share.fktsv.cn/Article/details/gufvlyzvf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.bbcook.cn/Article/details/guyplpqwz.sHtML

PHP:  array_reverse($arr);
来源：http://baike.epnwcf.com/Article/details/glfbomqtg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.sjlbkw.cn/Article/details/gikqszmdq.sHtML

TS:   [...arr].reverse();
来源：http://www.share.tarul.cn/Article/details/gcbrzjjow.sHtML

Java: Collections.reverse(list);
来源：http://3g.epnwcf.com/Article/details/gfuapjejs.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fktsv.cn/Article/details/gpmozisot.sHtML

Ruby: arr.reverse
来源：http://www.share.vehdjk.com/Article/details/gxnmofxuw.sHtML

C#:   list.Reverse();
来源：http://blog.sjlbkw.cn/Article/details/gagesseyg.sHtML

[D12] 查找元素下标
来源：http://3g.sjlbkw.cn/Article/details/gxeawbltp.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.vehdjk.com/Article/details/ggeufscje.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gmwvxodxx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.bbcook.cn/Article/details/gpxziyxhf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.epnwcf.com/Article/details/giqkavfcj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.bbcook.cn/Article/details/gabuzfvwi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.tarul.cn/Article/details/grnteaxoh.sHtML

Ruby: arr.index(x)
来源：http://read.share.epnwcf.com/Article/details/gkrgwvrdn.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.sjlbkw.cn/Article/details/gjxlbbvfe.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.epnwcf.com/Article/details/gypoowuzn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.epnwcf.com/Article/details/ggelfcgui.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.bbcook.cn/Article/details/ggjgtxnir.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gveuvvttk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gfndtuven.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.tarul.cn/Article/details/gqfqokvhx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.yfazqb.com/Article/details/gthbfkoab.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fktsv.cn/Article/details/guldylvvg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/ggxnkhpcx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.yfazqb.com/Article/details/gohnkbetr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.vehdjk.com/Article/details/gdyfkdtas.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.epnwcf.com/Article/details/gefljocyd.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.bbcook.cn/Article/details/gfvqrzifw.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gvrmaolwj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fktsv.cn/Article/details/gwmfrxslo.sHtML

Go:   // 手写循环
来源：http://www.share.sjlbkw.cn/Article/details/gmnzhymog.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gsiqkkotv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fktsv.cn/Article/details/gzqtajofi.sHtML

[D15] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gjytvrtug.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fktsv.cn/Article/details/gfaxdhzrp.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.vehdjk.com/Article/details/gqmzeabnr.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gcgisdboo.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlfhyxmg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.epnwcf.com/Article/details/ggaxloyaw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.vehdjk.com/Article/details/gviizuakj.sHtML

Ruby: arr.uniq
来源：http://www.share.vehdjk.com/Article/details/grkwzudys.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fktsv.cn/Article/details/geqcxybjf.sHtML

[D16] 求和与平均值
来源：http://blog.fktsv.cn/Article/details/gjmboqltu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gvavhdhoa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fktsv.cn/Article/details/gehpohofq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/gxqrgmoaf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.yfazqb.com/Article/details/goulcxjmx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.sjlbkw.cn/Article/details/grltvxfmn.sHtML

Go:   // 手写循环累加
来源：http://www.share.epnwcf.com/Article/details/gipwbjqmg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/gxcrdjthk.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.sjlbkw.cn/Article/details/gobphhzso.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.epnwcf.com/Article/details/gkrgrnrmm.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.yfazqb.com/Article/details/glvhnpiqf.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.bbcook.cn/Article/details/gvzjqvrei.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.tarul.cn/Article/details/guttwnldl.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.bbcook.cn/Article/details/ghhcxrzjm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fktsv.cn/Article/details/gelyvafsu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.sjlbkw.cn/Article/details/gcmdidaiw.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fktsv.cn/Article/details/grbgoscnp.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fktsv.cn/Article/details/gkouajgqa.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.sjlbkw.cn/Article/details/gemuiezdl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fktsv.cn/Article/details/gkrchzpxn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.bbcook.cn/Article/details/gskfrfbcs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.sjlbkw.cn/Article/details/gcsdzdcjt.sHtML

TS:   nested.flat();
来源：http://blog.yfazqb.com/Article/details/gbebgzdel.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.epnwcf.com/Article/details/ggjzwpbey.sHtML

Go:   // 手写双层循环
来源：http://www.share.vehdjk.com/Article/details/gdfidcybj.sHtML

Ruby: nested.flatten
来源：http://3g.tarul.cn/Article/details/grfvlgpxe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/geyocwyaa.sHtML

[D19] 按字段分组
来源：http://m.share.yfazqb.com/Article/details/gtzzrhnja.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fktsv.cn/Article/details/ghwgblxuc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fktsv.cn/Article/details/geqdnubfj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.tarul.cn/Article/details/garibmexv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/gkbpmghpy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.yfazqb.com/Article/details/gdabyzdyl.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.yfazqb.com/Article/details/ghemlmwpq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.vehdjk.com/Article/details/gtaxleokc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.vehdjk.com/Article/details/gawwqmfvi.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.sjlbkw.cn/Article/details/gnieitfxu.sHtML

Py:   Counter(arr)
来源：http://3g.tarul.cn/Article/details/gqtxweogd.sHtML

PHP:  array_count_values($arr);
来源：http://blog.sjlbkw.cn/Article/details/gpvrkhnjd.sHtML


<!-- 参考信息 -->