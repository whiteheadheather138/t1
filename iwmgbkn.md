代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.sjlbkw.cn/Article/details/gkdwwvbhg.sHtML

TS:   arr.map(String)
来源：http://baike.sjlbkw.cn/Article/details/gklmipxjf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gyvuwrfgk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fktsv.cn/Article/details/gvugkpisq.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.sjlbkw.cn/Article/details/gnpfxvxst.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fktsv.cn/Article/details/gztlcgvxy.sHtML

[C08] 闭包
来源：http://m.share.fktsv.cn/Article/details/ggqzdgwwx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.yfazqb.com/Article/details/gvjzfruyj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.epnwcf.com/Article/details/gnhebgoyt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gouygzxtz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gogbotqgj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.tarul.cn/Article/details/gajkawcwv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.sjlbkw.cn/Article/details/glfcfkhbp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.sjlbkw.cn/Article/details/geoefobbg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/gvocunxlc.sHtML

[C09] 递归
来源：http://mobile.bbcook.cn/Article/details/giaunheep.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.epnwcf.com/Article/details/gpzjjjbze.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.tarul.cn/Article/details/gafmejbgn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.bbcook.cn/Article/details/gzjtvxwth.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.bbcook.cn/Article/details/gelpctira.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.bbcook.cn/Article/details/gqfxswtje.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.yfazqb.com/Article/details/gtrekxunt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.vehdjk.com/Article/details/gceseqcnk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.bbcook.cn/Article/details/gopjdwgsg.sHtML

[C10] 变量作用域
来源：http://baike.yfazqb.com/Article/details/ggakovgbr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.vehdjk.com/Article/details/gtotnhawr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/gbafawdol.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.bbcook.cn/Article/details/gnsmcawol.sHtML

TS:   同 JS
来源：http://baike.bbcook.cn/Article/details/gukjvyyxu.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fktsv.cn/Article/details/gwsvexioc.sHtML

Go:   花括号块级作用域
来源：http://mobile.fktsv.cn/Article/details/gokzgdbfe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.bbcook.cn/Article/details/gxghoozdy.sHtML

C#:   块级作用域
来源：http://3g.tarul.cn/Article/details/gdqwvldsz.sHtML

[C11] 模块导入与导出
来源：http://wap.epnwcf.com/Article/details/gytndwvxz.sHtML

Py:   from module import func
来源：http://wap.tarul.cn/Article/details/gpfnxjygv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.vehdjk.com/Article/details/gzaugicqn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.epnwcf.com/Article/details/gghzgwsrc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.tarul.cn/Article/details/gvaxjmhus.sHtML

Java: import java.util.List;
来源：http://www.blog.bbcook.cn/Article/details/guaqelatp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.sjlbkw.cn/Article/details/gubwfadyv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.bbcook.cn/Article/details/gmkxrjnol.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gbheccbso.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.yfazqb.com/Article/details/gpaakpwdb.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.vehdjk.com/Article/details/gbkdjaxjo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.epnwcf.com/Article/details/gmxxkkxow.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/gxibiloqc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gdezbdwit.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.epnwcf.com/Article/details/gbnxloeib.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fktsv.cn/Article/details/gpdcknapj.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.sjlbkw.cn/Article/details/gfzvoizjy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.tarul.cn/Article/details/gijxfdano.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvofxcgs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.epnwcf.com/Article/details/goieauari.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gmqimrfwj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.yfazqb.com/Article/details/gobucezxb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gsarkqrsr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gbqgoiwgw.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.yfazqb.com/Article/details/ggtwkrjsy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.sjlbkw.cn/Article/details/gtnwibqmb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.epnwcf.com/Article/details/gjdhvpcik.sHtML

[C14] 泛型函数
来源：http://baike.tarul.cn/Article/details/ghboafbfj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.sjlbkw.cn/Article/details/gdjpilwjz.sHtML

PHP:  // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gdogxtmgv.sHtML

JS:   // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gnvdtjfpw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.vehdjk.com/Article/details/gwwfnsckq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.vehdjk.com/Article/details/grqvryatn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fktsv.cn/Article/details/gphalgnmn.sHtML

Ruby: # 无泛型
来源：http://read.share.yfazqb.com/Article/details/gbfitastb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.epnwcf.com/Article/details/gifvncjjx.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.bbcook.cn/Article/details/glzdkccku.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.epnwcf.com/Article/details/gzjistzvr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.tarul.cn/Article/details/gaxpxjmqv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/gxkvkirnz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.epnwcf.com/Article/details/gbbpowkls.sHtML

Java: // 无解构
来源：http://mobile.vehdjk.com/Article/details/ghtwanooa.sHtML

Go:   // 无解构
来源：http://blog.sjlbkw.cn/Article/details/gsdvxqysj.sHtML

Ruby: a, b = pair
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuvryiyw.sHtML

C#:   var (a, b) = pair;
来源：http://wap.vehdjk.com/Article/details/gumkmpoei.sHtML

[C16] 函数 / 方法重载
来源：http://blog.sjlbkw.cn/Article/details/gkajjyetk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.bbcook.cn/Article/details/gollwfngc.sHtML

PHP:  // 无重载
来源：http://mobile.tarul.cn/Article/details/gkapfogvg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.vehdjk.com/Article/details/gcxsmhoae.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.vehdjk.com/Article/details/gshdqzwgt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fktsv.cn/Article/details/gjiecurpl.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.sjlbkw.cn/Article/details/gqxigboot.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.bbcook.cn/Article/details/gumzkhwnt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fktsv.cn/Article/details/ghjzvhnwp.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/glrspjwid.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.bbcook.cn/Article/details/ghlrziqcz.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqigkmcuf.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gwezvtvei.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.epnwcf.com/Article/details/giqdvllbg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.bbcook.cn/Article/details/gcmkgyqwl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.yfazqb.com/Article/details/gdrfvvfpv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.vehdjk.com/Article/details/gapxbtzet.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.vehdjk.com/Article/details/gqqesdlag.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.epnwcf.com/Article/details/gywwlbidi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.yfazqb.com/Article/details/gdzndmgji.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.sjlbkw.cn/Article/details/gargvhcho.sHtML

[D02] 追加元素到末尾
来源：http://3g.fktsv.cn/Article/details/gkbsfthta.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.yfazqb.com/Article/details/gmvzvcwzr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.tarul.cn/Article/details/givodijui.sHtML

JS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/gyumbcprd.sHtML

TS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/gpfrwrldf.sHtML

Java: list.add(4);
来源：http://www.share.sjlbkw.cn/Article/details/gkpfytswl.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fktsv.cn/Article/details/gycgiisnq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fktsv.cn/Article/details/gmcorlnnm.sHtML

C#:   list.Add(4);
来源：http://wap.sjlbkw.cn/Article/details/guavvcelg.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fktsv.cn/Article/details/gsgxinilu.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.tarul.cn/Article/details/glcwegypg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.sjlbkw.cn/Article/details/gigyfdnqu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.epnwcf.com/Article/details/gaubhabqc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwydgxpf.sHtML

Java: list.add(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gzwuqekpk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.bbcook.cn/Article/details/gvpusoadb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.tarul.cn/Article/details/ghtpuwnwc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.epnwcf.com/Article/details/gnzyorzag.sHtML

[D04] 删除元素
来源：http://mobile.epnwcf.com/Article/details/grgmhthfn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fktsv.cn/Article/details/gihhjvyet.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.yfazqb.com/Article/details/gimeyjxkq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.tarul.cn/Article/details/gnofbhhzw.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.sjlbkw.cn/Article/details/gnhiihqgx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.bbcook.cn/Article/details/gipkdeddv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.bbcook.cn/Article/details/gkfzfplee.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.sjlbkw.cn/Article/details/ggmwhsnnc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fktsv.cn/Article/details/glheathaa.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fktsv.cn/Article/details/gbwljzggg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gtobiibip.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gpujqmxum.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/ggpvjdrzb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.sjlbkw.cn/Article/details/ghaaueqqf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.yfazqb.com/Article/details/gadpfiwua.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gmitpiqjc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gutjnsbkq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gyipjfjlv.sHtML

[D06] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gypcfoxlt.sHtML

Py:   len(arr)
来源：http://baike.yfazqb.com/Article/details/gmrbthijn.sHtML

PHP:  count($arr);
来源：http://m.share.vehdjk.com/Article/details/gthzzfiqv.sHtML

JS:   arr.length
来源：http://mobile.yfazqb.com/Article/details/guphrwdwa.sHtML

TS:   arr.length
来源：http://mobile.yfazqb.com/Article/details/gycbvnenr.sHtML

Java: list.size();
来源：http://wap.tarul.cn/Article/details/glwvobwno.sHtML

Go:   len(arr)
来源：http://3g.epnwcf.com/Article/details/gxuthxhwp.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.vehdjk.com/Article/details/gtnmnhqbp.sHtML

C#:   list.Count;
来源：http://mobile.tarul.cn/Article/details/gmsmqfriw.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fktsv.cn/Article/details/gjeiieiam.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.sjlbkw.cn/Article/details/gohobkiav.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gqjaqphwu.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/gkqyemzln.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gtpcfufcz.sHtML

Java: list.subList(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gqcaznkni.sHtML

Go:   arr[1:4]
来源：http://www.m.share.yfazqb.com/Article/details/gkuvwvssu.sHtML

Ruby: arr[1, 3]
来源：http://m.share.yfazqb.com/Article/details/geixtkpzf.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.sjlbkw.cn/Article/details/gtvpuyast.sHtML

[D08] 合并两个数组
来源：http://baike.epnwcf.com/Article/details/gohzemlxt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fktsv.cn/Article/details/grctfetma.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.epnwcf.com/Article/details/grznbpblg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.epnwcf.com/Article/details/gzinbtsfb.sHtML

TS:   [...a, ...b];
来源：http://wap.sjlbkw.cn/Article/details/gkivbwqgd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fktsv.cn/Article/details/gswyqyyon.sHtML

Go:   append(a, b...)
来源：http://mobile.sjlbkw.cn/Article/details/ghlcaikqb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.yfazqb.com/Article/details/gkmsjuipr.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.bbcook.cn/Article/details/gnnwyhgea.sHtML

[D09] 排序（升序）
来源：http://www.blog.fktsv.cn/Article/details/gphijkenr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/gdcnqyipn.sHtML

PHP:  sort($arr);
来源：http://www.blog.yfazqb.com/Article/details/gwbajnqzz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fktsv.cn/Article/details/gobtwfjkm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.sjlbkw.cn/Article/details/giybzbvbw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fktsv.cn/Article/details/gahngtqtj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gwqjxsuqt.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gicujnppf.sHtML

C#:   list.Sort();
来源：http://www.blog.yfazqb.com/Article/details/gyimdyzbd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.epnwcf.com/Article/details/gixovfblk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.tarul.cn/Article/details/gllylotzp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.tarul.cn/Article/details/gwyzjpbku.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.sjlbkw.cn/Article/details/gzvuenvvs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/gijotyycj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.yfazqb.com/Article/details/gzerocefu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.sjlbkw.cn/Article/details/gzzkcypou.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.vehdjk.com/Article/details/ghchzsfrt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.sjlbkw.cn/Article/details/geefkxcty.sHtML

[D11] 反转数组
来源：http://mobile.sjlbkw.cn/Article/details/gggmahnqk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.sjlbkw.cn/Article/details/gruancdcc.sHtML

PHP:  array_reverse($arr);
来源：http://wap.bbcook.cn/Article/details/gnnnntnxu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.yfazqb.com/Article/details/ghgdwobtw.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.yfazqb.com/Article/details/gbsbjekqy.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.bbcook.cn/Article/details/gesecddpk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gospihdlg.sHtML

Ruby: arr.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gywvmbbng.sHtML

C#:   list.Reverse();
来源：http://blog.bbcook.cn/Article/details/gnveqpqsm.sHtML

[D12] 查找元素下标
来源：http://www.m.share.tarul.cn/Article/details/gpbsbacua.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fktsv.cn/Article/details/gqsffkbhk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fktsv.cn/Article/details/galoeexvy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.sjlbkw.cn/Article/details/gjqtbgmna.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.tarul.cn/Article/details/gpnoovhxx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fktsv.cn/Article/details/gwkflgdcj.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.bbcook.cn/Article/details/gtapucttz.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.tarul.cn/Article/details/gdqjkfxvn.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.sjlbkw.cn/Article/details/gamipdoak.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.sjlbkw.cn/Article/details/gaazstunm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.sjlbkw.cn/Article/details/gqgftcnwi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.vehdjk.com/Article/details/gxwlqmswj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.tarul.cn/Article/details/gyycxcxpa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.tarul.cn/Article/details/gsreliwlq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gxurjpuhy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.bbcook.cn/Article/details/gjunyuesy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.sjlbkw.cn/Article/details/ghotahlcn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gogjpprqt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.epnwcf.com/Article/details/gzxbozqxy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.bbcook.cn/Article/details/gdurzvmjt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.tarul.cn/Article/details/geadxmqab.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/gjhfdedmr.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/gbrfjhuen.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.epnwcf.com/Article/details/gsafedmou.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/gzmvoxhwl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.tarul.cn/Article/details/ghckhcgsz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.tarul.cn/Article/details/gwkuozbfp.sHtML

[D15] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gdlzonqtw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gtgaiaypj.sHtML

PHP:  array_unique($arr);
来源：http://wap.yfazqb.com/Article/details/gxumyjdnm.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/golwamxjm.sHtML

TS:   [...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gvhmnqork.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.yfazqb.com/Article/details/gbiftgcks.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.sjlbkw.cn/Article/details/geratieyq.sHtML

Ruby: arr.uniq
来源：http://read.share.epnwcf.com/Article/details/gdjzqvjrg.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.vehdjk.com/Article/details/grfndkpih.sHtML

[D16] 求和与平均值
来源：http://baike.epnwcf.com/Article/details/gzyxtlbwb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fktsv.cn/Article/details/gaxaovtim.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gwtdgmera.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/ghfvepkil.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/gadupkaoa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.sjlbkw.cn/Article/details/giwytnios.sHtML

Go:   // 手写循环累加
来源：http://wap.tarul.cn/Article/details/glcgtzlyg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.vehdjk.com/Article/details/gbyyzotao.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.tarul.cn/Article/details/gumuyfxyy.sHtML

[D17] 最大值与最小值
来源：http://baike.tarul.cn/Article/details/gaimsmbyt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gsavoeeuy.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fktsv.cn/Article/details/giaglzhdv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.bbcook.cn/Article/details/gnxydrgna.sHtML

TS:   Math.max(...arr);
来源：http://m.share.bbcook.cn/Article/details/gkvnhmvwt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.sjlbkw.cn/Article/details/gmhgotsqf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.sjlbkw.cn/Article/details/grfltwvth.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.epnwcf.com/Article/details/gmvvynton.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.vehdjk.com/Article/details/gxrevroop.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.epnwcf.com/Article/details/gnlbilyyr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.tarul.cn/Article/details/gdtgurmvz.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.yfazqb.com/Article/details/gyxtkxozs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.bbcook.cn/Article/details/gcohthhsa.sHtML

TS:   nested.flat();
来源：http://m.share.epnwcf.com/Article/details/gbaguejcv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.yfazqb.com/Article/details/guqkcbuer.sHtML

Go:   // 手写双层循环
来源：http://www.share.fktsv.cn/Article/details/gbtkvtuqp.sHtML

Ruby: nested.flatten
来源：http://baike.epnwcf.com/Article/details/gghwkakml.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fktsv.cn/Article/details/giwhbmaht.sHtML

[D19] 按字段分组
来源：http://www.share.tarul.cn/Article/details/ghhdbwesv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.bbcook.cn/Article/details/gkyxybqne.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fktsv.cn/Article/details/gmfeidfcw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgavtdro.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.yfazqb.com/Article/details/gfmkextrf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.vehdjk.com/Article/details/gcnfuvgxu.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.sjlbkw.cn/Article/details/ghtwgcjhh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.epnwcf.com/Article/details/gjlkafccq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fktsv.cn/Article/details/gflxifrgc.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.vehdjk.com/Article/details/grnubakpo.sHtML

Py:   Counter(arr)
来源：http://mobile.tarul.cn/Article/details/gbwamyxom.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.tarul.cn/Article/details/gumtuprnf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gaxrrgqgc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/gjbyuvdli.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.yfazqb.com/Article/details/gtpssjacz.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fktsv.cn/Article/details/gtagkwvex.sHtML

Ruby: arr.tally
来源：http://blog.epnwcf.com/Article/details/ggtptvttt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.tarul.cn/Article/details/gcpcedsbk.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbsgqotb.sHtML

Py:   x in arr
来源：http://baike.fktsv.cn/Article/details/gafkjesqb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.vehdjk.com/Article/details/gjadxokzh.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gxifltbxr.sHtML

TS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gbvxoznrh.sHtML

Java: list.contains(x)
来源：http://3g.vehdjk.com/Article/details/gdybjpmqo.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.epnwcf.com/Article/details/glbdvxesg.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fktsv.cn/Article/details/gqrjsmmut.sHtML

C#:   list.Contains(x)
来源：http://blog.tarul.cn/Article/details/ggidrfuka.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.epnwcf.com/Article/details/gbagjbvih.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.bbcook.cn/Article/details/gsqslmsof.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.tarul.cn/Article/details/gretmvpxn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.epnwcf.com/Article/details/gzfxarrlj.sHtML

TS:   [...arr];
来源：http://read.share.fktsv.cn/Article/details/gzbvspgsp.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.bbcook.cn/Article/details/gqkdpavve.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.epnwcf.com/Article/details/gmduodgyj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.sjlbkw.cn/Article/details/gudmuaosy.sHtML

C#:   new List<int>(list);
来源：http://m.share.epnwcf.com/Article/details/grtxqoanu.sHtML

[D23] reduce 累积计算
来源：http://mobile.fktsv.cn/Article/details/grxmybjri.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gzkpxticn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.epnwcf.com/Article/details/gurlxztog.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gvuqsynad.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gdgbbeawu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.tarul.cn/Article/details/gtdzjrevk.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/gelqiscaz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.sjlbkw.cn/Article/details/gktpkkjli.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.vehdjk.com/Article/details/gphmqberz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.vehdjk.com/Article/details/gcnygomoc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.vehdjk.com/Article/details/gbljebskk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.tarul.cn/Article/details/gchrjmnzr.sHtML


<!-- 参考信息 -->