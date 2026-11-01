代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.epnwcf.com/Article/details/ghwcfkhxx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.sjlbkw.cn/Article/details/gizzhhjwo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gtlziwqmz.sHtML

[C09] 递归
来源：http://www.blog.bbcook.cn/Article/details/gnfmuhksq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.tarul.cn/Article/details/glnfiussr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.tarul.cn/Article/details/gzuetufxn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.tarul.cn/Article/details/gfqwhkuje.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.bbcook.cn/Article/details/gyxvylvqd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.vehdjk.com/Article/details/gkykmdtzo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.epnwcf.com/Article/details/gaabtzeid.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.bbcook.cn/Article/details/gyinulpnp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fktsv.cn/Article/details/gcrauypog.sHtML

[C10] 变量作用域
来源：http://mobile.sjlbkw.cn/Article/details/gbxvffekm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.yfazqb.com/Article/details/gbkbporik.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.tarul.cn/Article/details/gzdwxxzfp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.tarul.cn/Article/details/gbipnhxvm.sHtML

TS:   同 JS
来源：http://3g.fktsv.cn/Article/details/goqchqyjq.sHtML

Java: 方法内为块级作用域
来源：http://www.share.epnwcf.com/Article/details/gqixbvmoc.sHtML

Go:   花括号块级作用域
来源：http://wap.yfazqb.com/Article/details/gwdjzxgbu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.bbcook.cn/Article/details/ghqhdcloj.sHtML

C#:   块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/goovzerrm.sHtML

[C11] 模块导入与导出
来源：http://read.share.sjlbkw.cn/Article/details/geqiwpyta.sHtML

Py:   from module import func
来源：http://blog.bbcook.cn/Article/details/gvfkrkfus.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.tarul.cn/Article/details/goijwhrrx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/grjipfkzx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkmhktvt.sHtML

Java: import java.util.List;
来源：http://blog.fktsv.cn/Article/details/grlpgddlf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.vehdjk.com/Article/details/gxjzcweii.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fktsv.cn/Article/details/gcptrwutl.sHtML

C#:   using System.Text;
来源：http://mobile.fktsv.cn/Article/details/gigmdlirl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.bbcook.cn/Article/details/gotjjsbdv.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.tarul.cn/Article/details/gjvkgrgxd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.tarul.cn/Article/details/gdtauvtiz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.sjlbkw.cn/Article/details/gjokmeyfr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.vehdjk.com/Article/details/gyhekzogx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.vehdjk.com/Article/details/gfqawzjos.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.tarul.cn/Article/details/gbxqvciwv.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.epnwcf.com/Article/details/ggxgmcmbi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fktsv.cn/Article/details/gvqtetodo.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.epnwcf.com/Article/details/ghvqbbxro.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.tarul.cn/Article/details/gkxdrowrh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/glckbkugj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.vehdjk.com/Article/details/gvymmokkt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gmiqujwiy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gpmvrtjxw.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.bbcook.cn/Article/details/gvsrqnarg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fktsv.cn/Article/details/gbqxbgtgj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.yfazqb.com/Article/details/ggtlcbsec.sHtML

[C14] 泛型函数
来源：http://m.share.epnwcf.com/Article/details/gasxxtybz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.yfazqb.com/Article/details/gxzkpvube.sHtML

PHP:  // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gibgbimdy.sHtML

JS:   // 无泛型
来源：http://read.share.fktsv.cn/Article/details/gnfywxdis.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.epnwcf.com/Article/details/gqmbcptiq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.vehdjk.com/Article/details/gwlxoisio.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.tarul.cn/Article/details/gfnleopyt.sHtML

Ruby: # 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gvlhhlyvl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.vehdjk.com/Article/details/gxvzywjvc.sHtML

[C15] 解构 / 展开参数
来源：http://3g.tarul.cn/Article/details/gyagrlicd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.sjlbkw.cn/Article/details/gddcogejw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.yfazqb.com/Article/details/gmaamtrda.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.vehdjk.com/Article/details/ghfumlwpe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fktsv.cn/Article/details/gwxbnavzh.sHtML

Java: // 无解构
来源：http://wap.sjlbkw.cn/Article/details/gchhhwzwq.sHtML

Go:   // 无解构
来源：http://mobile.yfazqb.com/Article/details/ghzlrjkot.sHtML

Ruby: a, b = pair
来源：http://mobile.vehdjk.com/Article/details/gsamzoztp.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.vehdjk.com/Article/details/gxhetboes.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.vehdjk.com/Article/details/gxreyrgzr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.vehdjk.com/Article/details/gbgjzoubd.sHtML

PHP:  // 无重载
来源：http://wap.fktsv.cn/Article/details/gfojhybxn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fktsv.cn/Article/details/guxepodth.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.sjlbkw.cn/Article/details/ggbfflgom.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.epnwcf.com/Article/details/gguohbyto.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fktsv.cn/Article/details/garblyqcu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.yfazqb.com/Article/details/gfdgrvtqr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbpfjgtid.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/graugepuz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.vehdjk.com/Article/details/golaociao.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ghuuegsmj.sHtML

[D01] 创建数组 / 列表
来源：http://blog.bbcook.cn/Article/details/gxxlxdpvj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.bbcook.cn/Article/details/gscptepvx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.vehdjk.com/Article/details/gxchugsol.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gtoeuepoq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fktsv.cn/Article/details/gubnwnqzv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.epnwcf.com/Article/details/ghociedtw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.epnwcf.com/Article/details/glzjmmfua.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.vehdjk.com/Article/details/ghvkegwqw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.sjlbkw.cn/Article/details/gblcakjcj.sHtML

[D02] 追加元素到末尾
来源：http://mobile.tarul.cn/Article/details/gjrrgzfqg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.vehdjk.com/Article/details/gglvpxvaq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fktsv.cn/Article/details/gxzsafjqc.sHtML

JS:   arr.push(4);
来源：http://www.blog.epnwcf.com/Article/details/giydqfuqs.sHtML

TS:   arr.push(4);
来源：http://baike.vehdjk.com/Article/details/gjuisonvh.sHtML

Java: list.add(4);
来源：http://www.blog.bbcook.cn/Article/details/ghuetmchy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.bbcook.cn/Article/details/ggdnvqdgq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.bbcook.cn/Article/details/gsuannjkj.sHtML

C#:   list.Add(4);
来源：http://mobile.yfazqb.com/Article/details/gsmdakujs.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.epnwcf.com/Article/details/geypsefhw.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.epnwcf.com/Article/details/glvyulctz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.epnwcf.com/Article/details/gmmhsnqcg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.vehdjk.com/Article/details/gsbcjcjqt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.bbcook.cn/Article/details/gmmpnsxmv.sHtML

Java: list.add(0, 0);
来源：http://wap.fktsv.cn/Article/details/gumvyiqqt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.yfazqb.com/Article/details/gxdobqcwg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.tarul.cn/Article/details/gtdifqjuu.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.tarul.cn/Article/details/goikwcigw.sHtML

[D04] 删除元素
来源：http://wap.yfazqb.com/Article/details/gvkhtlzhz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.epnwcf.com/Article/details/gsyzshyrn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.bbcook.cn/Article/details/gfqfsbjaq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.vehdjk.com/Article/details/gwrzipiov.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.vehdjk.com/Article/details/gnaylggjg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.tarul.cn/Article/details/gjdtxhhwk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.epnwcf.com/Article/details/gymskrpok.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.tarul.cn/Article/details/gpwnyrrts.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.yfazqb.com/Article/details/gozmkvbsh.sHtML

[D05] 访问与修改元素
来源：http://baike.sjlbkw.cn/Article/details/gnfbaloit.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gdhsqyljn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.yfazqb.com/Article/details/gdtivtoci.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/grcbpvdnp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fktsv.cn/Article/details/ggapsnrlv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.yfazqb.com/Article/details/ghbmmpcuv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gjwxqgrpk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gbpfkedia.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/gxuajkxdn.sHtML

[D06] 数组长度
来源：http://read.share.tarul.cn/Article/details/gygiotebj.sHtML

Py:   len(arr)
来源：http://read.share.tarul.cn/Article/details/gllnfpklc.sHtML

PHP:  count($arr);
来源：http://www.blog.bbcook.cn/Article/details/gtdadbaph.sHtML

JS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/gwdzmujog.sHtML

TS:   arr.length
来源：http://baike.bbcook.cn/Article/details/gsltwrazt.sHtML

Java: list.size();
来源：http://www.m.share.epnwcf.com/Article/details/gmoxsqrye.sHtML

Go:   len(arr)
来源：http://m.share.tarul.cn/Article/details/gwelzfhqe.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.tarul.cn/Article/details/gxwjvyyng.sHtML

C#:   list.Count;
来源：http://www.share.yfazqb.com/Article/details/gnmqdygfu.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.epnwcf.com/Article/details/gzgxdpgwz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fktsv.cn/Article/details/gijvcfrcb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.vehdjk.com/Article/details/gzhbfmfki.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/grfmfteza.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/guchvsewj.sHtML

Java: list.subList(1, 4);
来源：http://baike.epnwcf.com/Article/details/gdslkeohw.sHtML

Go:   arr[1:4]
来源：http://baike.yfazqb.com/Article/details/gsswxpscq.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fktsv.cn/Article/details/ghlulvhux.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gjgfhgnei.sHtML

[D08] 合并两个数组
来源：http://m.share.tarul.cn/Article/details/gxxdsqrps.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.bbcook.cn/Article/details/govfgcbwu.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.vehdjk.com/Article/details/gorzcqfkf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fktsv.cn/Article/details/gkdocvgee.sHtML

TS:   [...a, ...b];
来源：http://blog.vehdjk.com/Article/details/gxmsybxrq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gddgjnhxq.sHtML

Go:   append(a, b...)
来源：http://baike.fktsv.cn/Article/details/grsivgtab.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.bbcook.cn/Article/details/gqdxgraqa.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.tarul.cn/Article/details/gjdxnwmmp.sHtML

[D09] 排序（升序）
来源：http://wap.tarul.cn/Article/details/gpbreqpti.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/gfcsycyns.sHtML

PHP:  sort($arr);
来源：http://read.share.epnwcf.com/Article/details/gfqqqqorg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.bbcook.cn/Article/details/guojjptfg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fktsv.cn/Article/details/gyhqgbitf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.yfazqb.com/Article/details/grvbseqxi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gkdewmbzb.sHtML

Ruby: arr.sort
来源：http://baike.bbcook.cn/Article/details/gxkipwqfq.sHtML

C#:   list.Sort();
来源：http://mobile.vehdjk.com/Article/details/gpqqcdhne.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.tarul.cn/Article/details/gzevpmnyg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.tarul.cn/Article/details/gmuiozyha.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/gpnrxxsto.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/gfnukiwtu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gxcpvkiva.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.bbcook.cn/Article/details/ggdbskqar.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.vehdjk.com/Article/details/gmokjfquv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.vehdjk.com/Article/details/gzwmfmrtg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.vehdjk.com/Article/details/gjtklvpsp.sHtML

[D11] 反转数组
来源：http://read.share.bbcook.cn/Article/details/gsvqizfwk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.epnwcf.com/Article/details/glhrfinqe.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/grlughlca.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.bbcook.cn/Article/details/gulcivoiq.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/gsmpbawsk.sHtML

Java: Collections.reverse(list);
来源：http://baike.sjlbkw.cn/Article/details/gaeqkxkds.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.sjlbkw.cn/Article/details/gjktjemks.sHtML

Ruby: arr.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gjxvniewz.sHtML

C#:   list.Reverse();
来源：http://wap.fktsv.cn/Article/details/gilmekpzt.sHtML

[D12] 查找元素下标
来源：http://m.share.fktsv.cn/Article/details/gdroacdcg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gjyxrfupw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/givkjzkbe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gmjvepfbl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gzkifkugj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.yfazqb.com/Article/details/gwehrzzzz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gnzhlphqd.sHtML

Ruby: arr.index(x)
来源：http://www.blog.tarul.cn/Article/details/gwlnmbamx.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.tarul.cn/Article/details/gmvvppjfy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.tarul.cn/Article/details/ggyuxrvlg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.tarul.cn/Article/details/gsbsyylat.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.sjlbkw.cn/Article/details/grsssvzvp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gjictvryw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gsttqshta.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.vehdjk.com/Article/details/gsryunvse.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.bbcook.cn/Article/details/gbpfsckwp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.epnwcf.com/Article/details/gpbsqbfdm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.tarul.cn/Article/details/gvextaczo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.bbcook.cn/Article/details/gguiohnwf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.yfazqb.com/Article/details/gsmcxzmqy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.tarul.cn/Article/details/grhruqkwc.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/gbagxsjvp.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/gjzexbyri.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.bbcook.cn/Article/details/goquymvys.sHtML

Go:   // 手写循环
来源：http://mobile.tarul.cn/Article/details/gbefnnlxm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.vehdjk.com/Article/details/gufwibpsh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.yfazqb.com/Article/details/goozgzfjd.sHtML

[D15] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gxaihpxuk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gwrnnuowo.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gewtmiddo.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gbqcyvpui.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gizgnlktn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.vehdjk.com/Article/details/gofbrocrb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.bbcook.cn/Article/details/gubcymvsl.sHtML

Ruby: arr.uniq
来源：http://www.blog.epnwcf.com/Article/details/groshfcaz.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.vehdjk.com/Article/details/glxwnqxyn.sHtML

[D16] 求和与平均值
来源：http://read.share.yfazqb.com/Article/details/gfjvpcgkx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.vehdjk.com/Article/details/gvrzeljgq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gizsaudxc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/gqabrrhay.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gyvafkrmk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.vehdjk.com/Article/details/gabeeaxtc.sHtML

Go:   // 手写循环累加
来源：http://www.share.yfazqb.com/Article/details/glneomxrk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.bbcook.cn/Article/details/giadprqzq.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.epnwcf.com/Article/details/gozxavfdy.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.bbcook.cn/Article/details/gcuctkogm.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.yfazqb.com/Article/details/gyjdpxhwi.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.tarul.cn/Article/details/ggmsumqoo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.tarul.cn/Article/details/goafmyeoa.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.epnwcf.com/Article/details/gfmyfuzvd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.sjlbkw.cn/Article/details/gdcthiolw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/gfivzraco.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.epnwcf.com/Article/details/gsyepetuj.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fktsv.cn/Article/details/gaypwhhhi.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.sjlbkw.cn/Article/details/gntrbwpag.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/gsywsmpmn.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.bbcook.cn/Article/details/gumnxafzi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fktsv.cn/Article/details/ghchumwsa.sHtML

TS:   nested.flat();
来源：http://blog.tarul.cn/Article/details/gvngksxwo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.tarul.cn/Article/details/grudrxvvz.sHtML

Go:   // 手写双层循环
来源：http://m.share.bbcook.cn/Article/details/gfykpvaez.sHtML

Ruby: nested.flatten
来源：http://read.share.bbcook.cn/Article/details/gzatcljjt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.vehdjk.com/Article/details/gkjeagwqd.sHtML

[D19] 按字段分组
来源：http://wap.fktsv.cn/Article/details/glgkvpjbk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.vehdjk.com/Article/details/gxhlccaic.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.bbcook.cn/Article/details/gihoxayka.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.vehdjk.com/Article/details/glnnenpnk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/gijulctyu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.sjlbkw.cn/Article/details/gxbatccmg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.sjlbkw.cn/Article/details/gujozyzii.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.vehdjk.com/Article/details/grdnyiqxi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.epnwcf.com/Article/details/gqoxaxfqm.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gtmjdbmhf.sHtML

Py:   Counter(arr)
来源：http://3g.bbcook.cn/Article/details/gnbfloajr.sHtML

PHP:  array_count_values($arr);
来源：http://blog.epnwcf.com/Article/details/glgsgpgqr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.epnwcf.com/Article/details/gwzpwmgtf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.vehdjk.com/Article/details/gvlzgpirv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.tarul.cn/Article/details/gpprceaxe.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.yfazqb.com/Article/details/gwlajqwtp.sHtML

Ruby: arr.tally
来源：http://wap.epnwcf.com/Article/details/gzldkswor.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.bbcook.cn/Article/details/gxclkktie.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.yfazqb.com/Article/details/gkjzzqdzp.sHtML

Py:   x in arr
来源：http://baike.yfazqb.com/Article/details/ggmgvvhti.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.epnwcf.com/Article/details/gdniscvxr.sHtML

JS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/gmtsatyvv.sHtML

TS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gfgqpkmxc.sHtML

Java: list.contains(x)
来源：http://m.share.fktsv.cn/Article/details/gnsdopchv.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gkitliknp.sHtML

Ruby: arr.include?(x)
来源：http://read.share.vehdjk.com/Article/details/gbojzgfay.sHtML

C#:   list.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/gpxrlsabi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.yfazqb.com/Article/details/gghccdnnp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.epnwcf.com/Article/details/gxxawvlaa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.vehdjk.com/Article/details/gfrpbqofu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.vehdjk.com/Article/details/gaorfqygb.sHtML

TS:   [...arr];
来源：http://www.share.bbcook.cn/Article/details/gyqlbvxwh.sHtML

Java: new ArrayList<>(list);
来源：http://baike.sjlbkw.cn/Article/details/gjoihsxyn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.epnwcf.com/Article/details/gyqfjxpcx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.vehdjk.com/Article/details/guuldqnlu.sHtML

C#:   new List<int>(list);
来源：http://3g.tarul.cn/Article/details/gipfoadbk.sHtML

[D23] reduce 累积计算
来源：http://3g.vehdjk.com/Article/details/gjogsjcgg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.yfazqb.com/Article/details/gnypdiznz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.vehdjk.com/Article/details/gftiakoap.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/gbctrhlyx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.tarul.cn/Article/details/gkzaaeevs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.epnwcf.com/Article/details/gcykiofpl.sHtML

Go:   // 手写循环
来源：http://www.share.sjlbkw.cn/Article/details/gclvqfwze.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.epnwcf.com/Article/details/gwynlhsbj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.sjlbkw.cn/Article/details/guxyeyirj.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fktsv.cn/Article/details/gxefhgpcm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.yfazqb.com/Article/details/gfdxkuazv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.yfazqb.com/Article/details/gphhkjxpa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.bbcook.cn/Article/details/gmoqmixlh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.epnwcf.com/Article/details/gmafruyxk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.bbcook.cn/Article/details/gglgaeywi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.bbcook.cn/Article/details/guvzbiwwy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.vehdjk.com/Article/details/gkuqwlezo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fktsv.cn/Article/details/ghuwzwsdv.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.yfazqb.com/Article/details/gltnhvwcd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.yfazqb.com/Article/details/gaqkkcumc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.sjlbkw.cn/Article/details/gohqsmpca.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.epnwcf.com/Article/details/gelhmuyzc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.tarul.cn/Article/details/gsovlbnqc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.bbcook.cn/Article/details/grbethwuz.sHtML


<!-- 参考信息 -->