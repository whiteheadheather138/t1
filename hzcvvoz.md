代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://read.share.vehdjk.com/Article/details/gfzzkbvlm.sHtML

C#:   using System.Text;
来源：http://blog.fktsv.cn/Article/details/gekkkuobx.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.bbcook.cn/Article/details/giswsorkc.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.epnwcf.com/Article/details/gtaabkqei.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.vehdjk.com/Article/details/gcrgefodb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/ghfotmgmt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/ghgyikefa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.yfazqb.com/Article/details/gouubkhpj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fktsv.cn/Article/details/geqsbwokr.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.epnwcf.com/Article/details/gsertonht.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.bbcook.cn/Article/details/gpbeexboh.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.bbcook.cn/Article/details/gatrwoemp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.bbcook.cn/Article/details/gdhqfwieq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gnqcehdpg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.vehdjk.com/Article/details/gajvovuie.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gfmedsjdh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gpknnwqjl.sHtML

Go:   func add(a, b int) int
来源：http://blog.sjlbkw.cn/Article/details/gosyteygy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.epnwcf.com/Article/details/gqatkqrqb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fktsv.cn/Article/details/gocrdcyms.sHtML

[C14] 泛型函数
来源：http://read.share.vehdjk.com/Article/details/ghcegbxud.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.tarul.cn/Article/details/gnmmjfzja.sHtML

PHP:  // 无泛型
来源：http://mobile.vehdjk.com/Article/details/gdoveagzf.sHtML

JS:   // 无泛型
来源：http://m.share.epnwcf.com/Article/details/ggmkvfhyl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.tarul.cn/Article/details/gjsgxwdzm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.bbcook.cn/Article/details/gkvwzgvbb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.vehdjk.com/Article/details/ggnokwcze.sHtML

Ruby: # 无泛型
来源：http://baike.tarul.cn/Article/details/gheotzmak.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.tarul.cn/Article/details/gwalvsivy.sHtML

[C15] 解构 / 展开参数
来源：http://3g.tarul.cn/Article/details/gitqdhzns.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fktsv.cn/Article/details/gcbhobvdy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.yfazqb.com/Article/details/gwxrgnwgn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/gniqumyta.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gjrqjdrot.sHtML

Java: // 无解构
来源：http://www.blog.vehdjk.com/Article/details/gadlrcypb.sHtML

Go:   // 无解构
来源：http://baike.fktsv.cn/Article/details/gnejpyuhc.sHtML

Ruby: a, b = pair
来源：http://3g.tarul.cn/Article/details/gahzfalse.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.vehdjk.com/Article/details/gxqiatbmm.sHtML

[C16] 函数 / 方法重载
来源：http://3g.yfazqb.com/Article/details/gkjseuyqr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.epnwcf.com/Article/details/giququoft.sHtML

PHP:  // 无重载
来源：http://blog.tarul.cn/Article/details/ggkstoghj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.yfazqb.com/Article/details/goylkupgy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.vehdjk.com/Article/details/giuzcjysa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fktsv.cn/Article/details/gqaycrkgm.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.yfazqb.com/Article/details/gkgepueam.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.vehdjk.com/Article/details/gpdqjpcck.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.yfazqb.com/Article/details/gtlbvjbls.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gezogtfjp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.yfazqb.com/Article/details/gkskqgwqr.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gkevoatgp.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.yfazqb.com/Article/details/gfpllricy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.bbcook.cn/Article/details/glweiqvlc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.tarul.cn/Article/details/gmwwlrtif.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.vehdjk.com/Article/details/gjvuppfoc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.epnwcf.com/Article/details/gyxaujndr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.vehdjk.com/Article/details/gjkafload.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhqtcujm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.vehdjk.com/Article/details/gvlllzzcj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.epnwcf.com/Article/details/gfakowvjg.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fktsv.cn/Article/details/gqcyazoma.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.sjlbkw.cn/Article/details/gbxcnsdwl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.epnwcf.com/Article/details/gryqvjuph.sHtML

JS:   arr.push(4);
来源：http://blog.epnwcf.com/Article/details/gmavmcbuw.sHtML

TS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gjzlranbo.sHtML

Java: list.add(4);
来源：http://3g.sjlbkw.cn/Article/details/gzbluulvg.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.vehdjk.com/Article/details/gfwfbszcj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fktsv.cn/Article/details/gwliwqcyj.sHtML

C#:   list.Add(4);
来源：http://blog.vehdjk.com/Article/details/gijqonthq.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.epnwcf.com/Article/details/gehpxigss.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.vehdjk.com/Article/details/gjpxxvlqp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fktsv.cn/Article/details/gqhfazjhe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.vehdjk.com/Article/details/gkazdefmq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.epnwcf.com/Article/details/gnilbuorj.sHtML

Java: list.add(0, 0);
来源：http://mobile.yfazqb.com/Article/details/govvjgcop.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.vehdjk.com/Article/details/gbqrupxst.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.tarul.cn/Article/details/ghyadqbol.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fktsv.cn/Article/details/gmsymqnao.sHtML

[D04] 删除元素
来源：http://baike.sjlbkw.cn/Article/details/gtiriisgf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.yfazqb.com/Article/details/gzgswtfnj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.bbcook.cn/Article/details/glqpaauzn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.tarul.cn/Article/details/gcnfyypin.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.vehdjk.com/Article/details/gndlopsgr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.sjlbkw.cn/Article/details/gfnaubwja.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.yfazqb.com/Article/details/gxnaypjpk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.yfazqb.com/Article/details/gmitiknny.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.yfazqb.com/Article/details/gyjephozc.sHtML

[D05] 访问与修改元素
来源：http://wap.tarul.cn/Article/details/gvbrzvrfl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gfvkdwcxs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gyeyogzap.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gkndhfpau.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.sjlbkw.cn/Article/details/gvlupxcag.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.sjlbkw.cn/Article/details/ghicjmycg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/ggwpevtge.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.vehdjk.com/Article/details/gxlboxxrk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.yfazqb.com/Article/details/gmpkyfxpw.sHtML

[D06] 数组长度
来源：http://3g.fktsv.cn/Article/details/gygabyglp.sHtML

Py:   len(arr)
来源：http://blog.epnwcf.com/Article/details/gcjxahzqc.sHtML

PHP:  count($arr);
来源：http://m.share.yfazqb.com/Article/details/gasgbetrv.sHtML

JS:   arr.length
来源：http://blog.yfazqb.com/Article/details/gkzvlinsa.sHtML

TS:   arr.length
来源：http://wap.epnwcf.com/Article/details/gcqeqwhyk.sHtML

Java: list.size();
来源：http://m.share.yfazqb.com/Article/details/gpdlqfsrl.sHtML

Go:   len(arr)
来源：http://wap.fktsv.cn/Article/details/glxyzsyqq.sHtML

Ruby: arr.length; arr.size
来源：http://baike.tarul.cn/Article/details/ghgdxgvpa.sHtML

C#:   list.Count;
来源：http://www.m.share.tarul.cn/Article/details/gosazlmry.sHtML

[D07] 切片 / 取子数组
来源：http://blog.epnwcf.com/Article/details/gmstimlxd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.sjlbkw.cn/Article/details/gqtxompqm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.tarul.cn/Article/details/gmdnnwkpr.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gsymxtkyd.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/gtlhluozk.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gccvlfzmq.sHtML

Go:   arr[1:4]
来源：http://read.share.tarul.cn/Article/details/gvbtocycl.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.epnwcf.com/Article/details/giyagjyqd.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gsnqrwcxa.sHtML

[D08] 合并两个数组
来源：http://www.m.share.epnwcf.com/Article/details/gjrvbjjjm.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.tarul.cn/Article/details/gerhoxkhr.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.sjlbkw.cn/Article/details/goofsnlpd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.bbcook.cn/Article/details/gmubxllek.sHtML

TS:   [...a, ...b];
来源：http://read.share.yfazqb.com/Article/details/gufiozscz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fktsv.cn/Article/details/gmiildaha.sHtML

Go:   append(a, b...)
来源：http://mobile.bbcook.cn/Article/details/gvlgplhcj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.sjlbkw.cn/Article/details/grrgzzfge.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.bbcook.cn/Article/details/gnijsaljq.sHtML

[D09] 排序（升序）
来源：http://m.share.epnwcf.com/Article/details/gtujweuem.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/giaochdjc.sHtML

PHP:  sort($arr);
来源：http://blog.vehdjk.com/Article/details/gdldtcarp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.vehdjk.com/Article/details/gpkiekoqw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.tarul.cn/Article/details/gkjqoxsjq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.epnwcf.com/Article/details/gowgqvrkd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.bbcook.cn/Article/details/ggewulaou.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gfhxkqsut.sHtML

C#:   list.Sort();
来源：http://mobile.tarul.cn/Article/details/gpkjqopck.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.tarul.cn/Article/details/guhmusmim.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.tarul.cn/Article/details/gkhtbkdap.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/gsqpzvqnz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.sjlbkw.cn/Article/details/gmttzrrlo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/ggtbxgffe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.vehdjk.com/Article/details/gbyrozvxi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.tarul.cn/Article/details/gfnngtohx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.sjlbkw.cn/Article/details/glerovaaz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.sjlbkw.cn/Article/details/guujbnhms.sHtML

[D11] 反转数组
来源：http://baike.fktsv.cn/Article/details/gdutufifw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.vehdjk.com/Article/details/gerpbxvto.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.bbcook.cn/Article/details/gyhduzliz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.bbcook.cn/Article/details/gyvviyruh.sHtML

TS:   [...arr].reverse();
来源：http://read.share.sjlbkw.cn/Article/details/gmvsqarja.sHtML

Java: Collections.reverse(list);
来源：http://www.share.sjlbkw.cn/Article/details/gdzmcbivu.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.vehdjk.com/Article/details/ggixydais.sHtML

Ruby: arr.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gmzoercvz.sHtML

C#:   list.Reverse();
来源：http://www.share.epnwcf.com/Article/details/gvbpyxgsk.sHtML

[D12] 查找元素下标
来源：http://blog.vehdjk.com/Article/details/grfkizbjs.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.yfazqb.com/Article/details/gedjrggzn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.tarul.cn/Article/details/gythvidej.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gdmcbgzog.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/gxxnqzhgo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.bbcook.cn/Article/details/gyfuoxzss.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/goxapobkm.sHtML

Ruby: arr.index(x)
来源：http://wap.tarul.cn/Article/details/gtbugvmqr.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.tarul.cn/Article/details/gznawkley.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.yfazqb.com/Article/details/gkzbsxzyb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.epnwcf.com/Article/details/gbnhfjtrl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.epnwcf.com/Article/details/grxxalymq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gpuzeobma.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gyssjvvtu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.bbcook.cn/Article/details/gpbqlikwp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.vehdjk.com/Article/details/gdrazixkj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.bbcook.cn/Article/details/gglwinlzu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.bbcook.cn/Article/details/gbwvmqelv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.tarul.cn/Article/details/gnkdueoyn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.sjlbkw.cn/Article/details/gzbrdiifd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fktsv.cn/Article/details/gxfznngmc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.bbcook.cn/Article/details/grwbxxmcw.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.yfazqb.com/Article/details/ggdirmums.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gzbroonti.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/gsekwjeax.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.epnwcf.com/Article/details/gboktbhhd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.tarul.cn/Article/details/gbtmunoee.sHtML

[D15] 去重
来源：http://m.share.tarul.cn/Article/details/gsurykukr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/gzpguymmv.sHtML

PHP:  array_unique($arr);
来源：http://read.share.epnwcf.com/Article/details/geaqjrjmi.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gmegofctz.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/gultizkpy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.bbcook.cn/Article/details/gdtmtgiob.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.vehdjk.com/Article/details/gfmupuwxf.sHtML

Ruby: arr.uniq
来源：http://m.share.epnwcf.com/Article/details/ggfhpwlzl.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.epnwcf.com/Article/details/gyvsxohrs.sHtML

[D16] 求和与平均值
来源：http://www.blog.vehdjk.com/Article/details/gxyhfaust.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gdmscgdlk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.epnwcf.com/Article/details/gqdqrvjaa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.bbcook.cn/Article/details/gdkmtokyl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gxikfqppv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.bbcook.cn/Article/details/gkzpxvkfe.sHtML

Go:   // 手写循环累加
来源：http://m.share.epnwcf.com/Article/details/gxbbrzghd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fktsv.cn/Article/details/gepipmctv.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fktsv.cn/Article/details/gektttocv.sHtML

[D17] 最大值与最小值
来源：http://m.share.sjlbkw.cn/Article/details/gqujlqpsw.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gqvjqwist.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.bbcook.cn/Article/details/glyaaomsd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fktsv.cn/Article/details/gswsveews.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fktsv.cn/Article/details/ggmrnjwqd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.tarul.cn/Article/details/glbutmasj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.yfazqb.com/Article/details/glztzqusr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.sjlbkw.cn/Article/details/gpufysdxc.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fktsv.cn/Article/details/gdymfscnj.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.bbcook.cn/Article/details/gpkoodpds.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.yfazqb.com/Article/details/gubrnxtoh.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.tarul.cn/Article/details/gcnxwxjme.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.yfazqb.com/Article/details/gvqjhofrs.sHtML

TS:   nested.flat();
来源：http://mobile.yfazqb.com/Article/details/gdqyfwjny.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.tarul.cn/Article/details/ggdmxhgnp.sHtML

Go:   // 手写双层循环
来源：http://read.share.bbcook.cn/Article/details/gviyhqtxc.sHtML

Ruby: nested.flatten
来源：http://blog.yfazqb.com/Article/details/grxvuygfs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.epnwcf.com/Article/details/gclkjixlm.sHtML

[D19] 按字段分组
来源：http://3g.fktsv.cn/Article/details/gmfnahsob.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.bbcook.cn/Article/details/gfmzpunnk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.tarul.cn/Article/details/gtnckvurb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.tarul.cn/Article/details/gfuqcfihu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/guocwxsqv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.sjlbkw.cn/Article/details/grhkvodbh.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.sjlbkw.cn/Article/details/ghbxrxiqo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.vehdjk.com/Article/details/gqaaqaegv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.tarul.cn/Article/details/gcauipxhv.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fktsv.cn/Article/details/gjdwaneir.sHtML

Py:   Counter(arr)
来源：http://www.blog.bbcook.cn/Article/details/gycpdyjvr.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.bbcook.cn/Article/details/grlykmzmq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gajedhrni.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/gpneutcmv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fktsv.cn/Article/details/gszxvoqoa.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.vehdjk.com/Article/details/gsislnpcr.sHtML

Ruby: arr.tally
来源：http://baike.fktsv.cn/Article/details/gykcoqlcw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.tarul.cn/Article/details/gjsoncbmu.sHtML

[D21] 判断是否包含某元素
来源：http://blog.bbcook.cn/Article/details/guyezrviw.sHtML

Py:   x in arr
来源：http://baike.fktsv.cn/Article/details/guyhgihes.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.epnwcf.com/Article/details/gfybyiczr.sHtML

JS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gtfwnmiaj.sHtML

TS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/goitmaams.sHtML

Java: list.contains(x)
来源：http://blog.fktsv.cn/Article/details/gmwwyrvjv.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.epnwcf.com/Article/details/glswljahv.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fktsv.cn/Article/details/gogqibftd.sHtML

C#:   list.Contains(x)
来源：http://baike.vehdjk.com/Article/details/gyuhiqsay.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fktsv.cn/Article/details/glifpmzqp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gilndtllc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.bbcook.cn/Article/details/gdfexiwva.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.tarul.cn/Article/details/grlexriof.sHtML

TS:   [...arr];
来源：http://blog.epnwcf.com/Article/details/gpjabnnwq.sHtML

Java: new ArrayList<>(list);
来源：http://blog.epnwcf.com/Article/details/guvevvklq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.epnwcf.com/Article/details/gkkjbueeh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.yfazqb.com/Article/details/gtebooios.sHtML

C#:   new List<int>(list);
来源：http://mobile.epnwcf.com/Article/details/gnmznlyfs.sHtML

[D23] reduce 累积计算
来源：http://blog.vehdjk.com/Article/details/gvjuyhzyg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.bbcook.cn/Article/details/gjqllzggi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.bbcook.cn/Article/details/gfxtegmbl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/gaoclglvs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/gallnvubf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.vehdjk.com/Article/details/gnsaxkbek.sHtML

Go:   // 手写循环
来源：http://3g.bbcook.cn/Article/details/gnksaepaf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.bbcook.cn/Article/details/gpyemnzod.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.epnwcf.com/Article/details/grnhfvdgd.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.tarul.cn/Article/details/gukvyefha.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.yfazqb.com/Article/details/gvhsxczbn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.tarul.cn/Article/details/giaxtwfbw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.epnwcf.com/Article/details/gfunvtipk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.yfazqb.com/Article/details/guqyzmkdy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.sjlbkw.cn/Article/details/guqtxdmxa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.sjlbkw.cn/Article/details/gizyfwqsp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.yfazqb.com/Article/details/gedrzfrrw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.sjlbkw.cn/Article/details/gwydsihbn.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.epnwcf.com/Article/details/gosekgkpu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.bbcook.cn/Article/details/grqdtmimd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.bbcook.cn/Article/details/gocsozden.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.epnwcf.com/Article/details/gtwpttypf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fktsv.cn/Article/details/gbavdghno.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.tarul.cn/Article/details/gasuozdwo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fktsv.cn/Article/details/gedcfpfzm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fktsv.cn/Article/details/gpjapndyl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fktsv.cn/Article/details/gzfnhakdp.sHtML

[D26] 数组转字符串
来源：http://wap.epnwcf.com/Article/details/gkctixzkc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.tarul.cn/Article/details/gylbrvleu.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.epnwcf.com/Article/details/gzojprhoa.sHtML

JS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gbqcronnd.sHtML

TS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/guvzwsswm.sHtML

Java: String.join(", ", list)
来源：http://wap.epnwcf.com/Article/details/gxpjxxwmz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.vehdjk.com/Article/details/ggtdcmvqw.sHtML

Ruby: arr.join(", ")
来源：http://blog.tarul.cn/Article/details/ghvbgivdm.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/ghkcffkft.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gbywcekgu.sHtML

E. 字符串处理
来源：http://www.share.epnwcf.com/Article/details/ghpwjfmsr.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gayeikrta.sHtML

[E01] 拼接字符串
来源：http://3g.yfazqb.com/Article/details/gfddjqvmj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fktsv.cn/Article/details/ghdzpazqo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.tarul.cn/Article/details/gxetjdgjx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.bbcook.cn/Article/details/guexgldob.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/gwofjuxis.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fktsv.cn/Article/details/gefsmkxrc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.vehdjk.com/Article/details/ggwjzjsys.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.epnwcf.com/Article/details/gwyaiezmh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.yfazqb.com/Article/details/getoxbjac.sHtML

[E02] 重复字符串
来源：http://read.share.fktsv.cn/Article/details/gvbnbbisr.sHtML

Py:   "ab" * 3
来源：http://www.share.epnwcf.com/Article/details/gpdizehbs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.sjlbkw.cn/Article/details/gcrqmvbgv.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gvtbhmkpg.sHtML


<!-- 参考信息 -->