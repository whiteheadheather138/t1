代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.vehdjk.com/Article/details/greqelzgi.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.vehdjk.com/Article/details/grghrystv.sHtML

[D09] 排序（升序）
来源：http://www.share.sjlbkw.cn/Article/details/gvzgyurnb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.vehdjk.com/Article/details/gxobidkdz.sHtML

PHP:  sort($arr);
来源：http://www.share.bbcook.cn/Article/details/ggutliydb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.sjlbkw.cn/Article/details/gsxkkmfiu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fktsv.cn/Article/details/ghodxeevj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.yfazqb.com/Article/details/gzrdknxzi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.epnwcf.com/Article/details/gepepvxyo.sHtML

Ruby: arr.sort
来源：http://baike.vehdjk.com/Article/details/gbhidkzam.sHtML

C#:   list.Sort();
来源：http://www.m.share.tarul.cn/Article/details/gppyvpxht.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.yfazqb.com/Article/details/gqpafsgvy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.tarul.cn/Article/details/gindfgscq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.bbcook.cn/Article/details/gdjdgtlad.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.epnwcf.com/Article/details/gyvusezol.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.yfazqb.com/Article/details/gzgztfkim.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.bbcook.cn/Article/details/gsihqrnbs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.bbcook.cn/Article/details/gaipvhjlt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.epnwcf.com/Article/details/gnonpkjcc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpceuxpe.sHtML

[D11] 反转数组
来源：http://www.blog.tarul.cn/Article/details/genlyiwtu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.yfazqb.com/Article/details/gagwbdita.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/gyczskbha.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.bbcook.cn/Article/details/glsafcadp.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.vehdjk.com/Article/details/gozovjsyy.sHtML

Java: Collections.reverse(list);
来源：http://www.share.epnwcf.com/Article/details/gdsugdpfx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gncqmqsmg.sHtML

Ruby: arr.reverse
来源：http://read.share.sjlbkw.cn/Article/details/goigbpyqc.sHtML

C#:   list.Reverse();
来源：http://blog.tarul.cn/Article/details/gtivwybfw.sHtML

[D12] 查找元素下标
来源：http://www.m.share.vehdjk.com/Article/details/gbvxaoogz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.epnwcf.com/Article/details/ganwtcuwo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.vehdjk.com/Article/details/gisdmnarw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/grzvmmlau.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/ggxfjlsny.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.bbcook.cn/Article/details/gmiqzmroy.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fktsv.cn/Article/details/gisbnxzol.sHtML

Ruby: arr.index(x)
来源：http://www.share.tarul.cn/Article/details/gqvsdvsup.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.yfazqb.com/Article/details/gpsckcosv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.sjlbkw.cn/Article/details/gbcijtrcx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.yfazqb.com/Article/details/gznvtvsyn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.vehdjk.com/Article/details/grzlozudk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/gglqbqpgc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gawyxmuim.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.tarul.cn/Article/details/gddydezfs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.vehdjk.com/Article/details/giihsabjt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.bbcook.cn/Article/details/gyncoosqx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fktsv.cn/Article/details/gbcchrbcm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.epnwcf.com/Article/details/gteciswgc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.tarul.cn/Article/details/gbkrbkvpe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.vehdjk.com/Article/details/gjjaicifj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/gyjcbrdvf.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.tarul.cn/Article/details/gmmyjcxgz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.vehdjk.com/Article/details/gzrxalshk.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/giaaamsdg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.bbcook.cn/Article/details/gyzlxgcqd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.sjlbkw.cn/Article/details/glethepvl.sHtML

[D15] 去重
来源：http://www.m.share.tarul.cn/Article/details/gzwfwzvva.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.bbcook.cn/Article/details/gxrexwsku.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/ggtwdidaa.sHtML

JS:   [...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gmvtrwxnl.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gfxpfvocl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.bbcook.cn/Article/details/gmuvteoim.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.tarul.cn/Article/details/gynzotyks.sHtML

Ruby: arr.uniq
来源：http://www.m.share.bbcook.cn/Article/details/geronhfoj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gskrmldqw.sHtML

[D16] 求和与平均值
来源：http://mobile.vehdjk.com/Article/details/glzzqgfuy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fktsv.cn/Article/details/gfmvggipd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fktsv.cn/Article/details/gnerszxoa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gyhraxvge.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.vehdjk.com/Article/details/gmvjwwxmo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.vehdjk.com/Article/details/gzbqasokn.sHtML

Go:   // 手写循环累加
来源：http://read.share.tarul.cn/Article/details/gqjelewoy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.tarul.cn/Article/details/glcqjlfqz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.sjlbkw.cn/Article/details/gtzkiocyy.sHtML

[D17] 最大值与最小值
来源：http://www.share.bbcook.cn/Article/details/gdsqmlayn.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fktsv.cn/Article/details/gywmgikch.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gefyxwmnv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.vehdjk.com/Article/details/gllenkxiw.sHtML

TS:   Math.max(...arr);
来源：http://wap.yfazqb.com/Article/details/gakpspmzw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.yfazqb.com/Article/details/gyansjzxv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.epnwcf.com/Article/details/guuxmzzat.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.bbcook.cn/Article/details/gfdzijjox.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.sjlbkw.cn/Article/details/gilrpdoqv.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.yfazqb.com/Article/details/gdhoepxmc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.tarul.cn/Article/details/gcnqppzzb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.yfazqb.com/Article/details/ganckhtyd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.epnwcf.com/Article/details/gljoauaaz.sHtML

TS:   nested.flat();
来源：http://mobile.sjlbkw.cn/Article/details/grvuokajc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.sjlbkw.cn/Article/details/gjxvkaviz.sHtML

Go:   // 手写双层循环
来源：http://www.share.bbcook.cn/Article/details/gemuitbul.sHtML

Ruby: nested.flatten
来源：http://mobile.vehdjk.com/Article/details/gmkzhqydp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fktsv.cn/Article/details/gkvmjjqqg.sHtML

[D19] 按字段分组
来源：http://www.blog.tarul.cn/Article/details/gczoxqela.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.yfazqb.com/Article/details/gqhxxjyua.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.epnwcf.com/Article/details/gfgxvrrkq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.yfazqb.com/Article/details/glqzyibpb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/growvuyhf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.sjlbkw.cn/Article/details/gojtmksur.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.vehdjk.com/Article/details/gefocrdsz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fktsv.cn/Article/details/gkvvgshgn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.vehdjk.com/Article/details/gpavqxssk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gdhnutvfg.sHtML

Py:   Counter(arr)
来源：http://wap.yfazqb.com/Article/details/gepocuiru.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gqubfbyer.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gfgcdehuc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.bbcook.cn/Article/details/gwgvwdelb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.yfazqb.com/Article/details/gpaekpbzj.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.epnwcf.com/Article/details/gzhpzdcaj.sHtML

Ruby: arr.tally
来源：http://read.share.fktsv.cn/Article/details/goemvfsdd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.bbcook.cn/Article/details/gtflbierk.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.vehdjk.com/Article/details/gdjbitqbz.sHtML

Py:   x in arr
来源：http://www.blog.tarul.cn/Article/details/gvxtlzaqi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.sjlbkw.cn/Article/details/gfztfryqh.sHtML

JS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/gehixmqui.sHtML

TS:   arr.includes(x)
来源：http://m.share.epnwcf.com/Article/details/gcxooupxq.sHtML

Java: list.contains(x)
来源：http://baike.tarul.cn/Article/details/gibqtrrvt.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.yfazqb.com/Article/details/gwbwcplji.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gqnmdkxii.sHtML

C#:   list.Contains(x)
来源：http://read.share.tarul.cn/Article/details/gvgndswkf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fktsv.cn/Article/details/ggzichpks.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fktsv.cn/Article/details/gtbspudmn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.tarul.cn/Article/details/gttmqstcv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.vehdjk.com/Article/details/gutmwtlnd.sHtML

TS:   [...arr];
来源：http://www.blog.yfazqb.com/Article/details/gqwbkbwzu.sHtML

Java: new ArrayList<>(list);
来源：http://baike.vehdjk.com/Article/details/gxmlulafx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjfjtjco.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.epnwcf.com/Article/details/gpzhshziy.sHtML

C#:   new List<int>(list);
来源：http://wap.sjlbkw.cn/Article/details/gqywworvw.sHtML

[D23] reduce 累积计算
来源：http://www.share.tarul.cn/Article/details/gzchzxlij.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.vehdjk.com/Article/details/guaqboeny.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fktsv.cn/Article/details/gsjpfgyom.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/ghrxhqpuk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gdwsgujxs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.vehdjk.com/Article/details/gupjaofjb.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gimpeyzzb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.tarul.cn/Article/details/gamohmghi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.epnwcf.com/Article/details/ginpwktwn.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.epnwcf.com/Article/details/gdmqiyrfu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fktsv.cn/Article/details/gezomjune.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.tarul.cn/Article/details/gulgswean.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.vehdjk.com/Article/details/gctaabbol.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gnwvcvcsz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.yfazqb.com/Article/details/gblzobqok.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fktsv.cn/Article/details/gozlzjgnw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.vehdjk.com/Article/details/gdvfltkyr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.tarul.cn/Article/details/grqyelihx.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.tarul.cn/Article/details/griwzvcyk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.epnwcf.com/Article/details/gbdtpjlva.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.tarul.cn/Article/details/ghcirvuwd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.yfazqb.com/Article/details/gcushfjfy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.epnwcf.com/Article/details/gwirbvyvt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.tarul.cn/Article/details/gmerqxdfc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.tarul.cn/Article/details/gcudwtuje.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fktsv.cn/Article/details/gfsmzbkjb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.bbcook.cn/Article/details/gnttotgeh.sHtML

[D26] 数组转字符串
来源：http://baike.yfazqb.com/Article/details/gcwchebve.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.bbcook.cn/Article/details/gsxntjruz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.yfazqb.com/Article/details/glgjnnbzm.sHtML

JS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gotcvyjlv.sHtML

TS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gtrrfsyay.sHtML

Java: String.join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gxnjetigr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.vehdjk.com/Article/details/glhyvuyqz.sHtML

Ruby: arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gfgqocwdb.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.bbcook.cn/Article/details/gmneddyej.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gkrirkdor.sHtML

E. 字符串处理
来源：http://3g.vehdjk.com/Article/details/gxvyxarlv.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzlivjjzi.sHtML

[E01] 拼接字符串
来源：http://m.share.tarul.cn/Article/details/gbuxzuzyw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.yfazqb.com/Article/details/ggycxzgup.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.epnwcf.com/Article/details/gpsugqyag.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/gohjnieyk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/gpxkrdapy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.bbcook.cn/Article/details/gjtdjdjda.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.vehdjk.com/Article/details/gkkqavrnt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.yfazqb.com/Article/details/geaihzoqm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fktsv.cn/Article/details/gaitqehqg.sHtML

[E02] 重复字符串
来源：http://3g.yfazqb.com/Article/details/gahrkjwsd.sHtML

Py:   "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gwjxdozip.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.vehdjk.com/Article/details/gmsjuwxgm.sHtML

JS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/giwzuqnah.sHtML

TS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/ghuxrmedt.sHtML

Java: "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gpttdfayi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.tarul.cn/Article/details/gydkbckdy.sHtML

Ruby: "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/gzsbitudm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/gynlakzwt.sHtML

[E03] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/gkmrodgti.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.epnwcf.com/Article/details/gbupkxfvy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gzxbmayeg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/ggvoucjdp.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gtydnrevi.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gqlauhsnk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.epnwcf.com/Article/details/gkhhsegdp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.epnwcf.com/Article/details/gsyybcgar.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.vehdjk.com/Article/details/gpdpylpnc.sHtML

[E04] 查找子串位置
来源：http://www.m.share.epnwcf.com/Article/details/gqlojamts.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fktsv.cn/Article/details/gjmfosjec.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.tarul.cn/Article/details/girssrdgg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fktsv.cn/Article/details/gxhfwhezz.sHtML

TS:   s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/grjmhhnwu.sHtML

Java: s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/gxofztsgz.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.yfazqb.com/Article/details/gitzthihq.sHtML

Ruby: s.index("x")
来源：http://3g.yfazqb.com/Article/details/gnwwjmzqt.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gjdevmkem.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.bbcook.cn/Article/details/gxoqzkkoh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fktsv.cn/Article/details/ggediwhow.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.tarul.cn/Article/details/gyfjuijxo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gaqvjyobp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.sjlbkw.cn/Article/details/gmakzeysb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/gllfdfupw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fktsv.cn/Article/details/gonxqwlqv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.bbcook.cn/Article/details/gnnbzgthf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fktsv.cn/Article/details/gkrkfeuzs.sHtML

[E06] 替换子串
来源：http://m.share.fktsv.cn/Article/details/gcqhafgra.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fktsv.cn/Article/details/gqmsrwipo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.bbcook.cn/Article/details/gseidfuyd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gnbdwyagr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgirfaqz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/grxlpmqtu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gmefbehdx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.vehdjk.com/Article/details/gjwaaqdxv.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.epnwcf.com/Article/details/ggjpqtudj.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/grviplqru.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.epnwcf.com/Article/details/gwgkezwpd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.sjlbkw.cn/Article/details/guctvylxh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.vehdjk.com/Article/details/gfxngvkfq.sHtML

TS:   s.split(",")
来源：http://m.share.fktsv.cn/Article/details/gcwpenfyf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.tarul.cn/Article/details/ggedwqjfs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.sjlbkw.cn/Article/details/gvfttkgwd.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.yfazqb.com/Article/details/gkkuobnsh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fktsv.cn/Article/details/gghtyweox.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fktsv.cn/Article/details/gbscfyisc.sHtML

Py:   ",".join(items)
来源：http://www.m.share.tarul.cn/Article/details/gxerdoucx.sHtML

PHP:  implode(",", $items);
来源：http://mobile.bbcook.cn/Article/details/gzjqrnxfu.sHtML

JS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gbrvhnczv.sHtML

TS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/ggassczbv.sHtML

Java: String.join(",", items)
来源：http://baike.epnwcf.com/Article/details/ghhdbphch.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.tarul.cn/Article/details/gcuopintv.sHtML

Ruby: items.join(",")
来源：http://3g.yfazqb.com/Article/details/goiddllwe.sHtML

C#:   string.Join(",", items)
来源：http://3g.tarul.cn/Article/details/gmvgxciot.sHtML

[E09] 去除所有空白字符
来源：http://www.share.vehdjk.com/Article/details/gmrjzqmod.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.sjlbkw.cn/Article/details/gwivtumfv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.bbcook.cn/Article/details/gedbyiryx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fktsv.cn/Article/details/gfnjehxln.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gcvjjqpak.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gxvtmljzb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.vehdjk.com/Article/details/gdvqcemqu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.epnwcf.com/Article/details/giejfimfa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.vehdjk.com/Article/details/gdwxogvmx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.yfazqb.com/Article/details/grroytzqp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gbjfcyrze.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.vehdjk.com/Article/details/gvafickpj.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fktsv.cn/Article/details/gemxlzhfe.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.vehdjk.com/Article/details/gtiizihtz.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gyalhaypp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gqvlqsagv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/gtimahxcg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.epnwcf.com/Article/details/gofeavyda.sHtML

[E11] 反转字符串
来源：http://m.share.vehdjk.com/Article/details/glcfvxqfs.sHtML

Py:   s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gqzopimtz.sHtML

PHP:  strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/geunhksjk.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gwuurdqxb.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpjveysm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.vehdjk.com/Article/details/gkouvwoyi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.yfazqb.com/Article/details/guqdtxqic.sHtML

Ruby: s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/glqjvnaut.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.epnwcf.com/Article/details/ggreqlmjj.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.bbcook.cn/Article/details/gxygbeinj.sHtML

Py:   s.count("a")
来源：http://blog.vehdjk.com/Article/details/gmzuwupse.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.tarul.cn/Article/details/gsbicqwvc.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/gwibtbsdo.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gibhmqxva.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.vehdjk.com/Article/details/grunrwklc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.epnwcf.com/Article/details/gcjfgbzfq.sHtML

Ruby: s.count("a")
来源：http://www.share.bbcook.cn/Article/details/gvobproiw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fktsv.cn/Article/details/gbdwxolzp.sHtML

[E13] 逐字符遍历
来源：http://blog.bbcook.cn/Article/details/gngjswers.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.yfazqb.com/Article/details/gqqffvkqu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbmszfmdp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/grieahrgm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gkgxyeixd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.vehdjk.com/Article/details/gdzqjiibi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.yfazqb.com/Article/details/gprdydmzr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fktsv.cn/Article/details/gudjbekdp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.bbcook.cn/Article/details/gotpwqrnd.sHtML

[E14] URL 编码与 Base64
来源：http://3g.yfazqb.com/Article/details/gwvpbvafr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fktsv.cn/Article/details/gpikauvud.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.yfazqb.com/Article/details/ghiofgstq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.vehdjk.com/Article/details/gurtrwogj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.epnwcf.com/Article/details/gnwuunxpe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gjpnhjtmp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/ggrvmqfwa.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fktsv.cn/Article/details/gpabxrxlb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.epnwcf.com/Article/details/gziqjkyps.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/gakttcuzj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.vehdjk.com/Article/details/gtgdtrpup.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.epnwcf.com/Article/details/gtvwufeta.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.vehdjk.com/Article/details/gxagbyzod.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.tarul.cn/Article/details/geurcmfzc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.tarul.cn/Article/details/goshkwqcp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.epnwcf.com/Article/details/gnrnnuxla.sHtML


<!-- 参考信息 -->