代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://baike.yfazqb.com/Article/details/gcywwusto.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.bbcook.cn/Article/details/gadncuucd.sHtML

[C08] 闭包
来源：http://www.blog.sjlbkw.cn/Article/details/gvyhuujpo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.yfazqb.com/Article/details/gwjjnxlgi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.tarul.cn/Article/details/gzuiolcbe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gyhwpbbtf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gknuylzzb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.tarul.cn/Article/details/gvybnhyto.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.tarul.cn/Article/details/glugubxpn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fktsv.cn/Article/details/gmohxnwux.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gufacmjgx.sHtML

[C09] 递归
来源：http://www.m.share.epnwcf.com/Article/details/gxibntlxd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.epnwcf.com/Article/details/gunjofqic.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fktsv.cn/Article/details/gauohprpm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.tarul.cn/Article/details/gefqrqtxc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/gbexfolyj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fktsv.cn/Article/details/gzihldyvu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhvrygkd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.epnwcf.com/Article/details/gpxqnuwym.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.vehdjk.com/Article/details/goqhjtacf.sHtML

[C10] 变量作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gbykusjrm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.tarul.cn/Article/details/gwbcelsnm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.vehdjk.com/Article/details/gnypblvts.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fktsv.cn/Article/details/gvdgdeyak.sHtML

TS:   同 JS
来源：http://wap.tarul.cn/Article/details/gzgohycsj.sHtML

Java: 方法内为块级作用域
来源：http://blog.fktsv.cn/Article/details/gbubevffh.sHtML

Go:   花括号块级作用域
来源：http://baike.yfazqb.com/Article/details/gxncfzrxx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.sjlbkw.cn/Article/details/gcniccvua.sHtML

C#:   块级作用域
来源：http://wap.epnwcf.com/Article/details/gqyrzkvkb.sHtML

[C11] 模块导入与导出
来源：http://wap.epnwcf.com/Article/details/gcmehqopw.sHtML

Py:   from module import func
来源：http://blog.vehdjk.com/Article/details/gzkwgpmrn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.bbcook.cn/Article/details/gsznowhzb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.vehdjk.com/Article/details/gqvqznvap.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.yfazqb.com/Article/details/gpqwfqlfa.sHtML

Java: import java.util.List;
来源：http://www.m.share.bbcook.cn/Article/details/glluizzzv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.yfazqb.com/Article/details/glkaupbqy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.tarul.cn/Article/details/glzutauhq.sHtML

C#:   using System.Text;
来源：http://www.blog.epnwcf.com/Article/details/gunzlwvkn.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.sjlbkw.cn/Article/details/gdknhbkpq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.yfazqb.com/Article/details/gryuazhtc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.bbcook.cn/Article/details/gehvkeklq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fktsv.cn/Article/details/gbqrudehq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/ghbmitybt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.bbcook.cn/Article/details/gvgjkefwd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.bbcook.cn/Article/details/ghisiazka.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.vehdjk.com/Article/details/gmealzxpa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.tarul.cn/Article/details/gpxpvlnec.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.tarul.cn/Article/details/gkgxaikeu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.vehdjk.com/Article/details/gyzjgmzrp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gyqvfnhav.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.tarul.cn/Article/details/gqjpgehxl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/ghsiecwhc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gqavaptqt.sHtML

Go:   func add(a, b int) int
来源：http://read.share.yfazqb.com/Article/details/gonftopwj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.tarul.cn/Article/details/gtxckdscy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.vehdjk.com/Article/details/gicnokckx.sHtML

[C14] 泛型函数
来源：http://baike.fktsv.cn/Article/details/ghhefghzc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.epnwcf.com/Article/details/gcakgqitd.sHtML

PHP:  // 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gipxwrnwn.sHtML

JS:   // 无泛型
来源：http://www.share.fktsv.cn/Article/details/gjbanyugy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.tarul.cn/Article/details/ggbyoglkn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.vehdjk.com/Article/details/gndlbepcv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.tarul.cn/Article/details/gvkkfkxru.sHtML

Ruby: # 无泛型
来源：http://read.share.epnwcf.com/Article/details/gzxvswviw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.bbcook.cn/Article/details/gxekfskgn.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fktsv.cn/Article/details/gowvmgtle.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.sjlbkw.cn/Article/details/gqnnaiozs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.vehdjk.com/Article/details/garpdiwds.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/garfqffhe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.tarul.cn/Article/details/gduzwkcdt.sHtML

Java: // 无解构
来源：http://3g.fktsv.cn/Article/details/garlklgtt.sHtML

Go:   // 无解构
来源：http://m.share.bbcook.cn/Article/details/ghfauvbnq.sHtML

Ruby: a, b = pair
来源：http://baike.fktsv.cn/Article/details/gedzjrrbo.sHtML

C#:   var (a, b) = pair;
来源：http://baike.sjlbkw.cn/Article/details/glbljgihx.sHtML

[C16] 函数 / 方法重载
来源：http://blog.sjlbkw.cn/Article/details/gkfzvquua.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.yfazqb.com/Article/details/guvabzfdb.sHtML

PHP:  // 无重载
来源：http://www.m.share.vehdjk.com/Article/details/gixidctzm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fktsv.cn/Article/details/gwhigngox.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.sjlbkw.cn/Article/details/ghikububr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.bbcook.cn/Article/details/genafhvnj.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.yfazqb.com/Article/details/glxbdbblp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fktsv.cn/Article/details/grwmiqani.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.yfazqb.com/Article/details/gprewqhxv.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtvkxxlqg.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.bbcook.cn/Article/details/gcyfhxkdn.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gejfqfjjj.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.sjlbkw.cn/Article/details/gngpfowdg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fktsv.cn/Article/details/gvjiqaesd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.epnwcf.com/Article/details/gtjeruskk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.tarul.cn/Article/details/giidvczbf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fktsv.cn/Article/details/grleijite.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.bbcook.cn/Article/details/ggrqfubht.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.tarul.cn/Article/details/gxlrarmam.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.tarul.cn/Article/details/gyvygsnrn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.bbcook.cn/Article/details/gqsyxurmd.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fktsv.cn/Article/details/gvhuyaiyd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.bbcook.cn/Article/details/ghpctbnjo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.sjlbkw.cn/Article/details/gyodstsog.sHtML

JS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/gqsqzjxmz.sHtML

TS:   arr.push(4);
来源：http://wap.sjlbkw.cn/Article/details/ggktbefqw.sHtML

Java: list.add(4);
来源：http://mobile.epnwcf.com/Article/details/glfmbfers.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpibprcbn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.vehdjk.com/Article/details/gsdsrbwkp.sHtML

C#:   list.Add(4);
来源：http://read.share.yfazqb.com/Article/details/gbfdksyyc.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fktsv.cn/Article/details/gwwpirgpw.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fktsv.cn/Article/details/geiwffhsa.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.vehdjk.com/Article/details/gipvfiatn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.epnwcf.com/Article/details/gvxorklfn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.epnwcf.com/Article/details/gsjqrobag.sHtML

Java: list.add(0, 0);
来源：http://wap.yfazqb.com/Article/details/gxpxnowch.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.epnwcf.com/Article/details/gospjautr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fktsv.cn/Article/details/gspsgavll.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fktsv.cn/Article/details/gbipdnrjw.sHtML

[D04] 删除元素
来源：http://m.share.sjlbkw.cn/Article/details/grzafithl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.tarul.cn/Article/details/ghhljhxcq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gyaeqostx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.epnwcf.com/Article/details/gyjvamxah.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.epnwcf.com/Article/details/gfpfyxlmz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.vehdjk.com/Article/details/gkvvsgciz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fktsv.cn/Article/details/gabdrcfqi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fktsv.cn/Article/details/gtygszzdu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.yfazqb.com/Article/details/gcfkxwdty.sHtML

[D05] 访问与修改元素
来源：http://read.share.vehdjk.com/Article/details/gnseaccez.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gjcsuxjuz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gzbbbznyw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gsuvtqzvv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.bbcook.cn/Article/details/gfvqfoyha.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.yfazqb.com/Article/details/gytizzfvg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gfgyxexei.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gyshwsryp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gakfccnyk.sHtML

[D06] 数组长度
来源：http://m.share.epnwcf.com/Article/details/gvcapnxcs.sHtML

Py:   len(arr)
来源：http://read.share.yfazqb.com/Article/details/gbpfivxtb.sHtML

PHP:  count($arr);
来源：http://www.m.share.fktsv.cn/Article/details/grazvjpvi.sHtML

JS:   arr.length
来源：http://www.m.share.yfazqb.com/Article/details/gyshijiho.sHtML

TS:   arr.length
来源：http://read.share.vehdjk.com/Article/details/gbogmjnuw.sHtML

Java: list.size();
来源：http://baike.tarul.cn/Article/details/gbvubzcnb.sHtML

Go:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gxnaggddp.sHtML

Ruby: arr.length; arr.size
来源：http://blog.vehdjk.com/Article/details/ggwotaxye.sHtML

C#:   list.Count;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaqnbjqs.sHtML

[D07] 切片 / 取子数组
来源：http://blog.bbcook.cn/Article/details/gauomlypv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.vehdjk.com/Article/details/gymdjtydd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.tarul.cn/Article/details/gyiwvteje.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gqbspdvsc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gpoimuwdh.sHtML

Java: list.subList(1, 4);
来源：http://baike.bbcook.cn/Article/details/gblotkcrg.sHtML

Go:   arr[1:4]
来源：http://wap.sjlbkw.cn/Article/details/gqjtrjpqo.sHtML

Ruby: arr[1, 3]
来源：http://www.share.vehdjk.com/Article/details/gyxghmnru.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.epnwcf.com/Article/details/gyvbceuih.sHtML

[D08] 合并两个数组
来源：http://baike.tarul.cn/Article/details/glogdexdx.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fktsv.cn/Article/details/gmiozljkj.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.yfazqb.com/Article/details/gjxboymlf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.bbcook.cn/Article/details/gbmvjkved.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.tarul.cn/Article/details/gsbuvktjh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fktsv.cn/Article/details/gohiafltx.sHtML

Go:   append(a, b...)
来源：http://m.share.bbcook.cn/Article/details/gybukyhcf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.vehdjk.com/Article/details/gzeycxcbc.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.yfazqb.com/Article/details/gxedvcifm.sHtML

[D09] 排序（升序）
来源：http://www.share.tarul.cn/Article/details/gkvzjvfay.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gzihfokem.sHtML

PHP:  sort($arr);
来源：http://m.share.tarul.cn/Article/details/gskwknkqn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.tarul.cn/Article/details/gjznkcrga.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.tarul.cn/Article/details/gjpoojqzd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fktsv.cn/Article/details/gejqmzqad.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/gpyzvpnaz.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gsadiemes.sHtML

C#:   list.Sort();
来源：http://baike.vehdjk.com/Article/details/glbunhoti.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.yfazqb.com/Article/details/goyajqafu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.epnwcf.com/Article/details/ggeoemkjp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gjvzjnsjx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gmfzfcfnm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/geqjouyac.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.bbcook.cn/Article/details/gphielabq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.epnwcf.com/Article/details/gwwxggfwh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fktsv.cn/Article/details/gicytbrum.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.tarul.cn/Article/details/guqhxjyfw.sHtML

[D11] 反转数组
来源：http://m.share.vehdjk.com/Article/details/gcauygfnz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fktsv.cn/Article/details/gyclgqbxz.sHtML

PHP:  array_reverse($arr);
来源：http://3g.vehdjk.com/Article/details/glsmdfads.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.yfazqb.com/Article/details/gtxecayqc.sHtML

TS:   [...arr].reverse();
来源：http://3g.bbcook.cn/Article/details/guwxrhlbq.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.bbcook.cn/Article/details/gatrtcufx.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fktsv.cn/Article/details/grbsckrgf.sHtML

Ruby: arr.reverse
来源：http://read.share.vehdjk.com/Article/details/grgsanfxf.sHtML

C#:   list.Reverse();
来源：http://www.blog.vehdjk.com/Article/details/ghabnvsqw.sHtML

[D12] 查找元素下标
来源：http://m.share.tarul.cn/Article/details/gprxfvdkc.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.tarul.cn/Article/details/gyvblppde.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.yfazqb.com/Article/details/gpoiyrlsp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/gykgaxvtu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.epnwcf.com/Article/details/gafuomlhl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.bbcook.cn/Article/details/gbjczblts.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.bbcook.cn/Article/details/gepxivenf.sHtML

Ruby: arr.index(x)
来源：http://baike.yfazqb.com/Article/details/glyxgbbwv.sHtML

C#:   list.IndexOf(x);
来源：http://baike.vehdjk.com/Article/details/grsjrhccg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.vehdjk.com/Article/details/gmqegszwx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fktsv.cn/Article/details/goktdhibt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fktsv.cn/Article/details/gionuifkd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.tarul.cn/Article/details/gqtnpyvkk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/gnxroaaka.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.epnwcf.com/Article/details/gejxuxlpw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.yfazqb.com/Article/details/gsnifikvq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fktsv.cn/Article/details/grcgbipam.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.tarul.cn/Article/details/gkzswyeax.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.yfazqb.com/Article/details/gagreydeo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.tarul.cn/Article/details/gbqeulipi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.bbcook.cn/Article/details/gugdhzwew.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.yfazqb.com/Article/details/gdeogqrgn.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.sjlbkw.cn/Article/details/gohaptgzh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gegdkyrdt.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/ggqlxkyac.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.yfazqb.com/Article/details/gymsfyzhl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gddtlodeh.sHtML

[D15] 去重
来源：http://mobile.bbcook.cn/Article/details/gnldxmijy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.epnwcf.com/Article/details/gqrgkmonb.sHtML

PHP:  array_unique($arr);
来源：http://www.share.sjlbkw.cn/Article/details/guzjsthzx.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/girvuppgq.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gemofezgi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.epnwcf.com/Article/details/gsyogqkwe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.sjlbkw.cn/Article/details/gsblgabbl.sHtML

Ruby: arr.uniq
来源：http://blog.bbcook.cn/Article/details/gboejwrhx.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.epnwcf.com/Article/details/gtchcbdib.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fktsv.cn/Article/details/gxpcdnjoq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.epnwcf.com/Article/details/gbwzbvsac.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.vehdjk.com/Article/details/govicwhjn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.epnwcf.com/Article/details/gvyouurbz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fktsv.cn/Article/details/gehggvoyu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.sjlbkw.cn/Article/details/grelplqzx.sHtML

Go:   // 手写循环累加
来源：http://wap.vehdjk.com/Article/details/gwybellie.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.tarul.cn/Article/details/gzuzgxqzy.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.epnwcf.com/Article/details/gmkhuycki.sHtML

[D17] 最大值与最小值
来源：http://read.share.bbcook.cn/Article/details/gbdexynyi.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fktsv.cn/Article/details/gdbpkaxgm.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.tarul.cn/Article/details/gzpsoyqxs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.epnwcf.com/Article/details/gmkxqswlt.sHtML

TS:   Math.max(...arr);
来源：http://wap.epnwcf.com/Article/details/gwikogzqn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.bbcook.cn/Article/details/gniqjvoel.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gsxsroykw.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.epnwcf.com/Article/details/grpbbdacr.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fktsv.cn/Article/details/ggogqnrlo.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.yfazqb.com/Article/details/grfnynmle.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.bbcook.cn/Article/details/gfvnixpeq.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.vehdjk.com/Article/details/gedcwobnn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fktsv.cn/Article/details/glsjqkgzq.sHtML

TS:   nested.flat();
来源：http://read.share.fktsv.cn/Article/details/gftwyyatl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.bbcook.cn/Article/details/gytfonjqd.sHtML

Go:   // 手写双层循环
来源：http://blog.bbcook.cn/Article/details/ghmkxvcsj.sHtML

Ruby: nested.flatten
来源：http://mobile.tarul.cn/Article/details/gvgwpdzpp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.vehdjk.com/Article/details/gmglquelf.sHtML

[D19] 按字段分组
来源：http://baike.vehdjk.com/Article/details/gejyrpbwx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.vehdjk.com/Article/details/gdariexam.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.epnwcf.com/Article/details/gjstavoqp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fktsv.cn/Article/details/gmobqtmij.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.vehdjk.com/Article/details/gkymetvir.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.tarul.cn/Article/details/gvalfcjfd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.epnwcf.com/Article/details/gbzwownah.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.yfazqb.com/Article/details/gokgtdmjm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fktsv.cn/Article/details/ggyouihdf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.epnwcf.com/Article/details/gzficrxkx.sHtML

Py:   Counter(arr)
来源：http://baike.fktsv.cn/Article/details/gwbdcjami.sHtML

PHP:  array_count_values($arr);
来源：http://wap.epnwcf.com/Article/details/gviiqmhsh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gvlawlusg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/ghehynnfy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.sjlbkw.cn/Article/details/gfayaopzd.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.bbcook.cn/Article/details/ggkjaioem.sHtML

Ruby: arr.tally
来源：http://www.m.share.yfazqb.com/Article/details/gimrbgmrf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.epnwcf.com/Article/details/geetfzlpy.sHtML

[D21] 判断是否包含某元素
来源：http://baike.yfazqb.com/Article/details/gexkxglnx.sHtML

Py:   x in arr
来源：http://baike.bbcook.cn/Article/details/gpwjrcjoj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.yfazqb.com/Article/details/gssngzvih.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/glqlieckh.sHtML

TS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gcueazgzg.sHtML

Java: list.contains(x)
来源：http://www.blog.vehdjk.com/Article/details/glqxeerfd.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.bbcook.cn/Article/details/grefadujd.sHtML

Ruby: arr.include?(x)
来源：http://wap.fktsv.cn/Article/details/gsjpqjklf.sHtML

C#:   list.Contains(x)
来源：http://wap.epnwcf.com/Article/details/glpvigkui.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.sjlbkw.cn/Article/details/grtookwms.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fktsv.cn/Article/details/gybjvrloo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.yfazqb.com/Article/details/gelgtiyyd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.epnwcf.com/Article/details/giafmaxae.sHtML

TS:   [...arr];
来源：http://www.blog.yfazqb.com/Article/details/grjgtfftw.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.vehdjk.com/Article/details/gfkcwyjzb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.epnwcf.com/Article/details/gmlbanchd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.vehdjk.com/Article/details/gprkykxxw.sHtML

C#:   new List<int>(list);
来源：http://m.share.sjlbkw.cn/Article/details/gikuoqkaa.sHtML

[D23] reduce 累积计算
来源：http://wap.bbcook.cn/Article/details/guznetcgb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.epnwcf.com/Article/details/gwlwydlmb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fktsv.cn/Article/details/gcsocnbxb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/gnxrjdyvr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/gwwpsmwxa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fktsv.cn/Article/details/ghvubxnwc.sHtML

Go:   // 手写循环
来源：http://m.share.tarul.cn/Article/details/gazqaexsr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.tarul.cn/Article/details/glhflibem.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.tarul.cn/Article/details/groztnndk.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.yfazqb.com/Article/details/gdzmuzqyd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fktsv.cn/Article/details/goxuvhjjz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fktsv.cn/Article/details/gkfiimhip.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.yfazqb.com/Article/details/gpdihbshd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/guwygleup.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fktsv.cn/Article/details/giozvaokj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.vehdjk.com/Article/details/gvjwugyak.sHtML


<!-- 参考信息 -->