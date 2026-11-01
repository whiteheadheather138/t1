代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fktsv.cn/Article/details/gzrfcjfjc.sHtML

[C03] 可变参数
来源：http://3g.fktsv.cn/Article/details/gxlevdqnr.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.yfazqb.com/Article/details/gevixuadl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fktsv.cn/Article/details/gcmgmjjvx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.epnwcf.com/Article/details/ghfkrnhwq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.vehdjk.com/Article/details/gzdhhgkkk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.sjlbkw.cn/Article/details/ghgxpvqap.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.epnwcf.com/Article/details/gwdcownci.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.sjlbkw.cn/Article/details/gplnorwpe.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.vehdjk.com/Article/details/gpkmsxaax.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.vehdjk.com/Article/details/gnqmwrjot.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.tarul.cn/Article/details/gfwewzvpp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.epnwcf.com/Article/details/gabhzvxjy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/gkiepynjx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.yfazqb.com/Article/details/gtkveubhd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.sjlbkw.cn/Article/details/gtkajfxpz.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.yfazqb.com/Article/details/gyvnkolhu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/ghncdelhv.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.epnwcf.com/Article/details/ghdzfbbff.sHtML

[C05] 返回多个值
来源：http://read.share.epnwcf.com/Article/details/gdkthtbqf.sHtML

Py:   return a, b
来源：http://mobile.fktsv.cn/Article/details/gyxuapldo.sHtML

PHP:  return [$a, $b];
来源：http://wap.fktsv.cn/Article/details/gpgejysbt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.sjlbkw.cn/Article/details/gzddsvvjt.sHtML

TS:   return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gctqrjirn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.vehdjk.com/Article/details/gykcvurti.sHtML

Go:   return a, b
来源：http://www.blog.fktsv.cn/Article/details/gzvskwycx.sHtML

Ruby: return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkrgzwmt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.vehdjk.com/Article/details/gjxdisbpd.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.epnwcf.com/Article/details/gywfirafn.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.yfazqb.com/Article/details/gbqawbclh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.epnwcf.com/Article/details/gisvakyba.sHtML

JS:   const square = x => x * x;
来源：http://m.share.tarul.cn/Article/details/gufgvfhdn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.bbcook.cn/Article/details/gkusemugd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.vehdjk.com/Article/details/gaindtpmq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.sjlbkw.cn/Article/details/gwbneuqav.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.sjlbkw.cn/Article/details/giduptksx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.tarul.cn/Article/details/gymeupszu.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.tarul.cn/Article/details/gbhagsfyx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fktsv.cn/Article/details/glndqptyr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.bbcook.cn/Article/details/gpwsibbhk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.sjlbkw.cn/Article/details/gsqsujiub.sHtML

TS:   arr.map(String)
来源：http://read.share.sjlbkw.cn/Article/details/grobupcfr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fktsv.cn/Article/details/guogcpbdo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.sjlbkw.cn/Article/details/gmzzajqrw.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fktsv.cn/Article/details/gxjcrtufp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.yfazqb.com/Article/details/gofiyadoa.sHtML

[C08] 闭包
来源：http://m.share.epnwcf.com/Article/details/gfwegyqve.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fktsv.cn/Article/details/guvqyggsy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.vehdjk.com/Article/details/gmhblpzot.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gutodghym.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.sjlbkw.cn/Article/details/gadoatuok.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.tarul.cn/Article/details/gkhlmdyhs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.bbcook.cn/Article/details/gmrkajwng.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.vehdjk.com/Article/details/gbilohoxd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gvdwtqyud.sHtML

[C09] 递归
来源：http://www.share.tarul.cn/Article/details/gwifomnoq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.bbcook.cn/Article/details/gebukbddz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.yfazqb.com/Article/details/gfkepdosc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/gmiadgpem.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gsagvjkwt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gdaagcbtd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbggftbkm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.tarul.cn/Article/details/gsvizppiu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.bbcook.cn/Article/details/gdjtvhdpr.sHtML

[C10] 变量作用域
来源：http://www.share.vehdjk.com/Article/details/gzskuxslt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.sjlbkw.cn/Article/details/gerlwknfo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.vehdjk.com/Article/details/gxcvobkts.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.yfazqb.com/Article/details/glnpgxlzk.sHtML

TS:   同 JS
来源：http://baike.vehdjk.com/Article/details/gadayolas.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.vehdjk.com/Article/details/ghhhtlguu.sHtML

Go:   花括号块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/grnqoqubg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.sjlbkw.cn/Article/details/gvhxmpjki.sHtML

C#:   块级作用域
来源：http://3g.fktsv.cn/Article/details/gzmqyymsw.sHtML

[C11] 模块导入与导出
来源：http://www.blog.epnwcf.com/Article/details/gjcunmpsc.sHtML

Py:   from module import func
来源：http://www.blog.epnwcf.com/Article/details/goqeasgyi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fktsv.cn/Article/details/gqxokczga.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.tarul.cn/Article/details/gquhssnbf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.epnwcf.com/Article/details/geatupdrs.sHtML

Java: import java.util.List;
来源：http://www.share.yfazqb.com/Article/details/gtyaqjwka.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fktsv.cn/Article/details/ggpvleeur.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.vehdjk.com/Article/details/gbuuucsou.sHtML

C#:   using System.Text;
来源：http://www.blog.sjlbkw.cn/Article/details/guonzfaep.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fktsv.cn/Article/details/giujxyfis.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fktsv.cn/Article/details/gpmebahxu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.sjlbkw.cn/Article/details/gucunwqop.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/gqmzctihn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.vehdjk.com/Article/details/gkxjqlyii.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.tarul.cn/Article/details/gldjjjulx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.bbcook.cn/Article/details/geyhhyuou.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.bbcook.cn/Article/details/gzvvuzaol.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.yfazqb.com/Article/details/gkrqljtcj.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.sjlbkw.cn/Article/details/gxqsofsxl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.vehdjk.com/Article/details/grbnrlxeg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/glrcovuvg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.epnwcf.com/Article/details/gjssxwvwr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.tarul.cn/Article/details/graadueck.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/grbkdjwem.sHtML

Go:   func add(a, b int) int
来源：http://3g.sjlbkw.cn/Article/details/grltpilcy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.sjlbkw.cn/Article/details/goonwzqcc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.vehdjk.com/Article/details/gudvtilsz.sHtML

[C14] 泛型函数
来源：http://wap.fktsv.cn/Article/details/gfdajcfxb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.yfazqb.com/Article/details/gxjepcvtq.sHtML

PHP:  // 无泛型
来源：http://m.share.epnwcf.com/Article/details/gyeyoosan.sHtML

JS:   // 无泛型
来源：http://blog.bbcook.cn/Article/details/gzaziotls.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghowldrbp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.sjlbkw.cn/Article/details/guxwbdnqc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.bbcook.cn/Article/details/gcvbgewmt.sHtML

Ruby: # 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gruaprvog.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.sjlbkw.cn/Article/details/gdsaqgmpm.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.bbcook.cn/Article/details/gunscgasd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.vehdjk.com/Article/details/gxryuxtbe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.sjlbkw.cn/Article/details/grkkvuqlu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/gzwqdejak.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.yfazqb.com/Article/details/gqsxklyfo.sHtML

Java: // 无解构
来源：http://www.blog.epnwcf.com/Article/details/gwdstedji.sHtML

Go:   // 无解构
来源：http://www.m.share.tarul.cn/Article/details/gjtrkzgut.sHtML

Ruby: a, b = pair
来源：http://m.share.fktsv.cn/Article/details/gphzbpofb.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fktsv.cn/Article/details/gvkpthfrv.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fktsv.cn/Article/details/glsjwvqae.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.yfazqb.com/Article/details/gsnfkwsob.sHtML

PHP:  // 无重载
来源：http://baike.tarul.cn/Article/details/geereoehs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.bbcook.cn/Article/details/gekndehto.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.yfazqb.com/Article/details/gdfyaxzdk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.epnwcf.com/Article/details/ggoofwtmc.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.sjlbkw.cn/Article/details/gxskvapqx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.tarul.cn/Article/details/grojksqel.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.sjlbkw.cn/Article/details/gxkscbcbm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqzvgwyql.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.yfazqb.com/Article/details/gynioavlt.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gtrufeezr.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.vehdjk.com/Article/details/gihinrvpb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.bbcook.cn/Article/details/gdemcqhzr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.tarul.cn/Article/details/ggyqcwweo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.bbcook.cn/Article/details/gvfvcebiu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.yfazqb.com/Article/details/gafjhnvxl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.tarul.cn/Article/details/grmufrark.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.tarul.cn/Article/details/gyoujnngv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.sjlbkw.cn/Article/details/gvqveovsp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.epnwcf.com/Article/details/gyaqxfdmm.sHtML

[D02] 追加元素到末尾
来源：http://3g.sjlbkw.cn/Article/details/gzugnzsyw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.vehdjk.com/Article/details/ghghncjkp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fktsv.cn/Article/details/gbdixmkou.sHtML

JS:   arr.push(4);
来源：http://mobile.fktsv.cn/Article/details/gcllpmmnu.sHtML

TS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/gzgumsttc.sHtML

Java: list.add(4);
来源：http://read.share.fktsv.cn/Article/details/gogljgufm.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.vehdjk.com/Article/details/gnahlakrc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.yfazqb.com/Article/details/guotkgoko.sHtML

C#:   list.Add(4);
来源：http://www.blog.tarul.cn/Article/details/gtfcwwpgw.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fktsv.cn/Article/details/gcfsyjdtz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gljfsnxfh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fktsv.cn/Article/details/glzqjoukt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.bbcook.cn/Article/details/gyjdggyep.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fktsv.cn/Article/details/gezwsqzly.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.tarul.cn/Article/details/gjyignlzt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.yfazqb.com/Article/details/glwhhbhut.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.vehdjk.com/Article/details/gyotnyrss.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gnvcpeuyu.sHtML

[D04] 删除元素
来源：http://read.share.fktsv.cn/Article/details/ghwpeigju.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.yfazqb.com/Article/details/gkovjwerq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.epnwcf.com/Article/details/gmtmeihil.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.bbcook.cn/Article/details/gqbtwvyrd.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.epnwcf.com/Article/details/gmdiipysm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.tarul.cn/Article/details/gwbrwzdxx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.vehdjk.com/Article/details/gbqiloyjr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.sjlbkw.cn/Article/details/gakwxkoef.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.epnwcf.com/Article/details/gwsswbqbm.sHtML

[D05] 访问与修改元素
来源：http://www.share.tarul.cn/Article/details/glwpxcwoj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/gqrrqddnc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gbznkmust.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/gwzmskxmy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.bbcook.cn/Article/details/gepmhzbug.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.vehdjk.com/Article/details/gkthvcvqx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gnnemexog.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/guvqcuklg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gqnqxddtb.sHtML

[D06] 数组长度
来源：http://www.blog.yfazqb.com/Article/details/ghortqlxz.sHtML

Py:   len(arr)
来源：http://baike.fktsv.cn/Article/details/gjkehzwwn.sHtML

PHP:  count($arr);
来源：http://www.share.bbcook.cn/Article/details/gytlmsllf.sHtML

JS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/gblxpxvxk.sHtML

TS:   arr.length
来源：http://www.share.sjlbkw.cn/Article/details/gpzkigzxh.sHtML

Java: list.size();
来源：http://blog.bbcook.cn/Article/details/gjiducbxo.sHtML

Go:   len(arr)
来源：http://baike.fktsv.cn/Article/details/gmptaxcaa.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.epnwcf.com/Article/details/glzsphnfv.sHtML

C#:   list.Count;
来源：http://mobile.bbcook.cn/Article/details/ghghjcpjz.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.bbcook.cn/Article/details/gahrqopfe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.yfazqb.com/Article/details/gyrlfjbje.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fktsv.cn/Article/details/gueepcqon.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/gkeutqzep.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.yfazqb.com/Article/details/ghihdfgrt.sHtML

Java: list.subList(1, 4);
来源：http://www.share.tarul.cn/Article/details/gedjkspwa.sHtML

Go:   arr[1:4]
来源：http://www.share.yfazqb.com/Article/details/gddsfvkky.sHtML

Ruby: arr[1, 3]
来源：http://wap.sjlbkw.cn/Article/details/gpsydvwdt.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.bbcook.cn/Article/details/gvolwkoyf.sHtML

[D08] 合并两个数组
来源：http://3g.fktsv.cn/Article/details/gvfgsnhqn.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.tarul.cn/Article/details/gaeneffwk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.vehdjk.com/Article/details/gmemhjfjd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.vehdjk.com/Article/details/gltlscmfe.sHtML

TS:   [...a, ...b];
来源：http://mobile.sjlbkw.cn/Article/details/geclhckax.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.epnwcf.com/Article/details/gugnakpyb.sHtML

Go:   append(a, b...)
来源：http://wap.vehdjk.com/Article/details/gopthkofu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.sjlbkw.cn/Article/details/gzqwrolxx.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.tarul.cn/Article/details/gfvsloyut.sHtML

[D09] 排序（升序）
来源：http://baike.epnwcf.com/Article/details/gidaqdepe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmezzccve.sHtML

PHP:  sort($arr);
来源：http://baike.yfazqb.com/Article/details/gvwyagsiq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.bbcook.cn/Article/details/gpuzeotot.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.epnwcf.com/Article/details/ghtmdtefn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.vehdjk.com/Article/details/gjkhobduo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/gvcfsilcg.sHtML

Ruby: arr.sort
来源：http://mobile.fktsv.cn/Article/details/gdwyyhhev.sHtML

C#:   list.Sort();
来源：http://read.share.sjlbkw.cn/Article/details/ggcacvqbx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.epnwcf.com/Article/details/guximzxpk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fktsv.cn/Article/details/gazutahrb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.epnwcf.com/Article/details/giulwxuyt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fktsv.cn/Article/details/gxfcqqbdg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/gewfesiuj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.bbcook.cn/Article/details/ggtckxrxz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.tarul.cn/Article/details/gxcyrqufb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.yfazqb.com/Article/details/gtplcmeox.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.vehdjk.com/Article/details/gdeonfeks.sHtML

[D11] 反转数组
来源：http://www.blog.tarul.cn/Article/details/giriinogc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/grlviolfq.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaeabkynt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fktsv.cn/Article/details/gdpaojakz.sHtML

TS:   [...arr].reverse();
来源：http://baike.sjlbkw.cn/Article/details/gjamxxvwp.sHtML

Java: Collections.reverse(list);
来源：http://wap.vehdjk.com/Article/details/gnghrosdc.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gxcqmukwr.sHtML

Ruby: arr.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gnorawekn.sHtML

C#:   list.Reverse();
来源：http://read.share.epnwcf.com/Article/details/gjcyrebzk.sHtML

[D12] 查找元素下标
来源：http://blog.tarul.cn/Article/details/gmqgvpjiv.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fktsv.cn/Article/details/granbrouj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.yfazqb.com/Article/details/gjglfszzz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.epnwcf.com/Article/details/gfuvbhdlg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.vehdjk.com/Article/details/gbtnsrxqq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.yfazqb.com/Article/details/gsqphkbll.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gemliezje.sHtML

Ruby: arr.index(x)
来源：http://wap.tarul.cn/Article/details/gpucnamgq.sHtML

C#:   list.IndexOf(x);
来源：http://wap.bbcook.cn/Article/details/ggrgwfvmv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.tarul.cn/Article/details/gqsblujdl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.sjlbkw.cn/Article/details/grzqifvqk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.epnwcf.com/Article/details/gaoyugpao.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.sjlbkw.cn/Article/details/gnswfnemt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gxdfmudto.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.yfazqb.com/Article/details/gfazoqvvd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fktsv.cn/Article/details/gqajjwpgx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.bbcook.cn/Article/details/gnzlyjctb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.tarul.cn/Article/details/gyjelgmvo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fktsv.cn/Article/details/gxysnepkv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.bbcook.cn/Article/details/gfhoreshf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.bbcook.cn/Article/details/gkuswozkd.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/grfuldqan.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.sjlbkw.cn/Article/details/gzmullssg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gefgmftfl.sHtML

Go:   // 手写循环
来源：http://www.m.share.tarul.cn/Article/details/gbudwrrbt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.epnwcf.com/Article/details/gnsvaelpj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.vehdjk.com/Article/details/goslyfhls.sHtML

[D15] 去重
来源：http://read.share.fktsv.cn/Article/details/gvynofrzr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.yfazqb.com/Article/details/gmfywsvmt.sHtML

PHP:  array_unique($arr);
来源：http://blog.epnwcf.com/Article/details/gjaczlvbb.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/galbrcwra.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gelsyujvb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.tarul.cn/Article/details/gkjnojkcn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.vehdjk.com/Article/details/gffimglqx.sHtML

Ruby: arr.uniq
来源：http://baike.sjlbkw.cn/Article/details/gchbvcxsf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.tarul.cn/Article/details/gffgtsazl.sHtML

[D16] 求和与平均值
来源：http://read.share.fktsv.cn/Article/details/gkyijlpgu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fktsv.cn/Article/details/geidomwjb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.bbcook.cn/Article/details/gfiumxnaa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/goijpabri.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/gzuctaevd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.vehdjk.com/Article/details/gqxragmgc.sHtML

Go:   // 手写循环累加
来源：http://blog.tarul.cn/Article/details/gasbsyocl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.yfazqb.com/Article/details/gafknuhlj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.vehdjk.com/Article/details/glyzrepys.sHtML

[D17] 最大值与最小值
来源：http://wap.fktsv.cn/Article/details/gnfnqbgwr.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.yfazqb.com/Article/details/grekgpwqc.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.bbcook.cn/Article/details/gyubrrxeq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.epnwcf.com/Article/details/gwavovawc.sHtML

TS:   Math.max(...arr);
来源：http://www.share.tarul.cn/Article/details/gwirvpwto.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.epnwcf.com/Article/details/gwbqaiksd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.tarul.cn/Article/details/gfucljdav.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.yfazqb.com/Article/details/gzmjqiybs.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.vehdjk.com/Article/details/gfyshgvhk.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/ggilrdybw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.yfazqb.com/Article/details/goiamlapf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.bbcook.cn/Article/details/gejrhxxih.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fktsv.cn/Article/details/gydtdiaak.sHtML

TS:   nested.flat();
来源：http://read.share.sjlbkw.cn/Article/details/gefngmdcw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.vehdjk.com/Article/details/gglauumvh.sHtML

Go:   // 手写双层循环
来源：http://blog.epnwcf.com/Article/details/grmclcozq.sHtML

Ruby: nested.flatten
来源：http://www.share.vehdjk.com/Article/details/gpsbziwlu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gwrqkovqc.sHtML

[D19] 按字段分组
来源：http://www.share.vehdjk.com/Article/details/goqttkycl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.tarul.cn/Article/details/guwoqohvx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fktsv.cn/Article/details/gugwcaccq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.vehdjk.com/Article/details/giimgbutk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/gsisgrmsj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.vehdjk.com/Article/details/gcxuvhfci.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.bbcook.cn/Article/details/gyshalnyl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.tarul.cn/Article/details/glsjkkrah.sHtML


<!-- 参考信息 -->