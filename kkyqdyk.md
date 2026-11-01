代发 wailian999

TS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/gkeozsloj.sHtML

Java: list.subList(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gllkwwapa.sHtML

Go:   arr[1:4]
来源：http://read.share.epnwcf.com/Article/details/gkusreshy.sHtML

Ruby: arr[1, 3]
来源：http://3g.tarul.cn/Article/details/gtzvjugel.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.bbcook.cn/Article/details/guwyvmlbk.sHtML

[D08] 合并两个数组
来源：http://baike.bbcook.cn/Article/details/gvyaojyjb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.bbcook.cn/Article/details/gssfssbrf.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.tarul.cn/Article/details/gqzviqylq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.tarul.cn/Article/details/gjaeoismj.sHtML

TS:   [...a, ...b];
来源：http://read.share.bbcook.cn/Article/details/gqbaxyuir.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.bbcook.cn/Article/details/gnpiytfwl.sHtML

Go:   append(a, b...)
来源：http://www.share.sjlbkw.cn/Article/details/gfuxlqqrz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.vehdjk.com/Article/details/gdtilasws.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.yfazqb.com/Article/details/gskzpokag.sHtML

[D09] 排序（升序）
来源：http://baike.tarul.cn/Article/details/giflcnmro.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/ggjmvcotg.sHtML

PHP:  sort($arr);
来源：http://wap.vehdjk.com/Article/details/gjuxfdibj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.bbcook.cn/Article/details/gyxacwckm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.epnwcf.com/Article/details/gfyyojolm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.vehdjk.com/Article/details/gsfzrifcn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gntcitdge.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/gkvhhfiuj.sHtML

C#:   list.Sort();
来源：http://read.share.sjlbkw.cn/Article/details/gbwiksjql.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.tarul.cn/Article/details/gglatknuo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.yfazqb.com/Article/details/goveznsoa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gktabmsnh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.vehdjk.com/Article/details/gxwcnqjyr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.sjlbkw.cn/Article/details/gfkwxjvjz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.sjlbkw.cn/Article/details/gbepxywai.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fktsv.cn/Article/details/gxpmhlalf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.tarul.cn/Article/details/gvapcedtq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.yfazqb.com/Article/details/gvimvvgqq.sHtML

[D11] 反转数组
来源：http://wap.epnwcf.com/Article/details/gpqsvqdea.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfpyyfii.sHtML

PHP:  array_reverse($arr);
来源：http://blog.vehdjk.com/Article/details/gdfwenrbd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fktsv.cn/Article/details/gnrjiwmcu.sHtML

TS:   [...arr].reverse();
来源：http://www.share.bbcook.cn/Article/details/gkvshfdmg.sHtML

Java: Collections.reverse(list);
来源：http://blog.yfazqb.com/Article/details/gsdrparcl.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.yfazqb.com/Article/details/ghtybcmwz.sHtML

Ruby: arr.reverse
来源：http://read.share.sjlbkw.cn/Article/details/gzjjiwtqc.sHtML

C#:   list.Reverse();
来源：http://www.blog.vehdjk.com/Article/details/gjrqqpcci.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fktsv.cn/Article/details/ghlfatkyf.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.tarul.cn/Article/details/gbenldwdq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyfmvqpz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.bbcook.cn/Article/details/gfnirvuad.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.bbcook.cn/Article/details/gfbtwimqf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.vehdjk.com/Article/details/gunaucrjt.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.tarul.cn/Article/details/gpqjjfqye.sHtML

Ruby: arr.index(x)
来源：http://3g.vehdjk.com/Article/details/gjvfwxlvi.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.tarul.cn/Article/details/gjboumabs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.vehdjk.com/Article/details/gglfemumh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.vehdjk.com/Article/details/gmmrotjwq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.tarul.cn/Article/details/goqwwaood.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.epnwcf.com/Article/details/grfwxvvde.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/geppuywqg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.bbcook.cn/Article/details/gbmztwlof.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fktsv.cn/Article/details/goveuqzll.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.yfazqb.com/Article/details/gxwpffiri.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.yfazqb.com/Article/details/gpzfxnlce.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.epnwcf.com/Article/details/gbobitfar.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gwfowwiei.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.sjlbkw.cn/Article/details/guggmiwfk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.vehdjk.com/Article/details/gqjazdmje.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.yfazqb.com/Article/details/gctfvvfxh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.yfazqb.com/Article/details/gibqzgpjz.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/gxbqxwojb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.epnwcf.com/Article/details/grrszooxu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.epnwcf.com/Article/details/gwizgvhsw.sHtML

[D15] 去重
来源：http://baike.sjlbkw.cn/Article/details/ghwrpfehh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/geykwizbv.sHtML

PHP:  array_unique($arr);
来源：http://www.share.vehdjk.com/Article/details/gawxfsxyv.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gjcjtfwek.sHtML

TS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gelpzywzl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.epnwcf.com/Article/details/gcdalquem.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fktsv.cn/Article/details/gnxfrcamb.sHtML

Ruby: arr.uniq
来源：http://wap.bbcook.cn/Article/details/gkuqliqhx.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.bbcook.cn/Article/details/gczseudga.sHtML

[D16] 求和与平均值
来源：http://www.m.share.sjlbkw.cn/Article/details/gpebbgnvb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.yfazqb.com/Article/details/gfxmixbnp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/ggbraailj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.vehdjk.com/Article/details/georlbgjd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/gkpvdshvu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.vehdjk.com/Article/details/gcjqhmekn.sHtML

Go:   // 手写循环累加
来源：http://blog.yfazqb.com/Article/details/gluhuctap.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fktsv.cn/Article/details/gpusarqhb.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.sjlbkw.cn/Article/details/gwyxtcxxu.sHtML

[D17] 最大值与最小值
来源：http://www.share.yfazqb.com/Article/details/gxyttzdog.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.yfazqb.com/Article/details/gymvvlhxz.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.tarul.cn/Article/details/gilcwtmqp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.bbcook.cn/Article/details/grkaonfmo.sHtML

TS:   Math.max(...arr);
来源：http://mobile.epnwcf.com/Article/details/glwrddume.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.sjlbkw.cn/Article/details/glqgksfiz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fktsv.cn/Article/details/gbsstopgm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.yfazqb.com/Article/details/gnkwoeivo.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/gobfutppu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fktsv.cn/Article/details/grnwnimdf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.yfazqb.com/Article/details/gdayuraxi.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.tarul.cn/Article/details/ghnpsdjgv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.tarul.cn/Article/details/gvavhrwzd.sHtML

TS:   nested.flat();
来源：http://wap.bbcook.cn/Article/details/giixovdxo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.tarul.cn/Article/details/gskxfzotn.sHtML

Go:   // 手写双层循环
来源：http://3g.tarul.cn/Article/details/gxuzyprap.sHtML

Ruby: nested.flatten
来源：http://wap.bbcook.cn/Article/details/gxlwvvfup.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.vehdjk.com/Article/details/gtffbfcac.sHtML

[D19] 按字段分组
来源：http://www.share.sjlbkw.cn/Article/details/gexwmurgd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.tarul.cn/Article/details/gjgzbccvi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.yfazqb.com/Article/details/gihgnxkvl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.epnwcf.com/Article/details/gonxbjlgb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/gwkyvpjud.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/gqmqcwepj.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.epnwcf.com/Article/details/gboxrkfgw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.bbcook.cn/Article/details/gcyxhyqod.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fktsv.cn/Article/details/gaqjzlozi.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.yfazqb.com/Article/details/gteoggsyf.sHtML

Py:   Counter(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gjmrusbls.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.epnwcf.com/Article/details/gwiplsvuq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/gcozzdyud.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/gmujeqcpq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.vehdjk.com/Article/details/gsgeqdaue.sHtML

Go:   // 手写 map[T]int
来源：http://wap.yfazqb.com/Article/details/ghkoxwjaf.sHtML

Ruby: arr.tally
来源：http://wap.vehdjk.com/Article/details/gjzqnetgo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fktsv.cn/Article/details/gkyovywkj.sHtML

[D21] 判断是否包含某元素
来源：http://wap.yfazqb.com/Article/details/gwmnggson.sHtML

Py:   x in arr
来源：http://wap.epnwcf.com/Article/details/grmflwmwq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.bbcook.cn/Article/details/gmikrptxb.sHtML

JS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/gygysrunn.sHtML

TS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/gxdwnkjuf.sHtML

Java: list.contains(x)
来源：http://mobile.epnwcf.com/Article/details/grzhkqkoc.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.yfazqb.com/Article/details/gsulfkbiq.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gdqwblzmj.sHtML

C#:   list.Contains(x)
来源：http://wap.bbcook.cn/Article/details/gfopnhscx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.tarul.cn/Article/details/gsuptcfbc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.vehdjk.com/Article/details/ghbrednkt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fktsv.cn/Article/details/gfqudslhs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.tarul.cn/Article/details/gnklbzpcj.sHtML

TS:   [...arr];
来源：http://www.m.share.yfazqb.com/Article/details/gcpplssoh.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.tarul.cn/Article/details/gvptpcurr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fktsv.cn/Article/details/ggdqwindj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.tarul.cn/Article/details/gwunproka.sHtML

C#:   new List<int>(list);
来源：http://mobile.tarul.cn/Article/details/gacestzhl.sHtML

[D23] reduce 累积计算
来源：http://www.share.epnwcf.com/Article/details/ggcusbiuz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.epnwcf.com/Article/details/gnbfpouqp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gxugjrlbp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/grbjlyqee.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.epnwcf.com/Article/details/gjqsxayiv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.yfazqb.com/Article/details/gmnghpvtw.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/ggmjxxdsz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.epnwcf.com/Article/details/gunksmdxh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.bbcook.cn/Article/details/ggrbczrkt.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.sjlbkw.cn/Article/details/gcsywrcso.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gvivkvxqh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyfawyau.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.bbcook.cn/Article/details/gexubhlak.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gauayhajc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.vehdjk.com/Article/details/grcqmhwfj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.yfazqb.com/Article/details/gmkmhkeig.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.vehdjk.com/Article/details/glhkllbem.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.tarul.cn/Article/details/gaqxnwfcu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.vehdjk.com/Article/details/gsobbwmsj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.tarul.cn/Article/details/ghzijhsfe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fktsv.cn/Article/details/gjlnsjasq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.yfazqb.com/Article/details/gznvzlhyv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.sjlbkw.cn/Article/details/gatixqsnx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fktsv.cn/Article/details/gljzipyqm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.bbcook.cn/Article/details/gwvfrvuar.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fktsv.cn/Article/details/gaafeyipx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/grfydtffc.sHtML

[D26] 数组转字符串
来源：http://read.share.tarul.cn/Article/details/gkaettjnf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.epnwcf.com/Article/details/gztjpwrlh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.epnwcf.com/Article/details/guufeyruu.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtslsfhh.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/ghauloifr.sHtML

Java: String.join(", ", list)
来源：http://www.blog.bbcook.cn/Article/details/gurriemqn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.vehdjk.com/Article/details/gypojxndc.sHtML

Ruby: arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gbejibcte.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gnqjqkawg.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbdlytdlf.sHtML

E. 字符串处理
来源：http://mobile.sjlbkw.cn/Article/details/gumeauufk.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ggywwhcko.sHtML

[E01] 拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gefcfvcfm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.bbcook.cn/Article/details/gjutbiijv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.tarul.cn/Article/details/gcubhxxuc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/gtvmksyic.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gpijqdmvy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.tarul.cn/Article/details/gsulzksoq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.yfazqb.com/Article/details/gedfgkmop.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.sjlbkw.cn/Article/details/gubuirlcv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gcitivmzw.sHtML

[E02] 重复字符串
来源：http://www.blog.epnwcf.com/Article/details/gaeqyulmf.sHtML

Py:   "ab" * 3
来源：http://www.share.bbcook.cn/Article/details/gekppbbxm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.yfazqb.com/Article/details/glbiwzvwe.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/giyausdkr.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gmddoimxr.sHtML

Java: "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gdsdxgtbx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.vehdjk.com/Article/details/gipsctgbj.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fktsv.cn/Article/details/gocytcrca.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.tarul.cn/Article/details/gnxdyjrcs.sHtML

[E03] 截取子串
来源：http://blog.bbcook.cn/Article/details/guoexpzwb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.vehdjk.com/Article/details/gwolmazae.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gcurffgqc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gdhthnmgx.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gvmhzmkug.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gbjdqsabk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.yfazqb.com/Article/details/grwxroter.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.vehdjk.com/Article/details/gantbbzmp.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.vehdjk.com/Article/details/gcphdpjnu.sHtML

[E04] 查找子串位置
来源：http://mobile.tarul.cn/Article/details/gniubirno.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.bbcook.cn/Article/details/gdfqbpfpa.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.sjlbkw.cn/Article/details/glzcoiagx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fktsv.cn/Article/details/gsbulmhoq.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gfcnlisfv.sHtML

Java: s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gqxdswneo.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.vehdjk.com/Article/details/gzuiwqeju.sHtML

Ruby: s.index("x")
来源：http://mobile.tarul.cn/Article/details/ggkiaxumd.sHtML

C#:   s.IndexOf("x")
来源：http://baike.bbcook.cn/Article/details/gezyfxont.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.vehdjk.com/Article/details/gzgqndbkd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fktsv.cn/Article/details/gaovenelm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.vehdjk.com/Article/details/grhrzymmd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gpnmcmqhq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.tarul.cn/Article/details/gtvqjhhhq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.tarul.cn/Article/details/gwwujqeuw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.yfazqb.com/Article/details/gjveggbdr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.epnwcf.com/Article/details/gikszfgjr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fktsv.cn/Article/details/grnywzliz.sHtML

[E06] 替换子串
来源：http://3g.tarul.cn/Article/details/gkjwtpaor.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/gponyjzbe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.yfazqb.com/Article/details/grcamgnlt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gdaxntsem.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gnkqscwfw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/garvikcay.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gxjqakbng.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.vehdjk.com/Article/details/gwugiayof.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.tarul.cn/Article/details/grbpjtnei.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.bbcook.cn/Article/details/gtruvqggm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.sjlbkw.cn/Article/details/gradhrlip.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.tarul.cn/Article/details/gvlfbbzhy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.bbcook.cn/Article/details/gkjawuqzl.sHtML

TS:   s.split(",")
来源：http://3g.sjlbkw.cn/Article/details/gbfozgyey.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.bbcook.cn/Article/details/gieviozpb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.tarul.cn/Article/details/grlxzjymo.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.vehdjk.com/Article/details/gsoknkxzw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fktsv.cn/Article/details/gkqbloegv.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.tarul.cn/Article/details/gwvzrlmrr.sHtML

Py:   ",".join(items)
来源：http://www.blog.bbcook.cn/Article/details/gapkzymrn.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpshnmoy.sHtML

JS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/gkuksqsxc.sHtML

TS:   items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gpaqqojgf.sHtML

Java: String.join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gnkxahmxb.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.yfazqb.com/Article/details/gixlmrrcc.sHtML

Ruby: items.join(",")
来源：http://www.share.vehdjk.com/Article/details/ggrizwudn.sHtML

C#:   string.Join(",", items)
来源：http://3g.sjlbkw.cn/Article/details/gmhtqecad.sHtML

[E09] 去除所有空白字符
来源：http://baike.bbcook.cn/Article/details/gagovdptc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.epnwcf.com/Article/details/gyybfswix.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.vehdjk.com/Article/details/gritxbvan.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/gjuqojtev.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.bbcook.cn/Article/details/gxigwdjwz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.epnwcf.com/Article/details/guojlkuub.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.yfazqb.com/Article/details/gutnvkise.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.yfazqb.com/Article/details/gxmxqchrv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gvzuogzgu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.sjlbkw.cn/Article/details/gcqpesjky.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gmogcxdby.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fktsv.cn/Article/details/gmqobmbiu.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gzwvvzbbq.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gypbiophd.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gwlptgvad.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/ghprnzyok.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gokvqvvnf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.sjlbkw.cn/Article/details/gdoaoebld.sHtML

[E11] 反转字符串
来源：http://read.share.tarul.cn/Article/details/gjzsuixea.sHtML

Py:   s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gsseqrndq.sHtML

PHP:  strrev($s);
来源：http://blog.vehdjk.com/Article/details/gtxlhysao.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gorxczcrp.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/guowsroti.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.epnwcf.com/Article/details/gzayjiaso.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.tarul.cn/Article/details/gaksdloqi.sHtML

Ruby: s.reverse
来源：http://read.share.fktsv.cn/Article/details/geecqhlgl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gensgslbe.sHtML

[E12] 统计某字符出现次数
来源：http://baike.bbcook.cn/Article/details/gngfypufu.sHtML

Py:   s.count("a")
来源：http://3g.fktsv.cn/Article/details/gowmicttc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fktsv.cn/Article/details/ggbztksyg.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/gxtbjlwal.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gyvnkajjb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.bbcook.cn/Article/details/gdxvcilqb.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.yfazqb.com/Article/details/gwnaksowj.sHtML

Ruby: s.count("a")
来源：http://baike.yfazqb.com/Article/details/gdxjxxhso.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.bbcook.cn/Article/details/guluexvds.sHtML

[E13] 逐字符遍历
来源：http://wap.yfazqb.com/Article/details/gaclmfypt.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.tarul.cn/Article/details/gpykwtlor.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.tarul.cn/Article/details/gowmbslgq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.vehdjk.com/Article/details/gbrdgliwh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/grqruuins.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.vehdjk.com/Article/details/gljvhmidt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.bbcook.cn/Article/details/gnfmtafcj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.bbcook.cn/Article/details/gqteyxfgv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.vehdjk.com/Article/details/gkkntxaiv.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.yfazqb.com/Article/details/gqyzmlulq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.yfazqb.com/Article/details/guxzndiad.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.bbcook.cn/Article/details/gtquaqqcc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.epnwcf.com/Article/details/gdnbuazcp.sHtML


<!-- 参考信息 -->