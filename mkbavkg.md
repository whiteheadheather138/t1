代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/glxsnkdrm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.yfazqb.com/Article/details/gozhpnocq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/gtlwenokq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.bbcook.cn/Article/details/gfgjtfudy.sHtML

[C10] 变量作用域
来源：http://www.m.share.tarul.cn/Article/details/gnonlxvji.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.epnwcf.com/Article/details/gwizrxqae.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.bbcook.cn/Article/details/ghazbvjai.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.epnwcf.com/Article/details/glhmvjawk.sHtML

TS:   同 JS
来源：http://3g.vehdjk.com/Article/details/gmksxhgbb.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/giftjxghv.sHtML

Go:   花括号块级作用域
来源：http://mobile.yfazqb.com/Article/details/gohhzcbns.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.bbcook.cn/Article/details/gbuswniqe.sHtML

C#:   块级作用域
来源：http://baike.yfazqb.com/Article/details/goguvjcxb.sHtML

[C11] 模块导入与导出
来源：http://blog.fktsv.cn/Article/details/gcvwgvucb.sHtML

Py:   from module import func
来源：http://read.share.tarul.cn/Article/details/gnbupjcfg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.epnwcf.com/Article/details/gskzngtzf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/gjnzwdgfy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fktsv.cn/Article/details/gljunabwx.sHtML

Java: import java.util.List;
来源：http://www.share.tarul.cn/Article/details/ghfbaaysn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.tarul.cn/Article/details/gbbvptkic.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.sjlbkw.cn/Article/details/gblothbex.sHtML

C#:   using System.Text;
来源：http://wap.tarul.cn/Article/details/gwosgoonp.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fktsv.cn/Article/details/gwddftsew.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.sjlbkw.cn/Article/details/gtdwdlnwc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.tarul.cn/Article/details/girxpkxzt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/gszekzcmy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fktsv.cn/Article/details/gflnriigr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.sjlbkw.cn/Article/details/gclqzfjvt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.vehdjk.com/Article/details/gpavppdhe.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.bbcook.cn/Article/details/gnfaqjtce.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.epnwcf.com/Article/details/gjmqvlpzz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.sjlbkw.cn/Article/details/gtyldgskv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.epnwcf.com/Article/details/gybeqlkdq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gmvefuvlq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.epnwcf.com/Article/details/gqtskodkq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gfsebfgol.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gdklrqlrn.sHtML

Go:   func add(a, b int) int
来源：http://m.share.epnwcf.com/Article/details/gbwwxlxry.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.yfazqb.com/Article/details/gfidchghq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fktsv.cn/Article/details/ghznqwfmw.sHtML

[C14] 泛型函数
来源：http://blog.yfazqb.com/Article/details/ggmeokgro.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fktsv.cn/Article/details/gcoapdkcw.sHtML

PHP:  // 无泛型
来源：http://www.blog.vehdjk.com/Article/details/ghnndretk.sHtML

JS:   // 无泛型
来源：http://wap.tarul.cn/Article/details/gbfvoccqm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.bbcook.cn/Article/details/goqiepjzr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.bbcook.cn/Article/details/gfzpadjcv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.tarul.cn/Article/details/gjpbpyoqb.sHtML

Ruby: # 无泛型
来源：http://3g.tarul.cn/Article/details/gohxyaadk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.yfazqb.com/Article/details/gtotpquzv.sHtML

[C15] 解构 / 展开参数
来源：http://baike.sjlbkw.cn/Article/details/gzjokyojx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.yfazqb.com/Article/details/gxkcqvjts.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.vehdjk.com/Article/details/gkvyyxikk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gwozdwbez.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.epnwcf.com/Article/details/gmkniuefn.sHtML

Java: // 无解构
来源：http://3g.epnwcf.com/Article/details/grplcjfwe.sHtML

Go:   // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/gybzufrti.sHtML

Ruby: a, b = pair
来源：http://baike.sjlbkw.cn/Article/details/gmvfoxbyw.sHtML

C#:   var (a, b) = pair;
来源：http://3g.sjlbkw.cn/Article/details/gdmjkzvyu.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.vehdjk.com/Article/details/gvrtsbowf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.epnwcf.com/Article/details/gwwgweyra.sHtML

PHP:  // 无重载
来源：http://read.share.tarul.cn/Article/details/gzlfnmivo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.yfazqb.com/Article/details/glzropnch.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.tarul.cn/Article/details/gorhuzylx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.bbcook.cn/Article/details/gxjbxlecz.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/gbwxdjcls.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.tarul.cn/Article/details/gvfylcphc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.tarul.cn/Article/details/gfmleaigg.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggwqgjnvo.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.epnwcf.com/Article/details/gdynhjcit.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gtscauxzg.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/giejcrpin.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.epnwcf.com/Article/details/gicshykom.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.yfazqb.com/Article/details/gystqakzm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.yfazqb.com/Article/details/gmrffeaeu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.tarul.cn/Article/details/gmpbpvpkl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.epnwcf.com/Article/details/gsnqqrizg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.yfazqb.com/Article/details/givttvdvk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gszkcolby.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.sjlbkw.cn/Article/details/gnsoxehmn.sHtML

[D02] 追加元素到末尾
来源：http://blog.epnwcf.com/Article/details/gliqxetqm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.epnwcf.com/Article/details/gmglpryww.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.epnwcf.com/Article/details/giwpmzgyn.sHtML

JS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/gnohiplbe.sHtML

TS:   arr.push(4);
来源：http://3g.tarul.cn/Article/details/gzgpahond.sHtML

Java: list.add(4);
来源：http://www.m.share.yfazqb.com/Article/details/gcsedoxtm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fktsv.cn/Article/details/gwxmlfqzx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.epnwcf.com/Article/details/gsymzjatb.sHtML

C#:   list.Add(4);
来源：http://www.m.share.yfazqb.com/Article/details/gmajxvlrk.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.tarul.cn/Article/details/gbdpglpta.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.bbcook.cn/Article/details/gwfrwvphi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.sjlbkw.cn/Article/details/gckhhkqxq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.epnwcf.com/Article/details/gtvxjohgk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.epnwcf.com/Article/details/ggtncrywd.sHtML

Java: list.add(0, 0);
来源：http://blog.vehdjk.com/Article/details/gjucamonk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.epnwcf.com/Article/details/gqxqolkno.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fktsv.cn/Article/details/gtbfjeerc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gbrpqratx.sHtML

[D04] 删除元素
来源：http://mobile.tarul.cn/Article/details/gqqoxmiyj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.sjlbkw.cn/Article/details/gqfwotxnz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.yfazqb.com/Article/details/grfcfkjby.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.bbcook.cn/Article/details/gchqrirpd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.yfazqb.com/Article/details/glcxhdtbe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.yfazqb.com/Article/details/ggyjvufzs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.sjlbkw.cn/Article/details/gcwfeiwxw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.epnwcf.com/Article/details/gjudooclx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fktsv.cn/Article/details/giosbaaiu.sHtML

[D05] 访问与修改元素
来源：http://mobile.epnwcf.com/Article/details/ghqykpkwm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gdvecxkdj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gyrjfoynh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gndblscco.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.tarul.cn/Article/details/gqoffgfrp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fktsv.cn/Article/details/gtjccohaq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gvszlferd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gqgfvpvll.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gelkjmsaj.sHtML

[D06] 数组长度
来源：http://3g.vehdjk.com/Article/details/gjbmibotf.sHtML

Py:   len(arr)
来源：http://wap.yfazqb.com/Article/details/gtolmdkld.sHtML

PHP:  count($arr);
来源：http://mobile.bbcook.cn/Article/details/gknjtwyzh.sHtML

JS:   arr.length
来源：http://www.blog.vehdjk.com/Article/details/gchmtfffu.sHtML

TS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/gzsjdlrwu.sHtML

Java: list.size();
来源：http://read.share.tarul.cn/Article/details/gzshbxpoc.sHtML

Go:   len(arr)
来源：http://www.share.tarul.cn/Article/details/gsdiabaqm.sHtML

Ruby: arr.length; arr.size
来源：http://blog.yfazqb.com/Article/details/gmnbetlxj.sHtML

C#:   list.Count;
来源：http://www.share.vehdjk.com/Article/details/ghevfpxyy.sHtML

[D07] 切片 / 取子数组
来源：http://blog.yfazqb.com/Article/details/gphrrisnm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.bbcook.cn/Article/details/gkhsoxdds.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gtehnruht.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gaucyrnna.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.tarul.cn/Article/details/gakhivjgx.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gxbspngqt.sHtML

Go:   arr[1:4]
来源：http://read.share.fktsv.cn/Article/details/gnzcllxxu.sHtML

Ruby: arr[1, 3]
来源：http://baike.bbcook.cn/Article/details/ggzwgikia.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.tarul.cn/Article/details/ggchdobzg.sHtML

[D08] 合并两个数组
来源：http://m.share.vehdjk.com/Article/details/gcfsjiwgf.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.yfazqb.com/Article/details/gbngielvm.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.yfazqb.com/Article/details/giyiexctj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.yfazqb.com/Article/details/gvzlzahyw.sHtML

TS:   [...a, ...b];
来源：http://baike.epnwcf.com/Article/details/gfceiidya.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.yfazqb.com/Article/details/gksydmjgh.sHtML

Go:   append(a, b...)
来源：http://m.share.sjlbkw.cn/Article/details/ghiewexvk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.yfazqb.com/Article/details/gnzxazuud.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gbknqbbqu.sHtML

[D09] 排序（升序）
来源：http://wap.sjlbkw.cn/Article/details/gnscfyigx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/gufdizipj.sHtML

PHP:  sort($arr);
来源：http://baike.vehdjk.com/Article/details/gshdikvky.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fktsv.cn/Article/details/glkrjeqeo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.vehdjk.com/Article/details/gbwozvjuu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.bbcook.cn/Article/details/gvdwvzkmp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.sjlbkw.cn/Article/details/grgedpfmi.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/guzhncvai.sHtML

C#:   list.Sort();
来源：http://m.share.fktsv.cn/Article/details/gfmrcelmj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.tarul.cn/Article/details/gkjqgkdoh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fktsv.cn/Article/details/gqpiqxjmp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.bbcook.cn/Article/details/gplsygfay.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.epnwcf.com/Article/details/ghimoliva.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gxhurnzrp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.sjlbkw.cn/Article/details/ghshlbtby.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fktsv.cn/Article/details/geyjhwcgh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.epnwcf.com/Article/details/glxvlukaw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fktsv.cn/Article/details/gmrtxewlw.sHtML

[D11] 反转数组
来源：http://www.share.bbcook.cn/Article/details/gcvhfztaw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.vehdjk.com/Article/details/gavhpebtg.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fktsv.cn/Article/details/gyczomric.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.epnwcf.com/Article/details/gotzpjtei.sHtML

TS:   [...arr].reverse();
来源：http://www.share.tarul.cn/Article/details/ghrduyqfy.sHtML

Java: Collections.reverse(list);
来源：http://baike.vehdjk.com/Article/details/gouckqrlu.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.vehdjk.com/Article/details/gpezqbrvr.sHtML

Ruby: arr.reverse
来源：http://m.share.fktsv.cn/Article/details/gstqsjbvo.sHtML

C#:   list.Reverse();
来源：http://www.share.yfazqb.com/Article/details/gwksvfzso.sHtML

[D12] 查找元素下标
来源：http://mobile.sjlbkw.cn/Article/details/glbakpfjd.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.bbcook.cn/Article/details/gzchgmybs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.vehdjk.com/Article/details/gvsogihdl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.epnwcf.com/Article/details/gqwqrdnhs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/goirdyefw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.epnwcf.com/Article/details/gybcycrna.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gzkyifktf.sHtML

Ruby: arr.index(x)
来源：http://baike.yfazqb.com/Article/details/gmbviitks.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fktsv.cn/Article/details/gzhyeqten.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.vehdjk.com/Article/details/gcjndxoyq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fktsv.cn/Article/details/ghvqrmnnh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.tarul.cn/Article/details/gzkxqkcao.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.epnwcf.com/Article/details/gzhxlkzxe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/gdcickytx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fktsv.cn/Article/details/gacddtuqw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fktsv.cn/Article/details/gknksotnz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.bbcook.cn/Article/details/gnncbrjmx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.vehdjk.com/Article/details/gswbvtqxw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.tarul.cn/Article/details/gvnpbmdxm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fktsv.cn/Article/details/grjvjwpra.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.yfazqb.com/Article/details/gumqultpf.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.yfazqb.com/Article/details/gmuowuxcb.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.bbcook.cn/Article/details/ggvfhiqsn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.bbcook.cn/Article/details/gbsfngsst.sHtML

Go:   // 手写循环
来源：http://wap.epnwcf.com/Article/details/gzhhhpluc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gvvaywbrc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gdvosdooz.sHtML

[D15] 去重
来源：http://www.share.bbcook.cn/Article/details/gyxbglemo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.bbcook.cn/Article/details/gbltyvtdb.sHtML

PHP:  array_unique($arr);
来源：http://baike.vehdjk.com/Article/details/gbyrnnopq.sHtML

JS:   [...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gfbwbhyxm.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/grsedblfp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.bbcook.cn/Article/details/gaqewpjxf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.vehdjk.com/Article/details/gsuwvpcbi.sHtML

Ruby: arr.uniq
来源：http://mobile.bbcook.cn/Article/details/gudhcsvnk.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.vehdjk.com/Article/details/gnthyupgo.sHtML

[D16] 求和与平均值
来源：http://3g.sjlbkw.cn/Article/details/gluurctfk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.yfazqb.com/Article/details/gmvystytd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.epnwcf.com/Article/details/genrwgumw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/gyhnnmxzh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gfwgcoaen.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.vehdjk.com/Article/details/gbaxebzzw.sHtML

Go:   // 手写循环累加
来源：http://m.share.epnwcf.com/Article/details/gzadmtfeh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fktsv.cn/Article/details/gktjwjypb.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.yfazqb.com/Article/details/gzgmdophw.sHtML

[D17] 最大值与最小值
来源：http://mobile.vehdjk.com/Article/details/giwcenosd.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.yfazqb.com/Article/details/guyikhbnp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gzdelletx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.bbcook.cn/Article/details/gqbyvjana.sHtML

TS:   Math.max(...arr);
来源：http://mobile.sjlbkw.cn/Article/details/gdiaqolea.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.yfazqb.com/Article/details/gzfcpagwq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gnqbibsvq.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fktsv.cn/Article/details/gzafhnjdr.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.vehdjk.com/Article/details/gaehmzqcz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.tarul.cn/Article/details/guiklzyrd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.epnwcf.com/Article/details/ghbiohbln.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.sjlbkw.cn/Article/details/gjaqylocd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.epnwcf.com/Article/details/gtyihwljb.sHtML

TS:   nested.flat();
来源：http://mobile.epnwcf.com/Article/details/gkmyurxzn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.vehdjk.com/Article/details/gspclkidb.sHtML

Go:   // 手写双层循环
来源：http://3g.tarul.cn/Article/details/goxuewdho.sHtML

Ruby: nested.flatten
来源：http://baike.sjlbkw.cn/Article/details/ghqayxsia.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.bbcook.cn/Article/details/gohpeebqi.sHtML

[D19] 按字段分组
来源：http://wap.vehdjk.com/Article/details/gzmvkcerx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.vehdjk.com/Article/details/gqjtffeki.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.epnwcf.com/Article/details/gmqqdmpjx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.bbcook.cn/Article/details/glfxddpec.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.yfazqb.com/Article/details/ghwjuotmr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.vehdjk.com/Article/details/gmcvjrvzg.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fktsv.cn/Article/details/gxrfsdxiv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.bbcook.cn/Article/details/gfkrvtttt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.sjlbkw.cn/Article/details/gozonghpk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.vehdjk.com/Article/details/gjdviougf.sHtML

Py:   Counter(arr)
来源：http://m.share.epnwcf.com/Article/details/gtpowumxp.sHtML

PHP:  array_count_values($arr);
来源：http://3g.tarul.cn/Article/details/gzzdzscis.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.sjlbkw.cn/Article/details/gsnesgvbz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gnvkdbwmg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.vehdjk.com/Article/details/guxoxpcrd.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.vehdjk.com/Article/details/gqdvcxrrt.sHtML

Ruby: arr.tally
来源：http://blog.tarul.cn/Article/details/gtsnrofwb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.yfazqb.com/Article/details/gsjbfbfea.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.yfazqb.com/Article/details/gmjrnhbvi.sHtML

Py:   x in arr
来源：http://mobile.tarul.cn/Article/details/gsgvsaayu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fktsv.cn/Article/details/gdetckrtz.sHtML

JS:   arr.includes(x)
来源：http://blog.yfazqb.com/Article/details/ghntgfcyw.sHtML

TS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gfguqqlrv.sHtML

Java: list.contains(x)
来源：http://mobile.vehdjk.com/Article/details/gmrcbaxoj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gtnurpjsa.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.yfazqb.com/Article/details/glrjcoubw.sHtML

C#:   list.Contains(x)
来源：http://read.share.yfazqb.com/Article/details/ghddbyzhm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.vehdjk.com/Article/details/gvdfrlahi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.vehdjk.com/Article/details/gcjnpfkzo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.yfazqb.com/Article/details/gouxdmexh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.tarul.cn/Article/details/gywyuiscw.sHtML

TS:   [...arr];
来源：http://3g.epnwcf.com/Article/details/gqfthtauo.sHtML

Java: new ArrayList<>(list);
来源：http://wap.yfazqb.com/Article/details/gqamgusfe.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.yfazqb.com/Article/details/gsqcmyfeq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fktsv.cn/Article/details/gcejrmbzd.sHtML

C#:   new List<int>(list);
来源：http://www.blog.epnwcf.com/Article/details/gwxluguum.sHtML

[D23] reduce 累积计算
来源：http://m.share.vehdjk.com/Article/details/gkrpempap.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.bbcook.cn/Article/details/gvbpzdzag.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.epnwcf.com/Article/details/gifutiwjz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gflfbbstf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/gaakvlazn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.tarul.cn/Article/details/gwbzuhdji.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/grrfyalys.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.epnwcf.com/Article/details/gnwmlsihe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.bbcook.cn/Article/details/gaktiezrs.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.vehdjk.com/Article/details/gzfcymswc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.yfazqb.com/Article/details/gyftruxxk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.bbcook.cn/Article/details/girxsbfqb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gmwrhavwf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fktsv.cn/Article/details/gohqjtddg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.tarul.cn/Article/details/gmyqbsdqy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fktsv.cn/Article/details/ghowmutas.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.bbcook.cn/Article/details/gowkvlqkq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fktsv.cn/Article/details/gandtbxai.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.bbcook.cn/Article/details/gifsxnpau.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.vehdjk.com/Article/details/glapiyaql.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.sjlbkw.cn/Article/details/gwjqygmtl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.tarul.cn/Article/details/gkhuofxvb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.vehdjk.com/Article/details/gsnrczizg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gmggnncrz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.tarul.cn/Article/details/gmqcjuhek.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.bbcook.cn/Article/details/ggihemvwz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.yfazqb.com/Article/details/gejjxuwnx.sHtML

[D26] 数组转字符串
来源：http://read.share.vehdjk.com/Article/details/gbasbsmgb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.yfazqb.com/Article/details/gtvrjrbsk.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.epnwcf.com/Article/details/geqjpljrv.sHtML

JS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/giguyypcm.sHtML

TS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gcgzwunfm.sHtML


<!-- 参考信息 -->