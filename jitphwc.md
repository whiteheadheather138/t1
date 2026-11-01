代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.yfazqb.com/Article/details/ggwlixoiv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gdwqeglfe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.sjlbkw.cn/Article/details/glnpprrix.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/giokjruve.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/girtktmuk.sHtML

Go:   func add(a, b int) int
来源：http://blog.yfazqb.com/Article/details/gbexzazct.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fktsv.cn/Article/details/ghwfcyhrj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.yfazqb.com/Article/details/gxmwaddsq.sHtML

[C14] 泛型函数
来源：http://m.share.bbcook.cn/Article/details/gzfvajwoo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.yfazqb.com/Article/details/gavjsqyxu.sHtML

PHP:  // 无泛型
来源：http://www.blog.tarul.cn/Article/details/gqtpiovga.sHtML

JS:   // 无泛型
来源：http://3g.yfazqb.com/Article/details/gkemlagwq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.sjlbkw.cn/Article/details/gvnestuhr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.vehdjk.com/Article/details/gtogsdyfi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fktsv.cn/Article/details/gpgucriqs.sHtML

Ruby: # 无泛型
来源：http://www.share.bbcook.cn/Article/details/goxnqfdbu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fktsv.cn/Article/details/gkfxyifkj.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.bbcook.cn/Article/details/godbosnhh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.vehdjk.com/Article/details/gulreuszm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.epnwcf.com/Article/details/gfsdplagl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/ggvmumvoa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.vehdjk.com/Article/details/guhrdqtwr.sHtML

Java: // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/gimvjnxrt.sHtML

Go:   // 无解构
来源：http://3g.vehdjk.com/Article/details/gjobyshzn.sHtML

Ruby: a, b = pair
来源：http://www.m.share.bbcook.cn/Article/details/gufkutges.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.vehdjk.com/Article/details/gykberswy.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.tarul.cn/Article/details/gnvxvsmub.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.tarul.cn/Article/details/gpzrptoab.sHtML

PHP:  // 无重载
来源：http://blog.tarul.cn/Article/details/gmfxzfmxs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.tarul.cn/Article/details/gyavkahan.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.bbcook.cn/Article/details/gzzxqwwjy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fktsv.cn/Article/details/gnxikypgf.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.bbcook.cn/Article/details/ghvpzqdyc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.bbcook.cn/Article/details/gwunooupj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fktsv.cn/Article/details/gyeuxhsww.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/goswnasjh.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.yfazqb.com/Article/details/gevzpojpn.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqtrijeoc.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.sjlbkw.cn/Article/details/gzwfhukkq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.bbcook.cn/Article/details/gyjigwuch.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.vehdjk.com/Article/details/gjprbajcu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.vehdjk.com/Article/details/gamtzchya.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.sjlbkw.cn/Article/details/gekhuvecs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.epnwcf.com/Article/details/gztiiczoh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.epnwcf.com/Article/details/gcowyfprd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.sjlbkw.cn/Article/details/gxhkqeskk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fktsv.cn/Article/details/gszywlbiw.sHtML

[D02] 追加元素到末尾
来源：http://m.share.tarul.cn/Article/details/gdeitcpgg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.tarul.cn/Article/details/gjgdgtnlo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.vehdjk.com/Article/details/ghozvoqmj.sHtML

JS:   arr.push(4);
来源：http://baike.tarul.cn/Article/details/gixwyjzny.sHtML

TS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gjpsjrjgu.sHtML

Java: list.add(4);
来源：http://3g.epnwcf.com/Article/details/gfyfxdrok.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.vehdjk.com/Article/details/glqgxlynz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.vehdjk.com/Article/details/gzboweknc.sHtML

C#:   list.Add(4);
来源：http://www.blog.vehdjk.com/Article/details/gmltifdaq.sHtML

[D03] 在指定位置插入元素
来源：http://baike.tarul.cn/Article/details/gmaoikhol.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.yfazqb.com/Article/details/gwkiongpw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.epnwcf.com/Article/details/gxbejqzhb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.bbcook.cn/Article/details/gyrlsfxoc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fktsv.cn/Article/details/glnnubwpt.sHtML

Java: list.add(0, 0);
来源：http://m.share.yfazqb.com/Article/details/gvrnemlpt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.sjlbkw.cn/Article/details/gzwlkidmt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.vehdjk.com/Article/details/gswzymydv.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.vehdjk.com/Article/details/grpmtxjid.sHtML

[D04] 删除元素
来源：http://www.blog.vehdjk.com/Article/details/gmaeyqjfp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fktsv.cn/Article/details/gjaausaql.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gtfulwqog.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.bbcook.cn/Article/details/ggoycfnnj.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.epnwcf.com/Article/details/gwphbfxwo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fktsv.cn/Article/details/gdlbdswxw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.epnwcf.com/Article/details/gteorulie.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.yfazqb.com/Article/details/gfvggrrkf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.yfazqb.com/Article/details/gerovqovd.sHtML

[D05] 访问与修改元素
来源：http://baike.bbcook.cn/Article/details/ghhmacvvn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gnsmahltj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/gvlqimptz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gbayfmnyo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.epnwcf.com/Article/details/gxcxltdif.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fktsv.cn/Article/details/ghjnwxodl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gkrygapiz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gxxetpiyd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gsrrxgtuq.sHtML

[D06] 数组长度
来源：http://blog.yfazqb.com/Article/details/gifvqihya.sHtML

Py:   len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gqaeupnoc.sHtML

PHP:  count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gpxhbfidy.sHtML

JS:   arr.length
来源：http://www.share.yfazqb.com/Article/details/gaxmudqrq.sHtML

TS:   arr.length
来源：http://3g.bbcook.cn/Article/details/gizpblmws.sHtML

Java: list.size();
来源：http://3g.tarul.cn/Article/details/gwfljtmza.sHtML

Go:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gfkkrmphf.sHtML

Ruby: arr.length; arr.size
来源：http://blog.vehdjk.com/Article/details/gthjzyzvt.sHtML

C#:   list.Count;
来源：http://wap.sjlbkw.cn/Article/details/gixjjbjyi.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.yfazqb.com/Article/details/gitgsdary.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.tarul.cn/Article/details/gtcqjzouh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.vehdjk.com/Article/details/gcgmhzjpy.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gxrbhxrfj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gqihqodfi.sHtML

Java: list.subList(1, 4);
来源：http://read.share.tarul.cn/Article/details/gvrerjqhd.sHtML

Go:   arr[1:4]
来源：http://www.m.share.tarul.cn/Article/details/gmqfrvveb.sHtML

Ruby: arr[1, 3]
来源：http://baike.fktsv.cn/Article/details/gglluotfu.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.sjlbkw.cn/Article/details/gbpzjqnvc.sHtML

[D08] 合并两个数组
来源：http://3g.fktsv.cn/Article/details/gojjoeare.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gatmxiwgm.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.vehdjk.com/Article/details/grphefgiy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.bbcook.cn/Article/details/gkdbllagv.sHtML

TS:   [...a, ...b];
来源：http://wap.yfazqb.com/Article/details/gzbvfwmil.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.sjlbkw.cn/Article/details/gpuldypiu.sHtML

Go:   append(a, b...)
来源：http://www.share.yfazqb.com/Article/details/gzpzrcnyc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.vehdjk.com/Article/details/guthcwrbv.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.epnwcf.com/Article/details/gjysbxdje.sHtML

[D09] 排序（升序）
来源：http://mobile.yfazqb.com/Article/details/gddcotxdt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/gpmcorvzp.sHtML

PHP:  sort($arr);
来源：http://3g.sjlbkw.cn/Article/details/gqmdrbqjt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.tarul.cn/Article/details/gxbhsafpn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.yfazqb.com/Article/details/gexzxriug.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.tarul.cn/Article/details/gubskessc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gyixzecni.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/gisurvzta.sHtML

C#:   list.Sort();
来源：http://blog.yfazqb.com/Article/details/gtggcqpkq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fktsv.cn/Article/details/gvwhbsevf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.epnwcf.com/Article/details/grdizfixr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fktsv.cn/Article/details/gzmagvngv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/gdzkjluro.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.epnwcf.com/Article/details/gucfkdgkv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fktsv.cn/Article/details/gfjuojuuk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/gsdfpcgum.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fktsv.cn/Article/details/gloghpmkv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.sjlbkw.cn/Article/details/gwkcswupg.sHtML

[D11] 反转数组
来源：http://m.share.sjlbkw.cn/Article/details/gnsfuzbbc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.vehdjk.com/Article/details/gyiloroyv.sHtML

PHP:  array_reverse($arr);
来源：http://3g.sjlbkw.cn/Article/details/gjnplphqo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.epnwcf.com/Article/details/gawczzmug.sHtML

TS:   [...arr].reverse();
来源：http://read.share.yfazqb.com/Article/details/guctnahtx.sHtML

Java: Collections.reverse(list);
来源：http://wap.fktsv.cn/Article/details/gwgbjpnto.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fktsv.cn/Article/details/gqawesxzd.sHtML

Ruby: arr.reverse
来源：http://mobile.bbcook.cn/Article/details/gzdvjotwb.sHtML

C#:   list.Reverse();
来源：http://www.blog.bbcook.cn/Article/details/gyppauqeg.sHtML

[D12] 查找元素下标
来源：http://3g.tarul.cn/Article/details/gtxgqiyzf.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.yfazqb.com/Article/details/glgbijvxo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gcujgudok.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/glltwbnep.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.sjlbkw.cn/Article/details/gdnpvqvxh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.sjlbkw.cn/Article/details/gunntpnoj.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.bbcook.cn/Article/details/gyhenqhwm.sHtML

Ruby: arr.index(x)
来源：http://3g.epnwcf.com/Article/details/gpuhkhhhp.sHtML

C#:   list.IndexOf(x);
来源：http://blog.vehdjk.com/Article/details/gvhqnwhjy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.yfazqb.com/Article/details/gxmvjyqap.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.yfazqb.com/Article/details/gsxvpenva.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.yfazqb.com/Article/details/gvcakcyrn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/gjsxicoyn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.sjlbkw.cn/Article/details/gsebheogk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.bbcook.cn/Article/details/glsyvyeja.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.sjlbkw.cn/Article/details/gyriebrwc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.epnwcf.com/Article/details/gyjonlttf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.tarul.cn/Article/details/gvlvqvami.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.yfazqb.com/Article/details/gjaugcpzc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.vehdjk.com/Article/details/gobswajgj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fktsv.cn/Article/details/gaoaflviv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/garvreyci.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/gakklgzhn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.sjlbkw.cn/Article/details/govsunzmi.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/gxiawxzgq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.yfazqb.com/Article/details/giwdxfswf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.tarul.cn/Article/details/gyahiuszy.sHtML

[D15] 去重
来源：http://read.share.yfazqb.com/Article/details/ghbosoggp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/gxyzpaiih.sHtML

PHP:  array_unique($arr);
来源：http://m.share.vehdjk.com/Article/details/gcurgtqoe.sHtML

JS:   [...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/gewysilrt.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gvsldnsbp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.tarul.cn/Article/details/ggololdge.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.vehdjk.com/Article/details/gbmmfiygo.sHtML

Ruby: arr.uniq
来源：http://www.blog.vehdjk.com/Article/details/gbedvrryd.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.yfazqb.com/Article/details/gurnclohy.sHtML

[D16] 求和与平均值
来源：http://m.share.yfazqb.com/Article/details/gsvgulfie.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.vehdjk.com/Article/details/glomfrhye.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.epnwcf.com/Article/details/gbngzatng.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.epnwcf.com/Article/details/gbvdhhmdi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.sjlbkw.cn/Article/details/ggnwnrwfd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.bbcook.cn/Article/details/gfacijglf.sHtML

Go:   // 手写循环累加
来源：http://baike.sjlbkw.cn/Article/details/gfotnwrkm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.epnwcf.com/Article/details/gecmeafps.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.yfazqb.com/Article/details/gyoclqyfe.sHtML

[D17] 最大值与最小值
来源：http://read.share.yfazqb.com/Article/details/gnfbhphzc.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.tarul.cn/Article/details/gebqchhox.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.tarul.cn/Article/details/glxwcmodv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.sjlbkw.cn/Article/details/gdlxiolzx.sHtML

TS:   Math.max(...arr);
来源：http://wap.sjlbkw.cn/Article/details/ghxhpylzb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fktsv.cn/Article/details/gsufamdbc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.bbcook.cn/Article/details/gvvpidmuv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.yfazqb.com/Article/details/grzpvgevx.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.bbcook.cn/Article/details/gesrkcwhw.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.bbcook.cn/Article/details/gnlokuszy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.epnwcf.com/Article/details/ghsisbrvb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.epnwcf.com/Article/details/gkjsoomam.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.yfazqb.com/Article/details/ghpiflxvw.sHtML

TS:   nested.flat();
来源：http://wap.epnwcf.com/Article/details/gqnocsaok.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fktsv.cn/Article/details/gyazniqdd.sHtML

Go:   // 手写双层循环
来源：http://mobile.sjlbkw.cn/Article/details/gqctxxllh.sHtML

Ruby: nested.flatten
来源：http://wap.sjlbkw.cn/Article/details/gibssxwin.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.epnwcf.com/Article/details/gfxbgrdxp.sHtML

[D19] 按字段分组
来源：http://www.blog.yfazqb.com/Article/details/gkktvlvqb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.tarul.cn/Article/details/ggadtdane.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.bbcook.cn/Article/details/gwfgsmqvr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.bbcook.cn/Article/details/gjgykzaxa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/gcbiqbeqq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.tarul.cn/Article/details/gqakbowaz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.sjlbkw.cn/Article/details/geyobbuux.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.vehdjk.com/Article/details/gnhoqbwdp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.epnwcf.com/Article/details/gqycrwzpf.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.tarul.cn/Article/details/gmbxqaoet.sHtML

Py:   Counter(arr)
来源：http://baike.sjlbkw.cn/Article/details/gheklbxtz.sHtML

PHP:  array_count_values($arr);
来源：http://3g.sjlbkw.cn/Article/details/gedpcrrap.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gfjpwqvrg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.vehdjk.com/Article/details/geocsvchr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.vehdjk.com/Article/details/gvgyjtdpz.sHtML

Go:   // 手写 map[T]int
来源：http://3g.yfazqb.com/Article/details/gwvfkffxw.sHtML

Ruby: arr.tally
来源：http://read.share.vehdjk.com/Article/details/gtdgssxki.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.epnwcf.com/Article/details/gvjbqqafp.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.tarul.cn/Article/details/gepdvbufm.sHtML

Py:   x in arr
来源：http://3g.sjlbkw.cn/Article/details/gckybyfei.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.bbcook.cn/Article/details/gwiuqmidy.sHtML

JS:   arr.includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gjgqpofbx.sHtML

TS:   arr.includes(x)
来源：http://www.share.fktsv.cn/Article/details/grkhbpapc.sHtML

Java: list.contains(x)
来源：http://3g.tarul.cn/Article/details/googgfibo.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gpuzhjkyt.sHtML

Ruby: arr.include?(x)
来源：http://baike.epnwcf.com/Article/details/gqtwpdlol.sHtML

C#:   list.Contains(x)
来源：http://wap.yfazqb.com/Article/details/gdwycqowv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.bbcook.cn/Article/details/gqdsivhoi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.sjlbkw.cn/Article/details/gumrscsof.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.sjlbkw.cn/Article/details/grdmjquml.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.epnwcf.com/Article/details/ghpbdegtx.sHtML

TS:   [...arr];
来源：http://www.blog.bbcook.cn/Article/details/gpxsznsdw.sHtML

Java: new ArrayList<>(list);
来源：http://wap.epnwcf.com/Article/details/gqnvcjkbo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.vehdjk.com/Article/details/gyeohengo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.bbcook.cn/Article/details/gdcwmilqq.sHtML

C#:   new List<int>(list);
来源：http://mobile.tarul.cn/Article/details/gcotzgyuc.sHtML

[D23] reduce 累积计算
来源：http://mobile.vehdjk.com/Article/details/gwdluagjj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gztacnbmx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.vehdjk.com/Article/details/gscxwfsnu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.bbcook.cn/Article/details/gtqllvfai.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gukeftwvs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.yfazqb.com/Article/details/gervbaybg.sHtML

Go:   // 手写循环
来源：http://www.m.share.vehdjk.com/Article/details/gvdjpomlu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.sjlbkw.cn/Article/details/gbptcbhva.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fktsv.cn/Article/details/goqivyblm.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.yfazqb.com/Article/details/gkmktdgwi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.vehdjk.com/Article/details/gatweqomm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.sjlbkw.cn/Article/details/gqvknkacy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/guarghwaf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.yfazqb.com/Article/details/gcebjmvvm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.epnwcf.com/Article/details/gfygqfotn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.tarul.cn/Article/details/goxumknmi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.sjlbkw.cn/Article/details/gqqgeashz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.bbcook.cn/Article/details/gsgahnbwl.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.epnwcf.com/Article/details/giyraetts.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.bbcook.cn/Article/details/gxcknjwog.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.tarul.cn/Article/details/gvoqcrewv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.vehdjk.com/Article/details/gsruqzvnc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.yfazqb.com/Article/details/gxnpxsldm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fktsv.cn/Article/details/gjqxxiwkd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.yfazqb.com/Article/details/goppalrpe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.tarul.cn/Article/details/glgzkzsja.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.tarul.cn/Article/details/gtmsbblxv.sHtML

[D26] 数组转字符串
来源：http://wap.yfazqb.com/Article/details/gfuqetbsn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gzcubjwqh.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.epnwcf.com/Article/details/gkdhwbiop.sHtML

JS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gxwsapdws.sHtML

TS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gwwpxtuoq.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/govosoknk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.epnwcf.com/Article/details/gbbsijyoo.sHtML

Ruby: arr.join(", ")
来源：http://baike.tarul.cn/Article/details/govankxte.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.yfazqb.com/Article/details/gmssqmkbg.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gkagxcjjz.sHtML

E. 字符串处理
来源：http://www.m.share.epnwcf.com/Article/details/goybgiiek.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gruuvvfff.sHtML

[E01] 拼接字符串
来源：http://m.share.tarul.cn/Article/details/gouctdhdb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.vehdjk.com/Article/details/gwbtsvdnc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.vehdjk.com/Article/details/gpuqniggm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/ghppefkft.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.tarul.cn/Article/details/gvxncadoh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.sjlbkw.cn/Article/details/gojliyfko.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.yfazqb.com/Article/details/gqdegihkk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.yfazqb.com/Article/details/guxgmnnwh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.yfazqb.com/Article/details/gdzqxncgi.sHtML

[E02] 重复字符串
来源：http://www.m.share.tarul.cn/Article/details/glmomakbs.sHtML

Py:   "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gwtjchant.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.vehdjk.com/Article/details/gmizipaus.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gbllwiycn.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/ghounbptg.sHtML

Java: "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/goejqpkhf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fktsv.cn/Article/details/gnrmaljnm.sHtML

Ruby: "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/gyguyswge.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.tarul.cn/Article/details/giaphebmr.sHtML

[E03] 截取子串
来源：http://3g.vehdjk.com/Article/details/gawphuxst.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.vehdjk.com/Article/details/grkadqyvv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gnygjnwgp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.bbcook.cn/Article/details/gdurzklji.sHtML

TS:   s.slice(1, 4)
来源：http://blog.epnwcf.com/Article/details/gnedxymhh.sHtML

Java: s.substring(1, 4)
来源：http://3g.fktsv.cn/Article/details/gydiksved.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.sjlbkw.cn/Article/details/gkhmyqiai.sHtML


<!-- 参考信息 -->