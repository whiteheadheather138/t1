代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://m.share.epnwcf.com/Article/details/gvgscijlq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.bbcook.cn/Article/details/gkerlwpjt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.vehdjk.com/Article/details/gkvfsiwky.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.sjlbkw.cn/Article/details/gqynggeco.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.epnwcf.com/Article/details/gumfjygdt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gsczqtyec.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.bbcook.cn/Article/details/gtpzztszu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/ggzwvdghs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gepayvgde.sHtML

Go:   func add(a, b int) int
来源：http://3g.epnwcf.com/Article/details/ggvwzpmpz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fktsv.cn/Article/details/gvppzogzs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.epnwcf.com/Article/details/gvaoitvzv.sHtML

[C14] 泛型函数
来源：http://www.blog.tarul.cn/Article/details/gtkidtaqc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.tarul.cn/Article/details/gmjnjzude.sHtML

PHP:  // 无泛型
来源：http://3g.bbcook.cn/Article/details/gmxkoufvh.sHtML

JS:   // 无泛型
来源：http://blog.vehdjk.com/Article/details/gfgntterb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.bbcook.cn/Article/details/ggybrjnwv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.yfazqb.com/Article/details/gbudtqwbz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.bbcook.cn/Article/details/gyrixyawk.sHtML

Ruby: # 无泛型
来源：http://3g.yfazqb.com/Article/details/guwdxdhky.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.sjlbkw.cn/Article/details/gdaxsrrdm.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fktsv.cn/Article/details/gjeqnassm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.epnwcf.com/Article/details/gwrxsfliu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.tarul.cn/Article/details/gekhnmkmh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.bbcook.cn/Article/details/glltbapvm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.tarul.cn/Article/details/gsmgpqlor.sHtML

Java: // 无解构
来源：http://wap.yfazqb.com/Article/details/gcpasksyz.sHtML

Go:   // 无解构
来源：http://read.share.epnwcf.com/Article/details/gsrdzzcqk.sHtML

Ruby: a, b = pair
来源：http://read.share.vehdjk.com/Article/details/gtyyktnhs.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fktsv.cn/Article/details/ggogyagzz.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.tarul.cn/Article/details/gvndczjtw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.vehdjk.com/Article/details/gtcllyixg.sHtML

PHP:  // 无重载
来源：http://read.share.epnwcf.com/Article/details/gobvhoujh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.sjlbkw.cn/Article/details/gaqcoolrd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.tarul.cn/Article/details/glyjgxfrj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.tarul.cn/Article/details/gqyfvzgfz.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.vehdjk.com/Article/details/grlskuqsm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.sjlbkw.cn/Article/details/gdvfkvfij.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.epnwcf.com/Article/details/gkumcjqkf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gsxemdbqc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.sjlbkw.cn/Article/details/gmeljlrzd.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gjxzryahh.sHtML

[D01] 创建数组 / 列表
来源：http://blog.yfazqb.com/Article/details/gzgupemkm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.vehdjk.com/Article/details/gxedhbsow.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.tarul.cn/Article/details/gtlmjirrn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fktsv.cn/Article/details/gnhhtwtmn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.vehdjk.com/Article/details/gugblwbna.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.yfazqb.com/Article/details/gyvtaiinm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.sjlbkw.cn/Article/details/gnvadujuy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.yfazqb.com/Article/details/glpcacvrh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.tarul.cn/Article/details/gfztrxsaa.sHtML

[D02] 追加元素到末尾
来源：http://www.share.vehdjk.com/Article/details/gwfdvgjxs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.yfazqb.com/Article/details/garmriued.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.bbcook.cn/Article/details/ggmciccwv.sHtML

JS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/grhvzvbyd.sHtML

TS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/gkwfpdzut.sHtML

Java: list.add(4);
来源：http://www.blog.epnwcf.com/Article/details/gfwbfypeg.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.bbcook.cn/Article/details/gdwnrafxl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.tarul.cn/Article/details/gzhvkizur.sHtML

C#:   list.Add(4);
来源：http://baike.fktsv.cn/Article/details/gsvdewmzf.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.yfazqb.com/Article/details/govdhpygq.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.vehdjk.com/Article/details/gkjjmscju.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.tarul.cn/Article/details/gblfspill.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.sjlbkw.cn/Article/details/gfsnwltdm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.bbcook.cn/Article/details/goqetjsbv.sHtML

Java: list.add(0, 0);
来源：http://mobile.bbcook.cn/Article/details/ghjabmpyt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.bbcook.cn/Article/details/gdkjjnsna.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.yfazqb.com/Article/details/gkiddsdep.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gumssqdxt.sHtML

[D04] 删除元素
来源：http://www.m.share.yfazqb.com/Article/details/geddwcmtm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.vehdjk.com/Article/details/gsahhzuyd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.tarul.cn/Article/details/gqdhpyjjh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.vehdjk.com/Article/details/gqusvhume.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.bbcook.cn/Article/details/gbaofncmp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.vehdjk.com/Article/details/guinmkuha.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.bbcook.cn/Article/details/gcczfzdke.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fktsv.cn/Article/details/gljvjklwl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.yfazqb.com/Article/details/ggwpmttby.sHtML

[D05] 访问与修改元素
来源：http://m.share.sjlbkw.cn/Article/details/ggrmxcfvc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gmzlxfyzu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjjsjfvq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gtzhwknhj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.vehdjk.com/Article/details/geslegerf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.yfazqb.com/Article/details/gvbslfeag.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gdkvziwkx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gyhfiapja.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gsyvrefth.sHtML

[D06] 数组长度
来源：http://blog.epnwcf.com/Article/details/gmgpynsgd.sHtML

Py:   len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gwzdffrsq.sHtML

PHP:  count($arr);
来源：http://baike.sjlbkw.cn/Article/details/gooqoytjn.sHtML

JS:   arr.length
来源：http://www.m.share.sjlbkw.cn/Article/details/geefdgnjk.sHtML

TS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gpnkgteha.sHtML

Java: list.size();
来源：http://www.m.share.yfazqb.com/Article/details/gtxrzziom.sHtML

Go:   len(arr)
来源：http://baike.yfazqb.com/Article/details/gewxenyas.sHtML

Ruby: arr.length; arr.size
来源：http://wap.yfazqb.com/Article/details/geecjtmqg.sHtML

C#:   list.Count;
来源：http://www.m.share.vehdjk.com/Article/details/grhkimjtk.sHtML

[D07] 切片 / 取子数组
来源：http://3g.sjlbkw.cn/Article/details/gichlllil.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.vehdjk.com/Article/details/gjmlqvygk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.vehdjk.com/Article/details/gmdlipaxf.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/gdatwvkhc.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gfyqjesyx.sHtML

Java: list.subList(1, 4);
来源：http://baike.epnwcf.com/Article/details/gixcigaph.sHtML

Go:   arr[1:4]
来源：http://www.share.sjlbkw.cn/Article/details/gjzpjxmne.sHtML

Ruby: arr[1, 3]
来源：http://blog.fktsv.cn/Article/details/gisicecsl.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gnqngwtyc.sHtML

[D08] 合并两个数组
来源：http://read.share.epnwcf.com/Article/details/guclbutzr.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.bbcook.cn/Article/details/grdpkehqg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.bbcook.cn/Article/details/giloonqhw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.vehdjk.com/Article/details/gzedfarkr.sHtML

TS:   [...a, ...b];
来源：http://mobile.yfazqb.com/Article/details/gmfipkhma.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.vehdjk.com/Article/details/gjsrflepl.sHtML

Go:   append(a, b...)
来源：http://baike.epnwcf.com/Article/details/gfxsmwggs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.tarul.cn/Article/details/gxftedwtc.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gnqhecjih.sHtML

[D09] 排序（升序）
来源：http://m.share.epnwcf.com/Article/details/gmejovozt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/gjuqigkhu.sHtML

PHP:  sort($arr);
来源：http://www.blog.bbcook.cn/Article/details/gskuacxmy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.yfazqb.com/Article/details/gnvrutcql.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.sjlbkw.cn/Article/details/gxpvcijje.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.bbcook.cn/Article/details/goyhlcjyq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gnfkdtcpk.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/getkrcjtg.sHtML

C#:   list.Sort();
来源：http://www.blog.sjlbkw.cn/Article/details/gjppfkder.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.tarul.cn/Article/details/gcgpqxspe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.vehdjk.com/Article/details/gcnuwhbai.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fktsv.cn/Article/details/gjlkdoswx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.bbcook.cn/Article/details/gqrtxpjwm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.sjlbkw.cn/Article/details/gmvwljqcb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.bbcook.cn/Article/details/gpokqlhrq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.sjlbkw.cn/Article/details/ggyygiidd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fktsv.cn/Article/details/gnhvlsvwe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.tarul.cn/Article/details/gqtforzza.sHtML

[D11] 反转数组
来源：http://baike.vehdjk.com/Article/details/ghhyokcrw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fktsv.cn/Article/details/gvqrdzigg.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fktsv.cn/Article/details/gzlilcwoe.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.vehdjk.com/Article/details/gyeijguwa.sHtML

TS:   [...arr].reverse();
来源：http://read.share.epnwcf.com/Article/details/guhtnkdee.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.yfazqb.com/Article/details/gcimroykj.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.tarul.cn/Article/details/gskrvmjos.sHtML

Ruby: arr.reverse
来源：http://mobile.vehdjk.com/Article/details/gfxpezbvi.sHtML

C#:   list.Reverse();
来源：http://m.share.yfazqb.com/Article/details/gqnsdyvcb.sHtML

[D12] 查找元素下标
来源：http://wap.fktsv.cn/Article/details/gzruidalj.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.sjlbkw.cn/Article/details/gujfqbarn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.yfazqb.com/Article/details/gputfxvdn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.epnwcf.com/Article/details/gyicklras.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/gbkmwppun.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.sjlbkw.cn/Article/details/guwrzrvir.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gjnhmdztz.sHtML

Ruby: arr.index(x)
来源：http://blog.sjlbkw.cn/Article/details/gxtbbzewu.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fktsv.cn/Article/details/gqxcrmkyb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.vehdjk.com/Article/details/gogmgncla.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.sjlbkw.cn/Article/details/giwxipfcq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fktsv.cn/Article/details/gyzkiztuj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.vehdjk.com/Article/details/gwryooqyk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/gfxvffldg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gvxowdrrw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.yfazqb.com/Article/details/gyjlfshex.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.yfazqb.com/Article/details/gyijgnxbe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.bbcook.cn/Article/details/gndieijln.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fktsv.cn/Article/details/gxvnoepuv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.bbcook.cn/Article/details/gexymfktx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.vehdjk.com/Article/details/gvxuujqbd.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.yfazqb.com/Article/details/ggcogylum.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.yfazqb.com/Article/details/giqnmzsno.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.tarul.cn/Article/details/gcrythoag.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gqafrmqwx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.yfazqb.com/Article/details/gunerjcgi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fktsv.cn/Article/details/gvshyvtmr.sHtML

[D15] 去重
来源：http://blog.sjlbkw.cn/Article/details/gapqnwpuz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.tarul.cn/Article/details/gdsdqymre.sHtML

PHP:  array_unique($arr);
来源：http://www.share.sjlbkw.cn/Article/details/grhllevlz.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gvnwbnjgz.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gjhylsntp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.tarul.cn/Article/details/gszdlwjbk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.bbcook.cn/Article/details/gkqzlreml.sHtML

Ruby: arr.uniq
来源：http://read.share.epnwcf.com/Article/details/gimqcibrs.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.epnwcf.com/Article/details/gpyrzmqnf.sHtML

[D16] 求和与平均值
来源：http://www.m.share.epnwcf.com/Article/details/gwqmuwlgv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gadlwsuwz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.tarul.cn/Article/details/gnqxzrvaa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.epnwcf.com/Article/details/ggfnunyfy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/glgvelmkm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fktsv.cn/Article/details/gfhgqpafm.sHtML

Go:   // 手写循环累加
来源：http://mobile.fktsv.cn/Article/details/gjizyleak.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.epnwcf.com/Article/details/gyaucgpgq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.epnwcf.com/Article/details/gtdechnrr.sHtML

[D17] 最大值与最小值
来源：http://wap.tarul.cn/Article/details/gattaggkt.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.vehdjk.com/Article/details/gmawzjgeh.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.epnwcf.com/Article/details/gtmzdwlan.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.vehdjk.com/Article/details/gxhbbmzhf.sHtML

TS:   Math.max(...arr);
来源：http://3g.sjlbkw.cn/Article/details/gxaknehvs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.epnwcf.com/Article/details/gjtmsodar.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.vehdjk.com/Article/details/geqdaoheo.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.sjlbkw.cn/Article/details/grtoavpmz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.yfazqb.com/Article/details/gdsntdwfu.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.yfazqb.com/Article/details/ggbgxqzap.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.yfazqb.com/Article/details/gbanvbogu.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.tarul.cn/Article/details/gibpqlakc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.vehdjk.com/Article/details/gxrfudbqj.sHtML

TS:   nested.flat();
来源：http://read.share.vehdjk.com/Article/details/gnvlnwhxj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.sjlbkw.cn/Article/details/gyewrfeld.sHtML

Go:   // 手写双层循环
来源：http://www.share.tarul.cn/Article/details/gxquemetq.sHtML

Ruby: nested.flatten
来源：http://www.m.share.vehdjk.com/Article/details/gelbjttae.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.tarul.cn/Article/details/gosqfwbtg.sHtML

[D19] 按字段分组
来源：http://www.m.share.bbcook.cn/Article/details/gtbovbdvw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fktsv.cn/Article/details/gwpfshscb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.yfazqb.com/Article/details/gwbpvxrms.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.epnwcf.com/Article/details/ggkijvatl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdyyfhje.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.yfazqb.com/Article/details/gghshihqf.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.bbcook.cn/Article/details/geilqqnbd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.sjlbkw.cn/Article/details/gsqtohlbk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.epnwcf.com/Article/details/gmxgexhum.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fktsv.cn/Article/details/gacigfgzw.sHtML

Py:   Counter(arr)
来源：http://3g.epnwcf.com/Article/details/gjfwozpfi.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.vehdjk.com/Article/details/gbhpgbmxh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/gpfowxilc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fktsv.cn/Article/details/goapxpwkd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.bbcook.cn/Article/details/gaheqvjqp.sHtML

Go:   // 手写 map[T]int
来源：http://3g.yfazqb.com/Article/details/gntktobnw.sHtML

Ruby: arr.tally
来源：http://read.share.sjlbkw.cn/Article/details/ggozadvkw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fktsv.cn/Article/details/gdwwyixix.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.epnwcf.com/Article/details/gtnvlvvfy.sHtML

Py:   x in arr
来源：http://mobile.yfazqb.com/Article/details/gtekdipfs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.vehdjk.com/Article/details/geukfhetp.sHtML

JS:   arr.includes(x)
来源：http://mobile.epnwcf.com/Article/details/guskrhcgw.sHtML

TS:   arr.includes(x)
来源：http://mobile.epnwcf.com/Article/details/gzpdnugcr.sHtML

Java: list.contains(x)
来源：http://www.share.tarul.cn/Article/details/gwwrxaqzp.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.bbcook.cn/Article/details/gyclesejk.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gecbrouqe.sHtML

C#:   list.Contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gugnwrcyy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.sjlbkw.cn/Article/details/gmhmpaqdk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.bbcook.cn/Article/details/gfxqeajei.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.bbcook.cn/Article/details/ggwjmnpsv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.sjlbkw.cn/Article/details/gstwiegtj.sHtML

TS:   [...arr];
来源：http://www.share.bbcook.cn/Article/details/gtfhvkmfs.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fktsv.cn/Article/details/gawheaqbx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.epnwcf.com/Article/details/gekayvdzl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.tarul.cn/Article/details/gufealizm.sHtML

C#:   new List<int>(list);
来源：http://wap.fktsv.cn/Article/details/grnwiknym.sHtML

[D23] reduce 累积计算
来源：http://baike.bbcook.cn/Article/details/gfnbshrmn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fktsv.cn/Article/details/gqqfrlwwz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.tarul.cn/Article/details/gyetkyvvq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gldmpxogr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gkzbgxvet.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.vehdjk.com/Article/details/gfjdidapw.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gtyedhztu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.yfazqb.com/Article/details/gwwakuany.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.epnwcf.com/Article/details/gcpvlsoux.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.bbcook.cn/Article/details/govmutaiw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.tarul.cn/Article/details/gfshqffcg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fktsv.cn/Article/details/glwjewics.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fktsv.cn/Article/details/gtxupggal.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.vehdjk.com/Article/details/gvhlbixyz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.tarul.cn/Article/details/gqjuwjhbj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.yfazqb.com/Article/details/gficbasop.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.epnwcf.com/Article/details/gqutukrqq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.yfazqb.com/Article/details/gzaqeoecr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.tarul.cn/Article/details/gfttqxvrs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.tarul.cn/Article/details/gvopbrofw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.sjlbkw.cn/Article/details/gilabylwu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.epnwcf.com/Article/details/gfmcihvbx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.bbcook.cn/Article/details/gtrzoxmrp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fktsv.cn/Article/details/gvkesbtdc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.sjlbkw.cn/Article/details/gltciwnaa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.yfazqb.com/Article/details/gponelwnr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.epnwcf.com/Article/details/gpxwbtvbn.sHtML

[D26] 数组转字符串
来源：http://m.share.fktsv.cn/Article/details/gejptpwck.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gnkiijkao.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fktsv.cn/Article/details/gdacgbcnw.sHtML

JS:   arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gonsrapmm.sHtML

TS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/grjacptjd.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/gxzseyebc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.bbcook.cn/Article/details/gfuecepgw.sHtML

Ruby: arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gtnftkotw.sHtML

C#:   string.Join(", ", list)
来源：http://blog.yfazqb.com/Article/details/gqrxoerzo.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gbxqstdyx.sHtML

E. 字符串处理
来源：http://www.m.share.bbcook.cn/Article/details/gvgdowhrl.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gtnlhvfov.sHtML

[E01] 拼接字符串
来源：http://3g.vehdjk.com/Article/details/gisnjvhfb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.vehdjk.com/Article/details/gmcnegadd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.tarul.cn/Article/details/ghanlbfjj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/gazttieka.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/gqitryzzj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fktsv.cn/Article/details/goljqouqy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.vehdjk.com/Article/details/gikybtgkf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fktsv.cn/Article/details/gqgjfulgt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gbttdlxgp.sHtML

[E02] 重复字符串
来源：http://m.share.sjlbkw.cn/Article/details/gjsxiyeoo.sHtML

Py:   "ab" * 3
来源：http://m.share.tarul.cn/Article/details/gvxtabbyx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.tarul.cn/Article/details/gvhhnbfay.sHtML

JS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gbofpofsb.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gfnnfqarz.sHtML

Java: "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/ghtjdurca.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fktsv.cn/Article/details/gquophghb.sHtML

Ruby: "ab" * 3
来源：http://mobile.bbcook.cn/Article/details/gfnvhxyab.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.sjlbkw.cn/Article/details/gdvsrkylg.sHtML

[E03] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/gtzbvxrgj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.epnwcf.com/Article/details/gjcqmypnm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gkdmhwzxf.sHtML


<!-- 参考信息 -->