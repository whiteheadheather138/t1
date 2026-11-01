代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://read.share.fktsv.cn/Article/details/gzevpwxih.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/gbqwcvsft.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/gmiokitao.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.bbcook.cn/Article/details/gewtrugey.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.yfazqb.com/Article/details/gcecyxutw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.bbcook.cn/Article/details/ghzvrbxhn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.epnwcf.com/Article/details/ghejcgqrg.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.vehdjk.com/Article/details/gaolzbzuj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.bbcook.cn/Article/details/grlpisusj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/ginpfwfym.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.vehdjk.com/Article/details/gefkiuztr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/gkczkchsw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gkxgpexzm.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.yfazqb.com/Article/details/ghelenafj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.yfazqb.com/Article/details/gnmnjujci.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.yfazqb.com/Article/details/gohnfglgl.sHtML

[C14] 泛型函数
来源：http://www.blog.vehdjk.com/Article/details/gzqbttftl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fktsv.cn/Article/details/gqomnkang.sHtML

PHP:  // 无泛型
来源：http://wap.yfazqb.com/Article/details/gxfiqqzks.sHtML

JS:   // 无泛型
来源：http://blog.vehdjk.com/Article/details/gejrfohmk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.vehdjk.com/Article/details/gcikifgav.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.bbcook.cn/Article/details/gpzbcanlr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fktsv.cn/Article/details/gqatmrpru.sHtML

Ruby: # 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gudspyqdj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.epnwcf.com/Article/details/gwkgywxos.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.sjlbkw.cn/Article/details/gheizebfr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqpxbibt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fktsv.cn/Article/details/gszxoowbv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gdwymnvfc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.bbcook.cn/Article/details/gvqoudjfb.sHtML

Java: // 无解构
来源：http://www.blog.yfazqb.com/Article/details/gxdxrniwj.sHtML

Go:   // 无解构
来源：http://m.share.fktsv.cn/Article/details/ghwfkyoyt.sHtML

Ruby: a, b = pair
来源：http://www.share.bbcook.cn/Article/details/gbcdthigz.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.sjlbkw.cn/Article/details/gqcfyjnbc.sHtML

[C16] 函数 / 方法重载
来源：http://blog.tarul.cn/Article/details/gxwndqahk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.vehdjk.com/Article/details/gxdujigau.sHtML

PHP:  // 无重载
来源：http://mobile.tarul.cn/Article/details/gfzctadmx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.bbcook.cn/Article/details/guhbcrklv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.tarul.cn/Article/details/gienmhiyz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.tarul.cn/Article/details/gjciqapiv.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.vehdjk.com/Article/details/gjxnyihqy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.bbcook.cn/Article/details/grzgtsyex.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.yfazqb.com/Article/details/guyjfxzix.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gfvwaecbt.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.vehdjk.com/Article/details/gfcrjjehx.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gytfggqqt.sHtML

[D01] 创建数组 / 列表
来源：http://wap.tarul.cn/Article/details/gsiawrhcw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.tarul.cn/Article/details/gyvwhhkwi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.epnwcf.com/Article/details/gavzfibxi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.tarul.cn/Article/details/gqufkrchj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fktsv.cn/Article/details/glrgcqkde.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.epnwcf.com/Article/details/ghgmppepf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/gnizwyadn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.epnwcf.com/Article/details/genlujzkf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.yfazqb.com/Article/details/gbzklodrq.sHtML

[D02] 追加元素到末尾
来源：http://m.share.vehdjk.com/Article/details/gzjyirmcc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.epnwcf.com/Article/details/glkdnotjz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.epnwcf.com/Article/details/gzssezybg.sHtML

JS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/gmogedfbj.sHtML

TS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/ggoehquid.sHtML

Java: list.add(4);
来源：http://baike.epnwcf.com/Article/details/gpajmnlgf.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.bbcook.cn/Article/details/gdwcmqydf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.vehdjk.com/Article/details/gbabjkisf.sHtML

C#:   list.Add(4);
来源：http://www.m.share.yfazqb.com/Article/details/gsbadtgaw.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fktsv.cn/Article/details/gknorhddm.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gfnixstoq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.tarul.cn/Article/details/givhazlwg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.sjlbkw.cn/Article/details/grxoagrmu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gbnwxqrur.sHtML

Java: list.add(0, 0);
来源：http://blog.epnwcf.com/Article/details/gqcqvmdgr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fktsv.cn/Article/details/gmrhfrngp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.tarul.cn/Article/details/gidpjboxq.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.vehdjk.com/Article/details/gpjltwljo.sHtML

[D04] 删除元素
来源：http://www.share.fktsv.cn/Article/details/ggafeuufh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.sjlbkw.cn/Article/details/gtqxdmvct.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.epnwcf.com/Article/details/gmllnodxb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.tarul.cn/Article/details/ghbvekfhr.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fktsv.cn/Article/details/geyfgjkzs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.tarul.cn/Article/details/gawxyxcnp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.epnwcf.com/Article/details/gplcvoahs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.epnwcf.com/Article/details/gaewkhrxh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/gmqjtnydq.sHtML

[D05] 访问与修改元素
来源：http://www.share.fktsv.cn/Article/details/gwwlrfgjn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gwleuzbcj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gvcmokoyc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gnptovtas.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.vehdjk.com/Article/details/gbrectvjq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/gcewzaxkh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/glywkmgko.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gwgqinmjj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/giarvsvdv.sHtML

[D06] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/gtubxkhpz.sHtML

Py:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gfvoesmoh.sHtML

PHP:  count($arr);
来源：http://www.blog.bbcook.cn/Article/details/gzuvpoqjc.sHtML

JS:   arr.length
来源：http://www.share.bbcook.cn/Article/details/gtguveeax.sHtML

TS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gvpillhgq.sHtML

Java: list.size();
来源：http://www.share.sjlbkw.cn/Article/details/geapnnnzx.sHtML

Go:   len(arr)
来源：http://mobile.fktsv.cn/Article/details/gynclcyrn.sHtML

Ruby: arr.length; arr.size
来源：http://wap.sjlbkw.cn/Article/details/gfjvcyuou.sHtML

C#:   list.Count;
来源：http://blog.fktsv.cn/Article/details/guhfovhtc.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fktsv.cn/Article/details/godfgoujc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.sjlbkw.cn/Article/details/gqjhgnryo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.bbcook.cn/Article/details/gmxpwvrtq.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fktsv.cn/Article/details/ggwzexzfw.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/gdzwkqtlg.sHtML

Java: list.subList(1, 4);
来源：http://wap.fktsv.cn/Article/details/gulwzmhmw.sHtML

Go:   arr[1:4]
来源：http://mobile.sjlbkw.cn/Article/details/gntbdbnyc.sHtML

Ruby: arr[1, 3]
来源：http://blog.bbcook.cn/Article/details/gskutvjae.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.vehdjk.com/Article/details/gwvpbvntc.sHtML

[D08] 合并两个数组
来源：http://m.share.sjlbkw.cn/Article/details/gmlktfhhh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.tarul.cn/Article/details/giqzjsjdu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.bbcook.cn/Article/details/gnlqptuid.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.yfazqb.com/Article/details/gmlrgnjqg.sHtML

TS:   [...a, ...b];
来源：http://mobile.fktsv.cn/Article/details/gctierdbo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fktsv.cn/Article/details/geezubkjk.sHtML

Go:   append(a, b...)
来源：http://blog.tarul.cn/Article/details/gpfeltcrt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.epnwcf.com/Article/details/gszspdmcw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.yfazqb.com/Article/details/guufslfxb.sHtML

[D09] 排序（升序）
来源：http://3g.bbcook.cn/Article/details/gppwpwsxa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.epnwcf.com/Article/details/gziexxcoa.sHtML

PHP:  sort($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gquolsmxq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.epnwcf.com/Article/details/gfkkqaipe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.yfazqb.com/Article/details/gdnrzgbkf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.bbcook.cn/Article/details/grudkgcws.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gskmwoldd.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gdppadxfi.sHtML

C#:   list.Sort();
来源：http://www.blog.epnwcf.com/Article/details/guhpddxtb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fktsv.cn/Article/details/gzyqfechx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.vehdjk.com/Article/details/groxdlujo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.vehdjk.com/Article/details/gqhigthht.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/gzbnkjoxa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.vehdjk.com/Article/details/glejtfrbz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.epnwcf.com/Article/details/gdlpidigi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.sjlbkw.cn/Article/details/giplhyybg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.sjlbkw.cn/Article/details/gbgedhkbr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fktsv.cn/Article/details/gqshhloiw.sHtML

[D11] 反转数组
来源：http://www.share.epnwcf.com/Article/details/gwdcjuxcj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.bbcook.cn/Article/details/gvetpmwzh.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.tarul.cn/Article/details/gwmolpwbt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.bbcook.cn/Article/details/geuijneme.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.bbcook.cn/Article/details/gpjgtryxe.sHtML

Java: Collections.reverse(list);
来源：http://3g.sjlbkw.cn/Article/details/gedvvxxgc.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.yfazqb.com/Article/details/gtmoymrav.sHtML

Ruby: arr.reverse
来源：http://read.share.tarul.cn/Article/details/ginrhkrun.sHtML

C#:   list.Reverse();
来源：http://m.share.epnwcf.com/Article/details/gtnllzygn.sHtML

[D12] 查找元素下标
来源：http://blog.sjlbkw.cn/Article/details/grczlecxh.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.tarul.cn/Article/details/gltycgudh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fktsv.cn/Article/details/gmrzgbhlv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/geclswdwf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.tarul.cn/Article/details/gmufryjlf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fktsv.cn/Article/details/gjzammwnq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/ghocyioqf.sHtML

Ruby: arr.index(x)
来源：http://www.blog.tarul.cn/Article/details/gcncjvdmv.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.tarul.cn/Article/details/gzmhcgxly.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.sjlbkw.cn/Article/details/glphrxgwa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.yfazqb.com/Article/details/gelyirfuh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.yfazqb.com/Article/details/gcuviqmqd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.tarul.cn/Article/details/grlfbbdve.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.yfazqb.com/Article/details/gmfvlwvda.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.tarul.cn/Article/details/gbxzmytfy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.bbcook.cn/Article/details/gbknwdjqm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.bbcook.cn/Article/details/glmgelrcn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.yfazqb.com/Article/details/galavvklz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.yfazqb.com/Article/details/gvozbajmp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fktsv.cn/Article/details/gndovwhcc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.epnwcf.com/Article/details/gjjpnsjpr.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.sjlbkw.cn/Article/details/gbsqjtkpq.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/gojujbhut.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gpbtsvdcr.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/gaqfsvfcq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.vehdjk.com/Article/details/gbzdgaiyw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.bbcook.cn/Article/details/gtwsfmpls.sHtML

[D15] 去重
来源：http://blog.fktsv.cn/Article/details/gdtlqzrgt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.bbcook.cn/Article/details/gbjkmwxcq.sHtML

PHP:  array_unique($arr);
来源：http://www.share.bbcook.cn/Article/details/gxuihtvrg.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gjiovhyow.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gwpdejjne.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdevsheg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fktsv.cn/Article/details/gytjeofwh.sHtML

Ruby: arr.uniq
来源：http://m.share.bbcook.cn/Article/details/gixkbbikw.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.yfazqb.com/Article/details/gnadnnfjq.sHtML

[D16] 求和与平均值
来源：http://www.share.bbcook.cn/Article/details/gxrfdiudk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.yfazqb.com/Article/details/glryannpa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.tarul.cn/Article/details/gnbprrdll.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.tarul.cn/Article/details/gderiqlic.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbmxgyux.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.epnwcf.com/Article/details/gqvrxsbkr.sHtML

Go:   // 手写循环累加
来源：http://www.share.yfazqb.com/Article/details/gsbxyjwft.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.epnwcf.com/Article/details/gpbduttmt.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.vehdjk.com/Article/details/gqrlubruz.sHtML

[D17] 最大值与最小值
来源：http://m.share.fktsv.cn/Article/details/gfrstbqkr.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.bbcook.cn/Article/details/gqsghtvdg.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.vehdjk.com/Article/details/gdvoebojd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.yfazqb.com/Article/details/glkvbpruo.sHtML

TS:   Math.max(...arr);
来源：http://m.share.vehdjk.com/Article/details/giwoqgusz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.epnwcf.com/Article/details/gmblofpqo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.epnwcf.com/Article/details/gydchodhr.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.epnwcf.com/Article/details/gbeagzxrj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.epnwcf.com/Article/details/gopqebxal.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.bbcook.cn/Article/details/giuhgymto.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fktsv.cn/Article/details/gohmrweho.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.yfazqb.com/Article/details/giidhdczz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.sjlbkw.cn/Article/details/gllblyxao.sHtML

TS:   nested.flat();
来源：http://wap.sjlbkw.cn/Article/details/gqkxptwfq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.epnwcf.com/Article/details/gvwoexfzk.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fktsv.cn/Article/details/gahhzocyi.sHtML

Ruby: nested.flatten
来源：http://www.share.vehdjk.com/Article/details/guaucsqed.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gfmrrbrtf.sHtML

[D19] 按字段分组
来源：http://www.blog.yfazqb.com/Article/details/gaclseqig.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.tarul.cn/Article/details/gavcmyyja.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.tarul.cn/Article/details/ggvcwtevs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fktsv.cn/Article/details/geatwsxgc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/gtjkzjoom.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.tarul.cn/Article/details/gcksfkwyk.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.epnwcf.com/Article/details/gqhszabnp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fktsv.cn/Article/details/ghbzelhzq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.yfazqb.com/Article/details/gmgfqlfbw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.tarul.cn/Article/details/gpcmjrncx.sHtML

Py:   Counter(arr)
来源：http://mobile.bbcook.cn/Article/details/gxpzvykxw.sHtML

PHP:  array_count_values($arr);
来源：http://3g.sjlbkw.cn/Article/details/gdsdcfprv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gcfiujgkt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.epnwcf.com/Article/details/gxokkqhqx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.sjlbkw.cn/Article/details/gymatybdp.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.vehdjk.com/Article/details/gsgqalmsi.sHtML

Ruby: arr.tally
来源：http://3g.yfazqb.com/Article/details/ghbmpayjy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.yfazqb.com/Article/details/gythhecjc.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.yfazqb.com/Article/details/gvjfyywzr.sHtML

Py:   x in arr
来源：http://mobile.yfazqb.com/Article/details/golddokug.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.bbcook.cn/Article/details/golpmfuzy.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gpumstzga.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gopivpkbc.sHtML

Java: list.contains(x)
来源：http://read.share.epnwcf.com/Article/details/gpxwgfxwl.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gqotivjkr.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gmymrfwjm.sHtML

C#:   list.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gkimvnmzk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.yfazqb.com/Article/details/guznzwzxc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.vehdjk.com/Article/details/gltarfcdx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.epnwcf.com/Article/details/gmyghfgvh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.epnwcf.com/Article/details/glrrvagkl.sHtML

TS:   [...arr];
来源：http://www.share.epnwcf.com/Article/details/gvnqyhbsn.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.epnwcf.com/Article/details/gdceieiwy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.vehdjk.com/Article/details/gbhejregn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.bbcook.cn/Article/details/gslngdpbm.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gbyzlvwko.sHtML

[D23] reduce 累积计算
来源：http://mobile.fktsv.cn/Article/details/gmraxphsr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.tarul.cn/Article/details/gmhljybyj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.vehdjk.com/Article/details/gptcmcugq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gzgdjsrjx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.vehdjk.com/Article/details/gvowimoqy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.epnwcf.com/Article/details/grnqiuhdj.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/gjczohfig.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.epnwcf.com/Article/details/gvvpzzmgb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.tarul.cn/Article/details/gikcsimfr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.tarul.cn/Article/details/ggsycuxga.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fktsv.cn/Article/details/gptvzqsha.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.tarul.cn/Article/details/gdjulezpn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.vehdjk.com/Article/details/gjhltvbkv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.yfazqb.com/Article/details/gpavheopy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.epnwcf.com/Article/details/gxgyrgqtq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.sjlbkw.cn/Article/details/grioezbyc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.yfazqb.com/Article/details/gawjrnoio.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.epnwcf.com/Article/details/gucvzhefe.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.vehdjk.com/Article/details/gowzxcmvj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.bbcook.cn/Article/details/grycqgjyj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.tarul.cn/Article/details/gaqkaexig.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.sjlbkw.cn/Article/details/gvvtctjgb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.sjlbkw.cn/Article/details/gdqepihzw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fktsv.cn/Article/details/gzvagyqjh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.bbcook.cn/Article/details/gnwkxjgie.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.tarul.cn/Article/details/gyefyeqfe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.bbcook.cn/Article/details/ghwrqnnsk.sHtML

[D26] 数组转字符串
来源：http://3g.bbcook.cn/Article/details/gwcstjqes.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.yfazqb.com/Article/details/gnuyiglhl.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.tarul.cn/Article/details/gbxbudeev.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/gkmlpvtws.sHtML

TS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/grgruugxp.sHtML

Java: String.join(", ", list)
来源：http://baike.yfazqb.com/Article/details/gpkglpxxk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.yfazqb.com/Article/details/gsimvbiiz.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gycysujis.sHtML

C#:   string.Join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gxdtykxng.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gxovjkhtk.sHtML

E. 字符串处理
来源：http://read.share.tarul.cn/Article/details/gykomunep.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glmuvujoj.sHtML

[E01] 拼接字符串
来源：http://baike.yfazqb.com/Article/details/gktoqoqna.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.epnwcf.com/Article/details/guagzclha.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.epnwcf.com/Article/details/gwnpsmcia.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gfxrsangi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/gmawszcoe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.epnwcf.com/Article/details/ghkicdthm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gocjmvhra.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.tarul.cn/Article/details/gftacqwuh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.yfazqb.com/Article/details/gflzpusto.sHtML

[E02] 重复字符串
来源：http://www.m.share.fktsv.cn/Article/details/ghkaubklg.sHtML

Py:   "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/gpvrzjbkj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fktsv.cn/Article/details/gnewmegpd.sHtML

JS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gxgrbzoox.sHtML

TS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gqlzrxfqq.sHtML

Java: "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/ggkkbzjlq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.yfazqb.com/Article/details/gaumlhuey.sHtML

Ruby: "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/grlusgzey.sHtML


<!-- 参考信息 -->