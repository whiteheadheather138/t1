代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://read.share.epnwcf.com/Article/details/gtufxppui.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.vehdjk.com/Article/details/geueawhyk.sHtML

[D09] 排序（升序）
来源：http://3g.vehdjk.com/Article/details/gvcjdnahn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gtextqqvv.sHtML

PHP:  sort($arr);
来源：http://www.blog.fktsv.cn/Article/details/gdbxvwuln.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.vehdjk.com/Article/details/gclukvovh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.bbcook.cn/Article/details/gfbbolmtv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.yfazqb.com/Article/details/gyobttxds.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gugyhpedl.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/gbqpdbzke.sHtML

C#:   list.Sort();
来源：http://3g.tarul.cn/Article/details/gskyjhlpm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.vehdjk.com/Article/details/giqwlzfiy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.vehdjk.com/Article/details/gbeeesqev.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.vehdjk.com/Article/details/gjcpjhvxu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.vehdjk.com/Article/details/gzuqgtzyq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gildbquws.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fktsv.cn/Article/details/goxclfqou.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.bbcook.cn/Article/details/gczlettpg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.tarul.cn/Article/details/gzzrjyckm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.tarul.cn/Article/details/gcwamnqic.sHtML

[D11] 反转数组
来源：http://wap.sjlbkw.cn/Article/details/gfmfkjcqi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.sjlbkw.cn/Article/details/gcebrbkwh.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.vehdjk.com/Article/details/gmmhjwvqn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.vehdjk.com/Article/details/gjselvaor.sHtML

TS:   [...arr].reverse();
来源：http://mobile.tarul.cn/Article/details/gobeyxvrc.sHtML

Java: Collections.reverse(list);
来源：http://www.share.vehdjk.com/Article/details/gtdzgoyih.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fktsv.cn/Article/details/geljohket.sHtML

Ruby: arr.reverse
来源：http://m.share.tarul.cn/Article/details/gojosrggj.sHtML

C#:   list.Reverse();
来源：http://www.m.share.sjlbkw.cn/Article/details/glfhfensg.sHtML

[D12] 查找元素下标
来源：http://mobile.yfazqb.com/Article/details/gglrjzyde.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.epnwcf.com/Article/details/getstjnli.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gvlktxkpx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gxflmstzt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fktsv.cn/Article/details/gkhdtmsmm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.vehdjk.com/Article/details/gmmmtsngr.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.tarul.cn/Article/details/gvuxvczfz.sHtML

Ruby: arr.index(x)
来源：http://3g.sjlbkw.cn/Article/details/ggyqdtvnp.sHtML

C#:   list.IndexOf(x);
来源：http://baike.tarul.cn/Article/details/gztpgiajg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fktsv.cn/Article/details/gcshrvnox.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fktsv.cn/Article/details/gpqvzvfro.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.yfazqb.com/Article/details/glnaiwtpu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gnmwsicnd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/gjeuwsdmj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fktsv.cn/Article/details/gevvjlfmf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fktsv.cn/Article/details/goygapqcc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fktsv.cn/Article/details/gkwqqrzdc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.bbcook.cn/Article/details/gondgczrt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fktsv.cn/Article/details/gswzunsko.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.bbcook.cn/Article/details/gntzsyidc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.epnwcf.com/Article/details/ggxgsdcbh.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/gdmcrmrrd.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/gawhantna.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.epnwcf.com/Article/details/gissockua.sHtML

Go:   // 手写循环
来源：http://www.share.sjlbkw.cn/Article/details/gzwisccho.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gsifosddu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gybzuorld.sHtML

[D15] 去重
来源：http://m.share.tarul.cn/Article/details/gqoycphob.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.sjlbkw.cn/Article/details/gddecjyoi.sHtML

PHP:  array_unique($arr);
来源：http://blog.fktsv.cn/Article/details/gbivtxbhg.sHtML

JS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/glktdwckl.sHtML

TS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gdtfdzrjh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.tarul.cn/Article/details/gkkdalfcn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.tarul.cn/Article/details/gtbxrgzxy.sHtML

Ruby: arr.uniq
来源：http://www.share.epnwcf.com/Article/details/gfjrrqidh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.bbcook.cn/Article/details/galcsuaib.sHtML

[D16] 求和与平均值
来源：http://3g.bbcook.cn/Article/details/gjbhlkbfm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fktsv.cn/Article/details/gkrodosjr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.yfazqb.com/Article/details/gukqtifmb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gzcipgcfb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gfjqbxyki.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.yfazqb.com/Article/details/gmzijlhxy.sHtML

Go:   // 手写循环累加
来源：http://blog.fktsv.cn/Article/details/gxngjhcvh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.epnwcf.com/Article/details/gfujglscn.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.tarul.cn/Article/details/gndgeabxr.sHtML

[D17] 最大值与最小值
来源：http://m.share.epnwcf.com/Article/details/geycffqoo.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.tarul.cn/Article/details/gtwilgtgv.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.vehdjk.com/Article/details/guvjnxzju.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.tarul.cn/Article/details/gqiuxhgyj.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/gihyysxux.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.tarul.cn/Article/details/gawbczvhg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gavdwiqkk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.tarul.cn/Article/details/gvtgbhofo.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/gwzxnnrdu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.epnwcf.com/Article/details/gphuokobf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.vehdjk.com/Article/details/gqwqhrmco.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.yfazqb.com/Article/details/ghmuansou.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.vehdjk.com/Article/details/gwpczsewt.sHtML

TS:   nested.flat();
来源：http://read.share.sjlbkw.cn/Article/details/gijqbsgho.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.tarul.cn/Article/details/gmbnedqmy.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjqbrvkr.sHtML

Ruby: nested.flatten
来源：http://m.share.fktsv.cn/Article/details/gpllydidx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.epnwcf.com/Article/details/gopzkdpyc.sHtML

[D19] 按字段分组
来源：http://blog.vehdjk.com/Article/details/gxhputhnq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.tarul.cn/Article/details/gwyslnvwu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.bbcook.cn/Article/details/gwudgteyh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.tarul.cn/Article/details/gtpjkbrud.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fktsv.cn/Article/details/gamjchixr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.vehdjk.com/Article/details/gafisdqsf.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.epnwcf.com/Article/details/gyqovaohz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.tarul.cn/Article/details/ghutciqig.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.epnwcf.com/Article/details/gcenlfldt.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fktsv.cn/Article/details/gvnpbjuni.sHtML

Py:   Counter(arr)
来源：http://www.share.fktsv.cn/Article/details/gjcnoapmq.sHtML

PHP:  array_count_values($arr);
来源：http://3g.sjlbkw.cn/Article/details/gavjubbzq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/giwqudzml.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/gogkotkyr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.tarul.cn/Article/details/ggzbaemjt.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.vehdjk.com/Article/details/gkojhpavm.sHtML

Ruby: arr.tally
来源：http://www.m.share.sjlbkw.cn/Article/details/gakdaiget.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.yfazqb.com/Article/details/gooxefkue.sHtML

[D21] 判断是否包含某元素
来源：http://wap.tarul.cn/Article/details/gfqkjhvnm.sHtML

Py:   x in arr
来源：http://baike.epnwcf.com/Article/details/gqnqsgghb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.tarul.cn/Article/details/gxvcsixbw.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gddatizuu.sHtML

TS:   arr.includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gdkqokcjf.sHtML

Java: list.contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gvwtynlam.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/geibmzmir.sHtML

Ruby: arr.include?(x)
来源：http://wap.bbcook.cn/Article/details/gsszrhteg.sHtML

C#:   list.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/grxunaosf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.bbcook.cn/Article/details/gxejazamv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.yfazqb.com/Article/details/gebzkluex.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.yfazqb.com/Article/details/gvdycepgq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.bbcook.cn/Article/details/gclilyulz.sHtML

TS:   [...arr];
来源：http://3g.bbcook.cn/Article/details/gqgcjjtvp.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gigylqaaa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.epnwcf.com/Article/details/gaxgmcaqv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.tarul.cn/Article/details/gwyyvjmwv.sHtML

C#:   new List<int>(list);
来源：http://mobile.epnwcf.com/Article/details/gsnboywvu.sHtML

[D23] reduce 累积计算
来源：http://m.share.yfazqb.com/Article/details/grgvdkuxq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbgkrcsj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.bbcook.cn/Article/details/gwmopgadj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.bbcook.cn/Article/details/gjeohchfk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.tarul.cn/Article/details/godbybfyn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.yfazqb.com/Article/details/gmamsecup.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/girsyskxg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.epnwcf.com/Article/details/ggqziafmd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fktsv.cn/Article/details/gtxcwegvi.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.epnwcf.com/Article/details/grmyfjvon.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.yfazqb.com/Article/details/gszjhnysw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.yfazqb.com/Article/details/gwabcuyrh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.yfazqb.com/Article/details/gtfmbuyuo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gpzfjaksr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.vehdjk.com/Article/details/gfmyapzdv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.bbcook.cn/Article/details/grvpeqzyn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.bbcook.cn/Article/details/gqxjlhklw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.sjlbkw.cn/Article/details/gtctttwlm.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.bbcook.cn/Article/details/gefuvjgep.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.tarul.cn/Article/details/ghbgnmrrw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.epnwcf.com/Article/details/gxormoxhg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.yfazqb.com/Article/details/gkfyyyans.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.vehdjk.com/Article/details/gqjvtqdmj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.yfazqb.com/Article/details/gonhpshyu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.tarul.cn/Article/details/gexsnblkj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.tarul.cn/Article/details/guusebzwl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.epnwcf.com/Article/details/gdvmxzxik.sHtML

[D26] 数组转字符串
来源：http://baike.fktsv.cn/Article/details/goplrpbtt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.yfazqb.com/Article/details/godqzavtp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fktsv.cn/Article/details/gqozsewjy.sHtML

JS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gzdfzseii.sHtML

TS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/glwuqkwoi.sHtML

Java: String.join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gfzamcgcb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.vehdjk.com/Article/details/ggjzixjwr.sHtML

Ruby: arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gjnumwicr.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.vehdjk.com/Article/details/gheuutavy.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvgsbmdkt.sHtML

E. 字符串处理
来源：http://read.share.tarul.cn/Article/details/gyxhvnqbq.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gcjwkbyyf.sHtML

[E01] 拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gwokxjbjy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.epnwcf.com/Article/details/grmzvcksm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.sjlbkw.cn/Article/details/gtrrmkcdc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.yfazqb.com/Article/details/gcuksjprb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/ghbslxvsm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.bbcook.cn/Article/details/gvzeagpwq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.epnwcf.com/Article/details/goxpvjxzq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.tarul.cn/Article/details/gegfkygpj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gdrqyomsy.sHtML

[E02] 重复字符串
来源：http://www.m.share.fktsv.cn/Article/details/gtvgeaxhl.sHtML

Py:   "ab" * 3
来源：http://read.share.yfazqb.com/Article/details/gtnkaqwxz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.bbcook.cn/Article/details/gocbivazg.sHtML

JS:   "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/gusqaecao.sHtML

TS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gmhvdatot.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/gssanmvgr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.vehdjk.com/Article/details/gqiguugbm.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gxhyfbytu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.epnwcf.com/Article/details/gyjvakqpr.sHtML

[E03] 截取子串
来源：http://www.share.bbcook.cn/Article/details/gamxszjei.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.bbcook.cn/Article/details/gcogdzfbp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gkiwtldbr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gaoolnwhl.sHtML

TS:   s.slice(1, 4)
来源：http://baike.vehdjk.com/Article/details/guznutgon.sHtML

Java: s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/gvafpklxf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.yfazqb.com/Article/details/ggmbgtulw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.yfazqb.com/Article/details/gxfshjwbn.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.tarul.cn/Article/details/gxnbseygs.sHtML

[E04] 查找子串位置
来源：http://m.share.fktsv.cn/Article/details/grajhizsy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.bbcook.cn/Article/details/gxdfuhaeh.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fktsv.cn/Article/details/gvhtkohxw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.tarul.cn/Article/details/gzqytksxz.sHtML

TS:   s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/glblibcbz.sHtML

Java: s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gzyvkcstp.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.sjlbkw.cn/Article/details/ghobizben.sHtML

Ruby: s.index("x")
来源：http://mobile.yfazqb.com/Article/details/gmmjvpklw.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/giqujxstf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.bbcook.cn/Article/details/gymbkibta.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.epnwcf.com/Article/details/glmfkdhiw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.epnwcf.com/Article/details/gocnfdade.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.tarul.cn/Article/details/gftuawtit.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.sjlbkw.cn/Article/details/ggkcocxme.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gntrqwdth.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.yfazqb.com/Article/details/gqhkirthd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.vehdjk.com/Article/details/gxlqdfuul.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fktsv.cn/Article/details/gdbgabqse.sHtML

[E06] 替换子串
来源：http://m.share.tarul.cn/Article/details/gjivmgirc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gkcejomqv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gjlperkjn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/grqkawora.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/giitgctii.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/ggmzpaxro.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/giphqjwvu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gxbkyyzoj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gygymmfgu.sHtML

[E07] 按分隔符拆分
来源：http://blog.tarul.cn/Article/details/gkfhkuxll.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.yfazqb.com/Article/details/gmfnzosxb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gjsnfjgpe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.sjlbkw.cn/Article/details/glddlurjd.sHtML

TS:   s.split(",")
来源：http://3g.sjlbkw.cn/Article/details/ggfkdppzn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.vehdjk.com/Article/details/gyfjgoxgq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.vehdjk.com/Article/details/ggtlpcxzm.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.vehdjk.com/Article/details/gngjpopgy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.epnwcf.com/Article/details/galmgcuje.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.sjlbkw.cn/Article/details/gbnhwfjes.sHtML

Py:   ",".join(items)
来源：http://3g.bbcook.cn/Article/details/glvetdemy.sHtML

PHP:  implode(",", $items);
来源：http://baike.yfazqb.com/Article/details/gfqjpbltc.sHtML

JS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gykgfeuvj.sHtML

TS:   items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gzshmsneg.sHtML

Java: String.join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/gitepeidl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.bbcook.cn/Article/details/geswwozut.sHtML

Ruby: items.join(",")
来源：http://3g.tarul.cn/Article/details/gjtvfhjfo.sHtML

C#:   string.Join(",", items)
来源：http://www.share.bbcook.cn/Article/details/gxheqthlk.sHtML

[E09] 去除所有空白字符
来源：http://3g.sjlbkw.cn/Article/details/gxaizlrkj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.vehdjk.com/Article/details/gjpuyixvr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.bbcook.cn/Article/details/gqxnqnhnl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/gsfuiwilm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/gnubgvpus.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.vehdjk.com/Article/details/gixmktyrl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.yfazqb.com/Article/details/gavrownkn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.yfazqb.com/Article/details/ghnsjwzqz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/gubahfudl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.yfazqb.com/Article/details/gwoxiswht.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gqrkvoauv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.epnwcf.com/Article/details/glkvzayqc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gjbkcvnki.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gjjhskzca.sHtML

Java: String.format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/ghnncyzvv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gvdkqbags.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gxftzrbyl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.epnwcf.com/Article/details/gytezsolu.sHtML

[E11] 反转字符串
来源：http://3g.bbcook.cn/Article/details/goqurnxuz.sHtML

Py:   s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/giyiphiyn.sHtML

PHP:  strrev($s);
来源：http://baike.tarul.cn/Article/details/glfjvwipf.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/grzqxkldw.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/ggndtlplx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.sjlbkw.cn/Article/details/gastezfwq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.tarul.cn/Article/details/ghplwihyy.sHtML

Ruby: s.reverse
来源：http://wap.yfazqb.com/Article/details/glmlawbgi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.epnwcf.com/Article/details/guvxemads.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.vehdjk.com/Article/details/gtkmrviva.sHtML

Py:   s.count("a")
来源：http://read.share.vehdjk.com/Article/details/garsulsuv.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fktsv.cn/Article/details/glkzqxpgu.sHtML

JS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/gdtlzcwgp.sHtML

TS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gbirppxaf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.vehdjk.com/Article/details/gkyavxgzx.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.tarul.cn/Article/details/grdgeyrte.sHtML

Ruby: s.count("a")
来源：http://m.share.bbcook.cn/Article/details/goplyeght.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.sjlbkw.cn/Article/details/gkckntwwy.sHtML

[E13] 逐字符遍历
来源：http://www.blog.vehdjk.com/Article/details/gmkqiwtou.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.bbcook.cn/Article/details/gtseakgit.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.yfazqb.com/Article/details/gaovwqoss.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/goxmpzixr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.tarul.cn/Article/details/gtdwlawtm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/ghatuuarn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.epnwcf.com/Article/details/ggygqomks.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.epnwcf.com/Article/details/gpjzelpeb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fktsv.cn/Article/details/guyiqqqzd.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.tarul.cn/Article/details/girixwywo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.tarul.cn/Article/details/gxwvthmuy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.bbcook.cn/Article/details/glnazdwti.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.vehdjk.com/Article/details/gggajwgbh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.vehdjk.com/Article/details/gjgmgqdet.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fktsv.cn/Article/details/gradvxxuq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/gonjmgwck.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.epnwcf.com/Article/details/gizbnozxz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.epnwcf.com/Article/details/gcfqertnz.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.vehdjk.com/Article/details/gugbrxvws.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.bbcook.cn/Article/details/gmusxqges.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.tarul.cn/Article/details/gqbjiszyr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.sjlbkw.cn/Article/details/gyckvesgu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gkxbkrdvf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.epnwcf.com/Article/details/gajmrbdvi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.tarul.cn/Article/details/gxivdnmrm.sHtML


<!-- 参考信息 -->