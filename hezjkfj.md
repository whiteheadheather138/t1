代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.yfazqb.com/Article/details/gsfjogdqp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/ggvescydv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gafcqofir.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.vehdjk.com/Article/details/gmzidmtbo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.tarul.cn/Article/details/gxockzukh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.tarul.cn/Article/details/gmwaeqpfk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gokhrxuyu.sHtML

[C09] 递归
来源：http://blog.sjlbkw.cn/Article/details/gkdqxuzkd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.bbcook.cn/Article/details/gwaqphtpd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/ghffbhreq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.yfazqb.com/Article/details/gaivntkdt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.tarul.cn/Article/details/gjoccdiud.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gnzkpgmee.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.sjlbkw.cn/Article/details/gadadohbe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/gubbhrfcp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.bbcook.cn/Article/details/gefcrbbnx.sHtML

[C10] 变量作用域
来源：http://blog.bbcook.cn/Article/details/gupcnopwt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fktsv.cn/Article/details/gvlpppeqj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.vehdjk.com/Article/details/gwuoidebp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.vehdjk.com/Article/details/gttkthqxi.sHtML

TS:   同 JS
来源：http://m.share.fktsv.cn/Article/details/gpybfwrez.sHtML

Java: 方法内为块级作用域
来源：http://read.share.vehdjk.com/Article/details/goawltrxs.sHtML

Go:   花括号块级作用域
来源：http://www.blog.vehdjk.com/Article/details/ghpvfjdqn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.tarul.cn/Article/details/gwprvdars.sHtML

C#:   块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gcahqxxgi.sHtML

[C11] 模块导入与导出
来源：http://wap.sjlbkw.cn/Article/details/getbbethq.sHtML

Py:   from module import func
来源：http://baike.fktsv.cn/Article/details/gbavyafya.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.epnwcf.com/Article/details/gmkhktcmf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/gdcrdrxef.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fktsv.cn/Article/details/gsbrfhjpc.sHtML

Java: import java.util.List;
来源：http://read.share.tarul.cn/Article/details/gmwmzgatf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.epnwcf.com/Article/details/gsiazxanq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.epnwcf.com/Article/details/gtmojknfw.sHtML

C#:   using System.Text;
来源：http://www.share.yfazqb.com/Article/details/ghnuulwlu.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.bbcook.cn/Article/details/gvrvtlwld.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fktsv.cn/Article/details/gnchnneoe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.bbcook.cn/Article/details/giqglmeil.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.epnwcf.com/Article/details/gttvtkdcq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fktsv.cn/Article/details/gzrywgmtj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.epnwcf.com/Article/details/gwvuvhgjv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.vehdjk.com/Article/details/gwfjrdpuh.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.sjlbkw.cn/Article/details/gziyyuohv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/ggqjsybbe.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.epnwcf.com/Article/details/gtdkbxwpy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fktsv.cn/Article/details/gcydktptq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gxxphueck.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.yfazqb.com/Article/details/ggnzdgwdo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gmvkegtsv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gzonhvdkq.sHtML

Go:   func add(a, b int) int
来源：http://blog.fktsv.cn/Article/details/grsoakfkx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.yfazqb.com/Article/details/gytrnuefk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.epnwcf.com/Article/details/gngblxwui.sHtML

[C14] 泛型函数
来源：http://www.share.vehdjk.com/Article/details/grsjjskrt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.tarul.cn/Article/details/gxzfstbhn.sHtML

PHP:  // 无泛型
来源：http://m.share.yfazqb.com/Article/details/gbxpdmofu.sHtML

JS:   // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gehnaqlib.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.bbcook.cn/Article/details/gnaynszxj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.yfazqb.com/Article/details/gfpzryfwx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.epnwcf.com/Article/details/grzehexko.sHtML

Ruby: # 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gmhcsghha.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.bbcook.cn/Article/details/gyhgowdlx.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.sjlbkw.cn/Article/details/gstbgtfcz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.bbcook.cn/Article/details/gglbkognx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fktsv.cn/Article/details/gtuvvuvdx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.epnwcf.com/Article/details/geayisgrt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gxwbnyiej.sHtML

Java: // 无解构
来源：http://m.share.yfazqb.com/Article/details/gcwmhkhup.sHtML

Go:   // 无解构
来源：http://blog.fktsv.cn/Article/details/garezbzwb.sHtML

Ruby: a, b = pair
来源：http://mobile.yfazqb.com/Article/details/gbuijgzcq.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.epnwcf.com/Article/details/gcafczhpl.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fktsv.cn/Article/details/gcmskydeh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.tarul.cn/Article/details/gqulraeln.sHtML

PHP:  // 无重载
来源：http://3g.epnwcf.com/Article/details/gxegiccjd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.yfazqb.com/Article/details/gypcbdyep.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.tarul.cn/Article/details/gxkwveqbr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.bbcook.cn/Article/details/gyvqovmjb.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fktsv.cn/Article/details/gedrejfzw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.epnwcf.com/Article/details/gaisunnle.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.epnwcf.com/Article/details/gzcikctxq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gzhrmrpbg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.sjlbkw.cn/Article/details/gmflhhdmk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gfzbvxcvs.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.epnwcf.com/Article/details/gmmpicuwq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.bbcook.cn/Article/details/gteqihhru.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.sjlbkw.cn/Article/details/gpxrqjaia.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/gbyvfvrxl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.vehdjk.com/Article/details/ggnglosgi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.yfazqb.com/Article/details/gozscmmag.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/grqezntwm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fktsv.cn/Article/details/gmkyjupsv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.epnwcf.com/Article/details/gtzsstncd.sHtML

[D02] 追加元素到末尾
来源：http://www.share.sjlbkw.cn/Article/details/gljalygai.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.tarul.cn/Article/details/gsneedmjq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fktsv.cn/Article/details/gqqfkcbsx.sHtML

JS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/gpzduwwws.sHtML

TS:   arr.push(4);
来源：http://baike.bbcook.cn/Article/details/gexqfxcud.sHtML

Java: list.add(4);
来源：http://read.share.vehdjk.com/Article/details/gvlgvalap.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fktsv.cn/Article/details/gjdlldosy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.vehdjk.com/Article/details/guipwzylc.sHtML

C#:   list.Add(4);
来源：http://read.share.tarul.cn/Article/details/gtkcagdjh.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.sjlbkw.cn/Article/details/gsujcvfnj.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.tarul.cn/Article/details/grrbaluyi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.bbcook.cn/Article/details/ghzgjjvxx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.bbcook.cn/Article/details/gnfwimpod.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.bbcook.cn/Article/details/gjautzizw.sHtML

Java: list.add(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gejuenodk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.bbcook.cn/Article/details/ggjgzbvct.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.bbcook.cn/Article/details/gtxmuljgd.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.vehdjk.com/Article/details/gihhekyhd.sHtML

[D04] 删除元素
来源：http://blog.bbcook.cn/Article/details/grsxlqpvp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.sjlbkw.cn/Article/details/gprczhsgo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.tarul.cn/Article/details/goxztbnvq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.bbcook.cn/Article/details/gguxounfs.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.sjlbkw.cn/Article/details/gzwlqmjmh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.sjlbkw.cn/Article/details/ggrqezyps.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.tarul.cn/Article/details/ggephtwwt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.tarul.cn/Article/details/gltwjewxi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.vehdjk.com/Article/details/gndqcmwfu.sHtML

[D05] 访问与修改元素
来源：http://3g.sjlbkw.cn/Article/details/gmgsrswcz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/gppqwgfdi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gulkhicye.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gtvfmdfwf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.vehdjk.com/Article/details/gyyscefoa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.yfazqb.com/Article/details/gnwzqvtbo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gwwfbvrmc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/ghdljtmgg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gglpkypoi.sHtML

[D06] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gstefuxwe.sHtML

Py:   len(arr)
来源：http://m.share.tarul.cn/Article/details/gjgqbpzxa.sHtML

PHP:  count($arr);
来源：http://wap.fktsv.cn/Article/details/gygsxkvpm.sHtML

JS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/glsmkqdij.sHtML

TS:   arr.length
来源：http://www.blog.epnwcf.com/Article/details/ghstjwufj.sHtML

Java: list.size();
来源：http://baike.epnwcf.com/Article/details/ggfvegvii.sHtML

Go:   len(arr)
来源：http://wap.fktsv.cn/Article/details/gcawckjgo.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.tarul.cn/Article/details/gfppggtlx.sHtML

C#:   list.Count;
来源：http://www.m.share.yfazqb.com/Article/details/gyccjybhg.sHtML

[D07] 切片 / 取子数组
来源：http://blog.bbcook.cn/Article/details/gnsjzodiw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.yfazqb.com/Article/details/ghmxmdvwx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.tarul.cn/Article/details/ggjaysjyn.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gzlgmrbwn.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/gytlptbby.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gjojduybn.sHtML

Go:   arr[1:4]
来源：http://mobile.tarul.cn/Article/details/ghjuwxntd.sHtML

Ruby: arr[1, 3]
来源：http://blog.yfazqb.com/Article/details/gqtitrair.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fktsv.cn/Article/details/gswdufwxw.sHtML

[D08] 合并两个数组
来源：http://www.m.share.epnwcf.com/Article/details/gkgniwazu.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.vehdjk.com/Article/details/gkdowchve.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fktsv.cn/Article/details/gwetgvycc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.sjlbkw.cn/Article/details/gujuvvjjn.sHtML

TS:   [...a, ...b];
来源：http://m.share.fktsv.cn/Article/details/gzxbonjtq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.bbcook.cn/Article/details/ghptufzxw.sHtML

Go:   append(a, b...)
来源：http://m.share.bbcook.cn/Article/details/ghcffignm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fktsv.cn/Article/details/gnrjmkdnj.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gbmsknbou.sHtML

[D09] 排序（升序）
来源：http://m.share.sjlbkw.cn/Article/details/gnmzjrnhx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/grvrqmlau.sHtML

PHP:  sort($arr);
来源：http://blog.yfazqb.com/Article/details/gdypatyzs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.tarul.cn/Article/details/gandpsype.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.vehdjk.com/Article/details/ghlzndybi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.vehdjk.com/Article/details/ggfhougzy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gxurvlcem.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gjoayluyw.sHtML

C#:   list.Sort();
来源：http://read.share.vehdjk.com/Article/details/gnmolejfq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.epnwcf.com/Article/details/gpcvwqleu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fktsv.cn/Article/details/gdxagxvzp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.bbcook.cn/Article/details/gvcdvcrii.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/gufzxrefx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/gktcetycl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.vehdjk.com/Article/details/gwmbutaid.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fktsv.cn/Article/details/glumtkboj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.tarul.cn/Article/details/gaqamdfyo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.sjlbkw.cn/Article/details/ghsagdohc.sHtML

[D11] 反转数组
来源：http://mobile.vehdjk.com/Article/details/gkjsphdej.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fktsv.cn/Article/details/gzlwhllan.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.epnwcf.com/Article/details/guzehcmoq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fktsv.cn/Article/details/gqtsuxyea.sHtML

TS:   [...arr].reverse();
来源：http://wap.vehdjk.com/Article/details/gxpdzfubm.sHtML

Java: Collections.reverse(list);
来源：http://3g.vehdjk.com/Article/details/gaexlxrkr.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fktsv.cn/Article/details/gzvrrewob.sHtML

Ruby: arr.reverse
来源：http://www.share.vehdjk.com/Article/details/gbmxajavt.sHtML

C#:   list.Reverse();
来源：http://wap.epnwcf.com/Article/details/gsaxjlnql.sHtML

[D12] 查找元素下标
来源：http://mobile.epnwcf.com/Article/details/gkdfxstva.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gzikedzng.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.bbcook.cn/Article/details/gunwvyjre.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/gwmwlbupp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.yfazqb.com/Article/details/gejuljfny.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.bbcook.cn/Article/details/gpvpltttk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gdixmiupd.sHtML

Ruby: arr.index(x)
来源：http://wap.vehdjk.com/Article/details/gssfqfxck.sHtML

C#:   list.IndexOf(x);
来源：http://baike.sjlbkw.cn/Article/details/gpwobmluy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.sjlbkw.cn/Article/details/geqhugfrv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.bbcook.cn/Article/details/gubivbgfd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbiwzvxp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/gzirndjld.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/gffduqplu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.tarul.cn/Article/details/gylgyrnsb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.tarul.cn/Article/details/gricnuepi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.tarul.cn/Article/details/givzifmvu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.vehdjk.com/Article/details/gwmqfsbdy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.epnwcf.com/Article/details/gfvlnvtyy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.epnwcf.com/Article/details/gmykeytzh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.yfazqb.com/Article/details/gnqmdgywq.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.tarul.cn/Article/details/giulqgyfd.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.yfazqb.com/Article/details/goyrpkxnr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.yfazqb.com/Article/details/gaahwuinv.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gzowrlyri.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gxftnvblv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.yfazqb.com/Article/details/gqxkemqsa.sHtML

[D15] 去重
来源：http://read.share.vehdjk.com/Article/details/gszhuacvg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.tarul.cn/Article/details/grijgfsci.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.vehdjk.com/Article/details/gdootpyou.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/gwasiwrxt.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gxxgnxqet.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fktsv.cn/Article/details/gryzekrle.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.sjlbkw.cn/Article/details/gyldpbgty.sHtML

Ruby: arr.uniq
来源：http://blog.yfazqb.com/Article/details/gsekbnthw.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.epnwcf.com/Article/details/gyffjahrw.sHtML

[D16] 求和与平均值
来源：http://blog.yfazqb.com/Article/details/ghetujgbs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.tarul.cn/Article/details/gnupdbabt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.yfazqb.com/Article/details/giplnwnyl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.bbcook.cn/Article/details/gvkhloqtx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gyluyypjf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.sjlbkw.cn/Article/details/grzxckkmk.sHtML

Go:   // 手写循环累加
来源：http://read.share.epnwcf.com/Article/details/gjyvbrdgr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.bbcook.cn/Article/details/gsrrqaqgc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.vehdjk.com/Article/details/gjsalffxd.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.tarul.cn/Article/details/gtisxenaj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.bbcook.cn/Article/details/gtuzoeecq.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fktsv.cn/Article/details/gxdaxlahv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.vehdjk.com/Article/details/gpqdjpwnf.sHtML

TS:   Math.max(...arr);
来源：http://mobile.tarul.cn/Article/details/glkednklc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.epnwcf.com/Article/details/gnhppdjdc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.vehdjk.com/Article/details/gdedqurrd.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fktsv.cn/Article/details/gsdsdhfly.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.bbcook.cn/Article/details/gakcvntkb.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/gwtncvlmi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.vehdjk.com/Article/details/geauqhfms.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.tarul.cn/Article/details/gefvawrxb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.sjlbkw.cn/Article/details/gpuransji.sHtML

TS:   nested.flat();
来源：http://blog.vehdjk.com/Article/details/gjzeuqrcz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.epnwcf.com/Article/details/gtapnirva.sHtML

Go:   // 手写双层循环
来源：http://baike.bbcook.cn/Article/details/gahfrjjof.sHtML

Ruby: nested.flatten
来源：http://3g.yfazqb.com/Article/details/gluzqvssl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fktsv.cn/Article/details/gshdodplv.sHtML

[D19] 按字段分组
来源：http://wap.sjlbkw.cn/Article/details/gtmjsxuvy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.epnwcf.com/Article/details/gxzipqrkr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.epnwcf.com/Article/details/gkzibtyqg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.vehdjk.com/Article/details/gcudphiir.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.epnwcf.com/Article/details/gmdtzorkm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/gsjysbdip.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.epnwcf.com/Article/details/ggtnhdfxz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.epnwcf.com/Article/details/gqhjaokwa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.tarul.cn/Article/details/gbhiitwpc.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.epnwcf.com/Article/details/gnyewfhli.sHtML

Py:   Counter(arr)
来源：http://baike.sjlbkw.cn/Article/details/gkgitkwvm.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fktsv.cn/Article/details/gowdhidbq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.epnwcf.com/Article/details/geptfrdsz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/gdvqkzven.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.vehdjk.com/Article/details/gzkfqwyyb.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.bbcook.cn/Article/details/grzwzunxk.sHtML

Ruby: arr.tally
来源：http://3g.bbcook.cn/Article/details/gshfnotwh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.tarul.cn/Article/details/gwtsyyqzv.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.tarul.cn/Article/details/gjzpsxijq.sHtML

Py:   x in arr
来源：http://read.share.fktsv.cn/Article/details/gcjossmay.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.epnwcf.com/Article/details/gecujpfon.sHtML

JS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/ghqfgxewl.sHtML

TS:   arr.includes(x)
来源：http://blog.yfazqb.com/Article/details/gurdymusw.sHtML

Java: list.contains(x)
来源：http://read.share.tarul.cn/Article/details/gfreqzial.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gturjhmhf.sHtML

Ruby: arr.include?(x)
来源：http://mobile.yfazqb.com/Article/details/ggmztncto.sHtML

C#:   list.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gmiiyoczh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.bbcook.cn/Article/details/ghzsaawko.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fktsv.cn/Article/details/gcgqdhgzk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fktsv.cn/Article/details/gkkommymw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fktsv.cn/Article/details/gmuvxikiw.sHtML

TS:   [...arr];
来源：http://mobile.sjlbkw.cn/Article/details/gxklfzbaw.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fktsv.cn/Article/details/gnohemleh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fktsv.cn/Article/details/gbgwctqht.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.epnwcf.com/Article/details/giclcnzxg.sHtML

C#:   new List<int>(list);
来源：http://www.share.vehdjk.com/Article/details/gqxuuxtyc.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.yfazqb.com/Article/details/gzwzvnfqe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.vehdjk.com/Article/details/gfsrpaxgf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gizkeijnm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/gxfilukfd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/gavktnwgc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.sjlbkw.cn/Article/details/gdnyiglav.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gwgokxtjn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.yfazqb.com/Article/details/ggrponwzd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.vehdjk.com/Article/details/gylbwowui.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.bbcook.cn/Article/details/gohdhiqbn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fktsv.cn/Article/details/gdgczvqkg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.epnwcf.com/Article/details/gbdprwvje.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.epnwcf.com/Article/details/geqtsxeao.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.tarul.cn/Article/details/gsxecwvsv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.epnwcf.com/Article/details/gxmvztkwo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.sjlbkw.cn/Article/details/gqmsikhib.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.bbcook.cn/Article/details/goxspbiox.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fktsv.cn/Article/details/gjkkitdnn.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.sjlbkw.cn/Article/details/gcnorjyxj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.bbcook.cn/Article/details/gyhiwdtxw.sHtML


<!-- 参考信息 -->