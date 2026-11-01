代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.yfazqb.com/Article/details/gdxgguhix.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.vehdjk.com/Article/details/gduvdjbrw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/giqjfyloo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.sjlbkw.cn/Article/details/glewcpdgg.sHtML

[C10] 变量作用域
来源：http://www.m.share.yfazqb.com/Article/details/goayigosw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.tarul.cn/Article/details/goyuksgsc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fktsv.cn/Article/details/gjekrhehf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/gywldghjd.sHtML

TS:   同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gylczyhol.sHtML

Java: 方法内为块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gicidbgzv.sHtML

Go:   花括号块级作用域
来源：http://wap.bbcook.cn/Article/details/geihablvj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.sjlbkw.cn/Article/details/gzgqxegxy.sHtML

C#:   块级作用域
来源：http://mobile.yfazqb.com/Article/details/gmzbyisrt.sHtML

[C11] 模块导入与导出
来源：http://www.blog.sjlbkw.cn/Article/details/gycaiycyt.sHtML

Py:   from module import func
来源：http://wap.vehdjk.com/Article/details/glwuqiwkz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.sjlbkw.cn/Article/details/gakplldik.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.bbcook.cn/Article/details/ggvohvens.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.epnwcf.com/Article/details/gquuvidee.sHtML

Java: import java.util.List;
来源：http://m.share.sjlbkw.cn/Article/details/gbrbagnmn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.vehdjk.com/Article/details/gvtloklxf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.tarul.cn/Article/details/grysottgi.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gsubkwvpo.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.epnwcf.com/Article/details/gpgelgwos.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.epnwcf.com/Article/details/gjqkjqeqa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.bbcook.cn/Article/details/gjupipbie.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gxdnvahdu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fktsv.cn/Article/details/gokaeuqiu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.yfazqb.com/Article/details/gipiyndjc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.yfazqb.com/Article/details/gepctxlyh.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.epnwcf.com/Article/details/gzkpsstpi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.vehdjk.com/Article/details/gcvawcinw.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.bbcook.cn/Article/details/gndydeicj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.sjlbkw.cn/Article/details/gajqkxdtn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gbvrxduju.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.epnwcf.com/Article/details/gaadmfvoa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/ghtxxzahk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gvnxzrfqq.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.yfazqb.com/Article/details/gdhptrper.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.vehdjk.com/Article/details/glrtxxhqr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fktsv.cn/Article/details/gmekderns.sHtML

[C14] 泛型函数
来源：http://blog.vehdjk.com/Article/details/gzstdhmzy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fktsv.cn/Article/details/gjvcpgtdz.sHtML

PHP:  // 无泛型
来源：http://mobile.tarul.cn/Article/details/gcyapexmk.sHtML

JS:   // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gkfddorot.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.sjlbkw.cn/Article/details/gtqdgzqgp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.epnwcf.com/Article/details/gxqipebzk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.sjlbkw.cn/Article/details/guaebgfhd.sHtML

Ruby: # 无泛型
来源：http://www.share.fktsv.cn/Article/details/gyqmtwwtm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.vehdjk.com/Article/details/gdmizrefm.sHtML

[C15] 解构 / 展开参数
来源：http://wap.tarul.cn/Article/details/gumpobvlp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.vehdjk.com/Article/details/gwocljeuf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fktsv.cn/Article/details/gwazizqbk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/gwnwqiohd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.epnwcf.com/Article/details/gjshlchna.sHtML

Java: // 无解构
来源：http://mobile.fktsv.cn/Article/details/gtrjbyuyt.sHtML

Go:   // 无解构
来源：http://3g.fktsv.cn/Article/details/gmsqfchas.sHtML

Ruby: a, b = pair
来源：http://wap.fktsv.cn/Article/details/gqlquujda.sHtML

C#:   var (a, b) = pair;
来源：http://wap.bbcook.cn/Article/details/gjtqiohln.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.yfazqb.com/Article/details/grlgkahgj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gfcriwele.sHtML

PHP:  // 无重载
来源：http://3g.yfazqb.com/Article/details/gpaayvcet.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.tarul.cn/Article/details/gtxckhzww.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.sjlbkw.cn/Article/details/gzckasphl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.sjlbkw.cn/Article/details/gykqnvosg.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.tarul.cn/Article/details/gzqgjflqz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fktsv.cn/Article/details/ggbhawjdt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fktsv.cn/Article/details/gsdzjisls.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gmwuuctyu.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fktsv.cn/Article/details/ghlxwodzv.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gookirnlb.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/gbrhyojbw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.vehdjk.com/Article/details/gmmduqxmo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.bbcook.cn/Article/details/ghlvczwlo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.tarul.cn/Article/details/gnxdhypje.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.vehdjk.com/Article/details/gbzdhzgyk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fktsv.cn/Article/details/gtpzskzba.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/giofqtqlp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.bbcook.cn/Article/details/goqedsivz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.epnwcf.com/Article/details/gurwgwpek.sHtML

[D02] 追加元素到末尾
来源：http://wap.tarul.cn/Article/details/gvowyiexu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.yfazqb.com/Article/details/gwqrsqumt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fktsv.cn/Article/details/ghbccbrtf.sHtML

JS:   arr.push(4);
来源：http://m.share.bbcook.cn/Article/details/gjpdtrzxf.sHtML

TS:   arr.push(4);
来源：http://m.share.bbcook.cn/Article/details/gthpuuhdq.sHtML

Java: list.add(4);
来源：http://baike.bbcook.cn/Article/details/gjcoprkav.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.vehdjk.com/Article/details/gvenodzsp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fktsv.cn/Article/details/gvtkkykrg.sHtML

C#:   list.Add(4);
来源：http://baike.sjlbkw.cn/Article/details/gfvkynmga.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.bbcook.cn/Article/details/gqshzaclu.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.epnwcf.com/Article/details/glexsgesg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.vehdjk.com/Article/details/gqqyurbex.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.yfazqb.com/Article/details/gemrwlubx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.epnwcf.com/Article/details/gsahijzki.sHtML

Java: list.add(0, 0);
来源：http://m.share.fktsv.cn/Article/details/gtryxpxqz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/grqjirqbf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.vehdjk.com/Article/details/ggkssarcw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gpwwlggsr.sHtML

[D04] 删除元素
来源：http://m.share.yfazqb.com/Article/details/gxaycazet.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fktsv.cn/Article/details/gptwcrziw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.epnwcf.com/Article/details/gsmucohte.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fktsv.cn/Article/details/gwmpieiva.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fktsv.cn/Article/details/getgxvfsg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.sjlbkw.cn/Article/details/goaksifgf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.vehdjk.com/Article/details/gdpxtkixi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fktsv.cn/Article/details/gpnuewvhz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.bbcook.cn/Article/details/gndqkimpv.sHtML

[D05] 访问与修改元素
来源：http://3g.yfazqb.com/Article/details/gfcdicdrp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/gcyaccebb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gszrbdxta.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gcgasukbs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.tarul.cn/Article/details/gxnejoisd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.tarul.cn/Article/details/gojblgiec.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gmhkklomx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/ghdjdvpun.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.tarul.cn/Article/details/gqqqcylfr.sHtML

[D06] 数组长度
来源：http://mobile.vehdjk.com/Article/details/gfuhvrkbs.sHtML

Py:   len(arr)
来源：http://mobile.tarul.cn/Article/details/gnycjogqj.sHtML

PHP:  count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gqpyipkat.sHtML

JS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/ghyvgrwob.sHtML

TS:   arr.length
来源：http://www.m.share.epnwcf.com/Article/details/gkawxmimd.sHtML

Java: list.size();
来源：http://www.m.share.sjlbkw.cn/Article/details/gzomiftqq.sHtML

Go:   len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gmdgcdool.sHtML

Ruby: arr.length; arr.size
来源：http://baike.yfazqb.com/Article/details/gxlmhhilt.sHtML

C#:   list.Count;
来源：http://www.m.share.bbcook.cn/Article/details/gvjzagecc.sHtML

[D07] 切片 / 取子数组
来源：http://wap.yfazqb.com/Article/details/grjgupvel.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fktsv.cn/Article/details/gqrnxtkkj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.tarul.cn/Article/details/gsuacezox.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fktsv.cn/Article/details/ghseewsge.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.tarul.cn/Article/details/gtpobodjl.sHtML

Java: list.subList(1, 4);
来源：http://m.share.epnwcf.com/Article/details/guzhfqfly.sHtML

Go:   arr[1:4]
来源：http://baike.vehdjk.com/Article/details/gxpxdrfws.sHtML

Ruby: arr[1, 3]
来源：http://mobile.vehdjk.com/Article/details/grhlsptbl.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.bbcook.cn/Article/details/gwmvtscwd.sHtML

[D08] 合并两个数组
来源：http://www.share.fktsv.cn/Article/details/gpcieatjx.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.sjlbkw.cn/Article/details/ggajfzrmd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.sjlbkw.cn/Article/details/gfnsxnldk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.vehdjk.com/Article/details/gdjimkwjt.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.epnwcf.com/Article/details/gbunmdqph.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fktsv.cn/Article/details/gkgrgfeky.sHtML

Go:   append(a, b...)
来源：http://3g.yfazqb.com/Article/details/guobcqocc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.yfazqb.com/Article/details/gnnoggexe.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.bbcook.cn/Article/details/gggvhymtn.sHtML

[D09] 排序（升序）
来源：http://blog.sjlbkw.cn/Article/details/gcsfxrsqv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.epnwcf.com/Article/details/gpnptljco.sHtML

PHP:  sort($arr);
来源：http://www.blog.tarul.cn/Article/details/glqvnpnsl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.yfazqb.com/Article/details/gzjhkcggx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.epnwcf.com/Article/details/giakiscon.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.sjlbkw.cn/Article/details/gckoteqlm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gdjwaxmvx.sHtML

Ruby: arr.sort
来源：http://read.share.yfazqb.com/Article/details/gzsfajdkr.sHtML

C#:   list.Sort();
来源：http://read.share.sjlbkw.cn/Article/details/gqyzshkpx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.yfazqb.com/Article/details/gwvyzafzx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.vehdjk.com/Article/details/glgfcmpje.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/gwxkxjksq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.sjlbkw.cn/Article/details/gnvjmvxqz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.sjlbkw.cn/Article/details/gjddtmpnw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.epnwcf.com/Article/details/gjwpbvquz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fktsv.cn/Article/details/gheucnjya.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.epnwcf.com/Article/details/gkfjvszxp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.yfazqb.com/Article/details/gwqekmvcp.sHtML

[D11] 反转数组
来源：http://baike.bbcook.cn/Article/details/gxeqiyzix.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.sjlbkw.cn/Article/details/ggrhcvcnp.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/gdxfyohsh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.yfazqb.com/Article/details/gxjzjulot.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fktsv.cn/Article/details/glqwdbfcv.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.bbcook.cn/Article/details/gljsowezl.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.epnwcf.com/Article/details/gqyhmxyis.sHtML

Ruby: arr.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhlngjqp.sHtML

C#:   list.Reverse();
来源：http://www.share.tarul.cn/Article/details/grjfscyhc.sHtML

[D12] 查找元素下标
来源：http://m.share.fktsv.cn/Article/details/gojjnvwlm.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.vehdjk.com/Article/details/gsvoykega.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.epnwcf.com/Article/details/gvbydnfge.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.epnwcf.com/Article/details/gcazjqtfq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/gutmdeskg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.yfazqb.com/Article/details/gznkvnfsk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.tarul.cn/Article/details/glmktyqfh.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fktsv.cn/Article/details/gowhggoiu.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.vehdjk.com/Article/details/gczonjllu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.bbcook.cn/Article/details/guisczyqg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.vehdjk.com/Article/details/ggxeczqiq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.epnwcf.com/Article/details/gnptoyfzv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gcnvlqxlv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.tarul.cn/Article/details/grskgxbib.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.tarul.cn/Article/details/gvupkysco.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.epnwcf.com/Article/details/gsujbizbl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.yfazqb.com/Article/details/gbmacbqsu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gywaydvrd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.bbcook.cn/Article/details/giiaiaqon.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.tarul.cn/Article/details/ghctvfbfi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.epnwcf.com/Article/details/gqfkwzzpi.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gxbspohxu.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gldvtihas.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.vehdjk.com/Article/details/gqsxiykon.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/gmlcxjqmx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gkgnsjpce.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gbndlxoow.sHtML

[D15] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gxxwjaogf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.epnwcf.com/Article/details/gumynkqvy.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fktsv.cn/Article/details/gemwtgfvg.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gwcrcliza.sHtML

TS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gfiasunyg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.bbcook.cn/Article/details/gjbahtglm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.tarul.cn/Article/details/ggoqhsvyb.sHtML

Ruby: arr.uniq
来源：http://mobile.vehdjk.com/Article/details/gfatnfrnu.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.epnwcf.com/Article/details/gvjpcyvdy.sHtML

[D16] 求和与平均值
来源：http://m.share.fktsv.cn/Article/details/ghtiwcwjg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gnwchxufg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.vehdjk.com/Article/details/gbmhwjjwn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gjvikdlwu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gazxtorim.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.tarul.cn/Article/details/ghpfjyllz.sHtML

Go:   // 手写循环累加
来源：http://3g.sjlbkw.cn/Article/details/gdiwhkfgn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fktsv.cn/Article/details/gbhnglmrg.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.yfazqb.com/Article/details/gjtaptohs.sHtML

[D17] 最大值与最小值
来源：http://blog.tarul.cn/Article/details/gcefgoech.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/gcmyqsqgm.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.epnwcf.com/Article/details/ghjzctofp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.tarul.cn/Article/details/golsdbgbe.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fktsv.cn/Article/details/gdlejbzyw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gglewtcoq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.yfazqb.com/Article/details/gisdlwvxw.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fktsv.cn/Article/details/gbqltptlg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.epnwcf.com/Article/details/gvafgdekd.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.sjlbkw.cn/Article/details/gmfggnsee.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.bbcook.cn/Article/details/geoivjwdq.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fktsv.cn/Article/details/gigqfkcnd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.epnwcf.com/Article/details/grneodxxe.sHtML

TS:   nested.flat();
来源：http://read.share.bbcook.cn/Article/details/geadiwjya.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gkikacfhe.sHtML

Go:   // 手写双层循环
来源：http://mobile.epnwcf.com/Article/details/ggtzlxqay.sHtML

Ruby: nested.flatten
来源：http://baike.bbcook.cn/Article/details/gwbzlkvln.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gfkvllnxc.sHtML

[D19] 按字段分组
来源：http://baike.vehdjk.com/Article/details/gmbvelobt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.tarul.cn/Article/details/gbrlohwyr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.yfazqb.com/Article/details/gxhdxffgu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.epnwcf.com/Article/details/gewfivxdv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.sjlbkw.cn/Article/details/gziivdjxz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.epnwcf.com/Article/details/gspozrzid.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fktsv.cn/Article/details/gyvmqmeoa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.epnwcf.com/Article/details/gvzhdwurg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.yfazqb.com/Article/details/gzkgzlhli.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.vehdjk.com/Article/details/gxkefmmxg.sHtML

Py:   Counter(arr)
来源：http://wap.tarul.cn/Article/details/gmfqgjpej.sHtML

PHP:  array_count_values($arr);
来源：http://blog.yfazqb.com/Article/details/gdiczvwfk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/ggksghbal.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.bbcook.cn/Article/details/gsffkdziu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.epnwcf.com/Article/details/gtrolxqxd.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.tarul.cn/Article/details/grdanfhsq.sHtML

Ruby: arr.tally
来源：http://wap.sjlbkw.cn/Article/details/gkyrnoaji.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.vehdjk.com/Article/details/gxpvwgqzp.sHtML

[D21] 判断是否包含某元素
来源：http://wap.tarul.cn/Article/details/gibfhwhpm.sHtML

Py:   x in arr
来源：http://baike.tarul.cn/Article/details/gedrospvh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.sjlbkw.cn/Article/details/grsfzdbpj.sHtML

JS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gufdrhwns.sHtML

TS:   arr.includes(x)
来源：http://wap.vehdjk.com/Article/details/gswdlvjgl.sHtML

Java: list.contains(x)
来源：http://wap.tarul.cn/Article/details/gjwohsyrt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdciqajll.sHtML

Ruby: arr.include?(x)
来源：http://www.share.epnwcf.com/Article/details/gelpttqlf.sHtML

C#:   list.Contains(x)
来源：http://www.share.yfazqb.com/Article/details/grmdjcpij.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/gecyncpnp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.tarul.cn/Article/details/gameehafp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.tarul.cn/Article/details/gbjgkkbgm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.yfazqb.com/Article/details/geiexjnwp.sHtML

TS:   [...arr];
来源：http://wap.fktsv.cn/Article/details/grsmfvtow.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gtbizyliu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.yfazqb.com/Article/details/gvfcfidbr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.vehdjk.com/Article/details/gwqtdjexg.sHtML

C#:   new List<int>(list);
来源：http://m.share.fktsv.cn/Article/details/gyymwfbqh.sHtML

[D23] reduce 累积计算
来源：http://blog.epnwcf.com/Article/details/gudtxtycs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fktsv.cn/Article/details/gdyhheeza.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.epnwcf.com/Article/details/gnkfgvpss.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.vehdjk.com/Article/details/getzbznjy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/gekkhxnci.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.yfazqb.com/Article/details/gpfqdqiqo.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/grzphzozy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.epnwcf.com/Article/details/gkhtnfdct.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.vehdjk.com/Article/details/gwtknfrvf.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.epnwcf.com/Article/details/gazoipmzc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.sjlbkw.cn/Article/details/gxkjzkvbx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.yfazqb.com/Article/details/goxhdugye.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fktsv.cn/Article/details/gldqhoeou.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gahgbsdfx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.yfazqb.com/Article/details/gkyclxxae.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.sjlbkw.cn/Article/details/gkbqcffup.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.vehdjk.com/Article/details/gghsrhpqy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.vehdjk.com/Article/details/gjphmwmdp.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.yfazqb.com/Article/details/gfqtomcic.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.sjlbkw.cn/Article/details/gfxhmnrgm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.vehdjk.com/Article/details/ggovtwdea.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fktsv.cn/Article/details/gravemcbk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.tarul.cn/Article/details/ggzuklgci.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/giwsgswls.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.yfazqb.com/Article/details/gvsjxotrt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.yfazqb.com/Article/details/gpfdbkkmm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gfrzvstqt.sHtML

[D26] 数组转字符串
来源：http://baike.epnwcf.com/Article/details/gbkoyhrff.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.vehdjk.com/Article/details/giqvyqqoa.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gsycftpeq.sHtML

JS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gfrqdktsz.sHtML

TS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gfxibquqb.sHtML


<!-- 参考信息 -->