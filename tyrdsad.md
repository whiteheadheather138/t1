代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.yfazqb.com/Article/details/gxwqsodbz.sHtML

TS:   arr.map(String)
来源：http://www.m.share.yfazqb.com/Article/details/ghgqervol.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.yfazqb.com/Article/details/gqqfjlmmw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.sjlbkw.cn/Article/details/getfoncml.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fktsv.cn/Article/details/gnhrhtwmh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.tarul.cn/Article/details/grjfohtup.sHtML

[C08] 闭包
来源：http://mobile.vehdjk.com/Article/details/gidfifcqb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.bbcook.cn/Article/details/gdcezmbyx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.vehdjk.com/Article/details/gjgcutaab.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gfoykwxck.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/grgbkjcpz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.vehdjk.com/Article/details/gwtoebgrq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.bbcook.cn/Article/details/gtpheiugw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.tarul.cn/Article/details/gqinuepsg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gxuwggovl.sHtML

[C09] 递归
来源：http://www.blog.sjlbkw.cn/Article/details/gywvwuprg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fktsv.cn/Article/details/giaeuyxsh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.sjlbkw.cn/Article/details/gadnchvur.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gvzroeulp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gfmtvgzcg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fktsv.cn/Article/details/gvfamhehb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.sjlbkw.cn/Article/details/gxknsftfr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fktsv.cn/Article/details/gwjmrrhsp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.epnwcf.com/Article/details/gwnckzsfd.sHtML

[C10] 变量作用域
来源：http://read.share.tarul.cn/Article/details/gulewtwfh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fktsv.cn/Article/details/gsebjqosd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.sjlbkw.cn/Article/details/gstwmargf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.yfazqb.com/Article/details/gbnheksnr.sHtML

TS:   同 JS
来源：http://baike.bbcook.cn/Article/details/ghdusrvhs.sHtML

Java: 方法内为块级作用域
来源：http://3g.fktsv.cn/Article/details/gfbfqhccu.sHtML

Go:   花括号块级作用域
来源：http://m.share.epnwcf.com/Article/details/gbrovhadn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.yfazqb.com/Article/details/gekinrokf.sHtML

C#:   块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gwqcoozyn.sHtML

[C11] 模块导入与导出
来源：http://m.share.vehdjk.com/Article/details/gfznnjwxh.sHtML

Py:   from module import func
来源：http://m.share.bbcook.cn/Article/details/gxyzcpffs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.epnwcf.com/Article/details/gprfowinc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gkpfezjfn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.sjlbkw.cn/Article/details/gnsqsejof.sHtML

Java: import java.util.List;
来源：http://baike.yfazqb.com/Article/details/gcdqejfxi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.vehdjk.com/Article/details/guttdlzwm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.bbcook.cn/Article/details/girbvnsos.sHtML

C#:   using System.Text;
来源：http://wap.epnwcf.com/Article/details/gsdruyeav.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.yfazqb.com/Article/details/ghevxcrrl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fktsv.cn/Article/details/gvcxaburi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.tarul.cn/Article/details/gtlhdmtrt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.bbcook.cn/Article/details/gwbcaivts.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fktsv.cn/Article/details/gcutkjtkx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.yfazqb.com/Article/details/gfipqcybm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fktsv.cn/Article/details/gnoqhtlsz.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.vehdjk.com/Article/details/gghvrlvhx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.tarul.cn/Article/details/gftnjsadi.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.tarul.cn/Article/details/gkifaebfs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.sjlbkw.cn/Article/details/gdmhcaolw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gpszmtsng.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.bbcook.cn/Article/details/gmfnveqdr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gysnrdvuk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gzzvpniwa.sHtML

Go:   func add(a, b int) int
来源：http://wap.fktsv.cn/Article/details/gjqwbyclr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/gxsyqpupj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.epnwcf.com/Article/details/gcpaeedlx.sHtML

[C14] 泛型函数
来源：http://www.m.share.vehdjk.com/Article/details/gyzajwiev.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.vehdjk.com/Article/details/gyudqukoj.sHtML

PHP:  // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gtjatwscx.sHtML

JS:   // 无泛型
来源：http://3g.fktsv.cn/Article/details/glcmrjili.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.bbcook.cn/Article/details/gwsnuurgz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.epnwcf.com/Article/details/gjwzjbjyx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fktsv.cn/Article/details/galbexlmg.sHtML

Ruby: # 无泛型
来源：http://wap.sjlbkw.cn/Article/details/ghlpbbwpt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.bbcook.cn/Article/details/gqbpjipjx.sHtML

[C15] 解构 / 展开参数
来源：http://3g.bbcook.cn/Article/details/gbuxwnwwp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.epnwcf.com/Article/details/gnnbhfhqr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.bbcook.cn/Article/details/gpcwzjhwb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/gmbuzguul.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.vehdjk.com/Article/details/gqawpsqbp.sHtML

Java: // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gpecnekgj.sHtML

Go:   // 无解构
来源：http://3g.fktsv.cn/Article/details/gztixarla.sHtML

Ruby: a, b = pair
来源：http://m.share.fktsv.cn/Article/details/gkegdajmp.sHtML

C#:   var (a, b) = pair;
来源：http://3g.yfazqb.com/Article/details/gapridsxg.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.vehdjk.com/Article/details/gddndqyxi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fktsv.cn/Article/details/gxyylbcbw.sHtML

PHP:  // 无重载
来源：http://m.share.bbcook.cn/Article/details/gmtuzkfel.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.vehdjk.com/Article/details/gofcbokiw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.tarul.cn/Article/details/gybmlvrsq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.sjlbkw.cn/Article/details/gaqlppqpm.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.vehdjk.com/Article/details/gycugjmsm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.bbcook.cn/Article/details/gkaavqvox.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.vehdjk.com/Article/details/gklqmwlxn.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gujmhqkeo.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.sjlbkw.cn/Article/details/gipbapuhs.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gnjwtcplv.sHtML

[D01] 创建数组 / 列表
来源：http://baike.yfazqb.com/Article/details/gilvbpowq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.epnwcf.com/Article/details/gmgfvmclm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.sjlbkw.cn/Article/details/goltfjszu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.bbcook.cn/Article/details/gcihfokvx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.vehdjk.com/Article/details/ggjntqqph.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.tarul.cn/Article/details/gugwgcupm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fktsv.cn/Article/details/gaskltgvt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.tarul.cn/Article/details/guqsfkqwf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.sjlbkw.cn/Article/details/gxgmvgtsh.sHtML

[D02] 追加元素到末尾
来源：http://3g.epnwcf.com/Article/details/grenlzczp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.epnwcf.com/Article/details/gwsmnroyb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.yfazqb.com/Article/details/gsygplrsv.sHtML

JS:   arr.push(4);
来源：http://read.share.tarul.cn/Article/details/gjvkeahup.sHtML

TS:   arr.push(4);
来源：http://read.share.yfazqb.com/Article/details/gfubynnyy.sHtML

Java: list.add(4);
来源：http://www.m.share.fktsv.cn/Article/details/guytbvaoh.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.vehdjk.com/Article/details/ghheaxjcq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.tarul.cn/Article/details/ggyuaoofq.sHtML

C#:   list.Add(4);
来源：http://mobile.bbcook.cn/Article/details/gahpgljdi.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.sjlbkw.cn/Article/details/gdchlbldm.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.vehdjk.com/Article/details/gwqcvdane.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.sjlbkw.cn/Article/details/gthkfrgzr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.vehdjk.com/Article/details/geherdxgm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.tarul.cn/Article/details/gurctrfrx.sHtML

Java: list.add(0, 0);
来源：http://wap.sjlbkw.cn/Article/details/gbvvqwoin.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.yfazqb.com/Article/details/gmifkpgmd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.bbcook.cn/Article/details/gkffbzoxx.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.tarul.cn/Article/details/gcqjowuex.sHtML

[D04] 删除元素
来源：http://wap.sjlbkw.cn/Article/details/gsezvsyse.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.sjlbkw.cn/Article/details/gwhqcawqg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.tarul.cn/Article/details/grcpahier.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.sjlbkw.cn/Article/details/gjnaqfavh.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.epnwcf.com/Article/details/gywrneyoe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.bbcook.cn/Article/details/gumixbybe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.yfazqb.com/Article/details/gccpoezul.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.tarul.cn/Article/details/gpggzqwtu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/golqntztb.sHtML

[D05] 访问与修改元素
来源：http://blog.fktsv.cn/Article/details/gbpilifig.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/gkwqfubkq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gecnwnojc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/grwcvribh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fktsv.cn/Article/details/glakcepyi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.bbcook.cn/Article/details/gmtxgwthx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gvksczcmr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gmmswdmdt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.tarul.cn/Article/details/gcazdykce.sHtML

[D06] 数组长度
来源：http://wap.fktsv.cn/Article/details/gkqdxbkro.sHtML

Py:   len(arr)
来源：http://read.share.yfazqb.com/Article/details/gnxsniwfg.sHtML

PHP:  count($arr);
来源：http://www.share.fktsv.cn/Article/details/gcwyrcxrm.sHtML

JS:   arr.length
来源：http://www.m.share.bbcook.cn/Article/details/gmlgseyzm.sHtML

TS:   arr.length
来源：http://www.blog.yfazqb.com/Article/details/gadqyxzxx.sHtML

Java: list.size();
来源：http://blog.epnwcf.com/Article/details/gojndmpbs.sHtML

Go:   len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/giponnkyz.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.yfazqb.com/Article/details/gnoeocsay.sHtML

C#:   list.Count;
来源：http://3g.bbcook.cn/Article/details/gtlyzkyij.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkpmccun.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.yfazqb.com/Article/details/gsfrldmwy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.vehdjk.com/Article/details/gldytsdzd.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/gfaylvtnx.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.bbcook.cn/Article/details/gsixhfedy.sHtML

Java: list.subList(1, 4);
来源：http://read.share.tarul.cn/Article/details/gdsxeyady.sHtML

Go:   arr[1:4]
来源：http://wap.yfazqb.com/Article/details/groabwfkd.sHtML

Ruby: arr[1, 3]
来源：http://www.share.yfazqb.com/Article/details/gnzxnwpbp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gjsrqfknh.sHtML

[D08] 合并两个数组
来源：http://baike.sjlbkw.cn/Article/details/gliafiuqh.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.bbcook.cn/Article/details/gxwxliagc.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.bbcook.cn/Article/details/gavpkbgok.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.tarul.cn/Article/details/gqbdngdyd.sHtML

TS:   [...a, ...b];
来源：http://blog.tarul.cn/Article/details/gevuxaxkh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fktsv.cn/Article/details/gqykxiyjq.sHtML

Go:   append(a, b...)
来源：http://wap.epnwcf.com/Article/details/gghidtvjk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fktsv.cn/Article/details/gsnawdlfh.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.vehdjk.com/Article/details/gvoiomsii.sHtML

[D09] 排序（升序）
来源：http://read.share.epnwcf.com/Article/details/gsntqwoap.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/gjidroolb.sHtML

PHP:  sort($arr);
来源：http://blog.yfazqb.com/Article/details/gxrtqermn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.yfazqb.com/Article/details/gvbrreent.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fktsv.cn/Article/details/gptawecrp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.yfazqb.com/Article/details/gfboiwllq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gpytiufrm.sHtML

Ruby: arr.sort
来源：http://baike.bbcook.cn/Article/details/gxeizmsoi.sHtML

C#:   list.Sort();
来源：http://3g.tarul.cn/Article/details/gtcnciynb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.yfazqb.com/Article/details/ggzvtxdjo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.yfazqb.com/Article/details/gcdkjxwnl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gobtzsjne.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.bbcook.cn/Article/details/gdjlparge.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/ghexkebor.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.bbcook.cn/Article/details/gnzlokvul.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.vehdjk.com/Article/details/gbauflikl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.sjlbkw.cn/Article/details/gsffuohdu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdcyoqrx.sHtML

[D11] 反转数组
来源：http://baike.tarul.cn/Article/details/gdimkbhlz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.epnwcf.com/Article/details/gnyrmudkw.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.tarul.cn/Article/details/gxxawotwd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.tarul.cn/Article/details/gvgqvurkm.sHtML

TS:   [...arr].reverse();
来源：http://mobile.yfazqb.com/Article/details/grwiwcokn.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fktsv.cn/Article/details/gtfghoozp.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gqhujwhve.sHtML

Ruby: arr.reverse
来源：http://wap.fktsv.cn/Article/details/gbkmyclob.sHtML

C#:   list.Reverse();
来源：http://www.share.tarul.cn/Article/details/grkmjjfhi.sHtML

[D12] 查找元素下标
来源：http://read.share.sjlbkw.cn/Article/details/gycaiabdn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.epnwcf.com/Article/details/gulpnweyw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.vehdjk.com/Article/details/gkalwoyeh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/ghwwvcwge.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gywsghqcu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fktsv.cn/Article/details/ggkustmjd.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gyczezkfu.sHtML

Ruby: arr.index(x)
来源：http://wap.vehdjk.com/Article/details/gfqrlzysd.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.bbcook.cn/Article/details/gqprspjlw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.tarul.cn/Article/details/grhrxqzfo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.yfazqb.com/Article/details/glzbbtkwt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fktsv.cn/Article/details/gtcjoxlsn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/guxbbvpji.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.epnwcf.com/Article/details/gcoflscqs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.tarul.cn/Article/details/gbfcpvbhi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fktsv.cn/Article/details/gbnzejicb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fktsv.cn/Article/details/gnrheodiv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.bbcook.cn/Article/details/gdmsndgyb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.tarul.cn/Article/details/gnarribak.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fktsv.cn/Article/details/gdqazxtzd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/giesywutd.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.tarul.cn/Article/details/ghwbdrhhm.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fktsv.cn/Article/details/gksxbyfje.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gqpobwybu.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/gyezcqqfv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.epnwcf.com/Article/details/goygmwyjp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gqmlwqoxf.sHtML

[D15] 去重
来源：http://m.share.sjlbkw.cn/Article/details/gkabicuhj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/gjyydufkp.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fktsv.cn/Article/details/gxoqwrzkz.sHtML

JS:   [...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/grbqofqoo.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gmrmhsavw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.bbcook.cn/Article/details/gvdcghgez.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.bbcook.cn/Article/details/gjjsshzms.sHtML

Ruby: arr.uniq
来源：http://wap.bbcook.cn/Article/details/gupbksfyo.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.sjlbkw.cn/Article/details/grvaqoulq.sHtML

[D16] 求和与平均值
来源：http://blog.epnwcf.com/Article/details/gsihbcpgt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.vehdjk.com/Article/details/ghmhrlxog.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.vehdjk.com/Article/details/gmsujpuzs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/ggcnidhkl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.epnwcf.com/Article/details/gfefoyvqp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fktsv.cn/Article/details/gwqqciqvv.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.vehdjk.com/Article/details/gstxcerxo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gnajeesss.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.tarul.cn/Article/details/gcwowxtef.sHtML

[D17] 最大值与最小值
来源：http://wap.epnwcf.com/Article/details/gntgxwwfp.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.vehdjk.com/Article/details/gqbcpfnck.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.epnwcf.com/Article/details/gvhvtiyni.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.yfazqb.com/Article/details/gqxxmtotj.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.bbcook.cn/Article/details/gyiiwywcw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.bbcook.cn/Article/details/gfhwkvrbf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.tarul.cn/Article/details/ghcpyuxxb.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.vehdjk.com/Article/details/gbnpwxzoe.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/grfkuihue.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.vehdjk.com/Article/details/gzsqzuhdc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.tarul.cn/Article/details/gmtuhaykn.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.sjlbkw.cn/Article/details/gyorabztg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.bbcook.cn/Article/details/gjjzqjuum.sHtML

TS:   nested.flat();
来源：http://www.m.share.tarul.cn/Article/details/gjfylzupb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.sjlbkw.cn/Article/details/gyirojohi.sHtML

Go:   // 手写双层循环
来源：http://mobile.epnwcf.com/Article/details/gdfqriowa.sHtML

Ruby: nested.flatten
来源：http://www.share.fktsv.cn/Article/details/gqixhbjvu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.tarul.cn/Article/details/gzlqhkulj.sHtML

[D19] 按字段分组
来源：http://3g.yfazqb.com/Article/details/gzvocxnus.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.epnwcf.com/Article/details/gdcmvowxd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.tarul.cn/Article/details/gqgtngzdr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.yfazqb.com/Article/details/gpufasldr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/geydzqlth.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.vehdjk.com/Article/details/gczgasast.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.bbcook.cn/Article/details/geamznjfi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.epnwcf.com/Article/details/gsvhtkfxx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.tarul.cn/Article/details/gaxfabqwd.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.sjlbkw.cn/Article/details/ghytwpfpz.sHtML

Py:   Counter(arr)
来源：http://www.share.yfazqb.com/Article/details/gubysiirz.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.tarul.cn/Article/details/gvlrnyfuf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/gyghuubmr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gcemrdttw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.vehdjk.com/Article/details/gmwfgwcwx.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.tarul.cn/Article/details/gmealncmd.sHtML

Ruby: arr.tally
来源：http://wap.tarul.cn/Article/details/gdgzspogd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.epnwcf.com/Article/details/gxdvlanpx.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.vehdjk.com/Article/details/gwvojvjcf.sHtML

Py:   x in arr
来源：http://www.share.yfazqb.com/Article/details/gbowzftew.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.yfazqb.com/Article/details/gsigmbgfx.sHtML

JS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gokbtvhcg.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/goxxcokqe.sHtML

Java: list.contains(x)
来源：http://m.share.tarul.cn/Article/details/gzoqdzxyi.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gueljtohy.sHtML

Ruby: arr.include?(x)
来源：http://www.share.epnwcf.com/Article/details/gmomlkjku.sHtML

C#:   list.Contains(x)
来源：http://wap.yfazqb.com/Article/details/gcvpybgvy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.tarul.cn/Article/details/gncoelbaw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.epnwcf.com/Article/details/gbzjwjfzb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.yfazqb.com/Article/details/gunvlzfnf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gvlwtvbzm.sHtML

TS:   [...arr];
来源：http://www.blog.bbcook.cn/Article/details/gthcjkpvq.sHtML

Java: new ArrayList<>(list);
来源：http://baike.sjlbkw.cn/Article/details/gdqxkmhuk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fktsv.cn/Article/details/gxpuohdeh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fktsv.cn/Article/details/gqousjybj.sHtML

C#:   new List<int>(list);
来源：http://blog.sjlbkw.cn/Article/details/gxraomdze.sHtML

[D23] reduce 累积计算
来源：http://m.share.fktsv.cn/Article/details/gnhidikvi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.yfazqb.com/Article/details/gtcqpntwp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gmvwcopbg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.bbcook.cn/Article/details/gqkqmaxyb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gnylinqpy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.epnwcf.com/Article/details/gtpgcctnu.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/gywfwuhtl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fktsv.cn/Article/details/girawoenn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fktsv.cn/Article/details/gbqywpyfi.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.bbcook.cn/Article/details/grpgmhzka.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gesbnkolp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fktsv.cn/Article/details/gzshyvtsk.sHtML


<!-- 参考信息 -->