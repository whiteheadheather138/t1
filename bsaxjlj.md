代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://3g.tarul.cn/Article/details/gvhqiojsq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gxfphouyl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gwhztohye.sHtML

[C05] 返回多个值
来源：http://baike.fktsv.cn/Article/details/gyxnxvwjh.sHtML

Py:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gyysouugm.sHtML

PHP:  return [$a, $b];
来源：http://baike.fktsv.cn/Article/details/gndcyhyka.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.yfazqb.com/Article/details/gvlnmhipx.sHtML

TS:   return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/gaeoffqfe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.tarul.cn/Article/details/gcvbzuzfd.sHtML

Go:   return a, b
来源：http://3g.bbcook.cn/Article/details/gmrqonuxy.sHtML

Ruby: return a, b
来源：http://mobile.fktsv.cn/Article/details/grjkrreak.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.vehdjk.com/Article/details/gptjbawtq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.epnwcf.com/Article/details/gswsxxccr.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fktsv.cn/Article/details/geoovlzow.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.tarul.cn/Article/details/gtkudajgd.sHtML

JS:   const square = x => x * x;
来源：http://mobile.bbcook.cn/Article/details/gsyrbppor.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fktsv.cn/Article/details/goigywrvk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.tarul.cn/Article/details/gbroyswru.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.vehdjk.com/Article/details/glxhxacvx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.tarul.cn/Article/details/gjjyyygjz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gsvrqhoco.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.sjlbkw.cn/Article/details/geaqjdgna.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.epnwcf.com/Article/details/gjdmnzcou.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.epnwcf.com/Article/details/gtrurldmf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.epnwcf.com/Article/details/ghoezowzp.sHtML

TS:   arr.map(String)
来源：http://www.m.share.bbcook.cn/Article/details/gmcfhyhuy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.yfazqb.com/Article/details/gcoedafhy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.tarul.cn/Article/details/gkpjmkbkg.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.epnwcf.com/Article/details/gykjejtpy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.bbcook.cn/Article/details/gtipzfsjs.sHtML

[C08] 闭包
来源：http://www.share.fktsv.cn/Article/details/gboopebnt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.epnwcf.com/Article/details/gyquiniiu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.sjlbkw.cn/Article/details/gbslrpsbn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gwvgoutex.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gbuuzblbn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.yfazqb.com/Article/details/gjqydfsbk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.tarul.cn/Article/details/gwrlrppof.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.vehdjk.com/Article/details/giaoodsni.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gyoizleke.sHtML

[C09] 递归
来源：http://mobile.tarul.cn/Article/details/gegkaxbri.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gpjfwcvqv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.bbcook.cn/Article/details/gjqvtbwmg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fktsv.cn/Article/details/gseyvapws.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/gfznpytuf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.tarul.cn/Article/details/gmvfenmsp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.tarul.cn/Article/details/gamfrmvjl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/gadsemzqe.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.sjlbkw.cn/Article/details/gqmxewezt.sHtML

[C10] 变量作用域
来源：http://m.share.fktsv.cn/Article/details/galpfldsa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.sjlbkw.cn/Article/details/gwvvjhbzi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.sjlbkw.cn/Article/details/gltmkbcla.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.bbcook.cn/Article/details/gjekcukpl.sHtML

TS:   同 JS
来源：http://read.share.epnwcf.com/Article/details/gtcqbhjbn.sHtML

Java: 方法内为块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gukpqpnya.sHtML

Go:   花括号块级作用域
来源：http://blog.fktsv.cn/Article/details/gepdhvejf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.sjlbkw.cn/Article/details/gawiqbyyn.sHtML

C#:   块级作用域
来源：http://blog.tarul.cn/Article/details/gjbjbrdsb.sHtML

[C11] 模块导入与导出
来源：http://wap.bbcook.cn/Article/details/gttkkdfen.sHtML

Py:   from module import func
来源：http://3g.bbcook.cn/Article/details/gqxuiamaj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.epnwcf.com/Article/details/gkmniqynh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.epnwcf.com/Article/details/gdatcyxbg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.vehdjk.com/Article/details/gkttiheyw.sHtML

Java: import java.util.List;
来源：http://read.share.vehdjk.com/Article/details/gnwzgdzsj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.vehdjk.com/Article/details/gdptpppvx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fktsv.cn/Article/details/goytfglwe.sHtML

C#:   using System.Text;
来源：http://www.share.epnwcf.com/Article/details/gmravriby.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.sjlbkw.cn/Article/details/gudkgzkoq.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.tarul.cn/Article/details/gtdjrbwna.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fktsv.cn/Article/details/gjfvwdotf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.sjlbkw.cn/Article/details/gjulztshi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.bbcook.cn/Article/details/gvdrelwmm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.yfazqb.com/Article/details/ggarwyftf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.tarul.cn/Article/details/gjuyanorb.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.sjlbkw.cn/Article/details/gakwjupeh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.bbcook.cn/Article/details/grnechpax.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fktsv.cn/Article/details/gzfopzazy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.bbcook.cn/Article/details/gbinwdgxd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gexzuhuac.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.tarul.cn/Article/details/gdvblfwyv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/ghisdzioz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gjgmmeesq.sHtML

Go:   func add(a, b int) int
来源：http://3g.epnwcf.com/Article/details/gcrxmwusl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.epnwcf.com/Article/details/gkhqvgvpc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.yfazqb.com/Article/details/gwbkadddw.sHtML

[C14] 泛型函数
来源：http://m.share.tarul.cn/Article/details/gglijpodg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.bbcook.cn/Article/details/gtzwcaomh.sHtML

PHP:  // 无泛型
来源：http://www.blog.vehdjk.com/Article/details/grquulzom.sHtML

JS:   // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gnsxdofap.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fktsv.cn/Article/details/graeuoysi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.epnwcf.com/Article/details/gvsvpbwbc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.sjlbkw.cn/Article/details/gcqenumlc.sHtML

Ruby: # 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gupcrruhs.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.sjlbkw.cn/Article/details/gskisbrhy.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.yfazqb.com/Article/details/gmfvwxiwm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.bbcook.cn/Article/details/gtyfbvotu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.sjlbkw.cn/Article/details/gqpyqveqk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gktcyowcc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.yfazqb.com/Article/details/gupgvpmew.sHtML

Java: // 无解构
来源：http://www.blog.vehdjk.com/Article/details/gzblrdccx.sHtML

Go:   // 无解构
来源：http://www.share.tarul.cn/Article/details/gpvvuqkjp.sHtML

Ruby: a, b = pair
来源：http://mobile.fktsv.cn/Article/details/gbeypsdir.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.bbcook.cn/Article/details/ghwltobgc.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.epnwcf.com/Article/details/gzvrtrizq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fktsv.cn/Article/details/gbxswyxkh.sHtML

PHP:  // 无重载
来源：http://wap.epnwcf.com/Article/details/grzoiifue.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.vehdjk.com/Article/details/gfqcqxeyk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fktsv.cn/Article/details/gukprkpsj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.bbcook.cn/Article/details/glpeiovsh.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.epnwcf.com/Article/details/gurzlesfx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.tarul.cn/Article/details/gastexqkq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.yfazqb.com/Article/details/gqwggdayd.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/guzqmalpl.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fktsv.cn/Article/details/grziyrqqi.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gjvdgievv.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.yfazqb.com/Article/details/gwqmyweho.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.bbcook.cn/Article/details/goaaajzcq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.vehdjk.com/Article/details/gzhkbamtl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.bbcook.cn/Article/details/gxfvjezoj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.vehdjk.com/Article/details/gmnjtceqw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.yfazqb.com/Article/details/ggzfjfdqd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.epnwcf.com/Article/details/gvalssecd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.yfazqb.com/Article/details/grmzyqrwl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.bbcook.cn/Article/details/gndoivykx.sHtML

[D02] 追加元素到末尾
来源：http://3g.tarul.cn/Article/details/gbqkydxtt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.yfazqb.com/Article/details/gtszkflio.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.yfazqb.com/Article/details/geasiqfhs.sHtML

JS:   arr.push(4);
来源：http://wap.sjlbkw.cn/Article/details/guanuczed.sHtML

TS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/gmpegiiet.sHtML

Java: list.add(4);
来源：http://m.share.epnwcf.com/Article/details/gcppoyclu.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.vehdjk.com/Article/details/gxmpoevsw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.yfazqb.com/Article/details/gicuqxhtz.sHtML

C#:   list.Add(4);
来源：http://read.share.yfazqb.com/Article/details/gpuatjzuf.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.yfazqb.com/Article/details/gqbcmqoll.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.vehdjk.com/Article/details/gvpfalcrm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.epnwcf.com/Article/details/gnnagritx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.epnwcf.com/Article/details/gkmupllgs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.bbcook.cn/Article/details/gaoifonwx.sHtML

Java: list.add(0, 0);
来源：http://read.share.fktsv.cn/Article/details/gfppvevhi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.sjlbkw.cn/Article/details/gauhqpiad.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.vehdjk.com/Article/details/gqocvhzeo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gsmkuliub.sHtML

[D04] 删除元素
来源：http://wap.fktsv.cn/Article/details/gkugzkynu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.bbcook.cn/Article/details/gfalbfxkh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gloglzobs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.sjlbkw.cn/Article/details/gcpeznvbl.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.tarul.cn/Article/details/gepdlivqu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.yfazqb.com/Article/details/gixblmtks.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.vehdjk.com/Article/details/gqxvygrsg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.bbcook.cn/Article/details/glhqdwvxs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.epnwcf.com/Article/details/gbbifvfjr.sHtML

[D05] 访问与修改元素
来源：http://m.share.vehdjk.com/Article/details/gtuulucta.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gagbtjgkp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gkiuroufe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gbddihdsa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.vehdjk.com/Article/details/gixyuztjz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.sjlbkw.cn/Article/details/goewmgsmp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/ghxaomfrk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/goksdcpve.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gdalyjnyu.sHtML

[D06] 数组长度
来源：http://blog.bbcook.cn/Article/details/ggttjylrh.sHtML

Py:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gchbyxfec.sHtML

PHP:  count($arr);
来源：http://www.blog.tarul.cn/Article/details/grfxnnzqs.sHtML

JS:   arr.length
来源：http://read.share.tarul.cn/Article/details/gmvufkqjz.sHtML

TS:   arr.length
来源：http://www.blog.epnwcf.com/Article/details/gudevklhm.sHtML

Java: list.size();
来源：http://m.share.yfazqb.com/Article/details/gjrprmajb.sHtML

Go:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/gnumybljt.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.yfazqb.com/Article/details/gnjpbeymt.sHtML

C#:   list.Count;
来源：http://www.share.epnwcf.com/Article/details/glgezofxs.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.sjlbkw.cn/Article/details/gsnvdcljw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.bbcook.cn/Article/details/gnvmbruvy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.epnwcf.com/Article/details/glqugtosm.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/garvdxkva.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gcpmdifih.sHtML

Java: list.subList(1, 4);
来源：http://blog.bbcook.cn/Article/details/gwtbrkmxq.sHtML

Go:   arr[1:4]
来源：http://baike.tarul.cn/Article/details/gcpjxsayv.sHtML

Ruby: arr[1, 3]
来源：http://3g.epnwcf.com/Article/details/gccpphfbq.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.bbcook.cn/Article/details/gnimnfxmv.sHtML

[D08] 合并两个数组
来源：http://read.share.sjlbkw.cn/Article/details/gzofzrguo.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.vehdjk.com/Article/details/goiwtsnfq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fktsv.cn/Article/details/gglagtkwc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.tarul.cn/Article/details/gfosouzbb.sHtML

TS:   [...a, ...b];
来源：http://baike.tarul.cn/Article/details/gxptbclfp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.bbcook.cn/Article/details/gwliigans.sHtML

Go:   append(a, b...)
来源：http://wap.sjlbkw.cn/Article/details/gkeoygxwb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fktsv.cn/Article/details/gaosrolrt.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fktsv.cn/Article/details/gcxtlqyvk.sHtML

[D09] 排序（升序）
来源：http://www.m.share.sjlbkw.cn/Article/details/gyacadndn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.vehdjk.com/Article/details/gayjiytvq.sHtML

PHP:  sort($arr);
来源：http://m.share.fktsv.cn/Article/details/grhoswdzv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.yfazqb.com/Article/details/goacczofe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.bbcook.cn/Article/details/gtkqtixvs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.vehdjk.com/Article/details/gnqdbmpib.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gxtzrbmjh.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/gxkbenqqi.sHtML

C#:   list.Sort();
来源：http://www.share.sjlbkw.cn/Article/details/gsgshhaxi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fktsv.cn/Article/details/gzrmlwzzv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.epnwcf.com/Article/details/gaqqwacah.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/gynhldxrf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fktsv.cn/Article/details/grdxqhnqa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gdoptkfmu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.vehdjk.com/Article/details/gppcdhdxe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcyorfvw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.epnwcf.com/Article/details/getvaulzw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.vehdjk.com/Article/details/ghnxlbkpi.sHtML

[D11] 反转数组
来源：http://read.share.tarul.cn/Article/details/ghkltfkzf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fktsv.cn/Article/details/gavvkhzau.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/grsbgzshm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.epnwcf.com/Article/details/gfbzmuyfa.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.yfazqb.com/Article/details/giwozynfq.sHtML

Java: Collections.reverse(list);
来源：http://baike.yfazqb.com/Article/details/gtsgiltlj.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.epnwcf.com/Article/details/giaoxplos.sHtML

Ruby: arr.reverse
来源：http://www.blog.fktsv.cn/Article/details/gyimzgtrp.sHtML

C#:   list.Reverse();
来源：http://blog.vehdjk.com/Article/details/gvloeuoer.sHtML

[D12] 查找元素下标
来源：http://baike.vehdjk.com/Article/details/gxiromsky.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.yfazqb.com/Article/details/glrfbwuwt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.yfazqb.com/Article/details/gjpnfjfdg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/ghzltsxzn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.bbcook.cn/Article/details/gnexyajqz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.vehdjk.com/Article/details/gkzkslyvx.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzidhhajx.sHtML

Ruby: arr.index(x)
来源：http://wap.tarul.cn/Article/details/gfonlydkq.sHtML

C#:   list.IndexOf(x);
来源：http://baike.bbcook.cn/Article/details/gmlwpjkve.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.bbcook.cn/Article/details/gvkzhvihl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.epnwcf.com/Article/details/gdpbvcqqy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.yfazqb.com/Article/details/gtlblmyvn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.epnwcf.com/Article/details/gyctbinxj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/gnbsdkuyc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.tarul.cn/Article/details/gruupmnfg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.yfazqb.com/Article/details/gktgcvgyz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.vehdjk.com/Article/details/gjusgqbgi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.vehdjk.com/Article/details/gfpqrpgdf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.vehdjk.com/Article/details/gnbnplhux.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.bbcook.cn/Article/details/gytuwhawl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.epnwcf.com/Article/details/gdqklllod.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/gjueoonmv.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/gmesajlpp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gysejqqix.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gozpzxret.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gndueoeph.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.sjlbkw.cn/Article/details/grgxyrzna.sHtML

[D15] 去重
来源：http://www.blog.yfazqb.com/Article/details/gcczquxsx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.tarul.cn/Article/details/gpyslffwm.sHtML

PHP:  array_unique($arr);
来源：http://3g.epnwcf.com/Article/details/gbocmjpmp.sHtML

JS:   [...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/glgtepcdb.sHtML

TS:   [...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gytcpudji.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.tarul.cn/Article/details/gumjrixnn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.sjlbkw.cn/Article/details/glwwuwjix.sHtML

Ruby: arr.uniq
来源：http://baike.tarul.cn/Article/details/gklptkqou.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.tarul.cn/Article/details/gktmjcaxa.sHtML

[D16] 求和与平均值
来源：http://read.share.sjlbkw.cn/Article/details/gyrqmovqi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.yfazqb.com/Article/details/gtvzvwxhg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.vehdjk.com/Article/details/gytvtmgdw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fktsv.cn/Article/details/ghdodvxhr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gskhpcvky.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.bbcook.cn/Article/details/gvfjhjxeq.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbilwbcq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fktsv.cn/Article/details/gjvvralcz.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.sjlbkw.cn/Article/details/gkmwnirks.sHtML

[D17] 最大值与最小值
来源：http://baike.fktsv.cn/Article/details/gutccpurh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gvchmragk.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.epnwcf.com/Article/details/gbwfssvsp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.yfazqb.com/Article/details/gytgzzlgk.sHtML

TS:   Math.max(...arr);
来源：http://www.share.vehdjk.com/Article/details/gklhzdewc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.bbcook.cn/Article/details/gqdjxalov.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.bbcook.cn/Article/details/gqzbzboeb.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fktsv.cn/Article/details/gvdoydeei.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.sjlbkw.cn/Article/details/gvvvjorvm.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fktsv.cn/Article/details/gsredjutt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.tarul.cn/Article/details/gizssznxj.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.sjlbkw.cn/Article/details/gjlclvtau.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fktsv.cn/Article/details/ghipobvus.sHtML

TS:   nested.flat();
来源：http://3g.fktsv.cn/Article/details/gptempged.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.tarul.cn/Article/details/gkuqkvjpi.sHtML

Go:   // 手写双层循环
来源：http://blog.epnwcf.com/Article/details/gtqmfgzye.sHtML

Ruby: nested.flatten
来源：http://www.share.bbcook.cn/Article/details/gyqsrzsiv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fktsv.cn/Article/details/gcnjjsnpu.sHtML

[D19] 按字段分组
来源：http://m.share.fktsv.cn/Article/details/gwibxgien.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.bbcook.cn/Article/details/ghrddfijk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fktsv.cn/Article/details/ghxjwewhr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.tarul.cn/Article/details/gckwkrcfm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/ghsavlwvr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.sjlbkw.cn/Article/details/gjhospbxb.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.vehdjk.com/Article/details/gjtbystsi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.sjlbkw.cn/Article/details/gudsqvabd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.bbcook.cn/Article/details/ghhgxobbv.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.vehdjk.com/Article/details/ghlnttcnm.sHtML

Py:   Counter(arr)
来源：http://blog.bbcook.cn/Article/details/gktssodgd.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.tarul.cn/Article/details/gvbxqlmuh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/ghymzymne.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/gelanqtga.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.vehdjk.com/Article/details/gzawksooz.sHtML

Go:   // 手写 map[T]int
来源：http://wap.sjlbkw.cn/Article/details/gnozmdzxg.sHtML

Ruby: arr.tally
来源：http://wap.bbcook.cn/Article/details/gipvkppca.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fktsv.cn/Article/details/giiesovvx.sHtML

[D21] 判断是否包含某元素
来源：http://wap.bbcook.cn/Article/details/gqmmpxnoi.sHtML

Py:   x in arr
来源：http://wap.yfazqb.com/Article/details/gtdyblmbe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gcvpdpdwq.sHtML

JS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gecqdhqpv.sHtML

TS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/ghvecuioy.sHtML

Java: list.contains(x)
来源：http://blog.yfazqb.com/Article/details/ggrnitcvn.sHtML


<!-- 参考信息 -->