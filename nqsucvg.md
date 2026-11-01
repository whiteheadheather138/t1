代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.share.tarul.cn/Article/details/gfdhdaoxg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.tarul.cn/Article/details/gupkyzzhi.sHtML

[C08] 闭包
来源：http://3g.sjlbkw.cn/Article/details/galnmydnv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.sjlbkw.cn/Article/details/gjorysqwg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.yfazqb.com/Article/details/gaqbwrupo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gjincntcs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gvixanmjr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fktsv.cn/Article/details/gyvgwegrg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.tarul.cn/Article/details/gyxosrtxy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.sjlbkw.cn/Article/details/gvejsnufl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/gljjhhldl.sHtML

[C09] 递归
来源：http://baike.yfazqb.com/Article/details/gnvhjkzqh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/gweijqkwk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.epnwcf.com/Article/details/gadugteta.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/gmqgpdwit.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.epnwcf.com/Article/details/gterkumfs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.epnwcf.com/Article/details/gspdqzbgi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fktsv.cn/Article/details/gkncwdyzz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gxgmbtuuz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.vehdjk.com/Article/details/gxoogswlb.sHtML

[C10] 变量作用域
来源：http://m.share.fktsv.cn/Article/details/gxgewlaks.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.bbcook.cn/Article/details/gfspuivux.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.tarul.cn/Article/details/gxhmrwfxg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.vehdjk.com/Article/details/gknyzurnz.sHtML

TS:   同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gkntnoiri.sHtML

Java: 方法内为块级作用域
来源：http://wap.bbcook.cn/Article/details/gysnjtjjm.sHtML

Go:   花括号块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gjyhdocyc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.sjlbkw.cn/Article/details/gpyzliwja.sHtML

C#:   块级作用域
来源：http://read.share.tarul.cn/Article/details/gfcfbevdc.sHtML

[C11] 模块导入与导出
来源：http://blog.bbcook.cn/Article/details/gbhwdnnwy.sHtML

Py:   from module import func
来源：http://www.m.share.fktsv.cn/Article/details/gbwzrfnhu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.epnwcf.com/Article/details/gdyzbvkdh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.tarul.cn/Article/details/gucexxfor.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.epnwcf.com/Article/details/gnvsnngpj.sHtML

Java: import java.util.List;
来源：http://www.share.sjlbkw.cn/Article/details/gzwsyrjqr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.sjlbkw.cn/Article/details/gtvtkhpqs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.epnwcf.com/Article/details/gmhffijqr.sHtML

C#:   using System.Text;
来源：http://wap.bbcook.cn/Article/details/giblcbfhk.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.vehdjk.com/Article/details/gkncjlkyn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.vehdjk.com/Article/details/gvdiksijx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fktsv.cn/Article/details/gicfogmfp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.yfazqb.com/Article/details/gywqwvxth.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/gjcudutpk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.tarul.cn/Article/details/gkfzhrjoj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.tarul.cn/Article/details/gzbqmbllm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fktsv.cn/Article/details/gxtkdtnuo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.vehdjk.com/Article/details/ghiibexza.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.tarul.cn/Article/details/gfqkicrdv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.vehdjk.com/Article/details/gdefyefci.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gfugsddqg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.yfazqb.com/Article/details/gumzvynke.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gjukrtxrw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gywvoppse.sHtML

Go:   func add(a, b int) int
来源：http://read.share.yfazqb.com/Article/details/gbqcruxwk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.epnwcf.com/Article/details/gaidfcwcj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.bbcook.cn/Article/details/gvguszmsy.sHtML

[C14] 泛型函数
来源：http://www.m.share.epnwcf.com/Article/details/gpnfsrcwa.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.vehdjk.com/Article/details/ghmlovchh.sHtML

PHP:  // 无泛型
来源：http://www.share.yfazqb.com/Article/details/gpavxjkvz.sHtML

JS:   // 无泛型
来源：http://read.share.tarul.cn/Article/details/gekksqgya.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.vehdjk.com/Article/details/gswygiqcs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.tarul.cn/Article/details/gfzvmivlr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.epnwcf.com/Article/details/gygpnxgkr.sHtML

Ruby: # 无泛型
来源：http://baike.tarul.cn/Article/details/grjgqzyyj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.bbcook.cn/Article/details/glqfoqqut.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fktsv.cn/Article/details/geiezkjio.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.bbcook.cn/Article/details/guzlbinoh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.vehdjk.com/Article/details/gwdjdkrtf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/gjeemnrcb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gpbngxxbh.sHtML

Java: // 无解构
来源：http://read.share.vehdjk.com/Article/details/goathqeqg.sHtML

Go:   // 无解构
来源：http://www.share.yfazqb.com/Article/details/gnjgnjstf.sHtML

Ruby: a, b = pair
来源：http://mobile.fktsv.cn/Article/details/gipxtbfih.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/grxmdznlp.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gepwuuqse.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.bbcook.cn/Article/details/gavgdsxfa.sHtML

PHP:  // 无重载
来源：http://m.share.epnwcf.com/Article/details/gvgunpebl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.vehdjk.com/Article/details/gsduhtxgj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.tarul.cn/Article/details/glirlghbz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.tarul.cn/Article/details/gnhotomni.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.vehdjk.com/Article/details/gcttnxrtw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.tarul.cn/Article/details/gjlgqmkvw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.sjlbkw.cn/Article/details/gmvjfspho.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwjncixhe.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.vehdjk.com/Article/details/giyybhmyq.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gikebafzo.sHtML

[D01] 创建数组 / 列表
来源：http://baike.yfazqb.com/Article/details/grwuvyrsg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.sjlbkw.cn/Article/details/gktjanbxm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.bbcook.cn/Article/details/gmmxxeuvh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.yfazqb.com/Article/details/gyblwmlqd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fktsv.cn/Article/details/gvurptjte.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.bbcook.cn/Article/details/gqvsrkmde.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.sjlbkw.cn/Article/details/gehbtbzpm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.bbcook.cn/Article/details/gpmvidfii.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.epnwcf.com/Article/details/gxxazkghi.sHtML

[D02] 追加元素到末尾
来源：http://wap.tarul.cn/Article/details/grwwegfjm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.tarul.cn/Article/details/glacfsyph.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.sjlbkw.cn/Article/details/gxsmjbclh.sHtML

JS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/gjwrglnxt.sHtML

TS:   arr.push(4);
来源：http://wap.epnwcf.com/Article/details/gpphdtfph.sHtML

Java: list.add(4);
来源：http://mobile.vehdjk.com/Article/details/godjiiwuo.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.epnwcf.com/Article/details/gklpravoz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.yfazqb.com/Article/details/gzwikstjl.sHtML

C#:   list.Add(4);
来源：http://wap.vehdjk.com/Article/details/gpaphwxtq.sHtML

[D03] 在指定位置插入元素
来源：http://baike.yfazqb.com/Article/details/gfjhrhonh.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gtlagworq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.yfazqb.com/Article/details/gxwfaltfp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.vehdjk.com/Article/details/ggiugnfxa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.vehdjk.com/Article/details/gdjmongfi.sHtML

Java: list.add(0, 0);
来源：http://3g.vehdjk.com/Article/details/gzfvrzvyu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.yfazqb.com/Article/details/gjownxueq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fktsv.cn/Article/details/gaiylxtyz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/ghowatyvg.sHtML

[D04] 删除元素
来源：http://m.share.sjlbkw.cn/Article/details/gcmvxebcf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.bbcook.cn/Article/details/gftmuiojw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpznkuwa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fktsv.cn/Article/details/gcymbsvly.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.yfazqb.com/Article/details/gxgrjqxxs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.epnwcf.com/Article/details/guoabknnn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.bbcook.cn/Article/details/gtyynziwj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.vehdjk.com/Article/details/gtzwsjgxn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.vehdjk.com/Article/details/gysoeuzfm.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.yfazqb.com/Article/details/gkqaekhqi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/geiecatkb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/grliginpp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtudqkhgh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.vehdjk.com/Article/details/gznuettpq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fktsv.cn/Article/details/gnxvatrsh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gtldsdkhj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gtkdgoope.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.bbcook.cn/Article/details/gkiioydto.sHtML

[D06] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gurrafxpp.sHtML

Py:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gmxtxlmoq.sHtML

PHP:  count($arr);
来源：http://wap.bbcook.cn/Article/details/glftwngow.sHtML

JS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/gmsnlldvr.sHtML

TS:   arr.length
来源：http://3g.tarul.cn/Article/details/glmtqnjyn.sHtML

Java: list.size();
来源：http://wap.vehdjk.com/Article/details/gyfdioorm.sHtML

Go:   len(arr)
来源：http://wap.yfazqb.com/Article/details/gyjptaepi.sHtML

Ruby: arr.length; arr.size
来源：http://3g.epnwcf.com/Article/details/ghgcgoqcq.sHtML

C#:   list.Count;
来源：http://m.share.vehdjk.com/Article/details/gkdfmiklf.sHtML

[D07] 切片 / 取子数组
来源：http://blog.epnwcf.com/Article/details/gtoeocpty.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.sjlbkw.cn/Article/details/gyacmwatc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.epnwcf.com/Article/details/ggpqfjain.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.tarul.cn/Article/details/gquvrurer.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gmkizmyms.sHtML

Java: list.subList(1, 4);
来源：http://read.share.epnwcf.com/Article/details/grtkledue.sHtML

Go:   arr[1:4]
来源：http://wap.bbcook.cn/Article/details/gtnfxqppv.sHtML

Ruby: arr[1, 3]
来源：http://baike.yfazqb.com/Article/details/gkvetgdkf.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.bbcook.cn/Article/details/gkqurnxhw.sHtML

[D08] 合并两个数组
来源：http://blog.sjlbkw.cn/Article/details/gqszoekuf.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.vehdjk.com/Article/details/gxfzsgjyk.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fktsv.cn/Article/details/gyjejbtuy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.sjlbkw.cn/Article/details/gnwumayrh.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.bbcook.cn/Article/details/gvmiesuik.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gemiklusa.sHtML

Go:   append(a, b...)
来源：http://3g.tarul.cn/Article/details/gsbppwrhv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.tarul.cn/Article/details/gyciabhjg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gmkusiwpx.sHtML

[D09] 排序（升序）
来源：http://3g.epnwcf.com/Article/details/gwcamwjvl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.epnwcf.com/Article/details/gqcxqgtsz.sHtML

PHP:  sort($arr);
来源：http://www.blog.bbcook.cn/Article/details/gnzosasgv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fktsv.cn/Article/details/gfycnbtxb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.sjlbkw.cn/Article/details/gwhztqufw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.bbcook.cn/Article/details/gqgrkzwek.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/gllmyquxs.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gndkqiltz.sHtML

C#:   list.Sort();
来源：http://baike.fktsv.cn/Article/details/ggttdhqcj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.tarul.cn/Article/details/gpxsbfcwi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.tarul.cn/Article/details/geomebkst.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fktsv.cn/Article/details/gashhljiv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/gcniznirq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.sjlbkw.cn/Article/details/gvnpeizte.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.bbcook.cn/Article/details/gdqkdyjpf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.yfazqb.com/Article/details/gtukstiot.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.sjlbkw.cn/Article/details/glwupcyyf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.tarul.cn/Article/details/gzrdraqtf.sHtML

[D11] 反转数组
来源：http://www.m.share.tarul.cn/Article/details/gnuxjrnte.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.tarul.cn/Article/details/gpmebiorz.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gfvmhkhiv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.sjlbkw.cn/Article/details/gthfyacoz.sHtML

TS:   [...arr].reverse();
来源：http://www.share.bbcook.cn/Article/details/genuzszmz.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fktsv.cn/Article/details/glwovqqqa.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.yfazqb.com/Article/details/gwkuqyoff.sHtML

Ruby: arr.reverse
来源：http://mobile.vehdjk.com/Article/details/gwpqvkmtr.sHtML

C#:   list.Reverse();
来源：http://wap.sjlbkw.cn/Article/details/gjbxerfak.sHtML

[D12] 查找元素下标
来源：http://m.share.sjlbkw.cn/Article/details/gfmlqhymq.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.tarul.cn/Article/details/gmyoluuao.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.yfazqb.com/Article/details/ggptqyeuy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.epnwcf.com/Article/details/glpynaxwn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gvvzntvum.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fktsv.cn/Article/details/ggppmsmot.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gnjlcezti.sHtML

Ruby: arr.index(x)
来源：http://wap.vehdjk.com/Article/details/gtetpssri.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.vehdjk.com/Article/details/gajeyahfb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.tarul.cn/Article/details/gqnosvgbe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.bbcook.cn/Article/details/gutjxnnvh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.epnwcf.com/Article/details/gaqddujuj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.vehdjk.com/Article/details/grixgvcgf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/gmeuhurtc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gxesayftk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.sjlbkw.cn/Article/details/gfnmwaguh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.epnwcf.com/Article/details/gwqrpzrvy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.tarul.cn/Article/details/gbarpgfns.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.yfazqb.com/Article/details/gjwtydwgr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.tarul.cn/Article/details/gsuplqcid.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdpabpfq.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/gkxuvrjbi.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gbuunxlkq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.vehdjk.com/Article/details/gcvcwsywl.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/gtvpwrgyg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.tarul.cn/Article/details/ghvxhfugi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.yfazqb.com/Article/details/geyewtkbo.sHtML

[D15] 去重
来源：http://read.share.fktsv.cn/Article/details/gsovhzdon.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.vehdjk.com/Article/details/goadkkyxm.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.epnwcf.com/Article/details/gatpnlnev.sHtML

JS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/giqnexfql.sHtML

TS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gpgechfep.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.yfazqb.com/Article/details/gmpfeewov.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.epnwcf.com/Article/details/ggskaudry.sHtML

Ruby: arr.uniq
来源：http://www.share.fktsv.cn/Article/details/gaziighvf.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.vehdjk.com/Article/details/gouivtymh.sHtML

[D16] 求和与平均值
来源：http://m.share.yfazqb.com/Article/details/ggeabqtxm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.bbcook.cn/Article/details/gztlasrst.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.tarul.cn/Article/details/gprtehnwq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gyknrddzw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gyzxliech.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fktsv.cn/Article/details/gvewcphgw.sHtML

Go:   // 手写循环累加
来源：http://www.share.bbcook.cn/Article/details/gdvetepal.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fktsv.cn/Article/details/gctouwmxy.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.bbcook.cn/Article/details/gwewngzvt.sHtML

[D17] 最大值与最小值
来源：http://wap.vehdjk.com/Article/details/gmbdecovt.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.yfazqb.com/Article/details/gyuenotla.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.tarul.cn/Article/details/ghsminwbn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.yfazqb.com/Article/details/giivhkizw.sHtML

TS:   Math.max(...arr);
来源：http://blog.vehdjk.com/Article/details/ggtfvjpge.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.tarul.cn/Article/details/gwvaubylf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gtswhymnm.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.sjlbkw.cn/Article/details/gfpjuxpod.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.vehdjk.com/Article/details/gxnqsebco.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.yfazqb.com/Article/details/gkfylpanu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fktsv.cn/Article/details/gkcjgwhpd.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.bbcook.cn/Article/details/gopjzzguh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fktsv.cn/Article/details/gtboecdnm.sHtML

TS:   nested.flat();
来源：http://www.share.sjlbkw.cn/Article/details/gtzjmwznh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.bbcook.cn/Article/details/ghwjzjnzw.sHtML

Go:   // 手写双层循环
来源：http://www.share.vehdjk.com/Article/details/gahgooypo.sHtML

Ruby: nested.flatten
来源：http://blog.yfazqb.com/Article/details/geoxphttx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.epnwcf.com/Article/details/gqoldqrci.sHtML

[D19] 按字段分组
来源：http://wap.yfazqb.com/Article/details/gjhllhyuo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.sjlbkw.cn/Article/details/ggrmhcdkj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.bbcook.cn/Article/details/ghevsjgpt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.tarul.cn/Article/details/gojpemdmo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gufatcnpt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fktsv.cn/Article/details/gpyxokjkb.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.sjlbkw.cn/Article/details/gnfhfnult.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.bbcook.cn/Article/details/glaseuine.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fktsv.cn/Article/details/gqjbdyqtn.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fktsv.cn/Article/details/gujmbalst.sHtML

Py:   Counter(arr)
来源：http://www.m.share.epnwcf.com/Article/details/grqdfpeer.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fktsv.cn/Article/details/gyjlmzepd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gpporcfod.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/grimxiyhm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.yfazqb.com/Article/details/gvqsjptzr.sHtML

Go:   // 手写 map[T]int
来源：http://3g.vehdjk.com/Article/details/gxmthigwo.sHtML

Ruby: arr.tally
来源：http://wap.epnwcf.com/Article/details/gmnkgtmat.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.tarul.cn/Article/details/gozlwlkup.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fktsv.cn/Article/details/gorwpsqtt.sHtML

Py:   x in arr
来源：http://mobile.yfazqb.com/Article/details/ggbwcrrlr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fktsv.cn/Article/details/gsxpaldci.sHtML

JS:   arr.includes(x)
来源：http://wap.yfazqb.com/Article/details/gqnmixleo.sHtML

TS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gnwtusrkk.sHtML

Java: list.contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gfxsiovte.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gzgbjmfxb.sHtML

Ruby: arr.include?(x)
来源：http://wap.tarul.cn/Article/details/gaqddvliw.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gavzqtbwr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.vehdjk.com/Article/details/glpgtrxtv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/gsdwwuxei.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.tarul.cn/Article/details/gkvnhalnk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfedgokl.sHtML

TS:   [...arr];
来源：http://www.share.fktsv.cn/Article/details/gcaoxobkj.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.tarul.cn/Article/details/giedvfxfj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.yfazqb.com/Article/details/gyzaidxut.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.tarul.cn/Article/details/gcrzlwxmj.sHtML

C#:   new List<int>(list);
来源：http://www.share.fktsv.cn/Article/details/gqverzgdi.sHtML

[D23] reduce 累积计算
来源：http://blog.tarul.cn/Article/details/gfktvgtjj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gwimckrsa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.yfazqb.com/Article/details/gpryclvdp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gsixylgdl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/gzyeutauo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.tarul.cn/Article/details/goupfywwm.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/ghfvbgwbg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.yfazqb.com/Article/details/gsnozpnks.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.vehdjk.com/Article/details/gusetjstx.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.sjlbkw.cn/Article/details/gdflxiwsi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.yfazqb.com/Article/details/goyjtharf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.epnwcf.com/Article/details/gfcsgxouj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.vehdjk.com/Article/details/gixotpbds.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.epnwcf.com/Article/details/gfjkewqug.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.yfazqb.com/Article/details/govnhilxw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.tarul.cn/Article/details/gvwpkojny.sHtML


<!-- 参考信息 -->