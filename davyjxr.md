代发 wailian999

[C10] 变量作用域
来源：http://blog.bbcook.cn/Article/details/gckzipwwq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fktsv.cn/Article/details/gpaauiqnd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.yfazqb.com/Article/details/ggtpxwehb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.tarul.cn/Article/details/gknpexmoi.sHtML

TS:   同 JS
来源：http://wap.sjlbkw.cn/Article/details/gefnqaelg.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.epnwcf.com/Article/details/gqbguezar.sHtML

Go:   花括号块级作用域
来源：http://www.share.tarul.cn/Article/details/gefgyylqm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fktsv.cn/Article/details/gwhlytfuy.sHtML

C#:   块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtnrpdax.sHtML

[C11] 模块导入与导出
来源：http://wap.fktsv.cn/Article/details/grbaxbcae.sHtML

Py:   from module import func
来源：http://www.m.share.vehdjk.com/Article/details/gvhgsggfx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fktsv.cn/Article/details/guqezfyre.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.yfazqb.com/Article/details/gofxzxcjo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fktsv.cn/Article/details/gkcqrllvd.sHtML

Java: import java.util.List;
来源：http://3g.tarul.cn/Article/details/ghckydtwt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.epnwcf.com/Article/details/gcdeuolqu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.tarul.cn/Article/details/gchcxncfi.sHtML

C#:   using System.Text;
来源：http://wap.sjlbkw.cn/Article/details/gkbhrcpxs.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.sjlbkw.cn/Article/details/gmlntyozl.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.epnwcf.com/Article/details/gsxawjxyg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.vehdjk.com/Article/details/gnxbwgttz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/gyadtqsmt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/gqnyvvvlz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.vehdjk.com/Article/details/goocnqnaa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.vehdjk.com/Article/details/ggfsbhkog.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fktsv.cn/Article/details/gfsulpols.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.bbcook.cn/Article/details/gdfukekpp.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fktsv.cn/Article/details/gihtffpde.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.sjlbkw.cn/Article/details/gmufcxxgu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gqojifkin.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.tarul.cn/Article/details/gpmxadime.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gfehbsies.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gokgdtapf.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.epnwcf.com/Article/details/gjpuhdvsh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fktsv.cn/Article/details/gqxeyqdoj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.epnwcf.com/Article/details/gizdisxrj.sHtML

[C14] 泛型函数
来源：http://3g.vehdjk.com/Article/details/gkvyptxip.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fktsv.cn/Article/details/gwyolucae.sHtML

PHP:  // 无泛型
来源：http://read.share.vehdjk.com/Article/details/gibxqogqj.sHtML

JS:   // 无泛型
来源：http://m.share.tarul.cn/Article/details/guvfldqdd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.sjlbkw.cn/Article/details/gviklhfdh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.yfazqb.com/Article/details/gfuaxipes.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.epnwcf.com/Article/details/gthesienr.sHtML

Ruby: # 无泛型
来源：http://blog.tarul.cn/Article/details/gmxltdfoh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.tarul.cn/Article/details/gggcpkoyg.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.yfazqb.com/Article/details/gkdpmosxb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fktsv.cn/Article/details/gsotycqez.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.bbcook.cn/Article/details/geejjwtqr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/gndgsiksi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.tarul.cn/Article/details/gtwafqngk.sHtML

Java: // 无解构
来源：http://wap.epnwcf.com/Article/details/gjfyohchi.sHtML

Go:   // 无解构
来源：http://www.blog.epnwcf.com/Article/details/gbvftvdkc.sHtML

Ruby: a, b = pair
来源：http://mobile.vehdjk.com/Article/details/gjyiupwbe.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.bbcook.cn/Article/details/gllqmdbxk.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.sjlbkw.cn/Article/details/ggribcqch.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.tarul.cn/Article/details/gmnugjhpp.sHtML

PHP:  // 无重载
来源：http://mobile.fktsv.cn/Article/details/gerirjqwl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.bbcook.cn/Article/details/gxouxwqlj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fktsv.cn/Article/details/gxvtblimr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.tarul.cn/Article/details/gcavtsotp.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.vehdjk.com/Article/details/gwaoobucd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.tarul.cn/Article/details/gunjgmeko.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.bbcook.cn/Article/details/gddozhltm.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gwtesttkn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.yfazqb.com/Article/details/gkodenpfi.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gqodxfhbj.sHtML

[D01] 创建数组 / 列表
来源：http://3g.tarul.cn/Article/details/gkdvmnbru.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.sjlbkw.cn/Article/details/ggaxkksfy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/gbrswvcce.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fktsv.cn/Article/details/gcevaxhdu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.vehdjk.com/Article/details/gwzccrlah.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.tarul.cn/Article/details/gpbexmgbt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.yfazqb.com/Article/details/gutuwtjke.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gsvqwsyos.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.tarul.cn/Article/details/gsnidjkrf.sHtML

[D02] 追加元素到末尾
来源：http://www.share.tarul.cn/Article/details/ghxlemwmf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.tarul.cn/Article/details/gohpffehf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fktsv.cn/Article/details/gwiujvlkl.sHtML

JS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/gldpljovz.sHtML

TS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/gyyksozyz.sHtML

Java: list.add(4);
来源：http://read.share.tarul.cn/Article/details/gweinoegp.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.sjlbkw.cn/Article/details/giwiuhout.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.vehdjk.com/Article/details/goztcgsdl.sHtML

C#:   list.Add(4);
来源：http://3g.epnwcf.com/Article/details/glimyxnvu.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.epnwcf.com/Article/details/gppgurdge.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.vehdjk.com/Article/details/gfiqzegoj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.epnwcf.com/Article/details/gvazarpay.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.tarul.cn/Article/details/ggwjuukom.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.bbcook.cn/Article/details/gondzzuix.sHtML

Java: list.add(0, 0);
来源：http://m.share.fktsv.cn/Article/details/gawddphgx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.epnwcf.com/Article/details/gfeqxffow.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.epnwcf.com/Article/details/goagcjwmb.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.vehdjk.com/Article/details/gvhfcjuzs.sHtML

[D04] 删除元素
来源：http://m.share.yfazqb.com/Article/details/glzuwkddy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fktsv.cn/Article/details/guuwodpyi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.yfazqb.com/Article/details/geztpmwwk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.epnwcf.com/Article/details/gnootyuun.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.yfazqb.com/Article/details/ggxohancn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.bbcook.cn/Article/details/grrwefsvp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.vehdjk.com/Article/details/gykdamdwb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.vehdjk.com/Article/details/gyblqjerm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.epnwcf.com/Article/details/gfikxgypc.sHtML

[D05] 访问与修改元素
来源：http://baike.yfazqb.com/Article/details/ggxpcjkju.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gjiqvpbzs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzwyltcl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gjqjzpsxf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.bbcook.cn/Article/details/ghvwbvmou.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.tarul.cn/Article/details/geckqsqvz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/guuguqenf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gudevqfpp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gzurtqgax.sHtML

[D06] 数组长度
来源：http://3g.tarul.cn/Article/details/gjillanob.sHtML

Py:   len(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gdouitzel.sHtML

PHP:  count($arr);
来源：http://m.share.bbcook.cn/Article/details/gfxcjbjhs.sHtML

JS:   arr.length
来源：http://read.share.sjlbkw.cn/Article/details/gqohmtkuw.sHtML

TS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/ghgghvfmo.sHtML

Java: list.size();
来源：http://mobile.epnwcf.com/Article/details/gfrabexwz.sHtML

Go:   len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gqshmvzcx.sHtML

Ruby: arr.length; arr.size
来源：http://blog.epnwcf.com/Article/details/gcpsldnbe.sHtML

C#:   list.Count;
来源：http://m.share.bbcook.cn/Article/details/gmwkgwfdv.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fktsv.cn/Article/details/geqagvnom.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.yfazqb.com/Article/details/gftqnvdst.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.bbcook.cn/Article/details/gppwdkwfa.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.bbcook.cn/Article/details/guetqgiqg.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/gshcwlvxe.sHtML

Java: list.subList(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gzasiuhtx.sHtML

Go:   arr[1:4]
来源：http://www.share.bbcook.cn/Article/details/gahxwadxo.sHtML

Ruby: arr[1, 3]
来源：http://blog.tarul.cn/Article/details/gizkppidg.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.yfazqb.com/Article/details/gpfjpcjyx.sHtML

[D08] 合并两个数组
来源：http://mobile.tarul.cn/Article/details/gifwnzunu.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fktsv.cn/Article/details/gmefvhbov.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.tarul.cn/Article/details/gvnegkpsr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.epnwcf.com/Article/details/gvleqgmsn.sHtML

TS:   [...a, ...b];
来源：http://wap.sjlbkw.cn/Article/details/gpgdbkkwj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.epnwcf.com/Article/details/gmvfpnfuf.sHtML

Go:   append(a, b...)
来源：http://baike.epnwcf.com/Article/details/gjpjzqrih.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.yfazqb.com/Article/details/gacmszezq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gyyraszzr.sHtML

[D09] 排序（升序）
来源：http://3g.sjlbkw.cn/Article/details/gypuajexa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.vehdjk.com/Article/details/grqeogkts.sHtML

PHP:  sort($arr);
来源：http://www.m.share.tarul.cn/Article/details/gzqpdvvxl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.vehdjk.com/Article/details/gsrkatwxm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.tarul.cn/Article/details/goflsvuez.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.tarul.cn/Article/details/gkkkbocoo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.bbcook.cn/Article/details/ghamifonx.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/gqvfusosi.sHtML

C#:   list.Sort();
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjxglhca.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvvddruh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.sjlbkw.cn/Article/details/gowqufyzb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.vehdjk.com/Article/details/gbqahqlxi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/gvwjlowsy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/grrwrketg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.vehdjk.com/Article/details/gmsurjagk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.epnwcf.com/Article/details/gvshnrjqy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.bbcook.cn/Article/details/ghjzsylnr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.bbcook.cn/Article/details/gzawahmkt.sHtML

[D11] 反转数组
来源：http://www.share.bbcook.cn/Article/details/gafxdcxwq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.bbcook.cn/Article/details/ggltxmdyn.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/gcqhpaaww.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.sjlbkw.cn/Article/details/gwgeomkrc.sHtML

TS:   [...arr].reverse();
来源：http://m.share.vehdjk.com/Article/details/gogkijqqs.sHtML

Java: Collections.reverse(list);
来源：http://wap.bbcook.cn/Article/details/gxxclmxdm.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.epnwcf.com/Article/details/gmlapvlaj.sHtML

Ruby: arr.reverse
来源：http://3g.yfazqb.com/Article/details/gezelswij.sHtML

C#:   list.Reverse();
来源：http://mobile.tarul.cn/Article/details/gvjnnsiga.sHtML

[D12] 查找元素下标
来源：http://www.blog.fktsv.cn/Article/details/guovegvno.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.vehdjk.com/Article/details/geryuxghj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fktsv.cn/Article/details/gigucqaoh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/ghkowcmpd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/galfcahkx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.bbcook.cn/Article/details/gvrknrzfq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gqsumhupo.sHtML

Ruby: arr.index(x)
来源：http://m.share.yfazqb.com/Article/details/guipswbkm.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.yfazqb.com/Article/details/grcxciifi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.yfazqb.com/Article/details/grfnqbnad.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.epnwcf.com/Article/details/gdkcbjdek.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.tarul.cn/Article/details/gzypmnsth.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.tarul.cn/Article/details/gigiabgxv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gnqohcdmg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.sjlbkw.cn/Article/details/gndrerhah.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.tarul.cn/Article/details/gqqprpykv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.bbcook.cn/Article/details/gnesxtgad.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.tarul.cn/Article/details/gmehuxdzb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.tarul.cn/Article/details/gadzblkzk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/ghcvzzbqy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.yfazqb.com/Article/details/ggcfkyuqm.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/ggiknolov.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/gvojhgucx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gtslnbbmo.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/gkyztevxa.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.tarul.cn/Article/details/gxzzpmxoi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.bbcook.cn/Article/details/gmhoxjrgs.sHtML

[D15] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkuioxum.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.sjlbkw.cn/Article/details/geouzdpna.sHtML

PHP:  array_unique($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gsthkhunx.sHtML

JS:   [...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gssijvojf.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gifkrljwz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.sjlbkw.cn/Article/details/goeterlrp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.yfazqb.com/Article/details/gkcozgmfx.sHtML

Ruby: arr.uniq
来源：http://mobile.sjlbkw.cn/Article/details/ggviuqgts.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.tarul.cn/Article/details/ggnulfyqn.sHtML

[D16] 求和与平均值
来源：http://m.share.epnwcf.com/Article/details/gznncogeg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gloppktkb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gfkcbnorl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.bbcook.cn/Article/details/giowjodxx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/gekagcmni.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.tarul.cn/Article/details/gadsoyruw.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/gittxoels.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.yfazqb.com/Article/details/glesstdfu.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.bbcook.cn/Article/details/gjrraqnrr.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/gsyyzgunz.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.tarul.cn/Article/details/gyjyludhh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.tarul.cn/Article/details/gfvtxpsii.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.bbcook.cn/Article/details/gsxysyzob.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.yfazqb.com/Article/details/gpavbaosd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.yfazqb.com/Article/details/gjkvvrnje.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.vehdjk.com/Article/details/gynvtxplk.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.sjlbkw.cn/Article/details/gsdkprzqb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.sjlbkw.cn/Article/details/gttwzhgtz.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.bbcook.cn/Article/details/gztuwutrs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.vehdjk.com/Article/details/gvjxbtaxx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.sjlbkw.cn/Article/details/gpuqqrqvd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.sjlbkw.cn/Article/details/gevlvggyb.sHtML

TS:   nested.flat();
来源：http://wap.vehdjk.com/Article/details/glrghqcri.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.bbcook.cn/Article/details/gyjeizmzc.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.tarul.cn/Article/details/gjkbfcycw.sHtML

Ruby: nested.flatten
来源：http://baike.sjlbkw.cn/Article/details/gnqeawksg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.bbcook.cn/Article/details/gzymndkdy.sHtML

[D19] 按字段分组
来源：http://www.blog.tarul.cn/Article/details/gpqncxeek.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.bbcook.cn/Article/details/ggcmqgafh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.epnwcf.com/Article/details/gewppiwpr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.vehdjk.com/Article/details/gwzdbudei.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.epnwcf.com/Article/details/gpuihdolm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.epnwcf.com/Article/details/gamicfrrr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fktsv.cn/Article/details/gbwuvsiuv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.vehdjk.com/Article/details/gsymxovdl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.tarul.cn/Article/details/gjdpsvvrf.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.sjlbkw.cn/Article/details/grjsqyppl.sHtML

Py:   Counter(arr)
来源：http://www.blog.fktsv.cn/Article/details/geyxtoqjz.sHtML

PHP:  array_count_values($arr);
来源：http://3g.yfazqb.com/Article/details/gkoxzlvsp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gvebukxjc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gpzbjzfqd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.vehdjk.com/Article/details/gdmaajkis.sHtML

Go:   // 手写 map[T]int
来源：http://blog.tarul.cn/Article/details/grqnhtkco.sHtML

Ruby: arr.tally
来源：http://blog.yfazqb.com/Article/details/gzojbagky.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.sjlbkw.cn/Article/details/gesuvogmi.sHtML

[D21] 判断是否包含某元素
来源：http://wap.epnwcf.com/Article/details/gfiavynmo.sHtML

Py:   x in arr
来源：http://www.m.share.fktsv.cn/Article/details/gaqsmwhce.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fktsv.cn/Article/details/gkpzwhrov.sHtML

JS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gjlljktqx.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/goritsnsa.sHtML

Java: list.contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gmwjokmik.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrnsswmi.sHtML

Ruby: arr.include?(x)
来源：http://read.share.yfazqb.com/Article/details/gsguvirwd.sHtML

C#:   list.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gtzoydwsl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.tarul.cn/Article/details/gryrghina.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.yfazqb.com/Article/details/gtqylgurl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.bbcook.cn/Article/details/gruioyrpv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.yfazqb.com/Article/details/gjghlvjlp.sHtML

TS:   [...arr];
来源：http://mobile.tarul.cn/Article/details/gqovpupba.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.vehdjk.com/Article/details/gwsmunhwc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.epnwcf.com/Article/details/gpwawrlih.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.yfazqb.com/Article/details/gydjwbjmq.sHtML

C#:   new List<int>(list);
来源：http://read.share.epnwcf.com/Article/details/gylottnwb.sHtML

[D23] reduce 累积计算
来源：http://www.blog.sjlbkw.cn/Article/details/gvjcplthh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.sjlbkw.cn/Article/details/gfoausaki.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fktsv.cn/Article/details/gpzfmyvuy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/glhbgpkaz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gmjkyqhov.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.bbcook.cn/Article/details/gsuxmffeh.sHtML

Go:   // 手写循环
来源：http://3g.fktsv.cn/Article/details/goqzzfbgq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.tarul.cn/Article/details/gjvvqutwk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.bbcook.cn/Article/details/ghfunzdqo.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.yfazqb.com/Article/details/gedkbyemq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fktsv.cn/Article/details/glwnanlkx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.tarul.cn/Article/details/gzisgdkvg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.tarul.cn/Article/details/gybmaqdpe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fktsv.cn/Article/details/gdphbkeki.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.sjlbkw.cn/Article/details/gayyzorkb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.tarul.cn/Article/details/gwtkaauld.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.sjlbkw.cn/Article/details/ggjxxjkdq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.yfazqb.com/Article/details/gevzjkbuk.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.sjlbkw.cn/Article/details/gvllsgttk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.tarul.cn/Article/details/ghemoelvh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.yfazqb.com/Article/details/gtmrwrmmc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.bbcook.cn/Article/details/giacrhjkf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.tarul.cn/Article/details/gdqpedhdd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.vehdjk.com/Article/details/ggvemdrvm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.yfazqb.com/Article/details/guokqnooi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.bbcook.cn/Article/details/gxbteispr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.tarul.cn/Article/details/grgucnaii.sHtML

[D26] 数组转字符串
来源：http://wap.yfazqb.com/Article/details/gdtfimnih.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.bbcook.cn/Article/details/gqmotnjpt.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.sjlbkw.cn/Article/details/ggoifcplp.sHtML

JS:   arr.join(", ")
来源：http://baike.fktsv.cn/Article/details/gfvzsmjdl.sHtML

TS:   arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gnioewhuv.sHtML

Java: String.join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gnlqwmtcj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.sjlbkw.cn/Article/details/gsgtvsajg.sHtML

Ruby: arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gdknrfmkv.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/gfrlstfuz.sHtML


<!-- 参考信息 -->