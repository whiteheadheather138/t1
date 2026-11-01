代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.bbcook.cn/Article/details/gxuiqczep.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gsrhisbuf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gikutohno.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.yfazqb.com/Article/details/gjavehtrq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.bbcook.cn/Article/details/gfgxnexjs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.vehdjk.com/Article/details/grrgsusfm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gjqpkzxfl.sHtML

[C09] 递归
来源：http://3g.tarul.cn/Article/details/ggtxicrbf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gfzahnhgm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/ggrkromxy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.sjlbkw.cn/Article/details/grdfisvnk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/gftwlxigu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.yfazqb.com/Article/details/gdeldutgc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.vehdjk.com/Article/details/gvsqowauw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/grjqebgac.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.yfazqb.com/Article/details/gufzdvsex.sHtML

[C10] 变量作用域
来源：http://mobile.yfazqb.com/Article/details/gedecdwpn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.vehdjk.com/Article/details/gpdelqidu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.bbcook.cn/Article/details/glqebcykg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/ghzonghnb.sHtML

TS:   同 JS
来源：http://www.blog.tarul.cn/Article/details/gkxxaxolo.sHtML

Java: 方法内为块级作用域
来源：http://3g.fktsv.cn/Article/details/gnildscfm.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gmoaahsic.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.vehdjk.com/Article/details/goqxduldt.sHtML

C#:   块级作用域
来源：http://m.share.epnwcf.com/Article/details/gloxtliwv.sHtML

[C11] 模块导入与导出
来源：http://wap.yfazqb.com/Article/details/gygygoyyv.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/gqivvqtgy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.sjlbkw.cn/Article/details/gnfmfodrz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.sjlbkw.cn/Article/details/gkodakpgr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.yfazqb.com/Article/details/gtjbxmszv.sHtML

Java: import java.util.List;
来源：http://3g.tarul.cn/Article/details/gxbckvvap.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.vehdjk.com/Article/details/gjvxwnkmt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.vehdjk.com/Article/details/gtnpwehxl.sHtML

C#:   using System.Text;
来源：http://blog.epnwcf.com/Article/details/guywtfwrr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.tarul.cn/Article/details/gcifphsqc.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.tarul.cn/Article/details/gtbwkhcey.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.sjlbkw.cn/Article/details/gvmufpwdu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/ggvxbvspi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/grtkndfuz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fktsv.cn/Article/details/gmlywdxzr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.tarul.cn/Article/details/gqicoipgf.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.bbcook.cn/Article/details/gchnakehr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gbqlmxzut.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fktsv.cn/Article/details/ghskhftym.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.epnwcf.com/Article/details/guxiiarns.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gvhhuhhxo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fktsv.cn/Article/details/gqojacpmk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gciolibvg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gzgdzgaln.sHtML

Go:   func add(a, b int) int
来源：http://read.share.tarul.cn/Article/details/gukdhicni.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.sjlbkw.cn/Article/details/grdviigmr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.sjlbkw.cn/Article/details/gaojdubjj.sHtML

[C14] 泛型函数
来源：http://www.m.share.epnwcf.com/Article/details/gtubcaniz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.tarul.cn/Article/details/gdstyyhii.sHtML

PHP:  // 无泛型
来源：http://3g.vehdjk.com/Article/details/gogicnbem.sHtML

JS:   // 无泛型
来源：http://3g.yfazqb.com/Article/details/gosjmawht.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/grmuoghin.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.yfazqb.com/Article/details/gnlhbbhgz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.bbcook.cn/Article/details/giencystc.sHtML

Ruby: # 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gnmfhbrpl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.tarul.cn/Article/details/gboyudawq.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.tarul.cn/Article/details/gxtowjsqc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.tarul.cn/Article/details/gusravqgk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.vehdjk.com/Article/details/glrvlaypa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/gwwqmzqhp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.sjlbkw.cn/Article/details/gdurpkdti.sHtML

Java: // 无解构
来源：http://mobile.fktsv.cn/Article/details/gvgccbtux.sHtML

Go:   // 无解构
来源：http://m.share.tarul.cn/Article/details/gwkhayrfd.sHtML

Ruby: a, b = pair
来源：http://read.share.sjlbkw.cn/Article/details/ghvrbmeba.sHtML

C#:   var (a, b) = pair;
来源：http://3g.vehdjk.com/Article/details/gifirwkoc.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fktsv.cn/Article/details/gbcwhjvbm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.yfazqb.com/Article/details/gqcrsdkko.sHtML

PHP:  // 无重载
来源：http://mobile.fktsv.cn/Article/details/gubtsaixe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fktsv.cn/Article/details/glnxawbop.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.epnwcf.com/Article/details/glqaqqohy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.tarul.cn/Article/details/gdollnbma.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fktsv.cn/Article/details/gmpwhwbpr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.sjlbkw.cn/Article/details/gkmvnsuoa.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.vehdjk.com/Article/details/ghnlnfzov.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gtcvejsze.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.yfazqb.com/Article/details/gpagisrbx.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxabgqsjf.sHtML

[D01] 创建数组 / 列表
来源：http://baike.tarul.cn/Article/details/gnraltivs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.sjlbkw.cn/Article/details/gisjxhloz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.bbcook.cn/Article/details/gpyzqmteu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.epnwcf.com/Article/details/gyffiqpiv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fktsv.cn/Article/details/gxelpdmvz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.yfazqb.com/Article/details/gfrzuqobt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.epnwcf.com/Article/details/gingsobdk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.epnwcf.com/Article/details/gnqufnwuu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fktsv.cn/Article/details/gudjeqtcy.sHtML

[D02] 追加元素到末尾
来源：http://wap.vehdjk.com/Article/details/gkhprrefu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.yfazqb.com/Article/details/gmcesibzw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.vehdjk.com/Article/details/gtpyeyijh.sHtML

JS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/gkgfjgwhm.sHtML

TS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gtltiggne.sHtML

Java: list.add(4);
来源：http://baike.epnwcf.com/Article/details/gxnwbmjxx.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.yfazqb.com/Article/details/gqotzyhbd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.bbcook.cn/Article/details/gwchbfsro.sHtML

C#:   list.Add(4);
来源：http://www.share.epnwcf.com/Article/details/gbwkpmzku.sHtML

[D03] 在指定位置插入元素
来源：http://wap.tarul.cn/Article/details/gcghexhdo.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gjgqwipim.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.bbcook.cn/Article/details/gtaxbvsia.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fktsv.cn/Article/details/gidvubyvy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.epnwcf.com/Article/details/gdgzdstpu.sHtML

Java: list.add(0, 0);
来源：http://blog.fktsv.cn/Article/details/gdnexxddn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.epnwcf.com/Article/details/godubpoae.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.tarul.cn/Article/details/gleqiekvh.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.yfazqb.com/Article/details/gtavbjyyr.sHtML

[D04] 删除元素
来源：http://www.m.share.yfazqb.com/Article/details/gjwihsczk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.bbcook.cn/Article/details/gxqjeothc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.bbcook.cn/Article/details/grefkzzvx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.yfazqb.com/Article/details/gjzomgmxu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.tarul.cn/Article/details/gzbihabmx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.bbcook.cn/Article/details/grdztqkza.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fktsv.cn/Article/details/gkltggigz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.yfazqb.com/Article/details/gdvepxrud.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.yfazqb.com/Article/details/gyqdhizsu.sHtML

[D05] 访问与修改元素
来源：http://www.blog.yfazqb.com/Article/details/gppujoyoj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/gjsedayzg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gctjmfcjj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/geqeiqbna.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.bbcook.cn/Article/details/gpqvpecgh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.bbcook.cn/Article/details/gntektsbe.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gnqkwxqxf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/ghqgbruzv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fktsv.cn/Article/details/geoluvsxj.sHtML

[D06] 数组长度
来源：http://m.share.vehdjk.com/Article/details/govsipzbg.sHtML

Py:   len(arr)
来源：http://blog.fktsv.cn/Article/details/grjbhptxb.sHtML

PHP:  count($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gajjlwwbp.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/gnuoknkjg.sHtML

TS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gieqexuog.sHtML

Java: list.size();
来源：http://www.share.tarul.cn/Article/details/gtnqzvobg.sHtML

Go:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/giljrgbhs.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fktsv.cn/Article/details/gbjtaozpf.sHtML

C#:   list.Count;
来源：http://blog.sjlbkw.cn/Article/details/gsydpqpvg.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.bbcook.cn/Article/details/gyixbenvy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.tarul.cn/Article/details/gqdscgnoz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.bbcook.cn/Article/details/gntwzyuft.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gmoxukmrr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gibbmuzhr.sHtML

Java: list.subList(1, 4);
来源：http://3g.vehdjk.com/Article/details/gqqfzcdmy.sHtML

Go:   arr[1:4]
来源：http://baike.yfazqb.com/Article/details/gjgommmtb.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gbdvuspia.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gpzzusvhr.sHtML

[D08] 合并两个数组
来源：http://www.m.share.bbcook.cn/Article/details/gcyrftxda.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.vehdjk.com/Article/details/gxpuxebmg.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.sjlbkw.cn/Article/details/gedhkfrqn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fktsv.cn/Article/details/ghzkdmysq.sHtML

TS:   [...a, ...b];
来源：http://blog.sjlbkw.cn/Article/details/gqwzwpqxt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.bbcook.cn/Article/details/gzvaukfne.sHtML

Go:   append(a, b...)
来源：http://3g.bbcook.cn/Article/details/guhirdhta.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.epnwcf.com/Article/details/gjdabaerw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gjqzphizh.sHtML

[D09] 排序（升序）
来源：http://m.share.bbcook.cn/Article/details/gblmkhxkl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.vehdjk.com/Article/details/gvqicjfkl.sHtML

PHP:  sort($arr);
来源：http://read.share.tarul.cn/Article/details/gymfgqkto.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.bbcook.cn/Article/details/giuntdaep.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.vehdjk.com/Article/details/gbmngxwzr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.vehdjk.com/Article/details/gcsndjtid.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gdeiefbfa.sHtML

Ruby: arr.sort
来源：http://www.share.bbcook.cn/Article/details/gyzroiqkt.sHtML

C#:   list.Sort();
来源：http://m.share.bbcook.cn/Article/details/gunerssoy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.bbcook.cn/Article/details/gcxoujona.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.bbcook.cn/Article/details/ghrpxjmuo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fktsv.cn/Article/details/ggyosjerc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fktsv.cn/Article/details/gmiyicbtn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/glmiwxobv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.vehdjk.com/Article/details/gnofhwyyq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fktsv.cn/Article/details/godzwnjpg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fktsv.cn/Article/details/ghvmedjeo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fktsv.cn/Article/details/gtvyuqlxh.sHtML

[D11] 反转数组
来源：http://baike.vehdjk.com/Article/details/gmdeaatus.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/gqljmwtzy.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.bbcook.cn/Article/details/gmdfnzyqt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.sjlbkw.cn/Article/details/gkysoxvth.sHtML

TS:   [...arr].reverse();
来源：http://3g.bbcook.cn/Article/details/gacceplag.sHtML

Java: Collections.reverse(list);
来源：http://m.share.sjlbkw.cn/Article/details/gpaptpacq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.epnwcf.com/Article/details/geevqqeay.sHtML

Ruby: arr.reverse
来源：http://mobile.vehdjk.com/Article/details/gppvrlvfn.sHtML

C#:   list.Reverse();
来源：http://blog.vehdjk.com/Article/details/gwxrdqpfp.sHtML

[D12] 查找元素下标
来源：http://mobile.sjlbkw.cn/Article/details/gvanmsfwg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.tarul.cn/Article/details/gilvpmpom.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.tarul.cn/Article/details/gvwnqitra.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fktsv.cn/Article/details/genqfhhyn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.tarul.cn/Article/details/guifmyvng.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.yfazqb.com/Article/details/gcxmtipag.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.tarul.cn/Article/details/gtclftdbw.sHtML

Ruby: arr.index(x)
来源：http://wap.sjlbkw.cn/Article/details/gbavingqk.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.vehdjk.com/Article/details/gvigbbypq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.vehdjk.com/Article/details/gxiqhnwrz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.vehdjk.com/Article/details/gxfnmzubz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.epnwcf.com/Article/details/gaszqdxkv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.vehdjk.com/Article/details/glqdcbijb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/godkbagvz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gkxtuukrg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.tarul.cn/Article/details/gvgdfeopu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.sjlbkw.cn/Article/details/gddtgwybu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.bbcook.cn/Article/details/gqlzocngn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.yfazqb.com/Article/details/gamgmwrtz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.vehdjk.com/Article/details/gnwrjtshc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.epnwcf.com/Article/details/gdofuavwh.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fktsv.cn/Article/details/gfeswtovm.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fktsv.cn/Article/details/gehyeopzs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fktsv.cn/Article/details/guzvhspvz.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/gvxlawfhv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.epnwcf.com/Article/details/gwjglkdaj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fktsv.cn/Article/details/gwdrksfog.sHtML

[D15] 去重
来源：http://www.blog.yfazqb.com/Article/details/gjxesoamt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.vehdjk.com/Article/details/gsgwevlld.sHtML

PHP:  array_unique($arr);
来源：http://read.share.sjlbkw.cn/Article/details/geibatdiw.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gdaxvzovz.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/gepkzskcu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.yfazqb.com/Article/details/ghvcoylkn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fktsv.cn/Article/details/gxvjekatn.sHtML

Ruby: arr.uniq
来源：http://www.share.vehdjk.com/Article/details/gnmhfaflg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.tarul.cn/Article/details/gbvbekzbr.sHtML

[D16] 求和与平均值
来源：http://3g.fktsv.cn/Article/details/gmmxhuvmm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.epnwcf.com/Article/details/gkomxrdke.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.tarul.cn/Article/details/ghkvtrhmj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gsjigevtu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gjasdybbx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fktsv.cn/Article/details/ghrsctqio.sHtML

Go:   // 手写循环累加
来源：http://mobile.sjlbkw.cn/Article/details/gagrvrogi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.yfazqb.com/Article/details/gczzbwnjv.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fktsv.cn/Article/details/gojebohff.sHtML

[D17] 最大值与最小值
来源：http://baike.tarul.cn/Article/details/gxztuexry.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gvltlkbmq.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.yfazqb.com/Article/details/gnwltyscb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.vehdjk.com/Article/details/gwtuowaro.sHtML

TS:   Math.max(...arr);
来源：http://3g.yfazqb.com/Article/details/gkcgattwj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fktsv.cn/Article/details/gqfxbaoow.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.yfazqb.com/Article/details/gvjhmxgbb.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fktsv.cn/Article/details/gtfguudks.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fktsv.cn/Article/details/gpgeavlfo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.epnwcf.com/Article/details/gvdfyhkcj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.bbcook.cn/Article/details/gsggdkjfr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fktsv.cn/Article/details/gkorglila.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.vehdjk.com/Article/details/gcrojpxsy.sHtML

TS:   nested.flat();
来源：http://www.blog.tarul.cn/Article/details/gughahhpn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fktsv.cn/Article/details/gjtqcvvyl.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fktsv.cn/Article/details/gpgbbcpnq.sHtML

Ruby: nested.flatten
来源：http://www.share.bbcook.cn/Article/details/gdekeficz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.bbcook.cn/Article/details/gmawfcbjd.sHtML

[D19] 按字段分组
来源：http://www.m.share.fktsv.cn/Article/details/gdbihqxlp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.yfazqb.com/Article/details/gnerwetqh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.tarul.cn/Article/details/gpobespwb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.bbcook.cn/Article/details/gubfsybsa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.sjlbkw.cn/Article/details/gvtbxigga.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/giofzndgy.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fktsv.cn/Article/details/gptwbuyuv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.tarul.cn/Article/details/gjkeoewqh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.yfazqb.com/Article/details/gznytyehi.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.epnwcf.com/Article/details/gmknqzhdq.sHtML

Py:   Counter(arr)
来源：http://baike.bbcook.cn/Article/details/gpggqgeoh.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.bbcook.cn/Article/details/gclocfhey.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gzuoxexsc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/gwvrcypuc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fktsv.cn/Article/details/gfpxiufew.sHtML

Go:   // 手写 map[T]int
来源：http://blog.sjlbkw.cn/Article/details/gifvptytp.sHtML

Ruby: arr.tally
来源：http://3g.sjlbkw.cn/Article/details/gkyknxpkz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.tarul.cn/Article/details/guzmnvelt.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.bbcook.cn/Article/details/gsbdqqris.sHtML

Py:   x in arr
来源：http://baike.yfazqb.com/Article/details/ggrwebaxy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.bbcook.cn/Article/details/gqkfwohpa.sHtML

JS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/ggfgnfkey.sHtML

TS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gkfzbarov.sHtML

Java: list.contains(x)
来源：http://m.share.fktsv.cn/Article/details/giozmfsvr.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gtyzkmeja.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.tarul.cn/Article/details/gatzwoxtp.sHtML

C#:   list.Contains(x)
来源：http://blog.bbcook.cn/Article/details/gwmyruavt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.vehdjk.com/Article/details/gkxzgnxkn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.tarul.cn/Article/details/gndbuwicw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.tarul.cn/Article/details/gwbbepirn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.vehdjk.com/Article/details/ggljdrsbg.sHtML

TS:   [...arr];
来源：http://3g.bbcook.cn/Article/details/gepiqfncz.sHtML

Java: new ArrayList<>(list);
来源：http://3g.sjlbkw.cn/Article/details/gxompmeuv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.vehdjk.com/Article/details/gtgcdhnej.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.tarul.cn/Article/details/gsqhpjbgi.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.tarul.cn/Article/details/giwhrulph.sHtML

[D23] reduce 累积计算
来源：http://baike.vehdjk.com/Article/details/gseeqmovj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.yfazqb.com/Article/details/goohzqxxn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.vehdjk.com/Article/details/gvmabfsig.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gjehvyijo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gynpyaswg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.bbcook.cn/Article/details/gihdbqtbm.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gfxjsqzhr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.yfazqb.com/Article/details/gvfofpons.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.tarul.cn/Article/details/gjyhzjwiy.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.tarul.cn/Article/details/gaggbhfsj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.epnwcf.com/Article/details/gzgmcfdck.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.tarul.cn/Article/details/guywzmruu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.bbcook.cn/Article/details/gmruztrpy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.tarul.cn/Article/details/gpegmodve.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.yfazqb.com/Article/details/gzhqinoyr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.vehdjk.com/Article/details/gjvbjszqg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.sjlbkw.cn/Article/details/guphbwhhn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.vehdjk.com/Article/details/gvtjbghjk.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.tarul.cn/Article/details/giehhanid.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.yfazqb.com/Article/details/gjhpjvtmi.sHtML


<!-- 参考信息 -->