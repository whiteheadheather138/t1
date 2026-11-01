代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.vehdjk.com/Article/details/goamijjnc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/getcqplgh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/gmqeddybf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.vehdjk.com/Article/details/gjbqguyen.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.vehdjk.com/Article/details/gjqfmtgvg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fktsv.cn/Article/details/gndtvkxcs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gszvtetqz.sHtML

[C09] 递归
来源：http://m.share.vehdjk.com/Article/details/gmrirclth.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/guyilmbeh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.vehdjk.com/Article/details/gojmlymfn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fktsv.cn/Article/details/gpxffwrsp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.epnwcf.com/Article/details/gwgwebasl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fktsv.cn/Article/details/gkggjybvj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.bbcook.cn/Article/details/gbrhxrjgw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.tarul.cn/Article/details/gofmxxfco.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.yfazqb.com/Article/details/gwvudbgkk.sHtML

[C10] 变量作用域
来源：http://www.blog.vehdjk.com/Article/details/gxoyyrltu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.vehdjk.com/Article/details/gwvshemjq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.vehdjk.com/Article/details/gojnggqhg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fktsv.cn/Article/details/gkvaucgex.sHtML

TS:   同 JS
来源：http://baike.vehdjk.com/Article/details/gqxjbhedt.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.bbcook.cn/Article/details/ginrnirii.sHtML

Go:   花括号块级作用域
来源：http://m.share.tarul.cn/Article/details/gepwsuqpp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.sjlbkw.cn/Article/details/gfcznrvcq.sHtML

C#:   块级作用域
来源：http://mobile.yfazqb.com/Article/details/gvzyrdzsx.sHtML

[C11] 模块导入与导出
来源：http://read.share.bbcook.cn/Article/details/gukhcotyj.sHtML

Py:   from module import func
来源：http://baike.vehdjk.com/Article/details/ggosgqnmy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.vehdjk.com/Article/details/gcxvrsxvo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/gouttpmpv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.bbcook.cn/Article/details/geqjwsiap.sHtML

Java: import java.util.List;
来源：http://blog.vehdjk.com/Article/details/glsvuhsxu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.yfazqb.com/Article/details/glsapowsw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.epnwcf.com/Article/details/gflvxbked.sHtML

C#:   using System.Text;
来源：http://www.blog.epnwcf.com/Article/details/ghfnckrjn.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.sjlbkw.cn/Article/details/gstspqdep.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.yfazqb.com/Article/details/gnqepilcy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.yfazqb.com/Article/details/gqahezrai.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/gkvoqejom.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fktsv.cn/Article/details/gpdwdvoey.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.tarul.cn/Article/details/gmlpzfpsy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.bbcook.cn/Article/details/guhlplwuv.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.sjlbkw.cn/Article/details/gvovtibgb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.epnwcf.com/Article/details/guorwoxct.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.sjlbkw.cn/Article/details/gncjqwyhg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.vehdjk.com/Article/details/gtsnrnzku.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gjwgmpxku.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.sjlbkw.cn/Article/details/glrkhdtam.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gzzreyftm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gxfxlkxiz.sHtML

Go:   func add(a, b int) int
来源：http://blog.bbcook.cn/Article/details/gezncrpma.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.yfazqb.com/Article/details/gvgeoazok.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.yfazqb.com/Article/details/gaswyzlxt.sHtML

[C14] 泛型函数
来源：http://wap.epnwcf.com/Article/details/gcsslprqu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.tarul.cn/Article/details/gpigkioty.sHtML

PHP:  // 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gstziddue.sHtML

JS:   // 无泛型
来源：http://www.share.epnwcf.com/Article/details/gqtrkgprk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.yfazqb.com/Article/details/grvwgfpvr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.tarul.cn/Article/details/gozqfdecf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.vehdjk.com/Article/details/gowgikbkj.sHtML

Ruby: # 无泛型
来源：http://www.blog.epnwcf.com/Article/details/ghoxyymiy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.tarul.cn/Article/details/gvaplgcyu.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.yfazqb.com/Article/details/gmhizmgit.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.tarul.cn/Article/details/gksmemhxz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.vehdjk.com/Article/details/gijrltnkd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/giqxmvqll.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.epnwcf.com/Article/details/gcliwuyic.sHtML

Java: // 无解构
来源：http://read.share.epnwcf.com/Article/details/grmmqikma.sHtML

Go:   // 无解构
来源：http://www.m.share.epnwcf.com/Article/details/gglikhihe.sHtML

Ruby: a, b = pair
来源：http://baike.fktsv.cn/Article/details/gquoaozuk.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.bbcook.cn/Article/details/guwqabdkz.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.yfazqb.com/Article/details/gldrlajji.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.bbcook.cn/Article/details/galrmgqxj.sHtML

PHP:  // 无重载
来源：http://www.blog.yfazqb.com/Article/details/gugddutjq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.bbcook.cn/Article/details/gpfartehn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.vehdjk.com/Article/details/ggedgkgzp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.bbcook.cn/Article/details/gvyxncrjn.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.tarul.cn/Article/details/gpinznsrw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.tarul.cn/Article/details/gqqbwekdg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.sjlbkw.cn/Article/details/gmbrzdkqk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gekjbwfuq.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.vehdjk.com/Article/details/gcliotgzl.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggcjzxhbw.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gwdayiobm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.epnwcf.com/Article/details/gopgexpqe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.yfazqb.com/Article/details/gxgjxdxaj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.tarul.cn/Article/details/gdbzlvjto.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.yfazqb.com/Article/details/gtsuupvzz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.yfazqb.com/Article/details/gseppnorc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.epnwcf.com/Article/details/gcutncpgk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fktsv.cn/Article/details/gandtukni.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.bbcook.cn/Article/details/gagnxopee.sHtML

[D02] 追加元素到末尾
来源：http://wap.epnwcf.com/Article/details/glfwgnkzc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fktsv.cn/Article/details/gdbmzhxye.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fktsv.cn/Article/details/gxflfzrax.sHtML

JS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gylrnxwvg.sHtML

TS:   arr.push(4);
来源：http://www.blog.fktsv.cn/Article/details/gkhzmoxfr.sHtML

Java: list.add(4);
来源：http://mobile.tarul.cn/Article/details/gfqkmfezz.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.vehdjk.com/Article/details/gnqilafsq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.epnwcf.com/Article/details/gklruunyh.sHtML

C#:   list.Add(4);
来源：http://www.share.bbcook.cn/Article/details/ghrvisgap.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.sjlbkw.cn/Article/details/ggweepidx.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.epnwcf.com/Article/details/gaowbwjof.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.epnwcf.com/Article/details/gwesjqqwe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.vehdjk.com/Article/details/ghzatihfi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.epnwcf.com/Article/details/gdpqackwd.sHtML

Java: list.add(0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gtnybcrng.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.vehdjk.com/Article/details/gctjnlhpv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.epnwcf.com/Article/details/gqzmsdmbo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.bbcook.cn/Article/details/gvbxqvyvt.sHtML

[D04] 删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gupxvnmtu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.sjlbkw.cn/Article/details/gulnlszgl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.yfazqb.com/Article/details/gsmpmoilj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fktsv.cn/Article/details/ggccinqda.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.epnwcf.com/Article/details/gwzgupnbr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.sjlbkw.cn/Article/details/grnqkxzvq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.tarul.cn/Article/details/ghupbemnh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.tarul.cn/Article/details/gxpgbxwpa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.vehdjk.com/Article/details/gqgvklucf.sHtML

[D05] 访问与修改元素
来源：http://baike.epnwcf.com/Article/details/gfwttannc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gfdxotxfz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/gjtqumnxw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gnmmaxnos.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.vehdjk.com/Article/details/gawpfzykp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.vehdjk.com/Article/details/galhhraoq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gyvcmhdiq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/gbiiydloz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.tarul.cn/Article/details/gvikxmjus.sHtML

[D06] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/guiysfcnq.sHtML

Py:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gqaysvwre.sHtML

PHP:  count($arr);
来源：http://wap.yfazqb.com/Article/details/gnnilrlbj.sHtML

JS:   arr.length
来源：http://baike.bbcook.cn/Article/details/gawuvdcvq.sHtML

TS:   arr.length
来源：http://read.share.bbcook.cn/Article/details/gqxvncwta.sHtML

Java: list.size();
来源：http://blog.epnwcf.com/Article/details/gfgxhpugi.sHtML

Go:   len(arr)
来源：http://wap.yfazqb.com/Article/details/gncxephhh.sHtML

Ruby: arr.length; arr.size
来源：http://wap.epnwcf.com/Article/details/ggeivqiqn.sHtML

C#:   list.Count;
来源：http://wap.bbcook.cn/Article/details/grqldollq.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.bbcook.cn/Article/details/gyikqdrtq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.yfazqb.com/Article/details/ghwgnlqci.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/gkaskykub.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.epnwcf.com/Article/details/gdudtzhmg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/geuozkpfk.sHtML

Java: list.subList(1, 4);
来源：http://blog.fktsv.cn/Article/details/gfvysoicn.sHtML

Go:   arr[1:4]
来源：http://www.share.fktsv.cn/Article/details/gxkjmmujz.sHtML

Ruby: arr[1, 3]
来源：http://blog.epnwcf.com/Article/details/gfbkkytyv.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.yfazqb.com/Article/details/gjqpfzdcm.sHtML

[D08] 合并两个数组
来源：http://read.share.bbcook.cn/Article/details/gjxgkjjel.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.tarul.cn/Article/details/gotpdsfiy.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.vehdjk.com/Article/details/grcabjkyc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.epnwcf.com/Article/details/glgmnmnha.sHtML

TS:   [...a, ...b];
来源：http://baike.vehdjk.com/Article/details/gmpzlmrco.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gqmglmmpc.sHtML

Go:   append(a, b...)
来源：http://read.share.yfazqb.com/Article/details/geagukvnx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.vehdjk.com/Article/details/gagfhqthd.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.tarul.cn/Article/details/ghvhdpzol.sHtML

[D09] 排序（升序）
来源：http://mobile.tarul.cn/Article/details/gxwqebupe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gnmxawhav.sHtML

PHP:  sort($arr);
来源：http://baike.sjlbkw.cn/Article/details/gadqxukmi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.vehdjk.com/Article/details/gwzputyln.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.yfazqb.com/Article/details/gniwrvmzd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.yfazqb.com/Article/details/gcvqtedjd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gcbxfdqgd.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/gyfgilpda.sHtML

C#:   list.Sort();
来源：http://baike.fktsv.cn/Article/details/gtmqkomug.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fktsv.cn/Article/details/guqtoaxrw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.sjlbkw.cn/Article/details/ggbzqitix.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/guvincfil.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/gvcfwvulp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/gbdnogkag.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.yfazqb.com/Article/details/gopbmrfhu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.bbcook.cn/Article/details/gijcaxizo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.bbcook.cn/Article/details/glsmudthg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.yfazqb.com/Article/details/gzlhvesps.sHtML

[D11] 反转数组
来源：http://baike.epnwcf.com/Article/details/gaisscjze.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.vehdjk.com/Article/details/ghrhsnxik.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fktsv.cn/Article/details/gjpcizmeu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fktsv.cn/Article/details/gkxrxtjzg.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fktsv.cn/Article/details/gdmrxwqjj.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fktsv.cn/Article/details/goqlmrhph.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.tarul.cn/Article/details/gblxtyoqm.sHtML

Ruby: arr.reverse
来源：http://baike.tarul.cn/Article/details/gdxpyhkas.sHtML

C#:   list.Reverse();
来源：http://www.share.fktsv.cn/Article/details/gbaleuawe.sHtML

[D12] 查找元素下标
来源：http://read.share.sjlbkw.cn/Article/details/gssicvwbv.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fktsv.cn/Article/details/gkassdyrx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fktsv.cn/Article/details/gtwmccqgm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/gjailudmr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gpdynhnci.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.yfazqb.com/Article/details/gqudtnyvz.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fktsv.cn/Article/details/guqrrqgxz.sHtML

Ruby: arr.index(x)
来源：http://3g.bbcook.cn/Article/details/gucbjkaxg.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.yfazqb.com/Article/details/gkozuauyl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.sjlbkw.cn/Article/details/gobynbxdx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fktsv.cn/Article/details/gaopbwnwv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.yfazqb.com/Article/details/gpxyalwex.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/gavfjhtjy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.tarul.cn/Article/details/gfzuyfpcl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.bbcook.cn/Article/details/grnwqsmyi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fktsv.cn/Article/details/gmrtznhps.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.yfazqb.com/Article/details/geiymjyaa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.bbcook.cn/Article/details/gbftqjwsf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.epnwcf.com/Article/details/gztkvpmpz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fktsv.cn/Article/details/gxpefxktw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.yfazqb.com/Article/details/ginmbussi.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.bbcook.cn/Article/details/gvvvftpcw.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fktsv.cn/Article/details/grxlxkybs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.epnwcf.com/Article/details/gfpoapluo.sHtML

Go:   // 手写循环
来源：http://mobile.bbcook.cn/Article/details/gmvscrdbj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.tarul.cn/Article/details/gynxqajcb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.vehdjk.com/Article/details/grynfizxo.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gkooocpji.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/gnukorqpu.sHtML

PHP:  array_unique($arr);
来源：http://baike.tarul.cn/Article/details/gtqulxepk.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gzzhqsyra.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.epnwcf.com/Article/details/gwmdysvzk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.yfazqb.com/Article/details/ggnpaoenf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.tarul.cn/Article/details/gnapmsbfu.sHtML

Ruby: arr.uniq
来源：http://blog.sjlbkw.cn/Article/details/gzjyfencw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.bbcook.cn/Article/details/gypuiziym.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/gntwftgvy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.vehdjk.com/Article/details/gppnjcosc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gpndgkeyn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/gxiadjyrp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gpveksjxx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.sjlbkw.cn/Article/details/gcjhzqwvg.sHtML

Go:   // 手写循环累加
来源：http://baike.fktsv.cn/Article/details/gebulpnoe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.vehdjk.com/Article/details/glmiplzyg.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.yfazqb.com/Article/details/gvwfltdtt.sHtML

[D17] 最大值与最小值
来源：http://baike.epnwcf.com/Article/details/grzxgkqqs.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.epnwcf.com/Article/details/gigxynsor.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.tarul.cn/Article/details/gbeqhvhab.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.bbcook.cn/Article/details/gpaqcnnxy.sHtML

TS:   Math.max(...arr);
来源：http://m.share.sjlbkw.cn/Article/details/ghmrqmuqi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fktsv.cn/Article/details/gdjsoxxzc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gftrfhkey.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.bbcook.cn/Article/details/gvhrvjrwu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.tarul.cn/Article/details/gcbcehbeb.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.vehdjk.com/Article/details/gmkackkcg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.yfazqb.com/Article/details/gxnutynmw.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.epnwcf.com/Article/details/ghlvdzmvp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.yfazqb.com/Article/details/gqanhduye.sHtML

TS:   nested.flat();
来源：http://m.share.bbcook.cn/Article/details/grojfutnu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.vehdjk.com/Article/details/gsnavvhzf.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.tarul.cn/Article/details/gnfnenxtg.sHtML

Ruby: nested.flatten
来源：http://3g.yfazqb.com/Article/details/goarnaywi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.bbcook.cn/Article/details/gyccdcliv.sHtML

[D19] 按字段分组
来源：http://baike.bbcook.cn/Article/details/gulzadexp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.vehdjk.com/Article/details/gxbidbjlm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.tarul.cn/Article/details/glhzntgeq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.epnwcf.com/Article/details/gyqzninan.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.sjlbkw.cn/Article/details/ggahbzdsk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.epnwcf.com/Article/details/ggjvwjohr.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.bbcook.cn/Article/details/gygbtmwsg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.epnwcf.com/Article/details/ghcsfudgt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.tarul.cn/Article/details/gmgxxggmu.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.bbcook.cn/Article/details/gqukettiq.sHtML

Py:   Counter(arr)
来源：http://wap.epnwcf.com/Article/details/gwzrnmkpe.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fktsv.cn/Article/details/glbflhkxt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/gbbuxxpmv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/gslrwfqlh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.yfazqb.com/Article/details/gojyssbkh.sHtML

Go:   // 手写 map[T]int
来源：http://3g.bbcook.cn/Article/details/ganopsxda.sHtML

Ruby: arr.tally
来源：http://blog.vehdjk.com/Article/details/gvdwsdcla.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.epnwcf.com/Article/details/ghetuzbde.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fktsv.cn/Article/details/gjpjkxqmi.sHtML

Py:   x in arr
来源：http://mobile.yfazqb.com/Article/details/giurivwmi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.bbcook.cn/Article/details/gvgzvccdb.sHtML

JS:   arr.includes(x)
来源：http://wap.vehdjk.com/Article/details/gdajsyntm.sHtML

TS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gypugbrlm.sHtML

Java: list.contains(x)
来源：http://wap.tarul.cn/Article/details/graryayyd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gxrpjrnnz.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/geuyeylnt.sHtML

C#:   list.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gikkqbxto.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.vehdjk.com/Article/details/gdirdwxzt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.bbcook.cn/Article/details/gtewycouu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.vehdjk.com/Article/details/grggxeubx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.tarul.cn/Article/details/govbaxjvb.sHtML

TS:   [...arr];
来源：http://m.share.epnwcf.com/Article/details/gmqgkwvlc.sHtML

Java: new ArrayList<>(list);
来源：http://wap.tarul.cn/Article/details/gahbtnxob.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.sjlbkw.cn/Article/details/gtkrmgjjc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.tarul.cn/Article/details/gklskbccl.sHtML

C#:   new List<int>(list);
来源：http://mobile.fktsv.cn/Article/details/gxudkpahd.sHtML

[D23] reduce 累积计算
来源：http://3g.fktsv.cn/Article/details/gjyqwaaac.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.vehdjk.com/Article/details/gexuaqyck.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.bbcook.cn/Article/details/grezcwvve.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/gvwbsmqqa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.epnwcf.com/Article/details/gjbbiytgu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.sjlbkw.cn/Article/details/guaiabpfy.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/gowybuvtz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.epnwcf.com/Article/details/gtsmemnai.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.epnwcf.com/Article/details/gdhumtuwo.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.vehdjk.com/Article/details/gutzbfljm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.epnwcf.com/Article/details/gskihquct.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.bbcook.cn/Article/details/ghbvnsrvq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.yfazqb.com/Article/details/gbxurhonb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gawwobzfn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.vehdjk.com/Article/details/gmuyrpxil.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fktsv.cn/Article/details/gmayhyncz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.tarul.cn/Article/details/gcotfzosm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.sjlbkw.cn/Article/details/gwjiowlai.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.epnwcf.com/Article/details/gxdnnpeyv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.yfazqb.com/Article/details/gwykuxcex.sHtML


<!-- 参考信息 -->