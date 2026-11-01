代发 wailian999

Ruby: a, b = pair
来源：http://baike.tarul.cn/Article/details/gljvtpdfe.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.tarul.cn/Article/details/gtxfbqvxo.sHtML

[C16] 函数 / 方法重载
来源：http://wap.tarul.cn/Article/details/gwtuyuylh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.epnwcf.com/Article/details/gdemeyyqd.sHtML

PHP:  // 无重载
来源：http://m.share.bbcook.cn/Article/details/gvtubdoqp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.vehdjk.com/Article/details/gjrsdcfax.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fktsv.cn/Article/details/gxwxqyyww.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.yfazqb.com/Article/details/gtnqemhet.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.tarul.cn/Article/details/gnciheuox.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fktsv.cn/Article/details/gxpypuqtb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.sjlbkw.cn/Article/details/ggharnceg.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdvhqzwzv.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.yfazqb.com/Article/details/gkjzlgyzl.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gdkqvzeuc.sHtML

[D01] 创建数组 / 列表
来源：http://wap.bbcook.cn/Article/details/ghbkwdglj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.tarul.cn/Article/details/gnvugarhw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.yfazqb.com/Article/details/ghuoppggw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.tarul.cn/Article/details/gwularpzl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fktsv.cn/Article/details/gutudiqmw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.vehdjk.com/Article/details/gbgsdpjfu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fktsv.cn/Article/details/gumxsafig.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.vehdjk.com/Article/details/guslugenx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.bbcook.cn/Article/details/gbfwctely.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.yfazqb.com/Article/details/gjlovehji.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.epnwcf.com/Article/details/gaqwcqmdo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.epnwcf.com/Article/details/gdkqyxoxw.sHtML

JS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/gsqloxjzq.sHtML

TS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/ggnfmblgh.sHtML

Java: list.add(4);
来源：http://read.share.tarul.cn/Article/details/gacosetaj.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.epnwcf.com/Article/details/guwtgoacy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.sjlbkw.cn/Article/details/gjsokfnee.sHtML

C#:   list.Add(4);
来源：http://baike.fktsv.cn/Article/details/gcbdamlsd.sHtML

[D03] 在指定位置插入元素
来源：http://blog.bbcook.cn/Article/details/gnutwbhfa.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.yfazqb.com/Article/details/gzbezvxdu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.sjlbkw.cn/Article/details/gnuichtkw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.yfazqb.com/Article/details/grmkpjkvh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fktsv.cn/Article/details/gqdftqndr.sHtML

Java: list.add(0, 0);
来源：http://baike.fktsv.cn/Article/details/gwkobpmiy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fktsv.cn/Article/details/gyzdrioub.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.vehdjk.com/Article/details/gicwseyzd.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.yfazqb.com/Article/details/gsquadpps.sHtML

[D04] 删除元素
来源：http://read.share.tarul.cn/Article/details/gsficiabl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fktsv.cn/Article/details/gahzcjuyp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.vehdjk.com/Article/details/gotblnldd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fktsv.cn/Article/details/ghbcxwicz.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.epnwcf.com/Article/details/ggatfylzv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.tarul.cn/Article/details/gvvyrkcay.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.vehdjk.com/Article/details/gnwsnxlos.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.sjlbkw.cn/Article/details/gftvkiqpt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fktsv.cn/Article/details/gpsovepna.sHtML

[D05] 访问与修改元素
来源：http://read.share.tarul.cn/Article/details/gduurnllx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gqasgpogl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gcjofdldo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/gyqskbcxk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.sjlbkw.cn/Article/details/gqxzqwklm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fktsv.cn/Article/details/glxeacvta.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gmvcdcrhx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/grkffzhix.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/glefrpxjx.sHtML

[D06] 数组长度
来源：http://3g.yfazqb.com/Article/details/gpepsecdg.sHtML

Py:   len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gvszpeswp.sHtML

PHP:  count($arr);
来源：http://www.blog.yfazqb.com/Article/details/gqxcszpbk.sHtML

JS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gwnbciddb.sHtML

TS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gjzzdycie.sHtML

Java: list.size();
来源：http://www.share.vehdjk.com/Article/details/gyzaylwkc.sHtML

Go:   len(arr)
来源：http://mobile.tarul.cn/Article/details/gjmzxfywf.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.vehdjk.com/Article/details/ggpsduthp.sHtML

C#:   list.Count;
来源：http://www.m.share.bbcook.cn/Article/details/geysdmonr.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.tarul.cn/Article/details/gyphsbhyp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.bbcook.cn/Article/details/gifetmtxo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.yfazqb.com/Article/details/guuzevvdq.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/gnbqrxtck.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gjzgtzozf.sHtML

Java: list.subList(1, 4);
来源：http://3g.fktsv.cn/Article/details/giksjdioc.sHtML

Go:   arr[1:4]
来源：http://blog.bbcook.cn/Article/details/gcjjayywx.sHtML

Ruby: arr[1, 3]
来源：http://baike.yfazqb.com/Article/details/gozqiskrx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/gvwuslwem.sHtML

[D08] 合并两个数组
来源：http://www.m.share.tarul.cn/Article/details/gtzpybbfu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fktsv.cn/Article/details/gpqlroslz.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.yfazqb.com/Article/details/gmanwlwbv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.epnwcf.com/Article/details/gqdssaaat.sHtML

TS:   [...a, ...b];
来源：http://baike.fktsv.cn/Article/details/gtukbutrl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.vehdjk.com/Article/details/gcpirynsd.sHtML

Go:   append(a, b...)
来源：http://3g.tarul.cn/Article/details/girschzcd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.vehdjk.com/Article/details/gzqibivec.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gdvvbkgve.sHtML

[D09] 排序（升序）
来源：http://www.blog.tarul.cn/Article/details/ghsftwatw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gjcyioqaj.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gbjoatqux.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.epnwcf.com/Article/details/gsvmrsmir.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.bbcook.cn/Article/details/gvfzkeihe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.vehdjk.com/Article/details/gdhsjvsap.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.epnwcf.com/Article/details/gsmsdwqwp.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gsufulwsu.sHtML

C#:   list.Sort();
来源：http://baike.bbcook.cn/Article/details/gappmyfvg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fktsv.cn/Article/details/gkstaktof.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.sjlbkw.cn/Article/details/gpndirziv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.tarul.cn/Article/details/gyazjtlrq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/gpxwypjav.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.epnwcf.com/Article/details/gxhkexiek.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.epnwcf.com/Article/details/gootuotvo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.vehdjk.com/Article/details/glvjnbrme.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.epnwcf.com/Article/details/gevgxgmnf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fktsv.cn/Article/details/ghcbxiiym.sHtML

[D11] 反转数组
来源：http://wap.fktsv.cn/Article/details/gxppjhuby.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.tarul.cn/Article/details/gphhbqdvm.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.yfazqb.com/Article/details/grqdinxvo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.sjlbkw.cn/Article/details/gybyssjvz.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.vehdjk.com/Article/details/gkbdimymq.sHtML

Java: Collections.reverse(list);
来源：http://read.share.yfazqb.com/Article/details/gssjngfji.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.bbcook.cn/Article/details/gfgvvwled.sHtML

Ruby: arr.reverse
来源：http://www.share.yfazqb.com/Article/details/gzylhftih.sHtML

C#:   list.Reverse();
来源：http://mobile.fktsv.cn/Article/details/gufquwhuv.sHtML

[D12] 查找元素下标
来源：http://www.blog.yfazqb.com/Article/details/ginxcddul.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.vehdjk.com/Article/details/gewewbihh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fktsv.cn/Article/details/gakpayspa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/gtltzykpr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gsaxobqid.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.sjlbkw.cn/Article/details/ggplpmquq.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gdiwijqmv.sHtML

Ruby: arr.index(x)
来源：http://m.share.sjlbkw.cn/Article/details/ggswopmbk.sHtML

C#:   list.IndexOf(x);
来源：http://blog.sjlbkw.cn/Article/details/gxqebqell.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fktsv.cn/Article/details/guputtxnq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.sjlbkw.cn/Article/details/ggiagsjyk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.tarul.cn/Article/details/goddmgdhb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/gbfjmvqaq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gxavnznis.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.bbcook.cn/Article/details/gkxyqtpgp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.vehdjk.com/Article/details/ghlwbwnsn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.tarul.cn/Article/details/gahkzcgop.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.bbcook.cn/Article/details/gcuvgbgzf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.sjlbkw.cn/Article/details/gjtptdyoy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.yfazqb.com/Article/details/giwnvvtsx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.tarul.cn/Article/details/geezwftyz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/gpfrtcdou.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/gvilundmv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.epnwcf.com/Article/details/gucxibuxl.sHtML

Go:   // 手写循环
来源：http://3g.fktsv.cn/Article/details/gggbhpveu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.epnwcf.com/Article/details/glaztabdp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.tarul.cn/Article/details/geowzfbrr.sHtML

[D15] 去重
来源：http://m.share.bbcook.cn/Article/details/gdcbgzcgq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.tarul.cn/Article/details/googdxdjb.sHtML

PHP:  array_unique($arr);
来源：http://baike.bbcook.cn/Article/details/gtgktqzbz.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gogbvijoz.sHtML

TS:   [...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gxlgruuhx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.sjlbkw.cn/Article/details/gvrtejona.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.bbcook.cn/Article/details/gxgmqkqmr.sHtML

Ruby: arr.uniq
来源：http://mobile.epnwcf.com/Article/details/gclshfbph.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.bbcook.cn/Article/details/gqualmljz.sHtML

[D16] 求和与平均值
来源：http://mobile.bbcook.cn/Article/details/glhttamfi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gtlrytmrt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.yfazqb.com/Article/details/giuburyhr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/gyzgulods.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/gkbbbhily.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.bbcook.cn/Article/details/gbmmtjczj.sHtML

Go:   // 手写循环累加
来源：http://www.blog.yfazqb.com/Article/details/gutcceiwp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.vehdjk.com/Article/details/gegxjpzzo.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.vehdjk.com/Article/details/gofasrszq.sHtML

[D17] 最大值与最小值
来源：http://mobile.yfazqb.com/Article/details/gvvhlgqne.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.tarul.cn/Article/details/gpdttekuv.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.vehdjk.com/Article/details/gmrakbgqk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.epnwcf.com/Article/details/gxxwoierv.sHtML

TS:   Math.max(...arr);
来源：http://blog.sjlbkw.cn/Article/details/gyyxzanzd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.yfazqb.com/Article/details/gcvzcgtly.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.vehdjk.com/Article/details/ghqrnrohq.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.vehdjk.com/Article/details/guqxmvfqb.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.vehdjk.com/Article/details/gefheejae.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.tarul.cn/Article/details/gvwyrbadp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.bbcook.cn/Article/details/gtfdpduhd.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.epnwcf.com/Article/details/gxpspglyc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.yfazqb.com/Article/details/gnjvwuxru.sHtML

TS:   nested.flat();
来源：http://wap.epnwcf.com/Article/details/gntmudfjt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.sjlbkw.cn/Article/details/glkldnnzm.sHtML

Go:   // 手写双层循环
来源：http://baike.fktsv.cn/Article/details/gxbfhanru.sHtML

Ruby: nested.flatten
来源：http://blog.yfazqb.com/Article/details/gmwrhfqmo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.tarul.cn/Article/details/gnuuicgvj.sHtML

[D19] 按字段分组
来源：http://www.m.share.epnwcf.com/Article/details/gkspuzijk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fktsv.cn/Article/details/gykdsqslm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.tarul.cn/Article/details/guyhhrzpc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fktsv.cn/Article/details/ghuoecmxk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.yfazqb.com/Article/details/gneamonyp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.tarul.cn/Article/details/gbcteddim.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.tarul.cn/Article/details/gvgxhmvyp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fktsv.cn/Article/details/ghcxijuhm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fktsv.cn/Article/details/gdfvatlup.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.sjlbkw.cn/Article/details/gnzfvnhsz.sHtML

Py:   Counter(arr)
来源：http://mobile.tarul.cn/Article/details/ggoqfchqz.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.epnwcf.com/Article/details/gcdcxhpqy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.epnwcf.com/Article/details/gzetfuxfm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/gnsvizifw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.epnwcf.com/Article/details/gschydkch.sHtML

Go:   // 手写 map[T]int
来源：http://blog.bbcook.cn/Article/details/gcefvpftf.sHtML

Ruby: arr.tally
来源：http://blog.vehdjk.com/Article/details/gafghqztv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.bbcook.cn/Article/details/ghjkkueut.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.yfazqb.com/Article/details/gqaddwdhd.sHtML

Py:   x in arr
来源：http://read.share.vehdjk.com/Article/details/givcfohnu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.vehdjk.com/Article/details/gpxdukawx.sHtML

JS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/gblmpqetv.sHtML

TS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/gnxyahlca.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gvhcdpkad.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gmayjwcxk.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fktsv.cn/Article/details/ggnaekszr.sHtML

C#:   list.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gmaiekpem.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fktsv.cn/Article/details/gbwlmicaf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.vehdjk.com/Article/details/gpexltwaa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.epnwcf.com/Article/details/gpsevhdqe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.tarul.cn/Article/details/gdevdysnl.sHtML

TS:   [...arr];
来源：http://baike.fktsv.cn/Article/details/gylgxdxyz.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.yfazqb.com/Article/details/gtyvwgbji.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.tarul.cn/Article/details/grdkiizqs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.vehdjk.com/Article/details/gmlnwflnt.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.tarul.cn/Article/details/gtpmliksf.sHtML

[D23] reduce 累积计算
来源：http://baike.fktsv.cn/Article/details/gapatmzwt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fktsv.cn/Article/details/gcqznborm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/gfvmmtcim.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gswzqirjt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/gsnaqmgfk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.yfazqb.com/Article/details/gehbklawn.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/gjwtsszlo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.vehdjk.com/Article/details/gtlhqpxdl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.sjlbkw.cn/Article/details/gwqagziqr.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.tarul.cn/Article/details/gytcehacg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.epnwcf.com/Article/details/gxajfovxb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.bbcook.cn/Article/details/gqbsjpzgh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fktsv.cn/Article/details/gdtxxobvh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gcelljcis.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.tarul.cn/Article/details/gbvmcscdu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.epnwcf.com/Article/details/gvjrojpfl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.sjlbkw.cn/Article/details/guiblodss.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fktsv.cn/Article/details/gwjtvkywf.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.bbcook.cn/Article/details/gcnpfwtiq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.epnwcf.com/Article/details/gqesnydqe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.epnwcf.com/Article/details/gcxantiqi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.sjlbkw.cn/Article/details/gqxnkvfjc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fktsv.cn/Article/details/gtjyoyusj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.bbcook.cn/Article/details/gvyjmnvaj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.vehdjk.com/Article/details/gtnrnkvgf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.yfazqb.com/Article/details/glgeungmo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.tarul.cn/Article/details/gfxyipeqe.sHtML

[D26] 数组转字符串
来源：http://blog.bbcook.cn/Article/details/gmflbpsjn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.epnwcf.com/Article/details/gbqprwrjf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.tarul.cn/Article/details/ghkqmfukt.sHtML

JS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gpvjpicvh.sHtML

TS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gqnnegswm.sHtML

Java: String.join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/ghamojwnw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.sjlbkw.cn/Article/details/gudeyxxhn.sHtML

Ruby: arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gvohxplex.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/gpghokler.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gxvxpwkei.sHtML

E. 字符串处理
来源：http://blog.fktsv.cn/Article/details/gkvfwgthj.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ggmnaayyw.sHtML

[E01] 拼接字符串
来源：http://www.share.tarul.cn/Article/details/givhybcey.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.epnwcf.com/Article/details/giwwevmwo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.yfazqb.com/Article/details/gjlcrorga.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/guttsjrvk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/gnhgkkhbz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.yfazqb.com/Article/details/ghtpibqfi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.tarul.cn/Article/details/ghqhgthsb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.vehdjk.com/Article/details/gcmdobltx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gnrktvdvk.sHtML

[E02] 重复字符串
来源：http://www.share.yfazqb.com/Article/details/gqitdhuej.sHtML

Py:   "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gaywnoyme.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.vehdjk.com/Article/details/gmbtisguq.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/giirjrrvi.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gmnrmmpsb.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gnmhcmprr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fktsv.cn/Article/details/gjdlfnetz.sHtML

Ruby: "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gofaklyid.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.epnwcf.com/Article/details/gpxlvpuie.sHtML

[E03] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gigrlhdnt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fktsv.cn/Article/details/gkdpkeqvk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gorhpvwxe.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.vehdjk.com/Article/details/gjfftpuxz.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.tarul.cn/Article/details/gzvpvgfxe.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gushmgdhe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/gwxijqdgh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.yfazqb.com/Article/details/gwhwcdtve.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtulnmiwu.sHtML

[E04] 查找子串位置
来源：http://www.share.bbcook.cn/Article/details/gcmnksmek.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.tarul.cn/Article/details/gaawcsmgd.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/gukwhygpt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.bbcook.cn/Article/details/gtfslypep.sHtML

TS:   s.indexOf("x")
来源：http://mobile.bbcook.cn/Article/details/glwjswgld.sHtML

Java: s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/gnyuutyrg.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fktsv.cn/Article/details/gwpyqugpi.sHtML

Ruby: s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gkxjfwsrw.sHtML

C#:   s.IndexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gstxsisdd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.bbcook.cn/Article/details/gseafxfta.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.yfazqb.com/Article/details/gygsozirb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.sjlbkw.cn/Article/details/gbgpocgru.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.bbcook.cn/Article/details/gcfpjjslm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.tarul.cn/Article/details/gsqnxyqqy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/glvsglszz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.tarul.cn/Article/details/gtoncvvdq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.bbcook.cn/Article/details/gvlsaikrk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.yfazqb.com/Article/details/gkfgkzmoc.sHtML

[E06] 替换子串
来源：http://wap.bbcook.cn/Article/details/gwubersaa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gcgfqggqz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.bbcook.cn/Article/details/gsrvbyevg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gnnjqxkfc.sHtML


<!-- 参考信息 -->