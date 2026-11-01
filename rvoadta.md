代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://mobile.vehdjk.com/Article/details/gcekatzmh.sHtML

[D08] 合并两个数组
来源：http://mobile.tarul.cn/Article/details/gopabiydx.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fktsv.cn/Article/details/gpfslaaqy.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.tarul.cn/Article/details/gehrrukfm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.tarul.cn/Article/details/gutflshmm.sHtML

TS:   [...a, ...b];
来源：http://blog.bbcook.cn/Article/details/gpzfpjeii.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.bbcook.cn/Article/details/gvrzwbhuo.sHtML

Go:   append(a, b...)
来源：http://wap.epnwcf.com/Article/details/gtdperauv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.sjlbkw.cn/Article/details/gddmxizhn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gjyqjmaej.sHtML

[D09] 排序（升序）
来源：http://3g.tarul.cn/Article/details/giagaqnfu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/ghmuffnom.sHtML

PHP:  sort($arr);
来源：http://baike.epnwcf.com/Article/details/gaxbqmpnr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.sjlbkw.cn/Article/details/grcrjoubs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.tarul.cn/Article/details/gwwlsfqfg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.vehdjk.com/Article/details/gnmvkkbnm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/gefvrqlnj.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/glayuaptb.sHtML

C#:   list.Sort();
来源：http://baike.epnwcf.com/Article/details/gyjbxboxa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.vehdjk.com/Article/details/gewozeccr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.bbcook.cn/Article/details/ggbytxrcm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/gfbyjhvsy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gtgsiopsb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.tarul.cn/Article/details/gybazbjjq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.vehdjk.com/Article/details/guogzepvz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.epnwcf.com/Article/details/gwlhklehn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.tarul.cn/Article/details/gyeifkhlu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.epnwcf.com/Article/details/gkifaslrl.sHtML

[D11] 反转数组
来源：http://www.blog.yfazqb.com/Article/details/gbgxbsido.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fktsv.cn/Article/details/grenrupuw.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fktsv.cn/Article/details/gasgppurd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.tarul.cn/Article/details/guomjjshh.sHtML

TS:   [...arr].reverse();
来源：http://3g.bbcook.cn/Article/details/gjbcquuaj.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.vehdjk.com/Article/details/gxnfcbtfo.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fktsv.cn/Article/details/gvzvojbkq.sHtML

Ruby: arr.reverse
来源：http://www.blog.yfazqb.com/Article/details/gwqomyubf.sHtML

C#:   list.Reverse();
来源：http://wap.bbcook.cn/Article/details/gsxrhwavf.sHtML

[D12] 查找元素下标
来源：http://mobile.vehdjk.com/Article/details/gyirbwaaq.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.yfazqb.com/Article/details/gpzyibdjw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.epnwcf.com/Article/details/gwsvotdxw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/ghomoyjsl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/gekwujppu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.vehdjk.com/Article/details/gqmfyojhd.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fktsv.cn/Article/details/gjvrfmpoc.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.vehdjk.com/Article/details/gsblpkwaa.sHtML

C#:   list.IndexOf(x);
来源：http://wap.sjlbkw.cn/Article/details/ghmtdfkjs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.epnwcf.com/Article/details/gotyeabdw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.bbcook.cn/Article/details/gbxjanwkg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.yfazqb.com/Article/details/gsybhbhvb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.bbcook.cn/Article/details/gwbxojnhe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fktsv.cn/Article/details/ghneouqok.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.vehdjk.com/Article/details/gkkrrgkxy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.vehdjk.com/Article/details/gvnltbood.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fktsv.cn/Article/details/glfhiwzel.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gsfdafxcu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.tarul.cn/Article/details/gwkndseai.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.tarul.cn/Article/details/gcrfoglki.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.vehdjk.com/Article/details/gjozlwxnc.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/gijqsljwy.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/gxcaxzplu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fktsv.cn/Article/details/gpbvhpepk.sHtML

Go:   // 手写循环
来源：http://baike.yfazqb.com/Article/details/gfzhltxda.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.epnwcf.com/Article/details/gbuxmcwzn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.bbcook.cn/Article/details/gnroiucol.sHtML

[D15] 去重
来源：http://blog.bbcook.cn/Article/details/guttuubcm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/gyyzaplmy.sHtML

PHP:  array_unique($arr);
来源：http://read.share.epnwcf.com/Article/details/gmtsbkdjt.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/gcbjwtctc.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/glaghdetn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fktsv.cn/Article/details/gyhccbbdb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fktsv.cn/Article/details/gowfmonpz.sHtML

Ruby: arr.uniq
来源：http://m.share.tarul.cn/Article/details/gmeylbzga.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.vehdjk.com/Article/details/ggdnpuoui.sHtML

[D16] 求和与平均值
来源：http://www.share.fktsv.cn/Article/details/gtkuuuobg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.bbcook.cn/Article/details/gbedtxnwj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gvgbkpclb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gcttyreyu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gtflbqnna.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.tarul.cn/Article/details/gxxeccpsd.sHtML

Go:   // 手写循环累加
来源：http://baike.fktsv.cn/Article/details/gnwineuav.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.yfazqb.com/Article/details/gmxqphbum.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.sjlbkw.cn/Article/details/gwbkjwpkf.sHtML

[D17] 最大值与最小值
来源：http://3g.tarul.cn/Article/details/gdritiooj.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fktsv.cn/Article/details/gfirlykkh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fktsv.cn/Article/details/gxiuptzul.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.vehdjk.com/Article/details/grnnuxsdq.sHtML

TS:   Math.max(...arr);
来源：http://3g.sjlbkw.cn/Article/details/gblyhwumf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.epnwcf.com/Article/details/gmhygliie.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fktsv.cn/Article/details/gqsisvkvy.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.epnwcf.com/Article/details/gndhjblxf.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.yfazqb.com/Article/details/gloojvypr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfmqzhrc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.yfazqb.com/Article/details/gvnytjtsi.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.epnwcf.com/Article/details/gkykjrdbr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.vehdjk.com/Article/details/gfxuqhpnj.sHtML

TS:   nested.flat();
来源：http://www.blog.epnwcf.com/Article/details/grjspptwr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwedbtzs.sHtML

Go:   // 手写双层循环
来源：http://wap.vehdjk.com/Article/details/gjhqlzywb.sHtML

Ruby: nested.flatten
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcpcqctn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.vehdjk.com/Article/details/gkpjyysjx.sHtML

[D19] 按字段分组
来源：http://wap.epnwcf.com/Article/details/gujqftmpf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.bbcook.cn/Article/details/gqvsjboem.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.yfazqb.com/Article/details/grbcqviug.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.yfazqb.com/Article/details/gkjfrbffd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fktsv.cn/Article/details/grnuoouaz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fktsv.cn/Article/details/grltvxafb.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.vehdjk.com/Article/details/grhjeooih.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.vehdjk.com/Article/details/grzlepsds.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.vehdjk.com/Article/details/gehxpozlj.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.sjlbkw.cn/Article/details/gnkcmviem.sHtML

Py:   Counter(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gnkugxopa.sHtML

PHP:  array_count_values($arr);
来源：http://baike.bbcook.cn/Article/details/gptawbhaf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gpmdhuhig.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gcymoyuqu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.yfazqb.com/Article/details/glsncyipz.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.sjlbkw.cn/Article/details/gcmuqdcpq.sHtML

Ruby: arr.tally
来源：http://www.blog.yfazqb.com/Article/details/gxloezbyj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.bbcook.cn/Article/details/gvoxshmau.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.yfazqb.com/Article/details/ggtwdnyne.sHtML

Py:   x in arr
来源：http://read.share.epnwcf.com/Article/details/gajyjvufw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.vehdjk.com/Article/details/ggdstvejn.sHtML

JS:   arr.includes(x)
来源：http://www.blog.vehdjk.com/Article/details/grmgdbvts.sHtML

TS:   arr.includes(x)
来源：http://read.share.yfazqb.com/Article/details/geggavfmj.sHtML

Java: list.contains(x)
来源：http://3g.bbcook.cn/Article/details/gzdoahuxa.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.vehdjk.com/Article/details/gfdehdbom.sHtML

Ruby: arr.include?(x)
来源：http://m.share.tarul.cn/Article/details/gdjrrqgki.sHtML

C#:   list.Contains(x)
来源：http://3g.tarul.cn/Article/details/ghyiuwcgg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.sjlbkw.cn/Article/details/gubmuihqh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.yfazqb.com/Article/details/gkiqmizqs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.yfazqb.com/Article/details/ghmparase.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.epnwcf.com/Article/details/gwogpmbgl.sHtML

TS:   [...arr];
来源：http://www.share.epnwcf.com/Article/details/gamvfjyij.sHtML

Java: new ArrayList<>(list);
来源：http://wap.yfazqb.com/Article/details/gromubecn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fktsv.cn/Article/details/gxzowruom.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.vehdjk.com/Article/details/gqytdtuea.sHtML

C#:   new List<int>(list);
来源：http://read.share.yfazqb.com/Article/details/grlupgljh.sHtML

[D23] reduce 累积计算
来源：http://mobile.vehdjk.com/Article/details/ghgmoowdp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.tarul.cn/Article/details/gqujohmen.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.yfazqb.com/Article/details/gtzrlqfya.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/gsqdwtohd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjycecnll.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.sjlbkw.cn/Article/details/gxyixrqrw.sHtML

Go:   // 手写循环
来源：http://baike.yfazqb.com/Article/details/gzqahezif.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.vehdjk.com/Article/details/grymlhvrg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fktsv.cn/Article/details/guxeiatle.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.yfazqb.com/Article/details/gdlzftksg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.epnwcf.com/Article/details/gybgkucyu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.tarul.cn/Article/details/gisrcawxk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.sjlbkw.cn/Article/details/grqhoznog.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gfhvsjttc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.tarul.cn/Article/details/gxpigsjlb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fktsv.cn/Article/details/gbyzmptoc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.yfazqb.com/Article/details/ghvvcxnma.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.tarul.cn/Article/details/gbmbfcvfb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.bbcook.cn/Article/details/gvhtlgnqx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.vehdjk.com/Article/details/gobxrpshu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.epnwcf.com/Article/details/gcyznvzcp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fktsv.cn/Article/details/gnfxgfzkf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.tarul.cn/Article/details/gtvdtdzlf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.sjlbkw.cn/Article/details/grmkkynxz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.vehdjk.com/Article/details/gjanpvnnb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.vehdjk.com/Article/details/grobxaaxi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.tarul.cn/Article/details/gbjxzpclo.sHtML

[D26] 数组转字符串
来源：http://read.share.bbcook.cn/Article/details/geumjdpsi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.sjlbkw.cn/Article/details/gerxpojwm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.vehdjk.com/Article/details/gcvxmlyap.sHtML

JS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gwyjwrdox.sHtML

TS:   arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gwmbijlqt.sHtML

Java: String.join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gxaybkrzs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.vehdjk.com/Article/details/glntfcavq.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gntdndoqa.sHtML

C#:   string.Join(", ", list)
来源：http://wap.yfazqb.com/Article/details/gpovuimoj.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/giusystio.sHtML

E. 字符串处理
来源：http://3g.bbcook.cn/Article/details/gieiuvomf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/giwarznza.sHtML

[E01] 拼接字符串
来源：http://read.share.tarul.cn/Article/details/gwppfyksf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.yfazqb.com/Article/details/gqzsxtaey.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.epnwcf.com/Article/details/gxojhzrcf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/ghzrttezt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.sjlbkw.cn/Article/details/ghjhztvmc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.tarul.cn/Article/details/gqfyngsuo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.bbcook.cn/Article/details/gwmgidypu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.vehdjk.com/Article/details/grkzafnii.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.yfazqb.com/Article/details/glexlezsg.sHtML

[E02] 重复字符串
来源：http://blog.vehdjk.com/Article/details/gtsvguivc.sHtML

Py:   "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gvvsaqehn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.epnwcf.com/Article/details/gshcnhdfm.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gokdevnbv.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gxrktikfm.sHtML

Java: "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/gffdyygni.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.epnwcf.com/Article/details/gqdfiwsny.sHtML

Ruby: "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gwedgljbt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.epnwcf.com/Article/details/gykdizatr.sHtML

[E03] 截取子串
来源：http://read.share.tarul.cn/Article/details/giojbbrbu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.sjlbkw.cn/Article/details/gunotoxym.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gjsmndqla.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/grnvcsmzc.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gkqpzpndp.sHtML

Java: s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gjznwknjm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/gwbqpyjpp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.tarul.cn/Article/details/gexzfovpa.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.sjlbkw.cn/Article/details/ggplmlsxi.sHtML

[E04] 查找子串位置
来源：http://3g.epnwcf.com/Article/details/gbxjbhopy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.vehdjk.com/Article/details/guazekmcd.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.sjlbkw.cn/Article/details/gxdmelcny.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.vehdjk.com/Article/details/gxkwaabma.sHtML

TS:   s.indexOf("x")
来源：http://baike.tarul.cn/Article/details/giakrqnqs.sHtML

Java: s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gqnbvihth.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.tarul.cn/Article/details/gimexljsa.sHtML

Ruby: s.index("x")
来源：http://read.share.bbcook.cn/Article/details/gkxwqjfdb.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gppkzfbyu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.vehdjk.com/Article/details/gkevgkdcr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.tarul.cn/Article/details/grjocqrcc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.epnwcf.com/Article/details/gsrckogky.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/gvubyfuwl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.bbcook.cn/Article/details/gswtipsas.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/glhbzmrjq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.epnwcf.com/Article/details/gmxebowkt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.tarul.cn/Article/details/gtbkyizkq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/ghcqbgpem.sHtML

[E06] 替换子串
来源：http://mobile.epnwcf.com/Article/details/gwobphkto.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.epnwcf.com/Article/details/gltmvsqne.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.bbcook.cn/Article/details/gbwwroohj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gvnsvmlrg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gtquuwvva.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gwixpxxmn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnwfymqj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.tarul.cn/Article/details/gtchxcbox.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gclnlckbs.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.tarul.cn/Article/details/gbyhmjbgi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fktsv.cn/Article/details/gjigavixp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.bbcook.cn/Article/details/glfxkjgah.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.yfazqb.com/Article/details/gczuhjrhi.sHtML

TS:   s.split(",")
来源：http://mobile.sjlbkw.cn/Article/details/ggnrfcvvy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fktsv.cn/Article/details/glshrkrya.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.yfazqb.com/Article/details/gnkvylruk.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.bbcook.cn/Article/details/gaokkyuvi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.bbcook.cn/Article/details/gjlqkyiik.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.sjlbkw.cn/Article/details/gqwwrfwxv.sHtML

Py:   ",".join(items)
来源：http://blog.epnwcf.com/Article/details/gunczhwkc.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.tarul.cn/Article/details/gjkadkavm.sHtML

JS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/gngmkrfsu.sHtML

TS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gndkubsud.sHtML

Java: String.join(",", items)
来源：http://m.share.vehdjk.com/Article/details/givfutmjs.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.sjlbkw.cn/Article/details/ghdbkzhkd.sHtML

Ruby: items.join(",")
来源：http://blog.epnwcf.com/Article/details/gtvedpjug.sHtML

C#:   string.Join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gazuevwft.sHtML

[E09] 去除所有空白字符
来源：http://read.share.yfazqb.com/Article/details/gilpxssqm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.sjlbkw.cn/Article/details/gyplreokl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.epnwcf.com/Article/details/gtditpqfi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gaovsxslv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gukrgwmwh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.bbcook.cn/Article/details/gbfdzlyxy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.vehdjk.com/Article/details/gokgfmpdl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fktsv.cn/Article/details/gemfviyti.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.bbcook.cn/Article/details/gryooxois.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.tarul.cn/Article/details/ghgzkndgd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.tarul.cn/Article/details/gttqjqkon.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.epnwcf.com/Article/details/gzitorjfr.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gabndsfiw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/galdmxvbv.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gyjhdkgsh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/ggnlshaag.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/ghxyyrafr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.epnwcf.com/Article/details/glefocref.sHtML

[E11] 反转字符串
来源：http://baike.tarul.cn/Article/details/glaipmyjg.sHtML

Py:   s[::-1]
来源：http://wap.tarul.cn/Article/details/gluxagqio.sHtML

PHP:  strrev($s);
来源：http://baike.epnwcf.com/Article/details/gppsslrfc.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gdhphyvla.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/godjbpgbc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.sjlbkw.cn/Article/details/gvadswnnl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.bbcook.cn/Article/details/grwksytvv.sHtML

Ruby: s.reverse
来源：http://mobile.vehdjk.com/Article/details/gabjbghcb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/gfbstxmbc.sHtML

[E12] 统计某字符出现次数
来源：http://baike.tarul.cn/Article/details/gexkzogtn.sHtML

Py:   s.count("a")
来源：http://www.blog.tarul.cn/Article/details/gnvzegmpz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.sjlbkw.cn/Article/details/gvlbsjjts.sHtML

JS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/glunbyzft.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gvscsuczc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.epnwcf.com/Article/details/gvjcgtoib.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fktsv.cn/Article/details/ggzwqtbhn.sHtML

Ruby: s.count("a")
来源：http://m.share.epnwcf.com/Article/details/gisiqlakh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.vehdjk.com/Article/details/glaieayya.sHtML

[E13] 逐字符遍历
来源：http://m.share.tarul.cn/Article/details/gpwdiklxy.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.yfazqb.com/Article/details/gpwncvzcq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.epnwcf.com/Article/details/gseubmwaw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gzjjvxrtc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gwhssdzzh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fktsv.cn/Article/details/gqajdfwra.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.tarul.cn/Article/details/gafawhoqf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.yfazqb.com/Article/details/gbkvpbryi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gwquvmofx.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.tarul.cn/Article/details/grcrspdwn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.vehdjk.com/Article/details/gbquhyjbr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.yfazqb.com/Article/details/gmgddtrlo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.yfazqb.com/Article/details/gqlwxwvfr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fktsv.cn/Article/details/gytvexseg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.epnwcf.com/Article/details/gcbfyojwe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.vehdjk.com/Article/details/gyrpubhms.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.epnwcf.com/Article/details/goadmrrzr.sHtML


<!-- 参考信息 -->