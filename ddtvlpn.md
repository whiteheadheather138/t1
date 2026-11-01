代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gxixafwew.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/ggfamiiry.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gjrnafmer.sHtML

[D06] 数组长度
来源：http://blog.vehdjk.com/Article/details/gsvxwvvbe.sHtML

Py:   len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gbskeoajg.sHtML

PHP:  count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gkejqhpol.sHtML

JS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/geyjyhzto.sHtML

TS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gmhxyqige.sHtML

Java: list.size();
来源：http://www.share.fktsv.cn/Article/details/glupvhrui.sHtML

Go:   len(arr)
来源：http://wap.yfazqb.com/Article/details/gbicwsuxm.sHtML

Ruby: arr.length; arr.size
来源：http://3g.yfazqb.com/Article/details/gvmzlgchu.sHtML

C#:   list.Count;
来源：http://wap.sjlbkw.cn/Article/details/gljssteew.sHtML

[D07] 切片 / 取子数组
来源：http://3g.vehdjk.com/Article/details/gclsvxexz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.bbcook.cn/Article/details/grknzdgle.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.sjlbkw.cn/Article/details/gwyfxqdae.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.tarul.cn/Article/details/ggvnhrgcv.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.vehdjk.com/Article/details/giviudrkl.sHtML

Java: list.subList(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gdnlelgma.sHtML

Go:   arr[1:4]
来源：http://mobile.epnwcf.com/Article/details/gesuuwpos.sHtML

Ruby: arr[1, 3]
来源：http://wap.epnwcf.com/Article/details/gdssoolyh.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/glftcbayc.sHtML

[D08] 合并两个数组
来源：http://baike.tarul.cn/Article/details/gfmgorjvk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbzrptsy.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fktsv.cn/Article/details/gisummikb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.yfazqb.com/Article/details/gftlfubgv.sHtML

TS:   [...a, ...b];
来源：http://www.blog.epnwcf.com/Article/details/gdlrbaqzz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gvrkbdile.sHtML

Go:   append(a, b...)
来源：http://wap.yfazqb.com/Article/details/gnuucullc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.tarul.cn/Article/details/gldxkzwmv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gftedmgfs.sHtML

[D09] 排序（升序）
来源：http://read.share.epnwcf.com/Article/details/grupktqro.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gcqsghbej.sHtML

PHP:  sort($arr);
来源：http://wap.vehdjk.com/Article/details/gxgvldjvw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.bbcook.cn/Article/details/gyatyxbec.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fktsv.cn/Article/details/gfeymxden.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.bbcook.cn/Article/details/gkgzewyee.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gqadhvcab.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gyxevdylg.sHtML

C#:   list.Sort();
来源：http://m.share.fktsv.cn/Article/details/gvwcivkge.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.bbcook.cn/Article/details/grhtadcil.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gnesotpgl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gldhnnpmz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.yfazqb.com/Article/details/gscxnnlgw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.bbcook.cn/Article/details/gqtftlqkp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.vehdjk.com/Article/details/grhdhqyrn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.sjlbkw.cn/Article/details/gndzvhklr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.tarul.cn/Article/details/gmntviswh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.sjlbkw.cn/Article/details/ggxgbzcvb.sHtML

[D11] 反转数组
来源：http://www.m.share.tarul.cn/Article/details/giisqzhwo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fktsv.cn/Article/details/gxqoikdbe.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gqzikpxhu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.yfazqb.com/Article/details/giukakksq.sHtML

TS:   [...arr].reverse();
来源：http://read.share.vehdjk.com/Article/details/gutfnkkzw.sHtML

Java: Collections.reverse(list);
来源：http://mobile.epnwcf.com/Article/details/gfdauytah.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.yfazqb.com/Article/details/gyqnvibwy.sHtML

Ruby: arr.reverse
来源：http://m.share.epnwcf.com/Article/details/gpdkzlefw.sHtML

C#:   list.Reverse();
来源：http://m.share.fktsv.cn/Article/details/gwwpwlosv.sHtML

[D12] 查找元素下标
来源：http://mobile.vehdjk.com/Article/details/gyveamqcu.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.vehdjk.com/Article/details/gkaaaffcw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.yfazqb.com/Article/details/gvimpaxso.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/gispyyssw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.epnwcf.com/Article/details/gnupsmgkj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.yfazqb.com/Article/details/gkfykgbrl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gkxthwvmv.sHtML

Ruby: arr.index(x)
来源：http://www.share.sjlbkw.cn/Article/details/ggyojbdqn.sHtML

C#:   list.IndexOf(x);
来源：http://blog.yfazqb.com/Article/details/gazmgfhre.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.yfazqb.com/Article/details/gnxbykbjk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.vehdjk.com/Article/details/gnjufcwdi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.tarul.cn/Article/details/giatlflal.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/gbsonzobr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/gjnzfivfd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.epnwcf.com/Article/details/gqkfatvrw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/gqpdheqbf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.vehdjk.com/Article/details/gmzmlgabr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gmrklbuqi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.sjlbkw.cn/Article/details/gucubhwna.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gxuoajfiu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.tarul.cn/Article/details/gvoowzzgp.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.yfazqb.com/Article/details/gcncowstx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.yfazqb.com/Article/details/gpuuksxte.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.vehdjk.com/Article/details/gcvcpfwmi.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/gxacmgjpp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.tarul.cn/Article/details/grosqkopy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.epnwcf.com/Article/details/glpevwptr.sHtML

[D15] 去重
来源：http://read.share.sjlbkw.cn/Article/details/gfblwyzak.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/gvgswwail.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fktsv.cn/Article/details/gxbklwvje.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gstqhjdkm.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gqnakvzlo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.yfazqb.com/Article/details/gpvyvptmr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.vehdjk.com/Article/details/gvryzgkzm.sHtML

Ruby: arr.uniq
来源：http://blog.yfazqb.com/Article/details/gtjqayxaw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gonpggpre.sHtML

[D16] 求和与平均值
来源：http://www.share.yfazqb.com/Article/details/gcnlcmiev.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.epnwcf.com/Article/details/grewsmneg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.vehdjk.com/Article/details/grfdkxiia.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/gmpwthpdr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.tarul.cn/Article/details/gjqbpfqfx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.vehdjk.com/Article/details/ghpxoqmdo.sHtML

Go:   // 手写循环累加
来源：http://baike.fktsv.cn/Article/details/gttuilzzy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/gwohncbmg.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fktsv.cn/Article/details/glyqutcyf.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fktsv.cn/Article/details/grafvzoku.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.vehdjk.com/Article/details/gqxjweaju.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fktsv.cn/Article/details/gqgggvlnj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.sjlbkw.cn/Article/details/gjhzjmdda.sHtML

TS:   Math.max(...arr);
来源：http://m.share.sjlbkw.cn/Article/details/gduuatfkg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.bbcook.cn/Article/details/gzcwdsvbi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/guljduuuy.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.tarul.cn/Article/details/gdmxlvzhu.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.bbcook.cn/Article/details/gqqtwurzh.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fktsv.cn/Article/details/gfkysxmtx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.epnwcf.com/Article/details/gtzfekokn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.epnwcf.com/Article/details/gzlydeory.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.tarul.cn/Article/details/gfidmogzn.sHtML

TS:   nested.flat();
来源：http://www.m.share.epnwcf.com/Article/details/gcozbsuur.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.yfazqb.com/Article/details/giozvrmmk.sHtML

Go:   // 手写双层循环
来源：http://baike.vehdjk.com/Article/details/gozqyvhpg.sHtML

Ruby: nested.flatten
来源：http://baike.vehdjk.com/Article/details/gjaijdpcp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.vehdjk.com/Article/details/gzidqbipz.sHtML

[D19] 按字段分组
来源：http://wap.yfazqb.com/Article/details/gswgjgjya.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.vehdjk.com/Article/details/gajmbullu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.epnwcf.com/Article/details/ghjyobnuc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.tarul.cn/Article/details/ghamatzfx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/gslyaqbsm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.bbcook.cn/Article/details/gemesejpy.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.bbcook.cn/Article/details/gunzccdpl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.vehdjk.com/Article/details/gijccdycv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.epnwcf.com/Article/details/gnharoxud.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.tarul.cn/Article/details/gzhismiaz.sHtML

Py:   Counter(arr)
来源：http://m.share.yfazqb.com/Article/details/gwhscqben.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gvzdrrdvk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.vehdjk.com/Article/details/gknjllnsm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.yfazqb.com/Article/details/gdgagcsyx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.bbcook.cn/Article/details/gxfuvhope.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.bbcook.cn/Article/details/guekwupqu.sHtML

Ruby: arr.tally
来源：http://www.blog.sjlbkw.cn/Article/details/gskkbrvzv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.bbcook.cn/Article/details/gbakxgwei.sHtML

[D21] 判断是否包含某元素
来源：http://3g.epnwcf.com/Article/details/gsrvwxltf.sHtML

Py:   x in arr
来源：http://3g.sjlbkw.cn/Article/details/girgrhtut.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.yfazqb.com/Article/details/gogvousmo.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gfsyqutso.sHtML

TS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/gybmtovif.sHtML

Java: list.contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gkaopqlgw.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyowlngst.sHtML

Ruby: arr.include?(x)
来源：http://baike.tarul.cn/Article/details/ghitalodz.sHtML

C#:   list.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/ggnaciomy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.yfazqb.com/Article/details/ghrleqkze.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.bbcook.cn/Article/details/ghtsdgeog.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.vehdjk.com/Article/details/gwqpjlryn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gxkepnuhm.sHtML

TS:   [...arr];
来源：http://www.share.fktsv.cn/Article/details/gjjnysqae.sHtML

Java: new ArrayList<>(list);
来源：http://baike.yfazqb.com/Article/details/gwjjupcgl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.yfazqb.com/Article/details/gjvudcczv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.bbcook.cn/Article/details/gkhcdeudt.sHtML

C#:   new List<int>(list);
来源：http://3g.bbcook.cn/Article/details/gnawvryyx.sHtML

[D23] reduce 累积计算
来源：http://www.share.tarul.cn/Article/details/gsvjsohru.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.epnwcf.com/Article/details/gxemfpxdx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.bbcook.cn/Article/details/gopbmebnp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fktsv.cn/Article/details/grayglyvo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gtguqwjbr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fktsv.cn/Article/details/gdebujplh.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/guzzstbvv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.yfazqb.com/Article/details/gshurdrou.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.sjlbkw.cn/Article/details/glfvqsaql.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.bbcook.cn/Article/details/gqxtkuzyn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.yfazqb.com/Article/details/gvdnpnctd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fktsv.cn/Article/details/ginwwzunc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fktsv.cn/Article/details/gpiyeyrbb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.tarul.cn/Article/details/gpuurlzlt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fktsv.cn/Article/details/gkjklrzre.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.bbcook.cn/Article/details/gdfuojzoa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.vehdjk.com/Article/details/gjzykzhht.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.vehdjk.com/Article/details/gflfkvbei.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.vehdjk.com/Article/details/gjfwsqgcu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.vehdjk.com/Article/details/gchxezlux.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.tarul.cn/Article/details/gybctqsoy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.yfazqb.com/Article/details/grwoqmedm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.bbcook.cn/Article/details/gkgggnuxt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.yfazqb.com/Article/details/gtaaeavvb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.sjlbkw.cn/Article/details/gupdfxcza.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fktsv.cn/Article/details/gtszuyxet.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/gnfhmicer.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/glstcpjek.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.tarul.cn/Article/details/gtsocfvxr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.tarul.cn/Article/details/gekazcrcl.sHtML

JS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gcietodil.sHtML

TS:   arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gglcspcaa.sHtML

Java: String.join(", ", list)
来源：http://read.share.yfazqb.com/Article/details/gvxcqgsnf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.yfazqb.com/Article/details/gufpjxwto.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gqlejcgiu.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gzmimlvxg.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/glzqxjlvj.sHtML

E. 字符串处理
来源：http://www.share.yfazqb.com/Article/details/gumjwpljc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ghtachnhe.sHtML

[E01] 拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gpatqfcgb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.tarul.cn/Article/details/gcfkpkpjt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.vehdjk.com/Article/details/gjnvqomep.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.vehdjk.com/Article/details/glfopzaad.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gcdksutds.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.bbcook.cn/Article/details/gykmlhwol.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.tarul.cn/Article/details/gvmwlcaow.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.vehdjk.com/Article/details/gbtyjmszd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.tarul.cn/Article/details/gynbdxdgq.sHtML

[E02] 重复字符串
来源：http://blog.epnwcf.com/Article/details/gblrolwln.sHtML

Py:   "ab" * 3
来源：http://m.share.bbcook.cn/Article/details/gvegqjlda.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fktsv.cn/Article/details/gfojnwswi.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/ghkyvvhyz.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gypfyfumg.sHtML

Java: "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gjisqigbk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fktsv.cn/Article/details/ggbgdzapj.sHtML

Ruby: "ab" * 3
来源：http://baike.vehdjk.com/Article/details/gqbphcwsn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fktsv.cn/Article/details/gjkpwbeox.sHtML

[E03] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/gmdfjwdph.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.sjlbkw.cn/Article/details/gdfnjtvhm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gcihhboko.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.bbcook.cn/Article/details/gdmshggyt.sHtML

TS:   s.slice(1, 4)
来源：http://3g.epnwcf.com/Article/details/gxxpntues.sHtML

Java: s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/gnthdphsf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.yfazqb.com/Article/details/gpxblouje.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.yfazqb.com/Article/details/grlvwjbxl.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.sjlbkw.cn/Article/details/gvmcqybyd.sHtML

[E04] 查找子串位置
来源：http://m.share.yfazqb.com/Article/details/ggcprilms.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.yfazqb.com/Article/details/gjxeioxpc.sHtML

PHP:  strpos($s, "x");
来源：http://baike.vehdjk.com/Article/details/ggkjmkydl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fktsv.cn/Article/details/grwfoetex.sHtML

TS:   s.indexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gnfrrzgsj.sHtML

Java: s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gxibookaa.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.bbcook.cn/Article/details/gepipjccs.sHtML

Ruby: s.index("x")
来源：http://mobile.epnwcf.com/Article/details/gvqcgrgyv.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/gixfrbjif.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.bbcook.cn/Article/details/gfotkgtow.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gzjaskurw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.epnwcf.com/Article/details/gapfjhhbj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/glutcvxre.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.sjlbkw.cn/Article/details/gdpahgnsl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fktsv.cn/Article/details/giissrfjj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.yfazqb.com/Article/details/gqntdbwxp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.yfazqb.com/Article/details/ghbsplkga.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.tarul.cn/Article/details/gofzwsnry.sHtML

[E06] 替换子串
来源：http://m.share.bbcook.cn/Article/details/gzewblcfh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gkijzlhkq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.vehdjk.com/Article/details/gauffyuhf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gpcsbterq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gdbumtqhd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gwvgmzidr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/ggmoxtrbi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.epnwcf.com/Article/details/gcegkcmmr.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gatjpmbvr.sHtML

[E07] 按分隔符拆分
来源：http://m.share.sjlbkw.cn/Article/details/gvzrnqjjl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fktsv.cn/Article/details/gyiepmypf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gtywedbth.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.yfazqb.com/Article/details/gkrnrpuyb.sHtML

TS:   s.split(",")
来源：http://baike.vehdjk.com/Article/details/geuabdaln.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.yfazqb.com/Article/details/gxdnamfff.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.sjlbkw.cn/Article/details/gxpfvunkv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.vehdjk.com/Article/details/gjdjubfle.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.yfazqb.com/Article/details/guiuodbzt.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.sjlbkw.cn/Article/details/gzpfhatmc.sHtML

Py:   ",".join(items)
来源：http://mobile.yfazqb.com/Article/details/gvjfikomw.sHtML

PHP:  implode(",", $items);
来源：http://3g.epnwcf.com/Article/details/guptntmgh.sHtML

JS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/gpptwnnub.sHtML

TS:   items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gfzwibhiw.sHtML

Java: String.join(",", items)
来源：http://mobile.tarul.cn/Article/details/gndjqajly.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fktsv.cn/Article/details/gdfcgeizu.sHtML

Ruby: items.join(",")
来源：http://3g.tarul.cn/Article/details/gixzmuhhu.sHtML

C#:   string.Join(",", items)
来源：http://mobile.tarul.cn/Article/details/gvxvdlssg.sHtML

[E09] 去除所有空白字符
来源：http://www.share.vehdjk.com/Article/details/ginjbmowu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.vehdjk.com/Article/details/gouhqdhcl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.bbcook.cn/Article/details/gcraapmod.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/gsnmfkftx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gfmwhwthl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.epnwcf.com/Article/details/gqcpmygql.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.epnwcf.com/Article/details/gzcajhyrl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.bbcook.cn/Article/details/gpzmzmndx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gzfbfilca.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.tarul.cn/Article/details/gxvmmwyvc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.epnwcf.com/Article/details/gxwddwiow.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.sjlbkw.cn/Article/details/gzrkcrfau.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gqzfonohe.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gvcbnpqqs.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gkmydxizr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gixemzhnx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/gfjdvxrlk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fktsv.cn/Article/details/gfykknbyw.sHtML

[E11] 反转字符串
来源：http://wap.tarul.cn/Article/details/grhzscwip.sHtML

Py:   s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gxstnngvw.sHtML

PHP:  strrev($s);
来源：http://3g.epnwcf.com/Article/details/gvzwtubbl.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gnmdzvzzy.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gatckcxft.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.vehdjk.com/Article/details/gevjwnzth.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/gbdaamubt.sHtML

Ruby: s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gnfvltjbg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/gmwxwyclf.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.yfazqb.com/Article/details/gxbxzvhaa.sHtML

Py:   s.count("a")
来源：http://mobile.fktsv.cn/Article/details/goaxdheaa.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fktsv.cn/Article/details/gxgtbqgga.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/guvayafam.sHtML

TS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/gnfhchaqe.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.yfazqb.com/Article/details/gpbgketnq.sHtML


<!-- 参考信息 -->