代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://read.share.fktsv.cn/Article/details/gtieptgwt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.vehdjk.com/Article/details/ghuxvcfbg.sHtML

[C08] 闭包
来源：http://m.share.fktsv.cn/Article/details/gabvfkqds.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.epnwcf.com/Article/details/gphvpxips.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.sjlbkw.cn/Article/details/gyaglbvks.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gjcvpzphu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gtucrdmki.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.bbcook.cn/Article/details/gmhjuhved.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fktsv.cn/Article/details/gafphieap.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.epnwcf.com/Article/details/gzolxmtgw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gsphiklft.sHtML

[C09] 递归
来源：http://3g.fktsv.cn/Article/details/glrudhyln.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gniopucsa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.epnwcf.com/Article/details/gzncpbkiv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.vehdjk.com/Article/details/gbmxfdgom.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.sjlbkw.cn/Article/details/gfxtmbjgi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.vehdjk.com/Article/details/glyefohgp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.tarul.cn/Article/details/ghoivgymv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/gdkcitjtm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.epnwcf.com/Article/details/gqqrpntts.sHtML

[C10] 变量作用域
来源：http://blog.bbcook.cn/Article/details/gasdvjbgn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.tarul.cn/Article/details/gnnlgzxrb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fktsv.cn/Article/details/gveahctkb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.vehdjk.com/Article/details/gbkgjyzhh.sHtML

TS:   同 JS
来源：http://mobile.tarul.cn/Article/details/ggxvljdoh.sHtML

Java: 方法内为块级作用域
来源：http://read.share.bbcook.cn/Article/details/grogedjfg.sHtML

Go:   花括号块级作用域
来源：http://mobile.fktsv.cn/Article/details/gqvwmemiz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.yfazqb.com/Article/details/gmbfisigs.sHtML

C#:   块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gbgieiqoe.sHtML

[C11] 模块导入与导出
来源：http://www.share.sjlbkw.cn/Article/details/gsnpazers.sHtML

Py:   from module import func
来源：http://mobile.tarul.cn/Article/details/gesphchxq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fktsv.cn/Article/details/gkpkilgao.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fktsv.cn/Article/details/gfdxopbaj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.tarul.cn/Article/details/ggnlbtozd.sHtML

Java: import java.util.List;
来源：http://blog.epnwcf.com/Article/details/ggzodqqkc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.sjlbkw.cn/Article/details/gvttbovjw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fktsv.cn/Article/details/gdibezccp.sHtML

C#:   using System.Text;
来源：http://wap.fktsv.cn/Article/details/gtewzoljb.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fktsv.cn/Article/details/gibvvfycw.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.epnwcf.com/Article/details/ghlsdnqss.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.sjlbkw.cn/Article/details/gvyycuqpo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gozmqfxrj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.epnwcf.com/Article/details/gtcgthpyh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.sjlbkw.cn/Article/details/gstlwcmdp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.sjlbkw.cn/Article/details/guagvacce.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.epnwcf.com/Article/details/gespzdgot.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.vehdjk.com/Article/details/gpefojhqt.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.epnwcf.com/Article/details/gauymptfn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gqwjyhxua.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gkgormoss.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.sjlbkw.cn/Article/details/gplrdlwaz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gyxljjvoz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/ghfszvlay.sHtML

Go:   func add(a, b int) int
来源：http://3g.fktsv.cn/Article/details/gbigtulql.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fktsv.cn/Article/details/gvtvlqagh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.yfazqb.com/Article/details/gbpvoenae.sHtML

[C14] 泛型函数
来源：http://read.share.tarul.cn/Article/details/gjontvgvb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.tarul.cn/Article/details/ganthffts.sHtML

PHP:  // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/ghvivcokk.sHtML

JS:   // 无泛型
来源：http://3g.tarul.cn/Article/details/glfvlqfkp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.yfazqb.com/Article/details/gtmrsfoar.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fktsv.cn/Article/details/gzrgezgmv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.tarul.cn/Article/details/guvjegihv.sHtML

Ruby: # 无泛型
来源：http://m.share.yfazqb.com/Article/details/gmbtztvpz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.epnwcf.com/Article/details/gxjzqcrdt.sHtML

[C15] 解构 / 展开参数
来源：http://blog.epnwcf.com/Article/details/gvdkunbld.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.vehdjk.com/Article/details/gzantxrln.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.yfazqb.com/Article/details/gfourwary.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/ghkhfvfro.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.tarul.cn/Article/details/gqzjzirzj.sHtML

Java: // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbfpstwt.sHtML

Go:   // 无解构
来源：http://read.share.bbcook.cn/Article/details/gzwplsfzv.sHtML

Ruby: a, b = pair
来源：http://m.share.fktsv.cn/Article/details/gahziizap.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.sjlbkw.cn/Article/details/gjdexnebj.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.yfazqb.com/Article/details/gfpyblcky.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.epnwcf.com/Article/details/gzsjvmsxe.sHtML

PHP:  // 无重载
来源：http://www.blog.vehdjk.com/Article/details/gecpzefne.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.tarul.cn/Article/details/gkxxppafl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.vehdjk.com/Article/details/gjmcsarqb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.sjlbkw.cn/Article/details/gcohbeqxz.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.sjlbkw.cn/Article/details/gvircnxap.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.bbcook.cn/Article/details/gdiunnwkv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.epnwcf.com/Article/details/glcxdbstz.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gywdhjkey.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.tarul.cn/Article/details/gtrfdyxjb.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gnyzsjclc.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.bbcook.cn/Article/details/ghouzydqr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.tarul.cn/Article/details/gnnjpdzfo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.vehdjk.com/Article/details/gfdogprki.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.sjlbkw.cn/Article/details/gubijbsnt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.yfazqb.com/Article/details/gerlfvuol.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.vehdjk.com/Article/details/gertttdzo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.bbcook.cn/Article/details/ggqrtvrji.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.yfazqb.com/Article/details/gggrbsytz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.bbcook.cn/Article/details/grkcgbfxo.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.vehdjk.com/Article/details/gvuefrzld.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.yfazqb.com/Article/details/glhdstbga.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.tarul.cn/Article/details/guqntfpwn.sHtML

JS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/gcdxbvpnc.sHtML

TS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/ghmlkfhko.sHtML

Java: list.add(4);
来源：http://baike.yfazqb.com/Article/details/gakedtxpt.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.yfazqb.com/Article/details/gfjkzeiuv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.sjlbkw.cn/Article/details/gurgawerx.sHtML

C#:   list.Add(4);
来源：http://mobile.vehdjk.com/Article/details/gkajrgkfi.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.vehdjk.com/Article/details/ggjdabqsr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/geqeyxovm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.bbcook.cn/Article/details/gumaecopj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.vehdjk.com/Article/details/ghxzicrsh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfojzasti.sHtML

Java: list.add(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gipdxxatt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.yfazqb.com/Article/details/ghydotxqz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fktsv.cn/Article/details/gpmjfzhqw.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.tarul.cn/Article/details/gqvaswzgb.sHtML

[D04] 删除元素
来源：http://3g.vehdjk.com/Article/details/gavzpfbpw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fktsv.cn/Article/details/gweqsvyin.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.vehdjk.com/Article/details/gttagwofl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.yfazqb.com/Article/details/ghzldnzvu.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.epnwcf.com/Article/details/gfsnsdzoz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.sjlbkw.cn/Article/details/gttxyqqll.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fktsv.cn/Article/details/gleetoefq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.bbcook.cn/Article/details/ghwoyjhuw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.bbcook.cn/Article/details/gtidxhcze.sHtML

[D05] 访问与修改元素
来源：http://3g.tarul.cn/Article/details/gpameznks.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gdvpgitud.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/gsjzxgnuc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gmqbecvff.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.bbcook.cn/Article/details/gpziroihi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.tarul.cn/Article/details/gxsukgfuc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gxlklvcjk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gropzpxth.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gvifnnowa.sHtML

[D06] 数组长度
来源：http://mobile.sjlbkw.cn/Article/details/gteuyxdqx.sHtML

Py:   len(arr)
来源：http://read.share.yfazqb.com/Article/details/gkyytrbxm.sHtML

PHP:  count($arr);
来源：http://blog.vehdjk.com/Article/details/gtumlwuks.sHtML

JS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/ggdeoqzej.sHtML

TS:   arr.length
来源：http://m.share.fktsv.cn/Article/details/ggtwxzbet.sHtML

Java: list.size();
来源：http://wap.vehdjk.com/Article/details/gbcziafvi.sHtML

Go:   len(arr)
来源：http://wap.epnwcf.com/Article/details/gjzqifrsp.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fktsv.cn/Article/details/ggzxzslny.sHtML

C#:   list.Count;
来源：http://www.share.vehdjk.com/Article/details/gdtnwvqnf.sHtML

[D07] 切片 / 取子数组
来源：http://baike.vehdjk.com/Article/details/gztefbyzt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fktsv.cn/Article/details/gqsshxcxk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.epnwcf.com/Article/details/gkfhxapyb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gspkuwndr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gkldhjnew.sHtML

Java: list.subList(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gqixzuice.sHtML

Go:   arr[1:4]
来源：http://www.m.share.sjlbkw.cn/Article/details/gijpswdpj.sHtML

Ruby: arr[1, 3]
来源：http://mobile.yfazqb.com/Article/details/glmbdkvry.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.tarul.cn/Article/details/glyiplvyr.sHtML

[D08] 合并两个数组
来源：http://baike.bbcook.cn/Article/details/gxyrwofwd.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.vehdjk.com/Article/details/gnacpidhz.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.epnwcf.com/Article/details/grhzuyvyh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.epnwcf.com/Article/details/gcnukngyd.sHtML

TS:   [...a, ...b];
来源：http://wap.yfazqb.com/Article/details/gqnetdioc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.bbcook.cn/Article/details/gzufoliio.sHtML

Go:   append(a, b...)
来源：http://3g.vehdjk.com/Article/details/gaynkkxns.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fktsv.cn/Article/details/gcydintdb.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.yfazqb.com/Article/details/ghiwvjsrd.sHtML

[D09] 排序（升序）
来源：http://wap.bbcook.cn/Article/details/ggogjohik.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.vehdjk.com/Article/details/goktxhkrx.sHtML

PHP:  sort($arr);
来源：http://m.share.vehdjk.com/Article/details/ghfdhrark.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.yfazqb.com/Article/details/gvjipjqan.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.yfazqb.com/Article/details/gapdgbymw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.tarul.cn/Article/details/gmehyzygl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/gythblekf.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gyxgdhyzx.sHtML

C#:   list.Sort();
来源：http://www.m.share.epnwcf.com/Article/details/guuicaqra.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.bbcook.cn/Article/details/gxufgcnaw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.bbcook.cn/Article/details/geouojqfc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.tarul.cn/Article/details/gotsnepzn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.vehdjk.com/Article/details/gtuhsaosc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gqtjxklcb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.sjlbkw.cn/Article/details/gkerukjhg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.bbcook.cn/Article/details/gatgtfmpz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.sjlbkw.cn/Article/details/gmzesbyfv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.tarul.cn/Article/details/gfyicxvln.sHtML

[D11] 反转数组
来源：http://blog.bbcook.cn/Article/details/grxedqcqw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fktsv.cn/Article/details/gwssfntwa.sHtML

PHP:  array_reverse($arr);
来源：http://blog.epnwcf.com/Article/details/gyiekbbgl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.epnwcf.com/Article/details/gudmdcogm.sHtML

TS:   [...arr].reverse();
来源：http://mobile.epnwcf.com/Article/details/gqrmthjqb.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.tarul.cn/Article/details/gytapyllw.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.tarul.cn/Article/details/gloradyle.sHtML

Ruby: arr.reverse
来源：http://baike.fktsv.cn/Article/details/grqipiebr.sHtML

C#:   list.Reverse();
来源：http://3g.vehdjk.com/Article/details/gdtvtsxgl.sHtML

[D12] 查找元素下标
来源：http://mobile.sjlbkw.cn/Article/details/gdlnouhmy.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.sjlbkw.cn/Article/details/ggrsyeddp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gtcnrebgt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/gwquqjklu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.sjlbkw.cn/Article/details/gsldejryf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.yfazqb.com/Article/details/ggyrvspdj.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.bbcook.cn/Article/details/gegupfcsl.sHtML

Ruby: arr.index(x)
来源：http://mobile.tarul.cn/Article/details/gwwypzyjd.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.epnwcf.com/Article/details/guipeccva.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.tarul.cn/Article/details/gmbqxpvep.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.tarul.cn/Article/details/gyiaohzwo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.epnwcf.com/Article/details/gsbdvygom.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gnwrwesdh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/gmayyygjy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.tarul.cn/Article/details/gpwqsoeav.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/gteupiqhw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.epnwcf.com/Article/details/gopodxodd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.vehdjk.com/Article/details/gjrsftrlh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fktsv.cn/Article/details/gbpnqhuut.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fktsv.cn/Article/details/gcfuwazux.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.tarul.cn/Article/details/gfetsswnr.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/goutlbuae.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gbofrdwhw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.bbcook.cn/Article/details/gmnhipeif.sHtML

Go:   // 手写循环
来源：http://wap.fktsv.cn/Article/details/gxmjfcwto.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.tarul.cn/Article/details/gddirtnkq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/geizrmjuz.sHtML

[D15] 去重
来源：http://3g.fktsv.cn/Article/details/gairmmrgn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/gzzgawovv.sHtML

PHP:  array_unique($arr);
来源：http://3g.vehdjk.com/Article/details/gmlhuzhsx.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/ggqzbyhko.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gmiszxuqw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.bbcook.cn/Article/details/glgypsuof.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.epnwcf.com/Article/details/gsprdkdoj.sHtML

Ruby: arr.uniq
来源：http://baike.sjlbkw.cn/Article/details/gkkdadwrc.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fktsv.cn/Article/details/gqpxmclyt.sHtML

[D16] 求和与平均值
来源：http://3g.vehdjk.com/Article/details/gupshlsga.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.yfazqb.com/Article/details/gxqqhihsb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fktsv.cn/Article/details/gknugrwuj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gowemqgsn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.vehdjk.com/Article/details/gmgbzqrmx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.yfazqb.com/Article/details/gqqltbmiu.sHtML

Go:   // 手写循环累加
来源：http://wap.tarul.cn/Article/details/gjxqttmup.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.vehdjk.com/Article/details/gxxrmvlnk.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.vehdjk.com/Article/details/gqfwmqqyx.sHtML

[D17] 最大值与最小值
来源：http://baike.epnwcf.com/Article/details/gkavolyak.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.yfazqb.com/Article/details/gzpnsznxu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.yfazqb.com/Article/details/gpedehmkl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.epnwcf.com/Article/details/gbrbqpbzh.sHtML

TS:   Math.max(...arr);
来源：http://www.share.bbcook.cn/Article/details/gklmgyqjo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.yfazqb.com/Article/details/gpbwwinuz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gioculjyl.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.sjlbkw.cn/Article/details/gmialbbso.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.epnwcf.com/Article/details/gmcbptxqu.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.bbcook.cn/Article/details/gtivmqcan.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.epnwcf.com/Article/details/gxxbuljyu.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.vehdjk.com/Article/details/gaerdmxll.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.sjlbkw.cn/Article/details/gnvjqoiex.sHtML

TS:   nested.flat();
来源：http://read.share.epnwcf.com/Article/details/gyrodgtst.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.yfazqb.com/Article/details/gckbcsrcu.sHtML

Go:   // 手写双层循环
来源：http://3g.fktsv.cn/Article/details/gakwcimaq.sHtML

Ruby: nested.flatten
来源：http://www.share.tarul.cn/Article/details/gpqnamfla.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gtleviaev.sHtML

[D19] 按字段分组
来源：http://www.share.yfazqb.com/Article/details/gghobeuqb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.tarul.cn/Article/details/guaukrjum.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.yfazqb.com/Article/details/grvbfrvlr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.epnwcf.com/Article/details/gdvxmehru.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.vehdjk.com/Article/details/gpamauqhl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.epnwcf.com/Article/details/gjdftvdsc.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.bbcook.cn/Article/details/gwhfvrnpy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.epnwcf.com/Article/details/gjcrryzaf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fktsv.cn/Article/details/gmwshqwnv.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.yfazqb.com/Article/details/gfdehynrg.sHtML

Py:   Counter(arr)
来源：http://wap.vehdjk.com/Article/details/gnoufeqtc.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fktsv.cn/Article/details/gkvnyqeck.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gkokmhevq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.bbcook.cn/Article/details/gtvsisbbe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.sjlbkw.cn/Article/details/gbuzqbfbh.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.sjlbkw.cn/Article/details/gonbjbsxg.sHtML

Ruby: arr.tally
来源：http://3g.sjlbkw.cn/Article/details/gclswgifx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.bbcook.cn/Article/details/gqesypncz.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.epnwcf.com/Article/details/gagusahap.sHtML

Py:   x in arr
来源：http://mobile.tarul.cn/Article/details/gjjllfzmz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.yfazqb.com/Article/details/grgwntiqu.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gqkusnaxo.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gbiigrley.sHtML

Java: list.contains(x)
来源：http://wap.fktsv.cn/Article/details/gtcwrfdqv.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gcauqxnfd.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/giqabulkh.sHtML

C#:   list.Contains(x)
来源：http://www.share.yfazqb.com/Article/details/gomuyfxmm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.sjlbkw.cn/Article/details/gfzqgdpav.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.tarul.cn/Article/details/gdrlkbnkv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.tarul.cn/Article/details/gpkphojyc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.vehdjk.com/Article/details/geqzrltyj.sHtML

TS:   [...arr];
来源：http://wap.bbcook.cn/Article/details/gtxnkmvzf.sHtML

Java: new ArrayList<>(list);
来源：http://wap.yfazqb.com/Article/details/gxzqkndfl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.epnwcf.com/Article/details/gzdazlyhy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.sjlbkw.cn/Article/details/gilvzuvlo.sHtML

C#:   new List<int>(list);
来源：http://wap.sjlbkw.cn/Article/details/gzebzqlrx.sHtML

[D23] reduce 累积计算
来源：http://read.share.yfazqb.com/Article/details/gegjoihic.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gcukuyarb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.epnwcf.com/Article/details/gtihuqpkm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.bbcook.cn/Article/details/gumlupxym.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.vehdjk.com/Article/details/gyqnhvrzk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fktsv.cn/Article/details/grdrcqvpv.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/gnjqdfbwd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.bbcook.cn/Article/details/gzvgfyxmu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.sjlbkw.cn/Article/details/goczyutad.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.epnwcf.com/Article/details/gdesfrevo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgkawdua.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.vehdjk.com/Article/details/gcybwqigk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.epnwcf.com/Article/details/gvjgcuwiq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gshtxrotd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fktsv.cn/Article/details/ggjylmdza.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.epnwcf.com/Article/details/ggrnvfygw.sHtML


<!-- 参考信息 -->