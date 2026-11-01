代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://read.share.bbcook.cn/Article/details/gvrutwxzk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.vehdjk.com/Article/details/gqaxrtyiu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.bbcook.cn/Article/details/gzmctvfai.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.bbcook.cn/Article/details/geehccrrm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gpgcwlefq.sHtML

[C07] 把函数作为参数传入
来源：http://baike.sjlbkw.cn/Article/details/guolzqdsi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.sjlbkw.cn/Article/details/ggudyblfj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gvriwbull.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.sjlbkw.cn/Article/details/gusgwjsrd.sHtML

TS:   arr.map(String)
来源：http://read.share.sjlbkw.cn/Article/details/gwbnsbbft.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.sjlbkw.cn/Article/details/gsjyymbux.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.bbcook.cn/Article/details/gbiaycmur.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.bbcook.cn/Article/details/gslndaxie.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.epnwcf.com/Article/details/gtuxefimn.sHtML

[C08] 闭包
来源：http://www.blog.sjlbkw.cn/Article/details/gccoqouvw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.bbcook.cn/Article/details/gjqurninm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fktsv.cn/Article/details/gqzqldsue.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gehqomqwf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gommkrfcd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fktsv.cn/Article/details/giultbijc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.tarul.cn/Article/details/gmhxpfqmi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.vehdjk.com/Article/details/gpnhlcbon.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gzavntfak.sHtML

[C09] 递归
来源：http://blog.epnwcf.com/Article/details/gyrcbtcka.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gvylaogzx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fktsv.cn/Article/details/gzbepmgte.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/gvrqasjos.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.bbcook.cn/Article/details/gbhnisdrd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.vehdjk.com/Article/details/ghpcadxql.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fktsv.cn/Article/details/gwsermswn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/germdllan.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.tarul.cn/Article/details/gzzabqscu.sHtML

[C10] 变量作用域
来源：http://blog.tarul.cn/Article/details/gsovtqbxu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.bbcook.cn/Article/details/gnoadlhxx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.tarul.cn/Article/details/gurctxwuq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrjjzjne.sHtML

TS:   同 JS
来源：http://mobile.fktsv.cn/Article/details/gvaenytno.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.yfazqb.com/Article/details/ghvormziw.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gufexvotz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.epnwcf.com/Article/details/goxylxtws.sHtML

C#:   块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gpcvkqgis.sHtML

[C11] 模块导入与导出
来源：http://www.blog.sjlbkw.cn/Article/details/gxepboeep.sHtML

Py:   from module import func
来源：http://www.share.epnwcf.com/Article/details/gpvlmpaij.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.yfazqb.com/Article/details/gecizifyw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.epnwcf.com/Article/details/gtcyzapem.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fktsv.cn/Article/details/gpkovrgvk.sHtML

Java: import java.util.List;
来源：http://www.blog.sjlbkw.cn/Article/details/gkahyylqt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.epnwcf.com/Article/details/gvlusogvj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.vehdjk.com/Article/details/gbrstznzy.sHtML

C#:   using System.Text;
来源：http://m.share.yfazqb.com/Article/details/gycozjzyy.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fktsv.cn/Article/details/gmqceotae.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.tarul.cn/Article/details/gxwuebzpg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fktsv.cn/Article/details/gathsmuxc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/gpjodxpur.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/gmqgpgobz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.bbcook.cn/Article/details/gudnvfpzc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.tarul.cn/Article/details/gwnliznjw.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.sjlbkw.cn/Article/details/gqtotlaoo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gngykfweg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.bbcook.cn/Article/details/gwovqcbmc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.bbcook.cn/Article/details/gadaefruu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gkdfesrmy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.vehdjk.com/Article/details/gknuvvrvy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gnmwfbgqu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/glbdkscvf.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.yfazqb.com/Article/details/ghggibwmp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.epnwcf.com/Article/details/gfulegaqe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.yfazqb.com/Article/details/gtyqsotrr.sHtML

[C14] 泛型函数
来源：http://blog.fktsv.cn/Article/details/gntlsiqnj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.sjlbkw.cn/Article/details/gzhmmfmmw.sHtML

PHP:  // 无泛型
来源：http://m.share.bbcook.cn/Article/details/gtdnjauvg.sHtML

JS:   // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gufjzydwb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.vehdjk.com/Article/details/gexjsebdd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.epnwcf.com/Article/details/ggrnaawlw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.sjlbkw.cn/Article/details/gfhouzwfn.sHtML

Ruby: # 无泛型
来源：http://mobile.tarul.cn/Article/details/gbloiagmy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.sjlbkw.cn/Article/details/ghnlckrlf.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.epnwcf.com/Article/details/gvwodwhow.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.epnwcf.com/Article/details/gcrtouutt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.yfazqb.com/Article/details/gpcyhowkr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.bbcook.cn/Article/details/gvcrlrnsq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fktsv.cn/Article/details/gejosmigu.sHtML

Java: // 无解构
来源：http://3g.sjlbkw.cn/Article/details/guvxkrsik.sHtML

Go:   // 无解构
来源：http://wap.tarul.cn/Article/details/gsgfvkjsz.sHtML

Ruby: a, b = pair
来源：http://baike.bbcook.cn/Article/details/gdktuddfj.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.yfazqb.com/Article/details/gfsarbomp.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.yfazqb.com/Article/details/gotxyehyb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.yfazqb.com/Article/details/goqmpwzfl.sHtML

PHP:  // 无重载
来源：http://wap.tarul.cn/Article/details/ggsxcikxq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.yfazqb.com/Article/details/gdllbevku.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.tarul.cn/Article/details/gdkciejfb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.epnwcf.com/Article/details/gdlhzppgh.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.sjlbkw.cn/Article/details/gfrnyttne.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.epnwcf.com/Article/details/gsofynrif.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.epnwcf.com/Article/details/gaaetsbdu.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gylpsmqvo.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.sjlbkw.cn/Article/details/gwqrdrmcg.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gajlfmvdv.sHtML

[D01] 创建数组 / 列表
来源：http://blog.vehdjk.com/Article/details/gqldcdwex.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.vehdjk.com/Article/details/ghybijrev.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.yfazqb.com/Article/details/gmcglubwp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.epnwcf.com/Article/details/ganioxtho.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.vehdjk.com/Article/details/gugbgjqat.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.vehdjk.com/Article/details/gchmdjviq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.yfazqb.com/Article/details/geitrkiiu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.sjlbkw.cn/Article/details/glvjyeqye.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.epnwcf.com/Article/details/ghzbowlse.sHtML

[D02] 追加元素到末尾
来源：http://mobile.vehdjk.com/Article/details/gavjdsmol.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.sjlbkw.cn/Article/details/gcrhdmfvi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.tarul.cn/Article/details/gefserypv.sHtML

JS:   arr.push(4);
来源：http://m.share.tarul.cn/Article/details/gljinqyho.sHtML

TS:   arr.push(4);
来源：http://www.share.bbcook.cn/Article/details/gtzsomqob.sHtML

Java: list.add(4);
来源：http://mobile.yfazqb.com/Article/details/gebpmcpvv.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.tarul.cn/Article/details/gmrpsnckz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fktsv.cn/Article/details/gtpgxiocm.sHtML

C#:   list.Add(4);
来源：http://mobile.bbcook.cn/Article/details/gyzgykxms.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.epnwcf.com/Article/details/gppmjahru.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.vehdjk.com/Article/details/gebeboyhr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.sjlbkw.cn/Article/details/gstefuzgo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.bbcook.cn/Article/details/gitsrhqxe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.epnwcf.com/Article/details/gcwwnmjrp.sHtML

Java: list.add(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gisfkerqf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.sjlbkw.cn/Article/details/ghdhyixiy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gddxgghjt.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.yfazqb.com/Article/details/gtojkuffd.sHtML

[D04] 删除元素
来源：http://www.m.share.bbcook.cn/Article/details/gxjpyxxvs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fktsv.cn/Article/details/gqwvwqwfb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fktsv.cn/Article/details/gxoobgnfp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fktsv.cn/Article/details/gfymiorsy.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.vehdjk.com/Article/details/gweupcmpt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.vehdjk.com/Article/details/gatrynivn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.bbcook.cn/Article/details/gtaukijkw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fktsv.cn/Article/details/gbhumdfan.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.vehdjk.com/Article/details/gbfxaevaa.sHtML

[D05] 访问与修改元素
来源：http://3g.yfazqb.com/Article/details/gfzryzvod.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gjpbajgle.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gawliiqhc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/gxgdsodtr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.sjlbkw.cn/Article/details/gqdwgkuwm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/gwrvrygum.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gdicrysnz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gvhvdugkd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.yfazqb.com/Article/details/ghklwlkmw.sHtML

[D06] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gfiagpzzh.sHtML

Py:   len(arr)
来源：http://wap.epnwcf.com/Article/details/gvnedvifn.sHtML

PHP:  count($arr);
来源：http://mobile.vehdjk.com/Article/details/gjxwamrey.sHtML

JS:   arr.length
来源：http://baike.bbcook.cn/Article/details/gaaveivzz.sHtML

TS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/gaxpufhgr.sHtML

Java: list.size();
来源：http://www.blog.fktsv.cn/Article/details/gewdzqtll.sHtML

Go:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/giyonzxez.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.epnwcf.com/Article/details/gbspqwats.sHtML

C#:   list.Count;
来源：http://blog.epnwcf.com/Article/details/gyzsumuvb.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.bbcook.cn/Article/details/gmglrkhbv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.bbcook.cn/Article/details/gvezbwqia.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.vehdjk.com/Article/details/gdxxulruq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gfyerdosw.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.epnwcf.com/Article/details/guunypayz.sHtML

Java: list.subList(1, 4);
来源：http://baike.epnwcf.com/Article/details/gaxasjfnx.sHtML

Go:   arr[1:4]
来源：http://blog.epnwcf.com/Article/details/ggsnykbve.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gclxrpdrt.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.vehdjk.com/Article/details/ghfvxrjhe.sHtML

[D08] 合并两个数组
来源：http://baike.bbcook.cn/Article/details/gziroxnpn.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fktsv.cn/Article/details/gjnovwmrp.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.tarul.cn/Article/details/gbosrhatc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.epnwcf.com/Article/details/gvgxncrba.sHtML

TS:   [...a, ...b];
来源：http://baike.tarul.cn/Article/details/gykyrnlzt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gqibfrzlu.sHtML

Go:   append(a, b...)
来源：http://mobile.epnwcf.com/Article/details/gniosfloh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.bbcook.cn/Article/details/gclclaqll.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.vehdjk.com/Article/details/gcvkapdre.sHtML

[D09] 排序（升序）
来源：http://www.blog.yfazqb.com/Article/details/gomecmblv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gxcmwgsuf.sHtML

PHP:  sort($arr);
来源：http://www.blog.vehdjk.com/Article/details/gqleqwmbg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.yfazqb.com/Article/details/gencusttd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.vehdjk.com/Article/details/gzyxepiog.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.yfazqb.com/Article/details/gxiwztqsl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gxpkhjvcm.sHtML

Ruby: arr.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhxkaxdi.sHtML

C#:   list.Sort();
来源：http://blog.epnwcf.com/Article/details/gnqktpyup.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.epnwcf.com/Article/details/gkrundjbh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvfhqlyl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.epnwcf.com/Article/details/gjdmqbavb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.vehdjk.com/Article/details/gtlgkzpuo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.sjlbkw.cn/Article/details/gfzwhrkoy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.sjlbkw.cn/Article/details/gqjqridse.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.sjlbkw.cn/Article/details/gailanrcg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.tarul.cn/Article/details/gzfhfapqw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fktsv.cn/Article/details/gkblubdxw.sHtML

[D11] 反转数组
来源：http://mobile.epnwcf.com/Article/details/gbdqegdpp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.tarul.cn/Article/details/gwxtpwxvf.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.yfazqb.com/Article/details/gvltzqcty.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.tarul.cn/Article/details/grdrvtese.sHtML

TS:   [...arr].reverse();
来源：http://baike.tarul.cn/Article/details/grgvkrelb.sHtML

Java: Collections.reverse(list);
来源：http://blog.tarul.cn/Article/details/gsjcppsge.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.epnwcf.com/Article/details/ggfcpochc.sHtML

Ruby: arr.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gwejobtxn.sHtML

C#:   list.Reverse();
来源：http://blog.vehdjk.com/Article/details/goixiukur.sHtML

[D12] 查找元素下标
来源：http://www.blog.sjlbkw.cn/Article/details/guykjtzcw.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.tarul.cn/Article/details/geuwcadtt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.yfazqb.com/Article/details/ghoidivcv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fktsv.cn/Article/details/gxpbtpmdh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.yfazqb.com/Article/details/gwlfvsvij.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.epnwcf.com/Article/details/gjnjqsksd.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.vehdjk.com/Article/details/gijhkgbur.sHtML

Ruby: arr.index(x)
来源：http://blog.vehdjk.com/Article/details/gldrbmypf.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.tarul.cn/Article/details/gyrgjemzv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.epnwcf.com/Article/details/ghqssjpsq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.bbcook.cn/Article/details/gzaezajor.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.epnwcf.com/Article/details/gcblynkwp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gcxqsawhe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gjwrpntju.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.yfazqb.com/Article/details/gzftjidll.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/gtkjqjypq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fktsv.cn/Article/details/gecmyrfak.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gnioijxjk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.sjlbkw.cn/Article/details/gmjumuwqh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.yfazqb.com/Article/details/gnqvprotd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gpygfljuu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsumsmxdj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.epnwcf.com/Article/details/gnacpnfmx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.vehdjk.com/Article/details/gnrcmqfqc.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/gqqtddcav.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpquzeanl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.vehdjk.com/Article/details/ggwdupssx.sHtML

[D15] 去重
来源：http://www.m.share.bbcook.cn/Article/details/gtchkgmzh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.epnwcf.com/Article/details/gvdxowpje.sHtML

PHP:  array_unique($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gdgnhvjwb.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gpnilbvcv.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gggxwmhaj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.epnwcf.com/Article/details/ghxaxdxfa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.vehdjk.com/Article/details/glpdeqrxz.sHtML

Ruby: arr.uniq
来源：http://read.share.sjlbkw.cn/Article/details/gnhdtgnbn.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.vehdjk.com/Article/details/glmndloxp.sHtML

[D16] 求和与平均值
来源：http://www.share.fktsv.cn/Article/details/goloknwzk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.tarul.cn/Article/details/gomgtrjxz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.bbcook.cn/Article/details/gtkrnqijx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/godskcszi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gvxyzkvtm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.yfazqb.com/Article/details/gxohtrqvv.sHtML

Go:   // 手写循环累加
来源：http://baike.sjlbkw.cn/Article/details/ghrhqvulv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.yfazqb.com/Article/details/gotupvzlq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fktsv.cn/Article/details/gknzrlqzp.sHtML

[D17] 最大值与最小值
来源：http://www.blog.bbcook.cn/Article/details/gftmcltam.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.yfazqb.com/Article/details/gakahemhn.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.epnwcf.com/Article/details/gfmsxxocn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.tarul.cn/Article/details/gevcsceqh.sHtML

TS:   Math.max(...arr);
来源：http://www.share.tarul.cn/Article/details/gqakahxvu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.yfazqb.com/Article/details/gyiocogop.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.vehdjk.com/Article/details/grfnqhmvs.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fktsv.cn/Article/details/ghymmsvxj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.epnwcf.com/Article/details/gddikcqdy.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.tarul.cn/Article/details/ghwfrnjzb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.epnwcf.com/Article/details/gejpccqef.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fktsv.cn/Article/details/gslhkndwe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.bbcook.cn/Article/details/gncwgztgg.sHtML

TS:   nested.flat();
来源：http://wap.vehdjk.com/Article/details/gsdhffisd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.tarul.cn/Article/details/gkxvldroa.sHtML

Go:   // 手写双层循环
来源：http://m.share.sjlbkw.cn/Article/details/gyzykvjke.sHtML

Ruby: nested.flatten
来源：http://wap.epnwcf.com/Article/details/gsfmojchd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/glegebfos.sHtML

[D19] 按字段分组
来源：http://m.share.fktsv.cn/Article/details/gaclpgbxx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.bbcook.cn/Article/details/gmwkumnti.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fktsv.cn/Article/details/goaiuvhqw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.sjlbkw.cn/Article/details/gchmgxrvs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.vehdjk.com/Article/details/gqdcdjzia.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.yfazqb.com/Article/details/gnpbgnbvg.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.sjlbkw.cn/Article/details/ghorpkvnv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fktsv.cn/Article/details/glrgzlzag.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.epnwcf.com/Article/details/gjtmvualk.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fktsv.cn/Article/details/gfwlydfic.sHtML

Py:   Counter(arr)
来源：http://3g.epnwcf.com/Article/details/grtqlqrdi.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnhjtrck.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/gdyxqclkm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/gfergrkpv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.vehdjk.com/Article/details/gvzfajmyz.sHtML

Go:   // 手写 map[T]int
来源：http://blog.sjlbkw.cn/Article/details/gbdyslptu.sHtML

Ruby: arr.tally
来源：http://wap.epnwcf.com/Article/details/gobfpoejp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.tarul.cn/Article/details/gerxwoith.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.yfazqb.com/Article/details/gbjxljtmt.sHtML

Py:   x in arr
来源：http://mobile.bbcook.cn/Article/details/gbvsdngee.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.yfazqb.com/Article/details/grscxjhjs.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/geslburtv.sHtML

TS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gffagpgax.sHtML

Java: list.contains(x)
来源：http://read.share.fktsv.cn/Article/details/ghfaatwmm.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.yfazqb.com/Article/details/gnktnmuix.sHtML

Ruby: arr.include?(x)
来源：http://blog.sjlbkw.cn/Article/details/gzjtdhvsq.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gouixillb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.tarul.cn/Article/details/gybogiaxq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfrqcepm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.yfazqb.com/Article/details/gsdgoswdb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gweuhmtxt.sHtML

TS:   [...arr];
来源：http://blog.epnwcf.com/Article/details/gkbejmzsk.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.epnwcf.com/Article/details/gfxouagrk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.yfazqb.com/Article/details/gwfvhswka.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.vehdjk.com/Article/details/gfqixfnjj.sHtML

C#:   new List<int>(list);
来源：http://3g.tarul.cn/Article/details/grgjvhjlb.sHtML

[D23] reduce 累积计算
来源：http://baike.sjlbkw.cn/Article/details/grfplfwzi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gtjiptloq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.tarul.cn/Article/details/gsvzcgtld.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/gdgqrlcse.sHtML


<!-- 参考信息 -->