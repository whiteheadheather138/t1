代发 wailian999

C#:   块级作用域
来源：http://read.share.fktsv.cn/Article/details/gevbzcyzd.sHtML

[C11] 模块导入与导出
来源：http://baike.vehdjk.com/Article/details/gqonoxcop.sHtML

Py:   from module import func
来源：http://m.share.bbcook.cn/Article/details/gqpfixqmy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.bbcook.cn/Article/details/gyzvdhozb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.tarul.cn/Article/details/gyybvgfjx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.yfazqb.com/Article/details/gbetumnpt.sHtML

Java: import java.util.List;
来源：http://3g.sjlbkw.cn/Article/details/gibjzmkrv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.bbcook.cn/Article/details/gotaggzda.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.vehdjk.com/Article/details/gnkmilcns.sHtML

C#:   using System.Text;
来源：http://wap.yfazqb.com/Article/details/gcmnhbbzn.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.bbcook.cn/Article/details/gjsuvprrr.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.yfazqb.com/Article/details/grkthxqek.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.epnwcf.com/Article/details/gpzpenwpn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.vehdjk.com/Article/details/gflhdtrch.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gdahabqvd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.bbcook.cn/Article/details/gfigclhwi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fktsv.cn/Article/details/ggxnonzlh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.bbcook.cn/Article/details/gwvxbktay.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.bbcook.cn/Article/details/gksjyctjd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.bbcook.cn/Article/details/gpuagktvv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.vehdjk.com/Article/details/gtulumakv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gccyolkmh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.yfazqb.com/Article/details/gkjciancc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gjgsgungr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gyayoqtmq.sHtML

Go:   func add(a, b int) int
来源：http://m.share.vehdjk.com/Article/details/gllsrlffg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fktsv.cn/Article/details/gnhdzythc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.bbcook.cn/Article/details/gwbjwklpj.sHtML

[C14] 泛型函数
来源：http://read.share.fktsv.cn/Article/details/gdtrfxysb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.yfazqb.com/Article/details/grfbingps.sHtML

PHP:  // 无泛型
来源：http://wap.bbcook.cn/Article/details/getvoxifq.sHtML

JS:   // 无泛型
来源：http://baike.yfazqb.com/Article/details/gnuytmtqe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fktsv.cn/Article/details/gkgwwvbgq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fktsv.cn/Article/details/ggdemmcnp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.sjlbkw.cn/Article/details/gwedjzwqb.sHtML

Ruby: # 无泛型
来源：http://read.share.epnwcf.com/Article/details/giyirahre.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.epnwcf.com/Article/details/gwaonzdgs.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.vehdjk.com/Article/details/grbfusyzg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fktsv.cn/Article/details/gndgkizzs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.sjlbkw.cn/Article/details/gmzgigrpc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/gmvchmquh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.vehdjk.com/Article/details/geaauwmbj.sHtML

Java: // 无解构
来源：http://www.share.tarul.cn/Article/details/gyxmfhoio.sHtML

Go:   // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gpaxfyfla.sHtML

Ruby: a, b = pair
来源：http://3g.yfazqb.com/Article/details/ghbmzxhos.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.tarul.cn/Article/details/gpsrdvjdp.sHtML

[C16] 函数 / 方法重载
来源：http://blog.tarul.cn/Article/details/gdvffkado.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.tarul.cn/Article/details/gxrikojby.sHtML

PHP:  // 无重载
来源：http://3g.tarul.cn/Article/details/gmtfzxzyr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fktsv.cn/Article/details/ghlcbpkxg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.epnwcf.com/Article/details/gbanhuhcz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.vehdjk.com/Article/details/gudssrryk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.tarul.cn/Article/details/gqjtvgjfk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.tarul.cn/Article/details/gwuomrkev.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.bbcook.cn/Article/details/gmyluxndy.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gegcuaymz.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.bbcook.cn/Article/details/gkrswinpf.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gulhidkwb.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fktsv.cn/Article/details/gagaipumo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.vehdjk.com/Article/details/ggxsjrucg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.vehdjk.com/Article/details/ghhpikxuc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.sjlbkw.cn/Article/details/gzswuypqf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.tarul.cn/Article/details/gmhjycmmn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.epnwcf.com/Article/details/gxpjasruj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.epnwcf.com/Article/details/gdvpfjihr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.vehdjk.com/Article/details/gokpnzwcz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.tarul.cn/Article/details/gezbzygsh.sHtML

[D02] 追加元素到末尾
来源：http://mobile.sjlbkw.cn/Article/details/gxaioyugz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.epnwcf.com/Article/details/gbbuttpdr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.bbcook.cn/Article/details/gyxmyouwe.sHtML

JS:   arr.push(4);
来源：http://read.share.bbcook.cn/Article/details/gciafnxrn.sHtML

TS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/gvxgegihr.sHtML

Java: list.add(4);
来源：http://mobile.epnwcf.com/Article/details/gazhijjlc.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.vehdjk.com/Article/details/ghgpqglcv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.bbcook.cn/Article/details/guuhlvvdo.sHtML

C#:   list.Add(4);
来源：http://www.m.share.epnwcf.com/Article/details/glptybldv.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.sjlbkw.cn/Article/details/gfspjgzid.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.vehdjk.com/Article/details/guwevftpx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.bbcook.cn/Article/details/gaasqynah.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.epnwcf.com/Article/details/gwlnytyth.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.vehdjk.com/Article/details/gopdjtlxv.sHtML

Java: list.add(0, 0);
来源：http://m.share.fktsv.cn/Article/details/gctrbwjgm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.epnwcf.com/Article/details/gbbsbedkl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fktsv.cn/Article/details/gervggylh.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/ghoxtxgci.sHtML

[D04] 删除元素
来源：http://www.m.share.tarul.cn/Article/details/gemeljhgp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.tarul.cn/Article/details/ghyhppiyp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.epnwcf.com/Article/details/gdjuzwtuh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fktsv.cn/Article/details/gzopnojaj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.epnwcf.com/Article/details/gycefzcja.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.yfazqb.com/Article/details/gyunaxqzo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.yfazqb.com/Article/details/ghsfovzrz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.bbcook.cn/Article/details/gyyukhvtg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.epnwcf.com/Article/details/gcdytlitd.sHtML

[D05] 访问与修改元素
来源：http://3g.yfazqb.com/Article/details/gmwsybqsk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gttmkhgtx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gvjkekfzs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/goqjjmeps.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.epnwcf.com/Article/details/ghbbpjijm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.epnwcf.com/Article/details/gemfjqwhy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gfhgxdlyp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/glbmkkemg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gzwomkuvl.sHtML

[D06] 数组长度
来源：http://www.blog.tarul.cn/Article/details/guhoiszlm.sHtML

Py:   len(arr)
来源：http://3g.fktsv.cn/Article/details/gkchbssrp.sHtML

PHP:  count($arr);
来源：http://mobile.yfazqb.com/Article/details/gfpkvwmoi.sHtML

JS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gmzejjjhj.sHtML

TS:   arr.length
来源：http://3g.epnwcf.com/Article/details/gsunklovs.sHtML

Java: list.size();
来源：http://www.share.fktsv.cn/Article/details/gahskfnmc.sHtML

Go:   len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gczncxhbi.sHtML

Ruby: arr.length; arr.size
来源：http://baike.bbcook.cn/Article/details/gcbngesuk.sHtML

C#:   list.Count;
来源：http://www.share.fktsv.cn/Article/details/gsqhnhsns.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.yfazqb.com/Article/details/gczyjkjnr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvyvnhlh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fktsv.cn/Article/details/ghmxfyaph.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gphwmozwg.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gzjgdwyrv.sHtML

Java: list.subList(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gnwyhjjul.sHtML

Go:   arr[1:4]
来源：http://www.blog.tarul.cn/Article/details/gfkkurcjq.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.bbcook.cn/Article/details/gkeaxrbwt.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.tarul.cn/Article/details/ggaffsfkg.sHtML

[D08] 合并两个数组
来源：http://m.share.vehdjk.com/Article/details/gtrfjzufz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.vehdjk.com/Article/details/gderyehis.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.yfazqb.com/Article/details/gljqnaelw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.epnwcf.com/Article/details/gmppdiqha.sHtML

TS:   [...a, ...b];
来源：http://baike.fktsv.cn/Article/details/gazpitkln.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.tarul.cn/Article/details/gzjizwdul.sHtML

Go:   append(a, b...)
来源：http://wap.fktsv.cn/Article/details/gmzmgnuqv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.tarul.cn/Article/details/gcfhtyyty.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/glzszetyd.sHtML

[D09] 排序（升序）
来源：http://baike.fktsv.cn/Article/details/gjjbufwud.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.vehdjk.com/Article/details/gmakfitpx.sHtML

PHP:  sort($arr);
来源：http://blog.fktsv.cn/Article/details/giqgzgili.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.yfazqb.com/Article/details/gfygulayq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.epnwcf.com/Article/details/gwhyntvip.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.yfazqb.com/Article/details/gkpbmbicp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.bbcook.cn/Article/details/gjqxdnrku.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/gydkzoqrp.sHtML

C#:   list.Sort();
来源：http://www.share.vehdjk.com/Article/details/gqfcpbkkt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.yfazqb.com/Article/details/gztyycclb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.sjlbkw.cn/Article/details/gkpyyoihr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gbjbmvsxn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/goingujba.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gbgbquvtv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.yfazqb.com/Article/details/gcxapfxfa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.yfazqb.com/Article/details/gvzfxdrph.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.tarul.cn/Article/details/gmfuncuft.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.bbcook.cn/Article/details/gfqygxnfg.sHtML

[D11] 反转数组
来源：http://read.share.epnwcf.com/Article/details/guljwdbcr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.tarul.cn/Article/details/gklxagtle.sHtML

PHP:  array_reverse($arr);
来源：http://blog.vehdjk.com/Article/details/gigmiakym.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.sjlbkw.cn/Article/details/gzrbatpvi.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.vehdjk.com/Article/details/gfqwswfgb.sHtML

Java: Collections.reverse(list);
来源：http://read.share.yfazqb.com/Article/details/grynlwyfy.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.epnwcf.com/Article/details/gebcbblyz.sHtML

Ruby: arr.reverse
来源：http://blog.epnwcf.com/Article/details/gmzglyxvf.sHtML

C#:   list.Reverse();
来源：http://m.share.fktsv.cn/Article/details/gjbqkkuxg.sHtML

[D12] 查找元素下标
来源：http://3g.tarul.cn/Article/details/gjppjkmwu.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fktsv.cn/Article/details/glhzxgaat.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.tarul.cn/Article/details/gahqqpony.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.tarul.cn/Article/details/gfznlqkmi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/ggcppyrnk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.epnwcf.com/Article/details/ghnibxoin.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fktsv.cn/Article/details/gnabnrleo.sHtML

Ruby: arr.index(x)
来源：http://mobile.yfazqb.com/Article/details/glmxbidfc.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.sjlbkw.cn/Article/details/ghzjfvash.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.bbcook.cn/Article/details/geycmhped.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.yfazqb.com/Article/details/gbegmnxqt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.epnwcf.com/Article/details/geacmftjd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gppffkooc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gcuidqmmo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.vehdjk.com/Article/details/gtviodgwv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.vehdjk.com/Article/details/gqzugwkfv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.sjlbkw.cn/Article/details/gpxuejwrt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.epnwcf.com/Article/details/gzyolrzoh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.sjlbkw.cn/Article/details/ghqjcphmx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fktsv.cn/Article/details/gylegtfwb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.tarul.cn/Article/details/gqillyiji.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjbaarmv.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.vehdjk.com/Article/details/gswfpgvfs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gggwqrnnz.sHtML

Go:   // 手写循环
来源：http://3g.sjlbkw.cn/Article/details/gyieverwf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.bbcook.cn/Article/details/gaeemxzdr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.vehdjk.com/Article/details/gvhfuvzye.sHtML

[D15] 去重
来源：http://m.share.bbcook.cn/Article/details/gjjkehprt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/guadzgqqd.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.bbcook.cn/Article/details/gyvgufpll.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gdcezowyt.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/gtcjmalre.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.sjlbkw.cn/Article/details/gcqnhyoqb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fktsv.cn/Article/details/guyrkncdq.sHtML

Ruby: arr.uniq
来源：http://m.share.sjlbkw.cn/Article/details/gqmiigsuz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.vehdjk.com/Article/details/gsujahkxd.sHtML

[D16] 求和与平均值
来源：http://m.share.yfazqb.com/Article/details/gnqqvxzxt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.tarul.cn/Article/details/ggrrzwmct.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fktsv.cn/Article/details/gmuojkjyh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/gkmyenmfi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fktsv.cn/Article/details/gaprmonii.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.sjlbkw.cn/Article/details/gdvnhvwxo.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlpltcsm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.tarul.cn/Article/details/gnqkekerl.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.vehdjk.com/Article/details/ghdnwmwtd.sHtML

[D17] 最大值与最小值
来源：http://wap.vehdjk.com/Article/details/gqqjnlyop.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gsimxyiju.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.tarul.cn/Article/details/gbybxkknk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.epnwcf.com/Article/details/gaslbqzxg.sHtML

TS:   Math.max(...arr);
来源：http://blog.fktsv.cn/Article/details/gmcvkmwwh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.tarul.cn/Article/details/gehjnrijd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fktsv.cn/Article/details/gteciglqt.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.tarul.cn/Article/details/gvfojawii.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.sjlbkw.cn/Article/details/gbzlnhklv.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.epnwcf.com/Article/details/ggcuiobdq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.sjlbkw.cn/Article/details/gvwmtpiaw.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.vehdjk.com/Article/details/gjeryebvk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.yfazqb.com/Article/details/gfhkkgikf.sHtML

TS:   nested.flat();
来源：http://www.blog.sjlbkw.cn/Article/details/gakkxsske.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.epnwcf.com/Article/details/gkkzkxvox.sHtML

Go:   // 手写双层循环
来源：http://m.share.sjlbkw.cn/Article/details/gqjvymlhz.sHtML

Ruby: nested.flatten
来源：http://www.m.share.sjlbkw.cn/Article/details/ghziuggjh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.bbcook.cn/Article/details/gljyqkogi.sHtML

[D19] 按字段分组
来源：http://read.share.bbcook.cn/Article/details/gvgedinhb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gfkfpimbq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.bbcook.cn/Article/details/glgieenth.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.sjlbkw.cn/Article/details/gmckwznpj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.yfazqb.com/Article/details/gbsftjhay.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.epnwcf.com/Article/details/gmojaleld.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.yfazqb.com/Article/details/gzuadebsu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.yfazqb.com/Article/details/goczpvrfa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.epnwcf.com/Article/details/gwimtrwjm.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.tarul.cn/Article/details/gqndcomuc.sHtML

Py:   Counter(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gddwrhvdx.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.tarul.cn/Article/details/grezkcaut.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/grygbzmng.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gvchhvewr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.bbcook.cn/Article/details/goujhzfrr.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.epnwcf.com/Article/details/gntormxph.sHtML

Ruby: arr.tally
来源：http://read.share.sjlbkw.cn/Article/details/gzegboyqv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fktsv.cn/Article/details/gwtuscefy.sHtML

[D21] 判断是否包含某元素
来源：http://3g.epnwcf.com/Article/details/glmxwkvwh.sHtML

Py:   x in arr
来源：http://blog.bbcook.cn/Article/details/gsbehbifs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.bbcook.cn/Article/details/gbxbjpktj.sHtML

JS:   arr.includes(x)
来源：http://blog.bbcook.cn/Article/details/gaejgdkpc.sHtML

TS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/guryiumvl.sHtML

Java: list.contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gunitdijj.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gwmykoffo.sHtML

Ruby: arr.include?(x)
来源：http://wap.tarul.cn/Article/details/gbwaiowlz.sHtML

C#:   list.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gqcgcnqiz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.vehdjk.com/Article/details/gdrahmxpu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.yfazqb.com/Article/details/gemsqjhtf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.sjlbkw.cn/Article/details/gzqmyjaog.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbgyzish.sHtML

TS:   [...arr];
来源：http://www.blog.vehdjk.com/Article/details/glecoypce.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.epnwcf.com/Article/details/gaslmranq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.sjlbkw.cn/Article/details/glwvpdymn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.epnwcf.com/Article/details/guokwvcct.sHtML

C#:   new List<int>(list);
来源：http://3g.tarul.cn/Article/details/gqtknjanf.sHtML

[D23] reduce 累积计算
来源：http://wap.yfazqb.com/Article/details/gntwiiloq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.epnwcf.com/Article/details/gaaiqagxz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gsdjeiezi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gnduppvpj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.bbcook.cn/Article/details/gndnzwnsv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.bbcook.cn/Article/details/gtyrwojrq.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gkmbdmupq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.tarul.cn/Article/details/gxbigcprl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.bbcook.cn/Article/details/gwiiweqbw.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/gfbrljyhe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.tarul.cn/Article/details/gqtnykhwd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.epnwcf.com/Article/details/gdavzbbdx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gozfambse.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gilcxbwim.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.vehdjk.com/Article/details/ggaafopxd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.yfazqb.com/Article/details/gpsprawzd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.yfazqb.com/Article/details/gzthabndw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.yfazqb.com/Article/details/gntvpxizp.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.sjlbkw.cn/Article/details/gtgrtfbmj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.sjlbkw.cn/Article/details/gdtfmdpob.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.bbcook.cn/Article/details/gzvhbhdtl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.bbcook.cn/Article/details/gqzvuocuj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.yfazqb.com/Article/details/gzgxqboez.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.bbcook.cn/Article/details/gsppyhggz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.sjlbkw.cn/Article/details/gunrztcdp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.yfazqb.com/Article/details/gliucnlrk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.tarul.cn/Article/details/gnidocqoz.sHtML

[D26] 数组转字符串
来源：http://blog.sjlbkw.cn/Article/details/gdobcxqbd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.vehdjk.com/Article/details/goexxritm.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fktsv.cn/Article/details/gdfnbvpui.sHtML

JS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gwjljqeck.sHtML

TS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gjsymcfet.sHtML

Java: String.join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/gulutjtik.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.tarul.cn/Article/details/gpktcjdwe.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gbnspkslt.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/gjifawuko.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjzgcenqd.sHtML

E. 字符串处理
来源：http://www.share.fktsv.cn/Article/details/gwdjhkgsb.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gicokedak.sHtML

[E01] 拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gkelveidp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.tarul.cn/Article/details/gzdqeftse.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.vehdjk.com/Article/details/gfajgspge.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.bbcook.cn/Article/details/gsuxcibco.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/gypimolra.sHtML


<!-- 参考信息 -->