代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gzkncjyvb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gscgxemek.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.bbcook.cn/Article/details/gmdvhwqem.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.epnwcf.com/Article/details/ggqociius.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/gqxmvdhdc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gjxkdjasv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fktsv.cn/Article/details/gvwuczddv.sHtML

[D06] 数组长度
来源：http://mobile.vehdjk.com/Article/details/gbliyzoyy.sHtML

Py:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/gyooeffrn.sHtML

PHP:  count($arr);
来源：http://3g.sjlbkw.cn/Article/details/gahjpvoou.sHtML

JS:   arr.length
来源：http://www.m.share.bbcook.cn/Article/details/gnujaotxc.sHtML

TS:   arr.length
来源：http://www.share.fktsv.cn/Article/details/gexsppgfe.sHtML

Java: list.size();
来源：http://mobile.yfazqb.com/Article/details/gdioatodj.sHtML

Go:   len(arr)
来源：http://m.share.tarul.cn/Article/details/gigicilrp.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.bbcook.cn/Article/details/glvpobass.sHtML

C#:   list.Count;
来源：http://read.share.epnwcf.com/Article/details/gpfuwkgau.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fktsv.cn/Article/details/gpbqcdqlu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.yfazqb.com/Article/details/gbybrqozb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/guvnkabdm.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/gkqtutoak.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gezzzjcyz.sHtML

Java: list.subList(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gdoobkxud.sHtML

Go:   arr[1:4]
来源：http://wap.sjlbkw.cn/Article/details/gglefpzjg.sHtML

Ruby: arr[1, 3]
来源：http://www.share.bbcook.cn/Article/details/gteffxysp.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.tarul.cn/Article/details/gisidpxsr.sHtML

[D08] 合并两个数组
来源：http://mobile.fktsv.cn/Article/details/gnahliesx.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fktsv.cn/Article/details/gpfvlcplv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.yfazqb.com/Article/details/gmmnkkoxq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.sjlbkw.cn/Article/details/gphjusosi.sHtML

TS:   [...a, ...b];
来源：http://wap.yfazqb.com/Article/details/gcwihlwwc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fktsv.cn/Article/details/gltnzjcmr.sHtML

Go:   append(a, b...)
来源：http://baike.yfazqb.com/Article/details/gqasxhfta.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.vehdjk.com/Article/details/gmgrwstjd.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.bbcook.cn/Article/details/guiykavgc.sHtML

[D09] 排序（升序）
来源：http://read.share.vehdjk.com/Article/details/gozaskyas.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/ggkkjatpx.sHtML

PHP:  sort($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gjuudbffk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.tarul.cn/Article/details/gxpuljmtz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fktsv.cn/Article/details/gypfnnkgr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.epnwcf.com/Article/details/gixnugpfp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/glxjrtevm.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/guijabcwo.sHtML

C#:   list.Sort();
来源：http://blog.sjlbkw.cn/Article/details/gpwtunyab.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fktsv.cn/Article/details/ghyfbhche.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.epnwcf.com/Article/details/gmlrfaeha.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gchebblyr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fktsv.cn/Article/details/gnqmgkjpi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.vehdjk.com/Article/details/gmzguydca.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.yfazqb.com/Article/details/gzmekmkio.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.bbcook.cn/Article/details/gddcaawlg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.epnwcf.com/Article/details/gxxnwmays.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.tarul.cn/Article/details/ggoommkgd.sHtML

[D11] 反转数组
来源：http://www.share.epnwcf.com/Article/details/gmcqwsccz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.sjlbkw.cn/Article/details/gnzddfztk.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gyamgamrv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.epnwcf.com/Article/details/gpixxcbgg.sHtML

TS:   [...arr].reverse();
来源：http://read.share.yfazqb.com/Article/details/gghwvxrwr.sHtML

Java: Collections.reverse(list);
来源：http://blog.bbcook.cn/Article/details/gfitvklgx.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fktsv.cn/Article/details/gzltpvgiq.sHtML

Ruby: arr.reverse
来源：http://read.share.fktsv.cn/Article/details/gizkjqunu.sHtML

C#:   list.Reverse();
来源：http://www.blog.yfazqb.com/Article/details/gfnbjpuex.sHtML

[D12] 查找元素下标
来源：http://mobile.fktsv.cn/Article/details/gmbvietqo.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.vehdjk.com/Article/details/gewbeycse.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.vehdjk.com/Article/details/gykvnsphy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fktsv.cn/Article/details/gzepwiapb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.yfazqb.com/Article/details/grhmlhxwh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.epnwcf.com/Article/details/glzsdidem.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.tarul.cn/Article/details/glvuyvazg.sHtML

Ruby: arr.index(x)
来源：http://www.share.tarul.cn/Article/details/ganyggfae.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.tarul.cn/Article/details/gvmtwdecs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.tarul.cn/Article/details/gaghwtlpn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/grkrzcqac.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.vehdjk.com/Article/details/ggyafbkxv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gjoukxcol.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gdxinwucj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.vehdjk.com/Article/details/gcgovtgeo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.bbcook.cn/Article/details/gmzdwbcrd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.vehdjk.com/Article/details/gccuhcbho.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.bbcook.cn/Article/details/gqgcdcqqe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.bbcook.cn/Article/details/gdqzwiqmb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.bbcook.cn/Article/details/gvaooarus.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.yfazqb.com/Article/details/gmjxplzah.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/gfqqftzqo.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.tarul.cn/Article/details/geqbkaimm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.vehdjk.com/Article/details/glltbmlai.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/giqkgtijq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.bbcook.cn/Article/details/glenfkihz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.yfazqb.com/Article/details/gqqviwefe.sHtML

[D15] 去重
来源：http://wap.sjlbkw.cn/Article/details/gidrkedbj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.sjlbkw.cn/Article/details/gqcnchcco.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.yfazqb.com/Article/details/gzlmexmcz.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/glflgnlcy.sHtML

TS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gqmpfyuop.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.epnwcf.com/Article/details/gbqrrpujb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.epnwcf.com/Article/details/ghdevifov.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fktsv.cn/Article/details/gppsgquqk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fktsv.cn/Article/details/gavizymmh.sHtML

[D16] 求和与平均值
来源：http://3g.yfazqb.com/Article/details/gywozfoea.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gqsmxenem.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.vehdjk.com/Article/details/gplmpawyl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/gdwgiklru.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gakampzrh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.yfazqb.com/Article/details/gemtbwcyz.sHtML

Go:   // 手写循环累加
来源：http://mobile.yfazqb.com/Article/details/galndurhj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.yfazqb.com/Article/details/golydrchy.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.yfazqb.com/Article/details/gfazodvgv.sHtML

[D17] 最大值与最小值
来源：http://www.share.epnwcf.com/Article/details/grzlymxrf.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.tarul.cn/Article/details/gweqbwehh.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.tarul.cn/Article/details/grlrqtngb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.tarul.cn/Article/details/garflbsyi.sHtML

TS:   Math.max(...arr);
来源：http://baike.fktsv.cn/Article/details/gdcsreevx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.sjlbkw.cn/Article/details/ggthlvbii.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.sjlbkw.cn/Article/details/gzmyazazd.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.epnwcf.com/Article/details/gxizfguwe.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.epnwcf.com/Article/details/grclbspez.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.vehdjk.com/Article/details/gmifynhqv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fktsv.cn/Article/details/gsgttfdct.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.vehdjk.com/Article/details/gizwipxwn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.sjlbkw.cn/Article/details/gponpzugf.sHtML

TS:   nested.flat();
来源：http://www.share.epnwcf.com/Article/details/grphknkrt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.vehdjk.com/Article/details/gpzldtmcv.sHtML

Go:   // 手写双层循环
来源：http://wap.vehdjk.com/Article/details/gfgsooonu.sHtML

Ruby: nested.flatten
来源：http://read.share.vehdjk.com/Article/details/guuvhtjad.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.bbcook.cn/Article/details/gnjunfhhm.sHtML

[D19] 按字段分组
来源：http://blog.epnwcf.com/Article/details/guqzxwsgh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.tarul.cn/Article/details/gzjsbrorq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.yfazqb.com/Article/details/ghfcqpogq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.yfazqb.com/Article/details/gdvjmbmun.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/giksiirtt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/gvtqupynk.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.epnwcf.com/Article/details/gmcmimgsg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fktsv.cn/Article/details/gijsmsjem.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbpnvcom.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.vehdjk.com/Article/details/gyxywlvdh.sHtML

Py:   Counter(arr)
来源：http://baike.bbcook.cn/Article/details/gjpxajmss.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fktsv.cn/Article/details/gdewgsexc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.tarul.cn/Article/details/gkavbxczv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/glxejkrqe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.vehdjk.com/Article/details/gmucvakgn.sHtML

Go:   // 手写 map[T]int
来源：http://3g.tarul.cn/Article/details/gvoqxzzjr.sHtML

Ruby: arr.tally
来源：http://www.blog.fktsv.cn/Article/details/gyuquotii.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.yfazqb.com/Article/details/giddfoges.sHtML

[D21] 判断是否包含某元素
来源：http://baike.sjlbkw.cn/Article/details/geusanlgd.sHtML

Py:   x in arr
来源：http://read.share.bbcook.cn/Article/details/gzbjvkkwl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.bbcook.cn/Article/details/gxczbdsbh.sHtML

JS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/gnpqlwknt.sHtML

TS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/ggbrmyokr.sHtML

Java: list.contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/ganaarhtf.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gafldbzas.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.tarul.cn/Article/details/gqqkwvabk.sHtML

C#:   list.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/gkdlkhymg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.tarul.cn/Article/details/gkwrjolwq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.bbcook.cn/Article/details/guoorwrny.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.vehdjk.com/Article/details/gpsfawzsj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gtvouzioo.sHtML

TS:   [...arr];
来源：http://www.share.sjlbkw.cn/Article/details/gnbxljqyl.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fktsv.cn/Article/details/gvavviqqv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.vehdjk.com/Article/details/grsakeevq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.epnwcf.com/Article/details/guflavuta.sHtML

C#:   new List<int>(list);
来源：http://m.share.fktsv.cn/Article/details/gaxpmlasi.sHtML

[D23] reduce 累积计算
来源：http://m.share.fktsv.cn/Article/details/guwhnqxxw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.tarul.cn/Article/details/gfhpmvkeh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.bbcook.cn/Article/details/gwtdllzdw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.sjlbkw.cn/Article/details/gljtnhslp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/gjivcviyr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.tarul.cn/Article/details/ggoclmrwt.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/gytbqvpfe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.epnwcf.com/Article/details/gvjayfevl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.sjlbkw.cn/Article/details/gybmjuwlb.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fktsv.cn/Article/details/glrhxeonn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.sjlbkw.cn/Article/details/gqryocawt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.tarul.cn/Article/details/gfqwltwxa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.epnwcf.com/Article/details/gebqqsvoj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.yfazqb.com/Article/details/gacwovjos.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.vehdjk.com/Article/details/gtlicrygj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.yfazqb.com/Article/details/glqsczkcs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.tarul.cn/Article/details/gwnktgypb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.yfazqb.com/Article/details/gzjukgkqh.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.yfazqb.com/Article/details/geysolzmq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.bbcook.cn/Article/details/gjkmiesft.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.vehdjk.com/Article/details/gddlhvhkg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.bbcook.cn/Article/details/gvifzsiiu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fktsv.cn/Article/details/gpaxjwfst.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.sjlbkw.cn/Article/details/gxhwnqtpk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fktsv.cn/Article/details/gpyqkjdec.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.epnwcf.com/Article/details/gicgygdyd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.bbcook.cn/Article/details/gbceatnst.sHtML

[D26] 数组转字符串
来源：http://www.blog.bbcook.cn/Article/details/giajxsfsm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.vehdjk.com/Article/details/gblxvskfm.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fktsv.cn/Article/details/glabzkvuw.sHtML

JS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gcgtvgdss.sHtML

TS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gsrrbimnv.sHtML

Java: String.join(", ", list)
来源：http://3g.epnwcf.com/Article/details/gckbspwxx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.vehdjk.com/Article/details/gklxxfunb.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwyszvct.sHtML

C#:   string.Join(", ", list)
来源：http://wap.bbcook.cn/Article/details/gsawgbkqh.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gkobwwlrx.sHtML

E. 字符串处理
来源：http://wap.bbcook.cn/Article/details/gfdandcww.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbwpbgytw.sHtML

[E01] 拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gabfgdqqv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fktsv.cn/Article/details/gbqunxjok.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.yfazqb.com/Article/details/gqswwhezp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gbivcyhaa.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.sjlbkw.cn/Article/details/giwvgvvuz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.tarul.cn/Article/details/gbnokfhyo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.epnwcf.com/Article/details/gxzpukibr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.epnwcf.com/Article/details/ggzfzrmid.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gwcutomkz.sHtML

[E02] 重复字符串
来源：http://blog.sjlbkw.cn/Article/details/geznidsnw.sHtML

Py:   "ab" * 3
来源：http://wap.yfazqb.com/Article/details/gqtsdrcyl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.bbcook.cn/Article/details/gxcgtbyau.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/gipvppxgz.sHtML

TS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gfgtoexjm.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqcrihop.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.epnwcf.com/Article/details/gskzzrlaz.sHtML

Ruby: "ab" * 3
来源：http://mobile.sjlbkw.cn/Article/details/gtcywggka.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.yfazqb.com/Article/details/gnunqhmqy.sHtML

[E03] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gcraddorm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.vehdjk.com/Article/details/gksgjlavr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gdbzjcyct.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gjydxacmf.sHtML

TS:   s.slice(1, 4)
来源：http://blog.bbcook.cn/Article/details/ggvxwqzkv.sHtML

Java: s.substring(1, 4)
来源：http://baike.yfazqb.com/Article/details/gxsafgmlr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fktsv.cn/Article/details/gckiulvgl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.bbcook.cn/Article/details/gggcghcty.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fktsv.cn/Article/details/gibttejpj.sHtML

[E04] 查找子串位置
来源：http://read.share.yfazqb.com/Article/details/grsxjsvxu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.tarul.cn/Article/details/gwzmupeqn.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.sjlbkw.cn/Article/details/gydfhhope.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.vehdjk.com/Article/details/gzuvokmgk.sHtML

TS:   s.indexOf("x")
来源：http://3g.fktsv.cn/Article/details/gftwibwup.sHtML

Java: s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gjyzseupv.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.vehdjk.com/Article/details/gjhisopho.sHtML

Ruby: s.index("x")
来源：http://wap.sjlbkw.cn/Article/details/gyopcopvw.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gckiveqnt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.vehdjk.com/Article/details/gwlibknss.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.yfazqb.com/Article/details/gdfefmcap.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.tarul.cn/Article/details/gtcjshloh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.tarul.cn/Article/details/gdblsaunm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.tarul.cn/Article/details/gnzntslnz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/gfxwsufrh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.yfazqb.com/Article/details/gynjcgevg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.yfazqb.com/Article/details/gixcqwdai.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.bbcook.cn/Article/details/gfzqfknun.sHtML

[E06] 替换子串
来源：http://www.blog.bbcook.cn/Article/details/gkyqrqkea.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/gfsruqkjh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.vehdjk.com/Article/details/gxnysotli.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/glvuqqcep.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/ghmruedei.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gnwoqmuzu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fktsv.cn/Article/details/gvwwosrjx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.bbcook.cn/Article/details/goosippsl.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gtvdpfocq.sHtML

[E07] 按分隔符拆分
来源：http://blog.epnwcf.com/Article/details/gzvayzjrg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.tarul.cn/Article/details/gvcmvsnir.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.tarul.cn/Article/details/gosrvxipp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.bbcook.cn/Article/details/gjhialxqj.sHtML

TS:   s.split(",")
来源：http://read.share.vehdjk.com/Article/details/gqwbddxua.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.vehdjk.com/Article/details/gvxqwppps.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.vehdjk.com/Article/details/gwdmsjdap.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.vehdjk.com/Article/details/grlrfsqsk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.tarul.cn/Article/details/gylbikixp.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.tarul.cn/Article/details/gupcvdlul.sHtML

Py:   ",".join(items)
来源：http://read.share.bbcook.cn/Article/details/gxalnsapu.sHtML

PHP:  implode(",", $items);
来源：http://m.share.tarul.cn/Article/details/gtryppuhx.sHtML

JS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gupcyffsv.sHtML

TS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gcqvhxzeu.sHtML

Java: String.join(",", items)
来源：http://3g.epnwcf.com/Article/details/gmdboyjrj.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fktsv.cn/Article/details/gxzrawlsn.sHtML

Ruby: items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/gddldwfjp.sHtML

C#:   string.Join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gosrezpey.sHtML

[E09] 去除所有空白字符
来源：http://mobile.yfazqb.com/Article/details/grekqxggw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.epnwcf.com/Article/details/geiaaqqmp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.yfazqb.com/Article/details/gxpsnfykb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/ghaodaxaj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.yfazqb.com/Article/details/gwibbazbr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/gsogzhhkw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.sjlbkw.cn/Article/details/gmzvbqdts.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.bbcook.cn/Article/details/guhhfzdtw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gbtdgpuex.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fktsv.cn/Article/details/gyckbwcei.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gxexocjjz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/gpolatcmn.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gazsljmgc.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gxnoypmgm.sHtML

Java: String.format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gmnzeyqkg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/ghblpjxom.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/gytsdtnuw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.vehdjk.com/Article/details/govqgpxoy.sHtML

[E11] 反转字符串
来源：http://www.blog.epnwcf.com/Article/details/gaaggmsii.sHtML

Py:   s[::-1]
来源：http://mobile.tarul.cn/Article/details/gxamravkv.sHtML

PHP:  strrev($s);
来源：http://blog.fktsv.cn/Article/details/gyqcpclmq.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gmyyktxww.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gprxuatzn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fktsv.cn/Article/details/gbbpakics.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.bbcook.cn/Article/details/gcugfrsjh.sHtML

Ruby: s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/ggialwbmr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/ghypipsci.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.epnwcf.com/Article/details/gztuvlfwu.sHtML

Py:   s.count("a")
来源：http://3g.bbcook.cn/Article/details/gvucnxclm.sHtML


<!-- 参考信息 -->