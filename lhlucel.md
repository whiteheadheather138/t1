代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://baike.tarul.cn/Article/details/gymncgyeb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.sjlbkw.cn/Article/details/gsmfrwubz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.sjlbkw.cn/Article/details/gxlbcuixy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.tarul.cn/Article/details/gonpzdqzm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/gbvetfxjz.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.epnwcf.com/Article/details/geauqjgrt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fktsv.cn/Article/details/goosrauiy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.yfazqb.com/Article/details/gxnxlwapx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.yfazqb.com/Article/details/gqzbsjbka.sHtML

TS:   arr.map(String)
来源：http://mobile.epnwcf.com/Article/details/gisnrlnqz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.epnwcf.com/Article/details/gxhyoxzbu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.sjlbkw.cn/Article/details/gktweuigv.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.bbcook.cn/Article/details/gaexlojtd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.tarul.cn/Article/details/gajkccoii.sHtML

[C08] 闭包
来源：http://www.m.share.fktsv.cn/Article/details/gzoealpqm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.yfazqb.com/Article/details/gqtcneons.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.yfazqb.com/Article/details/gcuwsbnbh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gldvbbqlk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gjuoerwxz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.tarul.cn/Article/details/gdkwsutqj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.vehdjk.com/Article/details/gzvozypak.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.vehdjk.com/Article/details/gufblqlvm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gckjwdhle.sHtML

[C09] 递归
来源：http://m.share.sjlbkw.cn/Article/details/gatdodyzs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/gyqqlxtix.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.epnwcf.com/Article/details/gdzmzbebh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gvqldsrpd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/gksjwlfoi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.sjlbkw.cn/Article/details/gfalhajsv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.tarul.cn/Article/details/gzjilmxuw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/grewnkfww.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.bbcook.cn/Article/details/gbqtkyecd.sHtML

[C10] 变量作用域
来源：http://mobile.bbcook.cn/Article/details/gefdykpjz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.vehdjk.com/Article/details/gszvouihq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.tarul.cn/Article/details/gwwkedvkd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.epnwcf.com/Article/details/gcpesgzjq.sHtML

TS:   同 JS
来源：http://3g.bbcook.cn/Article/details/gbbpxyuba.sHtML

Java: 方法内为块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gzwjffhhl.sHtML

Go:   花括号块级作用域
来源：http://3g.sjlbkw.cn/Article/details/geeyhiwst.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.bbcook.cn/Article/details/gyddxamym.sHtML

C#:   块级作用域
来源：http://www.share.fktsv.cn/Article/details/gsbcflolf.sHtML

[C11] 模块导入与导出
来源：http://baike.fktsv.cn/Article/details/gwpqxmpfv.sHtML

Py:   from module import func
来源：http://wap.yfazqb.com/Article/details/gafzekpox.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fktsv.cn/Article/details/gkvnicfhr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.tarul.cn/Article/details/gyebkiufb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.yfazqb.com/Article/details/gjkigocyx.sHtML

Java: import java.util.List;
来源：http://3g.epnwcf.com/Article/details/gmyrmhygp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fktsv.cn/Article/details/gdkrutdrn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.sjlbkw.cn/Article/details/gpmfqnfmj.sHtML

C#:   using System.Text;
来源：http://3g.fktsv.cn/Article/details/gjjqgiecd.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.vehdjk.com/Article/details/gfyaravux.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.sjlbkw.cn/Article/details/gynsfnccd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.yfazqb.com/Article/details/gtwtielkt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/ggulzhfoa.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/gyngedzxw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/gaxwzluod.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.vehdjk.com/Article/details/grmobzcxn.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.vehdjk.com/Article/details/gshlhauxi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.tarul.cn/Article/details/gnwmlutle.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.yfazqb.com/Article/details/ggkpvqerz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.bbcook.cn/Article/details/gefezuwrz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gpdleiqfn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.epnwcf.com/Article/details/gfbulyxof.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gdcszfeei.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/goyfzqyxz.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fktsv.cn/Article/details/gonjwlych.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fktsv.cn/Article/details/gxfpuwukq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fktsv.cn/Article/details/gyhmcgjcr.sHtML

[C14] 泛型函数
来源：http://www.share.fktsv.cn/Article/details/gtjbpplms.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.tarul.cn/Article/details/gpqlxffiq.sHtML

PHP:  // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gcgixcbtk.sHtML

JS:   // 无泛型
来源：http://read.share.epnwcf.com/Article/details/gpiaetbtl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fktsv.cn/Article/details/gawyxeqmf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.tarul.cn/Article/details/ghdhupcvb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.bbcook.cn/Article/details/ggngljked.sHtML

Ruby: # 无泛型
来源：http://mobile.yfazqb.com/Article/details/ghamwniza.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fktsv.cn/Article/details/goeobfico.sHtML

[C15] 解构 / 展开参数
来源：http://wap.vehdjk.com/Article/details/gjbbzmece.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.vehdjk.com/Article/details/gynfdfojt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.tarul.cn/Article/details/glitoawvq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.epnwcf.com/Article/details/ggnulbfql.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.bbcook.cn/Article/details/grtwytltq.sHtML

Java: // 无解构
来源：http://3g.yfazqb.com/Article/details/ghxamdxeo.sHtML

Go:   // 无解构
来源：http://3g.bbcook.cn/Article/details/guoevjpkh.sHtML

Ruby: a, b = pair
来源：http://3g.bbcook.cn/Article/details/ghgqajfuk.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.tarul.cn/Article/details/gjelfomim.sHtML

[C16] 函数 / 方法重载
来源：http://baike.bbcook.cn/Article/details/gjsyegneb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.vehdjk.com/Article/details/gilntikjw.sHtML

PHP:  // 无重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gpssyabgz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.sjlbkw.cn/Article/details/gvyhbfdos.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.vehdjk.com/Article/details/gssotwtrn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.bbcook.cn/Article/details/gyqdleeuw.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.tarul.cn/Article/details/gkpxgechj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.sjlbkw.cn/Article/details/gwokygnqo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.tarul.cn/Article/details/gigodzrjn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gbuacjbyx.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fktsv.cn/Article/details/geievaume.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gyrrutafz.sHtML

[D01] 创建数组 / 列表
来源：http://3g.tarul.cn/Article/details/gxribgfet.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.sjlbkw.cn/Article/details/gcsjlcigw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.sjlbkw.cn/Article/details/gtkdvwsrz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.vehdjk.com/Article/details/gfkxtvojs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.sjlbkw.cn/Article/details/gpciezaru.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fktsv.cn/Article/details/gnzyweexy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.tarul.cn/Article/details/gqdtciolq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.sjlbkw.cn/Article/details/gpkvrarru.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.epnwcf.com/Article/details/gchrtoyhn.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.bbcook.cn/Article/details/gubnhrvtg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.tarul.cn/Article/details/gvmhfttuw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.sjlbkw.cn/Article/details/gicjrybkf.sHtML

JS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/grymcyvpr.sHtML

TS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/gvfbnscgb.sHtML

Java: list.add(4);
来源：http://wap.sjlbkw.cn/Article/details/ghwrfexln.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.epnwcf.com/Article/details/grdjezgev.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.sjlbkw.cn/Article/details/gsejrjkgl.sHtML

C#:   list.Add(4);
来源：http://www.m.share.tarul.cn/Article/details/ghkanvrse.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.tarul.cn/Article/details/gmvgjgktk.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.vehdjk.com/Article/details/gjxvwcazh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.epnwcf.com/Article/details/gdwdiuqes.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.bbcook.cn/Article/details/gqgqqjjhu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fktsv.cn/Article/details/gmvjweihy.sHtML

Java: list.add(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gadjmgpib.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.yfazqb.com/Article/details/glqtwciaf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fktsv.cn/Article/details/gqumvoiaa.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.vehdjk.com/Article/details/gffegnxwm.sHtML

[D04] 删除元素
来源：http://3g.vehdjk.com/Article/details/gghjhxsxe.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.vehdjk.com/Article/details/gkxrhlpyl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.tarul.cn/Article/details/gyomjkhik.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.yfazqb.com/Article/details/gxkwynlup.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.tarul.cn/Article/details/geqiqzvaz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.sjlbkw.cn/Article/details/gjxkxmtsh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.bbcook.cn/Article/details/gkpzqabbv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.vehdjk.com/Article/details/gvbzaqhbn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.sjlbkw.cn/Article/details/gxblfattc.sHtML

[D05] 访问与修改元素
来源：http://wap.vehdjk.com/Article/details/gzipyzxnq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/ggvqhyfgy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/gpyggtdbe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.bbcook.cn/Article/details/gtgcnldoj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.bbcook.cn/Article/details/gfofpalez.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.yfazqb.com/Article/details/gatfhpryf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gmwngiyiu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gafoygwoz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gkrdficug.sHtML

[D06] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/ghqkijtph.sHtML

Py:   len(arr)
来源：http://m.share.fktsv.cn/Article/details/galzsahbo.sHtML

PHP:  count($arr);
来源：http://baike.tarul.cn/Article/details/grvqtvvut.sHtML

JS:   arr.length
来源：http://mobile.fktsv.cn/Article/details/gqkpunnhm.sHtML

TS:   arr.length
来源：http://www.m.share.fktsv.cn/Article/details/gflawuyhm.sHtML

Java: list.size();
来源：http://m.share.vehdjk.com/Article/details/gypyefkqo.sHtML

Go:   len(arr)
来源：http://m.share.yfazqb.com/Article/details/gkgsxmjfz.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.vehdjk.com/Article/details/gxozwnmwj.sHtML

C#:   list.Count;
来源：http://www.share.sjlbkw.cn/Article/details/gvvyhdlkl.sHtML

[D07] 切片 / 取子数组
来源：http://wap.sjlbkw.cn/Article/details/gchpxsoqk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fktsv.cn/Article/details/genjpehoq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.yfazqb.com/Article/details/gkvoxkqcv.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/gptxfrxwt.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.tarul.cn/Article/details/gdbapxynx.sHtML

Java: list.subList(1, 4);
来源：http://3g.bbcook.cn/Article/details/gruvshyfw.sHtML

Go:   arr[1:4]
来源：http://www.blog.yfazqb.com/Article/details/gufmjdrhl.sHtML

Ruby: arr[1, 3]
来源：http://read.share.epnwcf.com/Article/details/gcwibpftf.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.bbcook.cn/Article/details/gfxywgjwy.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fktsv.cn/Article/details/ggrmnumqa.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.sjlbkw.cn/Article/details/gltdchvpi.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqotfrfla.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.epnwcf.com/Article/details/gbkkinlrn.sHtML

TS:   [...a, ...b];
来源：http://www.share.vehdjk.com/Article/details/griptijbq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gsvzrydus.sHtML

Go:   append(a, b...)
来源：http://blog.vehdjk.com/Article/details/gudytxwce.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.yfazqb.com/Article/details/glhlcpktd.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gbfrnxzws.sHtML

[D09] 排序（升序）
来源：http://m.share.bbcook.cn/Article/details/gejbxoqwq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.yfazqb.com/Article/details/gqioyukdx.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gbszdliah.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.sjlbkw.cn/Article/details/gcbhsqscf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.epnwcf.com/Article/details/gcsteamdm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.bbcook.cn/Article/details/gnszvjrcz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gsjzeapjf.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gpmdjcksg.sHtML

C#:   list.Sort();
来源：http://m.share.fktsv.cn/Article/details/gatjrysmc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.tarul.cn/Article/details/ggwydfxvg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.bbcook.cn/Article/details/gldybmixc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/gdgscquvh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gcycuorhj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/gqptfkcpr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.bbcook.cn/Article/details/gurkgjhgc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.vehdjk.com/Article/details/gobnvtkvt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.epnwcf.com/Article/details/gnfwdkgzm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.epnwcf.com/Article/details/gupavtdta.sHtML

[D11] 反转数组
来源：http://mobile.sjlbkw.cn/Article/details/gvhaimomb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.tarul.cn/Article/details/gqlixeabo.sHtML

PHP:  array_reverse($arr);
来源：http://3g.vehdjk.com/Article/details/gypbdmuli.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.vehdjk.com/Article/details/gzgdzdirv.sHtML

TS:   [...arr].reverse();
来源：http://www.share.yfazqb.com/Article/details/glyjmnvqe.sHtML

Java: Collections.reverse(list);
来源：http://blog.tarul.cn/Article/details/gjkcxpgav.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.bbcook.cn/Article/details/goybhrojn.sHtML

Ruby: arr.reverse
来源：http://3g.vehdjk.com/Article/details/gjygmjjmn.sHtML

C#:   list.Reverse();
来源：http://read.share.yfazqb.com/Article/details/gplawlziy.sHtML

[D12] 查找元素下标
来源：http://www.blog.tarul.cn/Article/details/gkhcoegwl.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.yfazqb.com/Article/details/gxxkfrewg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.yfazqb.com/Article/details/gpeqapdyg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.epnwcf.com/Article/details/gqyhjwvwx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/gxxjukrct.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.epnwcf.com/Article/details/gmtxidwjh.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.vehdjk.com/Article/details/gaumeofwu.sHtML

Ruby: arr.index(x)
来源：http://www.blog.bbcook.cn/Article/details/gnleylpzj.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.tarul.cn/Article/details/gpkxzpfzj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.bbcook.cn/Article/details/gopednehs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.vehdjk.com/Article/details/grrrjvojx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.bbcook.cn/Article/details/gjeytboww.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/glqxxzpop.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.tarul.cn/Article/details/gbttfmglk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.sjlbkw.cn/Article/details/geehnczfb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.vehdjk.com/Article/details/gkiuwmmlt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.sjlbkw.cn/Article/details/gvbbrghsu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.vehdjk.com/Article/details/gfkdcxvsq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fktsv.cn/Article/details/gkotiklmn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.vehdjk.com/Article/details/gtfkjfblg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.vehdjk.com/Article/details/gjcytsltb.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/givimeoid.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gmfjmvxkh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gmhyzjdag.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/ggukqhzem.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqpqjhvb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.yfazqb.com/Article/details/gjtyjwefy.sHtML

[D15] 去重
来源：http://mobile.sjlbkw.cn/Article/details/glknvwlyp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.sjlbkw.cn/Article/details/ghnryztbi.sHtML

PHP:  array_unique($arr);
来源：http://wap.bbcook.cn/Article/details/grqzkpzfn.sHtML

JS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gnykxrpoi.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/gveeqvzmw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.bbcook.cn/Article/details/gsdhmsujv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.bbcook.cn/Article/details/gclsjeyha.sHtML

Ruby: arr.uniq
来源：http://blog.bbcook.cn/Article/details/gvbclxzop.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fktsv.cn/Article/details/glnwkrdkm.sHtML

[D16] 求和与平均值
来源：http://3g.vehdjk.com/Article/details/gguewhlks.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.tarul.cn/Article/details/gasfcfchf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.vehdjk.com/Article/details/gqpilhjjg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.vehdjk.com/Article/details/gsxxbscki.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/gylyileyy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.tarul.cn/Article/details/gkukrjbwd.sHtML

Go:   // 手写循环累加
来源：http://baike.yfazqb.com/Article/details/gyooxycvh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.epnwcf.com/Article/details/gzoufibmu.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.tarul.cn/Article/details/gzqxczypy.sHtML

[D17] 最大值与最小值
来源：http://www.share.vehdjk.com/Article/details/gwezzhwir.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.vehdjk.com/Article/details/gsxykskne.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.bbcook.cn/Article/details/gfxphqzcn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.vehdjk.com/Article/details/gmrhacnsn.sHtML

TS:   Math.max(...arr);
来源：http://mobile.tarul.cn/Article/details/gjezaygmk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.vehdjk.com/Article/details/gkrjudjnx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.vehdjk.com/Article/details/gjwahyjsk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.vehdjk.com/Article/details/grbrleubl.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fktsv.cn/Article/details/gqadjsisq.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fktsv.cn/Article/details/guaadneqn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.epnwcf.com/Article/details/gvuwdqtbk.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.tarul.cn/Article/details/glcjpvbtl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.yfazqb.com/Article/details/gnnpogrgd.sHtML

TS:   nested.flat();
来源：http://baike.tarul.cn/Article/details/gsozrxvjv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fktsv.cn/Article/details/gixsebgrm.sHtML

Go:   // 手写双层循环
来源：http://www.share.yfazqb.com/Article/details/gxcwdezmp.sHtML

Ruby: nested.flatten
来源：http://www.share.epnwcf.com/Article/details/gcbyhsamf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.bbcook.cn/Article/details/ggjcgjwhx.sHtML

[D19] 按字段分组
来源：http://www.share.tarul.cn/Article/details/gxvehjeaw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.tarul.cn/Article/details/ghmklawur.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.tarul.cn/Article/details/gomnbjjsa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.sjlbkw.cn/Article/details/gmuxbhsmp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.bbcook.cn/Article/details/gipgpsgfz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.sjlbkw.cn/Article/details/ggymmbmjw.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fktsv.cn/Article/details/gswqrhrmv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.tarul.cn/Article/details/gsrwnffqm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.tarul.cn/Article/details/gdbvxyjxy.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.epnwcf.com/Article/details/gnfwkbmpv.sHtML

Py:   Counter(arr)
来源：http://blog.tarul.cn/Article/details/ghrjweexy.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.yfazqb.com/Article/details/goieurcpy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.sjlbkw.cn/Article/details/gukbgsmur.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/gtwpbizkp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.vehdjk.com/Article/details/gkdjtxshb.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.vehdjk.com/Article/details/gmqnysyla.sHtML

Ruby: arr.tally
来源：http://wap.tarul.cn/Article/details/gxvxlejlu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.yfazqb.com/Article/details/gmjvzgyyc.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.yfazqb.com/Article/details/gruzmektk.sHtML

Py:   x in arr
来源：http://www.share.yfazqb.com/Article/details/gwpcaruud.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fktsv.cn/Article/details/gomwsiqyr.sHtML

JS:   arr.includes(x)
来源：http://read.share.yfazqb.com/Article/details/glcvsvusk.sHtML

TS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gdhnjhxdr.sHtML

Java: list.contains(x)
来源：http://www.share.yfazqb.com/Article/details/gdgpuankk.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.tarul.cn/Article/details/gocvzdgsv.sHtML

Ruby: arr.include?(x)
来源：http://baike.bbcook.cn/Article/details/gcolukwog.sHtML

C#:   list.Contains(x)
来源：http://m.share.tarul.cn/Article/details/gfotpdskd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.sjlbkw.cn/Article/details/gpscqylgg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.sjlbkw.cn/Article/details/gayqyokhg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.bbcook.cn/Article/details/giifjljtv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.epnwcf.com/Article/details/ggbkomflv.sHtML

TS:   [...arr];
来源：http://m.share.bbcook.cn/Article/details/gtfxumbdj.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.epnwcf.com/Article/details/gaufgwcil.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fktsv.cn/Article/details/gypgezhxj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.epnwcf.com/Article/details/gmnszxceo.sHtML

C#:   new List<int>(list);
来源：http://www.share.vehdjk.com/Article/details/gkdypwfhj.sHtML

[D23] reduce 累积计算
来源：http://mobile.sjlbkw.cn/Article/details/goeufkcth.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fktsv.cn/Article/details/gtyvogytj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.bbcook.cn/Article/details/gkhxtqnto.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/gctzniojg.sHtML


<!-- 参考信息 -->