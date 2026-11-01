代发 wailian999

[C06] 匿名函数 / lambda
来源：http://m.share.tarul.cn/Article/details/ggnehvoag.sHtML

Py:   square = lambda x: x * x
来源：http://wap.tarul.cn/Article/details/gomzhrrzi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.epnwcf.com/Article/details/gttcnwemm.sHtML

JS:   const square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/giymdoyit.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.tarul.cn/Article/details/gcoadmdre.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.vehdjk.com/Article/details/gqljxldki.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.vehdjk.com/Article/details/gzsblfrlo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.tarul.cn/Article/details/gkyjixuft.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/glraukstc.sHtML

[C07] 把函数作为参数传入
来源：http://blog.yfazqb.com/Article/details/gmraygzux.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.yfazqb.com/Article/details/gfyodrsik.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.sjlbkw.cn/Article/details/gbvidretn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.epnwcf.com/Article/details/gjckpnrmy.sHtML

TS:   arr.map(String)
来源：http://mobile.vehdjk.com/Article/details/gyjebrabz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fktsv.cn/Article/details/ghsintper.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.bbcook.cn/Article/details/gtddbcwoh.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.bbcook.cn/Article/details/gewbsrmnm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.vehdjk.com/Article/details/gtplpgiaz.sHtML

[C08] 闭包
来源：http://3g.epnwcf.com/Article/details/gcvgfcqaa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.vehdjk.com/Article/details/gntkqsqdf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.vehdjk.com/Article/details/gzvwgfhzj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gcrbycyrr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/ggfvoqoff.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/gazjvnnwb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.bbcook.cn/Article/details/geppwkuvl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.bbcook.cn/Article/details/gomyugkyk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gsaetwkvd.sHtML

[C09] 递归
来源：http://m.share.vehdjk.com/Article/details/gmxnmpoju.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/genqxeond.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fktsv.cn/Article/details/gecikmkwm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/ghhftzqqq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/gfmkfzxpf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.tarul.cn/Article/details/gvlygyibf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.epnwcf.com/Article/details/gavyxtkgc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.bbcook.cn/Article/details/gcizludyb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.yfazqb.com/Article/details/gmswypegb.sHtML

[C10] 变量作用域
来源：http://www.share.yfazqb.com/Article/details/gskaoqbep.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fktsv.cn/Article/details/gdiitxpay.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/goesfzant.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.yfazqb.com/Article/details/gjsjhawnb.sHtML

TS:   同 JS
来源：http://3g.vehdjk.com/Article/details/gxpblthqo.sHtML

Java: 方法内为块级作用域
来源：http://www.share.epnwcf.com/Article/details/gmlidwksi.sHtML

Go:   花括号块级作用域
来源：http://baike.bbcook.cn/Article/details/gjcppshfp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.tarul.cn/Article/details/gpjimbhnw.sHtML

C#:   块级作用域
来源：http://www.share.bbcook.cn/Article/details/gemziujgg.sHtML

[C11] 模块导入与导出
来源：http://wap.tarul.cn/Article/details/gxonscqzy.sHtML

Py:   from module import func
来源：http://read.share.yfazqb.com/Article/details/gwhxdqmxl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.vehdjk.com/Article/details/gleudhtpm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.vehdjk.com/Article/details/ghwxcufpf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.sjlbkw.cn/Article/details/gufwcwiwb.sHtML

Java: import java.util.List;
来源：http://www.blog.tarul.cn/Article/details/gluhqxwqb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.tarul.cn/Article/details/gmfxylhyf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.yfazqb.com/Article/details/ghezzvmia.sHtML

C#:   using System.Text;
来源：http://mobile.vehdjk.com/Article/details/gywarybub.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.sjlbkw.cn/Article/details/gppzthksy.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.bbcook.cn/Article/details/gitsneoss.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.vehdjk.com/Article/details/gkxpfmrur.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.tarul.cn/Article/details/gfhenjuyk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fktsv.cn/Article/details/gaefjfvdz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.epnwcf.com/Article/details/gpjszsjyj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.sjlbkw.cn/Article/details/gokdgvfsy.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.sjlbkw.cn/Article/details/gmgujvayq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fktsv.cn/Article/details/gndxcreee.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fktsv.cn/Article/details/gmjtkihcz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.tarul.cn/Article/details/gkaddqgrf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gqjrpzntz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.bbcook.cn/Article/details/ghpoqawbi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gusoefqoo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gfzvhauop.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fktsv.cn/Article/details/gnpcajjtk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.yfazqb.com/Article/details/geyulqlar.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fktsv.cn/Article/details/gikqqbquq.sHtML

[C14] 泛型函数
来源：http://www.blog.tarul.cn/Article/details/ghenttrye.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.bbcook.cn/Article/details/gtzicrblh.sHtML

PHP:  // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/graqfwxjz.sHtML

JS:   // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gzntuajpz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.epnwcf.com/Article/details/gcrclzutg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.vehdjk.com/Article/details/ghhrclvrd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.bbcook.cn/Article/details/ghkhaxpbb.sHtML

Ruby: # 无泛型
来源：http://read.share.epnwcf.com/Article/details/gsoxoxxop.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fktsv.cn/Article/details/gichfrfgy.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.vehdjk.com/Article/details/gcvbytxiu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.yfazqb.com/Article/details/gcljsavmt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.yfazqb.com/Article/details/gaclneezo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fktsv.cn/Article/details/gnzdopdnb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.yfazqb.com/Article/details/gxqyzwuia.sHtML

Java: // 无解构
来源：http://baike.epnwcf.com/Article/details/gsehyhwec.sHtML

Go:   // 无解构
来源：http://www.share.sjlbkw.cn/Article/details/ghdeljkix.sHtML

Ruby: a, b = pair
来源：http://wap.vehdjk.com/Article/details/grskljrni.sHtML

C#:   var (a, b) = pair;
来源：http://baike.sjlbkw.cn/Article/details/geynzqzsx.sHtML

[C16] 函数 / 方法重载
来源：http://3g.vehdjk.com/Article/details/gzqnbgnqg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.sjlbkw.cn/Article/details/gsetchsbt.sHtML

PHP:  // 无重载
来源：http://www.share.epnwcf.com/Article/details/gzepawegk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.tarul.cn/Article/details/getgigqpp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.sjlbkw.cn/Article/details/gyovgzqoa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.vehdjk.com/Article/details/gletyoxdx.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.yfazqb.com/Article/details/gxvxzhagc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.yfazqb.com/Article/details/gtpvgqfth.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.tarul.cn/Article/details/grurnccmx.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gylgkegss.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.tarul.cn/Article/details/gxpmucdzq.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gffxnavup.sHtML

[D01] 创建数组 / 列表
来源：http://blog.sjlbkw.cn/Article/details/gqaexpdkj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.sjlbkw.cn/Article/details/gthcoyrmh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.tarul.cn/Article/details/gzkddwkfb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.yfazqb.com/Article/details/gffsrdbie.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.yfazqb.com/Article/details/gcrxrxrxy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.yfazqb.com/Article/details/gazvwmcqp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.bbcook.cn/Article/details/gmyotlrjp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.epnwcf.com/Article/details/guvtrzzjq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.epnwcf.com/Article/details/gasjbdjsp.sHtML

[D02] 追加元素到末尾
来源：http://3g.yfazqb.com/Article/details/gefphhrhl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fktsv.cn/Article/details/ghidywzxf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.epnwcf.com/Article/details/gembxshzw.sHtML

JS:   arr.push(4);
来源：http://www.share.epnwcf.com/Article/details/gxyklprkx.sHtML

TS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/gonumwdkp.sHtML

Java: list.add(4);
来源：http://read.share.fktsv.cn/Article/details/gdiugfoua.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.yfazqb.com/Article/details/gsmdhguqm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fktsv.cn/Article/details/ggczsxned.sHtML

C#:   list.Add(4);
来源：http://www.m.share.bbcook.cn/Article/details/grshaspsa.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fktsv.cn/Article/details/ghsnqfgho.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fktsv.cn/Article/details/gwcbsgtzd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.tarul.cn/Article/details/gyrkbivqm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.yfazqb.com/Article/details/gphzinahj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.vehdjk.com/Article/details/grdnglbpu.sHtML

Java: list.add(0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gfozlnagt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.yfazqb.com/Article/details/gwdgrugpd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.epnwcf.com/Article/details/gzyukuljz.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.vehdjk.com/Article/details/gnekqwxjl.sHtML

[D04] 删除元素
来源：http://www.m.share.vehdjk.com/Article/details/gghelloqu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fktsv.cn/Article/details/geqpjawmd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.tarul.cn/Article/details/gfidcnamz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.sjlbkw.cn/Article/details/gbveialun.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.epnwcf.com/Article/details/gyxmlsjfi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.epnwcf.com/Article/details/gjsjkqbmu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.sjlbkw.cn/Article/details/gbvbsdmcc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.tarul.cn/Article/details/gbhfeslmv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.yfazqb.com/Article/details/gbpfjolmk.sHtML

[D05] 访问与修改元素
来源：http://m.share.tarul.cn/Article/details/gmldnxdkt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gypwtkeim.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gpdzuegkw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/glhlhgyjp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.tarul.cn/Article/details/gcqirzubt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.yfazqb.com/Article/details/gjumkmtpq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gwbzjvqns.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/gdpgwqzdf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gknxuywgq.sHtML

[D06] 数组长度
来源：http://wap.fktsv.cn/Article/details/givciwaky.sHtML

Py:   len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gohttcvkl.sHtML

PHP:  count($arr);
来源：http://3g.sjlbkw.cn/Article/details/gmvqocsla.sHtML

JS:   arr.length
来源：http://baike.tarul.cn/Article/details/gppdfpshj.sHtML

TS:   arr.length
来源：http://blog.epnwcf.com/Article/details/gaxpethwz.sHtML

Java: list.size();
来源：http://www.m.share.yfazqb.com/Article/details/ghsiknqts.sHtML

Go:   len(arr)
来源：http://www.share.yfazqb.com/Article/details/gjangoind.sHtML

Ruby: arr.length; arr.size
来源：http://3g.epnwcf.com/Article/details/gzrifugig.sHtML

C#:   list.Count;
来源：http://blog.bbcook.cn/Article/details/gxnjlwahy.sHtML

[D07] 切片 / 取子数组
来源：http://blog.tarul.cn/Article/details/gjfsrfhjz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.sjlbkw.cn/Article/details/govzdgriw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gtuzirfrh.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gxmhhlvke.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/grlawkliz.sHtML

Java: list.subList(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gqcxhlbwc.sHtML

Go:   arr[1:4]
来源：http://blog.yfazqb.com/Article/details/gsuknejmf.sHtML

Ruby: arr[1, 3]
来源：http://baike.epnwcf.com/Article/details/govauznbk.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.vehdjk.com/Article/details/gjqolneeu.sHtML

[D08] 合并两个数组
来源：http://blog.fktsv.cn/Article/details/gystqhhyu.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fktsv.cn/Article/details/gukrkbdem.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.yfazqb.com/Article/details/gojwyfxmr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.tarul.cn/Article/details/gscqijweo.sHtML

TS:   [...a, ...b];
来源：http://www.share.vehdjk.com/Article/details/gdshptwhs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.yfazqb.com/Article/details/gytuweawf.sHtML

Go:   append(a, b...)
来源：http://3g.tarul.cn/Article/details/gvbdoryee.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fktsv.cn/Article/details/ghqicqjnq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gcnpsdpjs.sHtML

[D09] 排序（升序）
来源：http://www.blog.bbcook.cn/Article/details/gmezkxzyx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gudskdjab.sHtML

PHP:  sort($arr);
来源：http://mobile.vehdjk.com/Article/details/grrvjqvlb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.bbcook.cn/Article/details/gfesxzuyj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fktsv.cn/Article/details/gcnacficd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.vehdjk.com/Article/details/ggbcezepc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.vehdjk.com/Article/details/gfwgdffgm.sHtML

Ruby: arr.sort
来源：http://www.blog.yfazqb.com/Article/details/gfjrssxlv.sHtML

C#:   list.Sort();
来源：http://m.share.yfazqb.com/Article/details/gonwkyzru.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.epnwcf.com/Article/details/gbxivwtiz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.bbcook.cn/Article/details/ggasksbfd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.epnwcf.com/Article/details/gulatrhga.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/gdxedomkt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/gcnjuyjvq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.epnwcf.com/Article/details/gqwfcggvp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.sjlbkw.cn/Article/details/gcycrhxwz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.tarul.cn/Article/details/gxucrycdq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.yfazqb.com/Article/details/giokrnkec.sHtML

[D11] 反转数组
来源：http://www.m.share.bbcook.cn/Article/details/gihryebxe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.epnwcf.com/Article/details/glxdwvtkn.sHtML

PHP:  array_reverse($arr);
来源：http://3g.yfazqb.com/Article/details/gflnsmdde.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.vehdjk.com/Article/details/gshcxpcir.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fktsv.cn/Article/details/gulgdqthn.sHtML

Java: Collections.reverse(list);
来源：http://read.share.sjlbkw.cn/Article/details/gmypohour.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fktsv.cn/Article/details/gnvncoyel.sHtML

Ruby: arr.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjrghtrn.sHtML

C#:   list.Reverse();
来源：http://read.share.sjlbkw.cn/Article/details/giuekzjkd.sHtML

[D12] 查找元素下标
来源：http://www.m.share.bbcook.cn/Article/details/gvcxnpkyf.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fktsv.cn/Article/details/gmcrrksju.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.epnwcf.com/Article/details/gergpkcxp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gtjsiblzq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gjenurvdq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fktsv.cn/Article/details/gzstcwtsd.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gptzunpld.sHtML

Ruby: arr.index(x)
来源：http://blog.epnwcf.com/Article/details/gduebqhvg.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.sjlbkw.cn/Article/details/gzmhqgfia.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.epnwcf.com/Article/details/gqvokgbsj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.epnwcf.com/Article/details/gafurjnxv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fktsv.cn/Article/details/ghamalwgy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/gkqdfglzu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/ggthbphts.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.yfazqb.com/Article/details/gifacsdzu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fktsv.cn/Article/details/gilctqthg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.yfazqb.com/Article/details/gzmspjhvi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gtuzanniv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.tarul.cn/Article/details/gleighlwl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.bbcook.cn/Article/details/gayhchvmk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.tarul.cn/Article/details/gepmybhvu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gulwgtnyi.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/gocroszoc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gdmmrdapt.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/gagnxdaoy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gdewkugwm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fktsv.cn/Article/details/gfvutprqh.sHtML

[D15] 去重
来源：http://baike.fktsv.cn/Article/details/gykimoovf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.vehdjk.com/Article/details/gjnqflugg.sHtML

PHP:  array_unique($arr);
来源：http://blog.fktsv.cn/Article/details/gberboyjd.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gluungoqu.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.epnwcf.com/Article/details/gcqxifvnk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.bbcook.cn/Article/details/guzsxbrsm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.yfazqb.com/Article/details/gtvemvgyo.sHtML

Ruby: arr.uniq
来源：http://wap.vehdjk.com/Article/details/gcanrilmt.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.bbcook.cn/Article/details/gwdypqjfc.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fktsv.cn/Article/details/gchdziuwu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.vehdjk.com/Article/details/gemdfsmev.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.tarul.cn/Article/details/goxozatau.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/gyzhpwodi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.bbcook.cn/Article/details/gzjvhbtnv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fktsv.cn/Article/details/gugtiormg.sHtML

Go:   // 手写循环累加
来源：http://baike.bbcook.cn/Article/details/gpjxzsefm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.bbcook.cn/Article/details/gvqkcpxhu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.vehdjk.com/Article/details/guaodrjwy.sHtML

[D17] 最大值与最小值
来源：http://m.share.tarul.cn/Article/details/gmdpziymd.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.vehdjk.com/Article/details/gtqvdmatw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.tarul.cn/Article/details/ggmfcqizj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.bbcook.cn/Article/details/gdriauuzn.sHtML

TS:   Math.max(...arr);
来源：http://baike.tarul.cn/Article/details/ghypixrvc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.bbcook.cn/Article/details/gueodduou.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.epnwcf.com/Article/details/gjykwzrla.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.epnwcf.com/Article/details/grybsqqvb.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/gcwwntwas.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.yfazqb.com/Article/details/gkififpsh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.bbcook.cn/Article/details/gqodvdkbm.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.vehdjk.com/Article/details/ggtscrujc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.bbcook.cn/Article/details/gajskvzkm.sHtML

TS:   nested.flat();
来源：http://wap.tarul.cn/Article/details/gdniumvyg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.epnwcf.com/Article/details/gxznhsols.sHtML

Go:   // 手写双层循环
来源：http://read.share.tarul.cn/Article/details/grurwdzrp.sHtML

Ruby: nested.flatten
来源：http://m.share.epnwcf.com/Article/details/gjhlgqazs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fktsv.cn/Article/details/gbffzpngf.sHtML

[D19] 按字段分组
来源：http://blog.epnwcf.com/Article/details/gsikjclvn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fktsv.cn/Article/details/gwfneqdfc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.epnwcf.com/Article/details/gpdpolzzu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fktsv.cn/Article/details/ggdzpviye.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.vehdjk.com/Article/details/gjlwlwxgm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.tarul.cn/Article/details/gnnekjqyw.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.epnwcf.com/Article/details/gpvtrjpef.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fktsv.cn/Article/details/gplhdqgsq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.sjlbkw.cn/Article/details/gnfeterkj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.tarul.cn/Article/details/gsdhrqhou.sHtML

Py:   Counter(arr)
来源：http://www.share.yfazqb.com/Article/details/gtpwkeszu.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.vehdjk.com/Article/details/gjongfrzi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/grnvnwmxq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fktsv.cn/Article/details/gisnujfpu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fktsv.cn/Article/details/gwnyejgxb.sHtML

Go:   // 手写 map[T]int
来源：http://wap.tarul.cn/Article/details/gapkgfytk.sHtML

Ruby: arr.tally
来源：http://mobile.fktsv.cn/Article/details/gafiwnwqe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.epnwcf.com/Article/details/gefbpehgg.sHtML

[D21] 判断是否包含某元素
来源：http://baike.epnwcf.com/Article/details/gbceqjrvr.sHtML

Py:   x in arr
来源：http://mobile.tarul.cn/Article/details/gugnxygzk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.sjlbkw.cn/Article/details/glsnksbzs.sHtML

JS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/gzzmikqex.sHtML

TS:   arr.includes(x)
来源：http://wap.yfazqb.com/Article/details/gmuifipsk.sHtML

Java: list.contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gmtmiouac.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.yfazqb.com/Article/details/ghkdpfnyc.sHtML

Ruby: arr.include?(x)
来源：http://read.share.tarul.cn/Article/details/gffjcbugi.sHtML

C#:   list.Contains(x)
来源：http://wap.fktsv.cn/Article/details/gggqhwtms.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.yfazqb.com/Article/details/gujkuobms.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.yfazqb.com/Article/details/gaxpzuqfr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.vehdjk.com/Article/details/grhydrdqj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.sjlbkw.cn/Article/details/ghtqfohhd.sHtML

TS:   [...arr];
来源：http://wap.sjlbkw.cn/Article/details/gcxooylrz.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.yfazqb.com/Article/details/gyloyibas.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fktsv.cn/Article/details/gfpynrzrr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fktsv.cn/Article/details/gqawfkshi.sHtML

C#:   new List<int>(list);
来源：http://3g.tarul.cn/Article/details/ghlpbxjfe.sHtML


<!-- 参考信息 -->