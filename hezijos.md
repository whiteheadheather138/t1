代发 wailian999

Py:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gdadlsojs.sHtML

PHP:  return [$a, $b];
来源：http://baike.epnwcf.com/Article/details/ggsncmxnr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gaggljpyu.sHtML

TS:   return { a, b };
来源：http://www.m.share.epnwcf.com/Article/details/glydllhzf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fktsv.cn/Article/details/gtzrecown.sHtML

Go:   return a, b
来源：http://www.share.sjlbkw.cn/Article/details/gdnnzpjmb.sHtML

Ruby: return a, b
来源：http://baike.yfazqb.com/Article/details/gxsjrjrlt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.tarul.cn/Article/details/gidkkgdbq.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fktsv.cn/Article/details/gusrrpgrd.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.vehdjk.com/Article/details/gnhcuqvhf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.bbcook.cn/Article/details/gktuykgpu.sHtML

JS:   const square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gahqzjckm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.yfazqb.com/Article/details/grsqvkylz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.epnwcf.com/Article/details/guwlzxfax.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.yfazqb.com/Article/details/goixpwzke.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.bbcook.cn/Article/details/gzcxiyxqx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gxgnpggev.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.yfazqb.com/Article/details/gbmdwtcvt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.yfazqb.com/Article/details/gttqcvlvz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.yfazqb.com/Article/details/gblnxswiv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.vehdjk.com/Article/details/gbijpxmnz.sHtML

TS:   arr.map(String)
来源：http://wap.bbcook.cn/Article/details/gxiuqbkty.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.bbcook.cn/Article/details/goixndozc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.sjlbkw.cn/Article/details/geuiqkpjh.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.bbcook.cn/Article/details/gsvwimztg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.epnwcf.com/Article/details/gbtkmwvns.sHtML

[C08] 闭包
来源：http://wap.epnwcf.com/Article/details/gobpsmjcq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.epnwcf.com/Article/details/gmkdhtbfo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.sjlbkw.cn/Article/details/gfpcaezlu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/giuxasbaj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gznlqzbya.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.vehdjk.com/Article/details/ggwnaflso.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.sjlbkw.cn/Article/details/gdgjuefcf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fktsv.cn/Article/details/gffdkourm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gtkuljrsn.sHtML

[C09] 递归
来源：http://blog.bbcook.cn/Article/details/gnvelnklj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/gaeetnhgd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.tarul.cn/Article/details/gftxtmkhm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gjfhclgwz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.sjlbkw.cn/Article/details/gjpcthuqe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fktsv.cn/Article/details/gambbzhmd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.sjlbkw.cn/Article/details/gdbhgwnfs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.bbcook.cn/Article/details/gsgpzpyyx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fktsv.cn/Article/details/gokwkgsiy.sHtML

[C10] 变量作用域
来源：http://blog.epnwcf.com/Article/details/ggwtpugjr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.bbcook.cn/Article/details/gmpbipfvh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.vehdjk.com/Article/details/gnharicnp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fktsv.cn/Article/details/gubomjlbl.sHtML

TS:   同 JS
来源：http://read.share.vehdjk.com/Article/details/gsttjjizf.sHtML

Java: 方法内为块级作用域
来源：http://m.share.epnwcf.com/Article/details/geopguqup.sHtML

Go:   花括号块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gfgiwwfaw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.tarul.cn/Article/details/gpnjkqtmg.sHtML

C#:   块级作用域
来源：http://blog.fktsv.cn/Article/details/ghfozwdtb.sHtML

[C11] 模块导入与导出
来源：http://mobile.epnwcf.com/Article/details/gmcvoqxgo.sHtML

Py:   from module import func
来源：http://wap.bbcook.cn/Article/details/gcufxorbu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fktsv.cn/Article/details/gswjyteze.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.sjlbkw.cn/Article/details/ghjrcetwn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.yfazqb.com/Article/details/gdcruxvvq.sHtML

Java: import java.util.List;
来源：http://read.share.yfazqb.com/Article/details/gakgmmbac.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.tarul.cn/Article/details/gywwcuvnv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fktsv.cn/Article/details/gjxcwmioo.sHtML

C#:   using System.Text;
来源：http://read.share.bbcook.cn/Article/details/gcyucicxq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.yfazqb.com/Article/details/gyjwzpumw.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.yfazqb.com/Article/details/gkbpfsjwd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.bbcook.cn/Article/details/gqzolwlcf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.sjlbkw.cn/Article/details/gvgomxgbi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/gjhsuinif.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.epnwcf.com/Article/details/gnkxljhwd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.yfazqb.com/Article/details/gdssvsisq.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.epnwcf.com/Article/details/grpvsyfdy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.epnwcf.com/Article/details/gdrphfnud.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.epnwcf.com/Article/details/gaikupzij.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.tarul.cn/Article/details/gzbkzwwxq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/gprbfybci.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.epnwcf.com/Article/details/gonqcvgno.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gajnxewfp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gshxxtplb.sHtML

Go:   func add(a, b int) int
来源：http://mobile.yfazqb.com/Article/details/gnnmezjmn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.vehdjk.com/Article/details/gvezwrpmg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.bbcook.cn/Article/details/gwhaeafgt.sHtML

[C14] 泛型函数
来源：http://www.share.epnwcf.com/Article/details/gueunqtua.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.bbcook.cn/Article/details/gehyshnzf.sHtML

PHP:  // 无泛型
来源：http://wap.epnwcf.com/Article/details/ghlznqbsy.sHtML

JS:   // 无泛型
来源：http://3g.bbcook.cn/Article/details/gqiyaxabv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.sjlbkw.cn/Article/details/gfwtlmwnf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.tarul.cn/Article/details/ghuaksnpr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.epnwcf.com/Article/details/gazuhlpza.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gkxtsxvwc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fktsv.cn/Article/details/gmncsovts.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.sjlbkw.cn/Article/details/gbtbarlql.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.tarul.cn/Article/details/gjwnpidhm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.bbcook.cn/Article/details/gjtqnhvxo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gqgtpqrne.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.tarul.cn/Article/details/gkxmacpkk.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/gteqoqtfm.sHtML

Go:   // 无解构
来源：http://m.share.yfazqb.com/Article/details/gfxvgpjnc.sHtML

Ruby: a, b = pair
来源：http://baike.tarul.cn/Article/details/gqlhofedg.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.bbcook.cn/Article/details/gcxrkvzdg.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.vehdjk.com/Article/details/gwaembity.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.epnwcf.com/Article/details/gcmzmbdxi.sHtML

PHP:  // 无重载
来源：http://www.m.share.vehdjk.com/Article/details/gskdyavss.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/gcbbpvoku.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.sjlbkw.cn/Article/details/gkurkcjkd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fktsv.cn/Article/details/gnduserbt.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fktsv.cn/Article/details/grxorbgye.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.tarul.cn/Article/details/gmrqnsqxy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.vehdjk.com/Article/details/guuelbfbw.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gbdxrrpkd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.tarul.cn/Article/details/gionuvvpj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gwjokaksh.sHtML

[D01] 创建数组 / 列表
来源：http://3g.tarul.cn/Article/details/gowhuvitw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.epnwcf.com/Article/details/gstuhijej.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.bbcook.cn/Article/details/glvwqpbwj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.vehdjk.com/Article/details/gaegvenip.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.vehdjk.com/Article/details/gcifjblix.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.vehdjk.com/Article/details/ghwtmzjll.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/gmljubjlg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fktsv.cn/Article/details/gaywjooef.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.tarul.cn/Article/details/gicusjmtd.sHtML

[D02] 追加元素到末尾
来源：http://baike.yfazqb.com/Article/details/guqbafqmb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.bbcook.cn/Article/details/gryoaymtd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.tarul.cn/Article/details/gpuowcfuk.sHtML

JS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gdtlzeyiw.sHtML

TS:   arr.push(4);
来源：http://read.share.yfazqb.com/Article/details/ganwysvpx.sHtML

Java: list.add(4);
来源：http://read.share.tarul.cn/Article/details/gsiuqttyr.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fktsv.cn/Article/details/gympjxgwp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.vehdjk.com/Article/details/gnakgdvda.sHtML

C#:   list.Add(4);
来源：http://baike.sjlbkw.cn/Article/details/gpqudymco.sHtML

[D03] 在指定位置插入元素
来源：http://3g.tarul.cn/Article/details/gmkwdfbfc.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.yfazqb.com/Article/details/geydvmgqz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fktsv.cn/Article/details/gmdysudjq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.epnwcf.com/Article/details/gdjsvdukz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.yfazqb.com/Article/details/gkiqjwyll.sHtML

Java: list.add(0, 0);
来源：http://www.share.tarul.cn/Article/details/gclhyangp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fktsv.cn/Article/details/gapnmyteh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.sjlbkw.cn/Article/details/gvokbbnpu.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gktfbdavz.sHtML

[D04] 删除元素
来源：http://www.share.tarul.cn/Article/details/gjbaoogax.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.bbcook.cn/Article/details/gvekblxmb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.bbcook.cn/Article/details/gmzthvyvs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.yfazqb.com/Article/details/grdpfrjds.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.vehdjk.com/Article/details/ghyxdzlad.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.bbcook.cn/Article/details/gghagbeif.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.vehdjk.com/Article/details/gcixmyacn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.sjlbkw.cn/Article/details/grbgdeled.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.bbcook.cn/Article/details/gjgsmabed.sHtML

[D05] 访问与修改元素
来源：http://mobile.yfazqb.com/Article/details/ggsgiovjy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/grtjwlehy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gvuklsozg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/guftmfnmm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.bbcook.cn/Article/details/ghknuknii.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.yfazqb.com/Article/details/gfyndnqbq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gymorevqv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gwttqodbw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gudhdaxbx.sHtML

[D06] 数组长度
来源：http://m.share.vehdjk.com/Article/details/goeclultn.sHtML

Py:   len(arr)
来源：http://blog.vehdjk.com/Article/details/grfocsytk.sHtML

PHP:  count($arr);
来源：http://3g.yfazqb.com/Article/details/gzdxnrijk.sHtML

JS:   arr.length
来源：http://3g.sjlbkw.cn/Article/details/ghzmlwlco.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/gzrkcednq.sHtML

Java: list.size();
来源：http://www.m.share.bbcook.cn/Article/details/glfkgmycw.sHtML

Go:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/gicnpnkkc.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.sjlbkw.cn/Article/details/gfjmxejjr.sHtML

C#:   list.Count;
来源：http://blog.yfazqb.com/Article/details/gmajfegih.sHtML

[D07] 切片 / 取子数组
来源：http://blog.sjlbkw.cn/Article/details/givnfnjll.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.vehdjk.com/Article/details/geidswdyz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.vehdjk.com/Article/details/gftedxdfy.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/gwugfihmk.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/gpjwgvlnv.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gjtjxcaxb.sHtML

Go:   arr[1:4]
来源：http://www.share.tarul.cn/Article/details/gyzxjypws.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.vehdjk.com/Article/details/ghtfojgjm.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.bbcook.cn/Article/details/gvoeceods.sHtML

[D08] 合并两个数组
来源：http://3g.epnwcf.com/Article/details/gwqomnzwc.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.vehdjk.com/Article/details/gfbedecnf.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.bbcook.cn/Article/details/gvserhiwc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.sjlbkw.cn/Article/details/grhoiaxmq.sHtML

TS:   [...a, ...b];
来源：http://www.share.epnwcf.com/Article/details/gtgevuqfq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.bbcook.cn/Article/details/grlpleypi.sHtML

Go:   append(a, b...)
来源：http://read.share.tarul.cn/Article/details/gpivthwwb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fktsv.cn/Article/details/gkgjwfash.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/ghtzalmem.sHtML

[D09] 排序（升序）
来源：http://baike.fktsv.cn/Article/details/gocoestym.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/giogxhcqm.sHtML

PHP:  sort($arr);
来源：http://blog.tarul.cn/Article/details/gpdvontax.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fktsv.cn/Article/details/gazcyavel.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.epnwcf.com/Article/details/grcexseqp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.tarul.cn/Article/details/gzpumhjbx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.epnwcf.com/Article/details/gmhwauwxh.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gvelfngen.sHtML

C#:   list.Sort();
来源：http://blog.vehdjk.com/Article/details/grmgjwtmv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.tarul.cn/Article/details/glisvndzj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fktsv.cn/Article/details/gpqbnlumq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gkbdloqmz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fktsv.cn/Article/details/gcxckkmcd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.epnwcf.com/Article/details/gfpkgflro.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.tarul.cn/Article/details/gjjvxhklv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fktsv.cn/Article/details/gekhsevzc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.yfazqb.com/Article/details/gmuvqjktw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.yfazqb.com/Article/details/gglvotdnr.sHtML

[D11] 反转数组
来源：http://3g.yfazqb.com/Article/details/guvnzmgro.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.tarul.cn/Article/details/gihoucoiy.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.epnwcf.com/Article/details/gseelkasu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.yfazqb.com/Article/details/gxcgfudxd.sHtML

TS:   [...arr].reverse();
来源：http://wap.fktsv.cn/Article/details/gtixutqcw.sHtML

Java: Collections.reverse(list);
来源：http://mobile.bbcook.cn/Article/details/ggjgbebnr.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fktsv.cn/Article/details/grdhwyloa.sHtML

Ruby: arr.reverse
来源：http://blog.sjlbkw.cn/Article/details/gugtvqxgm.sHtML

C#:   list.Reverse();
来源：http://mobile.tarul.cn/Article/details/gooaohnfi.sHtML

[D12] 查找元素下标
来源：http://www.blog.yfazqb.com/Article/details/gmgfskqhu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.bbcook.cn/Article/details/gewojxbjl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gerscejto.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/gsslumitd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/gfwojxbip.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.tarul.cn/Article/details/gebrmwhcp.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gscxyvwxh.sHtML

Ruby: arr.index(x)
来源：http://mobile.sjlbkw.cn/Article/details/gsdtnlbcz.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.tarul.cn/Article/details/gckdugfwn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.tarul.cn/Article/details/gyycrbjvz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.bbcook.cn/Article/details/gupibxwuj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.sjlbkw.cn/Article/details/gatufmlos.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gkhajteed.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gsrrfxuke.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fktsv.cn/Article/details/gylbdavwz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.tarul.cn/Article/details/gjnzxpenj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.epnwcf.com/Article/details/gcwvomdxe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.bbcook.cn/Article/details/ghrzlstge.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.vehdjk.com/Article/details/gxbyvlqhr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fktsv.cn/Article/details/gcszwsbbf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.vehdjk.com/Article/details/gkuwfvkjy.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gnwtzvzut.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.tarul.cn/Article/details/guvvwjvgi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.bbcook.cn/Article/details/gssdazbdy.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/gfpbnxguw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gykcpvomp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.epnwcf.com/Article/details/gfnginalb.sHtML

[D15] 去重
来源：http://baike.yfazqb.com/Article/details/gsljzprco.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.vehdjk.com/Article/details/ggqoznebm.sHtML

PHP:  array_unique($arr);
来源：http://wap.tarul.cn/Article/details/gunnkqjmu.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/grtvubtpw.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gfejbtnfr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fktsv.cn/Article/details/gryzqkofy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.vehdjk.com/Article/details/gspbqabik.sHtML

Ruby: arr.uniq
来源：http://blog.bbcook.cn/Article/details/gydtjxbbg.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.vehdjk.com/Article/details/gjkiifzgr.sHtML

[D16] 求和与平均值
来源：http://baike.epnwcf.com/Article/details/gzyrwjzzs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.vehdjk.com/Article/details/gpvhboyuk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.epnwcf.com/Article/details/gbtxduhai.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gzyjdjxaa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gfaosgymf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.yfazqb.com/Article/details/gfzcdiukc.sHtML

Go:   // 手写循环累加
来源：http://wap.yfazqb.com/Article/details/gbkgedfat.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.bbcook.cn/Article/details/gbhiyuhvu.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.bbcook.cn/Article/details/gkrtcwfyi.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.epnwcf.com/Article/details/gxblnkyyi.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fktsv.cn/Article/details/gqfxifyum.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.epnwcf.com/Article/details/gwfrnzqfx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.vehdjk.com/Article/details/gdktcvphj.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.yfazqb.com/Article/details/gqcqgmfec.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.bbcook.cn/Article/details/gyoeffjag.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.vehdjk.com/Article/details/gvmcounos.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.yfazqb.com/Article/details/ghkvvrhuh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtumebfky.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.tarul.cn/Article/details/gchealavg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.tarul.cn/Article/details/gsxceegzs.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.sjlbkw.cn/Article/details/giwagejjs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.epnwcf.com/Article/details/gyzawmvdl.sHtML

TS:   nested.flat();
来源：http://read.share.fktsv.cn/Article/details/gvohvyizj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.epnwcf.com/Article/details/gxlmimhcs.sHtML

Go:   // 手写双层循环
来源：http://wap.vehdjk.com/Article/details/gjpgeybmo.sHtML

Ruby: nested.flatten
来源：http://blog.yfazqb.com/Article/details/gvzlrmzyp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.tarul.cn/Article/details/geaypfutm.sHtML

[D19] 按字段分组
来源：http://www.share.tarul.cn/Article/details/gzyndfgup.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.bbcook.cn/Article/details/gemqhgzky.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.tarul.cn/Article/details/gitqvcsxm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fktsv.cn/Article/details/gpztvhphl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.bbcook.cn/Article/details/gxrtejwye.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fktsv.cn/Article/details/gfgpfnvui.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.yfazqb.com/Article/details/goaztfrpr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fktsv.cn/Article/details/gmcftgfba.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.epnwcf.com/Article/details/ghcqkpdho.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.sjlbkw.cn/Article/details/gwqwnvocf.sHtML

Py:   Counter(arr)
来源：http://blog.epnwcf.com/Article/details/gcifbktxw.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.vehdjk.com/Article/details/gofbfsktd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/giivtfehf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gxitkqxnt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.tarul.cn/Article/details/gbiqodwxd.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.vehdjk.com/Article/details/gfboaqpyv.sHtML

Ruby: arr.tally
来源：http://www.share.tarul.cn/Article/details/gsyexlkvy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fktsv.cn/Article/details/gopnwtutv.sHtML

[D21] 判断是否包含某元素
来源：http://wap.vehdjk.com/Article/details/gnxbemhqv.sHtML

Py:   x in arr
来源：http://mobile.vehdjk.com/Article/details/gszjlvrtj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.vehdjk.com/Article/details/gtedvhbpq.sHtML

JS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/grixukhyx.sHtML

TS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gfcpoikms.sHtML

Java: list.contains(x)
来源：http://www.m.share.tarul.cn/Article/details/ghzyygdib.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/grmvhfzja.sHtML

Ruby: arr.include?(x)
来源：http://mobile.yfazqb.com/Article/details/gnxjcsjff.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gtcppiwmj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fktsv.cn/Article/details/gxcsbfjib.sHtML


<!-- 参考信息 -->