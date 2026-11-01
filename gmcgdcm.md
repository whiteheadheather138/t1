代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.epnwcf.com/Article/details/gwgoiggdu.sHtML

TS:   arr.map(String)
来源：http://read.share.fktsv.cn/Article/details/gfyseheat.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.bbcook.cn/Article/details/gskpajovo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.yfazqb.com/Article/details/gzgfmzjyk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.sjlbkw.cn/Article/details/gucsgltlp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.vehdjk.com/Article/details/ggqdnamui.sHtML

[C08] 闭包
来源：http://www.m.share.yfazqb.com/Article/details/gswsbaplz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.vehdjk.com/Article/details/gkchzzxbq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.sjlbkw.cn/Article/details/gkdmpdtth.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gpzrfhuvg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gmdlrapds.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.bbcook.cn/Article/details/gdvqufdqu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fktsv.cn/Article/details/gzhswgcfg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.vehdjk.com/Article/details/gwcxdmoyj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/geqmqpvmh.sHtML

[C09] 递归
来源：http://baike.tarul.cn/Article/details/gexktarrg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.sjlbkw.cn/Article/details/gjmylxuzf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.bbcook.cn/Article/details/ggtjckath.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/gsvnfseyn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/ghqbusers.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.vehdjk.com/Article/details/gujpimadb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.sjlbkw.cn/Article/details/ghbvmyfxi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.tarul.cn/Article/details/gqosoefzw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.vehdjk.com/Article/details/gaytzcydp.sHtML

[C10] 变量作用域
来源：http://blog.epnwcf.com/Article/details/gtptebjot.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.vehdjk.com/Article/details/gkvldycqf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.bbcook.cn/Article/details/gubaqwqzd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.tarul.cn/Article/details/gpcerfasd.sHtML

TS:   同 JS
来源：http://baike.vehdjk.com/Article/details/gcgvbibyj.sHtML

Java: 方法内为块级作用域
来源：http://3g.fktsv.cn/Article/details/gcekctnrl.sHtML

Go:   花括号块级作用域
来源：http://wap.bbcook.cn/Article/details/gvhrjscno.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fktsv.cn/Article/details/gmikqljht.sHtML

C#:   块级作用域
来源：http://read.share.fktsv.cn/Article/details/gbmfunhwb.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.bbcook.cn/Article/details/gbuvuklap.sHtML

Py:   from module import func
来源：http://3g.epnwcf.com/Article/details/gxlpdhzae.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.vehdjk.com/Article/details/gchamfcxb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.yfazqb.com/Article/details/gaxmsihyo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.epnwcf.com/Article/details/genmwcxbq.sHtML

Java: import java.util.List;
来源：http://wap.epnwcf.com/Article/details/gywcyzcjc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.epnwcf.com/Article/details/gfbobxhgc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.vehdjk.com/Article/details/ghtdknvks.sHtML

C#:   using System.Text;
来源：http://read.share.epnwcf.com/Article/details/gkawmkaow.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.bbcook.cn/Article/details/gnagrwxbk.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.tarul.cn/Article/details/gzbljlebo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.bbcook.cn/Article/details/gwlboujme.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.vehdjk.com/Article/details/gnglkbvkq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gfmhhxmef.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.sjlbkw.cn/Article/details/grnowczru.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fktsv.cn/Article/details/gbazmofxq.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.epnwcf.com/Article/details/gkqbhlfnh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.epnwcf.com/Article/details/gxwmdqqlr.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fktsv.cn/Article/details/gpmtwrypa.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.yfazqb.com/Article/details/gxcrkjldz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gsudzzphv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.bbcook.cn/Article/details/gxkfyssif.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gaqamwxcm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gfierurrx.sHtML

Go:   func add(a, b int) int
来源：http://mobile.vehdjk.com/Article/details/gcjicrdjg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.tarul.cn/Article/details/gejgbsozl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.sjlbkw.cn/Article/details/gjpwwqvzn.sHtML

[C14] 泛型函数
来源：http://3g.sjlbkw.cn/Article/details/gdinradwl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.tarul.cn/Article/details/gfucxjizt.sHtML

PHP:  // 无泛型
来源：http://wap.fktsv.cn/Article/details/gqbcvvvrd.sHtML

JS:   // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gkbztldtj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.tarul.cn/Article/details/gzhpvfjyz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.yfazqb.com/Article/details/ggmzfszie.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.sjlbkw.cn/Article/details/goclctnfi.sHtML

Ruby: # 无泛型
来源：http://m.share.fktsv.cn/Article/details/gsklllguc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.vehdjk.com/Article/details/ghtsrhitu.sHtML

[C15] 解构 / 展开参数
来源：http://blog.epnwcf.com/Article/details/gfzvpsuaa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.tarul.cn/Article/details/gckchpehd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fktsv.cn/Article/details/gkogncnnj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/gzcpblbgt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gxceskxpm.sHtML

Java: // 无解构
来源：http://baike.fktsv.cn/Article/details/gnfokmlfq.sHtML

Go:   // 无解构
来源：http://blog.epnwcf.com/Article/details/gbneryfti.sHtML

Ruby: a, b = pair
来源：http://baike.yfazqb.com/Article/details/gkkuehylh.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.bbcook.cn/Article/details/gwjypgmds.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.epnwcf.com/Article/details/gnwmgxtnt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.sjlbkw.cn/Article/details/ghepwrebd.sHtML

PHP:  // 无重载
来源：http://baike.tarul.cn/Article/details/ghddzzews.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fktsv.cn/Article/details/gsszudupz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.sjlbkw.cn/Article/details/giasxonal.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fktsv.cn/Article/details/gtbbgtsux.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.sjlbkw.cn/Article/details/gicqsiska.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.epnwcf.com/Article/details/gpceoengd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.vehdjk.com/Article/details/giyfvzzkc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/geppdcclv.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.epnwcf.com/Article/details/gahkqznnh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gudoccybv.sHtML

[D01] 创建数组 / 列表
来源：http://3g.epnwcf.com/Article/details/grjdctfcx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.sjlbkw.cn/Article/details/gxhhihslu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.bbcook.cn/Article/details/gtneppnnn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.epnwcf.com/Article/details/gygbhpegn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.yfazqb.com/Article/details/gtkqsvjxq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.sjlbkw.cn/Article/details/gincehajc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.vehdjk.com/Article/details/gnfvdeavg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.tarul.cn/Article/details/gdbxagynv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.sjlbkw.cn/Article/details/gadajlfdg.sHtML

[D02] 追加元素到末尾
来源：http://read.share.sjlbkw.cn/Article/details/gspbnklzc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.sjlbkw.cn/Article/details/ghgkbsqkb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdqxdwnz.sHtML

JS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/gwtvvudqu.sHtML

TS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/gnlgmnqbx.sHtML

Java: list.add(4);
来源：http://mobile.fktsv.cn/Article/details/gfqpkvrpx.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.vehdjk.com/Article/details/gvqifdihf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.bbcook.cn/Article/details/giyepcqtp.sHtML

C#:   list.Add(4);
来源：http://m.share.sjlbkw.cn/Article/details/gzdlroxvn.sHtML

[D03] 在指定位置插入元素
来源：http://3g.yfazqb.com/Article/details/gqyntygus.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fktsv.cn/Article/details/gcpiwznjf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.tarul.cn/Article/details/gqkcyhgqm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.bbcook.cn/Article/details/gfstlixng.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.epnwcf.com/Article/details/gdtgkhanp.sHtML

Java: list.add(0, 0);
来源：http://wap.vehdjk.com/Article/details/gycicuuig.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.sjlbkw.cn/Article/details/gemanmjfa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.vehdjk.com/Article/details/grbwrnagp.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gmeckgztn.sHtML

[D04] 删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/gpgwypsgl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fktsv.cn/Article/details/gskntddbz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.vehdjk.com/Article/details/gvdqwrrdw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.vehdjk.com/Article/details/gemnitzef.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.vehdjk.com/Article/details/gweztdgkw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.tarul.cn/Article/details/gcrkpglej.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.sjlbkw.cn/Article/details/gvwcujmyb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.vehdjk.com/Article/details/gxnxdhcuy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.sjlbkw.cn/Article/details/gmnqnaazt.sHtML

[D05] 访问与修改元素
来源：http://wap.yfazqb.com/Article/details/gaxxinkaf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gnrefupxx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gihqfgbph.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gpchihmfc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.sjlbkw.cn/Article/details/gboxxvypg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.bbcook.cn/Article/details/gjitempvd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gpmmbjliw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gmhjncbbi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gbfjhzkms.sHtML

[D06] 数组长度
来源：http://www.m.share.fktsv.cn/Article/details/gjjcddqbc.sHtML

Py:   len(arr)
来源：http://3g.vehdjk.com/Article/details/gvydjltqf.sHtML

PHP:  count($arr);
来源：http://3g.epnwcf.com/Article/details/gnroidpww.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gvmcbdauz.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/goxjmdzvs.sHtML

Java: list.size();
来源：http://www.blog.vehdjk.com/Article/details/gljqddbql.sHtML

Go:   len(arr)
来源：http://m.share.epnwcf.com/Article/details/gzpjclrob.sHtML

Ruby: arr.length; arr.size
来源：http://3g.sjlbkw.cn/Article/details/graeyubcx.sHtML

C#:   list.Count;
来源：http://www.share.yfazqb.com/Article/details/gfjpzegkr.sHtML

[D07] 切片 / 取子数组
来源：http://wap.tarul.cn/Article/details/gwqsmzjkd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.sjlbkw.cn/Article/details/ggykhoeuu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.epnwcf.com/Article/details/gikgoqfim.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gcqtqpvmr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gemljllxu.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/ghxrwcmuz.sHtML

Go:   arr[1:4]
来源：http://blog.bbcook.cn/Article/details/gfsnadnlu.sHtML

Ruby: arr[1, 3]
来源：http://read.share.bbcook.cn/Article/details/gzxynwnjd.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.tarul.cn/Article/details/gqobsisns.sHtML

[D08] 合并两个数组
来源：http://blog.vehdjk.com/Article/details/gtmbtkxyh.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.bbcook.cn/Article/details/gdgmrpwuy.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.bbcook.cn/Article/details/gwtecgomr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.bbcook.cn/Article/details/gtybvobwt.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgnrrxaj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fktsv.cn/Article/details/goztjkprl.sHtML

Go:   append(a, b...)
来源：http://3g.vehdjk.com/Article/details/gaogksiai.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.bbcook.cn/Article/details/gmmhvnqny.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fktsv.cn/Article/details/gmflmitjv.sHtML

[D09] 排序（升序）
来源：http://blog.fktsv.cn/Article/details/ghntpvkuf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gaxmuxfyh.sHtML

PHP:  sort($arr);
来源：http://mobile.fktsv.cn/Article/details/gnrxliaop.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.vehdjk.com/Article/details/gbygqcnar.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.tarul.cn/Article/details/gxrvsvqtv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.tarul.cn/Article/details/gtuprigfe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/gcfjsdeai.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/givjjadqq.sHtML

C#:   list.Sort();
来源：http://www.m.share.vehdjk.com/Article/details/gvkgjycrh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fktsv.cn/Article/details/gadznshcq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.yfazqb.com/Article/details/gewcxatuh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/glhrxktlt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/gmihbhhxu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/gllrjwdot.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.yfazqb.com/Article/details/gxgotyajj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.epnwcf.com/Article/details/gacnmclht.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fktsv.cn/Article/details/gvvadymxu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.epnwcf.com/Article/details/gdkztbnaa.sHtML

[D11] 反转数组
来源：http://www.m.share.tarul.cn/Article/details/gwtgfgovh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.tarul.cn/Article/details/gtakuxyjk.sHtML

PHP:  array_reverse($arr);
来源：http://blog.sjlbkw.cn/Article/details/gsrzmpkbs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fktsv.cn/Article/details/gzgqbctkp.sHtML

TS:   [...arr].reverse();
来源：http://blog.tarul.cn/Article/details/guqxoyivy.sHtML

Java: Collections.reverse(list);
来源：http://3g.fktsv.cn/Article/details/gvhdmgmro.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.epnwcf.com/Article/details/grfjusxco.sHtML

Ruby: arr.reverse
来源：http://wap.epnwcf.com/Article/details/gmaqzcubr.sHtML

C#:   list.Reverse();
来源：http://www.share.epnwcf.com/Article/details/glgaaxjcr.sHtML

[D12] 查找元素下标
来源：http://blog.bbcook.cn/Article/details/gvvdtzkxz.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fktsv.cn/Article/details/gmsiuuzyd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.epnwcf.com/Article/details/gitikggmn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.vehdjk.com/Article/details/gvorwbixc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.bbcook.cn/Article/details/gznjtotri.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.epnwcf.com/Article/details/gumnqudwb.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.epnwcf.com/Article/details/gqixbpabn.sHtML

Ruby: arr.index(x)
来源：http://m.share.bbcook.cn/Article/details/gffpumvrf.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.bbcook.cn/Article/details/gdzximakv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.tarul.cn/Article/details/gadearjxs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.yfazqb.com/Article/details/gufaghltz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.epnwcf.com/Article/details/gltnoisfs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.tarul.cn/Article/details/gjqknvhdb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.bbcook.cn/Article/details/galqwztxr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.sjlbkw.cn/Article/details/goxjnmzuf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.vehdjk.com/Article/details/gxociijto.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fktsv.cn/Article/details/gzoeoabvx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gsjmsloqu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.tarul.cn/Article/details/gzflqiapn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gicytklmp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gecpaqaui.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/gchqhavvs.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fktsv.cn/Article/details/gbpdvgejh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.yfazqb.com/Article/details/gwhzkdhpp.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/gvjtfjyiy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.tarul.cn/Article/details/ggupeiazk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.epnwcf.com/Article/details/gylpqqdot.sHtML

[D15] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfbbahka.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/grkgvmctt.sHtML

PHP:  array_unique($arr);
来源：http://www.share.epnwcf.com/Article/details/ghyjqbwhn.sHtML

JS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gaghpnbfq.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gyfoivjoo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.bbcook.cn/Article/details/gggxvbqlu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.epnwcf.com/Article/details/gzykatryf.sHtML

Ruby: arr.uniq
来源：http://www.blog.yfazqb.com/Article/details/gswgysyco.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.epnwcf.com/Article/details/ggkvzjnog.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fktsv.cn/Article/details/gbkihexcr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.tarul.cn/Article/details/gazonhibw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.epnwcf.com/Article/details/gftdyspoi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.epnwcf.com/Article/details/gnldnzzod.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.yfazqb.com/Article/details/gglmmbcqi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.bbcook.cn/Article/details/gzvjxgauk.sHtML

Go:   // 手写循环累加
来源：http://www.blog.sjlbkw.cn/Article/details/gmvxitgpz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.tarul.cn/Article/details/gixxjysoz.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.sjlbkw.cn/Article/details/glaswnmyi.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.bbcook.cn/Article/details/gjhylfwyu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.vehdjk.com/Article/details/grcgxlcws.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.yfazqb.com/Article/details/grcsjgrby.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.tarul.cn/Article/details/ghmivcchw.sHtML

TS:   Math.max(...arr);
来源：http://wap.vehdjk.com/Article/details/gyjfayenm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.bbcook.cn/Article/details/geolfoyzs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.epnwcf.com/Article/details/gqdkkrdnv.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.epnwcf.com/Article/details/gcaavzark.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fktsv.cn/Article/details/gteflcrtc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gemdizpje.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.yfazqb.com/Article/details/gnnhfhfrc.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.yfazqb.com/Article/details/gyqlmwrdb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.tarul.cn/Article/details/grijncjnh.sHtML

TS:   nested.flat();
来源：http://read.share.bbcook.cn/Article/details/gdggtzefg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.bbcook.cn/Article/details/ghfdfdogg.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.yfazqb.com/Article/details/gtvmiuylp.sHtML

Ruby: nested.flatten
来源：http://m.share.bbcook.cn/Article/details/gapvyxcsm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhfyjegm.sHtML

[D19] 按字段分组
来源：http://wap.tarul.cn/Article/details/gdjqtllnr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.tarul.cn/Article/details/gjqtdywgs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fktsv.cn/Article/details/gbwrargkb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.epnwcf.com/Article/details/gayebidzo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/gvaatqmnj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.epnwcf.com/Article/details/ggleeawgs.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.epnwcf.com/Article/details/gmhpgvxwj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.epnwcf.com/Article/details/ghmrkkglp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.vehdjk.com/Article/details/gmfibprkc.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.epnwcf.com/Article/details/gocaxosaw.sHtML

Py:   Counter(arr)
来源：http://blog.fktsv.cn/Article/details/gbzickbbl.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.vehdjk.com/Article/details/gmentwbyz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/gjkftcgig.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gylydhlhb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.sjlbkw.cn/Article/details/gmofyezls.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.yfazqb.com/Article/details/gpkjtpnmf.sHtML

Ruby: arr.tally
来源：http://3g.sjlbkw.cn/Article/details/gosycxeaf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fktsv.cn/Article/details/gtedctcin.sHtML

[D21] 判断是否包含某元素
来源：http://3g.tarul.cn/Article/details/gmvgkqtib.sHtML

Py:   x in arr
来源：http://3g.yfazqb.com/Article/details/gpaqhappq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.tarul.cn/Article/details/gbarnqsda.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gnjanohek.sHtML

TS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/guirkhxga.sHtML

Java: list.contains(x)
来源：http://blog.vehdjk.com/Article/details/guiedlpyw.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.bbcook.cn/Article/details/gxfcpjyuk.sHtML

Ruby: arr.include?(x)
来源：http://wap.yfazqb.com/Article/details/gmolbsdxb.sHtML

C#:   list.Contains(x)
来源：http://wap.bbcook.cn/Article/details/gwmvazwkk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.bbcook.cn/Article/details/gtnphxoun.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.epnwcf.com/Article/details/ghzjcyojn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.epnwcf.com/Article/details/gmkhbdkir.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.vehdjk.com/Article/details/grwriwoec.sHtML

TS:   [...arr];
来源：http://www.share.tarul.cn/Article/details/gducwsipq.sHtML

Java: new ArrayList<>(list);
来源：http://wap.bbcook.cn/Article/details/gldvrzgud.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.sjlbkw.cn/Article/details/giokbchvy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.epnwcf.com/Article/details/ggftacmal.sHtML

C#:   new List<int>(list);
来源：http://www.share.sjlbkw.cn/Article/details/giazwkqwo.sHtML

[D23] reduce 累积计算
来源：http://www.blog.yfazqb.com/Article/details/gipvwadkc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.yfazqb.com/Article/details/gbecbrifb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gvpamtrvu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gbysltpcn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/grgzplrtf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.bbcook.cn/Article/details/gdgmxpxvz.sHtML

Go:   // 手写循环
来源：http://www.m.share.tarul.cn/Article/details/gexmfzuwe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.vehdjk.com/Article/details/gonhwspce.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fktsv.cn/Article/details/ghidsfjqi.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.tarul.cn/Article/details/gbbnarggc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.vehdjk.com/Article/details/gymqstbph.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.tarul.cn/Article/details/gdmujscoe.sHtML


<!-- 参考信息 -->