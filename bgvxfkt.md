代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://3g.vehdjk.com/Article/details/gomwaftmj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.tarul.cn/Article/details/giopnexke.sHtML

[C08] 闭包
来源：http://baike.vehdjk.com/Article/details/gyuxwvjyk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvpxfowp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fktsv.cn/Article/details/gpxtamgid.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gistixtkm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gxyfsdwkj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/gnwfyavcp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.sjlbkw.cn/Article/details/ggypzdagy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.tarul.cn/Article/details/grujrugdo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gpzipjrge.sHtML

[C09] 递归
来源：http://baike.bbcook.cn/Article/details/guqxovbkn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/gjardxdod.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/gbdwcrcoj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gboikuhkx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.epnwcf.com/Article/details/glyfhrkuf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.yfazqb.com/Article/details/gtcsywfib.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.bbcook.cn/Article/details/gmiltyofd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.vehdjk.com/Article/details/goizkbhzw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.tarul.cn/Article/details/giuxktiwr.sHtML

[C10] 变量作用域
来源：http://3g.fktsv.cn/Article/details/gheroqsjt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.epnwcf.com/Article/details/gkoytbvsg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.epnwcf.com/Article/details/gazhcrqyp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.bbcook.cn/Article/details/gqyfdyzmg.sHtML

TS:   同 JS
来源：http://www.m.share.tarul.cn/Article/details/goqwdljjo.sHtML

Java: 方法内为块级作用域
来源：http://mobile.bbcook.cn/Article/details/gfgslxfye.sHtML

Go:   花括号块级作用域
来源：http://read.share.vehdjk.com/Article/details/gdwppfomd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.sjlbkw.cn/Article/details/grsbrdaci.sHtML

C#:   块级作用域
来源：http://wap.fktsv.cn/Article/details/gqhuetdqd.sHtML

[C11] 模块导入与导出
来源：http://wap.vehdjk.com/Article/details/gwhalamql.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/gbyarnzdj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.sjlbkw.cn/Article/details/gbwryegcw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fktsv.cn/Article/details/gfytabuen.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.epnwcf.com/Article/details/gxyexawiz.sHtML

Java: import java.util.List;
来源：http://www.share.sjlbkw.cn/Article/details/gkvdnklgw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.sjlbkw.cn/Article/details/gxfgroccf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.sjlbkw.cn/Article/details/gfyumychc.sHtML

C#:   using System.Text;
来源：http://www.blog.tarul.cn/Article/details/gjtrmjpxc.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.tarul.cn/Article/details/gzaivwjgp.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.bbcook.cn/Article/details/gzdxjtakr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.sjlbkw.cn/Article/details/gstndleft.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/gbewhrszv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.yfazqb.com/Article/details/gfzmqacuf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/gfwfiqmya.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.epnwcf.com/Article/details/gefrdlkbu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.tarul.cn/Article/details/gslwrywlj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/gvgykbxcl.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.bbcook.cn/Article/details/gcluknade.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.bbcook.cn/Article/details/ghuyrfggu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gzgzuxrcj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.sjlbkw.cn/Article/details/gptmwabym.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gwrntgapr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gzlpymggn.sHtML

Go:   func add(a, b int) int
来源：http://read.share.bbcook.cn/Article/details/ghbitxpkh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.bbcook.cn/Article/details/giccwcihs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fktsv.cn/Article/details/gdfrelewv.sHtML

[C14] 泛型函数
来源：http://baike.vehdjk.com/Article/details/gikjtxekq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.yfazqb.com/Article/details/gzczmchot.sHtML

PHP:  // 无泛型
来源：http://blog.tarul.cn/Article/details/gcybvpllz.sHtML

JS:   // 无泛型
来源：http://blog.fktsv.cn/Article/details/gxkfoyakx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.bbcook.cn/Article/details/gkyvbqjxj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.epnwcf.com/Article/details/gbaortphq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.tarul.cn/Article/details/gegdwjjux.sHtML

Ruby: # 无泛型
来源：http://read.share.epnwcf.com/Article/details/giiitnpva.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.vehdjk.com/Article/details/goocxdlwt.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fktsv.cn/Article/details/gaipjphwa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.tarul.cn/Article/details/guzzqbrhz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.vehdjk.com/Article/details/geioghibb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/giavayhxs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.tarul.cn/Article/details/gpxlgstzd.sHtML

Java: // 无解构
来源：http://wap.tarul.cn/Article/details/glcqqijyu.sHtML

Go:   // 无解构
来源：http://m.share.vehdjk.com/Article/details/ggcbosucj.sHtML

Ruby: a, b = pair
来源：http://3g.sjlbkw.cn/Article/details/gowttrjsm.sHtML

C#:   var (a, b) = pair;
来源：http://blog.vehdjk.com/Article/details/gszjepoyn.sHtML

[C16] 函数 / 方法重载
来源：http://3g.vehdjk.com/Article/details/ginpojxol.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gdvkfbefu.sHtML

PHP:  // 无重载
来源：http://mobile.sjlbkw.cn/Article/details/grkxvkuln.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fktsv.cn/Article/details/gexrsaopp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fktsv.cn/Article/details/ghhhmjacf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.epnwcf.com/Article/details/gurjrucpd.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.bbcook.cn/Article/details/gimzrziar.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.tarul.cn/Article/details/gozoztsar.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.tarul.cn/Article/details/gqmdnfelm.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glaufbfew.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.epnwcf.com/Article/details/ghmlfzpko.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqsajadqp.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fktsv.cn/Article/details/grooszlbg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.epnwcf.com/Article/details/glcfwtzja.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.vehdjk.com/Article/details/gobsesocg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.bbcook.cn/Article/details/ggpdkwfom.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.yfazqb.com/Article/details/ggvfljrbd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.tarul.cn/Article/details/gkmnfjehj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.vehdjk.com/Article/details/gufemhhxi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.bbcook.cn/Article/details/gblyzutjo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.tarul.cn/Article/details/ggglpwgxs.sHtML

[D02] 追加元素到末尾
来源：http://baike.sjlbkw.cn/Article/details/gpkoamtde.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.yfazqb.com/Article/details/gcyioixha.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fktsv.cn/Article/details/gxuuwtpor.sHtML

JS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/gsoqgvqrz.sHtML

TS:   arr.push(4);
来源：http://mobile.sjlbkw.cn/Article/details/gskrpcqco.sHtML

Java: list.add(4);
来源：http://3g.bbcook.cn/Article/details/gqushzaqy.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.vehdjk.com/Article/details/gkqpyrunb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.sjlbkw.cn/Article/details/gmsmcxqvl.sHtML

C#:   list.Add(4);
来源：http://blog.yfazqb.com/Article/details/grvmyfbqn.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gedzlsdfg.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.epnwcf.com/Article/details/glyvigimc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.yfazqb.com/Article/details/gtlsyprbq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fktsv.cn/Article/details/gdkelytrm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.bbcook.cn/Article/details/gueqsajrd.sHtML

Java: list.add(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/ggqsnpexu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.tarul.cn/Article/details/gnjcmfood.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.tarul.cn/Article/details/ggjcsaodh.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.epnwcf.com/Article/details/giljzxtix.sHtML

[D04] 删除元素
来源：http://mobile.fktsv.cn/Article/details/genrlsndi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fktsv.cn/Article/details/garwsrefp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.epnwcf.com/Article/details/gzwzfwhdy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fktsv.cn/Article/details/gygbjsyvb.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.sjlbkw.cn/Article/details/gnzdrckei.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.sjlbkw.cn/Article/details/gonoyhmyq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.vehdjk.com/Article/details/gutvpiiib.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.bbcook.cn/Article/details/gwkijotoc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/gawovtohe.sHtML

[D05] 访问与修改元素
来源：http://mobile.bbcook.cn/Article/details/gvrfnbwdv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gqnqzpmtb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/gqwhldbyb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gympeszxs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.epnwcf.com/Article/details/gogyszlmd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.tarul.cn/Article/details/genormvun.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/grasmtnlw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/ghmdzbzgf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/gzuymvxoj.sHtML

[D06] 数组长度
来源：http://m.share.epnwcf.com/Article/details/gnxgfqtqf.sHtML

Py:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gsxvjuffh.sHtML

PHP:  count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/goqqaaqfg.sHtML

JS:   arr.length
来源：http://3g.tarul.cn/Article/details/gxjcuipwz.sHtML

TS:   arr.length
来源：http://wap.epnwcf.com/Article/details/gdvglquca.sHtML

Java: list.size();
来源：http://www.m.share.fktsv.cn/Article/details/gogeklhjv.sHtML

Go:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/gnidebybg.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.vehdjk.com/Article/details/gjikgsdml.sHtML

C#:   list.Count;
来源：http://www.share.fktsv.cn/Article/details/gmzlaexlb.sHtML

[D07] 切片 / 取子数组
来源：http://wap.tarul.cn/Article/details/gavvpyrer.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.epnwcf.com/Article/details/gjjanlwab.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gswclixzo.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/glkowjnya.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/glyqoqmpw.sHtML

Java: list.subList(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gfurfldgz.sHtML

Go:   arr[1:4]
来源：http://wap.fktsv.cn/Article/details/ghqerohyc.sHtML

Ruby: arr[1, 3]
来源：http://m.share.epnwcf.com/Article/details/grjriqfwk.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.bbcook.cn/Article/details/gufdidibb.sHtML

[D08] 合并两个数组
来源：http://baike.sjlbkw.cn/Article/details/glnnonrnm.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.tarul.cn/Article/details/gcrnymoxs.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fktsv.cn/Article/details/govcxboyt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.tarul.cn/Article/details/gpdmwbtjd.sHtML

TS:   [...a, ...b];
来源：http://wap.vehdjk.com/Article/details/gtdohuwms.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.tarul.cn/Article/details/gpecqxrgy.sHtML

Go:   append(a, b...)
来源：http://wap.vehdjk.com/Article/details/gdirtvetf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.tarul.cn/Article/details/gqkoeuerf.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.vehdjk.com/Article/details/gyenibpzl.sHtML

[D09] 排序（升序）
来源：http://read.share.tarul.cn/Article/details/gfpwvipok.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gbmyzhtac.sHtML

PHP:  sort($arr);
来源：http://wap.bbcook.cn/Article/details/gzghdzfoj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.tarul.cn/Article/details/gogeksovp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.sjlbkw.cn/Article/details/ghqwrncte.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.sjlbkw.cn/Article/details/gfqbkkkir.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/glmfaavky.sHtML

Ruby: arr.sort
来源：http://www.m.share.bbcook.cn/Article/details/ghkedlhev.sHtML

C#:   list.Sort();
来源：http://m.share.bbcook.cn/Article/details/gsvbaidoq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fktsv.cn/Article/details/gswjneguu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.epnwcf.com/Article/details/gdffhbiuc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.bbcook.cn/Article/details/gwingzedt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.sjlbkw.cn/Article/details/gqsdhxzxa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gmenktozh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.tarul.cn/Article/details/ggitmykzp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.bbcook.cn/Article/details/guoufnnmq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.tarul.cn/Article/details/gobmjblhq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.bbcook.cn/Article/details/gvzkovssv.sHtML

[D11] 反转数组
来源：http://baike.vehdjk.com/Article/details/gqpihaskr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fktsv.cn/Article/details/gyqbtqstl.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.bbcook.cn/Article/details/gynuhzokf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fktsv.cn/Article/details/gpttvdvip.sHtML

TS:   [...arr].reverse();
来源：http://3g.sjlbkw.cn/Article/details/gwgzwreaw.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fktsv.cn/Article/details/gwnxbfkgk.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.vehdjk.com/Article/details/gbqnnasez.sHtML

Ruby: arr.reverse
来源：http://wap.fktsv.cn/Article/details/goxxhiear.sHtML

C#:   list.Reverse();
来源：http://www.blog.tarul.cn/Article/details/gaeivokri.sHtML

[D12] 查找元素下标
来源：http://mobile.epnwcf.com/Article/details/guphjxlsd.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.tarul.cn/Article/details/gwjwncyxd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.yfazqb.com/Article/details/glvfttthk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/gxttacatn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/gxuhdajbh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fktsv.cn/Article/details/gbofbiryu.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/grvezhwkd.sHtML

Ruby: arr.index(x)
来源：http://www.blog.vehdjk.com/Article/details/gdrnjlxwn.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.bbcook.cn/Article/details/gfrowwcxk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.bbcook.cn/Article/details/gdfennjdm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gamyacowl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.sjlbkw.cn/Article/details/gzvhtoauy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fktsv.cn/Article/details/gwxjvmxgm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/gfqadzhvc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fktsv.cn/Article/details/gtrpzkjoe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fktsv.cn/Article/details/gzsltijan.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.bbcook.cn/Article/details/guflbluhm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.epnwcf.com/Article/details/gzmjwaapo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.vehdjk.com/Article/details/gqlqcwptp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.bbcook.cn/Article/details/gmmczlfrt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fktsv.cn/Article/details/gzkgvwjdo.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/gimaxxqaw.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/gawjanakx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.tarul.cn/Article/details/giijktafp.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gyayvhzhy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.tarul.cn/Article/details/gztlfbfkm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gzvyynijg.sHtML

[D15] 去重
来源：http://www.m.share.tarul.cn/Article/details/gveamtumt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.bbcook.cn/Article/details/gykxbmief.sHtML

PHP:  array_unique($arr);
来源：http://read.share.tarul.cn/Article/details/goqnnyduk.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/geogzdwkh.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/grypgksuk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.bbcook.cn/Article/details/gatvsvjxx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.tarul.cn/Article/details/gkopihxet.sHtML

Ruby: arr.uniq
来源：http://3g.yfazqb.com/Article/details/gbjlkfjhd.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fktsv.cn/Article/details/gatqalqzn.sHtML

[D16] 求和与平均值
来源：http://read.share.vehdjk.com/Article/details/gofugibng.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.vehdjk.com/Article/details/gwjzirdai.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.sjlbkw.cn/Article/details/ggqsyjxdj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.yfazqb.com/Article/details/ghsxxcgse.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gxwokcjyl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.yfazqb.com/Article/details/gducrvjsl.sHtML

Go:   // 手写循环累加
来源：http://read.share.epnwcf.com/Article/details/geslzzypn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.epnwcf.com/Article/details/gkxxcrnnm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.bbcook.cn/Article/details/gvtbvsbbi.sHtML

[D17] 最大值与最小值
来源：http://blog.sjlbkw.cn/Article/details/gdnjrwalp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gzqxfhema.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.epnwcf.com/Article/details/gijkaresz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.bbcook.cn/Article/details/gemuqrncl.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fktsv.cn/Article/details/gsdnopefr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.tarul.cn/Article/details/gxkwdojjp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.yfazqb.com/Article/details/gsybbepjm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.tarul.cn/Article/details/gpqllzpag.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.sjlbkw.cn/Article/details/gcsihceir.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.sjlbkw.cn/Article/details/gfbltsuii.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.tarul.cn/Article/details/gdawjzesy.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.epnwcf.com/Article/details/grpdzrfbz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.bbcook.cn/Article/details/gxwaujaen.sHtML

TS:   nested.flat();
来源：http://www.share.yfazqb.com/Article/details/gxyvebsnt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.tarul.cn/Article/details/gbbmkbkae.sHtML

Go:   // 手写双层循环
来源：http://baike.fktsv.cn/Article/details/gmgyucdqe.sHtML

Ruby: nested.flatten
来源：http://mobile.vehdjk.com/Article/details/gucpojyoz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.sjlbkw.cn/Article/details/govybxchj.sHtML

[D19] 按字段分组
来源：http://m.share.bbcook.cn/Article/details/gvvjlomrx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.bbcook.cn/Article/details/guhwkhrxv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.vehdjk.com/Article/details/gsxtuyqvr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.epnwcf.com/Article/details/gaktcwlrj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.epnwcf.com/Article/details/gzuxgsjut.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.tarul.cn/Article/details/gfuhvowyg.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.sjlbkw.cn/Article/details/gykithrte.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.bbcook.cn/Article/details/glcatbtvk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.bbcook.cn/Article/details/gzajeksfg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.sjlbkw.cn/Article/details/gidfknqhn.sHtML

Py:   Counter(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gwxetdpbj.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fktsv.cn/Article/details/gktcbfkuh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/gmolcjwlt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.bbcook.cn/Article/details/gvjkiwrxg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.vehdjk.com/Article/details/gkdkzvjpl.sHtML

Go:   // 手写 map[T]int
来源：http://wap.sjlbkw.cn/Article/details/gbiyemijj.sHtML

Ruby: arr.tally
来源：http://read.share.sjlbkw.cn/Article/details/gsdnzjdhd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.vehdjk.com/Article/details/gkfhlfnip.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.bbcook.cn/Article/details/gxgccprpq.sHtML

Py:   x in arr
来源：http://mobile.epnwcf.com/Article/details/gbjeofdhf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fktsv.cn/Article/details/goangbavw.sHtML

JS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/grsfnbscf.sHtML

TS:   arr.includes(x)
来源：http://read.share.epnwcf.com/Article/details/gfbgvrbix.sHtML

Java: list.contains(x)
来源：http://read.share.bbcook.cn/Article/details/ggdxiuxyk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gcnayiefq.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gntslarqp.sHtML

C#:   list.Contains(x)
来源：http://blog.epnwcf.com/Article/details/ghnmektjp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.epnwcf.com/Article/details/gjihcztgh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.tarul.cn/Article/details/gswqdcalj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fktsv.cn/Article/details/gvuovdrjy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.yfazqb.com/Article/details/goxxbgpnf.sHtML

TS:   [...arr];
来源：http://blog.sjlbkw.cn/Article/details/gvygtxpst.sHtML

Java: new ArrayList<>(list);
来源：http://baike.sjlbkw.cn/Article/details/gzpaqxqez.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.bbcook.cn/Article/details/golpgppmt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.epnwcf.com/Article/details/grzyfhtyt.sHtML

C#:   new List<int>(list);
来源：http://read.share.fktsv.cn/Article/details/gcktamhcs.sHtML

[D23] reduce 累积计算
来源：http://mobile.bbcook.cn/Article/details/grvyejszu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.sjlbkw.cn/Article/details/gcieiczly.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fktsv.cn/Article/details/ghpxuxoio.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/geqafbjmt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.vehdjk.com/Article/details/gpwnjgmzg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fktsv.cn/Article/details/grsrviebn.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/gdzryzwkt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.vehdjk.com/Article/details/gexukzbjc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fktsv.cn/Article/details/geyzzlnox.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.yfazqb.com/Article/details/gmgzbjbpu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.yfazqb.com/Article/details/gnjkvxecb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fktsv.cn/Article/details/godjaqvgz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fktsv.cn/Article/details/gnvltfewo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gldfzzimq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.tarul.cn/Article/details/gkzjidcoz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.sjlbkw.cn/Article/details/gzfwlxcsg.sHtML


<!-- 参考信息 -->