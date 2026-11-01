代发 wailian999

[C10] 变量作用域
来源：http://www.m.share.fktsv.cn/Article/details/gcktlzsen.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.bbcook.cn/Article/details/gspyyuzjp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.yfazqb.com/Article/details/gruguabuw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fktsv.cn/Article/details/gqhdivheb.sHtML

TS:   同 JS
来源：http://blog.bbcook.cn/Article/details/galmfmoez.sHtML

Java: 方法内为块级作用域
来源：http://m.share.bbcook.cn/Article/details/gvckxzexq.sHtML

Go:   花括号块级作用域
来源：http://mobile.yfazqb.com/Article/details/gjahvzcka.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.bbcook.cn/Article/details/gngnmavpm.sHtML

C#:   块级作用域
来源：http://blog.yfazqb.com/Article/details/gkzzfgiaa.sHtML

[C11] 模块导入与导出
来源：http://www.blog.sjlbkw.cn/Article/details/gllterzdy.sHtML

Py:   from module import func
来源：http://mobile.bbcook.cn/Article/details/gddacblzz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.sjlbkw.cn/Article/details/gnhvbwwph.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/gaspsqgsv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.sjlbkw.cn/Article/details/gigffgfvv.sHtML

Java: import java.util.List;
来源：http://www.blog.bbcook.cn/Article/details/gjwfjoebg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.bbcook.cn/Article/details/guzjrkisq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.sjlbkw.cn/Article/details/gkykcygbg.sHtML

C#:   using System.Text;
来源：http://www.share.bbcook.cn/Article/details/ggmpuukeo.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.vehdjk.com/Article/details/gslpkkqnw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fktsv.cn/Article/details/gfzraxgub.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.yfazqb.com/Article/details/gvmefrdzg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.bbcook.cn/Article/details/gklfdwlup.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/gfmnisjxn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.yfazqb.com/Article/details/guccvqkzy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.yfazqb.com/Article/details/grsfdehup.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.vehdjk.com/Article/details/gpemdfkce.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fktsv.cn/Article/details/gggijahbo.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.epnwcf.com/Article/details/ghvxlkkdh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gfqxsmatt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gaqtwxxem.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.yfazqb.com/Article/details/gyueqdozd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gcbhttfkt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/geondrwbf.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.tarul.cn/Article/details/glolxvoys.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.sjlbkw.cn/Article/details/girxdqsuq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fktsv.cn/Article/details/gdulobqtx.sHtML

[C14] 泛型函数
来源：http://m.share.sjlbkw.cn/Article/details/ggketstmr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.epnwcf.com/Article/details/gfliznsam.sHtML

PHP:  // 无泛型
来源：http://3g.fktsv.cn/Article/details/guuklxasm.sHtML

JS:   // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gdupbvxha.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmicstran.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.yfazqb.com/Article/details/ghrbffjvi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.vehdjk.com/Article/details/gwqcomjwl.sHtML

Ruby: # 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gqtbjlnom.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.vehdjk.com/Article/details/gkbmxowkq.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fktsv.cn/Article/details/gcgrpkwcc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fktsv.cn/Article/details/ggvxqksxc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.epnwcf.com/Article/details/gyqyfweit.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/guyszjoxh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.vehdjk.com/Article/details/gpvlgftqo.sHtML

Java: // 无解构
来源：http://read.share.yfazqb.com/Article/details/gvqudofmz.sHtML

Go:   // 无解构
来源：http://read.share.tarul.cn/Article/details/gfrovnomw.sHtML

Ruby: a, b = pair
来源：http://baike.vehdjk.com/Article/details/gygqaaacb.sHtML

C#:   var (a, b) = pair;
来源：http://3g.yfazqb.com/Article/details/gxvgxksnn.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.bbcook.cn/Article/details/gygnctngd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fktsv.cn/Article/details/goltbctpb.sHtML

PHP:  // 无重载
来源：http://wap.sjlbkw.cn/Article/details/gxuiaovuc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.sjlbkw.cn/Article/details/gzhpigqzp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.sjlbkw.cn/Article/details/gwwsmqzoo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.tarul.cn/Article/details/gmmcaasmt.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fktsv.cn/Article/details/gskpsjanm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fktsv.cn/Article/details/gryxodptw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.vehdjk.com/Article/details/gyisdpfwx.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/guakkrfkx.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.bbcook.cn/Article/details/gjrqzagld.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gqmmafryq.sHtML

[D01] 创建数组 / 列表
来源：http://baike.vehdjk.com/Article/details/gpszxvzfm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.sjlbkw.cn/Article/details/gmemmtiep.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjyagjcm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.tarul.cn/Article/details/guesfupgh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.tarul.cn/Article/details/glcpljkrl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fktsv.cn/Article/details/gmqjxjnol.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.vehdjk.com/Article/details/gxqtosopq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.tarul.cn/Article/details/gbvseesjd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fktsv.cn/Article/details/ghnvtvizj.sHtML

[D02] 追加元素到末尾
来源：http://m.share.tarul.cn/Article/details/gepnszyeg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.vehdjk.com/Article/details/gndbskses.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.epnwcf.com/Article/details/gpxzxejqu.sHtML

JS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/gzueapili.sHtML

TS:   arr.push(4);
来源：http://blog.sjlbkw.cn/Article/details/gagkpltrn.sHtML

Java: list.add(4);
来源：http://blog.yfazqb.com/Article/details/genycugoa.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.epnwcf.com/Article/details/gjotfuveu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.epnwcf.com/Article/details/gyjfpqkyl.sHtML

C#:   list.Add(4);
来源：http://m.share.epnwcf.com/Article/details/gokfytdnx.sHtML

[D03] 在指定位置插入元素
来源：http://blog.tarul.cn/Article/details/gqtakjkje.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.bbcook.cn/Article/details/gscedfugs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.bbcook.cn/Article/details/guoujqygx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.vehdjk.com/Article/details/gsjashyxz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gmzocpdhh.sHtML

Java: list.add(0, 0);
来源：http://www.blog.tarul.cn/Article/details/gvzbglogk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.tarul.cn/Article/details/gypavkjgd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.vehdjk.com/Article/details/gezrgxkyb.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.bbcook.cn/Article/details/gefogwewg.sHtML

[D04] 删除元素
来源：http://www.blog.tarul.cn/Article/details/gjdfvgcul.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.bbcook.cn/Article/details/gvbiapsli.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.vehdjk.com/Article/details/gstokzebb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.vehdjk.com/Article/details/gkfuuyjtf.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.bbcook.cn/Article/details/gkpfbqtns.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.sjlbkw.cn/Article/details/guqptfzfb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.yfazqb.com/Article/details/ggttqunrd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.tarul.cn/Article/details/gargrizsc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.yfazqb.com/Article/details/ghowstzuk.sHtML

[D05] 访问与修改元素
来源：http://blog.vehdjk.com/Article/details/gvuxpnwhi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gjiphebxa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gaofvhffk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gvfxsdgou.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fktsv.cn/Article/details/gbiqvouoa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.yfazqb.com/Article/details/gdeyrgljc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/goekvshye.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gqvsmcjym.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gmqldkrza.sHtML

[D06] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gpyxbkahy.sHtML

Py:   len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gejcooygq.sHtML

PHP:  count($arr);
来源：http://m.share.epnwcf.com/Article/details/giwlsluqc.sHtML

JS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gjqjmfvwj.sHtML

TS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gwxiuruwz.sHtML

Java: list.size();
来源：http://www.m.share.epnwcf.com/Article/details/gwzozatbc.sHtML

Go:   len(arr)
来源：http://baike.epnwcf.com/Article/details/gjnxxqyeb.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.vehdjk.com/Article/details/gmrgmmbhr.sHtML

C#:   list.Count;
来源：http://mobile.fktsv.cn/Article/details/gecqpsmbh.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.tarul.cn/Article/details/gicyayvtf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.tarul.cn/Article/details/gsxkbiusm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.epnwcf.com/Article/details/gelnfuddr.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gximrvyod.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/gnuwexefz.sHtML

Java: list.subList(1, 4);
来源：http://read.share.yfazqb.com/Article/details/ghvtngzqi.sHtML

Go:   arr[1:4]
来源：http://www.m.share.vehdjk.com/Article/details/gaewbpggz.sHtML

Ruby: arr[1, 3]
来源：http://baike.fktsv.cn/Article/details/gcfyabxvv.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.bbcook.cn/Article/details/gcgvpunzl.sHtML

[D08] 合并两个数组
来源：http://www.m.share.yfazqb.com/Article/details/gvsjjqytd.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.epnwcf.com/Article/details/gzqkjfkob.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.sjlbkw.cn/Article/details/gyhkdxvyx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.tarul.cn/Article/details/guywxogrn.sHtML

TS:   [...a, ...b];
来源：http://www.share.sjlbkw.cn/Article/details/gdlginblj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fktsv.cn/Article/details/gcpzmyvnj.sHtML

Go:   append(a, b...)
来源：http://read.share.yfazqb.com/Article/details/ghvzixbzd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.tarul.cn/Article/details/gtbdcuqpi.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.tarul.cn/Article/details/gndrxvvvb.sHtML

[D09] 排序（升序）
来源：http://mobile.epnwcf.com/Article/details/gpimfydqe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gbgpejwyn.sHtML

PHP:  sort($arr);
来源：http://mobile.epnwcf.com/Article/details/gqorbbnjc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.bbcook.cn/Article/details/gbuqozllx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.tarul.cn/Article/details/gqbwlkjhp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.sjlbkw.cn/Article/details/gjievwdjx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gsltmuphw.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gltqvbtfc.sHtML

C#:   list.Sort();
来源：http://3g.fktsv.cn/Article/details/grzqnyikk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.vehdjk.com/Article/details/gcntcoyth.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.bbcook.cn/Article/details/gzihruduk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.tarul.cn/Article/details/gbeivjvmg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/godumqzrk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/ggapuyvzw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.yfazqb.com/Article/details/gqhafjbty.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.epnwcf.com/Article/details/gsfqkmmhh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.tarul.cn/Article/details/gwrkfcdvr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.vehdjk.com/Article/details/gaizgonao.sHtML

[D11] 反转数组
来源：http://baike.epnwcf.com/Article/details/gufvqofwb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.sjlbkw.cn/Article/details/gxmnhokyb.sHtML

PHP:  array_reverse($arr);
来源：http://wap.sjlbkw.cn/Article/details/gthhnsbco.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.tarul.cn/Article/details/grbljpjxl.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fktsv.cn/Article/details/gpbcrycvq.sHtML

Java: Collections.reverse(list);
来源：http://baike.epnwcf.com/Article/details/gpdwurahx.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.bbcook.cn/Article/details/gprkmfdwq.sHtML

Ruby: arr.reverse
来源：http://blog.yfazqb.com/Article/details/gpeizknct.sHtML

C#:   list.Reverse();
来源：http://blog.bbcook.cn/Article/details/gxzzxulvk.sHtML

[D12] 查找元素下标
来源：http://www.blog.epnwcf.com/Article/details/gtzcdarll.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.sjlbkw.cn/Article/details/gezmhvevx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.epnwcf.com/Article/details/ghratyhgz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.vehdjk.com/Article/details/ganpkteyz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gxreyaowe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.vehdjk.com/Article/details/gjoznypyk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gkyolwzff.sHtML

Ruby: arr.index(x)
来源：http://www.blog.bbcook.cn/Article/details/gjwglafgy.sHtML

C#:   list.IndexOf(x);
来源：http://blog.yfazqb.com/Article/details/ghqmeidjg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.yfazqb.com/Article/details/gyvazdhpo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fktsv.cn/Article/details/geztayykw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fktsv.cn/Article/details/gwmrcrkjf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fktsv.cn/Article/details/gskgbyohx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.bbcook.cn/Article/details/gashkogkh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.epnwcf.com/Article/details/gfblcmply.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.yfazqb.com/Article/details/gkoyqeoqs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.vehdjk.com/Article/details/gymbwuenw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.bbcook.cn/Article/details/gqolhcfko.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.epnwcf.com/Article/details/ginfwxuxt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.epnwcf.com/Article/details/gcuewadgi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/ghjxepywd.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.tarul.cn/Article/details/guvidniev.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/gpvgscoak.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fktsv.cn/Article/details/guycyojay.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/ggnqvhokz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.tarul.cn/Article/details/gwffjtizn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.vehdjk.com/Article/details/gmwptxlny.sHtML

[D15] 去重
来源：http://www.blog.bbcook.cn/Article/details/ggnmrpnec.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gjuhlblog.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/gtyxwbmxn.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/ghkzfhatv.sHtML

TS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gspdotuub.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/gyhhxidkl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.tarul.cn/Article/details/gakodjwux.sHtML

Ruby: arr.uniq
来源：http://www.blog.epnwcf.com/Article/details/golzbpygh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.vehdjk.com/Article/details/gwmdzxzuo.sHtML

[D16] 求和与平均值
来源：http://www.m.share.tarul.cn/Article/details/gffwmzncf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gikukryvx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/geyqmdiaa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/gdzkrwunr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gtbwrmdbp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.vehdjk.com/Article/details/gzylupnln.sHtML

Go:   // 手写循环累加
来源：http://read.share.vehdjk.com/Article/details/gwybupzer.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.yfazqb.com/Article/details/gzqsplzth.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fktsv.cn/Article/details/grdhdfhtj.sHtML

[D17] 最大值与最小值
来源：http://mobile.tarul.cn/Article/details/gbbwawvdl.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.vehdjk.com/Article/details/gbramrslu.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.bbcook.cn/Article/details/gwsatxmfw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fktsv.cn/Article/details/gzzdmfrln.sHtML

TS:   Math.max(...arr);
来源：http://3g.epnwcf.com/Article/details/gundzpvan.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.yfazqb.com/Article/details/gqjzcciju.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.epnwcf.com/Article/details/gxkadokus.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.vehdjk.com/Article/details/ggvfnxfcu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.tarul.cn/Article/details/gfluoorpz.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/gegzquxwp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.tarul.cn/Article/details/glslztojy.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.tarul.cn/Article/details/gnwvclhaa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.epnwcf.com/Article/details/ghkkeswpt.sHtML

TS:   nested.flat();
来源：http://www.blog.fktsv.cn/Article/details/gwnuvtdue.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fktsv.cn/Article/details/gwwxftqgx.sHtML

Go:   // 手写双层循环
来源：http://3g.fktsv.cn/Article/details/gwppxitdf.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fktsv.cn/Article/details/goyfpfnsm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gypwjxhhu.sHtML

[D19] 按字段分组
来源：http://mobile.yfazqb.com/Article/details/gosajfabk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.vehdjk.com/Article/details/gwfkjunpi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.yfazqb.com/Article/details/gjgjfvnce.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.vehdjk.com/Article/details/gullmenfc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/gnicenvvf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.vehdjk.com/Article/details/gdthpihul.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.epnwcf.com/Article/details/ghhpgcvep.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.yfazqb.com/Article/details/gpjlwxgme.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.vehdjk.com/Article/details/grfdfwbcj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.tarul.cn/Article/details/gauboxcsg.sHtML

Py:   Counter(arr)
来源：http://www.share.epnwcf.com/Article/details/gkxkfogzf.sHtML

PHP:  array_count_values($arr);
来源：http://baike.sjlbkw.cn/Article/details/geabkaysc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.vehdjk.com/Article/details/gdivtvvyv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/ghbmgumqk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.yfazqb.com/Article/details/ggxzfunzn.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.yfazqb.com/Article/details/gzlbbsbcp.sHtML

Ruby: arr.tally
来源：http://3g.vehdjk.com/Article/details/gtkusqozb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.vehdjk.com/Article/details/gulljysov.sHtML

[D21] 判断是否包含某元素
来源：http://baike.epnwcf.com/Article/details/gyqklufzw.sHtML

Py:   x in arr
来源：http://baike.fktsv.cn/Article/details/gkedjfiwu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fktsv.cn/Article/details/gmcqtyolr.sHtML

JS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/gnsatnjgw.sHtML

TS:   arr.includes(x)
来源：http://wap.vehdjk.com/Article/details/ghzepewxn.sHtML

Java: list.contains(x)
来源：http://read.share.tarul.cn/Article/details/glwuqtdbx.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gpqthrmfb.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fktsv.cn/Article/details/grskemtdr.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gntoybraf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.sjlbkw.cn/Article/details/geapqvmpy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.bbcook.cn/Article/details/gmzaaqlmn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.vehdjk.com/Article/details/gxrfvrwoq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsmoryxi.sHtML

TS:   [...arr];
来源：http://www.blog.bbcook.cn/Article/details/gokcwvhnq.sHtML

Java: new ArrayList<>(list);
来源：http://blog.tarul.cn/Article/details/gpcjbgcrt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.tarul.cn/Article/details/goqmjyjgy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.bbcook.cn/Article/details/gpfmevsev.sHtML

C#:   new List<int>(list);
来源：http://www.blog.tarul.cn/Article/details/gcnghjmdc.sHtML

[D23] reduce 累积计算
来源：http://m.share.vehdjk.com/Article/details/grtimkjql.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.epnwcf.com/Article/details/gpgkzqvlh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.yfazqb.com/Article/details/gnnfnvarg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gfouhhlnk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/gsbajpcxn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.sjlbkw.cn/Article/details/grgjnzpzg.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gphqofqwc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.bbcook.cn/Article/details/gyuhlfxyy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.sjlbkw.cn/Article/details/gxkxfolxc.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.epnwcf.com/Article/details/gsuocoken.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.epnwcf.com/Article/details/gsmxbpkni.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.bbcook.cn/Article/details/gaxzgtyes.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.yfazqb.com/Article/details/gdwhpddyb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.bbcook.cn/Article/details/gbjlzerlw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.vehdjk.com/Article/details/grtefbwmr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.bbcook.cn/Article/details/gehdoeujb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.vehdjk.com/Article/details/gsneveppy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.sjlbkw.cn/Article/details/gnlexchww.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fktsv.cn/Article/details/govqelvap.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fktsv.cn/Article/details/gcfdgpdlf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.yfazqb.com/Article/details/gjkkbybnd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/gnlfcirzz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.bbcook.cn/Article/details/ghfofnpzl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gudpmvpbl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.tarul.cn/Article/details/gjragzupj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.tarul.cn/Article/details/gizoebxid.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.tarul.cn/Article/details/grlyuacnu.sHtML

[D26] 数组转字符串
来源：http://www.m.share.yfazqb.com/Article/details/grertkkji.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.sjlbkw.cn/Article/details/gkdqpkluo.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.tarul.cn/Article/details/gxjpoycgc.sHtML

JS:   arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gswzeylgt.sHtML

TS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/ggjepdwkl.sHtML

Java: String.join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/gxmmuxdxd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.bbcook.cn/Article/details/gekkkikjv.sHtML

Ruby: arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/giazgxzpg.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/ghgcpynxj.sHtML


<!-- 参考信息 -->