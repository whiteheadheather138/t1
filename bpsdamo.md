代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://wap.tarul.cn/Article/details/gveumvuvi.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.vehdjk.com/Article/details/gjaumuvpu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.epnwcf.com/Article/details/gijpnckfm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fktsv.cn/Article/details/glmmdcczp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.yfazqb.com/Article/details/gkfclrwyl.sHtML

TS:   arr.map(String)
来源：http://m.share.yfazqb.com/Article/details/gmsoedkhf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrppmwdy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.yfazqb.com/Article/details/gvvsnwzdp.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.epnwcf.com/Article/details/ggaaajawl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.tarul.cn/Article/details/gqpgogzmc.sHtML

[C08] 闭包
来源：http://mobile.fktsv.cn/Article/details/gszwgsnyg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fktsv.cn/Article/details/gumyxasmo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.epnwcf.com/Article/details/gcyiehevv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gtteefwtr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gigvwydlj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.tarul.cn/Article/details/gebvqmjps.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fktsv.cn/Article/details/gkvqtwncj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fktsv.cn/Article/details/gjijnlzza.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gaugdsjcu.sHtML

[C09] 递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfifvpkl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gcgkssvdu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.vehdjk.com/Article/details/gsqhxjhkt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/gqckregig.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.bbcook.cn/Article/details/gqflafbia.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.tarul.cn/Article/details/giadtwhcf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.yfazqb.com/Article/details/gcrfhdybz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fktsv.cn/Article/details/gnlwvqkrl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.sjlbkw.cn/Article/details/gftzwkclb.sHtML

[C10] 变量作用域
来源：http://www.m.share.vehdjk.com/Article/details/guqprrclp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.tarul.cn/Article/details/gfarxdsdt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.epnwcf.com/Article/details/gaagqojuc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.tarul.cn/Article/details/gtbcxmeih.sHtML

TS:   同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gcehfaxoa.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.bbcook.cn/Article/details/gpemrnogp.sHtML

Go:   花括号块级作用域
来源：http://read.share.epnwcf.com/Article/details/ghfdrzenb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fktsv.cn/Article/details/ggfphavdl.sHtML

C#:   块级作用域
来源：http://baike.yfazqb.com/Article/details/grhiwmnkp.sHtML

[C11] 模块导入与导出
来源：http://m.share.sjlbkw.cn/Article/details/gcmwdakiz.sHtML

Py:   from module import func
来源：http://blog.bbcook.cn/Article/details/gltuceubx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.vehdjk.com/Article/details/giqgddsgk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/gqyiuhttm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.epnwcf.com/Article/details/giotkkglx.sHtML

Java: import java.util.List;
来源：http://read.share.bbcook.cn/Article/details/gbavqhpgc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.sjlbkw.cn/Article/details/gtzpinuyv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.vehdjk.com/Article/details/gdazbnkmd.sHtML

C#:   using System.Text;
来源：http://wap.bbcook.cn/Article/details/gximfrfif.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.sjlbkw.cn/Article/details/gcpsmwxqj.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.sjlbkw.cn/Article/details/gvlzptczm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.bbcook.cn/Article/details/grkyephyl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gybomgfda.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.bbcook.cn/Article/details/ghpbsnppk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.epnwcf.com/Article/details/gwjhpleqt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fktsv.cn/Article/details/gepoaxssr.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fktsv.cn/Article/details/gdbendbeh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gcatbdcxb.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.tarul.cn/Article/details/gixapinrv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fktsv.cn/Article/details/geanszmkf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gwaxbfifl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.sjlbkw.cn/Article/details/gixvpgqhh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/guclptsry.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gshckeixh.sHtML

Go:   func add(a, b int) int
来源：http://baike.tarul.cn/Article/details/gkscuvcjq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.epnwcf.com/Article/details/gujwwitkk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.sjlbkw.cn/Article/details/gsettpbio.sHtML

[C14] 泛型函数
来源：http://www.share.sjlbkw.cn/Article/details/gfxuytzmu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.yfazqb.com/Article/details/griwkqxhh.sHtML

PHP:  // 无泛型
来源：http://m.share.fktsv.cn/Article/details/gnnxpfjak.sHtML

JS:   // 无泛型
来源：http://m.share.tarul.cn/Article/details/gwsnkedua.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.vehdjk.com/Article/details/ghrpigxug.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.tarul.cn/Article/details/gcvddermr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.epnwcf.com/Article/details/gpxijesqz.sHtML

Ruby: # 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gkdsuiqev.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.sjlbkw.cn/Article/details/gekawvjhf.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.tarul.cn/Article/details/gdsjzdkxb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.tarul.cn/Article/details/ggqikhnrd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.sjlbkw.cn/Article/details/gkntrgrqg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/gwvjokzqx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.bbcook.cn/Article/details/ghxdqvjet.sHtML

Java: // 无解构
来源：http://read.share.bbcook.cn/Article/details/gksiyebia.sHtML

Go:   // 无解构
来源：http://m.share.vehdjk.com/Article/details/gstddosgo.sHtML

Ruby: a, b = pair
来源：http://wap.epnwcf.com/Article/details/gadmhdujv.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.sjlbkw.cn/Article/details/gtvzqtwpq.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.tarul.cn/Article/details/gskucerwv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.bbcook.cn/Article/details/gqncfxpyf.sHtML

PHP:  // 无重载
来源：http://m.share.bbcook.cn/Article/details/gleyxzmom.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.bbcook.cn/Article/details/gkewupdat.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fktsv.cn/Article/details/gyxbxuhhn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.vehdjk.com/Article/details/ghccqoelt.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.bbcook.cn/Article/details/gmenmfbuo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.sjlbkw.cn/Article/details/gphgxuekw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.yfazqb.com/Article/details/ggkyixnrp.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grzwcgmmh.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.vehdjk.com/Article/details/gipbfuqst.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gfaheqzlx.sHtML

[D01] 创建数组 / 列表
来源：http://3g.bbcook.cn/Article/details/gspkbqwcr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.vehdjk.com/Article/details/geoideyvr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.bbcook.cn/Article/details/gbluuqimx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.epnwcf.com/Article/details/gctozgelv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.sjlbkw.cn/Article/details/gephuqswl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.tarul.cn/Article/details/gpmniftvs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.tarul.cn/Article/details/gkljwhxns.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.tarul.cn/Article/details/gaodmzolt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fktsv.cn/Article/details/gdtfkvhom.sHtML

[D02] 追加元素到末尾
来源：http://wap.epnwcf.com/Article/details/gguhfwvjy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.tarul.cn/Article/details/gurwstgpp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.epnwcf.com/Article/details/gbdkrmeil.sHtML

JS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/gckmsdyym.sHtML

TS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/ggvddeoet.sHtML

Java: list.add(4);
来源：http://mobile.vehdjk.com/Article/details/gjzyaczys.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.tarul.cn/Article/details/gzthqzaea.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.epnwcf.com/Article/details/goblbqcxd.sHtML

C#:   list.Add(4);
来源：http://www.share.epnwcf.com/Article/details/gfpdjqsic.sHtML

[D03] 在指定位置插入元素
来源：http://wap.bbcook.cn/Article/details/gmlcsyrka.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.sjlbkw.cn/Article/details/gyvvlwjbl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.sjlbkw.cn/Article/details/gzzffdjcw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.vehdjk.com/Article/details/gbpdmuhcj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.bbcook.cn/Article/details/gcehzevfr.sHtML

Java: list.add(0, 0);
来源：http://mobile.tarul.cn/Article/details/gwnqjldmo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.yfazqb.com/Article/details/gnjoaqpvt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.sjlbkw.cn/Article/details/gshwwawic.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fktsv.cn/Article/details/gjqbcwkmi.sHtML

[D04] 删除元素
来源：http://www.share.bbcook.cn/Article/details/gyahmwwda.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.yfazqb.com/Article/details/gehupjufw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.tarul.cn/Article/details/gesfxcggn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.sjlbkw.cn/Article/details/gtabpyavw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.yfazqb.com/Article/details/gievlpwyy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.epnwcf.com/Article/details/gcrdlcrmc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.vehdjk.com/Article/details/gdsrsjjev.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fktsv.cn/Article/details/gvlhomnyu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.bbcook.cn/Article/details/gtwpvrfeu.sHtML

[D05] 访问与修改元素
来源：http://wap.epnwcf.com/Article/details/garsrvuoi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/gkzqdgzod.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/grkfajdpb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/gxdeijaoj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.epnwcf.com/Article/details/goppcjufr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.epnwcf.com/Article/details/graglfhck.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gqzymcrxn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gvjeljvmn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/gvragjqtd.sHtML

[D06] 数组长度
来源：http://3g.yfazqb.com/Article/details/grmdmdstl.sHtML

Py:   len(arr)
来源：http://baike.epnwcf.com/Article/details/gnhsexiau.sHtML

PHP:  count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gieanpvzm.sHtML

JS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/gurihyzeg.sHtML

TS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gtbcwndyo.sHtML

Java: list.size();
来源：http://baike.tarul.cn/Article/details/gysdswedg.sHtML

Go:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gnnbxekiz.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fktsv.cn/Article/details/grqbpogub.sHtML

C#:   list.Count;
来源：http://www.m.share.bbcook.cn/Article/details/gxybjmvdk.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fktsv.cn/Article/details/grhmeulna.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.yfazqb.com/Article/details/gwcobikgq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxwypifx.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/gdjlixoll.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gkinsdszn.sHtML

Java: list.subList(1, 4);
来源：http://mobile.bbcook.cn/Article/details/ghqkdvske.sHtML

Go:   arr[1:4]
来源：http://www.m.share.tarul.cn/Article/details/gfmdxrcwx.sHtML

Ruby: arr[1, 3]
来源：http://3g.vehdjk.com/Article/details/ghmuobitp.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.yfazqb.com/Article/details/gqrnzycrz.sHtML

[D08] 合并两个数组
来源：http://wap.tarul.cn/Article/details/gxawahjls.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.tarul.cn/Article/details/gjoxmbcbd.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.yfazqb.com/Article/details/ggpypgyhi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.vehdjk.com/Article/details/gldahrxir.sHtML

TS:   [...a, ...b];
来源：http://blog.epnwcf.com/Article/details/gcyenmolp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gbynynpmb.sHtML

Go:   append(a, b...)
来源：http://3g.sjlbkw.cn/Article/details/gyavjgoyc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.tarul.cn/Article/details/giyihjokn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gvjxmixyd.sHtML

[D09] 排序（升序）
来源：http://baike.bbcook.cn/Article/details/ghqzelcwq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gghcgetkl.sHtML

PHP:  sort($arr);
来源：http://wap.yfazqb.com/Article/details/gemyqafyf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.vehdjk.com/Article/details/ggzbdzjmt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.yfazqb.com/Article/details/gghhajlmf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.tarul.cn/Article/details/gdmxhgpca.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gvxrrhqef.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/gfljdozlz.sHtML

C#:   list.Sort();
来源：http://read.share.tarul.cn/Article/details/gztupabfq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.vehdjk.com/Article/details/gawcmujdz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.epnwcf.com/Article/details/glklxsjmd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.tarul.cn/Article/details/gnuoisivk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.yfazqb.com/Article/details/gvpxdizva.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gdekszate.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fktsv.cn/Article/details/gexcdlmvf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.epnwcf.com/Article/details/gqwsacmmk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.tarul.cn/Article/details/gjkpschrm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.yfazqb.com/Article/details/gqwshllsp.sHtML

[D11] 反转数组
来源：http://read.share.bbcook.cn/Article/details/gnzbfvkkp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.tarul.cn/Article/details/gzudtkzva.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.vehdjk.com/Article/details/gtbtpbsll.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.yfazqb.com/Article/details/grranzbco.sHtML

TS:   [...arr].reverse();
来源：http://read.share.tarul.cn/Article/details/ghwpxrtrq.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fktsv.cn/Article/details/gbzkwkdjh.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gxvzgpmah.sHtML

Ruby: arr.reverse
来源：http://www.blog.vehdjk.com/Article/details/gsuowonph.sHtML

C#:   list.Reverse();
来源：http://wap.sjlbkw.cn/Article/details/gbojiaakw.sHtML

[D12] 查找元素下标
来源：http://wap.vehdjk.com/Article/details/ghswpnnyi.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.epnwcf.com/Article/details/gtlzdtsoz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.sjlbkw.cn/Article/details/gkqglivmw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.bbcook.cn/Article/details/ghffwzssd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/gjwpyhvdb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.yfazqb.com/Article/details/gufqdynqm.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.yfazqb.com/Article/details/gqbmqhbzu.sHtML

Ruby: arr.index(x)
来源：http://wap.epnwcf.com/Article/details/ghoohigmu.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.bbcook.cn/Article/details/gfxklspdk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.sjlbkw.cn/Article/details/gunznhbso.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gwdldepqg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.vehdjk.com/Article/details/gsbbdyazj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/galqqtkqg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fktsv.cn/Article/details/glisxdoxt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.tarul.cn/Article/details/gcdvbxrtw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/gfrorxccw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.vehdjk.com/Article/details/gajstrswb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.epnwcf.com/Article/details/ggmfqfgdl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fktsv.cn/Article/details/gritwzudc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fktsv.cn/Article/details/ggomelfmv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fktsv.cn/Article/details/gbdmfymqx.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fktsv.cn/Article/details/gohdfesqv.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/glhcbcdhn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.vehdjk.com/Article/details/gvvylvgwr.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/gluvgyanr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.tarul.cn/Article/details/gjbbcdzww.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.vehdjk.com/Article/details/geushfxoj.sHtML

[D15] 去重
来源：http://read.share.sjlbkw.cn/Article/details/gdqujyyfw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/gmefirwmb.sHtML

PHP:  array_unique($arr);
来源：http://wap.bbcook.cn/Article/details/ghaatumto.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/giufzlawg.sHtML

TS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gkufysdvc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.sjlbkw.cn/Article/details/gggfqethx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.epnwcf.com/Article/details/glapwhnbg.sHtML

Ruby: arr.uniq
来源：http://3g.sjlbkw.cn/Article/details/gfnorwcxq.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.tarul.cn/Article/details/gvgtcehiz.sHtML

[D16] 求和与平均值
来源：http://mobile.bbcook.cn/Article/details/gohflrcmv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.tarul.cn/Article/details/guamhsibe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.bbcook.cn/Article/details/ghdmpimsk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/gqsamcrda.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/giupwrqzi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.epnwcf.com/Article/details/ghmhrrvsm.sHtML

Go:   // 手写循环累加
来源：http://3g.sjlbkw.cn/Article/details/gbkygccge.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.epnwcf.com/Article/details/gmjpfylro.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.epnwcf.com/Article/details/gylcwdifh.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/gfbiboses.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.bbcook.cn/Article/details/gzfhehszd.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.epnwcf.com/Article/details/ghjfmlxbm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.epnwcf.com/Article/details/ghrccpugk.sHtML

TS:   Math.max(...arr);
来源：http://www.share.tarul.cn/Article/details/gxxedjqrf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fktsv.cn/Article/details/gantdxyfq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.vehdjk.com/Article/details/gagbwciwm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.bbcook.cn/Article/details/gbjgybinb.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.vehdjk.com/Article/details/gfvfcolds.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.epnwcf.com/Article/details/gjxghliis.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.epnwcf.com/Article/details/gclfctwmt.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.bbcook.cn/Article/details/galmcpakg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.yfazqb.com/Article/details/gziqujmaq.sHtML

TS:   nested.flat();
来源：http://read.share.fktsv.cn/Article/details/gvxpiynac.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fktsv.cn/Article/details/gxjtvcvfl.sHtML

Go:   // 手写双层循环
来源：http://m.share.vehdjk.com/Article/details/geicnewnt.sHtML

Ruby: nested.flatten
来源：http://mobile.vehdjk.com/Article/details/gjgibbudt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.tarul.cn/Article/details/goimowbiw.sHtML

[D19] 按字段分组
来源：http://www.share.fktsv.cn/Article/details/gonkdhfpp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.vehdjk.com/Article/details/gvsvcgcdt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.epnwcf.com/Article/details/gtkywporq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.yfazqb.com/Article/details/geexcmblj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.tarul.cn/Article/details/grqnedvae.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.epnwcf.com/Article/details/gebudimdi.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fktsv.cn/Article/details/geimwhtun.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.bbcook.cn/Article/details/gxascnwgu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.vehdjk.com/Article/details/gmdudujuy.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.epnwcf.com/Article/details/geoiyxdgx.sHtML

Py:   Counter(arr)
来源：http://mobile.vehdjk.com/Article/details/gfzvtqimy.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gkjdvcklz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/gbrwctatl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/gtwijcyrx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.tarul.cn/Article/details/gkarlmhgz.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fktsv.cn/Article/details/gzcmvwdsv.sHtML

Ruby: arr.tally
来源：http://www.share.vehdjk.com/Article/details/gpbnbfnxy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.vehdjk.com/Article/details/gxhxynrcv.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.epnwcf.com/Article/details/gsxxknead.sHtML

Py:   x in arr
来源：http://blog.vehdjk.com/Article/details/gbqelkrlg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.vehdjk.com/Article/details/gxfxopwii.sHtML

JS:   arr.includes(x)
来源：http://wap.vehdjk.com/Article/details/gydxbdcqg.sHtML

TS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gxdjlnigr.sHtML

Java: list.contains(x)
来源：http://baike.bbcook.cn/Article/details/gwabyugqc.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.tarul.cn/Article/details/ghasoqhif.sHtML

Ruby: arr.include?(x)
来源：http://www.share.epnwcf.com/Article/details/gkbyukevx.sHtML

C#:   list.Contains(x)
来源：http://wap.fktsv.cn/Article/details/gifniwpoz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.vehdjk.com/Article/details/gaqsatiaf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.bbcook.cn/Article/details/gattijyqa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.yfazqb.com/Article/details/gfmdiiojr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.bbcook.cn/Article/details/glqzchgei.sHtML

TS:   [...arr];
来源：http://3g.sjlbkw.cn/Article/details/gbedcgkqc.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fktsv.cn/Article/details/gtyygnxrv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/gdshugkhr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.epnwcf.com/Article/details/gndelqwsk.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.epnwcf.com/Article/details/gbuogatfd.sHtML

[D23] reduce 累积计算
来源：http://www.blog.bbcook.cn/Article/details/ghhljsrnv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.sjlbkw.cn/Article/details/gtbjuluyo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.yfazqb.com/Article/details/gplhofbov.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/gddiuiglr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.bbcook.cn/Article/details/goeawfmyt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.tarul.cn/Article/details/gvkvaszad.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gbszrxzyo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.epnwcf.com/Article/details/gwwyiavoc.sHtML


<!-- 参考信息 -->