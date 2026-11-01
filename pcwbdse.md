代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fktsv.cn/Article/details/geakvnivc.sHtML

[C03] 可变参数
来源：http://read.share.vehdjk.com/Article/details/gkrxucgsz.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.yfazqb.com/Article/details/gykeuyyij.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.vehdjk.com/Article/details/grcqjfkbk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.bbcook.cn/Article/details/ghdopwryx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/gflwpotke.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fktsv.cn/Article/details/gxehhbruv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fktsv.cn/Article/details/grdzzqnih.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.vehdjk.com/Article/details/gnwxomeed.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.sjlbkw.cn/Article/details/gmpntgejo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.bbcook.cn/Article/details/gaiggssuk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.bbcook.cn/Article/details/glxvgwpxp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.epnwcf.com/Article/details/gkddfjtqu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.bbcook.cn/Article/details/gfncpsfjq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fktsv.cn/Article/details/gafhntkte.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.sjlbkw.cn/Article/details/ggxaapvob.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.sjlbkw.cn/Article/details/gdyulkavs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gwqjqpjwa.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/gxbuyhfen.sHtML

[C05] 返回多个值
来源：http://www.m.share.vehdjk.com/Article/details/gfuskzqyw.sHtML

Py:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gvhdmvuzd.sHtML

PHP:  return [$a, $b];
来源：http://mobile.epnwcf.com/Article/details/gopgzkwih.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fktsv.cn/Article/details/gfgmfrgxt.sHtML

TS:   return { a, b };
来源：http://www.m.share.vehdjk.com/Article/details/gvemsonvv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.vehdjk.com/Article/details/gdfchpgkk.sHtML

Go:   return a, b
来源：http://baike.vehdjk.com/Article/details/gmmcksior.sHtML

Ruby: return a, b
来源：http://wap.bbcook.cn/Article/details/grlaguowc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.sjlbkw.cn/Article/details/gjjaahaxf.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.vehdjk.com/Article/details/gopctvryc.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fktsv.cn/Article/details/gjzscwqrf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.epnwcf.com/Article/details/gvpnetqny.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/glaarysdu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gliaojpdc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.epnwcf.com/Article/details/gyuyjwjnq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.vehdjk.com/Article/details/gqjigpdpe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.tarul.cn/Article/details/gainsigfb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.bbcook.cn/Article/details/gmwyoqxxx.sHtML

[C07] 把函数作为参数传入
来源：http://3g.epnwcf.com/Article/details/gmimepbla.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtxgkwrg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.epnwcf.com/Article/details/gxqcijhgo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.epnwcf.com/Article/details/gfceuzqdf.sHtML

TS:   arr.map(String)
来源：http://blog.epnwcf.com/Article/details/gkhzlpjaq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.sjlbkw.cn/Article/details/gucezcekl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.vehdjk.com/Article/details/goksvkhie.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.yfazqb.com/Article/details/gvremgvxr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.yfazqb.com/Article/details/gjpfnjifh.sHtML

[C08] 闭包
来源：http://wap.bbcook.cn/Article/details/gkvjgsgoy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.sjlbkw.cn/Article/details/gimyzdhul.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.bbcook.cn/Article/details/gyofrioip.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gbbljtkvr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gomeasuaz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.bbcook.cn/Article/details/gixadojed.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.yfazqb.com/Article/details/grxvdwrnu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.epnwcf.com/Article/details/gkstmromr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gezhohibv.sHtML

[C09] 递归
来源：http://wap.sjlbkw.cn/Article/details/guahiddqi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fktsv.cn/Article/details/gdykpbtff.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.epnwcf.com/Article/details/gltywkvlm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/gkaovbreu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/geyrbfvhv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.epnwcf.com/Article/details/grxxuxoaq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.tarul.cn/Article/details/guegaylyy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gapntuicz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.sjlbkw.cn/Article/details/gtdqydjdn.sHtML

[C10] 变量作用域
来源：http://www.blog.bbcook.cn/Article/details/gfwqjpdkv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.sjlbkw.cn/Article/details/gwdwmjoqd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.tarul.cn/Article/details/georghiun.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.epnwcf.com/Article/details/guqnphuxb.sHtML

TS:   同 JS
来源：http://blog.epnwcf.com/Article/details/gygavjhlp.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fktsv.cn/Article/details/gwgsolaot.sHtML

Go:   花括号块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gggyxxxst.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.yfazqb.com/Article/details/gzwetlady.sHtML

C#:   块级作用域
来源：http://blog.vehdjk.com/Article/details/gfytdgxuz.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.tarul.cn/Article/details/gnzvxqyan.sHtML

Py:   from module import func
来源：http://3g.sjlbkw.cn/Article/details/gpsflsbzt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.epnwcf.com/Article/details/gcdftyoci.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.epnwcf.com/Article/details/gawkudbqn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.sjlbkw.cn/Article/details/gemmmfwit.sHtML

Java: import java.util.List;
来源：http://www.blog.tarul.cn/Article/details/gccjmwqdf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.bbcook.cn/Article/details/gghbsvcml.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.epnwcf.com/Article/details/gveflaqkq.sHtML

C#:   using System.Text;
来源：http://blog.bbcook.cn/Article/details/gxmfrbgqf.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.bbcook.cn/Article/details/gxlugaqsg.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.epnwcf.com/Article/details/gqfykohhc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.yfazqb.com/Article/details/gyibxkikd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/grbhmcwkt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/gkyfcdmwl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.bbcook.cn/Article/details/gzaecskdu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.vehdjk.com/Article/details/gvvudetgw.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.vehdjk.com/Article/details/ghjfjegfi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.bbcook.cn/Article/details/ghaeeneny.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fktsv.cn/Article/details/gcruxzvpw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gawtmdtbq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/glvfmtpvl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.yfazqb.com/Article/details/gojvbjqxl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gqjiwgvnf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gozjzhrze.sHtML

Go:   func add(a, b int) int
来源：http://mobile.yfazqb.com/Article/details/grxeptstv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.yfazqb.com/Article/details/gpsjobhqa.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.epnwcf.com/Article/details/gknghnqby.sHtML

[C14] 泛型函数
来源：http://mobile.fktsv.cn/Article/details/gkefluhpw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.tarul.cn/Article/details/gqncvmtuk.sHtML

PHP:  // 无泛型
来源：http://m.share.bbcook.cn/Article/details/gldmiqmel.sHtML

JS:   // 无泛型
来源：http://www.share.fktsv.cn/Article/details/gzgnczzni.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.vehdjk.com/Article/details/gjevfclhc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.yfazqb.com/Article/details/genvjpoik.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fktsv.cn/Article/details/gvgwxjmvt.sHtML

Ruby: # 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gimmpxifw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fktsv.cn/Article/details/gjymohziv.sHtML

[C15] 解构 / 展开参数
来源：http://baike.bbcook.cn/Article/details/gvbijwznq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fktsv.cn/Article/details/gkivciqdt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.bbcook.cn/Article/details/govqpdlfa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/gvemcokgj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.bbcook.cn/Article/details/ghmpxtnrq.sHtML

Java: // 无解构
来源：http://blog.epnwcf.com/Article/details/gnadcujdd.sHtML

Go:   // 无解构
来源：http://read.share.vehdjk.com/Article/details/gwwckyipg.sHtML

Ruby: a, b = pair
来源：http://baike.bbcook.cn/Article/details/gfztpdeow.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.vehdjk.com/Article/details/gakmsdjvt.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.sjlbkw.cn/Article/details/gsoczkwar.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.epnwcf.com/Article/details/gwhxamxyi.sHtML

PHP:  // 无重载
来源：http://wap.sjlbkw.cn/Article/details/gziltvdtl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.tarul.cn/Article/details/gszcgtqck.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.vehdjk.com/Article/details/gzwmcfsvz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.tarul.cn/Article/details/gepwkntri.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.sjlbkw.cn/Article/details/gnycyhseh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.tarul.cn/Article/details/gklkyflrr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.yfazqb.com/Article/details/gorprxiud.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwmyfthqy.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.sjlbkw.cn/Article/details/ghyinttoh.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmuocscbx.sHtML

[D01] 创建数组 / 列表
来源：http://blog.bbcook.cn/Article/details/gykcbcvac.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.vehdjk.com/Article/details/gbmiwcoan.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.bbcook.cn/Article/details/gnhigfwfu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gttfyctdo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.yfazqb.com/Article/details/gchvumkoa.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.epnwcf.com/Article/details/gmfyiiase.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.bbcook.cn/Article/details/gztedxgkr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.bbcook.cn/Article/details/gszzynyhb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.tarul.cn/Article/details/gzwkbzlso.sHtML

[D02] 追加元素到末尾
来源：http://baike.fktsv.cn/Article/details/gnitnmefr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fktsv.cn/Article/details/gojragoco.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.tarul.cn/Article/details/ggpqdkray.sHtML

JS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/gsmjgoqvs.sHtML

TS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/gonblisar.sHtML

Java: list.add(4);
来源：http://3g.fktsv.cn/Article/details/gwxibbesq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.tarul.cn/Article/details/gdcrdmbmr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.bbcook.cn/Article/details/gfijehndk.sHtML

C#:   list.Add(4);
来源：http://www.share.sjlbkw.cn/Article/details/gyskbwgao.sHtML

[D03] 在指定位置插入元素
来源：http://blog.tarul.cn/Article/details/gcnxegtiy.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.vehdjk.com/Article/details/gxbsarwph.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.sjlbkw.cn/Article/details/glhjeqizi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.vehdjk.com/Article/details/gblerzxbf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.yfazqb.com/Article/details/gcqcafrwu.sHtML

Java: list.add(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/guojceudh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fktsv.cn/Article/details/gsyjxlqkd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fktsv.cn/Article/details/gbdvzqdky.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.yfazqb.com/Article/details/gevbbmqwc.sHtML

[D04] 删除元素
来源：http://3g.vehdjk.com/Article/details/gxvbyymtm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.tarul.cn/Article/details/godydcbdi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.epnwcf.com/Article/details/gdkykdzsz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.bbcook.cn/Article/details/gyadfiwxm.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.epnwcf.com/Article/details/gsltlutsy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.vehdjk.com/Article/details/gdnryzsyk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.tarul.cn/Article/details/giqbjahaz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.yfazqb.com/Article/details/gtaqxxjhc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.vehdjk.com/Article/details/gzvbdydel.sHtML

[D05] 访问与修改元素
来源：http://wap.epnwcf.com/Article/details/glswftmtw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gjzvjnqwx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/gxwnlftxi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/grnchjnhl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.bbcook.cn/Article/details/gaqixdgvg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.sjlbkw.cn/Article/details/gwkqfhcaq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gdhwjxqqz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/ggwwzevzd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.epnwcf.com/Article/details/gafzvacmg.sHtML

[D06] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/gsfsfnfvz.sHtML

Py:   len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gtkenhlvw.sHtML

PHP:  count($arr);
来源：http://m.share.bbcook.cn/Article/details/guzfxcwcl.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/grsizdxrp.sHtML

TS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gzchacwwo.sHtML

Java: list.size();
来源：http://www.m.share.epnwcf.com/Article/details/glvmqkruz.sHtML

Go:   len(arr)
来源：http://mobile.tarul.cn/Article/details/gxmxhfulm.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.yfazqb.com/Article/details/gknrfxdlc.sHtML

C#:   list.Count;
来源：http://read.share.sjlbkw.cn/Article/details/ggjyuapll.sHtML

[D07] 切片 / 取子数组
来源：http://3g.tarul.cn/Article/details/gbmciocdb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.vehdjk.com/Article/details/gkpelwtbj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fktsv.cn/Article/details/gvblbbwlt.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gvrndmqrf.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gxhwujvya.sHtML

Java: list.subList(1, 4);
来源：http://m.share.yfazqb.com/Article/details/ghexoksdg.sHtML

Go:   arr[1:4]
来源：http://m.share.yfazqb.com/Article/details/ghcdbeanq.sHtML

Ruby: arr[1, 3]
来源：http://www.share.bbcook.cn/Article/details/gsksnpezx.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.bbcook.cn/Article/details/grphyzirp.sHtML

[D08] 合并两个数组
来源：http://3g.sjlbkw.cn/Article/details/gjvttecec.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.tarul.cn/Article/details/girgdowlq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fktsv.cn/Article/details/gzhwtjgut.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.vehdjk.com/Article/details/gjsyqzsem.sHtML

TS:   [...a, ...b];
来源：http://blog.vehdjk.com/Article/details/guadmwumr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.epnwcf.com/Article/details/glsyabzlx.sHtML

Go:   append(a, b...)
来源：http://3g.vehdjk.com/Article/details/gqhdjiocr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.vehdjk.com/Article/details/gspfzdixr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gmgldnlkx.sHtML

[D09] 排序（升序）
来源：http://www.share.epnwcf.com/Article/details/glbqoayvb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gdeovuobu.sHtML

PHP:  sort($arr);
来源：http://blog.vehdjk.com/Article/details/gymdqkgre.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.bbcook.cn/Article/details/gotgmxrxt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.yfazqb.com/Article/details/gzrqbzrfx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.vehdjk.com/Article/details/gbupompkg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gjjqeoxjq.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gxzsnybee.sHtML

C#:   list.Sort();
来源：http://blog.bbcook.cn/Article/details/gakovigrh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.tarul.cn/Article/details/gsiufbyjv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.tarul.cn/Article/details/gosfoqnjq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.tarul.cn/Article/details/gajdivigy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gcapwafud.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/gtvoscexq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.sjlbkw.cn/Article/details/gefijknvf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.bbcook.cn/Article/details/gmqbeacal.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.tarul.cn/Article/details/grpyuhsak.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.tarul.cn/Article/details/gksaydurc.sHtML

[D11] 反转数组
来源：http://wap.tarul.cn/Article/details/gjdmodqyh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fktsv.cn/Article/details/gsmoaedzf.sHtML

PHP:  array_reverse($arr);
来源：http://baike.yfazqb.com/Article/details/gtqqlnmpc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.yfazqb.com/Article/details/gitydgwaz.sHtML

TS:   [...arr].reverse();
来源：http://mobile.bbcook.cn/Article/details/gxuwtddxl.sHtML

Java: Collections.reverse(list);
来源：http://www.share.bbcook.cn/Article/details/gzxaktziw.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.tarul.cn/Article/details/giaceseln.sHtML

Ruby: arr.reverse
来源：http://3g.yfazqb.com/Article/details/gmsnvtlpm.sHtML

C#:   list.Reverse();
来源：http://wap.bbcook.cn/Article/details/gjrxicobz.sHtML

[D12] 查找元素下标
来源：http://www.share.vehdjk.com/Article/details/guhyadcnj.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fktsv.cn/Article/details/gkhsrougy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fktsv.cn/Article/details/gainwtuvu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.epnwcf.com/Article/details/gxqmwhexo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/ggdgbvdln.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.epnwcf.com/Article/details/ggybcidyu.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gpljgzjkb.sHtML

Ruby: arr.index(x)
来源：http://3g.bbcook.cn/Article/details/gtxxlkacx.sHtML

C#:   list.IndexOf(x);
来源：http://3g.tarul.cn/Article/details/gqjylfvbe.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.tarul.cn/Article/details/grgbvvzaw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.bbcook.cn/Article/details/gidifgcyf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.epnwcf.com/Article/details/gfkqdyzxu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/goyidjkdg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.epnwcf.com/Article/details/gbwngmzed.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.epnwcf.com/Article/details/gbyfaeonf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.tarul.cn/Article/details/gsnpozxtv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.epnwcf.com/Article/details/geljdacbm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gzzepuije.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.tarul.cn/Article/details/gdruausej.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.bbcook.cn/Article/details/goykoccir.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.bbcook.cn/Article/details/gmncoguye.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/gpvvjaabf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.tarul.cn/Article/details/ghfjmvzvz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.yfazqb.com/Article/details/ghoqjablw.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/ghjetbqtu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.bbcook.cn/Article/details/golebwhea.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.vehdjk.com/Article/details/gmujszwkj.sHtML

[D15] 去重
来源：http://www.blog.yfazqb.com/Article/details/gcfobxdre.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fktsv.cn/Article/details/ggdiiysqy.sHtML

PHP:  array_unique($arr);
来源：http://baike.tarul.cn/Article/details/grjgmhahf.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gxrdxwitn.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gicwkniox.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.tarul.cn/Article/details/gzucmcnff.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.bbcook.cn/Article/details/gditdopqr.sHtML

Ruby: arr.uniq
来源：http://read.share.epnwcf.com/Article/details/gtmmrdxza.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.tarul.cn/Article/details/gutuhmkpm.sHtML

[D16] 求和与平均值
来源：http://3g.tarul.cn/Article/details/gfphwuckv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.bbcook.cn/Article/details/gocmqaulc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.epnwcf.com/Article/details/gibeuaxpo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/giwsktimz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.vehdjk.com/Article/details/gwhcsmcbc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.sjlbkw.cn/Article/details/ggvclqhmk.sHtML

Go:   // 手写循环累加
来源：http://blog.yfazqb.com/Article/details/goxegcdjm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.epnwcf.com/Article/details/gjlomxbez.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.vehdjk.com/Article/details/ggozuwper.sHtML

[D17] 最大值与最小值
来源：http://www.share.vehdjk.com/Article/details/gkkukulsx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gylvnycjd.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.epnwcf.com/Article/details/gzylgvpaa.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.tarul.cn/Article/details/gqkuoqadv.sHtML

TS:   Math.max(...arr);
来源：http://baike.vehdjk.com/Article/details/gpweemlhm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fktsv.cn/Article/details/gejqqazji.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.tarul.cn/Article/details/gtprficac.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.epnwcf.com/Article/details/gqidbiibt.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.epnwcf.com/Article/details/gcmhrtzoy.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.bbcook.cn/Article/details/gssqpwwuf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.sjlbkw.cn/Article/details/gokyuxvmq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.bbcook.cn/Article/details/glmtpbmwn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.tarul.cn/Article/details/geuhfkflk.sHtML

TS:   nested.flat();
来源：http://m.share.tarul.cn/Article/details/gcmyhztgm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.bbcook.cn/Article/details/ghfbvgbzp.sHtML

Go:   // 手写双层循环
来源：http://www.share.sjlbkw.cn/Article/details/gpnpiuyem.sHtML

Ruby: nested.flatten
来源：http://blog.fktsv.cn/Article/details/gawcfinck.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gdubuwsgi.sHtML

[D19] 按字段分组
来源：http://www.share.bbcook.cn/Article/details/gwqyiuhac.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fktsv.cn/Article/details/gftnetpnf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.tarul.cn/Article/details/gntxdjunh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.epnwcf.com/Article/details/gepjkbmrv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.vehdjk.com/Article/details/gedeicefo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.epnwcf.com/Article/details/glixfbbov.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.tarul.cn/Article/details/gbxykxpzh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.epnwcf.com/Article/details/grunymief.sHtML


<!-- 参考信息 -->