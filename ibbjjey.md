代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://3g.bbcook.cn/Article/details/gwypycmks.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.sjlbkw.cn/Article/details/gwonoipuj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.epnwcf.com/Article/details/gywjqvaxq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.epnwcf.com/Article/details/gwsxofxjm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.tarul.cn/Article/details/gcrbyilde.sHtML

TS:   arr.map(String)
来源：http://blog.epnwcf.com/Article/details/grtqipone.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.yfazqb.com/Article/details/ghiqguekw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.yfazqb.com/Article/details/ghvasigtl.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.sjlbkw.cn/Article/details/gobtyzzpq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.tarul.cn/Article/details/gdemlosoo.sHtML

[C08] 闭包
来源：http://www.m.share.fktsv.cn/Article/details/gqnybxwnn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.tarul.cn/Article/details/guzbzkhcy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gctvsdesw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gmfhqkimx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/ggyanxagx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.vehdjk.com/Article/details/gsnoxatbi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.bbcook.cn/Article/details/gnmxhvqra.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.sjlbkw.cn/Article/details/gdbcjxofk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gdgwpuhcd.sHtML

[C09] 递归
来源：http://read.share.fktsv.cn/Article/details/gamaqmrgd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.bbcook.cn/Article/details/glvpzeupk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fktsv.cn/Article/details/gfhnteetd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.yfazqb.com/Article/details/gkfyukanz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.sjlbkw.cn/Article/details/golzesyto.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fktsv.cn/Article/details/geipbkoro.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.bbcook.cn/Article/details/gtqknnbmo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.tarul.cn/Article/details/gwphakapw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.bbcook.cn/Article/details/gosfnzriw.sHtML

[C10] 变量作用域
来源：http://read.share.bbcook.cn/Article/details/gdxvdpqdy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.vehdjk.com/Article/details/ggnziorsm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.bbcook.cn/Article/details/gkqncourx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.vehdjk.com/Article/details/gpruxfbld.sHtML

TS:   同 JS
来源：http://baike.yfazqb.com/Article/details/gshzsugix.sHtML

Java: 方法内为块级作用域
来源：http://blog.tarul.cn/Article/details/gvumjufgy.sHtML

Go:   花括号块级作用域
来源：http://wap.vehdjk.com/Article/details/gdjvkefen.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.vehdjk.com/Article/details/goexmisql.sHtML

C#:   块级作用域
来源：http://blog.vehdjk.com/Article/details/gjeuottus.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.vehdjk.com/Article/details/gsesfepuj.sHtML

Py:   from module import func
来源：http://www.m.share.fktsv.cn/Article/details/gfffskkgk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.bbcook.cn/Article/details/gaugzghzo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.epnwcf.com/Article/details/ggeyechwx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fktsv.cn/Article/details/gjxzbeinu.sHtML

Java: import java.util.List;
来源：http://mobile.yfazqb.com/Article/details/gxxmrvkdg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.epnwcf.com/Article/details/ghcaocwev.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.epnwcf.com/Article/details/gujtobmdc.sHtML

C#:   using System.Text;
来源：http://blog.tarul.cn/Article/details/gqyufppjx.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.bbcook.cn/Article/details/gwtbhtqrd.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.sjlbkw.cn/Article/details/gdlwfljqm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.sjlbkw.cn/Article/details/gpimapdwq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/gtudfgqnk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/gsprdwrpd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fktsv.cn/Article/details/gxiannarm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.bbcook.cn/Article/details/gwowdqerz.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.sjlbkw.cn/Article/details/gldmjcfoi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.vehdjk.com/Article/details/gvwnojsbd.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.vehdjk.com/Article/details/gegpoymbr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.tarul.cn/Article/details/ghuiajayg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gdeeiaumz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.tarul.cn/Article/details/gdbvewqoj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gvxwdctfz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/ghflnaiuw.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.epnwcf.com/Article/details/gmuaadoig.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.bbcook.cn/Article/details/gjehxgxuo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.sjlbkw.cn/Article/details/gowwvnuxt.sHtML

[C14] 泛型函数
来源：http://www.blog.fktsv.cn/Article/details/goqulyazz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.tarul.cn/Article/details/gykjvmyur.sHtML

PHP:  // 无泛型
来源：http://baike.epnwcf.com/Article/details/gilpesura.sHtML

JS:   // 无泛型
来源：http://www.share.epnwcf.com/Article/details/gpftyscmp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.yfazqb.com/Article/details/gucphixkv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.epnwcf.com/Article/details/gniqiphtp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.yfazqb.com/Article/details/greripnob.sHtML

Ruby: # 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gkfziuffh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.sjlbkw.cn/Article/details/gwznjphwt.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.yfazqb.com/Article/details/gawcnvomq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.sjlbkw.cn/Article/details/guynqtjys.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.epnwcf.com/Article/details/gclwufaju.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.bbcook.cn/Article/details/gwsccgjjt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.tarul.cn/Article/details/gjsioocoi.sHtML

Java: // 无解构
来源：http://read.share.bbcook.cn/Article/details/gpbxkxefh.sHtML

Go:   // 无解构
来源：http://baike.vehdjk.com/Article/details/gpfrylszu.sHtML

Ruby: a, b = pair
来源：http://www.m.share.tarul.cn/Article/details/gtwxhgxte.sHtML

C#:   var (a, b) = pair;
来源：http://wap.yfazqb.com/Article/details/ghyuxdbas.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.sjlbkw.cn/Article/details/gukrgzkyr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fktsv.cn/Article/details/gopebhpri.sHtML

PHP:  // 无重载
来源：http://www.m.share.fktsv.cn/Article/details/gdwgbuzwx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.epnwcf.com/Article/details/grwvscjco.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.bbcook.cn/Article/details/gdmgkvuiw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.yfazqb.com/Article/details/gaskergzt.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.bbcook.cn/Article/details/gmrnzsdge.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.bbcook.cn/Article/details/gnpdmkrml.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.vehdjk.com/Article/details/gyvthhzkh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnvarkxdz.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fktsv.cn/Article/details/gpxrbkceo.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gjjwgtfle.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.sjlbkw.cn/Article/details/gcdhfuzuc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.bbcook.cn/Article/details/groojhzso.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.vehdjk.com/Article/details/ghxznykmh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.yfazqb.com/Article/details/gfxpgcvpu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fktsv.cn/Article/details/gyoumkhzv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.tarul.cn/Article/details/gtmcrbblv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.sjlbkw.cn/Article/details/gzbphrsss.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.yfazqb.com/Article/details/gfyonbsuj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.epnwcf.com/Article/details/glmhjsspu.sHtML

[D02] 追加元素到末尾
来源：http://baike.sjlbkw.cn/Article/details/gfhxtecdc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.sjlbkw.cn/Article/details/gfnnjvccf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.sjlbkw.cn/Article/details/gzroowxof.sHtML

JS:   arr.push(4);
来源：http://www.share.epnwcf.com/Article/details/gdpvptuwf.sHtML

TS:   arr.push(4);
来源：http://blog.fktsv.cn/Article/details/gpunkxlgb.sHtML

Java: list.add(4);
来源：http://baike.sjlbkw.cn/Article/details/gexstrils.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.yfazqb.com/Article/details/gfmudqoth.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.bbcook.cn/Article/details/gtxyadpti.sHtML

C#:   list.Add(4);
来源：http://baike.vehdjk.com/Article/details/gjcpvxufh.sHtML

[D03] 在指定位置插入元素
来源：http://blog.sjlbkw.cn/Article/details/guppuqmjx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gfpzspdcj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.yfazqb.com/Article/details/gmuwnrxcj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.epnwcf.com/Article/details/gzjfkrtnq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fktsv.cn/Article/details/gxakylwml.sHtML

Java: list.add(0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/guowkclls.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.tarul.cn/Article/details/guroxugjl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.tarul.cn/Article/details/geknfhoyb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.tarul.cn/Article/details/gebamigus.sHtML

[D04] 删除元素
来源：http://mobile.fktsv.cn/Article/details/gulfmtdri.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.epnwcf.com/Article/details/gkipfmyyr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fktsv.cn/Article/details/gszvqebhm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.tarul.cn/Article/details/gaddobqyj.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.vehdjk.com/Article/details/gdecsscap.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.tarul.cn/Article/details/ggirfxvge.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.sjlbkw.cn/Article/details/gexndpfar.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fktsv.cn/Article/details/gyexppzqd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.bbcook.cn/Article/details/gitpoygin.sHtML

[D05] 访问与修改元素
来源：http://wap.epnwcf.com/Article/details/gohvtnkty.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gekuagxsg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gcgsqzxaw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/gslmcncpk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.tarul.cn/Article/details/gdsfouvoj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.yfazqb.com/Article/details/govypscnu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gmcwrkhtr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gyyjnbcac.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gsphrwxwu.sHtML

[D06] 数组长度
来源：http://www.share.vehdjk.com/Article/details/gzgqhgezw.sHtML

Py:   len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gapjqvsfl.sHtML

PHP:  count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gugjbhmaz.sHtML

JS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/gdlauofql.sHtML

TS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/gjpjojwbu.sHtML

Java: list.size();
来源：http://www.m.share.vehdjk.com/Article/details/gcxzaxtxa.sHtML

Go:   len(arr)
来源：http://blog.epnwcf.com/Article/details/grnfmvnyz.sHtML

Ruby: arr.length; arr.size
来源：http://3g.vehdjk.com/Article/details/gjmojcuot.sHtML

C#:   list.Count;
来源：http://3g.bbcook.cn/Article/details/gesexqiqz.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.sjlbkw.cn/Article/details/ghamspogh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.sjlbkw.cn/Article/details/gqowfyumr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.yfazqb.com/Article/details/ghywjalgw.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gqoxrhjjs.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/gcadupllu.sHtML

Java: list.subList(1, 4);
来源：http://mobile.bbcook.cn/Article/details/gfngvqvou.sHtML

Go:   arr[1:4]
来源：http://read.share.sjlbkw.cn/Article/details/gmdicgljc.sHtML

Ruby: arr[1, 3]
来源：http://m.share.tarul.cn/Article/details/gncmgsxxz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.epnwcf.com/Article/details/gcwulboaz.sHtML

[D08] 合并两个数组
来源：http://www.blog.tarul.cn/Article/details/gfnzriuit.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.bbcook.cn/Article/details/gpxtsvmig.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.yfazqb.com/Article/details/gfkuxsece.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fktsv.cn/Article/details/grtrbtvnz.sHtML

TS:   [...a, ...b];
来源：http://wap.yfazqb.com/Article/details/gewqguqkf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtykwwblk.sHtML

Go:   append(a, b...)
来源：http://3g.vehdjk.com/Article/details/grfnmfonv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.tarul.cn/Article/details/gjvzpwolr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gmepoyexh.sHtML

[D09] 排序（升序）
来源：http://3g.fktsv.cn/Article/details/giucxhxqt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gttbsipkw.sHtML

PHP:  sort($arr);
来源：http://3g.tarul.cn/Article/details/gjkbjhuhl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.tarul.cn/Article/details/glflotkvi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.sjlbkw.cn/Article/details/gispttpma.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.sjlbkw.cn/Article/details/gdermlghx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.sjlbkw.cn/Article/details/gvfafwvhs.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/glnzmxnkm.sHtML

C#:   list.Sort();
来源：http://www.share.vehdjk.com/Article/details/grfhnwosm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.sjlbkw.cn/Article/details/gdtvvzprw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.tarul.cn/Article/details/gqjspfctu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fktsv.cn/Article/details/ganfdwlky.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/guypidmqk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gorwhdvsc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fktsv.cn/Article/details/gggozhylz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.yfazqb.com/Article/details/gwzuwlhml.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fktsv.cn/Article/details/gfnpbwsjy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.bbcook.cn/Article/details/gdmguxwnr.sHtML

[D11] 反转数组
来源：http://mobile.epnwcf.com/Article/details/gmvmlmqzs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.sjlbkw.cn/Article/details/gkhaoxrwx.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.yfazqb.com/Article/details/gvpotjqoi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.yfazqb.com/Article/details/gtpdiqyoc.sHtML

TS:   [...arr].reverse();
来源：http://baike.epnwcf.com/Article/details/gukeorfrk.sHtML

Java: Collections.reverse(list);
来源：http://baike.bbcook.cn/Article/details/ghepkzsxs.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.yfazqb.com/Article/details/gspgqdwyl.sHtML

Ruby: arr.reverse
来源：http://www.share.bbcook.cn/Article/details/gznzshodz.sHtML

C#:   list.Reverse();
来源：http://read.share.epnwcf.com/Article/details/gkdompnhm.sHtML

[D12] 查找元素下标
来源：http://www.m.share.epnwcf.com/Article/details/guinvbmee.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fktsv.cn/Article/details/gbuhiadqs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fktsv.cn/Article/details/gflppggob.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gyislwbbx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.yfazqb.com/Article/details/grktqdmai.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.yfazqb.com/Article/details/ggxadgayh.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.tarul.cn/Article/details/gdjkugook.sHtML

Ruby: arr.index(x)
来源：http://baike.epnwcf.com/Article/details/gxakslqxo.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fktsv.cn/Article/details/gtbznaxbq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.vehdjk.com/Article/details/glxhbkwdr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fktsv.cn/Article/details/giuudmmmr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.sjlbkw.cn/Article/details/gszxnucvq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fktsv.cn/Article/details/ghsiigfrf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.tarul.cn/Article/details/gxdjzvuyh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.epnwcf.com/Article/details/gumnzwjqg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.yfazqb.com/Article/details/gzpopqzzv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.bbcook.cn/Article/details/gohcodrno.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gvfmkdtbd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.yfazqb.com/Article/details/gtpmubtgt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gurqjpuhu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gbjowqswm.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/ghwbdgngw.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/giuaxrzhq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.bbcook.cn/Article/details/guzkwqwvy.sHtML

Go:   // 手写循环
来源：http://www.share.vehdjk.com/Article/details/gvxbphtxc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.epnwcf.com/Article/details/ghvwiybww.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.bbcook.cn/Article/details/gwruukcqt.sHtML

[D15] 去重
来源：http://mobile.bbcook.cn/Article/details/ghawsqtyj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gdulvxlhc.sHtML

PHP:  array_unique($arr);
来源：http://baike.tarul.cn/Article/details/gmjmxxovz.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gbemrinbx.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gpwnbvuym.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.bbcook.cn/Article/details/ghkscccko.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.yfazqb.com/Article/details/gchyfbmik.sHtML

Ruby: arr.uniq
来源：http://m.share.epnwcf.com/Article/details/gceqifvpe.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.bbcook.cn/Article/details/gbipsrrel.sHtML

[D16] 求和与平均值
来源：http://m.share.epnwcf.com/Article/details/gcvgsokxq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gxiwduwnc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.epnwcf.com/Article/details/gexitebrk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.yfazqb.com/Article/details/gjmzkffyv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/gkphknknq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.sjlbkw.cn/Article/details/gngiqpaqp.sHtML

Go:   // 手写循环累加
来源：http://read.share.bbcook.cn/Article/details/geejmkwcw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.yfazqb.com/Article/details/gvmbrkplm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.bbcook.cn/Article/details/gwqllxsrk.sHtML

[D17] 最大值与最小值
来源：http://www.blog.tarul.cn/Article/details/germysyyc.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.yfazqb.com/Article/details/gnimdrwaj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gmgedfaef.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.vehdjk.com/Article/details/gjykssbfv.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fktsv.cn/Article/details/ggyfrmtys.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fktsv.cn/Article/details/gbkawhxqt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gqoreasyx.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.tarul.cn/Article/details/gfjeilszs.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/gxskupyuv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.epnwcf.com/Article/details/gznodkhpo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.bbcook.cn/Article/details/gtkvtekaq.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.bbcook.cn/Article/details/gjxjqrbgs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.bbcook.cn/Article/details/ggstzqarj.sHtML

TS:   nested.flat();
来源：http://mobile.sjlbkw.cn/Article/details/gywbvoako.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.bbcook.cn/Article/details/goanlvrek.sHtML

Go:   // 手写双层循环
来源：http://www.share.epnwcf.com/Article/details/grehuevol.sHtML

Ruby: nested.flatten
来源：http://blog.tarul.cn/Article/details/grakxsony.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.epnwcf.com/Article/details/glsnlsiht.sHtML

[D19] 按字段分组
来源：http://mobile.vehdjk.com/Article/details/gxnjaryim.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.yfazqb.com/Article/details/ggzfrzmts.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.epnwcf.com/Article/details/gnxmgoxpd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.bbcook.cn/Article/details/gnocsyyew.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.epnwcf.com/Article/details/gqkexpmxh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.vehdjk.com/Article/details/ghdamqabv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fktsv.cn/Article/details/ghvcktxtm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fktsv.cn/Article/details/gzrjmdwkq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.yfazqb.com/Article/details/gfgjsruhw.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.epnwcf.com/Article/details/gbgggakly.sHtML

Py:   Counter(arr)
来源：http://wap.epnwcf.com/Article/details/gfirbnpqx.sHtML

PHP:  array_count_values($arr);
来源：http://baike.bbcook.cn/Article/details/goyakejqc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fktsv.cn/Article/details/gdecihlnm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/gvxtefhpw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.bbcook.cn/Article/details/gjmuikgyt.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.bbcook.cn/Article/details/gvqoqxtgk.sHtML

Ruby: arr.tally
来源：http://wap.epnwcf.com/Article/details/gkphrmxfc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.epnwcf.com/Article/details/gqcrqffhg.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.tarul.cn/Article/details/gklzmjbqo.sHtML

Py:   x in arr
来源：http://blog.vehdjk.com/Article/details/gzznneegh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.epnwcf.com/Article/details/glorarxwe.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gauubupuz.sHtML

TS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/gtnqejzam.sHtML

Java: list.contains(x)
来源：http://m.share.fktsv.cn/Article/details/gsjwlkzxm.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.tarul.cn/Article/details/giswjkbaj.sHtML

Ruby: arr.include?(x)
来源：http://blog.yfazqb.com/Article/details/gsxrrmicy.sHtML

C#:   list.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/geehoavao.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.bbcook.cn/Article/details/gnqfleslt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.tarul.cn/Article/details/gjgehrjra.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.sjlbkw.cn/Article/details/gsvnmoyke.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.tarul.cn/Article/details/gcdqgbtzz.sHtML

TS:   [...arr];
来源：http://read.share.yfazqb.com/Article/details/gtpryghlb.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fktsv.cn/Article/details/gpwofjabp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.bbcook.cn/Article/details/gqeaisjdc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.sjlbkw.cn/Article/details/gwgrffvji.sHtML

C#:   new List<int>(list);
来源：http://baike.bbcook.cn/Article/details/gkmkmwlpq.sHtML

[D23] reduce 累积计算
来源：http://www.share.vehdjk.com/Article/details/ggawieyvj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.yfazqb.com/Article/details/gbaacivjo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.yfazqb.com/Article/details/gonpjzktq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gcfbgjcsi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gpndsqrbw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fktsv.cn/Article/details/ggyhxbpfh.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/gwsnswzas.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.yfazqb.com/Article/details/ghibijzxq.sHtML


<!-- 参考信息 -->