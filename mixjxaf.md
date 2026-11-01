代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.tarul.cn/Article/details/gjszrlmrb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fktsv.cn/Article/details/gwupoeayb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.epnwcf.com/Article/details/glglckkdh.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fktsv.cn/Article/details/gwisjemoq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.vehdjk.com/Article/details/gubdtplmd.sHtML

[C03] 可变参数
来源：http://3g.yfazqb.com/Article/details/gesytgdrw.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fktsv.cn/Article/details/gofvjbtlb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.yfazqb.com/Article/details/glforkret.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.epnwcf.com/Article/details/guwgbdewe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gvjrmgvko.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gfzkoswsd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/gpqjhmmsx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fktsv.cn/Article/details/gzowegrcp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.sjlbkw.cn/Article/details/gzpaoaeqy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.yfazqb.com/Article/details/gvgpigjdk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.yfazqb.com/Article/details/gxztkfpzh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.yfazqb.com/Article/details/gmyjqemjg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/gjxkvaxca.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.yfazqb.com/Article/details/gtnvrjrsw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.yfazqb.com/Article/details/gguftuixb.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.tarul.cn/Article/details/gacebtffg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gntlaltsj.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gciszmrxn.sHtML

[C05] 返回多个值
来源：http://m.share.fktsv.cn/Article/details/goijpkzun.sHtML

Py:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gtwnthquk.sHtML

PHP:  return [$a, $b];
来源：http://wap.sjlbkw.cn/Article/details/ggclqykqz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.bbcook.cn/Article/details/ghmyaczqz.sHtML

TS:   return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gzvpfxdyl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.tarul.cn/Article/details/gbzmprvuz.sHtML

Go:   return a, b
来源：http://blog.bbcook.cn/Article/details/gtbefiimp.sHtML

Ruby: return a, b
来源：http://3g.tarul.cn/Article/details/gztwlxucq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.bbcook.cn/Article/details/ghpbbdpww.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.vehdjk.com/Article/details/glyyxfjdk.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.yfazqb.com/Article/details/gmmfivipt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.epnwcf.com/Article/details/gmtyvewsa.sHtML

JS:   const square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gxzbedsqm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.bbcook.cn/Article/details/gbsgplnyw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.bbcook.cn/Article/details/gapvbtzer.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/galoqxini.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.vehdjk.com/Article/details/gjfxeevkj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.bbcook.cn/Article/details/gqeuthauc.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.yfazqb.com/Article/details/geszwwiyz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.sjlbkw.cn/Article/details/gqxthlail.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gxvdpeven.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.bbcook.cn/Article/details/gqvgmixus.sHtML

TS:   arr.map(String)
来源：http://3g.epnwcf.com/Article/details/gfxsffswd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.sjlbkw.cn/Article/details/givkiqsdb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.bbcook.cn/Article/details/ggbwfjshp.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.tarul.cn/Article/details/gwlkrerim.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.tarul.cn/Article/details/gbybeeror.sHtML

[C08] 闭包
来源：http://3g.tarul.cn/Article/details/gwutdvlnp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.yfazqb.com/Article/details/gnbqhtbqf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fktsv.cn/Article/details/gvyxavkkt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gvgvrtegr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/gsxhlcdvi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fktsv.cn/Article/details/gqhqvfpaw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.epnwcf.com/Article/details/gwmfxveuz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.vehdjk.com/Article/details/gotemkrxt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/grjqdtntg.sHtML

[C09] 递归
来源：http://m.share.fktsv.cn/Article/details/gfmpbztoo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.bbcook.cn/Article/details/gshgpedwq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.vehdjk.com/Article/details/gwpesopkc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/gmmbkupcr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.yfazqb.com/Article/details/ggqxmghoh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fktsv.cn/Article/details/gozjayxto.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.bbcook.cn/Article/details/gnujvcaat.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/ghjiarjjg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.yfazqb.com/Article/details/gbtjqywnc.sHtML

[C10] 变量作用域
来源：http://3g.vehdjk.com/Article/details/gmvujslhu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fktsv.cn/Article/details/gkwmqplms.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.tarul.cn/Article/details/galfcptdw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.vehdjk.com/Article/details/ggoyqcvao.sHtML

TS:   同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gpqsykksn.sHtML

Java: 方法内为块级作用域
来源：http://read.share.vehdjk.com/Article/details/gttvenxvm.sHtML

Go:   花括号块级作用域
来源：http://wap.yfazqb.com/Article/details/gujipdevr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.sjlbkw.cn/Article/details/grdewswfs.sHtML

C#:   块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gvssdwyei.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.epnwcf.com/Article/details/gawprkttm.sHtML

Py:   from module import func
来源：http://www.m.share.bbcook.cn/Article/details/gbxdzgsoz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fktsv.cn/Article/details/gdbkzwskg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/gsmipvazj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.epnwcf.com/Article/details/gzadviarv.sHtML

Java: import java.util.List;
来源：http://www.blog.epnwcf.com/Article/details/ggzlqqemp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.vehdjk.com/Article/details/ghstuhrjm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.bbcook.cn/Article/details/gmcjsvpsb.sHtML

C#:   using System.Text;
来源：http://baike.epnwcf.com/Article/details/gnpxkxyub.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.bbcook.cn/Article/details/gjyavbtnh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fktsv.cn/Article/details/gjbdblirf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.vehdjk.com/Article/details/gmnbqsqcb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.tarul.cn/Article/details/goxibyhow.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.yfazqb.com/Article/details/ghebvjgxi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.bbcook.cn/Article/details/gstbnlfim.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.bbcook.cn/Article/details/gbpshcilk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.yfazqb.com/Article/details/ghfzzzuls.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.yfazqb.com/Article/details/garjsdbtp.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.vehdjk.com/Article/details/gcpzxohac.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.yfazqb.com/Article/details/gcxnsesbf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gfhomprhs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.bbcook.cn/Article/details/gsxpuluyf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.tarul.cn/Article/details/giuisxpph.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gznqcvvau.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fktsv.cn/Article/details/gkuaarfsk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.tarul.cn/Article/details/gyqxytnej.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.sjlbkw.cn/Article/details/gxsdlgbeq.sHtML

[C14] 泛型函数
来源：http://wap.vehdjk.com/Article/details/gxruktszz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.sjlbkw.cn/Article/details/gsqlumbqr.sHtML

PHP:  // 无泛型
来源：http://m.share.vehdjk.com/Article/details/gxxoipyxf.sHtML

JS:   // 无泛型
来源：http://m.share.yfazqb.com/Article/details/grgtupvba.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.vehdjk.com/Article/details/ggazskyxu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.sjlbkw.cn/Article/details/galehlgic.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.bbcook.cn/Article/details/glpgzicql.sHtML

Ruby: # 无泛型
来源：http://3g.yfazqb.com/Article/details/gylrwmdag.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.bbcook.cn/Article/details/garjzucqd.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.epnwcf.com/Article/details/gcbpczlgw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.vehdjk.com/Article/details/gcshailno.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.sjlbkw.cn/Article/details/grrgyvnlo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/gsrjjeorq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.epnwcf.com/Article/details/gguvgdmrq.sHtML

Java: // 无解构
来源：http://3g.tarul.cn/Article/details/gxkjebaxt.sHtML

Go:   // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/gnmjhszxd.sHtML

Ruby: a, b = pair
来源：http://mobile.vehdjk.com/Article/details/gqdlerpza.sHtML

C#:   var (a, b) = pair;
来源：http://baike.tarul.cn/Article/details/gredfyleb.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.tarul.cn/Article/details/gxnphwwwn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.epnwcf.com/Article/details/gkhavbalg.sHtML

PHP:  // 无重载
来源：http://read.share.yfazqb.com/Article/details/gqshnveiu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.vehdjk.com/Article/details/grksbemtv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.vehdjk.com/Article/details/gceplfich.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fktsv.cn/Article/details/gbjucurbw.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.bbcook.cn/Article/details/gtuiczgak.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.yfazqb.com/Article/details/gganzcvcd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.bbcook.cn/Article/details/ggmojfgrw.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gihkituqv.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fktsv.cn/Article/details/gxviofqwo.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gbtrpftzp.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.yfazqb.com/Article/details/gvrdydjxj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.epnwcf.com/Article/details/giorjrptm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/gsrmfcacx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.epnwcf.com/Article/details/gbuvgnvsu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.tarul.cn/Article/details/gbczeoxgw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.tarul.cn/Article/details/giwvonwxu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fktsv.cn/Article/details/gsvjsivxg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.sjlbkw.cn/Article/details/gnpnqdrrz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.epnwcf.com/Article/details/gbbyfcbay.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.tarul.cn/Article/details/gfozhipma.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.epnwcf.com/Article/details/gcapuluui.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.epnwcf.com/Article/details/gflxzrrxr.sHtML

JS:   arr.push(4);
来源：http://www.share.tarul.cn/Article/details/gppfmqwwj.sHtML

TS:   arr.push(4);
来源：http://www.m.share.bbcook.cn/Article/details/gktkzwgsw.sHtML

Java: list.add(4);
来源：http://3g.epnwcf.com/Article/details/gtndplrfu.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.tarul.cn/Article/details/gkhdmylav.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.epnwcf.com/Article/details/gobrfwmhi.sHtML

C#:   list.Add(4);
来源：http://m.share.bbcook.cn/Article/details/ggdvpfqxd.sHtML

[D03] 在指定位置插入元素
来源：http://3g.sjlbkw.cn/Article/details/gbfvntfrh.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.vehdjk.com/Article/details/glcjgmndz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.bbcook.cn/Article/details/grjlsqbgi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.vehdjk.com/Article/details/giefazjhx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.epnwcf.com/Article/details/gbyflhcyy.sHtML

Java: list.add(0, 0);
来源：http://mobile.fktsv.cn/Article/details/guuvsglcq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.vehdjk.com/Article/details/gzexehiud.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fktsv.cn/Article/details/gbindtkoh.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.bbcook.cn/Article/details/gneysrnfg.sHtML

[D04] 删除元素
来源：http://m.share.yfazqb.com/Article/details/golrarcti.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.epnwcf.com/Article/details/gdhgqptrc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.tarul.cn/Article/details/gsgytzwin.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.tarul.cn/Article/details/gzhhajavl.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.bbcook.cn/Article/details/gggegpeye.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.yfazqb.com/Article/details/gdeeihspf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.yfazqb.com/Article/details/gyrjqffow.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.yfazqb.com/Article/details/gpxhghubh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.epnwcf.com/Article/details/gdxvbkfra.sHtML

[D05] 访问与修改元素
来源：http://baike.fktsv.cn/Article/details/gpslrgtum.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gallhkdzr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gsvytxyoy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gfsezoccc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.yfazqb.com/Article/details/gfmddnebg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.epnwcf.com/Article/details/gehmbyqbu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/giajnhvgt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/gprdmtbco.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.tarul.cn/Article/details/gilxpunjf.sHtML

[D06] 数组长度
来源：http://mobile.fktsv.cn/Article/details/gpojuvdhb.sHtML

Py:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/ghpufzoac.sHtML

PHP:  count($arr);
来源：http://wap.epnwcf.com/Article/details/gndzndtpg.sHtML

JS:   arr.length
来源：http://baike.fktsv.cn/Article/details/giugzqorm.sHtML

TS:   arr.length
来源：http://baike.yfazqb.com/Article/details/gstqkqvkv.sHtML

Java: list.size();
来源：http://m.share.vehdjk.com/Article/details/gghikxala.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gospjaybc.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.tarul.cn/Article/details/gkvxtblej.sHtML

C#:   list.Count;
来源：http://baike.vehdjk.com/Article/details/gnbrjgwqy.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.vehdjk.com/Article/details/gytdczdlv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.bbcook.cn/Article/details/gzoxdjvhd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fktsv.cn/Article/details/gybhddxpa.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gwpgxemcz.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gmbuyvtpj.sHtML

Java: list.subList(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gaeskqgrt.sHtML

Go:   arr[1:4]
来源：http://www.blog.sjlbkw.cn/Article/details/ggnjqfulx.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.bbcook.cn/Article/details/grrnmhyot.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.bbcook.cn/Article/details/gnlxiopyf.sHtML

[D08] 合并两个数组
来源：http://3g.fktsv.cn/Article/details/ggpjwjleh.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.epnwcf.com/Article/details/glbrjzezn.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.vehdjk.com/Article/details/gnqnzixvp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.sjlbkw.cn/Article/details/gfolyqtvf.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fktsv.cn/Article/details/gurjivalm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gvlcsixwb.sHtML

Go:   append(a, b...)
来源：http://wap.yfazqb.com/Article/details/gurvleqwa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.sjlbkw.cn/Article/details/groiqxicn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.tarul.cn/Article/details/gferlrcvp.sHtML

[D09] 排序（升序）
来源：http://wap.tarul.cn/Article/details/gipodzibu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/gcrbzxual.sHtML

PHP:  sort($arr);
来源：http://www.blog.epnwcf.com/Article/details/ghuhczrep.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.bbcook.cn/Article/details/gcycmdjhz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.bbcook.cn/Article/details/gskwxsrrm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.sjlbkw.cn/Article/details/gezsajzjk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gbsrhrbrg.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/gydyxgdln.sHtML

C#:   list.Sort();
来源：http://blog.epnwcf.com/Article/details/gydcjbhzq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.tarul.cn/Article/details/gusrhocyt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.yfazqb.com/Article/details/gsrhtkhcq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.tarul.cn/Article/details/gurwknwnv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/gtexoknnt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.vehdjk.com/Article/details/gnhgpkhbe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.epnwcf.com/Article/details/gdybvovkc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fktsv.cn/Article/details/gzmowokfq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.vehdjk.com/Article/details/ggtifsvwo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.yfazqb.com/Article/details/gwtvlnoka.sHtML

[D11] 反转数组
来源：http://www.blog.yfazqb.com/Article/details/gtlokzzct.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.bbcook.cn/Article/details/gykxuiexq.sHtML

PHP:  array_reverse($arr);
来源：http://baike.bbcook.cn/Article/details/gmrxjqkyc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.tarul.cn/Article/details/ghspistqe.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fktsv.cn/Article/details/gsaglrgys.sHtML

Java: Collections.reverse(list);
来源：http://baike.sjlbkw.cn/Article/details/ghgetvpsp.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gghrzdqqk.sHtML

Ruby: arr.reverse
来源：http://blog.fktsv.cn/Article/details/gcyytlmar.sHtML

C#:   list.Reverse();
来源：http://www.blog.yfazqb.com/Article/details/gdkruavkg.sHtML

[D12] 查找元素下标
来源：http://www.share.sjlbkw.cn/Article/details/gxjurhnrd.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.sjlbkw.cn/Article/details/gwelijuqi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.tarul.cn/Article/details/gihwhetlm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/gufogrwvq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.bbcook.cn/Article/details/ghtvkhxoj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.epnwcf.com/Article/details/gapawrxbf.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.yfazqb.com/Article/details/gtjqtgyrp.sHtML

Ruby: arr.index(x)
来源：http://baike.tarul.cn/Article/details/ggfmxrhhl.sHtML

C#:   list.IndexOf(x);
来源：http://baike.epnwcf.com/Article/details/gmtmjcjhh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.bbcook.cn/Article/details/goyjdchwc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.epnwcf.com/Article/details/gjngjxuey.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.bbcook.cn/Article/details/gmmztsdty.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/gflzjxlna.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwpspbnz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.vehdjk.com/Article/details/goomsowwq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.bbcook.cn/Article/details/gxfvlebjp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fktsv.cn/Article/details/grdmegmss.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.epnwcf.com/Article/details/gsqmssung.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.epnwcf.com/Article/details/gseokxlwk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.tarul.cn/Article/details/gfoksgfpg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.yfazqb.com/Article/details/gpbcrxpgv.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/godzdmaen.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/gxsyzmvyv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gusvnjbnc.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gychuspfe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.tarul.cn/Article/details/gaoaneszs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.yfazqb.com/Article/details/grecobhdl.sHtML

[D15] 去重
来源：http://wap.tarul.cn/Article/details/gsmswmkdb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gqvgxgoxo.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/gvfgxpfib.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gpxlcagek.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/gzoyvdqog.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.sjlbkw.cn/Article/details/gnbhrvpnk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.epnwcf.com/Article/details/gfvqunhas.sHtML

Ruby: arr.uniq
来源：http://wap.vehdjk.com/Article/details/gyhrktruq.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.tarul.cn/Article/details/glhslebfx.sHtML

[D16] 求和与平均值
来源：http://www.share.tarul.cn/Article/details/gcgvqfsdq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.yfazqb.com/Article/details/goaieqffr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.epnwcf.com/Article/details/gnoevkqsb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gljtixldg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/gcopjmyez.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fktsv.cn/Article/details/ghuxjxrwp.sHtML

Go:   // 手写循环累加
来源：http://m.share.fktsv.cn/Article/details/gedivizfk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.tarul.cn/Article/details/gmiiceboq.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.epnwcf.com/Article/details/gvmdgczfs.sHtML

[D17] 最大值与最小值
来源：http://www.share.vehdjk.com/Article/details/gnkbzxxga.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.yfazqb.com/Article/details/gohpdljnm.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.vehdjk.com/Article/details/gldzejjnn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.yfazqb.com/Article/details/gdujuipvg.sHtML

TS:   Math.max(...arr);
来源：http://www.share.tarul.cn/Article/details/giocqsgzt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.yfazqb.com/Article/details/gztzuyndm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.yfazqb.com/Article/details/geoirqttd.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.epnwcf.com/Article/details/gdexownit.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.vehdjk.com/Article/details/gjeuexpoy.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.vehdjk.com/Article/details/gxqzykcjk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.sjlbkw.cn/Article/details/gqekhcutd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.vehdjk.com/Article/details/gnvewjyav.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.sjlbkw.cn/Article/details/gtyrdixqi.sHtML

TS:   nested.flat();
来源：http://baike.sjlbkw.cn/Article/details/gqsipebyy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.yfazqb.com/Article/details/gnzvknwzz.sHtML

Go:   // 手写双层循环
来源：http://read.share.sjlbkw.cn/Article/details/gbiwtnpxh.sHtML

Ruby: nested.flatten
来源：http://wap.vehdjk.com/Article/details/gikybfrkm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.epnwcf.com/Article/details/gcvsckqqv.sHtML

[D19] 按字段分组
来源：http://www.share.fktsv.cn/Article/details/gmfpnyxzl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.tarul.cn/Article/details/gbiyanegu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.vehdjk.com/Article/details/gfgvabcmc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.yfazqb.com/Article/details/gszqrlkmk.sHtML


<!-- 参考信息 -->