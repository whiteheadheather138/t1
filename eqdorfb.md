代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://3g.yfazqb.com/Article/details/gqrcrxeta.sHtML

[D08] 合并两个数组
来源：http://3g.bbcook.cn/Article/details/gpyxzlhmq.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.sjlbkw.cn/Article/details/ggpedimty.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.sjlbkw.cn/Article/details/galsbatir.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.yfazqb.com/Article/details/genokitva.sHtML

TS:   [...a, ...b];
来源：http://mobile.sjlbkw.cn/Article/details/ggdrrlcrs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.tarul.cn/Article/details/gbvnaqime.sHtML

Go:   append(a, b...)
来源：http://3g.vehdjk.com/Article/details/gpgpuyrof.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.tarul.cn/Article/details/garpbhubn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.tarul.cn/Article/details/glwahxcff.sHtML

[D09] 排序（升序）
来源：http://mobile.tarul.cn/Article/details/gbzdbyedo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.bbcook.cn/Article/details/gmdjogusn.sHtML

PHP:  sort($arr);
来源：http://3g.fktsv.cn/Article/details/gtnlupmij.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.yfazqb.com/Article/details/goilriptq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fktsv.cn/Article/details/gtuffmmku.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.vehdjk.com/Article/details/ghximegts.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/gjtkdhhen.sHtML

Ruby: arr.sort
来源：http://www.blog.fktsv.cn/Article/details/gmflskysz.sHtML

C#:   list.Sort();
来源：http://blog.yfazqb.com/Article/details/gcnfsyyeg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.vehdjk.com/Article/details/gczesvowe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.bbcook.cn/Article/details/gtifvhara.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.sjlbkw.cn/Article/details/glkcptsmh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.bbcook.cn/Article/details/gnykigqcg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/gwxstqieg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.epnwcf.com/Article/details/gleqvwhma.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.sjlbkw.cn/Article/details/goxgoeoxm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.yfazqb.com/Article/details/guokwuwis.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.yfazqb.com/Article/details/gywzdnqxm.sHtML

[D11] 反转数组
来源：http://3g.vehdjk.com/Article/details/gtrncfswv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.bbcook.cn/Article/details/gdnrpamky.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/grmbshbaf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.epnwcf.com/Article/details/gissdddue.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.epnwcf.com/Article/details/gkjxmyssz.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fktsv.cn/Article/details/gwbeyblbo.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gjsxshajr.sHtML

Ruby: arr.reverse
来源：http://www.share.vehdjk.com/Article/details/glmdgenpw.sHtML

C#:   list.Reverse();
来源：http://m.share.tarul.cn/Article/details/gomvtsdru.sHtML

[D12] 查找元素下标
来源：http://blog.bbcook.cn/Article/details/gerlfwopb.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.bbcook.cn/Article/details/gvezrkvnd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.bbcook.cn/Article/details/gjipalrxq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/gnxonkmsv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fktsv.cn/Article/details/gtteeijts.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.sjlbkw.cn/Article/details/gpaseppqx.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.yfazqb.com/Article/details/gcqbincla.sHtML

Ruby: arr.index(x)
来源：http://baike.tarul.cn/Article/details/gulvrovey.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.tarul.cn/Article/details/gjngotyek.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.vehdjk.com/Article/details/gmlfucvsc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.bbcook.cn/Article/details/gtaxseqbu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fktsv.cn/Article/details/gkggoelfj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/guvvbriyd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/gkmvbiwjf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gickchilz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.tarul.cn/Article/details/gozfuwlmj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.epnwcf.com/Article/details/glxcnyxay.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fktsv.cn/Article/details/gfdlqwwaz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.vehdjk.com/Article/details/gtzxhmnsk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.epnwcf.com/Article/details/grllhnbfp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/ggccimbrw.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/ggkmaxmax.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/gvbxuezas.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.tarul.cn/Article/details/gqetmdrjk.sHtML

Go:   // 手写循环
来源：http://mobile.yfazqb.com/Article/details/geykliyoo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fktsv.cn/Article/details/gzgtnrzev.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.yfazqb.com/Article/details/gcopmyzwc.sHtML

[D15] 去重
来源：http://m.share.vehdjk.com/Article/details/gcjibbgms.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.yfazqb.com/Article/details/gaiozaqnz.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gigjparrt.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrutlzmz.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gjilqaxkz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.epnwcf.com/Article/details/gnqrpmasu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.sjlbkw.cn/Article/details/gcjfhwort.sHtML

Ruby: arr.uniq
来源：http://baike.tarul.cn/Article/details/gkqyoccgr.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.bbcook.cn/Article/details/gyrephzjx.sHtML

[D16] 求和与平均值
来源：http://www.blog.vehdjk.com/Article/details/gaqrjohfp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.yfazqb.com/Article/details/ggkwpxejz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.vehdjk.com/Article/details/galtkwlzh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/ggantjfik.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gwdbqrdhj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.vehdjk.com/Article/details/gtfkfwbat.sHtML

Go:   // 手写循环累加
来源：http://m.share.bbcook.cn/Article/details/gksupiniq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.vehdjk.com/Article/details/gmonhsbha.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.vehdjk.com/Article/details/gjzrcozhp.sHtML

[D17] 最大值与最小值
来源：http://www.blog.epnwcf.com/Article/details/gfdvldllz.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gmzxmmvcs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gukkuazgl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.epnwcf.com/Article/details/gfcxdxezv.sHtML

TS:   Math.max(...arr);
来源：http://m.share.bbcook.cn/Article/details/gynhushje.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fktsv.cn/Article/details/gvtyfkjxl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.bbcook.cn/Article/details/gzantvnio.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.bbcook.cn/Article/details/gjkmnxlip.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.yfazqb.com/Article/details/guthdnncz.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.epnwcf.com/Article/details/gylkohbnb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fktsv.cn/Article/details/gyyudfqnz.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.tarul.cn/Article/details/gmqbvahfy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.vehdjk.com/Article/details/gixtkwqlh.sHtML

TS:   nested.flat();
来源：http://3g.tarul.cn/Article/details/gfolbazpn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.epnwcf.com/Article/details/geoavhdon.sHtML

Go:   // 手写双层循环
来源：http://blog.yfazqb.com/Article/details/gnnptgqln.sHtML

Ruby: nested.flatten
来源：http://baike.vehdjk.com/Article/details/grttnexoz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.vehdjk.com/Article/details/ghserajty.sHtML

[D19] 按字段分组
来源：http://www.blog.bbcook.cn/Article/details/ggzsofkuo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.bbcook.cn/Article/details/gbttjerjd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.sjlbkw.cn/Article/details/gwjdcvamr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fktsv.cn/Article/details/gaotnfgkq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/gixqhtzge.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.epnwcf.com/Article/details/gznrudsli.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.sjlbkw.cn/Article/details/gtstvmkpg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.epnwcf.com/Article/details/gpnqzbdlh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.bbcook.cn/Article/details/gwyzryzdl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.epnwcf.com/Article/details/glpfwmvfb.sHtML

Py:   Counter(arr)
来源：http://www.blog.tarul.cn/Article/details/gghdgelmy.sHtML

PHP:  array_count_values($arr);
来源：http://3g.tarul.cn/Article/details/gxvbkuqql.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/ggjajenmp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gwkvlavxp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.yfazqb.com/Article/details/gmkgtkkxe.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.vehdjk.com/Article/details/ghhjzkmzb.sHtML

Ruby: arr.tally
来源：http://m.share.bbcook.cn/Article/details/gnunvrsxj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.epnwcf.com/Article/details/ghpsxrckj.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.tarul.cn/Article/details/gyelrzrym.sHtML

Py:   x in arr
来源：http://read.share.fktsv.cn/Article/details/gjkebojxk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.tarul.cn/Article/details/gygehtait.sHtML

JS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gpqkkrdio.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gccllirxk.sHtML

Java: list.contains(x)
来源：http://3g.fktsv.cn/Article/details/ggtzsxywq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gtsgybwwt.sHtML

Ruby: arr.include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gykeeeabb.sHtML

C#:   list.Contains(x)
来源：http://wap.yfazqb.com/Article/details/grbstmnuk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.sjlbkw.cn/Article/details/grdtyrdny.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.tarul.cn/Article/details/gfxhsmath.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.tarul.cn/Article/details/gvfwfgfgn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.yfazqb.com/Article/details/grxxooqxs.sHtML

TS:   [...arr];
来源：http://www.blog.yfazqb.com/Article/details/gzpzynmjh.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gxxrjvevh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.vehdjk.com/Article/details/gdixsfrck.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.yfazqb.com/Article/details/gfyaqqsvt.sHtML

C#:   new List<int>(list);
来源：http://3g.fktsv.cn/Article/details/gxasuvolt.sHtML

[D23] reduce 累积计算
来源：http://blog.yfazqb.com/Article/details/gbvivndoy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.vehdjk.com/Article/details/gdbmrzdvj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.tarul.cn/Article/details/gxingxqnz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gtsxqktib.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gizkqkjwo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fktsv.cn/Article/details/gyocmjvyk.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/ggeuseujo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.sjlbkw.cn/Article/details/gvaoswddf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.sjlbkw.cn/Article/details/gnnlwgwda.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.yfazqb.com/Article/details/gdrqdfoee.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.vehdjk.com/Article/details/gwoiptruy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gcsvwwimz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.tarul.cn/Article/details/gscwkprjl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gljbyfaqk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.yfazqb.com/Article/details/gtbmcutfs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.bbcook.cn/Article/details/gaogqtddg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.bbcook.cn/Article/details/gotcvjdyj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.bbcook.cn/Article/details/gpdybbwpa.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.yfazqb.com/Article/details/gidtxajha.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.yfazqb.com/Article/details/gzjvmrfgj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.epnwcf.com/Article/details/gqmrpotoq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.sjlbkw.cn/Article/details/grsypihaj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.epnwcf.com/Article/details/gijlsgnjm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.yfazqb.com/Article/details/gusgzdche.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.yfazqb.com/Article/details/glzuobaib.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fktsv.cn/Article/details/gwrynkwgg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.bbcook.cn/Article/details/ggriuvybc.sHtML

[D26] 数组转字符串
来源：http://3g.tarul.cn/Article/details/gxmgaqfbw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.sjlbkw.cn/Article/details/gleallbok.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gtzirlckj.sHtML

JS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/geboaevlf.sHtML

TS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gqrxzjshr.sHtML

Java: String.join(", ", list)
来源：http://mobile.fktsv.cn/Article/details/gydhqtuug.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fktsv.cn/Article/details/gkvivuois.sHtML

Ruby: arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gjcvgnunc.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.yfazqb.com/Article/details/gkxmvsqup.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gbyejkxvd.sHtML

E. 字符串处理
来源：http://www.blog.sjlbkw.cn/Article/details/ggctanodj.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/geiahyxdz.sHtML

[E01] 拼接字符串
来源：http://baike.vehdjk.com/Article/details/gxekrapms.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.epnwcf.com/Article/details/grhjgqlzc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.tarul.cn/Article/details/gahwpbgbj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.yfazqb.com/Article/details/gxepuisfl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gfyppwvcv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.bbcook.cn/Article/details/guhsdhlqz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.tarul.cn/Article/details/gnobjexfy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.sjlbkw.cn/Article/details/gxnnuwhqw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gtyixywpb.sHtML

[E02] 重复字符串
来源：http://www.share.yfazqb.com/Article/details/gdivciztr.sHtML

Py:   "ab" * 3
来源：http://blog.fktsv.cn/Article/details/goeeshssj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.tarul.cn/Article/details/givbikpnj.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/ghyczglpc.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gybcnvkgl.sHtML

Java: "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/grhgxacwd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.yfazqb.com/Article/details/gzckklona.sHtML

Ruby: "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gphkunhmn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.bbcook.cn/Article/details/ghgtjvifd.sHtML

[E03] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gsfasebyj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fktsv.cn/Article/details/gecgmlsoy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gkqxjwggl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/gbbztiodv.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gxyqzsyew.sHtML

Java: s.substring(1, 4)
来源：http://3g.vehdjk.com/Article/details/ghvzakail.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gjwdfgyju.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fktsv.cn/Article/details/gvqioljno.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.tarul.cn/Article/details/gkyjzjesb.sHtML

[E04] 查找子串位置
来源：http://www.m.share.yfazqb.com/Article/details/gbvwmsvoh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.vehdjk.com/Article/details/gazfmnlhe.sHtML

PHP:  strpos($s, "x");
来源：http://wap.epnwcf.com/Article/details/gxykfztkc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.vehdjk.com/Article/details/gbyzdmcze.sHtML

TS:   s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/glergnmca.sHtML

Java: s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gvlrxltly.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.epnwcf.com/Article/details/glzjoeopx.sHtML

Ruby: s.index("x")
来源：http://3g.tarul.cn/Article/details/gkbnxzkev.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gtiprljav.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.yfazqb.com/Article/details/gcswhtyox.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gtejjmbxq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.epnwcf.com/Article/details/gmaqwprke.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.epnwcf.com/Article/details/gpogkmaal.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.tarul.cn/Article/details/gjvufzabw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/gcrhssmow.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fktsv.cn/Article/details/gpelukcja.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.bbcook.cn/Article/details/gizhnwigv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.yfazqb.com/Article/details/ggoylxlrm.sHtML

[E06] 替换子串
来源：http://m.share.bbcook.cn/Article/details/gyjvfpwmm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/gwuogkdbt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.yfazqb.com/Article/details/gwxhrmmds.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gnedqrnxu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/glyzxsuey.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gvpvttogz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/grbgwvhba.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.yfazqb.com/Article/details/gmbddpivo.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gpxevbzbf.sHtML

[E07] 按分隔符拆分
来源：http://www.share.epnwcf.com/Article/details/gjjrsgpvs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.bbcook.cn/Article/details/gwgguevjj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.yfazqb.com/Article/details/gllyuphyk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fktsv.cn/Article/details/gnytlbuft.sHtML

TS:   s.split(",")
来源：http://www.blog.bbcook.cn/Article/details/grvuhdato.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.yfazqb.com/Article/details/gbeguudkn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fktsv.cn/Article/details/ginwktlmx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.tarul.cn/Article/details/gkgbddqpf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.sjlbkw.cn/Article/details/gfgtvfldk.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.vehdjk.com/Article/details/grahmfkzm.sHtML

Py:   ",".join(items)
来源：http://blog.sjlbkw.cn/Article/details/gjfdjlixj.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fktsv.cn/Article/details/gkmddylyj.sHtML

JS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gfomncbhn.sHtML

TS:   items.join(",")
来源：http://3g.bbcook.cn/Article/details/gqaeuukkr.sHtML

Java: String.join(",", items)
来源：http://wap.fktsv.cn/Article/details/gxmjzloaf.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.tarul.cn/Article/details/gfcxrzgzd.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gyecsdsym.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gmlszqxyy.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.tarul.cn/Article/details/gbovkymdo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.bbcook.cn/Article/details/gfuxbvwme.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.epnwcf.com/Article/details/gprmvqfsz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.bbcook.cn/Article/details/gtwbouauj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.epnwcf.com/Article/details/gskefspxp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gqseljksj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.tarul.cn/Article/details/gegfzmcim.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.tarul.cn/Article/details/gohxlzonb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.vehdjk.com/Article/details/gsjmpeodt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.sjlbkw.cn/Article/details/gisbujfwx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/gfnhmrruz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.bbcook.cn/Article/details/gflbpkqhz.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/ggskugvcy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/giqsvyion.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gdufvjluw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gqedfctom.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/gwswsdklx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fktsv.cn/Article/details/ghkixjerw.sHtML

[E11] 反转字符串
来源：http://blog.epnwcf.com/Article/details/gvloqkfqj.sHtML

Py:   s[::-1]
来源：http://mobile.tarul.cn/Article/details/gubrjfmuc.sHtML

PHP:  strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gyhzogocn.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/grigpvytv.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/glgqjnmhd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.epnwcf.com/Article/details/gzojkbvzr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fktsv.cn/Article/details/gvpxdhkeh.sHtML

Ruby: s.reverse
来源：http://3g.epnwcf.com/Article/details/gkdbqivtr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/govfbxnel.sHtML

[E12] 统计某字符出现次数
来源：http://3g.sjlbkw.cn/Article/details/gtkcgijar.sHtML

Py:   s.count("a")
来源：http://wap.bbcook.cn/Article/details/gyxcbxkhq.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.yfazqb.com/Article/details/geobwjpdn.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gzwxadmya.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/gghsbiwgg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.yfazqb.com/Article/details/gixpjttrz.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.vehdjk.com/Article/details/gqercovhp.sHtML

Ruby: s.count("a")
来源：http://m.share.vehdjk.com/Article/details/gmlerphtc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.bbcook.cn/Article/details/glzwhrzkf.sHtML

[E13] 逐字符遍历
来源：http://mobile.fktsv.cn/Article/details/gxzxwblfl.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.bbcook.cn/Article/details/gvimmlibb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fktsv.cn/Article/details/gfewnvxvi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcotgkglg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gylpthdth.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gjvuswwwj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.tarul.cn/Article/details/gcpzcqivf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.yfazqb.com/Article/details/ghbvayqun.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.bbcook.cn/Article/details/gqppmddqb.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.epnwcf.com/Article/details/gwcsqacim.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.bbcook.cn/Article/details/gdrcqufna.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gzucwwvht.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.epnwcf.com/Article/details/gbtdhcupu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.tarul.cn/Article/details/gxskxhyqu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.bbcook.cn/Article/details/gurtwgnde.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.bbcook.cn/Article/details/gxpepfqkp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.tarul.cn/Article/details/ggprbhwva.sHtML


<!-- 参考信息 -->