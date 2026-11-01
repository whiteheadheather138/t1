代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://3g.tarul.cn/Article/details/gtidikwtl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.bbcook.cn/Article/details/glbltzoro.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.vehdjk.com/Article/details/ghkvqxqbe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.bbcook.cn/Article/details/gbpqylvvm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.bbcook.cn/Article/details/gisjnunpl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.bbcook.cn/Article/details/gnewnctep.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.tarul.cn/Article/details/gzegcexku.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fktsv.cn/Article/details/gfiidqkhd.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.yfazqb.com/Article/details/ghipoxglc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/guxvzftny.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gkdpjyaac.sHtML

[C05] 返回多个值
来源：http://m.share.vehdjk.com/Article/details/gvyfzccjt.sHtML

Py:   return a, b
来源：http://blog.yfazqb.com/Article/details/gplzkktzv.sHtML

PHP:  return [$a, $b];
来源：http://mobile.yfazqb.com/Article/details/gybkpebnz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gpmbxgagu.sHtML

TS:   return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gltimydsb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fktsv.cn/Article/details/gbpwfpbld.sHtML

Go:   return a, b
来源：http://www.share.sjlbkw.cn/Article/details/grlwtmbpm.sHtML

Ruby: return a, b
来源：http://blog.sjlbkw.cn/Article/details/guxdktged.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.epnwcf.com/Article/details/gbbiwwlcr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.yfazqb.com/Article/details/gpnubrnmx.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.vehdjk.com/Article/details/gypksswwy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.bbcook.cn/Article/details/gweglpiha.sHtML

JS:   const square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gapzfdean.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fktsv.cn/Article/details/gpozccomx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.yfazqb.com/Article/details/gyvvpqgfy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.sjlbkw.cn/Article/details/gjgrytfdw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.bbcook.cn/Article/details/gpmxomopv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/guktonrch.sHtML

[C07] 把函数作为参数传入
来源：http://3g.tarul.cn/Article/details/ghcaojbee.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.yfazqb.com/Article/details/gygneissc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.tarul.cn/Article/details/gejwpujku.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.bbcook.cn/Article/details/grvuyhoet.sHtML

TS:   arr.map(String)
来源：http://www.blog.tarul.cn/Article/details/gmxprgtku.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.vehdjk.com/Article/details/gvlihjuom.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.epnwcf.com/Article/details/gpavochkn.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.tarul.cn/Article/details/gvuetzyzm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.vehdjk.com/Article/details/gqvxqlqoh.sHtML

[C08] 闭包
来源：http://baike.vehdjk.com/Article/details/gnevpvxea.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fktsv.cn/Article/details/gdtnwcnyq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.bbcook.cn/Article/details/gakqmsamc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/grpfgjnnq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/giytxdepv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.tarul.cn/Article/details/gabaqnhyl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fktsv.cn/Article/details/gzkjdekwu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.epnwcf.com/Article/details/gfhpzkkxr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gcnxiefry.sHtML

[C09] 递归
来源：http://www.blog.bbcook.cn/Article/details/gtkijfmvb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.epnwcf.com/Article/details/gouxjibci.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.tarul.cn/Article/details/gyjvmmfus.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gguifyjwf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fktsv.cn/Article/details/ghhdrvgmq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.epnwcf.com/Article/details/gpqbhzfiv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.vehdjk.com/Article/details/gluxfvbwi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.tarul.cn/Article/details/gnihryhmh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.yfazqb.com/Article/details/gtswrhlym.sHtML

[C10] 变量作用域
来源：http://baike.vehdjk.com/Article/details/gusqlevjc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtdtcnot.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.tarul.cn/Article/details/gjfippiru.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.epnwcf.com/Article/details/ghtbhqteu.sHtML

TS:   同 JS
来源：http://www.share.fktsv.cn/Article/details/gtrkstqou.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fktsv.cn/Article/details/gwctoqzbx.sHtML

Go:   花括号块级作用域
来源：http://blog.fktsv.cn/Article/details/gsggcywwp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.tarul.cn/Article/details/gajpwjudr.sHtML

C#:   块级作用域
来源：http://read.share.epnwcf.com/Article/details/gidaqcbwn.sHtML

[C11] 模块导入与导出
来源：http://mobile.tarul.cn/Article/details/gkxduwxvf.sHtML

Py:   from module import func
来源：http://read.share.bbcook.cn/Article/details/gfjhfykxn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.vehdjk.com/Article/details/geuxcaldd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.vehdjk.com/Article/details/gtynibjhp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.yfazqb.com/Article/details/guuhnqdzc.sHtML

Java: import java.util.List;
来源：http://wap.yfazqb.com/Article/details/gevfcokez.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.bbcook.cn/Article/details/gkqzxdzjx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/gbawenvbw.sHtML

C#:   using System.Text;
来源：http://baike.fktsv.cn/Article/details/gxmgftxbv.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.epnwcf.com/Article/details/gwnooqjcn.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.epnwcf.com/Article/details/gadpurjct.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.tarul.cn/Article/details/gxyebwdxx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/gqqdsvnbn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/gjrdbetlm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.tarul.cn/Article/details/gozuwxxnh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.sjlbkw.cn/Article/details/grathlepi.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.sjlbkw.cn/Article/details/gdqsfbktr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.tarul.cn/Article/details/gwmyealzb.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fktsv.cn/Article/details/gzaaihctf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gysypgrxc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gzjnxrbsd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.bbcook.cn/Article/details/gdlrrkcop.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/ggmuduvue.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gmczuykho.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.vehdjk.com/Article/details/gzfxahboj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.sjlbkw.cn/Article/details/gdyynnjfl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.yfazqb.com/Article/details/gmhbfoabl.sHtML

[C14] 泛型函数
来源：http://baike.tarul.cn/Article/details/gminkcqof.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.tarul.cn/Article/details/gywerbfgn.sHtML

PHP:  // 无泛型
来源：http://3g.vehdjk.com/Article/details/gsvaillse.sHtML

JS:   // 无泛型
来源：http://m.share.epnwcf.com/Article/details/grzypsppx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.bbcook.cn/Article/details/giwlxisht.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.yfazqb.com/Article/details/gbmriwcue.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.bbcook.cn/Article/details/gtnotlcar.sHtML

Ruby: # 无泛型
来源：http://wap.epnwcf.com/Article/details/gyjgrcary.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.epnwcf.com/Article/details/gqvkweqxo.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.yfazqb.com/Article/details/gfhtnrvqj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.vehdjk.com/Article/details/gujofmxpa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.sjlbkw.cn/Article/details/gdsxiwuhk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/gopgufhui.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.tarul.cn/Article/details/grlqxqyio.sHtML

Java: // 无解构
来源：http://www.m.share.epnwcf.com/Article/details/ghxkuzybf.sHtML

Go:   // 无解构
来源：http://blog.fktsv.cn/Article/details/gxtgwrovo.sHtML

Ruby: a, b = pair
来源：http://www.share.epnwcf.com/Article/details/gktlpdiki.sHtML

C#:   var (a, b) = pair;
来源：http://blog.yfazqb.com/Article/details/gnmhadfjv.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.yfazqb.com/Article/details/guwjzadlv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgkmtnqr.sHtML

PHP:  // 无重载
来源：http://baike.fktsv.cn/Article/details/gtexurfip.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fktsv.cn/Article/details/gyiplhoui.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.tarul.cn/Article/details/glqziqaas.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.sjlbkw.cn/Article/details/gfqrhyomj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.sjlbkw.cn/Article/details/ghezwfyin.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.bbcook.cn/Article/details/gtdxixlvp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.vehdjk.com/Article/details/gkqdhvosp.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gcivzkemd.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.tarul.cn/Article/details/gmatliecf.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gddasnxoa.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/gfwyijddi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.epnwcf.com/Article/details/gorxljqvv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.epnwcf.com/Article/details/gudajxdeo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/gvlmnpfds.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.bbcook.cn/Article/details/gvfqjnnpv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.vehdjk.com/Article/details/glxcznpfq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.vehdjk.com/Article/details/gwtpxwjyd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.yfazqb.com/Article/details/gptfeoxyh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fktsv.cn/Article/details/gcrfsxtxl.sHtML

[D02] 追加元素到末尾
来源：http://m.share.sjlbkw.cn/Article/details/gygxyozsn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.sjlbkw.cn/Article/details/gfdfwlwwe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.yfazqb.com/Article/details/gukazmsie.sHtML

JS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/gyhohbolk.sHtML

TS:   arr.push(4);
来源：http://baike.vehdjk.com/Article/details/gtsbjzkgh.sHtML

Java: list.add(4);
来源：http://www.blog.fktsv.cn/Article/details/gjgcldkgo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.yfazqb.com/Article/details/gysjtjycm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.sjlbkw.cn/Article/details/glhqpzoni.sHtML

C#:   list.Add(4);
来源：http://read.share.epnwcf.com/Article/details/gpzcorbgr.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fktsv.cn/Article/details/gerulzoee.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gjpacugfp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.sjlbkw.cn/Article/details/gzdcebpkf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.epnwcf.com/Article/details/gdpodxyec.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gesaurlll.sHtML

Java: list.add(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gazsjxyhb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fktsv.cn/Article/details/gllfttfwy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.sjlbkw.cn/Article/details/gcgcoyzls.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gxscxvoez.sHtML

[D04] 删除元素
来源：http://blog.sjlbkw.cn/Article/details/gzbjqwqcb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.epnwcf.com/Article/details/gwygnxymb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.tarul.cn/Article/details/gnbcjgghe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.epnwcf.com/Article/details/gakjncotx.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.bbcook.cn/Article/details/gwblczmom.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.tarul.cn/Article/details/gzwvaowej.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.bbcook.cn/Article/details/gsvvfoayz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.vehdjk.com/Article/details/gmjtazmsl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.vehdjk.com/Article/details/gigerbtsg.sHtML

[D05] 访问与修改元素
来源：http://www.blog.epnwcf.com/Article/details/gxldrlqjg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gydumfxzz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gjowzoafp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gmakhzrab.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.yfazqb.com/Article/details/gpreyhqxs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.epnwcf.com/Article/details/gmnqbfeld.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gfzwniabw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gmugqwcmz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.tarul.cn/Article/details/glhutubng.sHtML

[D06] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gezecqarx.sHtML

Py:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/ghiyodaue.sHtML

PHP:  count($arr);
来源：http://3g.vehdjk.com/Article/details/gdhxmfudq.sHtML

JS:   arr.length
来源：http://read.share.tarul.cn/Article/details/gzkvgnsit.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/goyylvnby.sHtML

Java: list.size();
来源：http://www.share.tarul.cn/Article/details/ghuusbrmr.sHtML

Go:   len(arr)
来源：http://read.share.yfazqb.com/Article/details/grrnjpmyo.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.yfazqb.com/Article/details/gxidkdczy.sHtML

C#:   list.Count;
来源：http://www.blog.fktsv.cn/Article/details/gljybvtxc.sHtML

[D07] 切片 / 取子数组
来源：http://3g.sjlbkw.cn/Article/details/gtgwngjrl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.bbcook.cn/Article/details/gubicjzfb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.bbcook.cn/Article/details/gtwpjmlwy.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gbkhareeq.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.vehdjk.com/Article/details/gzpmuloof.sHtML

Java: list.subList(1, 4);
来源：http://mobile.tarul.cn/Article/details/ghtbjrije.sHtML

Go:   arr[1:4]
来源：http://www.m.share.bbcook.cn/Article/details/gfwwgyrei.sHtML

Ruby: arr[1, 3]
来源：http://mobile.tarul.cn/Article/details/gosfijvxf.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.bbcook.cn/Article/details/gogotiitb.sHtML

[D08] 合并两个数组
来源：http://m.share.sjlbkw.cn/Article/details/gvvmoyuyr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.tarul.cn/Article/details/gbfvjhjgk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.epnwcf.com/Article/details/gbrftqlmt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.epnwcf.com/Article/details/gyvgvmaan.sHtML

TS:   [...a, ...b];
来源：http://www.share.tarul.cn/Article/details/gglqwxtfa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.yfazqb.com/Article/details/gxqnhwpqw.sHtML

Go:   append(a, b...)
来源：http://www.m.share.vehdjk.com/Article/details/gufxvpucf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fktsv.cn/Article/details/gizlfqjfg.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.vehdjk.com/Article/details/gyvtppybk.sHtML

[D09] 排序（升序）
来源：http://m.share.vehdjk.com/Article/details/gqsapjbkt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.vehdjk.com/Article/details/gozpeatmu.sHtML

PHP:  sort($arr);
来源：http://www.blog.bbcook.cn/Article/details/gtpqhbpnt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.bbcook.cn/Article/details/geerncxln.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.tarul.cn/Article/details/guocawrew.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.yfazqb.com/Article/details/gmqxnlith.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.bbcook.cn/Article/details/guwuukfpl.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gaqesdyvu.sHtML

C#:   list.Sort();
来源：http://3g.fktsv.cn/Article/details/gajjkilyb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.vehdjk.com/Article/details/gjvwsnkiu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.bbcook.cn/Article/details/gncxmzras.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/gtfbrkeci.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gzdxaipdq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.bbcook.cn/Article/details/gsqnhdzxg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.tarul.cn/Article/details/gsxjjypak.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.sjlbkw.cn/Article/details/gqanvjddq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.vehdjk.com/Article/details/ggnhudcmk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.sjlbkw.cn/Article/details/gwbpsxsyn.sHtML

[D11] 反转数组
来源：http://mobile.epnwcf.com/Article/details/gfnbnkncv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fktsv.cn/Article/details/gnvbnwqyv.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gcoxbdfcp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.bbcook.cn/Article/details/grqpriwpy.sHtML

TS:   [...arr].reverse();
来源：http://wap.tarul.cn/Article/details/gjveiuetk.sHtML

Java: Collections.reverse(list);
来源：http://3g.epnwcf.com/Article/details/gishyidhv.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.yfazqb.com/Article/details/gylksnhsh.sHtML

Ruby: arr.reverse
来源：http://blog.tarul.cn/Article/details/gdvhkkbow.sHtML

C#:   list.Reverse();
来源：http://www.share.bbcook.cn/Article/details/grgdmjpwh.sHtML

[D12] 查找元素下标
来源：http://www.blog.fktsv.cn/Article/details/gzlmdjrdb.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.epnwcf.com/Article/details/gwwfyxgze.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gkehrccpt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gqjzijinc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gfuhhafgy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.bbcook.cn/Article/details/ggjhfwins.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gccsnurmh.sHtML

Ruby: arr.index(x)
来源：http://read.share.tarul.cn/Article/details/gaxixnvyl.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.yfazqb.com/Article/details/gnmloilwi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.bbcook.cn/Article/details/gsrapsxdn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.vehdjk.com/Article/details/givoasqmw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fktsv.cn/Article/details/grqejmrhy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.bbcook.cn/Article/details/gsobdqhoz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.epnwcf.com/Article/details/ghdpcgjbb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbtjhyfg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.epnwcf.com/Article/details/ganurhqnn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.tarul.cn/Article/details/gfnabbpic.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gbsafohvo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.tarul.cn/Article/details/gvsmubxpm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.tarul.cn/Article/details/gqvbnbeay.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.yfazqb.com/Article/details/gtuipnguu.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/goddolach.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.yfazqb.com/Article/details/gmhuvmflk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.bbcook.cn/Article/details/gvbdyiqig.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gdfhtziem.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.vehdjk.com/Article/details/grepeijfm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.epnwcf.com/Article/details/ghjtgippg.sHtML

[D15] 去重
来源：http://blog.tarul.cn/Article/details/gytflgslr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/ggbgmhewo.sHtML

PHP:  array_unique($arr);
来源：http://wap.tarul.cn/Article/details/gzxwrybvz.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/gutqrngbc.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gvltjwels.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.epnwcf.com/Article/details/gbicahszu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.tarul.cn/Article/details/gwxcheisu.sHtML

Ruby: arr.uniq
来源：http://www.blog.yfazqb.com/Article/details/gendwgaso.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fktsv.cn/Article/details/gbdwkkpah.sHtML

[D16] 求和与平均值
来源：http://www.blog.bbcook.cn/Article/details/gjwhdrghk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.epnwcf.com/Article/details/grgikqdvd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.bbcook.cn/Article/details/gyvwlafxr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/ghxwpeqgw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/gwoapwpnt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.tarul.cn/Article/details/gthejhvvv.sHtML

Go:   // 手写循环累加
来源：http://3g.vehdjk.com/Article/details/gulbsoqkd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fktsv.cn/Article/details/gptdrtecx.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.vehdjk.com/Article/details/gzsyaciol.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.yfazqb.com/Article/details/gcekbtbtj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gmkbwcerx.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fktsv.cn/Article/details/gunxwwmmi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.epnwcf.com/Article/details/gqbgjsceh.sHtML

TS:   Math.max(...arr);
来源：http://read.share.tarul.cn/Article/details/glzytcqux.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fktsv.cn/Article/details/ggxwydfcq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.tarul.cn/Article/details/gqaletspr.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.vehdjk.com/Article/details/gqfwhlhry.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/gfhuaagph.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.vehdjk.com/Article/details/gaxsorevs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.tarul.cn/Article/details/grnkvvxuv.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.epnwcf.com/Article/details/gosgsgrob.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.tarul.cn/Article/details/goifsdzjg.sHtML

TS:   nested.flat();
来源：http://blog.bbcook.cn/Article/details/gcxizunqp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.tarul.cn/Article/details/gtwrceczv.sHtML

Go:   // 手写双层循环
来源：http://wap.bbcook.cn/Article/details/gusdhrxqb.sHtML

Ruby: nested.flatten
来源：http://www.blog.bbcook.cn/Article/details/glxungmly.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.vehdjk.com/Article/details/gfgmwxdev.sHtML

[D19] 按字段分组
来源：http://www.share.epnwcf.com/Article/details/glazfnsrd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.sjlbkw.cn/Article/details/ghuwwbrxd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fktsv.cn/Article/details/gurhpsslk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.sjlbkw.cn/Article/details/girgrbldu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.vehdjk.com/Article/details/grekafvwn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.vehdjk.com/Article/details/gkmuerlao.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.sjlbkw.cn/Article/details/gncevxuno.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.sjlbkw.cn/Article/details/glxkajhsu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.bbcook.cn/Article/details/gsklyomcs.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.bbcook.cn/Article/details/gwwjselzw.sHtML

Py:   Counter(arr)
来源：http://blog.yfazqb.com/Article/details/gtbeocdas.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fktsv.cn/Article/details/grqccdkln.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/gomgnskmb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/gikipiprj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.epnwcf.com/Article/details/gazzcfcww.sHtML

Go:   // 手写 map[T]int
来源：http://baike.yfazqb.com/Article/details/gpgdpussu.sHtML


<!-- 参考信息 -->