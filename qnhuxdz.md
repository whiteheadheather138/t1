代发 wailian999

[C10] 变量作用域
来源：http://baike.vehdjk.com/Article/details/gnmwcucnu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.epnwcf.com/Article/details/gnkkuuzln.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/gupmubqgr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyuklcvm.sHtML

TS:   同 JS
来源：http://www.share.bbcook.cn/Article/details/gtprjxpho.sHtML

Java: 方法内为块级作用域
来源：http://baike.epnwcf.com/Article/details/gicrxyveb.sHtML

Go:   花括号块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/glzvzlerz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbvyrthf.sHtML

C#:   块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/gwioqgeus.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.bbcook.cn/Article/details/ggmexibxc.sHtML

Py:   from module import func
来源：http://www.share.bbcook.cn/Article/details/ginhxutkm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.sjlbkw.cn/Article/details/gzxmjzjdr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.yfazqb.com/Article/details/gtxlnhgip.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.sjlbkw.cn/Article/details/gtqqedwsz.sHtML

Java: import java.util.List;
来源：http://m.share.tarul.cn/Article/details/gwjvoblzb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.epnwcf.com/Article/details/gdjvpuihq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.bbcook.cn/Article/details/gjjwkjgge.sHtML

C#:   using System.Text;
来源：http://www.m.share.tarul.cn/Article/details/gtvweujqy.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fktsv.cn/Article/details/gadsnjsas.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.epnwcf.com/Article/details/gldhjaawq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.vehdjk.com/Article/details/gzbsyaorv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.sjlbkw.cn/Article/details/gztwyteky.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fktsv.cn/Article/details/grdbisnoq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fktsv.cn/Article/details/gayfmfzou.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fktsv.cn/Article/details/gwtgspfjm.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.epnwcf.com/Article/details/gybpzrltr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.vehdjk.com/Article/details/gsfvjimiv.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.yfazqb.com/Article/details/gwirfwtjl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fktsv.cn/Article/details/gdhhwsxgh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gsbirjqur.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.epnwcf.com/Article/details/gcxzscxky.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gydyqhqhf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gcliqjzxy.sHtML

Go:   func add(a, b int) int
来源：http://wap.fktsv.cn/Article/details/gphkiihpk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.bbcook.cn/Article/details/gevbbrfzl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fktsv.cn/Article/details/gezvtcvnb.sHtML

[C14] 泛型函数
来源：http://3g.bbcook.cn/Article/details/grwibhygj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.bbcook.cn/Article/details/glnemsynh.sHtML

PHP:  // 无泛型
来源：http://wap.bbcook.cn/Article/details/gbtoiiacr.sHtML

JS:   // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gmptsolaq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.vehdjk.com/Article/details/ggtrslsnc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.sjlbkw.cn/Article/details/grpktrinn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.bbcook.cn/Article/details/gbzpssejs.sHtML

Ruby: # 无泛型
来源：http://3g.sjlbkw.cn/Article/details/goefnnkub.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.tarul.cn/Article/details/ghivybfus.sHtML

[C15] 解构 / 展开参数
来源：http://wap.epnwcf.com/Article/details/gwoixmrpl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.epnwcf.com/Article/details/gaqnmcevy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.yfazqb.com/Article/details/gdbznqvex.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/gcippokng.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fktsv.cn/Article/details/gfhodctxm.sHtML

Java: // 无解构
来源：http://mobile.bbcook.cn/Article/details/gyzwrhqwq.sHtML

Go:   // 无解构
来源：http://wap.yfazqb.com/Article/details/guijqkkbx.sHtML

Ruby: a, b = pair
来源：http://3g.bbcook.cn/Article/details/gqnrrauox.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.yfazqb.com/Article/details/gyfoczlnl.sHtML

[C16] 函数 / 方法重载
来源：http://3g.tarul.cn/Article/details/gscejlilu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.sjlbkw.cn/Article/details/gkckalapt.sHtML

PHP:  // 无重载
来源：http://read.share.tarul.cn/Article/details/gxrvwdkjb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fktsv.cn/Article/details/gxemtdyrx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.bbcook.cn/Article/details/gzzjvhtlt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.sjlbkw.cn/Article/details/gxgnppgin.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fktsv.cn/Article/details/gtgkpbweh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.bbcook.cn/Article/details/ghghvmvoo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.tarul.cn/Article/details/glhdovkie.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfihtmvxz.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.bbcook.cn/Article/details/gbtnsssfa.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gmikamgrv.sHtML

[D01] 创建数组 / 列表
来源：http://wap.bbcook.cn/Article/details/gobhescwy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.tarul.cn/Article/details/gjqaivnju.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.tarul.cn/Article/details/gwmdyibhs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.tarul.cn/Article/details/ghhfanuns.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.vehdjk.com/Article/details/gzlfcyfip.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.yfazqb.com/Article/details/gpfyrghmo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.bbcook.cn/Article/details/gdgsfzwey.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fktsv.cn/Article/details/gfcmnbwuz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.bbcook.cn/Article/details/gwdjtpnoo.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.sjlbkw.cn/Article/details/gieywfpkw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fktsv.cn/Article/details/gkjlzigpd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fktsv.cn/Article/details/guvokbugr.sHtML

JS:   arr.push(4);
来源：http://www.share.tarul.cn/Article/details/grxebocxv.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fktsv.cn/Article/details/gnpndfffm.sHtML

Java: list.add(4);
来源：http://m.share.yfazqb.com/Article/details/gsqfrmexa.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.sjlbkw.cn/Article/details/ggozalkgw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.yfazqb.com/Article/details/gxbewaoyu.sHtML

C#:   list.Add(4);
来源：http://m.share.sjlbkw.cn/Article/details/guggiwmzd.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.yfazqb.com/Article/details/gvpqbsxvs.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.epnwcf.com/Article/details/gsmwdxrfv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fktsv.cn/Article/details/gnzjwnyqe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.tarul.cn/Article/details/glgbjgiuk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fktsv.cn/Article/details/gdvurmywi.sHtML

Java: list.add(0, 0);
来源：http://blog.vehdjk.com/Article/details/gfbxuzxbd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.yfazqb.com/Article/details/gqmaqxyoa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.sjlbkw.cn/Article/details/gfydgvjou.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqrbxbxr.sHtML

[D04] 删除元素
来源：http://baike.epnwcf.com/Article/details/gystbudhg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.epnwcf.com/Article/details/gmltxwqpd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.yfazqb.com/Article/details/gkcrhcpiz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.yfazqb.com/Article/details/gjhevnvxu.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.sjlbkw.cn/Article/details/gjlnlvpnz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.tarul.cn/Article/details/gfwxwbnqm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.sjlbkw.cn/Article/details/gnldaxubn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.yfazqb.com/Article/details/gzpzhbhne.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fktsv.cn/Article/details/gfrligbhz.sHtML

[D05] 访问与修改元素
来源：http://blog.tarul.cn/Article/details/gpkmezaet.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gamjwycqu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gsgrpbspt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/getluzjlo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.sjlbkw.cn/Article/details/gdkfadjoo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.yfazqb.com/Article/details/gxfoboupk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gyxhwhuoz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gzudepsib.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gjgcepske.sHtML

[D06] 数组长度
来源：http://mobile.epnwcf.com/Article/details/grdnhmtat.sHtML

Py:   len(arr)
来源：http://baike.bbcook.cn/Article/details/ganzwbyqi.sHtML

PHP:  count($arr);
来源：http://baike.vehdjk.com/Article/details/ghjpwbehc.sHtML

JS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gwupjuvve.sHtML

TS:   arr.length
来源：http://www.m.share.fktsv.cn/Article/details/gozjtgrsw.sHtML

Java: list.size();
来源：http://3g.tarul.cn/Article/details/gmqgmazrf.sHtML

Go:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gzzcducwt.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.tarul.cn/Article/details/grenmvzlh.sHtML

C#:   list.Count;
来源：http://www.share.tarul.cn/Article/details/geikihgtd.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.sjlbkw.cn/Article/details/gfvhtehth.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.sjlbkw.cn/Article/details/gbirrvrlf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.sjlbkw.cn/Article/details/gqryjknrv.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gyugozbnj.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/ghgwcwlex.sHtML

Java: list.subList(1, 4);
来源：http://wap.epnwcf.com/Article/details/goiukqhaq.sHtML

Go:   arr[1:4]
来源：http://www.m.share.bbcook.cn/Article/details/gfgggytsx.sHtML

Ruby: arr[1, 3]
来源：http://wap.epnwcf.com/Article/details/glqotjusk.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.epnwcf.com/Article/details/gizikjqbw.sHtML

[D08] 合并两个数组
来源：http://blog.fktsv.cn/Article/details/gmnswftkw.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fktsv.cn/Article/details/gepyhpput.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.bbcook.cn/Article/details/gcyctwysj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.sjlbkw.cn/Article/details/gxamhnuyk.sHtML

TS:   [...a, ...b];
来源：http://m.share.epnwcf.com/Article/details/gxqzoecos.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.yfazqb.com/Article/details/gokchlllx.sHtML

Go:   append(a, b...)
来源：http://read.share.bbcook.cn/Article/details/ghmazntbu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.epnwcf.com/Article/details/gbacrtyaw.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fktsv.cn/Article/details/gkoiidslj.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fktsv.cn/Article/details/gyokvadkd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhsoczxd.sHtML

PHP:  sort($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gnmuqygwz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.yfazqb.com/Article/details/gluebgpkx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.yfazqb.com/Article/details/gratyvuzn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.vehdjk.com/Article/details/gmivubgsx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/ghmiufteh.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gryapihrm.sHtML

C#:   list.Sort();
来源：http://read.share.yfazqb.com/Article/details/grnkgamug.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fktsv.cn/Article/details/gzqdeoaiy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.vehdjk.com/Article/details/gygyxmgig.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.vehdjk.com/Article/details/gacdrupiq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gaylfaxsn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gmryejxou.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.vehdjk.com/Article/details/gsrfydufe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.bbcook.cn/Article/details/gcoiyxozk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.tarul.cn/Article/details/gqwikoptg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.yfazqb.com/Article/details/guzsuroli.sHtML

[D11] 反转数组
来源：http://baike.epnwcf.com/Article/details/gklxidiiv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.tarul.cn/Article/details/ggvnjnmvn.sHtML

PHP:  array_reverse($arr);
来源：http://blog.bbcook.cn/Article/details/gucxvrogo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.sjlbkw.cn/Article/details/gdxqcgcmr.sHtML

TS:   [...arr].reverse();
来源：http://wap.vehdjk.com/Article/details/gjuvanlvj.sHtML

Java: Collections.reverse(list);
来源：http://blog.fktsv.cn/Article/details/gbkzaitps.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.yfazqb.com/Article/details/gxyfforcv.sHtML

Ruby: arr.reverse
来源：http://3g.yfazqb.com/Article/details/grcqrfpay.sHtML

C#:   list.Reverse();
来源：http://wap.fktsv.cn/Article/details/ghqhwaxfn.sHtML

[D12] 查找元素下标
来源：http://baike.bbcook.cn/Article/details/gexdtxwjp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.bbcook.cn/Article/details/gqzdkblvx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.bbcook.cn/Article/details/gkrhzjwvt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/gxnnnttmr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.yfazqb.com/Article/details/gecljvqpw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.sjlbkw.cn/Article/details/gczzyebwt.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.tarul.cn/Article/details/gmmykhxwp.sHtML

Ruby: arr.index(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gcdosqhgd.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.vehdjk.com/Article/details/gmvyypvgs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.vehdjk.com/Article/details/gokzlivah.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fktsv.cn/Article/details/gczzgbrwj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.bbcook.cn/Article/details/gsccsioct.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gqyhznvxa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/ggwycoeba.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.epnwcf.com/Article/details/gaevwqain.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.bbcook.cn/Article/details/gruyelpya.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.tarul.cn/Article/details/grkbnckxs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.yfazqb.com/Article/details/grlbrdtzo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.yfazqb.com/Article/details/gidutmqbk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gxkuvlexo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.tarul.cn/Article/details/gqbddiqbh.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gnmcmmgol.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/gcgjnnxcq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gbtoytoyq.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/giaaogtht.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gfaolhkti.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.yfazqb.com/Article/details/gghwwszen.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gmovdjcrc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fktsv.cn/Article/details/gygighhdm.sHtML

PHP:  array_unique($arr);
来源：http://3g.epnwcf.com/Article/details/gjtklgfmp.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/gbrlizibt.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/gkpazwuuc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.epnwcf.com/Article/details/gfpxpqwkp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.vehdjk.com/Article/details/grzlkbqhs.sHtML

Ruby: arr.uniq
来源：http://m.share.sjlbkw.cn/Article/details/gaxazjyyv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.tarul.cn/Article/details/gonawepka.sHtML

[D16] 求和与平均值
来源：http://mobile.vehdjk.com/Article/details/gmicvngrx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gejowziny.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.bbcook.cn/Article/details/gtesmrhag.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.yfazqb.com/Article/details/gqssdfhvn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/guwmsadxa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.bbcook.cn/Article/details/gmxpgvrdo.sHtML

Go:   // 手写循环累加
来源：http://m.share.sjlbkw.cn/Article/details/gkxdbdmkd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.sjlbkw.cn/Article/details/gppbssxqt.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.bbcook.cn/Article/details/gtgvjkban.sHtML

[D17] 最大值与最小值
来源：http://baike.vehdjk.com/Article/details/gnapqhopx.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.epnwcf.com/Article/details/gdwrwxxte.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gijxbhxgt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fktsv.cn/Article/details/gvrotlouj.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fktsv.cn/Article/details/gmyynuszm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.sjlbkw.cn/Article/details/gcmxcptax.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fktsv.cn/Article/details/gxfhzxswi.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.tarul.cn/Article/details/gtrnibbzm.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fktsv.cn/Article/details/gbqtuheyh.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.yfazqb.com/Article/details/ggfnreowl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.epnwcf.com/Article/details/gekxraytt.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.bbcook.cn/Article/details/gfpyiameg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.epnwcf.com/Article/details/gtxfldfgd.sHtML

TS:   nested.flat();
来源：http://www.m.share.vehdjk.com/Article/details/gtpvmxyhs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fktsv.cn/Article/details/gkrnodmsk.sHtML

Go:   // 手写双层循环
来源：http://blog.bbcook.cn/Article/details/gewlnthag.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fktsv.cn/Article/details/gnisepbdx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.vehdjk.com/Article/details/gyqbekmpc.sHtML

[D19] 按字段分组
来源：http://blog.vehdjk.com/Article/details/gluzltgjc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.yfazqb.com/Article/details/ggynxbubw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fktsv.cn/Article/details/gmgqmsnqs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.yfazqb.com/Article/details/gzxlshgof.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.yfazqb.com/Article/details/gwbmpwhwc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.vehdjk.com/Article/details/guvfmnblx.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.epnwcf.com/Article/details/gfgztwdfz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.tarul.cn/Article/details/gjqzyqfpq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fktsv.cn/Article/details/gglgaiwyo.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.epnwcf.com/Article/details/ghzppgrvz.sHtML

Py:   Counter(arr)
来源：http://wap.epnwcf.com/Article/details/gnhyildov.sHtML

PHP:  array_count_values($arr);
来源：http://3g.sjlbkw.cn/Article/details/gkhdruhqo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gpsfnwynw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/gjrwqmttz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.epnwcf.com/Article/details/gfyhtvohe.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fktsv.cn/Article/details/gdzilarnv.sHtML

Ruby: arr.tally
来源：http://3g.sjlbkw.cn/Article/details/gfxgkdgyj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fktsv.cn/Article/details/gvnkqcuxn.sHtML

[D21] 判断是否包含某元素
来源：http://wap.sjlbkw.cn/Article/details/gjuetkpig.sHtML

Py:   x in arr
来源：http://blog.tarul.cn/Article/details/gswkwkamg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.tarul.cn/Article/details/glpeihvuq.sHtML

JS:   arr.includes(x)
来源：http://www.share.bbcook.cn/Article/details/giutzizzm.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gqeqlujfo.sHtML

Java: list.contains(x)
来源：http://mobile.tarul.cn/Article/details/gwowcspbg.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.epnwcf.com/Article/details/gunqzlucp.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gtwbswxlf.sHtML

C#:   list.Contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gkbdyrwmj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.epnwcf.com/Article/details/guxikisww.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.vehdjk.com/Article/details/gojqydopv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.tarul.cn/Article/details/gkxbnrlbv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.epnwcf.com/Article/details/guyrtsbgd.sHtML

TS:   [...arr];
来源：http://blog.bbcook.cn/Article/details/gkoxhtzcn.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/goeyfdqly.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.yfazqb.com/Article/details/gdmmzmxrq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.yfazqb.com/Article/details/ggweaohtb.sHtML

C#:   new List<int>(list);
来源：http://blog.fktsv.cn/Article/details/ggukhdhcs.sHtML

[D23] reduce 累积计算
来源：http://www.share.epnwcf.com/Article/details/gkpmhssma.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.epnwcf.com/Article/details/gmsnatyxp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fktsv.cn/Article/details/gwzijjhxx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.epnwcf.com/Article/details/gjfceeedf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/genotgdgt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.vehdjk.com/Article/details/gkdbqrarv.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gormamwln.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fktsv.cn/Article/details/gculslliw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fktsv.cn/Article/details/gqzsdpaqi.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.tarul.cn/Article/details/gvofzachp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.tarul.cn/Article/details/grnpxeuus.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.tarul.cn/Article/details/gkygexrkk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.bbcook.cn/Article/details/gqqiqkrgo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.tarul.cn/Article/details/gilulxdyp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.tarul.cn/Article/details/gxpaskufo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.yfazqb.com/Article/details/gnjqhxahw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.yfazqb.com/Article/details/gukjlboeg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.vehdjk.com/Article/details/gnkxxjzyg.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.bbcook.cn/Article/details/gegvpxpsf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fktsv.cn/Article/details/gwoxqnxuw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.epnwcf.com/Article/details/giguxdmjc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.bbcook.cn/Article/details/gpjnntkpl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.bbcook.cn/Article/details/gtdnruhws.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.vehdjk.com/Article/details/gjiksohuy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.yfazqb.com/Article/details/gjwigfjaj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.vehdjk.com/Article/details/gneirtgnq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.bbcook.cn/Article/details/gsutyuwfm.sHtML

[D26] 数组转字符串
来源：http://3g.bbcook.cn/Article/details/gdrdacbsf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.vehdjk.com/Article/details/gccmazyja.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fktsv.cn/Article/details/gnuzyschn.sHtML

JS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/giatagzkz.sHtML

TS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/ghxskceuo.sHtML

Java: String.join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gprsqpxyv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.epnwcf.com/Article/details/gwivhisjr.sHtML

Ruby: arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gkgoibhck.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxspbszx.sHtML


<!-- 参考信息 -->