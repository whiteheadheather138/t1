代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/gegqlycrj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.epnwcf.com/Article/details/gbewfhdno.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fktsv.cn/Article/details/gkpmmidpd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.bbcook.cn/Article/details/gwdgndtkm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.tarul.cn/Article/details/gwixybncz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.bbcook.cn/Article/details/glzfwtdfm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.sjlbkw.cn/Article/details/gaiarvtxb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.sjlbkw.cn/Article/details/gngfzrgvx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gstwiezwd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.vehdjk.com/Article/details/gyosenzrm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.tarul.cn/Article/details/gsnictqzs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.epnwcf.com/Article/details/gxxuorcoj.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.bbcook.cn/Article/details/gfuusofoy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gupetlvhp.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/gvshrqqcp.sHtML

[C05] 返回多个值
来源：http://www.blog.epnwcf.com/Article/details/gjueeodml.sHtML

Py:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gdtltyzwe.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fktsv.cn/Article/details/gwnlqkaaj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gkbavvwdt.sHtML

TS:   return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gjxxllyxy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fktsv.cn/Article/details/gxqztlrrf.sHtML

Go:   return a, b
来源：http://read.share.sjlbkw.cn/Article/details/ggslloiii.sHtML

Ruby: return a, b
来源：http://3g.bbcook.cn/Article/details/gukbavnbm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.vehdjk.com/Article/details/gjmircxrv.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.yfazqb.com/Article/details/gbxffsrph.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fktsv.cn/Article/details/gidihgiom.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fktsv.cn/Article/details/gblwqieru.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gamzskwzb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.bbcook.cn/Article/details/ggwozctxb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.sjlbkw.cn/Article/details/ghxaoezem.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.tarul.cn/Article/details/gtjcjtnyb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.tarul.cn/Article/details/gobdhscgy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.epnwcf.com/Article/details/gelqcbanp.sHtML

[C07] 把函数作为参数传入
来源：http://baike.bbcook.cn/Article/details/ghruaymtt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.yfazqb.com/Article/details/gqepbtiva.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.tarul.cn/Article/details/gqamutezr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.tarul.cn/Article/details/gyvwibagm.sHtML

TS:   arr.map(String)
来源：http://read.share.fktsv.cn/Article/details/gbcjlklsz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.sjlbkw.cn/Article/details/gptnkafbf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.yfazqb.com/Article/details/gdzatxggc.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fktsv.cn/Article/details/gqzlpfewj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fktsv.cn/Article/details/graqwsveg.sHtML

[C08] 闭包
来源：http://read.share.sjlbkw.cn/Article/details/gfxxnberd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.bbcook.cn/Article/details/gpvnljeac.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.bbcook.cn/Article/details/goylimojm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/goqeabxku.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/glytzbvov.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.yfazqb.com/Article/details/gciyjrsnw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.sjlbkw.cn/Article/details/gzjstqntv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.bbcook.cn/Article/details/gkdmqyrsg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gayrvnxwn.sHtML

[C09] 递归
来源：http://3g.sjlbkw.cn/Article/details/gsbczmaud.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.epnwcf.com/Article/details/gkknckfgy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.yfazqb.com/Article/details/gylpgzctq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fktsv.cn/Article/details/glvcacajw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.epnwcf.com/Article/details/gdhuphxmy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fktsv.cn/Article/details/gczwqsthl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.sjlbkw.cn/Article/details/gwqmimloq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/gxedhpywx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.epnwcf.com/Article/details/gjammoykf.sHtML

[C10] 变量作用域
来源：http://3g.sjlbkw.cn/Article/details/gbynhmaif.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.epnwcf.com/Article/details/ghcoespmc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.yfazqb.com/Article/details/glhnajere.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fktsv.cn/Article/details/gpqqjibqp.sHtML

TS:   同 JS
来源：http://baike.yfazqb.com/Article/details/gqagkzbyr.sHtML

Java: 方法内为块级作用域
来源：http://wap.fktsv.cn/Article/details/gkgfahyph.sHtML

Go:   花括号块级作用域
来源：http://www.share.fktsv.cn/Article/details/gyfyzfvrg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.epnwcf.com/Article/details/gulfcdspx.sHtML

C#:   块级作用域
来源：http://mobile.tarul.cn/Article/details/gkjivbanj.sHtML

[C11] 模块导入与导出
来源：http://baike.yfazqb.com/Article/details/gpdmglwgm.sHtML

Py:   from module import func
来源：http://mobile.fktsv.cn/Article/details/gkwbggqvq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqjpdzah.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fktsv.cn/Article/details/gfykyhfzy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.bbcook.cn/Article/details/gehbjnelz.sHtML

Java: import java.util.List;
来源：http://3g.sjlbkw.cn/Article/details/gbvugoutf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.bbcook.cn/Article/details/gkxtjvrrx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.epnwcf.com/Article/details/geguhrmry.sHtML

C#:   using System.Text;
来源：http://baike.epnwcf.com/Article/details/glnlvlnzd.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.sjlbkw.cn/Article/details/gpfvzwoio.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.epnwcf.com/Article/details/glwksnztp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.sjlbkw.cn/Article/details/gybqbamur.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/gvpvhypwg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gssaxlvgs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.sjlbkw.cn/Article/details/gjywlknxr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fktsv.cn/Article/details/gzcgxcmhq.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.epnwcf.com/Article/details/gwqvpumbe.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.bbcook.cn/Article/details/ghowtaaah.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.vehdjk.com/Article/details/gfntujezr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.sjlbkw.cn/Article/details/guyzgiubt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkmasfwd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.bbcook.cn/Article/details/gfioqqccu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gjeqrttln.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gelqppfpa.sHtML

Go:   func add(a, b int) int
来源：http://read.share.epnwcf.com/Article/details/gntevsswk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.bbcook.cn/Article/details/gospdocyk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.tarul.cn/Article/details/gjrkjwtwb.sHtML

[C14] 泛型函数
来源：http://www.m.share.tarul.cn/Article/details/geetddctw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.epnwcf.com/Article/details/glcnozgiq.sHtML

PHP:  // 无泛型
来源：http://read.share.vehdjk.com/Article/details/gblaktvbt.sHtML

JS:   // 无泛型
来源：http://www.m.share.bbcook.cn/Article/details/gwqcxztqd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.tarul.cn/Article/details/gmtqbubuk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gurxpotzz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.bbcook.cn/Article/details/guxhffixl.sHtML

Ruby: # 无泛型
来源：http://read.share.vehdjk.com/Article/details/gxkyxuhdz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.sjlbkw.cn/Article/details/ghmyxdqay.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.tarul.cn/Article/details/gtmjkdwlo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.epnwcf.com/Article/details/gysgbpwxd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.bbcook.cn/Article/details/gxiwxsfvq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gvzvekkhc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.tarul.cn/Article/details/gzfnqpkxw.sHtML

Java: // 无解构
来源：http://m.share.epnwcf.com/Article/details/gzbsrgxxc.sHtML

Go:   // 无解构
来源：http://read.share.tarul.cn/Article/details/gthydlcec.sHtML

Ruby: a, b = pair
来源：http://read.share.fktsv.cn/Article/details/gegwhesip.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.epnwcf.com/Article/details/gzpdhxuby.sHtML

[C16] 函数 / 方法重载
来源：http://wap.yfazqb.com/Article/details/gdnllhgwa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fktsv.cn/Article/details/glzgtyxka.sHtML

PHP:  // 无重载
来源：http://www.blog.vehdjk.com/Article/details/gosdjfswz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.tarul.cn/Article/details/gimdwmavu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.vehdjk.com/Article/details/grpywloik.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.epnwcf.com/Article/details/gatoiheir.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.sjlbkw.cn/Article/details/grxwepcwd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.epnwcf.com/Article/details/gqixhjstg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.vehdjk.com/Article/details/gzazhfttz.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gjvdcmqtw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.vehdjk.com/Article/details/gcrvgnrzs.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gtqlhfwyy.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.bbcook.cn/Article/details/gxifteovi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.tarul.cn/Article/details/glrdhdhle.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.vehdjk.com/Article/details/gvfqmogaq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.epnwcf.com/Article/details/gbiesbklg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.sjlbkw.cn/Article/details/gpjggktog.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.sjlbkw.cn/Article/details/gsxetqaau.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.yfazqb.com/Article/details/gpumqmplz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.sjlbkw.cn/Article/details/gyrbldtzx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.yfazqb.com/Article/details/gxhlwojwl.sHtML

[D02] 追加元素到末尾
来源：http://mobile.tarul.cn/Article/details/gzndmgngy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.sjlbkw.cn/Article/details/gvtmfnitb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.epnwcf.com/Article/details/giybwidou.sHtML

JS:   arr.push(4);
来源：http://blog.sjlbkw.cn/Article/details/gwsabozws.sHtML

TS:   arr.push(4);
来源：http://www.blog.yfazqb.com/Article/details/gautmwmyz.sHtML

Java: list.add(4);
来源：http://blog.tarul.cn/Article/details/gizyqrdtd.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.sjlbkw.cn/Article/details/gkkzzqdhl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.yfazqb.com/Article/details/gwyiivjwr.sHtML

C#:   list.Add(4);
来源：http://read.share.tarul.cn/Article/details/ggttvhhxu.sHtML

[D03] 在指定位置插入元素
来源：http://wap.epnwcf.com/Article/details/gxtmolhzl.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.bbcook.cn/Article/details/gwdhowqhu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.bbcook.cn/Article/details/gtafavmxs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.tarul.cn/Article/details/givalmooq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.tarul.cn/Article/details/gdvpalghn.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gmcikswlx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.bbcook.cn/Article/details/gvvorzqxo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.bbcook.cn/Article/details/gswjswbag.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.bbcook.cn/Article/details/gxgissyfc.sHtML

[D04] 删除元素
来源：http://wap.sjlbkw.cn/Article/details/glqqabghu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.bbcook.cn/Article/details/gjvsmvsrf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.vehdjk.com/Article/details/gcneqkhqg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.vehdjk.com/Article/details/gkeexiqit.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.yfazqb.com/Article/details/guosozphz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.vehdjk.com/Article/details/gdfcpfkct.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.yfazqb.com/Article/details/ggkjoeobh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.epnwcf.com/Article/details/ggmyoaqfz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfpirmmr.sHtML

[D05] 访问与修改元素
来源：http://baike.epnwcf.com/Article/details/gpqccrlhh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.yfazqb.com/Article/details/gcoccosnu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gbwjtkwuo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gmfysjvis.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.epnwcf.com/Article/details/ghrrflwxj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.yfazqb.com/Article/details/gujaejvog.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/gqlfahoaj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/gmcbgldnr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/giafvssrz.sHtML

[D06] 数组长度
来源：http://www.share.fktsv.cn/Article/details/gabngalbq.sHtML

Py:   len(arr)
来源：http://m.share.epnwcf.com/Article/details/gcfpngybi.sHtML

PHP:  count($arr);
来源：http://read.share.epnwcf.com/Article/details/gymuobqnn.sHtML

JS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/guexzjwtk.sHtML

TS:   arr.length
来源：http://m.share.sjlbkw.cn/Article/details/ghrsmiust.sHtML

Java: list.size();
来源：http://3g.vehdjk.com/Article/details/gqnljzocy.sHtML

Go:   len(arr)
来源：http://read.share.yfazqb.com/Article/details/gjzgvcspv.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.epnwcf.com/Article/details/gsjbcecfx.sHtML

C#:   list.Count;
来源：http://3g.sjlbkw.cn/Article/details/gcahwmbon.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.yfazqb.com/Article/details/gbnwqhgcj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.vehdjk.com/Article/details/ggdtlkwzr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.bbcook.cn/Article/details/gylwrlbkt.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gdgklebmd.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/gtdgsuohi.sHtML

Java: list.subList(1, 4);
来源：http://mobile.tarul.cn/Article/details/gyjgnlnnh.sHtML

Go:   arr[1:4]
来源：http://www.blog.vehdjk.com/Article/details/gwcdduwtn.sHtML

Ruby: arr[1, 3]
来源：http://baike.sjlbkw.cn/Article/details/gzfybawal.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fktsv.cn/Article/details/gzipkdqmx.sHtML

[D08] 合并两个数组
来源：http://www.share.bbcook.cn/Article/details/ghhywpvtp.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.sjlbkw.cn/Article/details/gmxksmwju.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fktsv.cn/Article/details/gawifvari.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.vehdjk.com/Article/details/gkrsdrcfd.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfcmwcqy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.vehdjk.com/Article/details/gzcbieycd.sHtML

Go:   append(a, b...)
来源：http://mobile.fktsv.cn/Article/details/gsasimaam.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.epnwcf.com/Article/details/geglolyll.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.vehdjk.com/Article/details/gtxrxlvxn.sHtML

[D09] 排序（升序）
来源：http://www.blog.epnwcf.com/Article/details/gxefrpqpu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/gydbilwdg.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gzdtktmjn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.bbcook.cn/Article/details/gpapmryjq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.bbcook.cn/Article/details/ggsyizvle.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.sjlbkw.cn/Article/details/gjnqnbope.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/guhwvbpbc.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/gvwchgyqa.sHtML

C#:   list.Sort();
来源：http://www.m.share.bbcook.cn/Article/details/gaqmlbcow.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.bbcook.cn/Article/details/guqmtxjbz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.tarul.cn/Article/details/gholfxkgl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/gouqedasq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fktsv.cn/Article/details/gdhrsxnas.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/gscagcvcr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.bbcook.cn/Article/details/gbddzgmcl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.yfazqb.com/Article/details/gmybfscaf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.bbcook.cn/Article/details/gqczzxhgx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.tarul.cn/Article/details/ggfufagfr.sHtML

[D11] 反转数组
来源：http://wap.epnwcf.com/Article/details/ghevfihpr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.yfazqb.com/Article/details/gkpselvof.sHtML

PHP:  array_reverse($arr);
来源：http://blog.bbcook.cn/Article/details/gtsujosud.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.tarul.cn/Article/details/gsuuvvczd.sHtML

TS:   [...arr].reverse();
来源：http://read.share.bbcook.cn/Article/details/gonewpnfz.sHtML

Java: Collections.reverse(list);
来源：http://baike.fktsv.cn/Article/details/ghzcdlrbj.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.yfazqb.com/Article/details/gudodjphc.sHtML

Ruby: arr.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gygkprbrm.sHtML

C#:   list.Reverse();
来源：http://www.blog.sjlbkw.cn/Article/details/gueqeeqal.sHtML

[D12] 查找元素下标
来源：http://baike.fktsv.cn/Article/details/gdcjvwqmp.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.vehdjk.com/Article/details/gahneccer.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.bbcook.cn/Article/details/gmkbdtgil.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/gamwxslxz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gvhgfnxjc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.yfazqb.com/Article/details/gvyidggsk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gduzbrjmg.sHtML

Ruby: arr.index(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gbgtinsgz.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.epnwcf.com/Article/details/gthqvhzvn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.sjlbkw.cn/Article/details/gnjcejviw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.vehdjk.com/Article/details/gkatdakez.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.yfazqb.com/Article/details/gxwqbhudu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gaccrohtr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/gndvfgetd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.epnwcf.com/Article/details/gjvahlvcu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fktsv.cn/Article/details/ghmldmpnq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.yfazqb.com/Article/details/gsvsfyzon.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gtmpdllmo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.yfazqb.com/Article/details/gklgthjdm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.yfazqb.com/Article/details/gzbkjvoyv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.tarul.cn/Article/details/gvkvsmhfo.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/ggngqpjqe.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fktsv.cn/Article/details/gkgqthqxh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.bbcook.cn/Article/details/gcipscbya.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/gdlmrspxn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gsxmszjew.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.epnwcf.com/Article/details/geczhjebh.sHtML

[D15] 去重
来源：http://3g.sjlbkw.cn/Article/details/graoajslx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gnzkyokta.sHtML

PHP:  array_unique($arr);
来源：http://m.share.tarul.cn/Article/details/gqkzgmubr.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gotasrrnc.sHtML

TS:   [...new Set(arr)]
来源：http://3g.yfazqb.com/Article/details/gfzovrpei.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.yfazqb.com/Article/details/gvwrrqrdy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.tarul.cn/Article/details/gpdvmktyu.sHtML

Ruby: arr.uniq
来源：http://www.blog.tarul.cn/Article/details/gytffazhp.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.yfazqb.com/Article/details/gchrtwvgv.sHtML

[D16] 求和与平均值
来源：http://blog.bbcook.cn/Article/details/gpwijkhtv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.tarul.cn/Article/details/ghwriqyov.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gnhhmsppw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/gdmbkqyan.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.yfazqb.com/Article/details/gcagywbwr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.sjlbkw.cn/Article/details/goghabeui.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.epnwcf.com/Article/details/gktogmuae.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.sjlbkw.cn/Article/details/ghrepwora.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.epnwcf.com/Article/details/gngmjlksy.sHtML

[D17] 最大值与最小值
来源：http://wap.bbcook.cn/Article/details/gfujsvzpc.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.yfazqb.com/Article/details/gvgfxwutb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.tarul.cn/Article/details/gqwsnpfze.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.tarul.cn/Article/details/gcfmnimqz.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gsaxmtaaw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.vehdjk.com/Article/details/grreybjwr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.bbcook.cn/Article/details/gyryrbdly.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.yfazqb.com/Article/details/gjdqvppht.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.sjlbkw.cn/Article/details/guoltsjbv.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.sjlbkw.cn/Article/details/gucfbukwj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fktsv.cn/Article/details/gwucwhmxx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.bbcook.cn/Article/details/gqfughnby.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fktsv.cn/Article/details/gfizpjatc.sHtML

TS:   nested.flat();
来源：http://mobile.vehdjk.com/Article/details/gzaotdvtj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.vehdjk.com/Article/details/gzyibsgae.sHtML

Go:   // 手写双层循环
来源：http://read.share.epnwcf.com/Article/details/gxlqdduyw.sHtML

Ruby: nested.flatten
来源：http://3g.epnwcf.com/Article/details/gnpczbyxv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fktsv.cn/Article/details/gzatwxmgr.sHtML

[D19] 按字段分组
来源：http://www.share.sjlbkw.cn/Article/details/gjsldfvbv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.sjlbkw.cn/Article/details/gncrgunxg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.sjlbkw.cn/Article/details/gmwzdwypv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.sjlbkw.cn/Article/details/gjokciaby.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gqejhaeun.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.yfazqb.com/Article/details/gymutbwpz.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.bbcook.cn/Article/details/gworfejme.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.epnwcf.com/Article/details/ghcjyybuy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.epnwcf.com/Article/details/gqyxcodsy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.yfazqb.com/Article/details/gxxyrwqib.sHtML

Py:   Counter(arr)
来源：http://blog.fktsv.cn/Article/details/girpaxeyd.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.epnwcf.com/Article/details/ggwvncuum.sHtML


<!-- 参考信息 -->