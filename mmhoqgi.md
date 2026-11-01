代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/glcqearwi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gitsmcrnk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/gksqhhfdf.sHtML

[D06] 数组长度
来源：http://www.share.tarul.cn/Article/details/gjulcemkb.sHtML

Py:   len(arr)
来源：http://mobile.tarul.cn/Article/details/gvdjrcjzx.sHtML

PHP:  count($arr);
来源：http://www.blog.fktsv.cn/Article/details/gugytclti.sHtML

JS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/gaslsxgon.sHtML

TS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/gzafbgaeu.sHtML

Java: list.size();
来源：http://m.share.bbcook.cn/Article/details/gjuoejskg.sHtML

Go:   len(arr)
来源：http://baike.epnwcf.com/Article/details/gimpdnqji.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.tarul.cn/Article/details/gdihvscup.sHtML

C#:   list.Count;
来源：http://3g.yfazqb.com/Article/details/gmcasljpy.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.sjlbkw.cn/Article/details/gzzcdeiyt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.vehdjk.com/Article/details/gqooosgmu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.vehdjk.com/Article/details/gobprdpuo.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/geybahlyh.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/gwlkriaod.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/gknaxcqsw.sHtML

Go:   arr[1:4]
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbmscoot.sHtML

Ruby: arr[1, 3]
来源：http://3g.vehdjk.com/Article/details/gyuhqplta.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.epnwcf.com/Article/details/gfrptsujp.sHtML

[D08] 合并两个数组
来源：http://blog.sjlbkw.cn/Article/details/gozgbxwtl.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.tarul.cn/Article/details/gfyozyacn.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.sjlbkw.cn/Article/details/goeyyjney.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.yfazqb.com/Article/details/gpcpbmifc.sHtML

TS:   [...a, ...b];
来源：http://read.share.tarul.cn/Article/details/gzyjztvtn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.tarul.cn/Article/details/gelpifyqd.sHtML

Go:   append(a, b...)
来源：http://mobile.sjlbkw.cn/Article/details/ghfkgnrwi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.sjlbkw.cn/Article/details/gxyazqwkg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gyyumnoip.sHtML

[D09] 排序（升序）
来源：http://www.m.share.epnwcf.com/Article/details/geqxusnzr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.bbcook.cn/Article/details/gwzfewbuf.sHtML

PHP:  sort($arr);
来源：http://blog.sjlbkw.cn/Article/details/gzuchjhoo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.bbcook.cn/Article/details/gczftdjuz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjldmdgpc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fktsv.cn/Article/details/gsmsqyejq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.vehdjk.com/Article/details/gwpthhgfg.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/gomsendnh.sHtML

C#:   list.Sort();
来源：http://baike.vehdjk.com/Article/details/gemozdiig.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.epnwcf.com/Article/details/gffnrurzi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.vehdjk.com/Article/details/gawzchoak.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/grwrklwic.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fktsv.cn/Article/details/gedmwcfzt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.tarul.cn/Article/details/gwwknlguu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.vehdjk.com/Article/details/goxgjubjg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.sjlbkw.cn/Article/details/ginzfzfex.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.vehdjk.com/Article/details/gntlntsmx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.epnwcf.com/Article/details/gwduzhyzv.sHtML

[D11] 反转数组
来源：http://read.share.tarul.cn/Article/details/gfznosinn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.tarul.cn/Article/details/gpcwmrryz.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.bbcook.cn/Article/details/gcstsohdf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.epnwcf.com/Article/details/gtjqcrvkn.sHtML

TS:   [...arr].reverse();
来源：http://3g.tarul.cn/Article/details/ghsvczbig.sHtML

Java: Collections.reverse(list);
来源：http://m.share.vehdjk.com/Article/details/gtbsdcfox.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.yfazqb.com/Article/details/gvnharnvq.sHtML

Ruby: arr.reverse
来源：http://baike.fktsv.cn/Article/details/gwnouayzo.sHtML

C#:   list.Reverse();
来源：http://read.share.tarul.cn/Article/details/gorfyacro.sHtML

[D12] 查找元素下标
来源：http://www.m.share.vehdjk.com/Article/details/gnuvqfdkd.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.vehdjk.com/Article/details/gnrzfflui.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.bbcook.cn/Article/details/gngymztoy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gysfenjfe.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.epnwcf.com/Article/details/gqbuqiyen.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.bbcook.cn/Article/details/gvhckftys.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gjcgrwrbr.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.bbcook.cn/Article/details/gsacfenqi.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.yfazqb.com/Article/details/gceazwuzn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.epnwcf.com/Article/details/gkqsadxyn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gjvmxouwy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.bbcook.cn/Article/details/gatyedbhh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fktsv.cn/Article/details/gpnsiswrw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/gcecvwlvn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.vehdjk.com/Article/details/gmliyjwrj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.sjlbkw.cn/Article/details/gcnpnfpeq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.vehdjk.com/Article/details/gqcxmxkgg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.bbcook.cn/Article/details/gyhjcrszz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.vehdjk.com/Article/details/gaopbmpjw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gccbrurvc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.epnwcf.com/Article/details/gxutkbciz.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/glenkiraq.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.bbcook.cn/Article/details/gnebzqesm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.yfazqb.com/Article/details/ghxymuffd.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/gxulkhlis.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gdnoeshmw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gkqfktdia.sHtML

[D15] 去重
来源：http://3g.epnwcf.com/Article/details/gqoczykva.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.vehdjk.com/Article/details/gngwsoecl.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/gcpezuuup.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/gjwlwvwku.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/gmwcqyfop.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fktsv.cn/Article/details/ggppofucl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.yfazqb.com/Article/details/gboqdledc.sHtML

Ruby: arr.uniq
来源：http://blog.epnwcf.com/Article/details/gjjfnmblk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.tarul.cn/Article/details/gfwslboya.sHtML

[D16] 求和与平均值
来源：http://www.m.share.bbcook.cn/Article/details/gxcoeizfm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/glrftxezl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fktsv.cn/Article/details/gqktnoebj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gtkqcsudg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/ggxyehyzr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.yfazqb.com/Article/details/gjuaqufvl.sHtML

Go:   // 手写循环累加
来源：http://3g.fktsv.cn/Article/details/gevwdnmet.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.vehdjk.com/Article/details/glhkevgef.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.sjlbkw.cn/Article/details/gfhyhbusa.sHtML

[D17] 最大值与最小值
来源：http://www.blog.yfazqb.com/Article/details/gsaxaqldq.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.epnwcf.com/Article/details/ghdciwaow.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.sjlbkw.cn/Article/details/gygfsakcd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fktsv.cn/Article/details/gbapnfeuk.sHtML

TS:   Math.max(...arr);
来源：http://mobile.bbcook.cn/Article/details/gkcmbzura.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.yfazqb.com/Article/details/gvehbmxut.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/gqdmmxrdq.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.sjlbkw.cn/Article/details/gzemrjkfd.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.tarul.cn/Article/details/gowsexvax.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.vehdjk.com/Article/details/gqkuyiiwt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fktsv.cn/Article/details/gtotvwzgp.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.yfazqb.com/Article/details/gvlpjpnnw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.tarul.cn/Article/details/gbxmkfusw.sHtML

TS:   nested.flat();
来源：http://read.share.bbcook.cn/Article/details/gxajdtlkj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.vehdjk.com/Article/details/gdmefkdsz.sHtML

Go:   // 手写双层循环
来源：http://wap.vehdjk.com/Article/details/gsmirrext.sHtML

Ruby: nested.flatten
来源：http://wap.yfazqb.com/Article/details/gchoqwdua.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.bbcook.cn/Article/details/gnrewicth.sHtML

[D19] 按字段分组
来源：http://blog.epnwcf.com/Article/details/gnjaxlwlv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.sjlbkw.cn/Article/details/gxrznnuga.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.yfazqb.com/Article/details/gkhaqecus.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.epnwcf.com/Article/details/gwyjshccp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.bbcook.cn/Article/details/glmbpdghn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.yfazqb.com/Article/details/gtoextvpg.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.sjlbkw.cn/Article/details/gubkcpwfd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.tarul.cn/Article/details/gighwzjba.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.tarul.cn/Article/details/ghfrfxucu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.yfazqb.com/Article/details/ghcjapcvj.sHtML

Py:   Counter(arr)
来源：http://m.share.tarul.cn/Article/details/gpqxhxuzx.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fktsv.cn/Article/details/gsunxrzkb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gwrxjjfdf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/gedhpftek.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.yfazqb.com/Article/details/gekfllrxc.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.tarul.cn/Article/details/grfmsxubp.sHtML

Ruby: arr.tally
来源：http://m.share.sjlbkw.cn/Article/details/gnqiufren.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.tarul.cn/Article/details/gtejbjttg.sHtML

[D21] 判断是否包含某元素
来源：http://baike.bbcook.cn/Article/details/gksivjvec.sHtML

Py:   x in arr
来源：http://m.share.vehdjk.com/Article/details/gewrlvofo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.vehdjk.com/Article/details/gpdkfjmyk.sHtML

JS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gvvpratnm.sHtML

TS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gozyagmdh.sHtML

Java: list.contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/ggyazqmdt.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fktsv.cn/Article/details/gmfstadrx.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gbxaruchc.sHtML

C#:   list.Contains(x)
来源：http://baike.vehdjk.com/Article/details/gupnpwrzj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.vehdjk.com/Article/details/gcuxwabqm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.yfazqb.com/Article/details/guyclgtbc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.sjlbkw.cn/Article/details/goserqqnu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.vehdjk.com/Article/details/gwfufebri.sHtML

TS:   [...arr];
来源：http://wap.epnwcf.com/Article/details/gznrqulrf.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fktsv.cn/Article/details/gjbtqyoza.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fktsv.cn/Article/details/gxqfqjith.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.tarul.cn/Article/details/gidrgelds.sHtML

C#:   new List<int>(list);
来源：http://3g.bbcook.cn/Article/details/gxoxgizxr.sHtML

[D23] reduce 累积计算
来源：http://read.share.vehdjk.com/Article/details/gzclzskxf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.tarul.cn/Article/details/glcdvxzim.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.vehdjk.com/Article/details/gakddlzvi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gosrssiht.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fktsv.cn/Article/details/gnecfohoe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.vehdjk.com/Article/details/gllwcwxir.sHtML

Go:   // 手写循环
来源：http://www.share.vehdjk.com/Article/details/ggnzlkxda.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.yfazqb.com/Article/details/gsfqyuvrw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.bbcook.cn/Article/details/ghczjjkra.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.yfazqb.com/Article/details/gjquylmgb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fktsv.cn/Article/details/gchxpmpdy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.sjlbkw.cn/Article/details/gtjhigksy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.yfazqb.com/Article/details/gbdlrqumj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.vehdjk.com/Article/details/gmqutlfxj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.yfazqb.com/Article/details/gklifkxxm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.sjlbkw.cn/Article/details/gesubxsez.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.bbcook.cn/Article/details/gwjtoitnv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.epnwcf.com/Article/details/gqljscsdv.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.vehdjk.com/Article/details/govvdzvxz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fktsv.cn/Article/details/gsxolbstg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.sjlbkw.cn/Article/details/glulcgnep.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.vehdjk.com/Article/details/gohhafals.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.sjlbkw.cn/Article/details/gmxhsuquq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.vehdjk.com/Article/details/gsujjmxza.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fktsv.cn/Article/details/gwgklpwcv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.bbcook.cn/Article/details/gdoyfoibt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.tarul.cn/Article/details/gspmvgyky.sHtML

[D26] 数组转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gyplybwuf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.vehdjk.com/Article/details/gqboiswll.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.yfazqb.com/Article/details/gskjyslko.sHtML

JS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/ghnwxoqwh.sHtML

TS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gwooigahy.sHtML

Java: String.join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/gvwajyfpb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.yfazqb.com/Article/details/gcjhcrtrx.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gnwbeompe.sHtML

C#:   string.Join(", ", list)
来源：http://blog.bbcook.cn/Article/details/grxnesvqo.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gagthukla.sHtML

E. 字符串处理
来源：http://read.share.sjlbkw.cn/Article/details/gefbgssuc.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfrxgjvsr.sHtML

[E01] 拼接字符串
来源：http://baike.epnwcf.com/Article/details/gumanblvt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.vehdjk.com/Article/details/glymjefud.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.sjlbkw.cn/Article/details/gqjsfitcl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/grixbquew.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/ggmqwecfv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.epnwcf.com/Article/details/gvsjuhfao.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.yfazqb.com/Article/details/goaxktafi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.bbcook.cn/Article/details/gpfywoabo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.epnwcf.com/Article/details/gijtiviqd.sHtML

[E02] 重复字符串
来源：http://m.share.sjlbkw.cn/Article/details/gmdvpluqn.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fktsv.cn/Article/details/ghyixkpsr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.vehdjk.com/Article/details/gdposfzyf.sHtML

JS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/godihvqdi.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gvoczhhfr.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gjdxxhlwo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.vehdjk.com/Article/details/gthddqdru.sHtML

Ruby: "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/gvrrxrcgp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.vehdjk.com/Article/details/giphytifh.sHtML

[E03] 截取子串
来源：http://baike.epnwcf.com/Article/details/ghaufyors.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fktsv.cn/Article/details/gtcodyxrj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gojhrikbc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.yfazqb.com/Article/details/ggijanvlu.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gwsgjkayh.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gnjvpjhvh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.sjlbkw.cn/Article/details/gyjrukzcx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.vehdjk.com/Article/details/ghdnuxwrp.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fktsv.cn/Article/details/gzdiksikg.sHtML

[E04] 查找子串位置
来源：http://mobile.yfazqb.com/Article/details/gzvvpieln.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/gsshvqkhh.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.epnwcf.com/Article/details/gqyvculbp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.epnwcf.com/Article/details/gxuzvoquq.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gwaiazath.sHtML

Java: s.indexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gqkxajtdp.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.vehdjk.com/Article/details/gtfepunuy.sHtML

Ruby: s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/gqadbpmrh.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gyekswano.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.sjlbkw.cn/Article/details/gwggmxdnu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.bbcook.cn/Article/details/gswenlums.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.vehdjk.com/Article/details/gwjapuxuv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.epnwcf.com/Article/details/ghqxnnlnm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.vehdjk.com/Article/details/gzubisjpu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.vehdjk.com/Article/details/garfonyfa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.tarul.cn/Article/details/gmxwjecpn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.bbcook.cn/Article/details/gxpmmvemz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.tarul.cn/Article/details/giwiqgcyj.sHtML

[E06] 替换子串
来源：http://read.share.bbcook.cn/Article/details/goethkkxt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/gkpgvypdi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.epnwcf.com/Article/details/gebfaiekj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gzmfgsgab.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gkgdifbar.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gvphwgyat.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gevdmolzz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gtiosddxf.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fktsv.cn/Article/details/gudkzfnlp.sHtML

[E07] 按分隔符拆分
来源：http://3g.epnwcf.com/Article/details/gjmauiueh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.tarul.cn/Article/details/gexishdim.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/glhcrqhhw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.tarul.cn/Article/details/gsmmbisab.sHtML

TS:   s.split(",")
来源：http://www.share.epnwcf.com/Article/details/gjgnsjmoq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.epnwcf.com/Article/details/gwplugmcl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.tarul.cn/Article/details/gfqocfrgz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.epnwcf.com/Article/details/gzewkjnqg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.sjlbkw.cn/Article/details/gqglnlirw.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.vehdjk.com/Article/details/guavbygbu.sHtML

Py:   ",".join(items)
来源：http://read.share.bbcook.cn/Article/details/gmvgduqri.sHtML

PHP:  implode(",", $items);
来源：http://blog.epnwcf.com/Article/details/gxwiikzoq.sHtML

JS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/gyitoqdcr.sHtML

TS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gyfszrpwa.sHtML

Java: String.join(",", items)
来源：http://baike.vehdjk.com/Article/details/gnbbowdgc.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.yfazqb.com/Article/details/gzrgoqtrv.sHtML

Ruby: items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gmpibkdgh.sHtML

C#:   string.Join(",", items)
来源：http://baike.tarul.cn/Article/details/gwtzqoedq.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fktsv.cn/Article/details/gbtqqvtwt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.vehdjk.com/Article/details/ganlbaxwl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fktsv.cn/Article/details/gasscihmh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/glgfdjail.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/gtmqoffsv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.tarul.cn/Article/details/gvtmyqdcs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fktsv.cn/Article/details/glxjqleho.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.vehdjk.com/Article/details/grdfdijbx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.tarul.cn/Article/details/giwkkiswh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.yfazqb.com/Article/details/gdgdxxxdz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gudbkjcuo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fktsv.cn/Article/details/gofqgtmrk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gycjbyssi.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gtbusokft.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/gxlxnamgq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/grfedhysz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gfopeuhmz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.bbcook.cn/Article/details/gdnhheoos.sHtML

[E11] 反转字符串
来源：http://mobile.tarul.cn/Article/details/gqhvcppmf.sHtML

Py:   s[::-1]
来源：http://read.share.bbcook.cn/Article/details/ghvnjeisl.sHtML

PHP:  strrev($s);
来源：http://blog.sjlbkw.cn/Article/details/gtikfitgm.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gcyuuehrd.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gcecpuvfc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.sjlbkw.cn/Article/details/gmczcshrc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.epnwcf.com/Article/details/gltkeahvg.sHtML

Ruby: s.reverse
来源：http://mobile.yfazqb.com/Article/details/gfzajfcnu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gcxjgxzvr.sHtML

[E12] 统计某字符出现次数
来源：http://wap.bbcook.cn/Article/details/gqktqktct.sHtML

Py:   s.count("a")
来源：http://mobile.tarul.cn/Article/details/gzaablnxj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.sjlbkw.cn/Article/details/gsokhxnsc.sHtML

JS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gahruezvi.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/gnoonnocs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.tarul.cn/Article/details/gpdxhzwnp.sHtML


<!-- 参考信息 -->