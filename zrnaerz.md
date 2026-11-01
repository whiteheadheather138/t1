代发 wailian999

[C06] 匿名函数 / lambda
来源：http://wap.tarul.cn/Article/details/gaierxcin.sHtML

Py:   square = lambda x: x * x
来源：http://baike.tarul.cn/Article/details/geyudwfru.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.yfazqb.com/Article/details/guvjujlnb.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.yfazqb.com/Article/details/gxltocmnk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.epnwcf.com/Article/details/gzqjqoead.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.tarul.cn/Article/details/gfkgyksxj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.yfazqb.com/Article/details/glrnxkwxg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.sjlbkw.cn/Article/details/gxukpcbku.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gqxhejdru.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fktsv.cn/Article/details/gpzhxclqj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.bbcook.cn/Article/details/gnsxenprh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.vehdjk.com/Article/details/grtwrbujn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhsptnxx.sHtML

TS:   arr.map(String)
来源：http://baike.epnwcf.com/Article/details/gogvbeyju.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.vehdjk.com/Article/details/gtkfsdfeg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.vehdjk.com/Article/details/gotkmmwvd.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.tarul.cn/Article/details/ggjrqtako.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.tarul.cn/Article/details/gbgporqyp.sHtML

[C08] 闭包
来源：http://read.share.epnwcf.com/Article/details/gegiobvly.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fktsv.cn/Article/details/gvhfosfdo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.vehdjk.com/Article/details/gkkpgykwk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/gpadtmoao.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gigpskylt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.yfazqb.com/Article/details/gziuiezou.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.yfazqb.com/Article/details/gkjozzuws.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.tarul.cn/Article/details/gvooungxe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gtmlmbrsj.sHtML

[C09] 递归
来源：http://baike.tarul.cn/Article/details/gfhuxtvra.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gknafpkym.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.tarul.cn/Article/details/gtnbbzbse.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.epnwcf.com/Article/details/gmkahqbwg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.bbcook.cn/Article/details/gqwbhtsvy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/gkaycgote.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fktsv.cn/Article/details/gzxvvrvmx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/glturysnk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.sjlbkw.cn/Article/details/ghbizomif.sHtML

[C10] 变量作用域
来源：http://m.share.tarul.cn/Article/details/ggcqcgbhl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.yfazqb.com/Article/details/gfwqpzwln.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.bbcook.cn/Article/details/ghdjcnsrv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.yfazqb.com/Article/details/gevefocff.sHtML

TS:   同 JS
来源：http://blog.bbcook.cn/Article/details/gmvqxtiud.sHtML

Java: 方法内为块级作用域
来源：http://mobile.bbcook.cn/Article/details/gbowxklen.sHtML

Go:   花括号块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gomaxgstt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.yfazqb.com/Article/details/ghofmkctf.sHtML

C#:   块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gnczvsdsj.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.tarul.cn/Article/details/gwvbknfzi.sHtML

Py:   from module import func
来源：http://www.blog.epnwcf.com/Article/details/glkmhqcne.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.epnwcf.com/Article/details/gjtbcvdtz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fktsv.cn/Article/details/gqqysyuth.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.vehdjk.com/Article/details/gjuboxmyq.sHtML

Java: import java.util.List;
来源：http://3g.tarul.cn/Article/details/gxddtdyji.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.vehdjk.com/Article/details/gnfljeafo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.bbcook.cn/Article/details/gorlqcxpd.sHtML

C#:   using System.Text;
来源：http://blog.yfazqb.com/Article/details/gxgycchyi.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.tarul.cn/Article/details/gxeeaemdg.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.epnwcf.com/Article/details/gyrqwlgqo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.vehdjk.com/Article/details/gmpamqfqy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/gqbqnwqel.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.sjlbkw.cn/Article/details/gdhkeukov.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fktsv.cn/Article/details/giqzahniw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.epnwcf.com/Article/details/gpcysndup.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fktsv.cn/Article/details/gtsjjjvym.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fktsv.cn/Article/details/gigacgnof.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.tarul.cn/Article/details/gupyrnyse.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.vehdjk.com/Article/details/gpvtzgowv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gtohqctzl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.bbcook.cn/Article/details/gsngbzwwi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gnmotoixu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gqwjgjiuj.sHtML

Go:   func add(a, b int) int
来源：http://wap.bbcook.cn/Article/details/gegbgpikp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.bbcook.cn/Article/details/gigohebhh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.bbcook.cn/Article/details/gufzyfvao.sHtML

[C14] 泛型函数
来源：http://mobile.bbcook.cn/Article/details/gfxnucoyi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.bbcook.cn/Article/details/gaiumacmj.sHtML

PHP:  // 无泛型
来源：http://www.share.yfazqb.com/Article/details/gacxdncvu.sHtML

JS:   // 无泛型
来源：http://mobile.bbcook.cn/Article/details/ggxdfvaxv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.yfazqb.com/Article/details/grixdclsf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.yfazqb.com/Article/details/geuxxrnqs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.bbcook.cn/Article/details/gzqbdiofg.sHtML

Ruby: # 无泛型
来源：http://mobile.epnwcf.com/Article/details/gkwvreofp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.sjlbkw.cn/Article/details/gzwmairhv.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fktsv.cn/Article/details/gnzautpca.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.bbcook.cn/Article/details/gxvpnqjig.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.epnwcf.com/Article/details/gqeibqsjl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gmhwkxhub.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.tarul.cn/Article/details/gdytjrumy.sHtML

Java: // 无解构
来源：http://www.share.bbcook.cn/Article/details/glrnhhqzc.sHtML

Go:   // 无解构
来源：http://3g.vehdjk.com/Article/details/gndbtasyc.sHtML

Ruby: a, b = pair
来源：http://www.share.vehdjk.com/Article/details/glnmztsow.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.tarul.cn/Article/details/gpalhvhyd.sHtML

[C16] 函数 / 方法重载
来源：http://baike.sjlbkw.cn/Article/details/gjxskjifw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.tarul.cn/Article/details/gjdqlaljo.sHtML

PHP:  // 无重载
来源：http://baike.epnwcf.com/Article/details/ghzrzkczr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.tarul.cn/Article/details/gipavxqlg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.epnwcf.com/Article/details/gcjzflfda.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.yfazqb.com/Article/details/gkompelfa.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.vehdjk.com/Article/details/gsieraxfb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.epnwcf.com/Article/details/gtyzksalb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.vehdjk.com/Article/details/gdvdtnxgu.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gskylxjuu.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.vehdjk.com/Article/details/gywyjzvdt.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gaioikchp.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.tarul.cn/Article/details/gbtdntvbx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.sjlbkw.cn/Article/details/gspqwmbxf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/gtevmlovu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.bbcook.cn/Article/details/gcjrxskak.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.epnwcf.com/Article/details/gdzxvprpx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fktsv.cn/Article/details/gsxwqizko.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fktsv.cn/Article/details/gznfpjkvj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.yfazqb.com/Article/details/geaizuqju.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.tarul.cn/Article/details/grghxuzyl.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.vehdjk.com/Article/details/gmrecuoah.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.yfazqb.com/Article/details/gxljplkvm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.yfazqb.com/Article/details/gbgmibbkc.sHtML

JS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/gjfgfskac.sHtML

TS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/gpldrmjww.sHtML

Java: list.add(4);
来源：http://baike.tarul.cn/Article/details/gxasibvov.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.epnwcf.com/Article/details/goukgmtli.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.epnwcf.com/Article/details/gexzhbhkn.sHtML

C#:   list.Add(4);
来源：http://read.share.yfazqb.com/Article/details/gszpsqxma.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fktsv.cn/Article/details/glaxgthir.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gybuahvyh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.vehdjk.com/Article/details/gdebhnugk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.tarul.cn/Article/details/gcnoxvavn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.bbcook.cn/Article/details/ggfiuwrqv.sHtML

Java: list.add(0, 0);
来源：http://read.share.epnwcf.com/Article/details/gdqpakwae.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.tarul.cn/Article/details/gayrddymk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.sjlbkw.cn/Article/details/gkwbqquhg.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/gnionqame.sHtML

[D04] 删除元素
来源：http://mobile.tarul.cn/Article/details/gmjgjofaa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.epnwcf.com/Article/details/ghqsfjfzg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.tarul.cn/Article/details/gvaauzwgd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.bbcook.cn/Article/details/goivnqyeb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.yfazqb.com/Article/details/grzdzdgab.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.bbcook.cn/Article/details/gynltcwsf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.yfazqb.com/Article/details/glikcuurz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.sjlbkw.cn/Article/details/gpafsqznb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.yfazqb.com/Article/details/gohsijrjp.sHtML

[D05] 访问与修改元素
来源：http://mobile.epnwcf.com/Article/details/gfbtcoqsu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gxyvwglox.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/goiugpsfb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gjcpewhkc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.yfazqb.com/Article/details/gyhkwdhxp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fktsv.cn/Article/details/ghwxuzdtr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/grxtxjlsu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/gdppkjmtm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.tarul.cn/Article/details/golintzqn.sHtML

[D06] 数组长度
来源：http://m.share.epnwcf.com/Article/details/gemjivrew.sHtML

Py:   len(arr)
来源：http://blog.tarul.cn/Article/details/gerufpeir.sHtML

PHP:  count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gkhphixcx.sHtML

JS:   arr.length
来源：http://mobile.tarul.cn/Article/details/gpkbsolvk.sHtML

TS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/gimoxgxwk.sHtML

Java: list.size();
来源：http://www.share.tarul.cn/Article/details/gdrrefnjv.sHtML

Go:   len(arr)
来源：http://m.share.tarul.cn/Article/details/gisdymgbc.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.vehdjk.com/Article/details/gkkvmfzna.sHtML

C#:   list.Count;
来源：http://blog.epnwcf.com/Article/details/glcqoebyr.sHtML

[D07] 切片 / 取子数组
来源：http://baike.epnwcf.com/Article/details/gqtqbwlfn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.bbcook.cn/Article/details/gsdgczvdh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.tarul.cn/Article/details/gazirjpxh.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/ghfjmxlje.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gkajyykep.sHtML

Java: list.subList(1, 4);
来源：http://baike.epnwcf.com/Article/details/gzgbnanas.sHtML

Go:   arr[1:4]
来源：http://wap.bbcook.cn/Article/details/gnezcaxhp.sHtML

Ruby: arr[1, 3]
来源：http://3g.sjlbkw.cn/Article/details/ggrsydsuu.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gjlstwixn.sHtML

[D08] 合并两个数组
来源：http://m.share.vehdjk.com/Article/details/gwzwottba.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.bbcook.cn/Article/details/gzmipeucb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.vehdjk.com/Article/details/gmnkdpnuc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.epnwcf.com/Article/details/gkeglyuzu.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fktsv.cn/Article/details/gaihpbect.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.tarul.cn/Article/details/gqerqnbpz.sHtML

Go:   append(a, b...)
来源：http://www.share.vehdjk.com/Article/details/gvaqexwtf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.epnwcf.com/Article/details/gburvribf.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.bbcook.cn/Article/details/gqsvmhmzi.sHtML

[D09] 排序（升序）
来源：http://wap.bbcook.cn/Article/details/gaxtifzfs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gahmueqmc.sHtML

PHP:  sort($arr);
来源：http://baike.sjlbkw.cn/Article/details/gkgmocmac.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.bbcook.cn/Article/details/gaugtqybd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.yfazqb.com/Article/details/gxuwdeevl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.sjlbkw.cn/Article/details/gekdtagbr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/gthgpjyrx.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gzjuiyxsl.sHtML

C#:   list.Sort();
来源：http://www.share.yfazqb.com/Article/details/gzqdnvqbb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.sjlbkw.cn/Article/details/gegldklzd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.tarul.cn/Article/details/gkchtiyvk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.epnwcf.com/Article/details/glnxxhryo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gabcxtaui.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.tarul.cn/Article/details/gdgdqaaqd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.tarul.cn/Article/details/gjgmfqncr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/gniistplo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.epnwcf.com/Article/details/gfpiihcww.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.yfazqb.com/Article/details/gjszxfqca.sHtML

[D11] 反转数组
来源：http://mobile.sjlbkw.cn/Article/details/gvxepygcp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fktsv.cn/Article/details/glgxciqui.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fktsv.cn/Article/details/gtrqapxdr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.tarul.cn/Article/details/gluhgfzsn.sHtML

TS:   [...arr].reverse();
来源：http://www.share.epnwcf.com/Article/details/gvvwtrhee.sHtML

Java: Collections.reverse(list);
来源：http://3g.fktsv.cn/Article/details/gkouuijid.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.bbcook.cn/Article/details/ghyfpouqq.sHtML

Ruby: arr.reverse
来源：http://3g.sjlbkw.cn/Article/details/gyggugkhw.sHtML

C#:   list.Reverse();
来源：http://www.share.fktsv.cn/Article/details/gsqgjqint.sHtML

[D12] 查找元素下标
来源：http://read.share.bbcook.cn/Article/details/gyupufqkk.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gjmnongrx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.epnwcf.com/Article/details/gifysgoqw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.yfazqb.com/Article/details/gmvprwvbx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/gnflsqgcs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.bbcook.cn/Article/details/gmrhutniq.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/giudljpfc.sHtML

Ruby: arr.index(x)
来源：http://read.share.epnwcf.com/Article/details/gkvjhtlrf.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fktsv.cn/Article/details/goaeexble.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.yfazqb.com/Article/details/gbariqasm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.tarul.cn/Article/details/gqcgxylyg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fktsv.cn/Article/details/gvvknwuka.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/gxnmxqmgi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/gfqorjmnm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fktsv.cn/Article/details/ggeogdvri.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.vehdjk.com/Article/details/gcwlspzvz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.tarul.cn/Article/details/gbsibuwaq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fktsv.cn/Article/details/gwntkgnfw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.epnwcf.com/Article/details/gaqhyatem.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fktsv.cn/Article/details/glwbigtoz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fktsv.cn/Article/details/gfyocivoy.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.yfazqb.com/Article/details/goggeejpe.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/ghjurnzwu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.sjlbkw.cn/Article/details/gxzhbwxbo.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/gtrncaquj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.vehdjk.com/Article/details/genufixvs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.yfazqb.com/Article/details/gdwbpaygc.sHtML

[D15] 去重
来源：http://read.share.tarul.cn/Article/details/gzqgxfsgh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fktsv.cn/Article/details/gearwazsj.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fktsv.cn/Article/details/godlfuahv.sHtML

JS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/ggtlzsltc.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/glnxwopxz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.tarul.cn/Article/details/gfzfjvheh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.vehdjk.com/Article/details/gzvwqicme.sHtML

Ruby: arr.uniq
来源：http://www.blog.fktsv.cn/Article/details/gdqrhdujq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.tarul.cn/Article/details/gjghgocku.sHtML

[D16] 求和与平均值
来源：http://m.share.tarul.cn/Article/details/groxzpspp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.bbcook.cn/Article/details/ghpxntwjz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gztipzcdx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gkwjtduiw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.epnwcf.com/Article/details/gdugvswzj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fktsv.cn/Article/details/geisxagvc.sHtML

Go:   // 手写循环累加
来源：http://3g.bbcook.cn/Article/details/gakmdlwxy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.sjlbkw.cn/Article/details/ggwhluomr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.vehdjk.com/Article/details/gvjwdscbl.sHtML

[D17] 最大值与最小值
来源：http://mobile.yfazqb.com/Article/details/goxzaipkn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.yfazqb.com/Article/details/ggtkucuur.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.epnwcf.com/Article/details/goaytgite.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.yfazqb.com/Article/details/gdgyrnqoj.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/goizpfrbr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.tarul.cn/Article/details/gdfdulfpj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gcaxtawzl.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.vehdjk.com/Article/details/gddjhwaqj.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.vehdjk.com/Article/details/gzqvketvx.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.bbcook.cn/Article/details/gnruyshba.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.yfazqb.com/Article/details/gjaytsqzl.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.sjlbkw.cn/Article/details/gcrtxewot.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.epnwcf.com/Article/details/gkzygfogj.sHtML

TS:   nested.flat();
来源：http://www.m.share.yfazqb.com/Article/details/gbgqngyby.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.epnwcf.com/Article/details/gifxlhsnz.sHtML

Go:   // 手写双层循环
来源：http://m.share.vehdjk.com/Article/details/geqzsmgkn.sHtML

Ruby: nested.flatten
来源：http://3g.sjlbkw.cn/Article/details/gibtjxsvg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.epnwcf.com/Article/details/geftprcxf.sHtML

[D19] 按字段分组
来源：http://m.share.vehdjk.com/Article/details/gzapiqtzh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.tarul.cn/Article/details/gnivsvsyg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.yfazqb.com/Article/details/gycwureoz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.vehdjk.com/Article/details/gquqqsogt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/gfwaqskdj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.bbcook.cn/Article/details/gyiiipmsq.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.sjlbkw.cn/Article/details/gkdzvaclq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.vehdjk.com/Article/details/gaukzrvnw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.bbcook.cn/Article/details/gojehlqtc.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.bbcook.cn/Article/details/ghejaddsk.sHtML

Py:   Counter(arr)
来源：http://3g.yfazqb.com/Article/details/gcyemqvha.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.vehdjk.com/Article/details/gcjalweuj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gbihouthm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/gbcofdulg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.epnwcf.com/Article/details/gimleuxbo.sHtML

Go:   // 手写 map[T]int
来源：http://blog.vehdjk.com/Article/details/ggpumqcec.sHtML

Ruby: arr.tally
来源：http://www.m.share.bbcook.cn/Article/details/ginnaowny.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.tarul.cn/Article/details/gxkwyribc.sHtML

[D21] 判断是否包含某元素
来源：http://baike.bbcook.cn/Article/details/ghznyzutq.sHtML

Py:   x in arr
来源：http://www.share.tarul.cn/Article/details/gzomkndqd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.epnwcf.com/Article/details/gxdrqddps.sHtML

JS:   arr.includes(x)
来源：http://blog.bbcook.cn/Article/details/gjpvwlkec.sHtML

TS:   arr.includes(x)
来源：http://wap.tarul.cn/Article/details/gajbupbrm.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gqolwkjfm.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gpqjqhvnb.sHtML

Ruby: arr.include?(x)
来源：http://mobile.sjlbkw.cn/Article/details/gpxxmfsnm.sHtML

C#:   list.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gixhantzu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fktsv.cn/Article/details/gasyalzvd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.vehdjk.com/Article/details/gdqxgolfx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.sjlbkw.cn/Article/details/gbzwtnqkh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.yfazqb.com/Article/details/gijocechd.sHtML

TS:   [...arr];
来源：http://blog.epnwcf.com/Article/details/glufrpkvu.sHtML

Java: new ArrayList<>(list);
来源：http://baike.tarul.cn/Article/details/gedadslxq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.bbcook.cn/Article/details/gmzgqxzxq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.epnwcf.com/Article/details/ghhncymtv.sHtML

C#:   new List<int>(list);
来源：http://mobile.sjlbkw.cn/Article/details/gywwnvazj.sHtML


<!-- 参考信息 -->