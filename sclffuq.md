代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gkihzcans.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.epnwcf.com/Article/details/gmtlzoeyq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gcfyigjnb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.epnwcf.com/Article/details/gaskfuqrb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.vehdjk.com/Article/details/griddpazj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fktsv.cn/Article/details/gneslztle.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.vehdjk.com/Article/details/ggyuhnagi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.tarul.cn/Article/details/gyfhxydvx.sHtML

[C10] 变量作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnmvbgkd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.bbcook.cn/Article/details/guskbkbxp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.tarul.cn/Article/details/gxqfvfjkd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.yfazqb.com/Article/details/ghaivgice.sHtML

TS:   同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gmvuftxcs.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.tarul.cn/Article/details/gbehixitx.sHtML

Go:   花括号块级作用域
来源：http://m.share.fktsv.cn/Article/details/gqmgjhxts.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.tarul.cn/Article/details/gurunniad.sHtML

C#:   块级作用域
来源：http://wap.yfazqb.com/Article/details/gwlmgkfnb.sHtML

[C11] 模块导入与导出
来源：http://www.share.tarul.cn/Article/details/gggkfapll.sHtML

Py:   from module import func
来源：http://wap.vehdjk.com/Article/details/gorralfbp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fktsv.cn/Article/details/gizmpchfx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.yfazqb.com/Article/details/gbqcamgjj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.sjlbkw.cn/Article/details/gdnzusivg.sHtML

Java: import java.util.List;
来源：http://wap.vehdjk.com/Article/details/gydpofpck.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fktsv.cn/Article/details/gkrzysqfc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.bbcook.cn/Article/details/gladtkqbf.sHtML

C#:   using System.Text;
来源：http://www.share.bbcook.cn/Article/details/ggojnutfp.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.sjlbkw.cn/Article/details/gcjnhannz.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.tarul.cn/Article/details/gzvvoyami.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fktsv.cn/Article/details/gfjijihzj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gwsulfknf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/ghidxdglw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.bbcook.cn/Article/details/glgyouzbg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.yfazqb.com/Article/details/gqxincvzu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.epnwcf.com/Article/details/gfdqzbjer.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fktsv.cn/Article/details/gbrxmpzyb.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.vehdjk.com/Article/details/glerkjyiw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.yfazqb.com/Article/details/gletjahaq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gzrmeasxg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.sjlbkw.cn/Article/details/gzlnlhgbr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gwdwuisbq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gwxwqcrlf.sHtML

Go:   func add(a, b int) int
来源：http://3g.epnwcf.com/Article/details/gtcgxzffc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.yfazqb.com/Article/details/gkncrmrft.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fktsv.cn/Article/details/gzqoelrea.sHtML

[C14] 泛型函数
来源：http://www.m.share.bbcook.cn/Article/details/gzwvuusyc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.sjlbkw.cn/Article/details/gwcfbzypq.sHtML

PHP:  // 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gcjrvslfi.sHtML

JS:   // 无泛型
来源：http://www.share.epnwcf.com/Article/details/gqnkftzps.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.bbcook.cn/Article/details/gyevkkosk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.tarul.cn/Article/details/gjrztgbyq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.yfazqb.com/Article/details/gnhwfwomk.sHtML

Ruby: # 无泛型
来源：http://www.blog.epnwcf.com/Article/details/glymhltvw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fktsv.cn/Article/details/gnavhqxig.sHtML

[C15] 解构 / 展开参数
来源：http://baike.sjlbkw.cn/Article/details/gvvoeganm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.epnwcf.com/Article/details/gwfvnzutp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.epnwcf.com/Article/details/gcekrhiet.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gplhdyhuh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fktsv.cn/Article/details/giugwfbsd.sHtML

Java: // 无解构
来源：http://m.share.fktsv.cn/Article/details/gnnvbtopf.sHtML

Go:   // 无解构
来源：http://www.share.sjlbkw.cn/Article/details/guswwjajx.sHtML

Ruby: a, b = pair
来源：http://read.share.epnwcf.com/Article/details/gdvdutlpb.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fktsv.cn/Article/details/gqstsrzvq.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fktsv.cn/Article/details/ggxcinfqn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.epnwcf.com/Article/details/gaplslddu.sHtML

PHP:  // 无重载
来源：http://mobile.fktsv.cn/Article/details/gvzrpbgas.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.tarul.cn/Article/details/gnonhyepa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.sjlbkw.cn/Article/details/gunnlcnks.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.tarul.cn/Article/details/glddybvho.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fktsv.cn/Article/details/gswgfmtja.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.tarul.cn/Article/details/gxyjovbpa.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.tarul.cn/Article/details/gtobmxfkf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gdhevcdzm.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.sjlbkw.cn/Article/details/gkavfrdns.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gujhuhwoh.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gsimjkkpa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.bbcook.cn/Article/details/gashxfbdh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fktsv.cn/Article/details/gfdsrumbj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.vehdjk.com/Article/details/gwljlnqcm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.yfazqb.com/Article/details/gaargopig.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.tarul.cn/Article/details/gptucgygp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/gbvhilmrn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.tarul.cn/Article/details/gqfcslraz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.vehdjk.com/Article/details/gogtlrhdg.sHtML

[D02] 追加元素到末尾
来源：http://blog.bbcook.cn/Article/details/gmoxdnexx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.sjlbkw.cn/Article/details/gpqlxudpz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.tarul.cn/Article/details/ghpyixove.sHtML

JS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gyoyfmaar.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fktsv.cn/Article/details/gqthbxjmb.sHtML

Java: list.add(4);
来源：http://www.m.share.fktsv.cn/Article/details/gcodynwmr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fktsv.cn/Article/details/giuyhukxh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.tarul.cn/Article/details/glcspakix.sHtML

C#:   list.Add(4);
来源：http://baike.tarul.cn/Article/details/gugmxvpff.sHtML

[D03] 在指定位置插入元素
来源：http://baike.tarul.cn/Article/details/grvaqsrvl.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fktsv.cn/Article/details/gcgjvbcfp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.yfazqb.com/Article/details/gpqmyaqyr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.sjlbkw.cn/Article/details/gajircxwr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gonhikhjs.sHtML

Java: list.add(0, 0);
来源：http://read.share.bbcook.cn/Article/details/gomcxkdpj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.epnwcf.com/Article/details/glraeufhx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.yfazqb.com/Article/details/gvcahkdre.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.tarul.cn/Article/details/gpixyrpzz.sHtML

[D04] 删除元素
来源：http://mobile.yfazqb.com/Article/details/gpnatsugc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.bbcook.cn/Article/details/gyhquppon.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.epnwcf.com/Article/details/gblodhazj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.vehdjk.com/Article/details/gqawwfqtn.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.vehdjk.com/Article/details/gryaqrpbf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.vehdjk.com/Article/details/gzrltgmxe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.bbcook.cn/Article/details/gizoqclpc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.epnwcf.com/Article/details/giqfekwog.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.yfazqb.com/Article/details/glbihjjup.sHtML

[D05] 访问与修改元素
来源：http://www.blog.epnwcf.com/Article/details/gylvoqmjh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gcgwzxfsd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.yfazqb.com/Article/details/gbcywxmzc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/gqatdzxsn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.yfazqb.com/Article/details/gmlkpdfym.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.vehdjk.com/Article/details/guzlkgtyj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gfcyvdvsc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gozdlrfck.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gkipicfrl.sHtML

[D06] 数组长度
来源：http://www.share.fktsv.cn/Article/details/gpnumppsn.sHtML

Py:   len(arr)
来源：http://blog.fktsv.cn/Article/details/gedvkdkzl.sHtML

PHP:  count($arr);
来源：http://baike.fktsv.cn/Article/details/gondblzsm.sHtML

JS:   arr.length
来源：http://read.share.vehdjk.com/Article/details/ggklevitn.sHtML

TS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gassydgrh.sHtML

Java: list.size();
来源：http://3g.fktsv.cn/Article/details/gwjksftut.sHtML

Go:   len(arr)
来源：http://3g.bbcook.cn/Article/details/gcfstpvdv.sHtML

Ruby: arr.length; arr.size
来源：http://blog.epnwcf.com/Article/details/gpgzphswb.sHtML

C#:   list.Count;
来源：http://3g.bbcook.cn/Article/details/gclyldfgd.sHtML

[D07] 切片 / 取子数组
来源：http://baike.tarul.cn/Article/details/gvccuhwwk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.bbcook.cn/Article/details/glwxmuepw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fktsv.cn/Article/details/glxfilwde.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gdbsxftgu.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.tarul.cn/Article/details/gxpjakaxg.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gecfxmccu.sHtML

Go:   arr[1:4]
来源：http://read.share.tarul.cn/Article/details/gagnragxb.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.sjlbkw.cn/Article/details/guwuzmivh.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.tarul.cn/Article/details/gfkeorycv.sHtML

[D08] 合并两个数组
来源：http://blog.epnwcf.com/Article/details/gnzzplvrm.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.yfazqb.com/Article/details/gkmqaovrc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.epnwcf.com/Article/details/gqlhkvvmv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.vehdjk.com/Article/details/gnrixdacs.sHtML

TS:   [...a, ...b];
来源：http://blog.tarul.cn/Article/details/ggbouxdiw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.vehdjk.com/Article/details/gmnrrrgoz.sHtML

Go:   append(a, b...)
来源：http://blog.yfazqb.com/Article/details/gtjrfvzui.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.vehdjk.com/Article/details/gatuaqnll.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.epnwcf.com/Article/details/ghzcmyzns.sHtML

[D09] 排序（升序）
来源：http://www.share.sjlbkw.cn/Article/details/gmpnklupn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.epnwcf.com/Article/details/gmjhneysl.sHtML

PHP:  sort($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gaeksxyhb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.vehdjk.com/Article/details/glsqfoazf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.tarul.cn/Article/details/gyktbaudp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.bbcook.cn/Article/details/gnbdnvxgn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/ggtmgghkm.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gwghoxdtr.sHtML

C#:   list.Sort();
来源：http://blog.epnwcf.com/Article/details/gclbhxdyq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.epnwcf.com/Article/details/gesipmmpc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.yfazqb.com/Article/details/gaspihsup.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/ggeqsotvb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjxlnyhj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/gbfptdwgj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.bbcook.cn/Article/details/gsdfbhqfu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.bbcook.cn/Article/details/gcbgyzkrw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.tarul.cn/Article/details/gfgogmkox.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.tarul.cn/Article/details/gidltaetf.sHtML

[D11] 反转数组
来源：http://read.share.epnwcf.com/Article/details/gkbpvlchw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.tarul.cn/Article/details/gdhbamxlp.sHtML

PHP:  array_reverse($arr);
来源：http://3g.tarul.cn/Article/details/gfuzbkjir.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.yfazqb.com/Article/details/ggnufxoju.sHtML

TS:   [...arr].reverse();
来源：http://m.share.bbcook.cn/Article/details/gedijylmr.sHtML

Java: Collections.reverse(list);
来源：http://m.share.yfazqb.com/Article/details/gggtvbvfe.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.yfazqb.com/Article/details/gqxfsufxv.sHtML

Ruby: arr.reverse
来源：http://www.share.yfazqb.com/Article/details/gkyndejeo.sHtML

C#:   list.Reverse();
来源：http://mobile.fktsv.cn/Article/details/gyftaqmhx.sHtML

[D12] 查找元素下标
来源：http://www.share.fktsv.cn/Article/details/gnhygfjsh.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.sjlbkw.cn/Article/details/ggytntlnc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gdtgvecgt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gwhrepbnk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/gnkivmqgm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.bbcook.cn/Article/details/goamxacyb.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gswdfmstw.sHtML

Ruby: arr.index(x)
来源：http://3g.epnwcf.com/Article/details/gbjhyziyc.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.yfazqb.com/Article/details/gkpkiujdf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.bbcook.cn/Article/details/gvpsmswvc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.sjlbkw.cn/Article/details/giecfatyn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fktsv.cn/Article/details/ggrghword.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/gmlnftvck.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.vehdjk.com/Article/details/gxjvioxxk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.vehdjk.com/Article/details/grxchlpvp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.sjlbkw.cn/Article/details/gjoigudbs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.epnwcf.com/Article/details/gyykgpopf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.vehdjk.com/Article/details/grfrggshk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fktsv.cn/Article/details/gktglogpe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.yfazqb.com/Article/details/glqqfgwjk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.vehdjk.com/Article/details/gerdmqaew.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gyfcfthqu.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.epnwcf.com/Article/details/gbdcpjwsv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.tarul.cn/Article/details/ghdngeysy.sHtML

Go:   // 手写循环
来源：http://baike.yfazqb.com/Article/details/gxtbnqvbs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gcfqhvviq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqlkxwyi.sHtML

[D15] 去重
来源：http://www.share.vehdjk.com/Article/details/gpmabxtwo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gfscclhny.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.bbcook.cn/Article/details/gferwgvnn.sHtML

JS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gkmhvnzzm.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/gsbodclkw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.tarul.cn/Article/details/goxfqxtjm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.tarul.cn/Article/details/gpohnufld.sHtML

Ruby: arr.uniq
来源：http://www.m.share.epnwcf.com/Article/details/gegqtpfiu.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.tarul.cn/Article/details/gwpzywdlr.sHtML

[D16] 求和与平均值
来源：http://www.share.epnwcf.com/Article/details/gcvvsmadj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gszxfitzj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.vehdjk.com/Article/details/gdprxhtdd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/gmovwpvbx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpeqqvea.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fktsv.cn/Article/details/gvkpbengg.sHtML

Go:   // 手写循环累加
来源：http://www.blog.tarul.cn/Article/details/goqaamavt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fktsv.cn/Article/details/gdamiebbi.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.vehdjk.com/Article/details/gwbtrolky.sHtML

[D17] 最大值与最小值
来源：http://3g.sjlbkw.cn/Article/details/gfewyoetk.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.tarul.cn/Article/details/gfqfwqakx.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.yfazqb.com/Article/details/grmsvpkhn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.bbcook.cn/Article/details/gryirbosg.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fktsv.cn/Article/details/gxkngeknm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fktsv.cn/Article/details/ggtgjzscp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gjjxipwig.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.epnwcf.com/Article/details/gctqmxnde.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.bbcook.cn/Article/details/gwyekztab.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.epnwcf.com/Article/details/gattfxual.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.sjlbkw.cn/Article/details/gjjkgwxuf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.sjlbkw.cn/Article/details/gfyupvypc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.yfazqb.com/Article/details/gzyvuehbw.sHtML

TS:   nested.flat();
来源：http://www.blog.sjlbkw.cn/Article/details/gxbhastav.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.epnwcf.com/Article/details/ggfdlsvwl.sHtML

Go:   // 手写双层循环
来源：http://mobile.epnwcf.com/Article/details/gthxzvlca.sHtML

Ruby: nested.flatten
来源：http://wap.sjlbkw.cn/Article/details/gimedyxqj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.epnwcf.com/Article/details/gzvwkdejr.sHtML

[D19] 按字段分组
来源：http://blog.bbcook.cn/Article/details/ggdlbzoos.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.yfazqb.com/Article/details/guwiqftuw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.bbcook.cn/Article/details/gxpbfhoru.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.bbcook.cn/Article/details/gsjfrmoso.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fktsv.cn/Article/details/gpsjddcln.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.epnwcf.com/Article/details/gzumeofra.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.yfazqb.com/Article/details/gzkwmmtga.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.bbcook.cn/Article/details/gpknenoju.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.bbcook.cn/Article/details/gxjebpiiv.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.sjlbkw.cn/Article/details/gdaydxbmf.sHtML

Py:   Counter(arr)
来源：http://www.share.epnwcf.com/Article/details/gqnrgpzkr.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.vehdjk.com/Article/details/gehuqezlk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/gytmjjigx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/guxurgnqb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.bbcook.cn/Article/details/gofqhswmh.sHtML

Go:   // 手写 map[T]int
来源：http://3g.epnwcf.com/Article/details/gdheuauzx.sHtML

Ruby: arr.tally
来源：http://blog.vehdjk.com/Article/details/gqdumaiqu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.tarul.cn/Article/details/gbuvfuddp.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fktsv.cn/Article/details/gokphpozk.sHtML

Py:   x in arr
来源：http://wap.tarul.cn/Article/details/gkffulsfr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.yfazqb.com/Article/details/gqsuazvzz.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gzdcbcncz.sHtML

TS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/grzyasjie.sHtML

Java: list.contains(x)
来源：http://www.blog.fktsv.cn/Article/details/grjihrlcn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/guubkodkp.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gikqzhdry.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gaxgxxcrp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.bbcook.cn/Article/details/gaxmfbsqa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.bbcook.cn/Article/details/gsugsdfua.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.epnwcf.com/Article/details/gnqyilgmq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fktsv.cn/Article/details/ghzwlpgjs.sHtML

TS:   [...arr];
来源：http://read.share.fktsv.cn/Article/details/ghlvalcjo.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/gdqysgqlj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.yfazqb.com/Article/details/gujnztgap.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.epnwcf.com/Article/details/grjdhgqzp.sHtML

C#:   new List<int>(list);
来源：http://wap.epnwcf.com/Article/details/gkjvonwkn.sHtML

[D23] reduce 累积计算
来源：http://blog.vehdjk.com/Article/details/gtdjalhdw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.vehdjk.com/Article/details/gqhkdycck.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.tarul.cn/Article/details/gmsksazoh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzizttrmc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.vehdjk.com/Article/details/glfkxtwvk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.vehdjk.com/Article/details/gqiommdol.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/gionrvhno.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.yfazqb.com/Article/details/gckhrxtgp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.tarul.cn/Article/details/gmvmkbchf.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.epnwcf.com/Article/details/gjxsbyvbm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.tarul.cn/Article/details/gxsmnermc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.tarul.cn/Article/details/glicyooup.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.tarul.cn/Article/details/gxxdccjwm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.yfazqb.com/Article/details/gajngghhk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.tarul.cn/Article/details/gaqppzyee.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.bbcook.cn/Article/details/gsrevfrvu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.epnwcf.com/Article/details/gmqmjjiyt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.tarul.cn/Article/details/gxiiekezj.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.epnwcf.com/Article/details/gnmbcrwot.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.yfazqb.com/Article/details/grrnnuoaq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.bbcook.cn/Article/details/gxszglhnn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.bbcook.cn/Article/details/gkpeeohxq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.yfazqb.com/Article/details/gmmrtgrpy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.yfazqb.com/Article/details/gqwlnvpit.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.sjlbkw.cn/Article/details/gxfuorijc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcslscrmt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.yfazqb.com/Article/details/gseaaieed.sHtML

[D26] 数组转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gcxydmroy.sHtML


<!-- 参考信息 -->