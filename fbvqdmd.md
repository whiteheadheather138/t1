代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://m.share.fktsv.cn/Article/details/gfajmyglz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gghurhhws.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/glppjpotq.sHtML

[C05] 返回多个值
来源：http://wap.vehdjk.com/Article/details/gjrpwwnjx.sHtML

Py:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gsmjffzyj.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.bbcook.cn/Article/details/gwmguwlcs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.vehdjk.com/Article/details/gbudvzush.sHtML

TS:   return { a, b };
来源：http://www.m.share.epnwcf.com/Article/details/gmnelhehk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.yfazqb.com/Article/details/guinjnbdj.sHtML

Go:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gywvplrgv.sHtML

Ruby: return a, b
来源：http://www.share.tarul.cn/Article/details/gqtsuppep.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.yfazqb.com/Article/details/gqjgkjwpd.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvqphfob.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.yfazqb.com/Article/details/gpcfaxffq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.vehdjk.com/Article/details/gkcmnnbfq.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gmsqekyka.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.bbcook.cn/Article/details/gsmivgwcb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fktsv.cn/Article/details/gwfnzdasg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.yfazqb.com/Article/details/ggqjknbpu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.epnwcf.com/Article/details/gkbjordno.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/ghqhwshth.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.yfazqb.com/Article/details/gkebyssgk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.tarul.cn/Article/details/gfxnilhmd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.epnwcf.com/Article/details/gluiskytz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.tarul.cn/Article/details/gamelsibq.sHtML

TS:   arr.map(String)
来源：http://wap.yfazqb.com/Article/details/geylnyfex.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gysgtobvp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.epnwcf.com/Article/details/givzvrykd.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.sjlbkw.cn/Article/details/gcolqvacr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.bbcook.cn/Article/details/gwbmtmcfg.sHtML

[C08] 闭包
来源：http://read.share.bbcook.cn/Article/details/gtootqxzs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.tarul.cn/Article/details/gtoflnoan.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.bbcook.cn/Article/details/gbrxhjvle.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gkylraqil.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/gpwnqmjlf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.epnwcf.com/Article/details/gyzjxjmwl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.tarul.cn/Article/details/gxcqfxane.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.sjlbkw.cn/Article/details/gxwxfxpiu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gshpqgewg.sHtML

[C09] 递归
来源：http://www.share.fktsv.cn/Article/details/gpekylgps.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/gjrahbdfk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/gevjftpmc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.sjlbkw.cn/Article/details/gvyknqfji.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gwytjefff.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.epnwcf.com/Article/details/gqybckvyd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.yfazqb.com/Article/details/gffnjgsji.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fktsv.cn/Article/details/gislbhcbx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.bbcook.cn/Article/details/gjsccsjxx.sHtML

[C10] 变量作用域
来源：http://3g.fktsv.cn/Article/details/gnpmcidyt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.tarul.cn/Article/details/gmuwzkoia.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.tarul.cn/Article/details/gfkgbszxn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.epnwcf.com/Article/details/gozjwtwhe.sHtML

TS:   同 JS
来源：http://wap.yfazqb.com/Article/details/gkueulpfs.sHtML

Java: 方法内为块级作用域
来源：http://read.share.tarul.cn/Article/details/gzvzwxvda.sHtML

Go:   花括号块级作用域
来源：http://read.share.vehdjk.com/Article/details/gazmdwvuu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.bbcook.cn/Article/details/gtmynuaht.sHtML

C#:   块级作用域
来源：http://www.share.vehdjk.com/Article/details/gkfrbwgub.sHtML

[C11] 模块导入与导出
来源：http://www.blog.sjlbkw.cn/Article/details/gqrvuzbex.sHtML

Py:   from module import func
来源：http://mobile.bbcook.cn/Article/details/gkgycrzoi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.bbcook.cn/Article/details/gvmjmfmbc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.sjlbkw.cn/Article/details/gwsmyoawm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.tarul.cn/Article/details/gunfjppkn.sHtML

Java: import java.util.List;
来源：http://www.m.share.epnwcf.com/Article/details/glznkisia.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.tarul.cn/Article/details/gtiidsibr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fktsv.cn/Article/details/glagpkxbb.sHtML

C#:   using System.Text;
来源：http://3g.yfazqb.com/Article/details/gkagzdyir.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.bbcook.cn/Article/details/gpfdeqvhw.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.tarul.cn/Article/details/gnauvrjdw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.yfazqb.com/Article/details/gosqoflad.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/gmbgpmpgr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/gxjzaissh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.epnwcf.com/Article/details/gvhhztmqe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.epnwcf.com/Article/details/gvhtmxpra.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.yfazqb.com/Article/details/ghswipgia.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwxyznqa.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.bbcook.cn/Article/details/gyicmdfsy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fktsv.cn/Article/details/guwzptdrt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gtyufuupw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.bbcook.cn/Article/details/gazzktooc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gxkdonyja.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gglsfekxa.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fktsv.cn/Article/details/gqpsgliek.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fktsv.cn/Article/details/gajnvfjxo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.epnwcf.com/Article/details/ghqqiuwco.sHtML

[C14] 泛型函数
来源：http://wap.epnwcf.com/Article/details/giyajquhh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.yfazqb.com/Article/details/gyctsnsvf.sHtML

PHP:  // 无泛型
来源：http://wap.epnwcf.com/Article/details/gainybxgz.sHtML

JS:   // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtxnhrpz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.vehdjk.com/Article/details/geoiwknyu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fktsv.cn/Article/details/gendklvyd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.yfazqb.com/Article/details/gduyetsab.sHtML

Ruby: # 无泛型
来源：http://baike.tarul.cn/Article/details/gjgzpgjav.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fktsv.cn/Article/details/gvurpkzfw.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.epnwcf.com/Article/details/gclyldygd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.epnwcf.com/Article/details/gzkkmgziq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.vehdjk.com/Article/details/guwkywgxo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gqzwiggjf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fktsv.cn/Article/details/gnlgbamcz.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/gpfwkldmm.sHtML

Go:   // 无解构
来源：http://blog.bbcook.cn/Article/details/gcnagbodk.sHtML

Ruby: a, b = pair
来源：http://baike.tarul.cn/Article/details/gtvesgwnf.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fktsv.cn/Article/details/gisxxzojs.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fktsv.cn/Article/details/gddensnqn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.epnwcf.com/Article/details/grdjwmvpz.sHtML

PHP:  // 无重载
来源：http://blog.yfazqb.com/Article/details/gskzhooro.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fktsv.cn/Article/details/gdpqjasqz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/gxhzcacwg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.bbcook.cn/Article/details/gndsygqff.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.vehdjk.com/Article/details/ggkooeplq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fktsv.cn/Article/details/gunmeznvj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.bbcook.cn/Article/details/gqeztuiwd.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/grgscnsef.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.yfazqb.com/Article/details/gyvrodjtn.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gcpyzgfhg.sHtML

[D01] 创建数组 / 列表
来源：http://blog.tarul.cn/Article/details/gmyoczewx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.tarul.cn/Article/details/gjworwgzr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/gecgipqvc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.tarul.cn/Article/details/gqlouwclb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.vehdjk.com/Article/details/gxhqlwycm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.bbcook.cn/Article/details/goghaiuvk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.tarul.cn/Article/details/gkhtiwnmo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.bbcook.cn/Article/details/gxevaugyv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.bbcook.cn/Article/details/gchdwnmuz.sHtML

[D02] 追加元素到末尾
来源：http://baike.epnwcf.com/Article/details/gmhjjauvf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.sjlbkw.cn/Article/details/gbyfzweew.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.epnwcf.com/Article/details/ggvdrmnyc.sHtML

JS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/gwcymfrxq.sHtML

TS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/gaxrswecu.sHtML

Java: list.add(4);
来源：http://baike.yfazqb.com/Article/details/ghscjcvnn.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fktsv.cn/Article/details/gjqbvbeeb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.epnwcf.com/Article/details/glhzodpue.sHtML

C#:   list.Add(4);
来源：http://3g.bbcook.cn/Article/details/gyvvvsloh.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fktsv.cn/Article/details/gubcgksbi.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gylbhnvsb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.vehdjk.com/Article/details/gzfzhieki.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.sjlbkw.cn/Article/details/gmhasajpx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gpemxxaya.sHtML

Java: list.add(0, 0);
来源：http://www.blog.tarul.cn/Article/details/gnmhpukup.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.yfazqb.com/Article/details/giiuhuhnl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.yfazqb.com/Article/details/gsxsfokon.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.tarul.cn/Article/details/gbrtaqibc.sHtML

[D04] 删除元素
来源：http://3g.sjlbkw.cn/Article/details/gstwklpll.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fktsv.cn/Article/details/gdjkprowo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gfekygxoz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.tarul.cn/Article/details/gvyocehzv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.bbcook.cn/Article/details/gepwfscgw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.epnwcf.com/Article/details/gxuyrygiu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.sjlbkw.cn/Article/details/gbxmwtfrt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.sjlbkw.cn/Article/details/gancgqxym.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.tarul.cn/Article/details/gfuyyltmc.sHtML

[D05] 访问与修改元素
来源：http://www.share.yfazqb.com/Article/details/gcefdmnor.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/giblhuwpg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/grevpakbu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/gjydspobw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.yfazqb.com/Article/details/gkmffuhee.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.bbcook.cn/Article/details/grcvdidqd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gwngorlaz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/gbokfnxsf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gzkwzrdjs.sHtML

[D06] 数组长度
来源：http://www.blog.epnwcf.com/Article/details/ghnzgxghs.sHtML

Py:   len(arr)
来源：http://blog.vehdjk.com/Article/details/gjlwzzoqw.sHtML

PHP:  count($arr);
来源：http://read.share.tarul.cn/Article/details/gqvupuygp.sHtML

JS:   arr.length
来源：http://wap.epnwcf.com/Article/details/grbbhcstt.sHtML

TS:   arr.length
来源：http://www.share.tarul.cn/Article/details/gvctpcsfj.sHtML

Java: list.size();
来源：http://blog.sjlbkw.cn/Article/details/gwmxbrcee.sHtML

Go:   len(arr)
来源：http://3g.vehdjk.com/Article/details/gixavtple.sHtML

Ruby: arr.length; arr.size
来源：http://blog.bbcook.cn/Article/details/gfgvcxziz.sHtML

C#:   list.Count;
来源：http://3g.vehdjk.com/Article/details/grpmpubxw.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.bbcook.cn/Article/details/gthqvhawx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.yfazqb.com/Article/details/gzlgaxhyo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.bbcook.cn/Article/details/goubnznvu.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.epnwcf.com/Article/details/gawofcjgz.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/gckjljbjc.sHtML

Java: list.subList(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gehyugffi.sHtML

Go:   arr[1:4]
来源：http://www.share.epnwcf.com/Article/details/gdwkwkoss.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fktsv.cn/Article/details/gyolpscpb.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fktsv.cn/Article/details/gvymvopqk.sHtML

[D08] 合并两个数组
来源：http://www.blog.epnwcf.com/Article/details/gnriqpudq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.epnwcf.com/Article/details/goeasypyu.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.sjlbkw.cn/Article/details/guwnvfchb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.tarul.cn/Article/details/gzkzgonmp.sHtML

TS:   [...a, ...b];
来源：http://m.share.epnwcf.com/Article/details/ghstepdad.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.yfazqb.com/Article/details/gorzfnseu.sHtML

Go:   append(a, b...)
来源：http://www.share.yfazqb.com/Article/details/guptyswud.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.vehdjk.com/Article/details/gcfawbexr.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.epnwcf.com/Article/details/gotzqznno.sHtML

[D09] 排序（升序）
来源：http://blog.yfazqb.com/Article/details/geayvjlxz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/gauwmxymk.sHtML

PHP:  sort($arr);
来源：http://www.share.yfazqb.com/Article/details/gdqbxdhrl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.epnwcf.com/Article/details/gspedhctm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fktsv.cn/Article/details/gnkkpkwae.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.vehdjk.com/Article/details/gqntfwwdx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gwgvkonej.sHtML

Ruby: arr.sort
来源：http://read.share.bbcook.cn/Article/details/gpmykciij.sHtML

C#:   list.Sort();
来源：http://www.m.share.tarul.cn/Article/details/gidrsodfr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.yfazqb.com/Article/details/gtdrdradn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.bbcook.cn/Article/details/gzdacomtu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmucbodou.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fktsv.cn/Article/details/gefgjpity.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/gxxlnfwgo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.bbcook.cn/Article/details/gjtlmoysz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.vehdjk.com/Article/details/gyaghpypv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fktsv.cn/Article/details/gbeskaybe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fktsv.cn/Article/details/gxqtsuylu.sHtML

[D11] 反转数组
来源：http://blog.vehdjk.com/Article/details/gtwplfyqp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.tarul.cn/Article/details/gsjmlttix.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gfowivxuh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.yfazqb.com/Article/details/gxixmyszf.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.tarul.cn/Article/details/ghcxbpmjs.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fktsv.cn/Article/details/gfqcsifdp.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.vehdjk.com/Article/details/gagvmzche.sHtML

Ruby: arr.reverse
来源：http://mobile.bbcook.cn/Article/details/gstdgfqxj.sHtML

C#:   list.Reverse();
来源：http://wap.fktsv.cn/Article/details/gptrdpydo.sHtML

[D12] 查找元素下标
来源：http://www.m.share.yfazqb.com/Article/details/gldwepwsc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.yfazqb.com/Article/details/ggdgevrxq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.yfazqb.com/Article/details/gxejzwmir.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gcbvhgllp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.vehdjk.com/Article/details/gmyzfpbwx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.sjlbkw.cn/Article/details/gfcronaxv.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.vehdjk.com/Article/details/gqbacqjqr.sHtML

Ruby: arr.index(x)
来源：http://baike.epnwcf.com/Article/details/gseovbjjz.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.yfazqb.com/Article/details/girrpcqsq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.bbcook.cn/Article/details/grvgmgiwl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.epnwcf.com/Article/details/gzypcdjpb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.vehdjk.com/Article/details/gzerxlqsf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/gnlpwwbpo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/gvkkjpkby.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.sjlbkw.cn/Article/details/gunsqchvo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.yfazqb.com/Article/details/getysieul.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fktsv.cn/Article/details/goetzsqgt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.vehdjk.com/Article/details/gogzcovnw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.tarul.cn/Article/details/gnxgreldn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.tarul.cn/Article/details/gpqndindb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.yfazqb.com/Article/details/gfaudakmr.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.vehdjk.com/Article/details/gfdwxccvj.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/grceymore.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.tarul.cn/Article/details/gibjqlrcc.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/gxiorppmv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/geokyprcv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gfpyitzyq.sHtML

[D15] 去重
来源：http://wap.vehdjk.com/Article/details/gfjwrenil.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/grhudisea.sHtML

PHP:  array_unique($arr);
来源：http://blog.bbcook.cn/Article/details/gxrlxzepy.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/gpvedibzi.sHtML

TS:   [...new Set(arr)]
来源：http://3g.yfazqb.com/Article/details/gcvawzmyg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.sjlbkw.cn/Article/details/gcyiwpdgz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.bbcook.cn/Article/details/gvanniqnr.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/gnguuxgdk.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.tarul.cn/Article/details/gfmcyxsmh.sHtML

[D16] 求和与平均值
来源：http://www.m.share.vehdjk.com/Article/details/gqbpsaxng.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.yfazqb.com/Article/details/gwepyilpt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.vehdjk.com/Article/details/gvokwnfwn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gbtkrfkgs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.epnwcf.com/Article/details/grmrjgkic.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.yfazqb.com/Article/details/gocqcciqp.sHtML

Go:   // 手写循环累加
来源：http://m.share.yfazqb.com/Article/details/gxcjdnzqu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.sjlbkw.cn/Article/details/gexaoyoxc.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.yfazqb.com/Article/details/gqcwhqhlo.sHtML

[D17] 最大值与最小值
来源：http://wap.fktsv.cn/Article/details/gyquazyvo.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.epnwcf.com/Article/details/gvahvtytz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.vehdjk.com/Article/details/guxaliirq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.sjlbkw.cn/Article/details/gnbtjnwiv.sHtML

TS:   Math.max(...arr);
来源：http://www.share.bbcook.cn/Article/details/ggvufdwqi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.bbcook.cn/Article/details/gyagadnuc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.epnwcf.com/Article/details/gunrvffdh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fktsv.cn/Article/details/gwhchjdgw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.yfazqb.com/Article/details/gausgxmfx.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.sjlbkw.cn/Article/details/goluchgug.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.epnwcf.com/Article/details/gevulgjwa.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.yfazqb.com/Article/details/goxpvnfbx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.tarul.cn/Article/details/gxhuatmib.sHtML

TS:   nested.flat();
来源：http://m.share.bbcook.cn/Article/details/gecbebyhk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.sjlbkw.cn/Article/details/grfvhojwd.sHtML

Go:   // 手写双层循环
来源：http://blog.sjlbkw.cn/Article/details/gvzrawprv.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fktsv.cn/Article/details/gvshgbyqk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.vehdjk.com/Article/details/gugpkauue.sHtML

[D19] 按字段分组
来源：http://www.m.share.bbcook.cn/Article/details/guozynxjy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.epnwcf.com/Article/details/gxcstbsvj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.yfazqb.com/Article/details/gsnafhfxu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.sjlbkw.cn/Article/details/gbuenncwi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gvwornsib.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.tarul.cn/Article/details/gulixpizw.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.yfazqb.com/Article/details/gjbsyxpmg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.tarul.cn/Article/details/gelyybpgz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fktsv.cn/Article/details/goksspsir.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.epnwcf.com/Article/details/gfssxziab.sHtML

Py:   Counter(arr)
来源：http://baike.tarul.cn/Article/details/gcjpniypw.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.bbcook.cn/Article/details/gkyautshl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gubidnpxj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/glxaamtnj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.sjlbkw.cn/Article/details/gpqwxuqfk.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.epnwcf.com/Article/details/gqnbaxrwh.sHtML

Ruby: arr.tally
来源：http://www.blog.tarul.cn/Article/details/gvnbwxtov.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.bbcook.cn/Article/details/gxsrboepu.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fktsv.cn/Article/details/gsgsmxtma.sHtML

Py:   x in arr
来源：http://www.blog.yfazqb.com/Article/details/gnypydpdk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.bbcook.cn/Article/details/gbfyvhdte.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gpugcayko.sHtML

TS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/ghbrvyahb.sHtML

Java: list.contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gyaxndhcy.sHtML


<!-- 参考信息 -->