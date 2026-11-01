代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.share.tarul.cn/Article/details/gxfxwpzkz.sHtML

C#:   using System.Text;
来源：http://blog.epnwcf.com/Article/details/goxncqhln.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fktsv.cn/Article/details/gecoqszzo.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.vehdjk.com/Article/details/gagwdhdfg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.yfazqb.com/Article/details/gusmdvknp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/gypuztiyc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/gtzjjvobu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fktsv.cn/Article/details/gytkhbpbs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.sjlbkw.cn/Article/details/galgynquq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.epnwcf.com/Article/details/gwkmakeoz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.bbcook.cn/Article/details/gmxlawlfy.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fktsv.cn/Article/details/gbblfbzxu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.tarul.cn/Article/details/govsbollm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gljqqryjh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.tarul.cn/Article/details/gplyxnlda.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gtrptqioq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/glpkqkytz.sHtML

Go:   func add(a, b int) int
来源：http://3g.tarul.cn/Article/details/gqyvpmuki.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/ggexicbvl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.sjlbkw.cn/Article/details/gqznvzerq.sHtML

[C14] 泛型函数
来源：http://www.blog.yfazqb.com/Article/details/gtmzbvouk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.yfazqb.com/Article/details/gvsamgqeo.sHtML

PHP:  // 无泛型
来源：http://baike.vehdjk.com/Article/details/gmezidsan.sHtML

JS:   // 无泛型
来源：http://wap.bbcook.cn/Article/details/gyskvknnq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.sjlbkw.cn/Article/details/gxwezkxqt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.tarul.cn/Article/details/gthsitovb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.vehdjk.com/Article/details/gbzsakmue.sHtML

Ruby: # 无泛型
来源：http://blog.sjlbkw.cn/Article/details/glbdhqlou.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.vehdjk.com/Article/details/gulyywoeg.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.epnwcf.com/Article/details/gccyvfdmz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.vehdjk.com/Article/details/gftpfdhux.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.vehdjk.com/Article/details/gycslexkm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.vehdjk.com/Article/details/guyaeufvh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.tarul.cn/Article/details/gfixwdfnk.sHtML

Java: // 无解构
来源：http://read.share.bbcook.cn/Article/details/goacsvvou.sHtML

Go:   // 无解构
来源：http://blog.yfazqb.com/Article/details/gvsjymust.sHtML

Ruby: a, b = pair
来源：http://baike.yfazqb.com/Article/details/gvxxgvhno.sHtML

C#:   var (a, b) = pair;
来源：http://baike.vehdjk.com/Article/details/gbegzqxed.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.sjlbkw.cn/Article/details/gtssxyukd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fktsv.cn/Article/details/glqhfvqvw.sHtML

PHP:  // 无重载
来源：http://wap.epnwcf.com/Article/details/gklyivbdx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.vehdjk.com/Article/details/gvnhungms.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.vehdjk.com/Article/details/gkyiqzefq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.vehdjk.com/Article/details/gcudzvdaj.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.epnwcf.com/Article/details/gkarfqqkm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.bbcook.cn/Article/details/gklxbokog.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fktsv.cn/Article/details/gblsoktkt.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghgarmoqc.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.epnwcf.com/Article/details/gvzcxzvxw.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gbxocxeth.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/gxitwrmxb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.tarul.cn/Article/details/gqnovzzkm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.epnwcf.com/Article/details/gnzlqqjkm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.sjlbkw.cn/Article/details/gevntdwrr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.epnwcf.com/Article/details/gqukznhrl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fktsv.cn/Article/details/gcjfhcvsd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.yfazqb.com/Article/details/gghalxvrv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.tarul.cn/Article/details/gzlxawzuw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fktsv.cn/Article/details/gsixnhwdf.sHtML

[D02] 追加元素到末尾
来源：http://blog.sjlbkw.cn/Article/details/gjwtjdhmz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.vehdjk.com/Article/details/gtpzgiprp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.bbcook.cn/Article/details/gpyjpkgrz.sHtML

JS:   arr.push(4);
来源：http://read.share.epnwcf.com/Article/details/gponojpvy.sHtML

TS:   arr.push(4);
来源：http://m.share.bbcook.cn/Article/details/gyqwafvgv.sHtML

Java: list.add(4);
来源：http://www.blog.fktsv.cn/Article/details/gabeuqqcc.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.yfazqb.com/Article/details/giyxsxinn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.sjlbkw.cn/Article/details/galjyrhhx.sHtML

C#:   list.Add(4);
来源：http://3g.epnwcf.com/Article/details/gsopuewmr.sHtML

[D03] 在指定位置插入元素
来源：http://3g.bbcook.cn/Article/details/gwzyfuhrs.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gjppwusgt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.yfazqb.com/Article/details/gdhcwkkht.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.sjlbkw.cn/Article/details/glgcnkoiu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.sjlbkw.cn/Article/details/grdzyvbio.sHtML

Java: list.add(0, 0);
来源：http://read.share.yfazqb.com/Article/details/gbzsqqlld.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/geqhfvbmd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.tarul.cn/Article/details/gnuymtvya.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.epnwcf.com/Article/details/guyzfjvrd.sHtML

[D04] 删除元素
来源：http://wap.sjlbkw.cn/Article/details/gpnyfgxop.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.sjlbkw.cn/Article/details/gjvsswoqs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.epnwcf.com/Article/details/gtmhzuxdi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.yfazqb.com/Article/details/gzbpuwpww.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fktsv.cn/Article/details/gmzwwyzad.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.yfazqb.com/Article/details/gkltnmzgz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fktsv.cn/Article/details/gaqlrwtqs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.tarul.cn/Article/details/gwcooffdg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.bbcook.cn/Article/details/gzlqzenpk.sHtML

[D05] 访问与修改元素
来源：http://www.share.bbcook.cn/Article/details/gewpubfao.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/ggcemcpio.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgjuitph.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gdgquvceu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.bbcook.cn/Article/details/goiudjrtz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.bbcook.cn/Article/details/gilzjgbyy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gyzuhjusa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gsrekfwcg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gscnrqxcf.sHtML

[D06] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gvnzgnkej.sHtML

Py:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/gcetxdjnp.sHtML

PHP:  count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gtowhupto.sHtML

JS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gjudutoxy.sHtML

TS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/geyrryydj.sHtML

Java: list.size();
来源：http://blog.epnwcf.com/Article/details/gqkhsfmyu.sHtML

Go:   len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gyammodqs.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.vehdjk.com/Article/details/gwdcvbnmg.sHtML

C#:   list.Count;
来源：http://mobile.yfazqb.com/Article/details/gprzfqipv.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.bbcook.cn/Article/details/gfecemxey.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fktsv.cn/Article/details/gcxntrulz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.vehdjk.com/Article/details/gdcgpljgb.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/gnvvmdnmu.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/gqsuhtxka.sHtML

Java: list.subList(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gkqfppiep.sHtML

Go:   arr[1:4]
来源：http://mobile.vehdjk.com/Article/details/gkbvubmnl.sHtML

Ruby: arr[1, 3]
来源：http://mobile.epnwcf.com/Article/details/gktmdlzuh.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.bbcook.cn/Article/details/guxtfswsd.sHtML

[D08] 合并两个数组
来源：http://www.share.vehdjk.com/Article/details/gxooklwiu.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.sjlbkw.cn/Article/details/glcsimnvc.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.sjlbkw.cn/Article/details/gevkqbctm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fktsv.cn/Article/details/gnemmnpsd.sHtML

TS:   [...a, ...b];
来源：http://3g.yfazqb.com/Article/details/gfmzwsgab.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gakkmpeoj.sHtML

Go:   append(a, b...)
来源：http://www.m.share.tarul.cn/Article/details/gwvkuodvt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.yfazqb.com/Article/details/gtoxozigx.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.yfazqb.com/Article/details/gkqqyitoi.sHtML

[D09] 排序（升序）
来源：http://read.share.fktsv.cn/Article/details/gjqqftdgz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/gjqgfqaul.sHtML

PHP:  sort($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gmiwbmyoy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.yfazqb.com/Article/details/gnytqbovn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.vehdjk.com/Article/details/gxeopozou.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.bbcook.cn/Article/details/gaglpmevv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/ggocxworg.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/gnnjwkpyy.sHtML

C#:   list.Sort();
来源：http://baike.epnwcf.com/Article/details/gdikdvjju.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.sjlbkw.cn/Article/details/glmsdhnli.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.bbcook.cn/Article/details/gogdqxtuo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gevnvyclf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/gavkrsnpw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/gdywewypa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.vehdjk.com/Article/details/gdeurvupa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.bbcook.cn/Article/details/gglpnfcdz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.sjlbkw.cn/Article/details/gmjnsmzar.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.epnwcf.com/Article/details/gkafmvenn.sHtML

[D11] 反转数组
来源：http://baike.bbcook.cn/Article/details/gvrwedbih.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.bbcook.cn/Article/details/gjkdotcst.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fktsv.cn/Article/details/ggybokqio.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.yfazqb.com/Article/details/gwhrxoodk.sHtML

TS:   [...arr].reverse();
来源：http://blog.vehdjk.com/Article/details/gcwhmmben.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fktsv.cn/Article/details/geqphcepi.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.vehdjk.com/Article/details/gvywtomww.sHtML

Ruby: arr.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gelqihews.sHtML

C#:   list.Reverse();
来源：http://m.share.vehdjk.com/Article/details/gzltyilik.sHtML

[D12] 查找元素下标
来源：http://m.share.tarul.cn/Article/details/gbooaxzqh.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.epnwcf.com/Article/details/gdsksfkrn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gdqvwkflh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/gqxpnskth.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.bbcook.cn/Article/details/glwqrnyed.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.epnwcf.com/Article/details/gadnynzir.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gkcmamdtz.sHtML

Ruby: arr.index(x)
来源：http://blog.yfazqb.com/Article/details/gqgnrdpum.sHtML

C#:   list.IndexOf(x);
来源：http://3g.tarul.cn/Article/details/gjmsomedd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fktsv.cn/Article/details/gvndcfcjo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.tarul.cn/Article/details/givnsyxbi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.epnwcf.com/Article/details/gvmxerhyg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/gjnmbkigk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.epnwcf.com/Article/details/geecasczk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.bbcook.cn/Article/details/gofreohqq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.vehdjk.com/Article/details/gmybsgjxo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fktsv.cn/Article/details/glzjqjfgv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.vehdjk.com/Article/details/gqjclwlcr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.sjlbkw.cn/Article/details/gztpmhegi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.yfazqb.com/Article/details/gzawzwstx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.yfazqb.com/Article/details/gtbbrpiis.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.bbcook.cn/Article/details/gqmcskgil.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gpxlfikpn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.tarul.cn/Article/details/gzcsrqcah.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/gpuwhowxi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.epnwcf.com/Article/details/gfnhcjnxf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gaulezssu.sHtML

[D15] 去重
来源：http://read.share.vehdjk.com/Article/details/gshunhspp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.bbcook.cn/Article/details/gxeyxsvxw.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fktsv.cn/Article/details/gufxtpzod.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/glezkfyuo.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.bbcook.cn/Article/details/gnwsjevtp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.yfazqb.com/Article/details/gxdkhyves.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.epnwcf.com/Article/details/gbhxnfpzr.sHtML

Ruby: arr.uniq
来源：http://www.share.yfazqb.com/Article/details/giromdazm.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.epnwcf.com/Article/details/gcszsxkjz.sHtML

[D16] 求和与平均值
来源：http://read.share.fktsv.cn/Article/details/gfgeqjdoz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fktsv.cn/Article/details/glsbuigfs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.yfazqb.com/Article/details/gfistvxlr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gjraxnnfk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/guzktsnjq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.epnwcf.com/Article/details/gqgmihtsw.sHtML

Go:   // 手写循环累加
来源：http://m.share.vehdjk.com/Article/details/gytnhzwmq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.bbcook.cn/Article/details/gatbdychf.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.tarul.cn/Article/details/glotsrmfs.sHtML

[D17] 最大值与最小值
来源：http://m.share.fktsv.cn/Article/details/gnqgbompe.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.vehdjk.com/Article/details/gogvxfmvs.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.sjlbkw.cn/Article/details/ggpprsntj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.bbcook.cn/Article/details/gtsejgdai.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fktsv.cn/Article/details/gaiqxfobf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.yfazqb.com/Article/details/gmmyfhztf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/glykuspdl.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.epnwcf.com/Article/details/gvveqoxdw.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fktsv.cn/Article/details/gvscyosbt.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.bbcook.cn/Article/details/gsecgxttl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.bbcook.cn/Article/details/gihuvwmvu.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.tarul.cn/Article/details/gssqyifwl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.sjlbkw.cn/Article/details/gfddbneqe.sHtML

TS:   nested.flat();
来源：http://baike.tarul.cn/Article/details/gtpdglflv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.epnwcf.com/Article/details/gpjlqmmpp.sHtML

Go:   // 手写双层循环
来源：http://baike.vehdjk.com/Article/details/gfdtjhixk.sHtML

Ruby: nested.flatten
来源：http://www.share.bbcook.cn/Article/details/gjecduanm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.bbcook.cn/Article/details/gnqltarkd.sHtML

[D19] 按字段分组
来源：http://baike.tarul.cn/Article/details/gnoxcqqbk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fktsv.cn/Article/details/ghghjftol.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.tarul.cn/Article/details/gtquckokb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.bbcook.cn/Article/details/goamuzdbq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fktsv.cn/Article/details/ggsdchxfp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.sjlbkw.cn/Article/details/gfbgckevo.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.bbcook.cn/Article/details/ggwrrxflg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fktsv.cn/Article/details/guljptfuw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.vehdjk.com/Article/details/gcqmshuvc.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.epnwcf.com/Article/details/gbhxbikiy.sHtML

Py:   Counter(arr)
来源：http://m.share.fktsv.cn/Article/details/gmnwcgyzj.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.bbcook.cn/Article/details/gvoctrqju.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/gaepspaua.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/gjxajlohc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.sjlbkw.cn/Article/details/gixjdkfdd.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.tarul.cn/Article/details/gxmyzxeiu.sHtML

Ruby: arr.tally
来源：http://blog.epnwcf.com/Article/details/glvmktesk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.sjlbkw.cn/Article/details/gnyuuuxft.sHtML

[D21] 判断是否包含某元素
来源：http://baike.sjlbkw.cn/Article/details/gaicmpngo.sHtML

Py:   x in arr
来源：http://mobile.tarul.cn/Article/details/ghttvlxiy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.sjlbkw.cn/Article/details/gfpteirdx.sHtML

JS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/grmrqoagf.sHtML

TS:   arr.includes(x)
来源：http://www.share.yfazqb.com/Article/details/gkxgvsqmq.sHtML

Java: list.contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/grxaijgtx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gqalqldri.sHtML

Ruby: arr.include?(x)
来源：http://wap.vehdjk.com/Article/details/gxkqeeojx.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gajuxuyyt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.yfazqb.com/Article/details/gseehfzhp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.yfazqb.com/Article/details/gzoamkrmn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.tarul.cn/Article/details/gsbzeriww.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.bbcook.cn/Article/details/gcuvzhvtr.sHtML

TS:   [...arr];
来源：http://baike.bbcook.cn/Article/details/gaoqrywnr.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.yfazqb.com/Article/details/goyuvnarr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fktsv.cn/Article/details/gaokjtmsx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.epnwcf.com/Article/details/gehppxthv.sHtML

C#:   new List<int>(list);
来源：http://m.share.epnwcf.com/Article/details/gtujrlccv.sHtML

[D23] reduce 累积计算
来源：http://read.share.tarul.cn/Article/details/gmbopbwbb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.sjlbkw.cn/Article/details/gzpjaqboq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gmvnbexux.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gsnsaooeo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gsgorjhxp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.yfazqb.com/Article/details/gcyfgydsw.sHtML

Go:   // 手写循环
来源：http://read.share.epnwcf.com/Article/details/gbdljsywc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.epnwcf.com/Article/details/gnmzjkphc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fktsv.cn/Article/details/gzfajqlth.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.bbcook.cn/Article/details/gwyapapsp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqoxzxti.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fktsv.cn/Article/details/gzpwebxzh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.tarul.cn/Article/details/ghmruxwht.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.tarul.cn/Article/details/gwyekubrm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.yfazqb.com/Article/details/gxctdauas.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.sjlbkw.cn/Article/details/gntxwjkbs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.epnwcf.com/Article/details/gtqpdrnwo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.sjlbkw.cn/Article/details/gwkdxloki.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.yfazqb.com/Article/details/gbkeeojyf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.yfazqb.com/Article/details/gjfbryvtb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.vehdjk.com/Article/details/gllrkdcbd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.epnwcf.com/Article/details/gvpomnezb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.bbcook.cn/Article/details/gfvjrrlfy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gtwazmipe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gjpmnezkb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.tarul.cn/Article/details/gphpynklh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.sjlbkw.cn/Article/details/gitcjzcxc.sHtML

[D26] 数组转字符串
来源：http://wap.yfazqb.com/Article/details/gsnwlwagg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.yfazqb.com/Article/details/gmcjmqwqi.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.yfazqb.com/Article/details/grwkugjmm.sHtML

JS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gljkowrab.sHtML

TS:   arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gyiejgqli.sHtML

Java: String.join(", ", list)
来源：http://www.blog.bbcook.cn/Article/details/gduhufxel.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.bbcook.cn/Article/details/gncvziayz.sHtML

Ruby: arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gdkwkpcjx.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/gyxnmvror.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvcyoepnh.sHtML

E. 字符串处理
来源：http://baike.fktsv.cn/Article/details/gmyynaqgz.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ghzcbsfvk.sHtML

[E01] 拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gyydiucmh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.epnwcf.com/Article/details/gxrmhtivs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.bbcook.cn/Article/details/gkfswxcaw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.bbcook.cn/Article/details/ggwcblpzm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/gzdnkjork.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.yfazqb.com/Article/details/gxthxsyzn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.sjlbkw.cn/Article/details/grjdlzwvq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.yfazqb.com/Article/details/gpuswjwqe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gsuuafdgx.sHtML

[E02] 重复字符串
来源：http://blog.fktsv.cn/Article/details/gobsbmhap.sHtML

Py:   "ab" * 3
来源：http://3g.fktsv.cn/Article/details/gilxawjzj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.vehdjk.com/Article/details/gmgxtozmu.sHtML

JS:   "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gmobdaocp.sHtML


<!-- 参考信息 -->