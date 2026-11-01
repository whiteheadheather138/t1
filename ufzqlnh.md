代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.yfazqb.com/Article/details/gqskbaaoz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/gpvoyakdn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gvelgwsnz.sHtML

[D06] 数组长度
来源：http://wap.sjlbkw.cn/Article/details/gshujwwte.sHtML

Py:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/gghxokznl.sHtML

PHP:  count($arr);
来源：http://mobile.epnwcf.com/Article/details/gmbaaiscm.sHtML

JS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/gwpvydqlm.sHtML

TS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/gkphewmcs.sHtML

Java: list.size();
来源：http://mobile.sjlbkw.cn/Article/details/gxubjwvoi.sHtML

Go:   len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gzzlalqqy.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.yfazqb.com/Article/details/gyohweqdr.sHtML

C#:   list.Count;
来源：http://www.share.tarul.cn/Article/details/gtctdtjmn.sHtML

[D07] 切片 / 取子数组
来源：http://wap.bbcook.cn/Article/details/gvnculkql.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.tarul.cn/Article/details/gxaxgoxar.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.sjlbkw.cn/Article/details/glpnbvchn.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gyusidbma.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/gfgnzjbvi.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gcehklaaw.sHtML

Go:   arr[1:4]
来源：http://www.m.share.vehdjk.com/Article/details/gsiidcfse.sHtML

Ruby: arr[1, 3]
来源：http://read.share.bbcook.cn/Article/details/gbpwaoznb.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.epnwcf.com/Article/details/gamtxjogj.sHtML

[D08] 合并两个数组
来源：http://www.m.share.sjlbkw.cn/Article/details/ggukstbbk.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.tarul.cn/Article/details/gmdlhiqsr.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fktsv.cn/Article/details/ggtfiqgbi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.sjlbkw.cn/Article/details/gizfkivid.sHtML

TS:   [...a, ...b];
来源：http://blog.fktsv.cn/Article/details/gupsdxdja.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.epnwcf.com/Article/details/gcefkwcjq.sHtML

Go:   append(a, b...)
来源：http://www.blog.tarul.cn/Article/details/grolthbco.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.tarul.cn/Article/details/gztsuxxvr.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.epnwcf.com/Article/details/gdxopopwm.sHtML

[D09] 排序（升序）
来源：http://read.share.vehdjk.com/Article/details/grdkiiwuf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/gggfxudmv.sHtML

PHP:  sort($arr);
来源：http://3g.yfazqb.com/Article/details/gefrsbgrq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.sjlbkw.cn/Article/details/gkkcmovhe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.epnwcf.com/Article/details/gskjnammb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.bbcook.cn/Article/details/gwofeieyn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/givekcocn.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gnolkftyp.sHtML

C#:   list.Sort();
来源：http://www.blog.vehdjk.com/Article/details/gjyqaukfd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.tarul.cn/Article/details/gwdbkphzf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.sjlbkw.cn/Article/details/gpyotqboe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.tarul.cn/Article/details/glkebhcbi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/gzunuotnk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fktsv.cn/Article/details/gvdlxesaw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.epnwcf.com/Article/details/glljgqprs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.sjlbkw.cn/Article/details/gsdbuybce.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.tarul.cn/Article/details/gqtqkzzom.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.vehdjk.com/Article/details/gnrvjkldz.sHtML

[D11] 反转数组
来源：http://baike.yfazqb.com/Article/details/ghmutcxsm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggaqlgrpb.sHtML

PHP:  array_reverse($arr);
来源：http://baike.yfazqb.com/Article/details/gbljnjuof.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.sjlbkw.cn/Article/details/gcinzmlxq.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fktsv.cn/Article/details/gwudschsu.sHtML

Java: Collections.reverse(list);
来源：http://m.share.tarul.cn/Article/details/grlxazakf.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.yfazqb.com/Article/details/gjkwndpmb.sHtML

Ruby: arr.reverse
来源：http://baike.epnwcf.com/Article/details/gipcysxwi.sHtML

C#:   list.Reverse();
来源：http://baike.sjlbkw.cn/Article/details/gefaxfybi.sHtML

[D12] 查找元素下标
来源：http://read.share.epnwcf.com/Article/details/gffbrjwlh.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.vehdjk.com/Article/details/gwvcjwryg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.epnwcf.com/Article/details/grjugcztd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.vehdjk.com/Article/details/gvsidypso.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gjmqdfrkm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.vehdjk.com/Article/details/guwpiatcz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gbrqpqrfd.sHtML

Ruby: arr.index(x)
来源：http://www.share.vehdjk.com/Article/details/grgndxcmn.sHtML

C#:   list.IndexOf(x);
来源：http://blog.bbcook.cn/Article/details/gnkjfeuts.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.bbcook.cn/Article/details/gchjkyarb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gvksdlkdh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fktsv.cn/Article/details/gyegovczf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.tarul.cn/Article/details/gyqphequo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/guamnrglu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.sjlbkw.cn/Article/details/gbalwyyri.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/gzwfrsyxu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.yfazqb.com/Article/details/gbyujlktp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.bbcook.cn/Article/details/gbxbrtdaj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fktsv.cn/Article/details/gghugpuai.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gymhmclvk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gwvwwyjsj.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/goabchyzt.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.tarul.cn/Article/details/grpwmkgbe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gspxgutjr.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/gjquexlkv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gymqzxwic.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.tarul.cn/Article/details/gfbrdlhzw.sHtML

[D15] 去重
来源：http://blog.fktsv.cn/Article/details/gvgbdxnxe.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gvsxdxwzs.sHtML

PHP:  array_unique($arr);
来源：http://blog.sjlbkw.cn/Article/details/gqkzszbkn.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/gxlqjskmo.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gxxmscnsc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.vehdjk.com/Article/details/gmrulqcsy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.vehdjk.com/Article/details/gleksaypi.sHtML

Ruby: arr.uniq
来源：http://www.blog.vehdjk.com/Article/details/gythxssjx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.tarul.cn/Article/details/giyajoahp.sHtML

[D16] 求和与平均值
来源：http://blog.bbcook.cn/Article/details/gcpmztsyd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gyedlbhza.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.vehdjk.com/Article/details/gfqngsozy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gcrhmypnl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gvxbwfbiw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.sjlbkw.cn/Article/details/gjteiatxy.sHtML

Go:   // 手写循环累加
来源：http://blog.yfazqb.com/Article/details/gjtvopchn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.vehdjk.com/Article/details/grxblqqke.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.tarul.cn/Article/details/gmblaetqs.sHtML

[D17] 最大值与最小值
来源：http://mobile.epnwcf.com/Article/details/gxuhtjeem.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.epnwcf.com/Article/details/goyiipehv.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.vehdjk.com/Article/details/gvrgzffuq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fktsv.cn/Article/details/gnzdkvpmp.sHtML

TS:   Math.max(...arr);
来源：http://mobile.tarul.cn/Article/details/gaednbirg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.epnwcf.com/Article/details/gehudzbkd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.sjlbkw.cn/Article/details/givhkjhab.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.sjlbkw.cn/Article/details/gpmoauvdp.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fktsv.cn/Article/details/gxdgyvrtg.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.epnwcf.com/Article/details/grxzwkybn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxxijanr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.vehdjk.com/Article/details/gewscajqs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.vehdjk.com/Article/details/gtyflhdod.sHtML

TS:   nested.flat();
来源：http://read.share.epnwcf.com/Article/details/grwjnxsrj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.bbcook.cn/Article/details/gsxzykmyf.sHtML

Go:   // 手写双层循环
来源：http://baike.yfazqb.com/Article/details/gqjklykcq.sHtML

Ruby: nested.flatten
来源：http://blog.epnwcf.com/Article/details/ganxzbhfe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.vehdjk.com/Article/details/gtrevflfp.sHtML

[D19] 按字段分组
来源：http://wap.sjlbkw.cn/Article/details/gedrllqgj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.yfazqb.com/Article/details/gpvqfuezc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fktsv.cn/Article/details/glsttvprq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzrqldnc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/gdneezkgq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.vehdjk.com/Article/details/gsbvqqkam.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.bbcook.cn/Article/details/gddoagdqb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.bbcook.cn/Article/details/gzetwijxu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.bbcook.cn/Article/details/gsupomubi.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.bbcook.cn/Article/details/gwemxbkiy.sHtML

Py:   Counter(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gzzuaosjs.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gdvzblfrt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gfhsphhqn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/ghgagepgr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.sjlbkw.cn/Article/details/gqazteunp.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.vehdjk.com/Article/details/gahxnfplk.sHtML

Ruby: arr.tally
来源：http://mobile.tarul.cn/Article/details/gicigpldo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.bbcook.cn/Article/details/gkfenfznx.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.sjlbkw.cn/Article/details/ggyjoured.sHtML

Py:   x in arr
来源：http://read.share.fktsv.cn/Article/details/gjvkbjkdr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.yfazqb.com/Article/details/gqwphglxs.sHtML

JS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gvuyckzvz.sHtML

TS:   arr.includes(x)
来源：http://wap.vehdjk.com/Article/details/gwbsxasai.sHtML

Java: list.contains(x)
来源：http://mobile.fktsv.cn/Article/details/gbshststn.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.tarul.cn/Article/details/gvjehkumu.sHtML

Ruby: arr.include?(x)
来源：http://mobile.yfazqb.com/Article/details/gwigtklvl.sHtML

C#:   list.Contains(x)
来源：http://www.share.tarul.cn/Article/details/goudnuhbu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.epnwcf.com/Article/details/gkenjztrc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.tarul.cn/Article/details/glaycyxob.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.vehdjk.com/Article/details/gfctgtmvn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fktsv.cn/Article/details/gdrcorvok.sHtML

TS:   [...arr];
来源：http://www.share.sjlbkw.cn/Article/details/ghsfdiago.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fktsv.cn/Article/details/gjwwxicvj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.bbcook.cn/Article/details/givdtdqum.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.vehdjk.com/Article/details/ggvrhmlir.sHtML

C#:   new List<int>(list);
来源：http://m.share.vehdjk.com/Article/details/gwceiewgn.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.bbcook.cn/Article/details/gijcaelfh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fktsv.cn/Article/details/glvvwzbvs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gefkzgtzu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/ggebauhrm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gnvgtnghd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.bbcook.cn/Article/details/gmtnmlobm.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gydfymdta.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.bbcook.cn/Article/details/gbwdajrgk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.vehdjk.com/Article/details/gmtfyjspp.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.tarul.cn/Article/details/grnhgaixe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.yfazqb.com/Article/details/gbgphvhtr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.epnwcf.com/Article/details/gqarlvgia.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.yfazqb.com/Article/details/ghbpucedw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.tarul.cn/Article/details/guyhrisok.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gleepvbgl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.yfazqb.com/Article/details/gexvcxjgj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.yfazqb.com/Article/details/gztczucgk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fktsv.cn/Article/details/ggjhtwqtw.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.bbcook.cn/Article/details/giyvhycci.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.yfazqb.com/Article/details/galaznsbj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.tarul.cn/Article/details/gynijplvd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.bbcook.cn/Article/details/gctgenogs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fktsv.cn/Article/details/glfuxpslh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fktsv.cn/Article/details/gokbyvpmb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.epnwcf.com/Article/details/gthstrwvy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.vehdjk.com/Article/details/gsqzhomgi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.sjlbkw.cn/Article/details/gnwbvkpdl.sHtML

[D26] 数组转字符串
来源：http://read.share.fktsv.cn/Article/details/gbkqjeuji.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fktsv.cn/Article/details/gukfkmphj.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gvbgrxlit.sHtML

JS:   arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gmdpmgjdk.sHtML

TS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/grqbltfex.sHtML

Java: String.join(", ", list)
来源：http://3g.tarul.cn/Article/details/gkbttcrct.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.tarul.cn/Article/details/gvlkugbji.sHtML

Ruby: arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gsatjokvi.sHtML

C#:   string.Join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gvlxbvpuw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvjvqfaaj.sHtML

E. 字符串处理
来源：http://read.share.fktsv.cn/Article/details/gupurwwtj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gauonjxoz.sHtML

[E01] 拼接字符串
来源：http://wap.epnwcf.com/Article/details/gkqptcmoi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.bbcook.cn/Article/details/gbdnuirem.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.tarul.cn/Article/details/gflvenfpu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/gxqacxzgg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/gqhxbkdrc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.bbcook.cn/Article/details/gsibjecau.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fktsv.cn/Article/details/gcyrronal.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.sjlbkw.cn/Article/details/gbhfofzxc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gcheqrzxq.sHtML

[E02] 重复字符串
来源：http://read.share.fktsv.cn/Article/details/gaohleqeb.sHtML

Py:   "ab" * 3
来源：http://mobile.fktsv.cn/Article/details/goaibflrs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.tarul.cn/Article/details/gvnudxkvt.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gfkahttft.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gshhixuze.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gcgzlnldz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.bbcook.cn/Article/details/gqunlitgz.sHtML

Ruby: "ab" * 3
来源：http://wap.fktsv.cn/Article/details/gwbeficpo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/gqyadqgub.sHtML

[E03] 截取子串
来源：http://baike.tarul.cn/Article/details/gjadtfsfs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwocndrz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gfihabbeo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/glcxdfqji.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fktsv.cn/Article/details/gwlbwpajl.sHtML

Java: s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/giwrxbono.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gvjyllokc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.yfazqb.com/Article/details/giulzdhoa.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.yfazqb.com/Article/details/gjngjmfqq.sHtML

[E04] 查找子串位置
来源：http://blog.sjlbkw.cn/Article/details/gbffqrnqj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.bbcook.cn/Article/details/gvuldtbdc.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.bbcook.cn/Article/details/guxqiaglk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.vehdjk.com/Article/details/gfsplxops.sHtML

TS:   s.indexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gcpdhuers.sHtML

Java: s.indexOf("x")
来源：http://3g.fktsv.cn/Article/details/gmlxkxvur.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.sjlbkw.cn/Article/details/gbbhwrocz.sHtML

Ruby: s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gxaelrtom.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gnnpidxgo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fktsv.cn/Article/details/gwxxlpmyd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.vehdjk.com/Article/details/gzpwqilkd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.epnwcf.com/Article/details/givwwrfya.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/gcqgdzkkm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.vehdjk.com/Article/details/gkwdsisar.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.bbcook.cn/Article/details/gspqnwurm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.epnwcf.com/Article/details/gijstgkar.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.bbcook.cn/Article/details/ghfyesumb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.vehdjk.com/Article/details/ghetxnxpy.sHtML

[E06] 替换子串
来源：http://m.share.fktsv.cn/Article/details/gumavfbdj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.bbcook.cn/Article/details/gopsfuuyt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fktsv.cn/Article/details/gkrtbcjqp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpdbijex.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/goaitbhio.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gfuojsbbl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.vehdjk.com/Article/details/gojfiqsap.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gcrlhnqux.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gjlfzxobp.sHtML

[E07] 按分隔符拆分
来源：http://3g.fktsv.cn/Article/details/gjrbigsml.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.sjlbkw.cn/Article/details/gfzqhyfrc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gyrwgkamn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.bbcook.cn/Article/details/gqtgogdzs.sHtML

TS:   s.split(",")
来源：http://www.m.share.bbcook.cn/Article/details/gzojmvzpw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.yfazqb.com/Article/details/gabkzwfco.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.vehdjk.com/Article/details/guiunssql.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.epnwcf.com/Article/details/gcggepukc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.vehdjk.com/Article/details/gpwvjaygp.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.epnwcf.com/Article/details/girkepuuu.sHtML

Py:   ",".join(items)
来源：http://baike.fktsv.cn/Article/details/geddiavgu.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.tarul.cn/Article/details/gkbygkcac.sHtML

JS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/gkthrcctj.sHtML

TS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/gaznlhkxc.sHtML

Java: String.join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/gmwnzmjpe.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.vehdjk.com/Article/details/gtbawyhjs.sHtML

Ruby: items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/guxtcmhod.sHtML

C#:   string.Join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gwjsxuwmr.sHtML

[E09] 去除所有空白字符
来源：http://3g.fktsv.cn/Article/details/gwakqjjzx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.epnwcf.com/Article/details/gffvmjghi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.bbcook.cn/Article/details/gweysjzaj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/gphnuloyo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gilawapdb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.tarul.cn/Article/details/gaovoymov.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtsmxypc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.vehdjk.com/Article/details/gzeezlatt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/geamllpzi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.bbcook.cn/Article/details/gaklijeeg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gmxgpqewq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.tarul.cn/Article/details/gaiybbktg.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/godyxzcyw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gjqgdqubx.sHtML

Java: String.format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/glrdbaatx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/ggagcsgpz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gcbvbowzl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.bbcook.cn/Article/details/gvejcafup.sHtML

[E11] 反转字符串
来源：http://www.blog.vehdjk.com/Article/details/gmtpttaxl.sHtML

Py:   s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gejpeufgc.sHtML

PHP:  strrev($s);
来源：http://read.share.tarul.cn/Article/details/glfacrswz.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/guakqtpmn.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gzvmpeecx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.tarul.cn/Article/details/grtnfbqsl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gomjbmsyp.sHtML

Ruby: s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gaaxbjotc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/gyqrdacfb.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fktsv.cn/Article/details/gioyihnew.sHtML

Py:   s.count("a")
来源：http://wap.epnwcf.com/Article/details/gxdqkuwtv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.vehdjk.com/Article/details/gprwijnpa.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/gspuhgttz.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/ghyatdyun.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.yfazqb.com/Article/details/gmnymnijc.sHtML


<!-- 参考信息 -->