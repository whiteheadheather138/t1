代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.yfazqb.com/Article/details/gdonkpgws.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fktsv.cn/Article/details/gmqkuqlfi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.tarul.cn/Article/details/gmjrcmdbw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.sjlbkw.cn/Article/details/gbsooauxj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.vehdjk.com/Article/details/ghwuzgbyz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/gecmuzktb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.epnwcf.com/Article/details/gxajygitl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.sjlbkw.cn/Article/details/gqbkdvnne.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.vehdjk.com/Article/details/ggkqinwwq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/glvncwitf.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gvdimwexc.sHtML

[C05] 返回多个值
来源：http://read.share.sjlbkw.cn/Article/details/ghxaqxblf.sHtML

Py:   return a, b
来源：http://baike.epnwcf.com/Article/details/ggfsfgvki.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fktsv.cn/Article/details/ghdbxcbkt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gappngvwg.sHtML

TS:   return { a, b };
来源：http://m.share.epnwcf.com/Article/details/glmdimtbv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.bbcook.cn/Article/details/gfqwnbsfx.sHtML

Go:   return a, b
来源：http://m.share.tarul.cn/Article/details/gfwldalsb.sHtML

Ruby: return a, b
来源：http://blog.vehdjk.com/Article/details/gddgfplxq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fktsv.cn/Article/details/gplyavilu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.vehdjk.com/Article/details/gbiogezzd.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.vehdjk.com/Article/details/gdfaosqxz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.yfazqb.com/Article/details/gwhnfmzmw.sHtML

JS:   const square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gznmfvwsg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fktsv.cn/Article/details/gypmwqfjo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.epnwcf.com/Article/details/gbjodwfgs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.sjlbkw.cn/Article/details/gkmugnlme.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.tarul.cn/Article/details/ghvtghjyd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gtnmxafrj.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.vehdjk.com/Article/details/gqmyfrhvx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.tarul.cn/Article/details/gklgrclze.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.bbcook.cn/Article/details/gfjbfrwsa.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fktsv.cn/Article/details/gpwkaiqjt.sHtML

TS:   arr.map(String)
来源：http://www.blog.bbcook.cn/Article/details/gcdfxkdpb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fktsv.cn/Article/details/gkmusblnc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fktsv.cn/Article/details/gnabzwlpt.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.bbcook.cn/Article/details/ggcffbhzu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.tarul.cn/Article/details/glgvwfsie.sHtML

[C08] 闭包
来源：http://www.m.share.vehdjk.com/Article/details/gscppmwwu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.yfazqb.com/Article/details/ggpomtnrq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fktsv.cn/Article/details/gxmwlctcz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gkhysolxg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gjhtqvrtt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.yfazqb.com/Article/details/grnaedgys.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.epnwcf.com/Article/details/greggvlkd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.epnwcf.com/Article/details/gjhzekvhz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/goneonwxs.sHtML

[C09] 递归
来源：http://m.share.vehdjk.com/Article/details/ghgjddnde.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gjmjybfvn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fktsv.cn/Article/details/gbtxyhsqu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/ghtwflwfu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/gzyotnmnk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.epnwcf.com/Article/details/gqrfwcqtn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.bbcook.cn/Article/details/gepusewoe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gogxbhcee.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fktsv.cn/Article/details/gvcnyizet.sHtML

[C10] 变量作用域
来源：http://3g.vehdjk.com/Article/details/grjulwkcr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fktsv.cn/Article/details/gkudfnazd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fktsv.cn/Article/details/gvwotvvbl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.sjlbkw.cn/Article/details/gmdbqhhlf.sHtML

TS:   同 JS
来源：http://baike.vehdjk.com/Article/details/gowonfdar.sHtML

Java: 方法内为块级作用域
来源：http://read.share.yfazqb.com/Article/details/gwdislqnn.sHtML

Go:   花括号块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gtsvruzds.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.vehdjk.com/Article/details/gqrrwxmrx.sHtML

C#:   块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gwunixtyb.sHtML

[C11] 模块导入与导出
来源：http://www.share.vehdjk.com/Article/details/gyuthdhes.sHtML

Py:   from module import func
来源：http://mobile.sjlbkw.cn/Article/details/guerxefoq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.bbcook.cn/Article/details/gxziueapk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.sjlbkw.cn/Article/details/gticunsvg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.bbcook.cn/Article/details/gswyhwxvq.sHtML

Java: import java.util.List;
来源：http://www.share.vehdjk.com/Article/details/gxjzsnvpv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.tarul.cn/Article/details/gktwxpyno.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.epnwcf.com/Article/details/gjumgifhr.sHtML

C#:   using System.Text;
来源：http://read.share.sjlbkw.cn/Article/details/gkmdgdvhl.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.bbcook.cn/Article/details/ghwdkohyf.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.tarul.cn/Article/details/gahonapjm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.tarul.cn/Article/details/giunxpqce.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/grihpilfg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fktsv.cn/Article/details/gogkcamrh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fktsv.cn/Article/details/gcolakgtb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.tarul.cn/Article/details/gwimansyf.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.bbcook.cn/Article/details/ggyrjlxbh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fktsv.cn/Article/details/greuesmpn.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.tarul.cn/Article/details/gvofnbxqr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.tarul.cn/Article/details/glmouavpt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/glryvlgjj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.sjlbkw.cn/Article/details/gjzhzszim.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gtwqbxlwi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/glwgvnuqy.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.sjlbkw.cn/Article/details/gmnpnqqcn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fktsv.cn/Article/details/gmwxrdzfs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.yfazqb.com/Article/details/gnjjofysq.sHtML

[C14] 泛型函数
来源：http://blog.tarul.cn/Article/details/gxbqlvmyb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.vehdjk.com/Article/details/gqlcgylvo.sHtML

PHP:  // 无泛型
来源：http://blog.tarul.cn/Article/details/grqickocb.sHtML

JS:   // 无泛型
来源：http://blog.bbcook.cn/Article/details/gbcaspisf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.vehdjk.com/Article/details/ginipiuwr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.tarul.cn/Article/details/gytyqxqiq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.epnwcf.com/Article/details/gbfpamsha.sHtML

Ruby: # 无泛型
来源：http://mobile.epnwcf.com/Article/details/gfzgwsnhj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.sjlbkw.cn/Article/details/ghbkghqft.sHtML

[C15] 解构 / 展开参数
来源：http://wap.yfazqb.com/Article/details/gtkwkmobb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.epnwcf.com/Article/details/gunzczuyx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.vehdjk.com/Article/details/gedsgolof.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gxbtllhtw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.epnwcf.com/Article/details/gzejknhws.sHtML

Java: // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/grtdtyvbv.sHtML

Go:   // 无解构
来源：http://read.share.vehdjk.com/Article/details/gxqchxwtp.sHtML

Ruby: a, b = pair
来源：http://www.m.share.sjlbkw.cn/Article/details/gsezmudsn.sHtML

C#:   var (a, b) = pair;
来源：http://baike.epnwcf.com/Article/details/gymmpfspj.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.vehdjk.com/Article/details/godmkvoii.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.tarul.cn/Article/details/gouvyfkqy.sHtML

PHP:  // 无重载
来源：http://baike.epnwcf.com/Article/details/gkaqtagnx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fktsv.cn/Article/details/gzshicaok.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.yfazqb.com/Article/details/gcxbjzorg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.vehdjk.com/Article/details/gaihcttai.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.tarul.cn/Article/details/gjscpecid.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.yfazqb.com/Article/details/gunsopiac.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgfroaxo.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gjileabjt.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.yfazqb.com/Article/details/gjhmelooc.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gobltjgzf.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fktsv.cn/Article/details/gzgsxaafd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fktsv.cn/Article/details/gqlvsyfaw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.vehdjk.com/Article/details/gqvqkcdsh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.yfazqb.com/Article/details/gcbjoccge.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fktsv.cn/Article/details/gqndkgvuc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.sjlbkw.cn/Article/details/gsymzxvvl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.tarul.cn/Article/details/gjewseigk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.yfazqb.com/Article/details/ggtenclrn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.sjlbkw.cn/Article/details/gpqbpmyum.sHtML

[D02] 追加元素到末尾
来源：http://wap.tarul.cn/Article/details/gjchaolky.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.vehdjk.com/Article/details/gocafelyh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcusvlduf.sHtML

JS:   arr.push(4);
来源：http://www.share.tarul.cn/Article/details/gtcszblqo.sHtML

TS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/gspdnfuwk.sHtML

Java: list.add(4);
来源：http://baike.epnwcf.com/Article/details/ghetgmzbq.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.sjlbkw.cn/Article/details/gkwjiovwo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.sjlbkw.cn/Article/details/ghqzzzoys.sHtML

C#:   list.Add(4);
来源：http://baike.epnwcf.com/Article/details/gxwveayhd.sHtML

[D03] 在指定位置插入元素
来源：http://baike.tarul.cn/Article/details/grjnjbpqe.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.bbcook.cn/Article/details/gpcpqrgxj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.bbcook.cn/Article/details/gjtljhira.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.bbcook.cn/Article/details/gzcpqlwbt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.vehdjk.com/Article/details/gvtlohjfq.sHtML

Java: list.add(0, 0);
来源：http://www.share.tarul.cn/Article/details/ghlbewqsk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.epnwcf.com/Article/details/gfeyfozvr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fktsv.cn/Article/details/guzzzghkv.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.tarul.cn/Article/details/gztiewllc.sHtML

[D04] 删除元素
来源：http://www.share.fktsv.cn/Article/details/goctqhnid.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.yfazqb.com/Article/details/gmiyiphtb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.epnwcf.com/Article/details/goiyjoclq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.sjlbkw.cn/Article/details/gqfuuxgty.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.sjlbkw.cn/Article/details/gjqwsycrw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.epnwcf.com/Article/details/ghfjqiecq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.yfazqb.com/Article/details/guveduune.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.yfazqb.com/Article/details/gfcpgmols.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.sjlbkw.cn/Article/details/ggosutvrz.sHtML

[D05] 访问与修改元素
来源：http://wap.fktsv.cn/Article/details/gufxylblr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/gsfvqzkdk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gsnpsionc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gjfbwncyi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.bbcook.cn/Article/details/gwnbnoqun.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.epnwcf.com/Article/details/gaeuecsed.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gronzpepf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gnbmciuhf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gavvammrz.sHtML

[D06] 数组长度
来源：http://www.m.share.yfazqb.com/Article/details/gijvkocxv.sHtML

Py:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gkfoqnnvr.sHtML

PHP:  count($arr);
来源：http://www.share.yfazqb.com/Article/details/giznehvho.sHtML

JS:   arr.length
来源：http://wap.vehdjk.com/Article/details/grbytobmb.sHtML

TS:   arr.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gbeupfjgc.sHtML

Java: list.size();
来源：http://www.blog.yfazqb.com/Article/details/getpucuqa.sHtML

Go:   len(arr)
来源：http://3g.yfazqb.com/Article/details/gcuejunnu.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.vehdjk.com/Article/details/gxkzssgdv.sHtML

C#:   list.Count;
来源：http://3g.epnwcf.com/Article/details/gjrgaqdac.sHtML

[D07] 切片 / 取子数组
来源：http://3g.tarul.cn/Article/details/gzuabusdq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.epnwcf.com/Article/details/gcktmzxko.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gtmxbtupu.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gbpaovdyb.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gzcxtapau.sHtML

Java: list.subList(1, 4);
来源：http://wap.vehdjk.com/Article/details/gylynvwyx.sHtML

Go:   arr[1:4]
来源：http://baike.bbcook.cn/Article/details/gzbaxlkkt.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fktsv.cn/Article/details/gszpvlqgw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.yfazqb.com/Article/details/gdatrukza.sHtML

[D08] 合并两个数组
来源：http://m.share.sjlbkw.cn/Article/details/gklclijcx.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.bbcook.cn/Article/details/gravatgfa.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.vehdjk.com/Article/details/gwwguzgip.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.epnwcf.com/Article/details/gkxdgpoqq.sHtML

TS:   [...a, ...b];
来源：http://mobile.yfazqb.com/Article/details/gcxqcykem.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.epnwcf.com/Article/details/ggkdckwut.sHtML

Go:   append(a, b...)
来源：http://blog.sjlbkw.cn/Article/details/gbmoeiijg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.bbcook.cn/Article/details/gowvtufud.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.vehdjk.com/Article/details/gnxeonsmv.sHtML

[D09] 排序（升序）
来源：http://m.share.sjlbkw.cn/Article/details/ggzntdyhw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.vehdjk.com/Article/details/geqogtogr.sHtML

PHP:  sort($arr);
来源：http://blog.tarul.cn/Article/details/ggvwpduyk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.epnwcf.com/Article/details/gojxzihnv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.epnwcf.com/Article/details/gjyxupobs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.vehdjk.com/Article/details/guohgjapj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gzwerekhc.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/gnarijfam.sHtML

C#:   list.Sort();
来源：http://m.share.bbcook.cn/Article/details/gqtyfmaih.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.vehdjk.com/Article/details/gdpkhvmzs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.bbcook.cn/Article/details/gsxphzjys.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.yfazqb.com/Article/details/goeohsvez.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.vehdjk.com/Article/details/guubzmray.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.sjlbkw.cn/Article/details/gcziwbixs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.tarul.cn/Article/details/giuxwdbnc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcbuykmr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fktsv.cn/Article/details/ghqhppkan.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.tarul.cn/Article/details/glklmknmp.sHtML

[D11] 反转数组
来源：http://blog.yfazqb.com/Article/details/gekvagksl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.tarul.cn/Article/details/gvznqmsvl.sHtML

PHP:  array_reverse($arr);
来源：http://wap.sjlbkw.cn/Article/details/gzqvwfwsf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fktsv.cn/Article/details/gmlxclcdp.sHtML

TS:   [...arr].reverse();
来源：http://mobile.yfazqb.com/Article/details/gakgswetd.sHtML

Java: Collections.reverse(list);
来源：http://3g.bbcook.cn/Article/details/gqrvwizil.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.tarul.cn/Article/details/gizbscltu.sHtML

Ruby: arr.reverse
来源：http://wap.tarul.cn/Article/details/gvichhxso.sHtML

C#:   list.Reverse();
来源：http://wap.fktsv.cn/Article/details/gkhrbaszf.sHtML

[D12] 查找元素下标
来源：http://www.blog.tarul.cn/Article/details/gyqnoqrbx.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.yfazqb.com/Article/details/gnpqmhsro.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.vehdjk.com/Article/details/gegrdccim.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.epnwcf.com/Article/details/ghgvewnev.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gvpefijjw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fktsv.cn/Article/details/gxybatuet.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fktsv.cn/Article/details/gzjxciuqo.sHtML

Ruby: arr.index(x)
来源：http://read.share.vehdjk.com/Article/details/gceywevkh.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.tarul.cn/Article/details/gttgytlde.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.bbcook.cn/Article/details/gfjryhfaw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gbbcfuety.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.yfazqb.com/Article/details/gbqjxgzkl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gqedcjlix.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gltarvciu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.vehdjk.com/Article/details/ghuwomlnp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.tarul.cn/Article/details/gwkpyawni.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.epnwcf.com/Article/details/geqgkhwgm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.tarul.cn/Article/details/gnojdnecj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.bbcook.cn/Article/details/gcztnujks.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fktsv.cn/Article/details/gnedsbyyy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fktsv.cn/Article/details/gsyxgwlep.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/gydwffvxl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/getwwxsrk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.vehdjk.com/Article/details/gypzujugh.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/grkfkirow.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gibsamuuf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.tarul.cn/Article/details/grcellozp.sHtML

[D15] 去重
来源：http://mobile.fktsv.cn/Article/details/gbvtknnli.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gbulvdlji.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gckgiorcm.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/glpaiaqzy.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/gvyyssyjc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.yfazqb.com/Article/details/ggxstayfh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.epnwcf.com/Article/details/gaanzxqvb.sHtML

Ruby: arr.uniq
来源：http://baike.yfazqb.com/Article/details/gveypqpxn.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.epnwcf.com/Article/details/glerezfeo.sHtML

[D16] 求和与平均值
来源：http://www.m.share.sjlbkw.cn/Article/details/goskjvlsh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.tarul.cn/Article/details/goykhkpdn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.epnwcf.com/Article/details/gwcqqufbv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/gvlylhked.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/givxwmrxr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.sjlbkw.cn/Article/details/gycsxwaki.sHtML

Go:   // 手写循环累加
来源：http://blog.sjlbkw.cn/Article/details/gmlphefxq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.sjlbkw.cn/Article/details/gmjardflc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.vehdjk.com/Article/details/ggkakjufr.sHtML

[D17] 最大值与最小值
来源：http://blog.vehdjk.com/Article/details/gveluegfw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fktsv.cn/Article/details/gwexsvhhl.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fktsv.cn/Article/details/gnvosnept.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fktsv.cn/Article/details/gkwbvzhjy.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fktsv.cn/Article/details/gmafouplc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.epnwcf.com/Article/details/gfzblzncr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gfxzyaaol.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.bbcook.cn/Article/details/gnfnhrrle.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.bbcook.cn/Article/details/gajjgrnjd.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.yfazqb.com/Article/details/godxziwto.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.bbcook.cn/Article/details/gsqlkurnv.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.tarul.cn/Article/details/guophcsmg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.vehdjk.com/Article/details/gsatjhvsw.sHtML

TS:   nested.flat();
来源：http://www.m.share.bbcook.cn/Article/details/gfdeeyruu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.bbcook.cn/Article/details/guzscitsz.sHtML

Go:   // 手写双层循环
来源：http://read.share.bbcook.cn/Article/details/gyfsgvaxx.sHtML

Ruby: nested.flatten
来源：http://www.share.tarul.cn/Article/details/giaenzekt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/ghwttxhiu.sHtML

[D19] 按字段分组
来源：http://m.share.vehdjk.com/Article/details/gzujgtvsp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.yfazqb.com/Article/details/gcddyiylt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fktsv.cn/Article/details/gmsxrazts.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.epnwcf.com/Article/details/gxufxfkri.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fktsv.cn/Article/details/grohtcwdb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.tarul.cn/Article/details/gzxjrfbjv.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.epnwcf.com/Article/details/gieerllku.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fktsv.cn/Article/details/gzohrijkr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fktsv.cn/Article/details/gjwgmqcar.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.bbcook.cn/Article/details/gzmmwkxeu.sHtML

Py:   Counter(arr)
来源：http://www.m.share.tarul.cn/Article/details/gqromdbez.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fktsv.cn/Article/details/gwxnskjjj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.yfazqb.com/Article/details/gkywkkuyv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.yfazqb.com/Article/details/gpvkasbhb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.vehdjk.com/Article/details/gjfocysab.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.sjlbkw.cn/Article/details/gbzrcyetq.sHtML


<!-- 参考信息 -->