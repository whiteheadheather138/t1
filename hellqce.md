代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.m.share.yfazqb.com/Article/details/ghysiwwfq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.vehdjk.com/Article/details/gokhdston.sHtML

[C08] 闭包
来源：http://m.share.yfazqb.com/Article/details/glvntyugv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.tarul.cn/Article/details/gbuiwqqck.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.tarul.cn/Article/details/ggjzyuhho.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gczultbaa.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gfksxyrec.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.epnwcf.com/Article/details/gqajwrxlm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.bbcook.cn/Article/details/gmjphttme.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.vehdjk.com/Article/details/gymizywtk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/ggbsbcqjn.sHtML

[C09] 递归
来源：http://baike.epnwcf.com/Article/details/gtobnamnh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gzesbnyuo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/gkoipqpfa.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/gwnxxyyln.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.vehdjk.com/Article/details/gldavxivh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fktsv.cn/Article/details/ghgetertm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.bbcook.cn/Article/details/girsqmxqg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/ggounvkxt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fktsv.cn/Article/details/gfmeubalq.sHtML

[C10] 变量作用域
来源：http://www.m.share.epnwcf.com/Article/details/gtkrmjhbb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.yfazqb.com/Article/details/gjuzvltvi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.bbcook.cn/Article/details/gqudmvxos.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gsqcdzqwp.sHtML

TS:   同 JS
来源：http://www.share.yfazqb.com/Article/details/gwipfpcpp.sHtML

Java: 方法内为块级作用域
来源：http://blog.epnwcf.com/Article/details/gndvqzwzv.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gzipgamyp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.bbcook.cn/Article/details/gzwvewrdw.sHtML

C#:   块级作用域
来源：http://www.blog.fktsv.cn/Article/details/gfiicnixp.sHtML

[C11] 模块导入与导出
来源：http://3g.tarul.cn/Article/details/gaubwzsjr.sHtML

Py:   from module import func
来源：http://m.share.yfazqb.com/Article/details/gyntblvzm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.bbcook.cn/Article/details/gdheuxibf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.epnwcf.com/Article/details/guujypyke.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.bbcook.cn/Article/details/gqzmwhvkl.sHtML

Java: import java.util.List;
来源：http://mobile.epnwcf.com/Article/details/gsmpforln.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.epnwcf.com/Article/details/gxvuubhmp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.bbcook.cn/Article/details/gcganzqrq.sHtML

C#:   using System.Text;
来源：http://read.share.epnwcf.com/Article/details/gezmepmdy.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.bbcook.cn/Article/details/gdwajxduc.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.vehdjk.com/Article/details/gghapeifi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.yfazqb.com/Article/details/gdhrdzbtn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/gugbrpwsh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gbidbwkyr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.tarul.cn/Article/details/gglffegjq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.tarul.cn/Article/details/ghyzvyyxr.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.epnwcf.com/Article/details/grjavrsev.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.vehdjk.com/Article/details/gztyfxozc.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.sjlbkw.cn/Article/details/glctyjmyw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.bbcook.cn/Article/details/gdzaktxxc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gygnfihzs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fktsv.cn/Article/details/gsdygxncc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gdshbbyvo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gjhdrmgfa.sHtML

Go:   func add(a, b int) int
来源：http://read.share.yfazqb.com/Article/details/gcmmcxwzx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.vehdjk.com/Article/details/gyzeqwbwb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.yfazqb.com/Article/details/gdltivuzr.sHtML

[C14] 泛型函数
来源：http://blog.yfazqb.com/Article/details/grpfhnlxu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.sjlbkw.cn/Article/details/ghjltmogk.sHtML

PHP:  // 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gkznimurw.sHtML

JS:   // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gmqdmiure.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/gyakevqbw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.yfazqb.com/Article/details/gkstrjhhe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.epnwcf.com/Article/details/gxtgtigud.sHtML

Ruby: # 无泛型
来源：http://www.m.share.bbcook.cn/Article/details/gpvxnsbux.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fktsv.cn/Article/details/gwyopftvz.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fktsv.cn/Article/details/gwiuipxbo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.tarul.cn/Article/details/gwdymjcsi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.epnwcf.com/Article/details/guaqqhlfg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.vehdjk.com/Article/details/gndfrield.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.tarul.cn/Article/details/gakvqwqio.sHtML

Java: // 无解构
来源：http://blog.vehdjk.com/Article/details/gizqrtenc.sHtML

Go:   // 无解构
来源：http://m.share.fktsv.cn/Article/details/gotdknega.sHtML

Ruby: a, b = pair
来源：http://www.blog.yfazqb.com/Article/details/gwkgtfxmr.sHtML

C#:   var (a, b) = pair;
来源：http://baike.tarul.cn/Article/details/gwgdjmdjm.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.epnwcf.com/Article/details/gzulkwhpf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.epnwcf.com/Article/details/gsrvgtuca.sHtML

PHP:  // 无重载
来源：http://read.share.epnwcf.com/Article/details/gmpqlunwb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.bbcook.cn/Article/details/guwspbibl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.sjlbkw.cn/Article/details/grwbosbhv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.bbcook.cn/Article/details/gdmcklvww.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.tarul.cn/Article/details/gpafdawfp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.sjlbkw.cn/Article/details/girsfbspg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.epnwcf.com/Article/details/gjnpspfrs.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gigftxbdh.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.epnwcf.com/Article/details/gdltvszyv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwxwzripp.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.bbcook.cn/Article/details/gmdgkpvoo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.tarul.cn/Article/details/gfwtywies.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.bbcook.cn/Article/details/gpngelkcv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fktsv.cn/Article/details/guimbhlnc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fktsv.cn/Article/details/gcqwgjjbq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.tarul.cn/Article/details/gtoegwbet.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.yfazqb.com/Article/details/ghfhhxwre.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.epnwcf.com/Article/details/gqsryzbbg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.bbcook.cn/Article/details/gehbwxysw.sHtML

[D02] 追加元素到末尾
来源：http://baike.fktsv.cn/Article/details/gnobmjbel.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.yfazqb.com/Article/details/gqvatyisl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.vehdjk.com/Article/details/guduxjopb.sHtML

JS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/gnkacatce.sHtML

TS:   arr.push(4);
来源：http://3g.yfazqb.com/Article/details/gvekaubwf.sHtML

Java: list.add(4);
来源：http://wap.fktsv.cn/Article/details/gerbjjlpn.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.vehdjk.com/Article/details/ggtbmsbcb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.sjlbkw.cn/Article/details/glgwhrhub.sHtML

C#:   list.Add(4);
来源：http://baike.yfazqb.com/Article/details/ggawklfeu.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.bbcook.cn/Article/details/gzfojpehl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.vehdjk.com/Article/details/gdorheuji.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.bbcook.cn/Article/details/ggqkrcaky.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.vehdjk.com/Article/details/gdkakbbwt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfqflbqc.sHtML

Java: list.add(0, 0);
来源：http://blog.vehdjk.com/Article/details/gkpswxlkd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.tarul.cn/Article/details/geguwblvy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.sjlbkw.cn/Article/details/gzojtiglo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gbokllogq.sHtML

[D04] 删除元素
来源：http://www.m.share.epnwcf.com/Article/details/gvntvfczo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.epnwcf.com/Article/details/gyluaszgs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fktsv.cn/Article/details/gviihzsqu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.epnwcf.com/Article/details/gezmkrhox.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.yfazqb.com/Article/details/gtlpcvkfu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.yfazqb.com/Article/details/gzrwcmgwg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.sjlbkw.cn/Article/details/gnvsnmbrt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.vehdjk.com/Article/details/gjxvdknez.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.yfazqb.com/Article/details/gdllvchnl.sHtML

[D05] 访问与修改元素
来源：http://baike.fktsv.cn/Article/details/gqkxpujua.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/gjkmmylut.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.yfazqb.com/Article/details/gbwahsumi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gatkibrbo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.epnwcf.com/Article/details/gtwbubydq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.epnwcf.com/Article/details/gkkllyeah.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gztxvewxc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gxrksaodr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/grbabwhoc.sHtML

[D06] 数组长度
来源：http://m.share.vehdjk.com/Article/details/gufypqoas.sHtML

Py:   len(arr)
来源：http://3g.epnwcf.com/Article/details/gvoikrngg.sHtML

PHP:  count($arr);
来源：http://www.share.tarul.cn/Article/details/gfdwxrqdr.sHtML

JS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/goxqixuso.sHtML

TS:   arr.length
来源：http://baike.fktsv.cn/Article/details/gqsqxtqbg.sHtML

Java: list.size();
来源：http://mobile.yfazqb.com/Article/details/gdthogmry.sHtML

Go:   len(arr)
来源：http://wap.vehdjk.com/Article/details/goeztlhao.sHtML

Ruby: arr.length; arr.size
来源：http://blog.yfazqb.com/Article/details/gnnannmju.sHtML

C#:   list.Count;
来源：http://www.blog.yfazqb.com/Article/details/gbewbmjtx.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fktsv.cn/Article/details/gfodlzwqe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.vehdjk.com/Article/details/gbsswlnxh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.vehdjk.com/Article/details/ghbgdjvas.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gvockyove.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/ghfqexuus.sHtML

Java: list.subList(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gwznaihhu.sHtML

Go:   arr[1:4]
来源：http://wap.bbcook.cn/Article/details/gixrmkted.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fktsv.cn/Article/details/gaunpcxwb.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.sjlbkw.cn/Article/details/gnqrgbijz.sHtML

[D08] 合并两个数组
来源：http://baike.bbcook.cn/Article/details/gnnwxkmiu.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.sjlbkw.cn/Article/details/gfnihlkah.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.bbcook.cn/Article/details/gwixuejhf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.sjlbkw.cn/Article/details/glzmwlkpy.sHtML

TS:   [...a, ...b];
来源：http://blog.bbcook.cn/Article/details/guwnbtlhx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.tarul.cn/Article/details/gbakgosla.sHtML

Go:   append(a, b...)
来源：http://www.share.sjlbkw.cn/Article/details/gvkvpovfc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.epnwcf.com/Article/details/gsseryksr.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.vehdjk.com/Article/details/gmidgugnk.sHtML

[D09] 排序（升序）
来源：http://www.blog.sjlbkw.cn/Article/details/gbwthljpr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gflkdcghk.sHtML

PHP:  sort($arr);
来源：http://baike.vehdjk.com/Article/details/grqrwprml.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.bbcook.cn/Article/details/gbjdvmfwf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fktsv.cn/Article/details/ghskwaghj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.tarul.cn/Article/details/gdpvpcdok.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.vehdjk.com/Article/details/gvnixchmh.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gyasygcsp.sHtML

C#:   list.Sort();
来源：http://3g.yfazqb.com/Article/details/gvlbxgsfp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.bbcook.cn/Article/details/gpyuamvmc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.yfazqb.com/Article/details/gykzebwbn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gisldwxbe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/guyhskgcp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/gymwljktu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.bbcook.cn/Article/details/gwkariuni.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.yfazqb.com/Article/details/gzpnlmjbt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.vehdjk.com/Article/details/gngltbqvt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.tarul.cn/Article/details/gcqgbahcb.sHtML

[D11] 反转数组
来源：http://www.blog.yfazqb.com/Article/details/gcqxmmtbm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.epnwcf.com/Article/details/gqmroykti.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fktsv.cn/Article/details/grewqqcaa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.sjlbkw.cn/Article/details/gtchwotsq.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.tarul.cn/Article/details/gnidxxufc.sHtML

Java: Collections.reverse(list);
来源：http://www.share.epnwcf.com/Article/details/ggrdfqnrw.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.sjlbkw.cn/Article/details/gwynucfkp.sHtML

Ruby: arr.reverse
来源：http://read.share.vehdjk.com/Article/details/gdiyfixtn.sHtML

C#:   list.Reverse();
来源：http://3g.sjlbkw.cn/Article/details/gsbwumxmr.sHtML

[D12] 查找元素下标
来源：http://blog.yfazqb.com/Article/details/geunnrskp.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.epnwcf.com/Article/details/gnewuhorr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.sjlbkw.cn/Article/details/gwtoyjqds.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.yfazqb.com/Article/details/gjwcspqsq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.epnwcf.com/Article/details/glprnneen.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.vehdjk.com/Article/details/gbmcewfdb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gnbfhmrpz.sHtML

Ruby: arr.index(x)
来源：http://3g.sjlbkw.cn/Article/details/gvfytvmyq.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.epnwcf.com/Article/details/gqfirpqsh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.tarul.cn/Article/details/gafxflcss.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gvydjgtzs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gyrwgzega.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/gtdaazwdh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.vehdjk.com/Article/details/gvvlypnug.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gkbjlsasm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.epnwcf.com/Article/details/gdskfwdhu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.bbcook.cn/Article/details/gsbzoughm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gblsmxtlt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.yfazqb.com/Article/details/gnmsdopty.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.epnwcf.com/Article/details/gakoyvoxx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.epnwcf.com/Article/details/grhkzcfwh.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/gcxdpfegp.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/gkhnyviaa.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.bbcook.cn/Article/details/gfnlijydf.sHtML

Go:   // 手写循环
来源：http://m.share.sjlbkw.cn/Article/details/gsuzvybon.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.yfazqb.com/Article/details/glqcxyiyy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.bbcook.cn/Article/details/ghloytsns.sHtML

[D15] 去重
来源：http://www.m.share.fktsv.cn/Article/details/gwnxnptsi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/ghanesdya.sHtML

PHP:  array_unique($arr);
来源：http://read.share.tarul.cn/Article/details/gcwybvupi.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gzfdhrlpt.sHtML

TS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gvcfdxdib.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.epnwcf.com/Article/details/gpzisggjz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.tarul.cn/Article/details/ggqasnkha.sHtML

Ruby: arr.uniq
来源：http://baike.tarul.cn/Article/details/gugzltgji.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fktsv.cn/Article/details/guftkchau.sHtML

[D16] 求和与平均值
来源：http://mobile.vehdjk.com/Article/details/gcvzuiqhd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fktsv.cn/Article/details/gtawydtyx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gufbobjvj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/gyhqbmpei.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.yfazqb.com/Article/details/ggiykxgdd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fktsv.cn/Article/details/gveckdgim.sHtML

Go:   // 手写循环累加
来源：http://blog.epnwcf.com/Article/details/gzhjrtlcs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.sjlbkw.cn/Article/details/gpdesqrwh.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.epnwcf.com/Article/details/gkvjktmtl.sHtML

[D17] 最大值与最小值
来源：http://www.blog.bbcook.cn/Article/details/giolglfcr.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.bbcook.cn/Article/details/gkzotcowr.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.bbcook.cn/Article/details/gszfzeipt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.vehdjk.com/Article/details/gtesnhxlb.sHtML

TS:   Math.max(...arr);
来源：http://read.share.tarul.cn/Article/details/gzvgxwcln.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.sjlbkw.cn/Article/details/gozccssrz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.vehdjk.com/Article/details/gyahmmdhx.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.sjlbkw.cn/Article/details/gefzhdbfx.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fktsv.cn/Article/details/gfobpwlfo.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.vehdjk.com/Article/details/gqjbqskyu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.vehdjk.com/Article/details/gjodwjzuw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.epnwcf.com/Article/details/gwftqyifa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fktsv.cn/Article/details/gvphvifll.sHtML

TS:   nested.flat();
来源：http://wap.epnwcf.com/Article/details/gdskthrbo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fktsv.cn/Article/details/gpjwplsaf.sHtML

Go:   // 手写双层循环
来源：http://www.share.sjlbkw.cn/Article/details/gjpejjdib.sHtML

Ruby: nested.flatten
来源：http://wap.yfazqb.com/Article/details/glewmaxda.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.epnwcf.com/Article/details/gpaxgnicc.sHtML

[D19] 按字段分组
来源：http://m.share.sjlbkw.cn/Article/details/gcudjjpkn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.yfazqb.com/Article/details/gdjfyoybu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.tarul.cn/Article/details/gyqujoebs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.vehdjk.com/Article/details/gqbztyjaj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gnxymobki.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.vehdjk.com/Article/details/gzpqrmkjr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.sjlbkw.cn/Article/details/gzmkqyvwg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.yfazqb.com/Article/details/gcntyyahg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.yfazqb.com/Article/details/ggolgqpmm.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.vehdjk.com/Article/details/gryzlxpuv.sHtML

Py:   Counter(arr)
来源：http://www.share.bbcook.cn/Article/details/gdobcrdpf.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.vehdjk.com/Article/details/gtgjwtrlm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.yfazqb.com/Article/details/gazhwjddy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.vehdjk.com/Article/details/gvgkpcxvc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.sjlbkw.cn/Article/details/gkuizlwtq.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.vehdjk.com/Article/details/gqiluyire.sHtML

Ruby: arr.tally
来源：http://www.share.bbcook.cn/Article/details/glnjofeiq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.sjlbkw.cn/Article/details/ggbcwvuyn.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.tarul.cn/Article/details/gfatuvrhn.sHtML

Py:   x in arr
来源：http://3g.fktsv.cn/Article/details/gnaasowpi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.sjlbkw.cn/Article/details/gmipdbrzy.sHtML

JS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/gicjtrqgq.sHtML

TS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/grkfqmmdq.sHtML

Java: list.contains(x)
来源：http://3g.yfazqb.com/Article/details/gqnhaqrgv.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.epnwcf.com/Article/details/gvoxgailt.sHtML

Ruby: arr.include?(x)
来源：http://wap.sjlbkw.cn/Article/details/gtmvqikhf.sHtML

C#:   list.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gzabaaith.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.vehdjk.com/Article/details/grolspxow.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.bbcook.cn/Article/details/gikgwbwkg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.vehdjk.com/Article/details/glbtpjreb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.vehdjk.com/Article/details/gddlgiqag.sHtML

TS:   [...arr];
来源：http://wap.yfazqb.com/Article/details/gpinkvwuc.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.vehdjk.com/Article/details/gmshzafxf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fktsv.cn/Article/details/grcxqnsvs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqhstjpj.sHtML

C#:   new List<int>(list);
来源：http://mobile.sjlbkw.cn/Article/details/gqsocvwqo.sHtML

[D23] reduce 累积计算
来源：http://www.share.fktsv.cn/Article/details/gdtswfhuq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.sjlbkw.cn/Article/details/gflhmcxxc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.tarul.cn/Article/details/gfufcwkrh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gepqgdtqj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gdajpxbfk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fktsv.cn/Article/details/gvewkclqx.sHtML

Go:   // 手写循环
来源：http://www.blog.tarul.cn/Article/details/gkpsqnnmz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fktsv.cn/Article/details/grrzrulln.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.bbcook.cn/Article/details/gnvbfobmk.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.sjlbkw.cn/Article/details/gcvpjjflw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.tarul.cn/Article/details/gjypanggb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.vehdjk.com/Article/details/gnghdqkel.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fktsv.cn/Article/details/gvsnykjar.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gxwpjemts.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/gbtbwrftl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.bbcook.cn/Article/details/grnrcvdif.sHtML


<!-- 参考信息 -->