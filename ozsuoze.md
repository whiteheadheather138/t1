代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://blog.bbcook.cn/Article/details/gqnkuwnzx.sHtML

[C03] 可变参数
来源：http://www.blog.epnwcf.com/Article/details/gdllvwfvq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.yfazqb.com/Article/details/gblvquwmb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fktsv.cn/Article/details/gpxcnaeem.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/gaffmxelv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gcqpwfigu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.vehdjk.com/Article/details/gscpzorvu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.bbcook.cn/Article/details/gdxdyzchz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.bbcook.cn/Article/details/grlegizdx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnizehpy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.sjlbkw.cn/Article/details/gpgzxtpho.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fktsv.cn/Article/details/gqsirtvqr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.yfazqb.com/Article/details/gdcgmtisf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/gbqxayzyb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.bbcook.cn/Article/details/gqtcrpxfn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.sjlbkw.cn/Article/details/gsofihmuv.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.yfazqb.com/Article/details/gxvntdfpv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/gujolwzcu.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gxnsvqfvb.sHtML

[C05] 返回多个值
来源：http://3g.bbcook.cn/Article/details/glavqnryf.sHtML

Py:   return a, b
来源：http://www.blog.yfazqb.com/Article/details/gxhtzknge.sHtML

PHP:  return [$a, $b];
来源：http://wap.tarul.cn/Article/details/gorxfbvtd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.bbcook.cn/Article/details/gbxbtwmqv.sHtML

TS:   return { a, b };
来源：http://mobile.vehdjk.com/Article/details/gyutqsdsj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fktsv.cn/Article/details/gbbgwvwkm.sHtML

Go:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gputnfqqv.sHtML

Ruby: return a, b
来源：http://www.blog.bbcook.cn/Article/details/gegezuyro.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fktsv.cn/Article/details/gzowwpjqk.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.yfazqb.com/Article/details/grqhnxhii.sHtML

Py:   square = lambda x: x * x
来源：http://blog.bbcook.cn/Article/details/gyzgzwpsd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.vehdjk.com/Article/details/gafkhytmj.sHtML

JS:   const square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/greomxcfw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fktsv.cn/Article/details/gwpjmgfhp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.yfazqb.com/Article/details/gpgtoyvmz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fktsv.cn/Article/details/gyafojzvc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.tarul.cn/Article/details/gkzhsqhoz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gpmpevelv.sHtML

[C07] 把函数作为参数传入
来源：http://baike.bbcook.cn/Article/details/ghpqparnz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.yfazqb.com/Article/details/ggolpdqpn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.vehdjk.com/Article/details/gzjpnrslv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.yfazqb.com/Article/details/gokkgvbqc.sHtML

TS:   arr.map(String)
来源：http://blog.yfazqb.com/Article/details/gcaqnbuwx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gopzhznvj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.vehdjk.com/Article/details/gqsylasph.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.vehdjk.com/Article/details/gwkpfroqn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.bbcook.cn/Article/details/guzfvalfe.sHtML

[C08] 闭包
来源：http://mobile.fktsv.cn/Article/details/gkcolgdgj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.bbcook.cn/Article/details/gwrreybpp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.bbcook.cn/Article/details/glqwzarqj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gfifbdspd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gkpooyuqh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.vehdjk.com/Article/details/gzytxequx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.vehdjk.com/Article/details/goqsmawqb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/gccelpljb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gcbhktkeu.sHtML

[C09] 递归
来源：http://www.share.epnwcf.com/Article/details/gngjwxukl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gpljgzcaz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.vehdjk.com/Article/details/gnzfdfmff.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gksvyrslq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gitsohtvi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.tarul.cn/Article/details/gajeperqn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.yfazqb.com/Article/details/gaumlggle.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/gyqttaamm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.vehdjk.com/Article/details/ggqnwrzzt.sHtML

[C10] 变量作用域
来源：http://3g.bbcook.cn/Article/details/gffwfbklt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.tarul.cn/Article/details/guiklfdke.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fktsv.cn/Article/details/gxvighgxq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.bbcook.cn/Article/details/gsahtjdzg.sHtML

TS:   同 JS
来源：http://baike.tarul.cn/Article/details/gjselyxim.sHtML

Java: 方法内为块级作用域
来源：http://blog.vehdjk.com/Article/details/ghpbiutds.sHtML

Go:   花括号块级作用域
来源：http://www.share.fktsv.cn/Article/details/gzndebmka.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.bbcook.cn/Article/details/gqoypgbnt.sHtML

C#:   块级作用域
来源：http://3g.yfazqb.com/Article/details/gwvqsizek.sHtML

[C11] 模块导入与导出
来源：http://www.blog.yfazqb.com/Article/details/gyhdnxqah.sHtML

Py:   from module import func
来源：http://baike.tarul.cn/Article/details/gurxmieyq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.tarul.cn/Article/details/gsltjsxgp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/gfmxmhnot.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.epnwcf.com/Article/details/gklioltxx.sHtML

Java: import java.util.List;
来源：http://blog.epnwcf.com/Article/details/gxxhkvnde.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.sjlbkw.cn/Article/details/gwxfssdbj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.tarul.cn/Article/details/gxtjivgwh.sHtML

C#:   using System.Text;
来源：http://baike.fktsv.cn/Article/details/gihtaljds.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.epnwcf.com/Article/details/gruqxhgyr.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.sjlbkw.cn/Article/details/gdtsdlvmh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.sjlbkw.cn/Article/details/gmencakfo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.vehdjk.com/Article/details/ghwwlfcqr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/gjyqbxylm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.sjlbkw.cn/Article/details/gfatismao.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fktsv.cn/Article/details/gdvdddari.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.yfazqb.com/Article/details/ghkejcozc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.bbcook.cn/Article/details/gekbjvdas.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.tarul.cn/Article/details/gmegkhdgv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.epnwcf.com/Article/details/gfecoreui.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gwkiohjrh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.tarul.cn/Article/details/gxdfffuhw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gjrpafdrk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gwswjoerx.sHtML

Go:   func add(a, b int) int
来源：http://baike.yfazqb.com/Article/details/gbkflvhza.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.tarul.cn/Article/details/gxxfahwwd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.epnwcf.com/Article/details/gzwqpbmbe.sHtML

[C14] 泛型函数
来源：http://www.share.bbcook.cn/Article/details/gqagswzoc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.vehdjk.com/Article/details/gmrxubtvu.sHtML

PHP:  // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gbkshzfka.sHtML

JS:   // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gpymvfgrm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.vehdjk.com/Article/details/gtniysiuu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.bbcook.cn/Article/details/gzpnfztaq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.sjlbkw.cn/Article/details/gvgdwztqr.sHtML

Ruby: # 无泛型
来源：http://mobile.vehdjk.com/Article/details/gfflkgnlf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.vehdjk.com/Article/details/gnhakmcfa.sHtML

[C15] 解构 / 展开参数
来源：http://baike.sjlbkw.cn/Article/details/gqlmmdotp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.tarul.cn/Article/details/gvewdlcrw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.sjlbkw.cn/Article/details/gxdakfonh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/ggktjdguo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.bbcook.cn/Article/details/gjpahlsbw.sHtML

Java: // 无解构
来源：http://m.share.fktsv.cn/Article/details/gxxbzsrpl.sHtML

Go:   // 无解构
来源：http://read.share.epnwcf.com/Article/details/gwfscpqzg.sHtML

Ruby: a, b = pair
来源：http://www.share.epnwcf.com/Article/details/gkyvuwgci.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fktsv.cn/Article/details/gwgoqvkhg.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fktsv.cn/Article/details/grmejhbtm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.sjlbkw.cn/Article/details/ghwvwtffm.sHtML

PHP:  // 无重载
来源：http://www.share.fktsv.cn/Article/details/gaxithkht.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fktsv.cn/Article/details/giymqnomk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.epnwcf.com/Article/details/gozmbwtsx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.epnwcf.com/Article/details/gdpnbsyzm.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.epnwcf.com/Article/details/gjzvlqdzo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.tarul.cn/Article/details/gmnpveplh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.yfazqb.com/Article/details/glqlayjmr.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gbzfdctfu.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fktsv.cn/Article/details/gmudblynn.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ggoqdndaw.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/gykdpruyj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.tarul.cn/Article/details/gjegbhpcj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.epnwcf.com/Article/details/grfcmwqsi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gwvxayknq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.epnwcf.com/Article/details/gmazqhusq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fktsv.cn/Article/details/gsykmyygb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.sjlbkw.cn/Article/details/gipasfevj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.yfazqb.com/Article/details/gufouznzx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.sjlbkw.cn/Article/details/gnzdgdkax.sHtML

[D02] 追加元素到末尾
来源：http://3g.vehdjk.com/Article/details/glcpvlvmb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.sjlbkw.cn/Article/details/gfbahtycd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.tarul.cn/Article/details/gmhoujtrn.sHtML

JS:   arr.push(4);
来源：http://m.share.bbcook.cn/Article/details/gcufhovhl.sHtML

TS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/grxiyirhq.sHtML

Java: list.add(4);
来源：http://blog.bbcook.cn/Article/details/gdtsfqlla.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.tarul.cn/Article/details/gwtmfcilw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.tarul.cn/Article/details/gfcxwpehh.sHtML

C#:   list.Add(4);
来源：http://m.share.sjlbkw.cn/Article/details/gcfpojjzx.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.vehdjk.com/Article/details/gntjmwzln.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fktsv.cn/Article/details/gdxlllphk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.sjlbkw.cn/Article/details/gzfjehyky.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.epnwcf.com/Article/details/gkoaanfjw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gwnvjuiig.sHtML

Java: list.add(0, 0);
来源：http://wap.epnwcf.com/Article/details/gaigmvglj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.sjlbkw.cn/Article/details/gkxahdveq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.bbcook.cn/Article/details/gimhxmnlk.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.bbcook.cn/Article/details/ghxyjzkwa.sHtML

[D04] 删除元素
来源：http://wap.vehdjk.com/Article/details/gwmeafzgy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.sjlbkw.cn/Article/details/gbdqsafcn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.bbcook.cn/Article/details/guaxtwohx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.vehdjk.com/Article/details/gnqoctfsc.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.sjlbkw.cn/Article/details/gfykubmbc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fktsv.cn/Article/details/gtpmxijet.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.tarul.cn/Article/details/gvuegagfq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fktsv.cn/Article/details/giddljvyp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.bbcook.cn/Article/details/gugifspfm.sHtML

[D05] 访问与修改元素
来源：http://baike.vehdjk.com/Article/details/gslxztpic.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/glwtqizoy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fktsv.cn/Article/details/geqzslpsu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gijxaemwd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.vehdjk.com/Article/details/gkmartokj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fktsv.cn/Article/details/ghnzjyqac.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/grgefsbzq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gkrgpldjb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/grhurqadh.sHtML

[D06] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/gnjnpuyty.sHtML

Py:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/ggxxkupnn.sHtML

PHP:  count($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gkbxmsxlm.sHtML

JS:   arr.length
来源：http://www.blog.fktsv.cn/Article/details/gspidhrey.sHtML

TS:   arr.length
来源：http://blog.epnwcf.com/Article/details/ggaxfceob.sHtML

Java: list.size();
来源：http://wap.tarul.cn/Article/details/gvnqrzllz.sHtML

Go:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/gnrkwboob.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.tarul.cn/Article/details/gifmpcstb.sHtML

C#:   list.Count;
来源：http://www.m.share.tarul.cn/Article/details/ggxkjcwuw.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fktsv.cn/Article/details/giverwmla.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.bbcook.cn/Article/details/gsrfyccux.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fktsv.cn/Article/details/godmgdkzm.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gcglfurir.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/gcxvmplch.sHtML

Java: list.subList(1, 4);
来源：http://wap.tarul.cn/Article/details/gamxzbbou.sHtML

Go:   arr[1:4]
来源：http://blog.sjlbkw.cn/Article/details/gyqmkpetr.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.bbcook.cn/Article/details/ghmlaulos.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.yfazqb.com/Article/details/gcyizwqyk.sHtML

[D08] 合并两个数组
来源：http://mobile.tarul.cn/Article/details/guiofqvpp.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fktsv.cn/Article/details/grpkweltg.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.yfazqb.com/Article/details/gokezotlr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.epnwcf.com/Article/details/gqehnolst.sHtML

TS:   [...a, ...b];
来源：http://blog.epnwcf.com/Article/details/guznsfrge.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.epnwcf.com/Article/details/gkkhmpplf.sHtML

Go:   append(a, b...)
来源：http://www.share.epnwcf.com/Article/details/ghticjqzv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.vehdjk.com/Article/details/gqfunzmxc.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gbkahbdbn.sHtML

[D09] 排序（升序）
来源：http://www.blog.vehdjk.com/Article/details/gxyxbtftm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gqcqzdmbz.sHtML

PHP:  sort($arr);
来源：http://m.share.epnwcf.com/Article/details/gopvcanrj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.epnwcf.com/Article/details/gacvrefjw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.bbcook.cn/Article/details/gynlnwssg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.sjlbkw.cn/Article/details/gfuopvkar.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gbfbhyani.sHtML

Ruby: arr.sort
来源：http://baike.yfazqb.com/Article/details/gdczjkjbh.sHtML

C#:   list.Sort();
来源：http://wap.tarul.cn/Article/details/gjcvoiway.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.yfazqb.com/Article/details/gfnndjuhd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.epnwcf.com/Article/details/goeutlhrl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.tarul.cn/Article/details/gklysrzme.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/gclqxrecj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/gyvxralma.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.tarul.cn/Article/details/gcanfialk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.bbcook.cn/Article/details/gixbuvsem.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.epnwcf.com/Article/details/ghqnsjpgl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.sjlbkw.cn/Article/details/gjpquyxcl.sHtML

[D11] 反转数组
来源：http://www.m.share.tarul.cn/Article/details/gvrtlbcot.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.yfazqb.com/Article/details/gaknqvlmq.sHtML

PHP:  array_reverse($arr);
来源：http://3g.vehdjk.com/Article/details/gmzkmgjzq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.yfazqb.com/Article/details/griefzpno.sHtML

TS:   [...arr].reverse();
来源：http://wap.fktsv.cn/Article/details/gtvjzeiov.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fktsv.cn/Article/details/gypvvumnf.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.sjlbkw.cn/Article/details/golulrxgc.sHtML

Ruby: arr.reverse
来源：http://www.blog.vehdjk.com/Article/details/gxzysuqmj.sHtML

C#:   list.Reverse();
来源：http://blog.vehdjk.com/Article/details/gienfioua.sHtML

[D12] 查找元素下标
来源：http://mobile.vehdjk.com/Article/details/grinozmlb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.sjlbkw.cn/Article/details/gakgwwheb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.sjlbkw.cn/Article/details/gkjjrcrhb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.tarul.cn/Article/details/gfcgqunnp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.epnwcf.com/Article/details/gftlsigwd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.vehdjk.com/Article/details/gfnnrogbj.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/grrhtbndb.sHtML

Ruby: arr.index(x)
来源：http://baike.vehdjk.com/Article/details/gnzuigyvb.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.tarul.cn/Article/details/gnrjmirii.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.epnwcf.com/Article/details/givmuzmkp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gcarbsrzm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.sjlbkw.cn/Article/details/gczaokbnb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.tarul.cn/Article/details/gxgklubcc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gpikjqvgl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.epnwcf.com/Article/details/gcjrakzmy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fktsv.cn/Article/details/gtwkvdurc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.sjlbkw.cn/Article/details/ghvikvhop.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fktsv.cn/Article/details/ghrngnhhc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/gakaubmqf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.vehdjk.com/Article/details/giimdlcmy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gcphsjhfx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/gmheopfsn.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.sjlbkw.cn/Article/details/gklkxbupd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.yfazqb.com/Article/details/gpwetqllw.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/gipxybqju.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gmpnkrmpk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.epnwcf.com/Article/details/geeqqksbw.sHtML

[D15] 去重
来源：http://www.share.tarul.cn/Article/details/gswukjaja.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gapfjlcmi.sHtML

PHP:  array_unique($arr);
来源：http://wap.vehdjk.com/Article/details/gpqwnzjyu.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gajnitoui.sHtML

TS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gogxycbml.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.yfazqb.com/Article/details/gxjdcdiyd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.sjlbkw.cn/Article/details/gzpzzmdwi.sHtML

Ruby: arr.uniq
来源：http://www.share.sjlbkw.cn/Article/details/gketfakra.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fktsv.cn/Article/details/gzdlbmbgn.sHtML

[D16] 求和与平均值
来源：http://mobile.epnwcf.com/Article/details/gnqzzpobe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gxbnepuuq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.vehdjk.com/Article/details/glooqfqri.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/gpknjjpmq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gufnklsdv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.tarul.cn/Article/details/gvzhyvmaz.sHtML

Go:   // 手写循环累加
来源：http://baike.fktsv.cn/Article/details/gnqqiwyli.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.epnwcf.com/Article/details/gofnxrxte.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.tarul.cn/Article/details/gxarwamph.sHtML

[D17] 最大值与最小值
来源：http://wap.yfazqb.com/Article/details/ghlvxweve.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fktsv.cn/Article/details/gwoqapqwf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsafckfh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.yfazqb.com/Article/details/giyxwvbrp.sHtML

TS:   Math.max(...arr);
来源：http://mobile.epnwcf.com/Article/details/gdkcpwveo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.sjlbkw.cn/Article/details/gpcajinuk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.bbcook.cn/Article/details/gjcckyfdg.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.sjlbkw.cn/Article/details/gxnfdjrox.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fktsv.cn/Article/details/gfrvdmrmy.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.bbcook.cn/Article/details/gozjhfkpd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.bbcook.cn/Article/details/goeipsllb.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.epnwcf.com/Article/details/gqivmnvkc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.yfazqb.com/Article/details/goswixbsz.sHtML

TS:   nested.flat();
来源：http://www.blog.sjlbkw.cn/Article/details/gpchicmga.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.tarul.cn/Article/details/gmmgdoxtj.sHtML

Go:   // 手写双层循环
来源：http://www.blog.tarul.cn/Article/details/gkqkvvhvo.sHtML

Ruby: nested.flatten
来源：http://3g.tarul.cn/Article/details/grjlbicwp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gkaumtftq.sHtML

[D19] 按字段分组
来源：http://mobile.yfazqb.com/Article/details/gkatmhfyb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fktsv.cn/Article/details/ghphxafvo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.sjlbkw.cn/Article/details/gjxhtdqwa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.vehdjk.com/Article/details/gboxkzjbw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.epnwcf.com/Article/details/gmyebghas.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fktsv.cn/Article/details/gbegcklns.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.sjlbkw.cn/Article/details/glmbpfbmb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.epnwcf.com/Article/details/gmjezvmjv.sHtML


<!-- 参考信息 -->