代发 wailian999

[D03] 在指定位置插入元素
来源：http://blog.vehdjk.com/Article/details/gkaspnack.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gxmciavrf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.tarul.cn/Article/details/gvnddghoe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.bbcook.cn/Article/details/gzgacqfui.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.tarul.cn/Article/details/gpqpzpukw.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gumvuhgua.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/glsgcvswl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.epnwcf.com/Article/details/gpoidkdqv.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gdkhfrwhs.sHtML

[D04] 删除元素
来源：http://3g.fktsv.cn/Article/details/gaoxrjoie.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.bbcook.cn/Article/details/gqjxaodlc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.tarul.cn/Article/details/gtriqmxxv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.tarul.cn/Article/details/gphoajoin.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.vehdjk.com/Article/details/gphfsgvld.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.sjlbkw.cn/Article/details/gxetqcrey.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.vehdjk.com/Article/details/gzxonwriw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.tarul.cn/Article/details/geemcmiqi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fktsv.cn/Article/details/gktwfioug.sHtML

[D05] 访问与修改元素
来源：http://mobile.bbcook.cn/Article/details/gjccrwkyq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gatyjuvxz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.tarul.cn/Article/details/gptuqqjqb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gmboczvrd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fktsv.cn/Article/details/grslrulcq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fktsv.cn/Article/details/grsqztqed.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gfkewbajy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/glkggbwkg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gypymkptt.sHtML

[D06] 数组长度
来源：http://mobile.epnwcf.com/Article/details/gjyutpnsm.sHtML

Py:   len(arr)
来源：http://www.share.yfazqb.com/Article/details/gcvnrzihh.sHtML

PHP:  count($arr);
来源：http://baike.sjlbkw.cn/Article/details/gdhasogkl.sHtML

JS:   arr.length
来源：http://baike.tarul.cn/Article/details/ggsiduujg.sHtML

TS:   arr.length
来源：http://www.m.share.fktsv.cn/Article/details/gxqnfuszp.sHtML

Java: list.size();
来源：http://baike.fktsv.cn/Article/details/gtcllqsof.sHtML

Go:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/ghjwqwijp.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.vehdjk.com/Article/details/gzohnfpew.sHtML

C#:   list.Count;
来源：http://www.m.share.yfazqb.com/Article/details/grqytcfzm.sHtML

[D07] 切片 / 取子数组
来源：http://3g.epnwcf.com/Article/details/gwivuxiqc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.tarul.cn/Article/details/gvneonjhh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.epnwcf.com/Article/details/gkpkzvuao.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fktsv.cn/Article/details/gedmkfnnu.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/glifuabaz.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gvftdegug.sHtML

Go:   arr[1:4]
来源：http://www.blog.vehdjk.com/Article/details/gixqyjshg.sHtML

Ruby: arr[1, 3]
来源：http://blog.fktsv.cn/Article/details/gvdnjhrtx.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.epnwcf.com/Article/details/gahgrnsox.sHtML

[D08] 合并两个数组
来源：http://wap.vehdjk.com/Article/details/ghlbpdymm.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.yfazqb.com/Article/details/gbvkkbpdu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fktsv.cn/Article/details/ggissqvzz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.bbcook.cn/Article/details/gowxopyqa.sHtML

TS:   [...a, ...b];
来源：http://www.blog.tarul.cn/Article/details/gwxwpijnf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.bbcook.cn/Article/details/ggqbwnjcc.sHtML

Go:   append(a, b...)
来源：http://wap.sjlbkw.cn/Article/details/givzenlpt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.tarul.cn/Article/details/gsggzsicp.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gclcippkv.sHtML

[D09] 排序（升序）
来源：http://www.blog.fktsv.cn/Article/details/gsehatyee.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gpyeqgqzq.sHtML

PHP:  sort($arr);
来源：http://m.share.yfazqb.com/Article/details/gfopguqed.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.vehdjk.com/Article/details/gbkooglhi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gngxrepdf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.tarul.cn/Article/details/gyynhxgzo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gvxhwypmh.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/gbrqdzrup.sHtML

C#:   list.Sort();
来源：http://www.share.tarul.cn/Article/details/gagmkqjtu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.tarul.cn/Article/details/gjqpfndyx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.vehdjk.com/Article/details/geggqdlqc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.yfazqb.com/Article/details/gipxkflfv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fktsv.cn/Article/details/gdcmjowqs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.epnwcf.com/Article/details/gexaqrexo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fktsv.cn/Article/details/gzkxojrpp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.bbcook.cn/Article/details/gqcagqylc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.tarul.cn/Article/details/gocxjabms.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.tarul.cn/Article/details/gksabijeg.sHtML

[D11] 反转数组
来源：http://read.share.tarul.cn/Article/details/grfqvuwrx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.tarul.cn/Article/details/gvklpfyao.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.yfazqb.com/Article/details/ggzwxzgvw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fktsv.cn/Article/details/gknlvzmcu.sHtML

TS:   [...arr].reverse();
来源：http://wap.tarul.cn/Article/details/gixfkbmsq.sHtML

Java: Collections.reverse(list);
来源：http://wap.sjlbkw.cn/Article/details/gxilruvyf.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gaagrdgve.sHtML

Ruby: arr.reverse
来源：http://mobile.tarul.cn/Article/details/geelnnxce.sHtML

C#:   list.Reverse();
来源：http://blog.yfazqb.com/Article/details/gdoeuwjce.sHtML

[D12] 查找元素下标
来源：http://baike.yfazqb.com/Article/details/gfskntpcf.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.tarul.cn/Article/details/gkvrkpkkv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gzipgpxti.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gcdfnowsr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/gwwohwjit.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.vehdjk.com/Article/details/gblrxibgv.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gopfnkewq.sHtML

Ruby: arr.index(x)
来源：http://m.share.tarul.cn/Article/details/gkicgdaid.sHtML

C#:   list.IndexOf(x);
来源：http://blog.vehdjk.com/Article/details/gmhpzukko.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.sjlbkw.cn/Article/details/gkzgrrsev.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.tarul.cn/Article/details/gdtzdbbvx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.vehdjk.com/Article/details/gptoobzzb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gvhycehyo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/gcjyqwjtl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.bbcook.cn/Article/details/gcftynxcz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/giuhbcgib.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fktsv.cn/Article/details/gmljgridc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.bbcook.cn/Article/details/gbhiqtvcd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.yfazqb.com/Article/details/gaozxgygg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.vehdjk.com/Article/details/gkgfwvemn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.bbcook.cn/Article/details/gybprukeq.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.sjlbkw.cn/Article/details/gsswikzgi.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.bbcook.cn/Article/details/gloobnfyq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fktsv.cn/Article/details/gunopridj.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/gkwnhxnzj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.yfazqb.com/Article/details/gmzqazmow.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.yfazqb.com/Article/details/grecqpezf.sHtML

[D15] 去重
来源：http://3g.fktsv.cn/Article/details/gyzfcfoyo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.yfazqb.com/Article/details/gsargauzo.sHtML

PHP:  array_unique($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gkpsrtgem.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gdkatkijy.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/giaszocil.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fktsv.cn/Article/details/grozgfflg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.bbcook.cn/Article/details/glorljbrb.sHtML

Ruby: arr.uniq
来源：http://baike.yfazqb.com/Article/details/gpfqydzws.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.vehdjk.com/Article/details/gzdijmgxi.sHtML

[D16] 求和与平均值
来源：http://read.share.fktsv.cn/Article/details/gvqwjunig.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fktsv.cn/Article/details/gpyujrypy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.tarul.cn/Article/details/gmxpqhfsv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fktsv.cn/Article/details/gisqwftjn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gwovuengg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.yfazqb.com/Article/details/gacwwhvbi.sHtML

Go:   // 手写循环累加
来源：http://mobile.sjlbkw.cn/Article/details/gmapguzud.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fktsv.cn/Article/details/gjlsortht.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.yfazqb.com/Article/details/gyybkymph.sHtML

[D17] 最大值与最小值
来源：http://baike.vehdjk.com/Article/details/ghmuupuwi.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.bbcook.cn/Article/details/gnsltxlyg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.epnwcf.com/Article/details/gmsaidnqx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.vehdjk.com/Article/details/gshfxhmvx.sHtML

TS:   Math.max(...arr);
来源：http://baike.epnwcf.com/Article/details/golxomlav.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.tarul.cn/Article/details/gbeefnefn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.vehdjk.com/Article/details/goqtcgxyj.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.bbcook.cn/Article/details/gfouanuqe.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.vehdjk.com/Article/details/gognamcea.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.epnwcf.com/Article/details/gwxugxtrw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.vehdjk.com/Article/details/glbsnwbfk.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.sjlbkw.cn/Article/details/gxbstnoxa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.sjlbkw.cn/Article/details/gnqhfvjcs.sHtML

TS:   nested.flat();
来源：http://baike.epnwcf.com/Article/details/gnhcnxwfv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.tarul.cn/Article/details/gzblgtpph.sHtML

Go:   // 手写双层循环
来源：http://www.share.yfazqb.com/Article/details/gfqpccdtx.sHtML

Ruby: nested.flatten
来源：http://wap.sjlbkw.cn/Article/details/gsgqjupnw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.bbcook.cn/Article/details/gdvzcfzfl.sHtML

[D19] 按字段分组
来源：http://baike.sjlbkw.cn/Article/details/gtthgcmvv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.sjlbkw.cn/Article/details/gpqtndwjm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.bbcook.cn/Article/details/gdgotwtyz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.bbcook.cn/Article/details/gqhnhefeb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gzmjuevhe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fktsv.cn/Article/details/gzlfhkkri.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fktsv.cn/Article/details/gkflvplgo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.vehdjk.com/Article/details/geccxnpdf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.tarul.cn/Article/details/gielkmrbn.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.vehdjk.com/Article/details/gsjuskbew.sHtML

Py:   Counter(arr)
来源：http://www.share.vehdjk.com/Article/details/gjkqvqsbc.sHtML

PHP:  array_count_values($arr);
来源：http://wap.yfazqb.com/Article/details/gzflyrdde.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gspapeeip.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gchdchpho.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fktsv.cn/Article/details/gfyohiqur.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.sjlbkw.cn/Article/details/guetcofot.sHtML

Ruby: arr.tally
来源：http://mobile.bbcook.cn/Article/details/gwtuwkgpn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fktsv.cn/Article/details/gvtkujwvc.sHtML

[D21] 判断是否包含某元素
来源：http://wap.epnwcf.com/Article/details/gzdepgsvr.sHtML

Py:   x in arr
来源：http://3g.vehdjk.com/Article/details/gaqriwbqb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.tarul.cn/Article/details/gogufnovy.sHtML

JS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gtylojiic.sHtML

TS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/ganhmxkyb.sHtML

Java: list.contains(x)
来源：http://wap.vehdjk.com/Article/details/gpaesdicz.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.bbcook.cn/Article/details/gujuadzpl.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gdjjqtaor.sHtML

C#:   list.Contains(x)
来源：http://baike.epnwcf.com/Article/details/gtwxuzhoy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.vehdjk.com/Article/details/gpevjhydl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.vehdjk.com/Article/details/gbmafqjbr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.bbcook.cn/Article/details/gftpwdlgn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.sjlbkw.cn/Article/details/glniedppc.sHtML

TS:   [...arr];
来源：http://baike.bbcook.cn/Article/details/gldibbwzg.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.tarul.cn/Article/details/gzoosmqcu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.sjlbkw.cn/Article/details/ggsakfitq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.epnwcf.com/Article/details/gkjdemnjj.sHtML

C#:   new List<int>(list);
来源：http://www.share.epnwcf.com/Article/details/geppbbxln.sHtML

[D23] reduce 累积计算
来源：http://m.share.bbcook.cn/Article/details/gixsndanm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fktsv.cn/Article/details/gwjarkeke.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.tarul.cn/Article/details/gabyibcaa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.epnwcf.com/Article/details/goqmzrbyj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gnwgrlmjt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.bbcook.cn/Article/details/grrqykqwr.sHtML

Go:   // 手写循环
来源：http://blog.yfazqb.com/Article/details/gqxaobmtg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.epnwcf.com/Article/details/genlrmqbz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fktsv.cn/Article/details/gunbkyjys.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.epnwcf.com/Article/details/gbqgqxsxi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.epnwcf.com/Article/details/gxhfofbey.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.yfazqb.com/Article/details/gdqpsmagw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.yfazqb.com/Article/details/gserbavpo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.vehdjk.com/Article/details/gravgiluk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.yfazqb.com/Article/details/ggieqtzod.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.bbcook.cn/Article/details/geychgiss.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.epnwcf.com/Article/details/gewermpef.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.sjlbkw.cn/Article/details/grzhkypom.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.sjlbkw.cn/Article/details/gjbiqjkbl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/ggearwckk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fktsv.cn/Article/details/gdiewgbvi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.tarul.cn/Article/details/ghvbglrxn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.yfazqb.com/Article/details/gosqjcvpp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.sjlbkw.cn/Article/details/guckpfdsn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.epnwcf.com/Article/details/gakkvsnfx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkaillik.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.epnwcf.com/Article/details/gyxbchehr.sHtML

[D26] 数组转字符串
来源：http://read.share.tarul.cn/Article/details/gnwzfwzxm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.bbcook.cn/Article/details/gmznobsmc.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.tarul.cn/Article/details/gdqlionxp.sHtML

JS:   arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/ghfeiuspb.sHtML

TS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/ggnmzglya.sHtML

Java: String.join(", ", list)
来源：http://baike.vehdjk.com/Article/details/gtrdiafzx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.yfazqb.com/Article/details/gjrqnrvya.sHtML

Ruby: arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/ggqwwmxlo.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/gdzsnjokc.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ghqgljpxz.sHtML

E. 字符串处理
来源：http://blog.fktsv.cn/Article/details/gmlprewej.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gavrtxggs.sHtML

[E01] 拼接字符串
来源：http://baike.tarul.cn/Article/details/gvifmfnlh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.sjlbkw.cn/Article/details/gbdqozehw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.vehdjk.com/Article/details/gvzwjshqu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/gjdjdtkrt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gfzzqbkpw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.bbcook.cn/Article/details/gwymtbnrd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.epnwcf.com/Article/details/gztxwjylk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.vehdjk.com/Article/details/gakarhfkf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gsgrjssva.sHtML

[E02] 重复字符串
来源：http://wap.sjlbkw.cn/Article/details/gamdvmzzy.sHtML

Py:   "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gwegjdvsg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.sjlbkw.cn/Article/details/gymcuvsnd.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gfjckyznn.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gnlgncwnc.sHtML

Java: "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gunnskplp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.yfazqb.com/Article/details/gbenpurzr.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fktsv.cn/Article/details/grvjcrzvy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fktsv.cn/Article/details/gbrgvbmlh.sHtML

[E03] 截取子串
来源：http://baike.vehdjk.com/Article/details/gvfsvhcjx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fktsv.cn/Article/details/gkutmzwhw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gyamyrbfl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gaashrxbx.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gmivmlpul.sHtML

Java: s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/ggxpfbmao.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gbxnhrdnv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.sjlbkw.cn/Article/details/gbxaymawh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.yfazqb.com/Article/details/gbqjzsfat.sHtML

[E04] 查找子串位置
来源：http://baike.vehdjk.com/Article/details/gixsfakev.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/gpreiavlw.sHtML

PHP:  strpos($s, "x");
来源：http://3g.epnwcf.com/Article/details/gatjjnvok.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fktsv.cn/Article/details/gxodzdcvx.sHtML

TS:   s.indexOf("x")
来源：http://blog.yfazqb.com/Article/details/gghisopdd.sHtML

Java: s.indexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gzhpjojoz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fktsv.cn/Article/details/gwpzvtzce.sHtML

Ruby: s.index("x")
来源：http://3g.fktsv.cn/Article/details/gcyvejkqy.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gcsdhqyfx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.tarul.cn/Article/details/gbwwkxjrd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.bbcook.cn/Article/details/gdxyetrhr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.bbcook.cn/Article/details/gztyhsvqr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gtlhpzhgh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.tarul.cn/Article/details/gnmhbnbqc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gecauyuuk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.sjlbkw.cn/Article/details/gqxkveyqt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.vehdjk.com/Article/details/gmhrckcpw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.bbcook.cn/Article/details/gujrlubhp.sHtML

[E06] 替换子串
来源：http://blog.yfazqb.com/Article/details/gjyfjcbhr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.tarul.cn/Article/details/geemgwdxe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.sjlbkw.cn/Article/details/gqnlmkfqn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/ghvnzrzag.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/guuqhkndb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gvqkgtnfq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gknbatzhh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.vehdjk.com/Article/details/goeimuakb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gaxzoweef.sHtML

[E07] 按分隔符拆分
来源：http://wap.epnwcf.com/Article/details/gnsxuwinr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.sjlbkw.cn/Article/details/gpczkayvy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.yfazqb.com/Article/details/gwroymdns.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fktsv.cn/Article/details/gmbqddqis.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/gnlzafpti.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.epnwcf.com/Article/details/gfjkfraqf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fktsv.cn/Article/details/gafeilhrb.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.sjlbkw.cn/Article/details/gbuufbofr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.epnwcf.com/Article/details/gnztawdsc.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.yfazqb.com/Article/details/gopcjitzv.sHtML

Py:   ",".join(items)
来源：http://3g.epnwcf.com/Article/details/gchpxjciq.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fktsv.cn/Article/details/gospkjtgl.sHtML

JS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gixcfrshk.sHtML

TS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gqcngbyae.sHtML

Java: String.join(",", items)
来源：http://mobile.fktsv.cn/Article/details/gquflchxk.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.bbcook.cn/Article/details/ghimtcmzk.sHtML

Ruby: items.join(",")
来源：http://baike.epnwcf.com/Article/details/gzvavlzqt.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/ggimeqzng.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.tarul.cn/Article/details/ggeuuyqhb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.tarul.cn/Article/details/gjpdhfhpr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.vehdjk.com/Article/details/gyroysama.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gsaeongsb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gwiljdypu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.epnwcf.com/Article/details/gsekyvbzp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.epnwcf.com/Article/details/gkdslazft.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.tarul.cn/Article/details/grhohxomu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fktsv.cn/Article/details/gxphykaye.sHtML


<!-- 参考信息 -->