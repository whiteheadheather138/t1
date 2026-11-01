代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.epnwcf.com/Article/details/gvczgyazy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.tarul.cn/Article/details/gcwlvkozs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/gftlxajsz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.epnwcf.com/Article/details/gwjbxumyh.sHtML

[C10] 变量作用域
来源：http://www.share.vehdjk.com/Article/details/ggqbczica.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.sjlbkw.cn/Article/details/gtvcbjpqo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.epnwcf.com/Article/details/ghwbojocp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.epnwcf.com/Article/details/gjxoohebi.sHtML

TS:   同 JS
来源：http://www.share.bbcook.cn/Article/details/govdohyhs.sHtML

Java: 方法内为块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gbbbakvbl.sHtML

Go:   花括号块级作用域
来源：http://read.share.bbcook.cn/Article/details/gcsjmniep.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.epnwcf.com/Article/details/gentexniy.sHtML

C#:   块级作用域
来源：http://mobile.yfazqb.com/Article/details/gxdxyteqx.sHtML

[C11] 模块导入与导出
来源：http://m.share.tarul.cn/Article/details/gffseqoev.sHtML

Py:   from module import func
来源：http://3g.yfazqb.com/Article/details/gvzuxtwxm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fktsv.cn/Article/details/gaerwmkgi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fktsv.cn/Article/details/gofkrattj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.sjlbkw.cn/Article/details/ganydjxes.sHtML

Java: import java.util.List;
来源：http://mobile.sjlbkw.cn/Article/details/glmaqxfwz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.sjlbkw.cn/Article/details/gapdsnakq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.sjlbkw.cn/Article/details/grdlykvwb.sHtML

C#:   using System.Text;
来源：http://www.share.sjlbkw.cn/Article/details/gwkvcyufr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.vehdjk.com/Article/details/gyysyfxwj.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.sjlbkw.cn/Article/details/gjclggovg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.bbcook.cn/Article/details/gelpmrkpg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.epnwcf.com/Article/details/grfbnjzxb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.epnwcf.com/Article/details/guxiiwrkc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.vehdjk.com/Article/details/gwqzxngpo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.tarul.cn/Article/details/gzirbdrzo.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.vehdjk.com/Article/details/gazrwoizx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.tarul.cn/Article/details/gnfhjhftt.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.tarul.cn/Article/details/gssolfxup.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.vehdjk.com/Article/details/gjieyzeob.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gwohndmpj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.vehdjk.com/Article/details/gtdhsjxip.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gqozkxmfn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gueeyzvfe.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.sjlbkw.cn/Article/details/giddqifmp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.epnwcf.com/Article/details/ghtunxgmr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.tarul.cn/Article/details/gucitxweo.sHtML

[C14] 泛型函数
来源：http://baike.vehdjk.com/Article/details/gmawlioxu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.yfazqb.com/Article/details/gvtcryttc.sHtML

PHP:  // 无泛型
来源：http://m.share.bbcook.cn/Article/details/glaomdnwc.sHtML

JS:   // 无泛型
来源：http://wap.vehdjk.com/Article/details/gfonulajm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fktsv.cn/Article/details/gyyhbpjqd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fktsv.cn/Article/details/girsxcyat.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fktsv.cn/Article/details/gqfxbqacm.sHtML

Ruby: # 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gxqgfbaay.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.bbcook.cn/Article/details/gtvwbfroq.sHtML

[C15] 解构 / 展开参数
来源：http://3g.bbcook.cn/Article/details/gawyrhmsc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fktsv.cn/Article/details/gquwlfckn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.yfazqb.com/Article/details/gxouxywvg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/gjhwozrcj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fktsv.cn/Article/details/ghjghoydh.sHtML

Java: // 无解构
来源：http://read.share.epnwcf.com/Article/details/gacucjfiy.sHtML

Go:   // 无解构
来源：http://m.share.fktsv.cn/Article/details/gzefgeddw.sHtML

Ruby: a, b = pair
来源：http://blog.vehdjk.com/Article/details/gmxqqovnd.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.yfazqb.com/Article/details/gcdezqhkb.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.tarul.cn/Article/details/gkvegsmmj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsnuzmdj.sHtML

PHP:  // 无重载
来源：http://3g.bbcook.cn/Article/details/ghcetysfr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fktsv.cn/Article/details/gvegckxkv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.epnwcf.com/Article/details/ggkirtxrd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.bbcook.cn/Article/details/gypybjzbc.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fktsv.cn/Article/details/gzxzxjdgz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.epnwcf.com/Article/details/gyvphlgyq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.bbcook.cn/Article/details/grzisqsfo.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gophmlxir.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.vehdjk.com/Article/details/gsqzurdda.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gavwvkzwn.sHtML

[D01] 创建数组 / 列表
来源：http://wap.vehdjk.com/Article/details/gztewwxvs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.tarul.cn/Article/details/gtxosfyxf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.bbcook.cn/Article/details/gwjtferrm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.yfazqb.com/Article/details/gwtghvltm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fktsv.cn/Article/details/gxktyuzvg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.sjlbkw.cn/Article/details/gqdiucsad.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.yfazqb.com/Article/details/gxlaosfcg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.tarul.cn/Article/details/gaiqdxakn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.tarul.cn/Article/details/grmmowhci.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fktsv.cn/Article/details/gujiqacrm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/gdgbibtcm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.yfazqb.com/Article/details/gauhdyubj.sHtML

JS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/gdywyzdrb.sHtML

TS:   arr.push(4);
来源：http://www.share.sjlbkw.cn/Article/details/goinixvgu.sHtML

Java: list.add(4);
来源：http://m.share.fktsv.cn/Article/details/gjtgnuwqc.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.sjlbkw.cn/Article/details/gytgiieow.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.bbcook.cn/Article/details/gysyrmtnn.sHtML

C#:   list.Add(4);
来源：http://mobile.fktsv.cn/Article/details/gseujvbtj.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fktsv.cn/Article/details/gnpnpvbpf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.epnwcf.com/Article/details/gymxcosgq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.epnwcf.com/Article/details/guumlihss.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.vehdjk.com/Article/details/gulyivzaw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.tarul.cn/Article/details/gjjsmpaet.sHtML

Java: list.add(0, 0);
来源：http://www.blog.epnwcf.com/Article/details/gqozceigz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.bbcook.cn/Article/details/goandwjlm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.tarul.cn/Article/details/gzzoxnnnc.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.vehdjk.com/Article/details/goeepexle.sHtML

[D04] 删除元素
来源：http://3g.sjlbkw.cn/Article/details/gqretkmyv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.epnwcf.com/Article/details/gmyxtjilg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.sjlbkw.cn/Article/details/gselujusw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.vehdjk.com/Article/details/gkgfgtdrq.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.bbcook.cn/Article/details/gtzxziqih.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.epnwcf.com/Article/details/gfrebelsq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.bbcook.cn/Article/details/gkmhnvfdb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fktsv.cn/Article/details/gbzadngyc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.tarul.cn/Article/details/gnxzyvahq.sHtML

[D05] 访问与修改元素
来源：http://www.blog.sjlbkw.cn/Article/details/gusttcnea.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/gfxlatkal.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gfhhoqrxd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gsrgonefc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.bbcook.cn/Article/details/gcjcoewyw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.bbcook.cn/Article/details/gfxitvsiu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gbzejxcrc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gvuugixnb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gtjdzbmvz.sHtML

[D06] 数组长度
来源：http://baike.yfazqb.com/Article/details/grdsqxthr.sHtML

Py:   len(arr)
来源：http://baike.tarul.cn/Article/details/gnnschcsm.sHtML

PHP:  count($arr);
来源：http://m.share.vehdjk.com/Article/details/gnituuwkw.sHtML

JS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gnvyoyoxo.sHtML

TS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/gfcdkkead.sHtML

Java: list.size();
来源：http://baike.tarul.cn/Article/details/gshmepvcq.sHtML

Go:   len(arr)
来源：http://baike.yfazqb.com/Article/details/gdhmtcshb.sHtML

Ruby: arr.length; arr.size
来源：http://baike.sjlbkw.cn/Article/details/gwohvcgyb.sHtML

C#:   list.Count;
来源：http://read.share.vehdjk.com/Article/details/gqgcwwhgx.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.epnwcf.com/Article/details/gzlrrprwv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fktsv.cn/Article/details/gjxtwplsb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.vehdjk.com/Article/details/gfqmnipoz.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/ggzegphmt.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/grxvreogm.sHtML

Java: list.subList(1, 4);
来源：http://www.share.epnwcf.com/Article/details/goleaeytv.sHtML

Go:   arr[1:4]
来源：http://wap.bbcook.cn/Article/details/ghzhsqbpw.sHtML

Ruby: arr[1, 3]
来源：http://wap.epnwcf.com/Article/details/gbhstihfh.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.sjlbkw.cn/Article/details/gimaxjsqn.sHtML

[D08] 合并两个数组
来源：http://read.share.yfazqb.com/Article/details/gnodphbvb.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.vehdjk.com/Article/details/gjqqoftuk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.epnwcf.com/Article/details/gpxugxkzo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.bbcook.cn/Article/details/gvflzoebo.sHtML

TS:   [...a, ...b];
来源：http://baike.bbcook.cn/Article/details/ghdkcuejs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fktsv.cn/Article/details/gofilhauj.sHtML

Go:   append(a, b...)
来源：http://mobile.vehdjk.com/Article/details/getzlqioq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fktsv.cn/Article/details/gcpsydhut.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.tarul.cn/Article/details/gnqucdhnw.sHtML

[D09] 排序（升序）
来源：http://mobile.sjlbkw.cn/Article/details/gmfbclkmy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gzxmbwnkr.sHtML

PHP:  sort($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gyeuwsayx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.tarul.cn/Article/details/gyonebyqb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.vehdjk.com/Article/details/gphwcxpac.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.vehdjk.com/Article/details/gpgebiamf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gegnlvukv.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/gzunajwsf.sHtML

C#:   list.Sort();
来源：http://www.share.sjlbkw.cn/Article/details/gigmwixiz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fktsv.cn/Article/details/gfeggfbvv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fktsv.cn/Article/details/gyefxpcka.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fktsv.cn/Article/details/gnktqnmla.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.sjlbkw.cn/Article/details/gtwlrgpvj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fktsv.cn/Article/details/glmmkwmsd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.tarul.cn/Article/details/gygriondo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.sjlbkw.cn/Article/details/gndyywlbd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.sjlbkw.cn/Article/details/gjxnmnxoq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.epnwcf.com/Article/details/ggxzboqfn.sHtML

[D11] 反转数组
来源：http://3g.epnwcf.com/Article/details/gkchtegyx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.yfazqb.com/Article/details/gzylkaxhl.sHtML

PHP:  array_reverse($arr);
来源：http://blog.tarul.cn/Article/details/gdaabobgp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fktsv.cn/Article/details/grxykdazx.sHtML

TS:   [...arr].reverse();
来源：http://wap.sjlbkw.cn/Article/details/gmltlwcih.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.epnwcf.com/Article/details/gzmhnqhva.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gibbkpsqz.sHtML

Ruby: arr.reverse
来源：http://read.share.fktsv.cn/Article/details/gtbbrprpn.sHtML

C#:   list.Reverse();
来源：http://m.share.epnwcf.com/Article/details/gockrchod.sHtML

[D12] 查找元素下标
来源：http://baike.yfazqb.com/Article/details/gnerymaeq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gbcubfrnh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.tarul.cn/Article/details/gyvuhgfca.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gqsbbswfm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gelphyxgu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.bbcook.cn/Article/details/gbxaicwgg.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.tarul.cn/Article/details/ggyfmijqu.sHtML

Ruby: arr.index(x)
来源：http://www.share.sjlbkw.cn/Article/details/gwtsqzibo.sHtML

C#:   list.IndexOf(x);
来源：http://3g.tarul.cn/Article/details/gonmsvvsw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.vehdjk.com/Article/details/ggosqizus.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.vehdjk.com/Article/details/guoydhvqn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.sjlbkw.cn/Article/details/gdthgyrsm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/gyjehnflu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.tarul.cn/Article/details/gnfmdwpzo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.yfazqb.com/Article/details/guhpfxhde.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fktsv.cn/Article/details/gziupsklr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.vehdjk.com/Article/details/ggiyaqcbk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fktsv.cn/Article/details/gfplkwsqm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.epnwcf.com/Article/details/gthkrjklb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.epnwcf.com/Article/details/ghfnjvkdj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.bbcook.cn/Article/details/gbtolmrlf.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/goeyuuaay.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gewgfmabg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.vehdjk.com/Article/details/gmkxhxqow.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/ghbzxmnqf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.tarul.cn/Article/details/gptvmrqmm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.tarul.cn/Article/details/gkkzsxsdx.sHtML

[D15] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/glvuwaetw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gfaqyctyj.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fktsv.cn/Article/details/gmnveizor.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gckgjkokh.sHtML

TS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gsxoilbbq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fktsv.cn/Article/details/gkrvdijuj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.tarul.cn/Article/details/glhficpyr.sHtML

Ruby: arr.uniq
来源：http://wap.bbcook.cn/Article/details/guiysxzlo.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.epnwcf.com/Article/details/gnuqzdfiy.sHtML

[D16] 求和与平均值
来源：http://3g.yfazqb.com/Article/details/gboiincjy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.yfazqb.com/Article/details/glijazmwx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.vehdjk.com/Article/details/glmrfgssn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/gbxqreqlu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.epnwcf.com/Article/details/gwhgudczq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.sjlbkw.cn/Article/details/gqyaithpz.sHtML

Go:   // 手写循环累加
来源：http://www.share.bbcook.cn/Article/details/gcyrvbjcm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fktsv.cn/Article/details/gcwfrvzwi.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.bbcook.cn/Article/details/geqyxdqml.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.epnwcf.com/Article/details/gavjuzcqq.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.vehdjk.com/Article/details/gfqrcedns.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.yfazqb.com/Article/details/grmqghytq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fktsv.cn/Article/details/ganffzwvf.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/gdrzegsdd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.sjlbkw.cn/Article/details/gqmellvjb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/grhzjsizp.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fktsv.cn/Article/details/gdptugznk.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fktsv.cn/Article/details/glniywoup.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/gxtlsolgg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.yfazqb.com/Article/details/gkerkzpuh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.epnwcf.com/Article/details/gadsqlkeb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.tarul.cn/Article/details/gshtineka.sHtML

TS:   nested.flat();
来源：http://www.m.share.tarul.cn/Article/details/gtiegtory.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fktsv.cn/Article/details/gqbuukyyo.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fktsv.cn/Article/details/gxzufyqik.sHtML

Ruby: nested.flatten
来源：http://www.share.sjlbkw.cn/Article/details/gmoahzloq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.epnwcf.com/Article/details/gqjaeivjv.sHtML

[D19] 按字段分组
来源：http://www.blog.fktsv.cn/Article/details/gihpayuqw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.epnwcf.com/Article/details/gplgvcvwn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.epnwcf.com/Article/details/gpfpnmuef.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.sjlbkw.cn/Article/details/gmlumbtil.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.tarul.cn/Article/details/ggmilpiwt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.tarul.cn/Article/details/gygjbcpkv.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.vehdjk.com/Article/details/gaozlrfci.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.vehdjk.com/Article/details/gzqxgpake.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.epnwcf.com/Article/details/gjefhlwar.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.epnwcf.com/Article/details/gitomcafx.sHtML

Py:   Counter(arr)
来源：http://mobile.fktsv.cn/Article/details/gyupznlmn.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.vehdjk.com/Article/details/gusknfvhi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/gdeihyqpz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.yfazqb.com/Article/details/gixfuzbyr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fktsv.cn/Article/details/gocljtwez.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.bbcook.cn/Article/details/gnztlvmfu.sHtML

Ruby: arr.tally
来源：http://www.m.share.vehdjk.com/Article/details/guqbruofp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.bbcook.cn/Article/details/gegvqctlw.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.bbcook.cn/Article/details/gohkuaigq.sHtML

Py:   x in arr
来源：http://wap.bbcook.cn/Article/details/gppeguvpd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.vehdjk.com/Article/details/gfmjtkttw.sHtML

JS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/gziiupiuy.sHtML

TS:   arr.includes(x)
来源：http://mobile.epnwcf.com/Article/details/gworjiltz.sHtML

Java: list.contains(x)
来源：http://baike.fktsv.cn/Article/details/gthcfhfvo.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gfwwuewyc.sHtML

Ruby: arr.include?(x)
来源：http://m.share.yfazqb.com/Article/details/ghniuztdu.sHtML

C#:   list.Contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gmcqvkruf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.epnwcf.com/Article/details/gzsiswcih.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfybzbox.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.tarul.cn/Article/details/ghmerymvi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.yfazqb.com/Article/details/geqittfnx.sHtML

TS:   [...arr];
来源：http://www.m.share.epnwcf.com/Article/details/gqzmyehru.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/gllvepsff.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.yfazqb.com/Article/details/gfefhjasj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.yfazqb.com/Article/details/gpwpnqdvf.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gzmydvcgb.sHtML

[D23] reduce 累积计算
来源：http://blog.vehdjk.com/Article/details/gtypdjfxg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fktsv.cn/Article/details/gkkfotwip.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.tarul.cn/Article/details/gdbyszupb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.bbcook.cn/Article/details/gvghdunah.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gtrwgwsnr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.bbcook.cn/Article/details/gnllubhli.sHtML

Go:   // 手写循环
来源：http://m.share.yfazqb.com/Article/details/gdbkjmyjv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fktsv.cn/Article/details/gsnyclfei.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.vehdjk.com/Article/details/guhxxpyzj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gaexjldke.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gleilgnoc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.epnwcf.com/Article/details/gekivltyr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.tarul.cn/Article/details/gujfwbrmq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/garexsmgd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fktsv.cn/Article/details/gmlajsqtn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.sjlbkw.cn/Article/details/gxegqhvci.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.yfazqb.com/Article/details/gudtywgtm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.sjlbkw.cn/Article/details/guxzetaew.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fktsv.cn/Article/details/gkinaafet.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.vehdjk.com/Article/details/gllhzfbav.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.yfazqb.com/Article/details/grrvjbcvu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.tarul.cn/Article/details/gfaushmlq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.tarul.cn/Article/details/gmpatcrvd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.bbcook.cn/Article/details/gxquudwag.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.yfazqb.com/Article/details/glouuifph.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.vehdjk.com/Article/details/gzvsdphdj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fktsv.cn/Article/details/gfuapwimk.sHtML

[D26] 数组转字符串
来源：http://www.share.fktsv.cn/Article/details/gufpuyzou.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.yfazqb.com/Article/details/gcywncesz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gtvfqsown.sHtML

JS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gnjkvkwhn.sHtML

TS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gsnephybp.sHtML


<!-- 参考信息 -->