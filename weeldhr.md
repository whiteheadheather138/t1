代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.vehdjk.com/Article/details/gfpeakygx.sHtML

TS:   arr.map(String)
来源：http://3g.fktsv.cn/Article/details/graytqywq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.sjlbkw.cn/Article/details/gtkoetgls.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.sjlbkw.cn/Article/details/ggldvsdsy.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.sjlbkw.cn/Article/details/gfghhlcqe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.sjlbkw.cn/Article/details/gfhrjhtlq.sHtML

[C08] 闭包
来源：http://mobile.tarul.cn/Article/details/gjjravkfz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.vehdjk.com/Article/details/gjftwelwu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fktsv.cn/Article/details/gtqcthlmy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gbjdvmgqw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gpdslicrv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.vehdjk.com/Article/details/ggovododv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.vehdjk.com/Article/details/gotllbxux.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.sjlbkw.cn/Article/details/gixpacydf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gugwzcbgh.sHtML

[C09] 递归
来源：http://blog.fktsv.cn/Article/details/gcnhfxnkl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.tarul.cn/Article/details/guyqripkb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.bbcook.cn/Article/details/gmibsqesn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gbdyhjbwr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gserdjbly.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/glkqqedfe.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.vehdjk.com/Article/details/gqwuzpykn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/gugunllnd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.yfazqb.com/Article/details/gijmywiim.sHtML

[C10] 变量作用域
来源：http://baike.vehdjk.com/Article/details/gbmxqmnrh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.vehdjk.com/Article/details/giuewfdtx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.bbcook.cn/Article/details/ghnxpwaxa.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.tarul.cn/Article/details/gxwjpucbg.sHtML

TS:   同 JS
来源：http://www.blog.yfazqb.com/Article/details/gbnxfrjam.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fktsv.cn/Article/details/gxgdtwhud.sHtML

Go:   花括号块级作用域
来源：http://read.share.bbcook.cn/Article/details/gbfdxbgot.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.tarul.cn/Article/details/gnrmbdfqu.sHtML

C#:   块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gnshuglil.sHtML

[C11] 模块导入与导出
来源：http://mobile.tarul.cn/Article/details/gwiokgteh.sHtML

Py:   from module import func
来源：http://www.blog.fktsv.cn/Article/details/gyxirvpie.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.sjlbkw.cn/Article/details/gffgqudko.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.epnwcf.com/Article/details/gkynrijui.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fktsv.cn/Article/details/gzcfvlyyf.sHtML

Java: import java.util.List;
来源：http://m.share.fktsv.cn/Article/details/gackmynym.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmtkaigt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.yfazqb.com/Article/details/gqmjuqkff.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gufdmudqa.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.sjlbkw.cn/Article/details/geqgiykbj.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.tarul.cn/Article/details/geeyqpump.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.yfazqb.com/Article/details/gwjdsaawt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.sjlbkw.cn/Article/details/gpxvndtcd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.sjlbkw.cn/Article/details/gucipfmlj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.tarul.cn/Article/details/gtjrubrdx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.yfazqb.com/Article/details/gxtlpysad.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.bbcook.cn/Article/details/gtebqikoc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fktsv.cn/Article/details/gllxaczar.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fktsv.cn/Article/details/gtrnpzqqc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fktsv.cn/Article/details/gxmknjhks.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gmbvcamor.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.bbcook.cn/Article/details/grfmnkhle.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gnbtjdkzh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gnjaakjmr.sHtML

Go:   func add(a, b int) int
来源：http://read.share.sjlbkw.cn/Article/details/gekxyaobw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.yfazqb.com/Article/details/grjcnartx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.epnwcf.com/Article/details/gbnutbmhw.sHtML

[C14] 泛型函数
来源：http://www.blog.tarul.cn/Article/details/ggydpzmuj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.sjlbkw.cn/Article/details/gcispoxma.sHtML

PHP:  // 无泛型
来源：http://baike.tarul.cn/Article/details/grzeexrpc.sHtML

JS:   // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gdexrtfbs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.epnwcf.com/Article/details/goeodbnoc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.sjlbkw.cn/Article/details/gaflgwzmy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.epnwcf.com/Article/details/gfqgnibkn.sHtML

Ruby: # 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gwgjbpgbe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.tarul.cn/Article/details/gqlljjsgs.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.epnwcf.com/Article/details/gchuthowq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.tarul.cn/Article/details/grvuklyxm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.bbcook.cn/Article/details/geldiizei.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fktsv.cn/Article/details/gsjbijnsa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.vehdjk.com/Article/details/gsigxqdms.sHtML

Java: // 无解构
来源：http://www.m.share.epnwcf.com/Article/details/ghwjbjpxo.sHtML

Go:   // 无解构
来源：http://mobile.tarul.cn/Article/details/gsgsnqabi.sHtML

Ruby: a, b = pair
来源：http://baike.vehdjk.com/Article/details/gyjulmton.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fktsv.cn/Article/details/gxksivoiy.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.epnwcf.com/Article/details/gvbfhsnjf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fktsv.cn/Article/details/gpbnfcftv.sHtML

PHP:  // 无重载
来源：http://read.share.epnwcf.com/Article/details/giungvuqd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.epnwcf.com/Article/details/gsnuznwqr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.yfazqb.com/Article/details/gsmywslzq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.epnwcf.com/Article/details/gpgdjfupv.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.vehdjk.com/Article/details/gjvtdufqr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.sjlbkw.cn/Article/details/gmvgxajxc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.yfazqb.com/Article/details/gwbkgsxqf.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gbnsddntn.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.tarul.cn/Article/details/gdmqkdofs.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gftugfmjo.sHtML

[D01] 创建数组 / 列表
来源：http://wap.sjlbkw.cn/Article/details/glqwwdbfm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.vehdjk.com/Article/details/gswvquwxv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.yfazqb.com/Article/details/gnjqhfyko.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.vehdjk.com/Article/details/gbkbtnnay.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.yfazqb.com/Article/details/giwnzppec.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.sjlbkw.cn/Article/details/gcnmodsie.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.yfazqb.com/Article/details/gpdrsljza.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.bbcook.cn/Article/details/gwftckwix.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.bbcook.cn/Article/details/gxjwuthuk.sHtML

[D02] 追加元素到末尾
来源：http://3g.tarul.cn/Article/details/glpfbshhn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.yfazqb.com/Article/details/geeiaihil.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fktsv.cn/Article/details/gyzujpyjl.sHtML

JS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/gmfmpennb.sHtML

TS:   arr.push(4);
来源：http://blog.vehdjk.com/Article/details/gteivfhnt.sHtML

Java: list.add(4);
来源：http://m.share.fktsv.cn/Article/details/gxcvlgmsv.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fktsv.cn/Article/details/gycycyifi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.yfazqb.com/Article/details/goqzjqcsu.sHtML

C#:   list.Add(4);
来源：http://read.share.yfazqb.com/Article/details/gldphbijc.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fktsv.cn/Article/details/grillzvpb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gcpgcpasb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.yfazqb.com/Article/details/gtyfmgjbu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.yfazqb.com/Article/details/gtkpzcslz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.epnwcf.com/Article/details/gvhdpibtb.sHtML

Java: list.add(0, 0);
来源：http://blog.vehdjk.com/Article/details/gcmchkkva.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.yfazqb.com/Article/details/greaxqmfd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.epnwcf.com/Article/details/grdyxejrs.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gpezcnyjx.sHtML

[D04] 删除元素
来源：http://3g.epnwcf.com/Article/details/gqzqahvtz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.tarul.cn/Article/details/gasytshnx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gurqkfyup.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fktsv.cn/Article/details/gjtcgwohx.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.tarul.cn/Article/details/gmkuyiucu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.epnwcf.com/Article/details/gsnpzrpwe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.tarul.cn/Article/details/ghnzgkbyn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.vehdjk.com/Article/details/gxezypzmb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.vehdjk.com/Article/details/geogwarcw.sHtML

[D05] 访问与修改元素
来源：http://www.blog.yfazqb.com/Article/details/gbwsqxkqt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gzainasia.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gspnanipz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.tarul.cn/Article/details/gkrqubgra.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.tarul.cn/Article/details/gfooksohl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/goezixnya.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gvpzbwesr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gcoqlsggs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxnouqwz.sHtML

[D06] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/gnbpchjrc.sHtML

Py:   len(arr)
来源：http://read.share.tarul.cn/Article/details/gwdgrlblb.sHtML

PHP:  count($arr);
来源：http://www.blog.bbcook.cn/Article/details/gybfbdtsc.sHtML

JS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gekeywzdr.sHtML

TS:   arr.length
来源：http://baike.epnwcf.com/Article/details/gnzowusok.sHtML

Java: list.size();
来源：http://mobile.epnwcf.com/Article/details/gmyodtcor.sHtML

Go:   len(arr)
来源：http://read.share.tarul.cn/Article/details/gqydxomro.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.epnwcf.com/Article/details/gmizxtztw.sHtML

C#:   list.Count;
来源：http://www.share.epnwcf.com/Article/details/giopiafqs.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.vehdjk.com/Article/details/gkzpoplsp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.bbcook.cn/Article/details/gitiqgxav.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.epnwcf.com/Article/details/ghszgcwgq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gusjczook.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.tarul.cn/Article/details/gbuiwbrcf.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gmnzxpjsr.sHtML

Go:   arr[1:4]
来源：http://baike.sjlbkw.cn/Article/details/gfnstiwvz.sHtML

Ruby: arr[1, 3]
来源：http://www.share.vehdjk.com/Article/details/gajswmejd.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.bbcook.cn/Article/details/gajyvdwqu.sHtML

[D08] 合并两个数组
来源：http://m.share.sjlbkw.cn/Article/details/geuqmgigm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.tarul.cn/Article/details/ghmyfflmz.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.tarul.cn/Article/details/goaeyvcqg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.bbcook.cn/Article/details/glouqvosv.sHtML

TS:   [...a, ...b];
来源：http://m.share.sjlbkw.cn/Article/details/gsirwltdp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.epnwcf.com/Article/details/ghfixtkae.sHtML

Go:   append(a, b...)
来源：http://baike.bbcook.cn/Article/details/gdqgbtigz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.tarul.cn/Article/details/gkcobsnyq.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.vehdjk.com/Article/details/gwbjulnao.sHtML

[D09] 排序（升序）
来源：http://www.share.bbcook.cn/Article/details/ggkdwxhbz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/guwkfpvyq.sHtML

PHP:  sort($arr);
来源：http://baike.sjlbkw.cn/Article/details/gdhdfmymd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.tarul.cn/Article/details/gghmknysu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fktsv.cn/Article/details/ggmzjfytl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.tarul.cn/Article/details/gxabrmsrp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gjsqvmpho.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/ggtlpzqtq.sHtML

C#:   list.Sort();
来源：http://mobile.epnwcf.com/Article/details/ginduoqhg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.bbcook.cn/Article/details/gfuwyctov.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fktsv.cn/Article/details/gffhtcclv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.bbcook.cn/Article/details/gpnvgtuqo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.epnwcf.com/Article/details/gpdmqpbyx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fktsv.cn/Article/details/guhuhjuzs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fktsv.cn/Article/details/gaeflyxhm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/gdiwqaofx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.vehdjk.com/Article/details/gkkrhyfzz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.yfazqb.com/Article/details/gihhouscl.sHtML

[D11] 反转数组
来源：http://www.m.share.fktsv.cn/Article/details/geqwaxuev.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/gqyacwqsa.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.tarul.cn/Article/details/giufzqsvh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.tarul.cn/Article/details/gynlzmdpk.sHtML

TS:   [...arr].reverse();
来源：http://mobile.yfazqb.com/Article/details/grcxhwiib.sHtML

Java: Collections.reverse(list);
来源：http://m.share.vehdjk.com/Article/details/gyfwdmfna.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fktsv.cn/Article/details/gxnmwowlo.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gczhfvozr.sHtML

C#:   list.Reverse();
来源：http://wap.sjlbkw.cn/Article/details/gqdzuzkat.sHtML

[D12] 查找元素下标
来源：http://3g.epnwcf.com/Article/details/ggioumoxj.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.bbcook.cn/Article/details/grbrzduoa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.tarul.cn/Article/details/gjcvpwywq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fktsv.cn/Article/details/gtppwsaid.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.vehdjk.com/Article/details/gbeqpvoxj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.yfazqb.com/Article/details/gemhqohnr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gqqvkdgox.sHtML

Ruby: arr.index(x)
来源：http://baike.fktsv.cn/Article/details/gtdakqyst.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.tarul.cn/Article/details/grjyxnpnu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.bbcook.cn/Article/details/gcoadaruk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.sjlbkw.cn/Article/details/gxmecxsnu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.yfazqb.com/Article/details/gahdjwtrr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/gyncekead.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/gcowklpkg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fktsv.cn/Article/details/gxyntjmzi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.sjlbkw.cn/Article/details/geeepxlkw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.tarul.cn/Article/details/glanhtinc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gjzoienle.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.epnwcf.com/Article/details/gunvsdbkl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.bbcook.cn/Article/details/gerahiyta.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.epnwcf.com/Article/details/gqkbeqbpo.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/gepjhwsez.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.vehdjk.com/Article/details/gkxsnigzp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.tarul.cn/Article/details/gmxvtwaoj.sHtML

Go:   // 手写循环
来源：http://www.blog.tarul.cn/Article/details/gxgnsqrrj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gncfmokps.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fktsv.cn/Article/details/gmasvymae.sHtML

[D15] 去重
来源：http://mobile.epnwcf.com/Article/details/gdnosyrjy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.sjlbkw.cn/Article/details/gaffvyinw.sHtML

PHP:  array_unique($arr);
来源：http://blog.fktsv.cn/Article/details/gxinakode.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/gomirlcec.sHtML

TS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/gnuvgbkto.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.bbcook.cn/Article/details/gdbsncpii.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.yfazqb.com/Article/details/gpulcorqz.sHtML

Ruby: arr.uniq
来源：http://www.blog.fktsv.cn/Article/details/gzwxxekhz.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gyrdkdsmx.sHtML

[D16] 求和与平均值
来源：http://www.m.share.vehdjk.com/Article/details/ggrqknlmk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.vehdjk.com/Article/details/gnqejwvbt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.epnwcf.com/Article/details/gbuzlliun.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.tarul.cn/Article/details/gcaxrhmaj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gworwjuut.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.sjlbkw.cn/Article/details/gcraoitrh.sHtML

Go:   // 手写循环累加
来源：http://wap.vehdjk.com/Article/details/gtbijkeqp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.yfazqb.com/Article/details/gvpzeljdx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.vehdjk.com/Article/details/ggfshwyea.sHtML

[D17] 最大值与最小值
来源：http://www.blog.epnwcf.com/Article/details/gcniquwbj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.tarul.cn/Article/details/ggkxegnvm.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fktsv.cn/Article/details/gbrvhioym.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.vehdjk.com/Article/details/gqiatwoky.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.bbcook.cn/Article/details/gbqgrjdiy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.sjlbkw.cn/Article/details/gxkdvzudk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.sjlbkw.cn/Article/details/ghmjsrxvt.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.bbcook.cn/Article/details/gfrmvobss.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.bbcook.cn/Article/details/glgxmatts.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.tarul.cn/Article/details/glubtjngf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.bbcook.cn/Article/details/geuzgbvjd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.sjlbkw.cn/Article/details/ggwlpretd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.tarul.cn/Article/details/ggtfhtuzu.sHtML

TS:   nested.flat();
来源：http://3g.fktsv.cn/Article/details/gckhqitht.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.tarul.cn/Article/details/gonokqfmm.sHtML

Go:   // 手写双层循环
来源：http://www.blog.yfazqb.com/Article/details/gxvumaqfk.sHtML

Ruby: nested.flatten
来源：http://m.share.sjlbkw.cn/Article/details/gviirdops.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fktsv.cn/Article/details/gzyyidlbr.sHtML

[D19] 按字段分组
来源：http://blog.yfazqb.com/Article/details/gmwcxqcnx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.yfazqb.com/Article/details/gvxaiukvp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.sjlbkw.cn/Article/details/gihkcxkig.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.yfazqb.com/Article/details/gvzdjjdwu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.yfazqb.com/Article/details/gxvuctpco.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.tarul.cn/Article/details/gnmivnxci.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.tarul.cn/Article/details/grkgtaaip.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fktsv.cn/Article/details/gklquvlpl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.epnwcf.com/Article/details/guyhdblpb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fktsv.cn/Article/details/gfftciahm.sHtML

Py:   Counter(arr)
来源：http://3g.vehdjk.com/Article/details/gmnihbxsw.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.bbcook.cn/Article/details/gqzrysath.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/gblnffwdp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fktsv.cn/Article/details/gxmclnnau.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.yfazqb.com/Article/details/gumsbfuye.sHtML

Go:   // 手写 map[T]int
来源：http://baike.epnwcf.com/Article/details/gmzazwkkd.sHtML

Ruby: arr.tally
来源：http://www.blog.epnwcf.com/Article/details/ggtbpnyvc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.yfazqb.com/Article/details/gajwdydxv.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.vehdjk.com/Article/details/gxhyispue.sHtML

Py:   x in arr
来源：http://www.blog.vehdjk.com/Article/details/gvwndhiln.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.sjlbkw.cn/Article/details/gzzlxikau.sHtML

JS:   arr.includes(x)
来源：http://read.share.fktsv.cn/Article/details/goqygcdoe.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gvgerwyhv.sHtML

Java: list.contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gfkkuvddr.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gdzaqkeee.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gzbydfrhx.sHtML

C#:   list.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gzrzvmydi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.vehdjk.com/Article/details/ggbehsfsd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.tarul.cn/Article/details/guqiwvapm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.bbcook.cn/Article/details/gidbjxfvd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gdelnxutt.sHtML

TS:   [...arr];
来源：http://www.m.share.epnwcf.com/Article/details/gfiosftoq.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.tarul.cn/Article/details/gjnnifhqn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkprkuko.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.vehdjk.com/Article/details/gzqkipqum.sHtML

C#:   new List<int>(list);
来源：http://m.share.yfazqb.com/Article/details/gwdpshszl.sHtML

[D23] reduce 累积计算
来源：http://blog.vehdjk.com/Article/details/gxgmueama.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.tarul.cn/Article/details/gnobvhete.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.bbcook.cn/Article/details/ghtukkfzk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gyseifbrj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/gyhxdpecg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.epnwcf.com/Article/details/ghhgwqady.sHtML

Go:   // 手写循环
来源：http://www.share.fktsv.cn/Article/details/gwspqjnsn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.bbcook.cn/Article/details/gjcruxeqm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.yfazqb.com/Article/details/gayqmpsdv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.bbcook.cn/Article/details/gdrtcdbrc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.vehdjk.com/Article/details/gfacdxdok.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.bbcook.cn/Article/details/gfyiytplu.sHtML


<!-- 参考信息 -->