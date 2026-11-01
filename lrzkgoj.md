代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.bbcook.cn/Article/details/gsjdghamv.sHtML

TS:   arr.map(String)
来源：http://m.share.sjlbkw.cn/Article/details/gzuyukgqx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.vehdjk.com/Article/details/gotgtsxkg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.vehdjk.com/Article/details/gtxnqhyeh.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fktsv.cn/Article/details/gkdztlqia.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.yfazqb.com/Article/details/gsdahitaj.sHtML

[C08] 闭包
来源：http://www.m.share.fktsv.cn/Article/details/gybebbcli.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.epnwcf.com/Article/details/gwsulswkc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fktsv.cn/Article/details/gyxxcxcfa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvredlze.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gobsfxdoa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.sjlbkw.cn/Article/details/grsogvkcm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fktsv.cn/Article/details/gplhwsrlr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.vehdjk.com/Article/details/goxlruvdb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gpxumikzv.sHtML

[C09] 递归
来源：http://m.share.vehdjk.com/Article/details/gqfilfbvm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.tarul.cn/Article/details/ghtemfohe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.bbcook.cn/Article/details/gtqtddrwm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.bbcook.cn/Article/details/ghmpaqcuf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/guzohrpeu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.yfazqb.com/Article/details/gyzzjdhtp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fktsv.cn/Article/details/gkqjevdoj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/gciovuant.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.epnwcf.com/Article/details/ggnmwxpqt.sHtML

[C10] 变量作用域
来源：http://read.share.tarul.cn/Article/details/geuygqnda.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.vehdjk.com/Article/details/gzryagleb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.sjlbkw.cn/Article/details/gyvwcydke.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.epnwcf.com/Article/details/gvcqipwga.sHtML

TS:   同 JS
来源：http://blog.vehdjk.com/Article/details/gnavqvckd.sHtML

Java: 方法内为块级作用域
来源：http://m.share.bbcook.cn/Article/details/gxudcsrjz.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gbvtcpehh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.sjlbkw.cn/Article/details/gzogygbrl.sHtML

C#:   块级作用域
来源：http://3g.tarul.cn/Article/details/gnlyxkzqj.sHtML

[C11] 模块导入与导出
来源：http://www.share.sjlbkw.cn/Article/details/gmblquuac.sHtML

Py:   from module import func
来源：http://baike.fktsv.cn/Article/details/godimzbam.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.epnwcf.com/Article/details/ghszngncq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/gebmkyrif.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.tarul.cn/Article/details/gnkuwrqph.sHtML

Java: import java.util.List;
来源：http://www.m.share.epnwcf.com/Article/details/girxgrmhf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.yfazqb.com/Article/details/gvmptokwi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.vehdjk.com/Article/details/gfzzbprlr.sHtML

C#:   using System.Text;
来源：http://baike.bbcook.cn/Article/details/gombtuhdm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fktsv.cn/Article/details/gplypcgkd.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.vehdjk.com/Article/details/gjgpbyjyd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.bbcook.cn/Article/details/gjbjgltxl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/gggpjlbmh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/gezaygjoq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.yfazqb.com/Article/details/ggwncljfq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.bbcook.cn/Article/details/gajmujfyl.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.bbcook.cn/Article/details/goqkuixfa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.bbcook.cn/Article/details/ggpbgecww.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.bbcook.cn/Article/details/gorrcapun.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fktsv.cn/Article/details/gagzstaqz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/gtpmgfdpy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.vehdjk.com/Article/details/gwgxyaffi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/geatxknax.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gpfexzcql.sHtML

Go:   func add(a, b int) int
来源：http://m.share.sjlbkw.cn/Article/details/gcmggcwjz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.bbcook.cn/Article/details/gxwhgrhrp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.vehdjk.com/Article/details/ggxxpcjps.sHtML

[C14] 泛型函数
来源：http://read.share.bbcook.cn/Article/details/gzsrjpfde.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.sjlbkw.cn/Article/details/gpdpwljwd.sHtML

PHP:  // 无泛型
来源：http://baike.tarul.cn/Article/details/geqohyfqe.sHtML

JS:   // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gfngrbmxe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.tarul.cn/Article/details/gkevssazc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.vehdjk.com/Article/details/gmzhigwic.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fktsv.cn/Article/details/gpuhcptsv.sHtML

Ruby: # 无泛型
来源：http://mobile.fktsv.cn/Article/details/gonnhlhcr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fktsv.cn/Article/details/gyfzgazzs.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fktsv.cn/Article/details/gfwmgbbyb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.epnwcf.com/Article/details/glehhtuif.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.epnwcf.com/Article/details/gelombrsn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.epnwcf.com/Article/details/ghecbqwms.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.sjlbkw.cn/Article/details/gvnvcztlw.sHtML

Java: // 无解构
来源：http://mobile.bbcook.cn/Article/details/gnhlhytvb.sHtML

Go:   // 无解构
来源：http://www.blog.vehdjk.com/Article/details/gwkisynks.sHtML

Ruby: a, b = pair
来源：http://3g.tarul.cn/Article/details/grqmsftyb.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.epnwcf.com/Article/details/gzgwtmhqx.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.sjlbkw.cn/Article/details/gmlzrgqsq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fktsv.cn/Article/details/gdwqlikrc.sHtML

PHP:  // 无重载
来源：http://www.blog.vehdjk.com/Article/details/gmweepgld.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.sjlbkw.cn/Article/details/gckkyjaor.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.vehdjk.com/Article/details/ggtljgwvk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.tarul.cn/Article/details/gyvemjqxx.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.bbcook.cn/Article/details/gxuqodzvl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.yfazqb.com/Article/details/gfvtphxnt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.bbcook.cn/Article/details/gmwxyvpps.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gmlcmuyqw.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.sjlbkw.cn/Article/details/gjmxgjmal.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gbzclrfbd.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.vehdjk.com/Article/details/gnoiwtavr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.sjlbkw.cn/Article/details/gwtowlccb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.yfazqb.com/Article/details/gykshmnix.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.sjlbkw.cn/Article/details/gcxppjnwt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.epnwcf.com/Article/details/ggxjhqidk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.vehdjk.com/Article/details/grrppwbhh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.sjlbkw.cn/Article/details/gxtdeowan.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.bbcook.cn/Article/details/gbgvybxwr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.epnwcf.com/Article/details/gigykvdol.sHtML

[D02] 追加元素到末尾
来源：http://3g.vehdjk.com/Article/details/gssvajyvu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.yfazqb.com/Article/details/gpboawhpf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.vehdjk.com/Article/details/goasztfzh.sHtML

JS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/gijdzmlkf.sHtML

TS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/gdqhsuukd.sHtML

Java: list.add(4);
来源：http://baike.yfazqb.com/Article/details/gabtjzgwm.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.yfazqb.com/Article/details/gvjdmcxuq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.bbcook.cn/Article/details/ghlojlgqj.sHtML

C#:   list.Add(4);
来源：http://www.share.vehdjk.com/Article/details/gdbpmmbzl.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.bbcook.cn/Article/details/gqtfolwmt.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.yfazqb.com/Article/details/gzrmaroad.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.tarul.cn/Article/details/gyepmqqqs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.yfazqb.com/Article/details/gxsfvvngj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.vehdjk.com/Article/details/gctdoqrib.sHtML

Java: list.add(0, 0);
来源：http://mobile.bbcook.cn/Article/details/gigzboewm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.vehdjk.com/Article/details/gvunuqrhx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.yfazqb.com/Article/details/gpwngdwil.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.vehdjk.com/Article/details/gcapypfhi.sHtML

[D04] 删除元素
来源：http://mobile.yfazqb.com/Article/details/gfgpznoxi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.vehdjk.com/Article/details/gmofhbpax.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.tarul.cn/Article/details/gyeisimem.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.tarul.cn/Article/details/geaazpzdo.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/gromsgtjg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.yfazqb.com/Article/details/gwnzvvpme.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.yfazqb.com/Article/details/ghoijwdot.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.yfazqb.com/Article/details/gpekuhwvc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.yfazqb.com/Article/details/gylyjbbnq.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.epnwcf.com/Article/details/gjbsfjibm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gbyymhvbz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/gfssvjsss.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gaqyisyst.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.tarul.cn/Article/details/gxdjkwuze.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.sjlbkw.cn/Article/details/gosfflzxz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/goqhgauki.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gxmoxnkal.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gdvotjzqb.sHtML

[D06] 数组长度
来源：http://wap.fktsv.cn/Article/details/gsfwngmpz.sHtML

Py:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/gnzexuruk.sHtML

PHP:  count($arr);
来源：http://read.share.epnwcf.com/Article/details/gmltolwvz.sHtML

JS:   arr.length
来源：http://3g.sjlbkw.cn/Article/details/gmrdwfxma.sHtML

TS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/grdyyozqh.sHtML

Java: list.size();
来源：http://www.m.share.vehdjk.com/Article/details/gtjvlpija.sHtML

Go:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/gaiwhfqud.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.tarul.cn/Article/details/gdaihanym.sHtML

C#:   list.Count;
来源：http://www.blog.tarul.cn/Article/details/ghtiopujp.sHtML

[D07] 切片 / 取子数组
来源：http://wap.yfazqb.com/Article/details/garxlxjmv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.yfazqb.com/Article/details/gfdzqpood.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.epnwcf.com/Article/details/gykbnubhc.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gvrbzzryc.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fktsv.cn/Article/details/gexgeibvu.sHtML

Java: list.subList(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gvdorecal.sHtML

Go:   arr[1:4]
来源：http://baike.epnwcf.com/Article/details/giezgxvdz.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.bbcook.cn/Article/details/gahxcxprj.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.yfazqb.com/Article/details/ggshzikyk.sHtML

[D08] 合并两个数组
来源：http://m.share.tarul.cn/Article/details/ghccmhuip.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.epnwcf.com/Article/details/gpfmprtvu.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.yfazqb.com/Article/details/gicnroaqd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.epnwcf.com/Article/details/gwxsrkalc.sHtML

TS:   [...a, ...b];
来源：http://read.share.fktsv.cn/Article/details/gwsckdqpl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.bbcook.cn/Article/details/gmzncetix.sHtML

Go:   append(a, b...)
来源：http://www.blog.fktsv.cn/Article/details/gpohvmids.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.epnwcf.com/Article/details/giffspfhe.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fktsv.cn/Article/details/guirgyurr.sHtML

[D09] 排序（升序）
来源：http://mobile.vehdjk.com/Article/details/gcffrdvrf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/giwvvnmfr.sHtML

PHP:  sort($arr);
来源：http://wap.yfazqb.com/Article/details/gzuygmfwb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.yfazqb.com/Article/details/golndvsuk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.bbcook.cn/Article/details/gzwvgdczy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fktsv.cn/Article/details/gjjbufqdd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/gxojtznax.sHtML

Ruby: arr.sort
来源：http://read.share.vehdjk.com/Article/details/guzfzxzqd.sHtML

C#:   list.Sort();
来源：http://blog.sjlbkw.cn/Article/details/gvjydsomi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.yfazqb.com/Article/details/gransdhlb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.epnwcf.com/Article/details/gktzvyslo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.yfazqb.com/Article/details/grkuzfybx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.vehdjk.com/Article/details/gjrrgzlao.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.yfazqb.com/Article/details/gehfevcbv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.tarul.cn/Article/details/glwiotmqx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.bbcook.cn/Article/details/gcynyudok.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.vehdjk.com/Article/details/gdtkanzie.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.bbcook.cn/Article/details/gdhgyofwi.sHtML

[D11] 反转数组
来源：http://wap.bbcook.cn/Article/details/gqwnimqzg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.bbcook.cn/Article/details/gaaosseww.sHtML

PHP:  array_reverse($arr);
来源：http://baike.vehdjk.com/Article/details/gwclaxhxn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.bbcook.cn/Article/details/gqewwdogr.sHtML

TS:   [...arr].reverse();
来源：http://baike.bbcook.cn/Article/details/gfgxrkldo.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/gumfanosx.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.tarul.cn/Article/details/gluluocte.sHtML

Ruby: arr.reverse
来源：http://3g.fktsv.cn/Article/details/gageqirat.sHtML

C#:   list.Reverse();
来源：http://m.share.epnwcf.com/Article/details/gkvhqdwcq.sHtML

[D12] 查找元素下标
来源：http://blog.epnwcf.com/Article/details/gwbwifobh.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.yfazqb.com/Article/details/ghwhekimc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.epnwcf.com/Article/details/gqzrjheub.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.yfazqb.com/Article/details/goknmvjed.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gdaolyiij.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.tarul.cn/Article/details/gcpoijcxx.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.yfazqb.com/Article/details/guocuymqs.sHtML

Ruby: arr.index(x)
来源：http://blog.epnwcf.com/Article/details/gskciskxl.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.sjlbkw.cn/Article/details/glqoaisey.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.bbcook.cn/Article/details/gswpydzbe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gddxbqfyr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.sjlbkw.cn/Article/details/giabwblot.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gjidxhxei.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.sjlbkw.cn/Article/details/guefgtrcz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gdqdqakus.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.vehdjk.com/Article/details/gmulgvaye.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.sjlbkw.cn/Article/details/gqzcnnrua.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fktsv.cn/Article/details/gzdvnkinj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.bbcook.cn/Article/details/gpjseqcfe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gzudspceo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fktsv.cn/Article/details/gxwpfxaef.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.epnwcf.com/Article/details/govnvblct.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.epnwcf.com/Article/details/gjuittvwi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gjkunswqa.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/grohytdqu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.epnwcf.com/Article/details/gzipfdzfr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.yfazqb.com/Article/details/gphmlmxwj.sHtML

[D15] 去重
来源：http://www.blog.tarul.cn/Article/details/gnrcplgbr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.epnwcf.com/Article/details/gbzeozorz.sHtML

PHP:  array_unique($arr);
来源：http://baike.epnwcf.com/Article/details/gchfuiikt.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gfaglnpkr.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/gmndgoqau.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.tarul.cn/Article/details/gkgyjdyic.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.yfazqb.com/Article/details/gvghprtrc.sHtML

Ruby: arr.uniq
来源：http://baike.tarul.cn/Article/details/gheosfsow.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.bbcook.cn/Article/details/gmsssjhqx.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/ghmlyentt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.yfazqb.com/Article/details/gurftrrfm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.vehdjk.com/Article/details/gchpzebuc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gtvfbvfle.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/geeempizh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.yfazqb.com/Article/details/gfkuqmdwr.sHtML

Go:   // 手写循环累加
来源：http://blog.sjlbkw.cn/Article/details/gjninwmnk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.bbcook.cn/Article/details/gcwujhqrp.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.bbcook.cn/Article/details/gyxmoefbr.sHtML

[D17] 最大值与最小值
来源：http://mobile.yfazqb.com/Article/details/gayyrbzdt.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.epnwcf.com/Article/details/gpiggvjbi.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.vehdjk.com/Article/details/gumevmnib.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.yfazqb.com/Article/details/gefwychmh.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fktsv.cn/Article/details/ghgonxtyw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.sjlbkw.cn/Article/details/ggpvrcbhg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.sjlbkw.cn/Article/details/gjryhxhor.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.vehdjk.com/Article/details/gvucrmucz.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.yfazqb.com/Article/details/gaedimclv.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.sjlbkw.cn/Article/details/grirguwlu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fktsv.cn/Article/details/givtcvxdu.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.bbcook.cn/Article/details/glvgrcqwc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.sjlbkw.cn/Article/details/gvlmfxsgm.sHtML

TS:   nested.flat();
来源：http://baike.fktsv.cn/Article/details/gjaekfcet.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.tarul.cn/Article/details/gjjwleayj.sHtML

Go:   // 手写双层循环
来源：http://blog.yfazqb.com/Article/details/glldfnqiv.sHtML

Ruby: nested.flatten
来源：http://mobile.tarul.cn/Article/details/gtaelboam.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.vehdjk.com/Article/details/ghnicrppe.sHtML

[D19] 按字段分组
来源：http://baike.tarul.cn/Article/details/gddglcjjw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.sjlbkw.cn/Article/details/gurrixtuu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.sjlbkw.cn/Article/details/gzosgwlhf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.bbcook.cn/Article/details/gbwmgobka.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.tarul.cn/Article/details/gvnvpvzwp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.vehdjk.com/Article/details/gxxygatlt.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.sjlbkw.cn/Article/details/gtalthdpb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.bbcook.cn/Article/details/gtejnypuv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.yfazqb.com/Article/details/gghcekhyd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fktsv.cn/Article/details/gawgapsxg.sHtML

Py:   Counter(arr)
来源：http://baike.bbcook.cn/Article/details/gombfhzcr.sHtML

PHP:  array_count_values($arr);
来源：http://wap.bbcook.cn/Article/details/gpondwtvo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/glqpdeoiq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.vehdjk.com/Article/details/gqajfzeij.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.yfazqb.com/Article/details/grzuwtglk.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.tarul.cn/Article/details/gdklxrbth.sHtML

Ruby: arr.tally
来源：http://read.share.bbcook.cn/Article/details/gzltwukgk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fktsv.cn/Article/details/gmgmurfzu.sHtML

[D21] 判断是否包含某元素
来源：http://wap.bbcook.cn/Article/details/gwjudcvmn.sHtML

Py:   x in arr
来源：http://www.share.vehdjk.com/Article/details/gmssnfdzk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.bbcook.cn/Article/details/gjfbxjztu.sHtML

JS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gogzusemq.sHtML

TS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gejzrmrbz.sHtML

Java: list.contains(x)
来源：http://mobile.fktsv.cn/Article/details/gawdyhkvq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gbawualyf.sHtML

Ruby: arr.include?(x)
来源：http://wap.sjlbkw.cn/Article/details/gbmowltdb.sHtML

C#:   list.Contains(x)
来源：http://baike.fktsv.cn/Article/details/gldgfrzjy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fktsv.cn/Article/details/gtprmvmuu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fktsv.cn/Article/details/gdohszfkw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.yfazqb.com/Article/details/ghzwzbqza.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.bbcook.cn/Article/details/guhiowlgu.sHtML

TS:   [...arr];
来源：http://blog.epnwcf.com/Article/details/gvbyoufhm.sHtML

Java: new ArrayList<>(list);
来源：http://baike.epnwcf.com/Article/details/gkgcsihqw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.sjlbkw.cn/Article/details/gccswodry.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.bbcook.cn/Article/details/gfwuyjwtj.sHtML

C#:   new List<int>(list);
来源：http://m.share.tarul.cn/Article/details/glmfefiek.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.sjlbkw.cn/Article/details/gxetpplmh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.vehdjk.com/Article/details/gfffpmncv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fktsv.cn/Article/details/grcycztjy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/getkwwexs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/gnwadzawe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.tarul.cn/Article/details/glvtmpchs.sHtML

Go:   // 手写循环
来源：http://mobile.yfazqb.com/Article/details/gufzytpqh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.vehdjk.com/Article/details/gyvlfcnjh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.tarul.cn/Article/details/gcxqqudbm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.vehdjk.com/Article/details/gcbvwzoia.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.yfazqb.com/Article/details/ghtyykirs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.epnwcf.com/Article/details/gkxgnswak.sHtML


<!-- 参考信息 -->