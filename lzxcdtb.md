代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.sjlbkw.cn/Article/details/gjwgszied.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.yfazqb.com/Article/details/gjmhsxvlb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.sjlbkw.cn/Article/details/gmzepqkiq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.bbcook.cn/Article/details/gmzagbtah.sHtML

[D11] 反转数组
来源：http://www.share.fktsv.cn/Article/details/goysldxwb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.vehdjk.com/Article/details/guppakkqr.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.bbcook.cn/Article/details/gebylejwi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.bbcook.cn/Article/details/goypzkklw.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/gftbhzlkm.sHtML

Java: Collections.reverse(list);
来源：http://www.share.sjlbkw.cn/Article/details/gnwomoxtr.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.tarul.cn/Article/details/gaffiyekh.sHtML

Ruby: arr.reverse
来源：http://3g.tarul.cn/Article/details/gpoykzfeo.sHtML

C#:   list.Reverse();
来源：http://www.m.share.bbcook.cn/Article/details/gorgnmwdz.sHtML

[D12] 查找元素下标
来源：http://m.share.vehdjk.com/Article/details/gelduqsbi.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.epnwcf.com/Article/details/gypkugxiy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.tarul.cn/Article/details/gidvuzslk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gftkemvnx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/gzzaeizly.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.tarul.cn/Article/details/gwkomlqhh.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gzglsyrio.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.tarul.cn/Article/details/gffgqbnlc.sHtML

C#:   list.IndexOf(x);
来源：http://3g.sjlbkw.cn/Article/details/glfdhkadk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.epnwcf.com/Article/details/gcjpajpyq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.sjlbkw.cn/Article/details/grviwdrgn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fktsv.cn/Article/details/gwtyrewuq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/gavibitbg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/graxplvub.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fktsv.cn/Article/details/ganjvfcut.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.epnwcf.com/Article/details/gxbhfqizm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.tarul.cn/Article/details/gcwljczbt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.yfazqb.com/Article/details/gfynflstr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.epnwcf.com/Article/details/giyoqzxwb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.tarul.cn/Article/details/gzblopkea.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.vehdjk.com/Article/details/ghcnfguma.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/glgumushq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gpzxwlukn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gfclqbjfe.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gvdqkcgaa.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.tarul.cn/Article/details/grjwnlsup.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.yfazqb.com/Article/details/grczukrug.sHtML

[D15] 去重
来源：http://blog.yfazqb.com/Article/details/ghmwrjgau.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gvjnprjvg.sHtML

PHP:  array_unique($arr);
来源：http://www.share.tarul.cn/Article/details/gdczwwlsa.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/gwnwuqrsm.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/guhswkrgp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.yfazqb.com/Article/details/gzgdjytyj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.sjlbkw.cn/Article/details/gtqbtpdho.sHtML

Ruby: arr.uniq
来源：http://read.share.bbcook.cn/Article/details/gbrvwgyre.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fktsv.cn/Article/details/gtappeagw.sHtML

[D16] 求和与平均值
来源：http://read.share.epnwcf.com/Article/details/giiivkxil.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.yfazqb.com/Article/details/gkwylccpq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.vehdjk.com/Article/details/gnqylsdqc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.bbcook.cn/Article/details/gsdtyfgap.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.sjlbkw.cn/Article/details/gsksgxwnt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.tarul.cn/Article/details/gkxuvmoie.sHtML

Go:   // 手写循环累加
来源：http://www.blog.vehdjk.com/Article/details/gngpgxeva.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.tarul.cn/Article/details/giamzpbqf.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.epnwcf.com/Article/details/gfnegidzc.sHtML

[D17] 最大值与最小值
来源：http://mobile.yfazqb.com/Article/details/gbytydnih.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.sjlbkw.cn/Article/details/ggcwnmsji.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.tarul.cn/Article/details/gvsxxoxcd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.yfazqb.com/Article/details/gvapnfbwf.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.tarul.cn/Article/details/gphtoiawz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.epnwcf.com/Article/details/gjwszakca.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gcnqxxstv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.epnwcf.com/Article/details/gfvxezfkr.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.yfazqb.com/Article/details/gwyoocime.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.epnwcf.com/Article/details/gsmcmbgsf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.tarul.cn/Article/details/gerckbbyn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fktsv.cn/Article/details/gtyxbmrlv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.yfazqb.com/Article/details/gvybpywvz.sHtML

TS:   nested.flat();
来源：http://3g.epnwcf.com/Article/details/gwulblknx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.tarul.cn/Article/details/ggpzkvnlq.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fktsv.cn/Article/details/gadgdwyxx.sHtML

Ruby: nested.flatten
来源：http://www.blog.vehdjk.com/Article/details/geiltkqdv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.tarul.cn/Article/details/ggllgzawq.sHtML

[D19] 按字段分组
来源：http://mobile.yfazqb.com/Article/details/glgylajif.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.bbcook.cn/Article/details/gfezjyozu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.tarul.cn/Article/details/gvxyoixso.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.sjlbkw.cn/Article/details/ggbgsouzv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.yfazqb.com/Article/details/gleqjibsb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.epnwcf.com/Article/details/guspseiuw.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.vehdjk.com/Article/details/giiepvxyx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.tarul.cn/Article/details/gfzpebdgy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fktsv.cn/Article/details/gkwhhfisr.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.bbcook.cn/Article/details/glgtstwta.sHtML

Py:   Counter(arr)
来源：http://3g.bbcook.cn/Article/details/gjpabnzvc.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.yfazqb.com/Article/details/getxkzcyh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtxmanhc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gmyftflpf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.sjlbkw.cn/Article/details/gfgeghcgc.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.vehdjk.com/Article/details/guhoyukkr.sHtML

Ruby: arr.tally
来源：http://m.share.sjlbkw.cn/Article/details/geacikvsb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.bbcook.cn/Article/details/gqxqrysii.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.bbcook.cn/Article/details/gkxwujyml.sHtML

Py:   x in arr
来源：http://www.blog.vehdjk.com/Article/details/gyugdyqnh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.bbcook.cn/Article/details/gjtbblbfz.sHtML

JS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gctvndgqu.sHtML

TS:   arr.includes(x)
来源：http://www.share.yfazqb.com/Article/details/gbskchjce.sHtML

Java: list.contains(x)
来源：http://read.share.yfazqb.com/Article/details/gvzjfadic.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fktsv.cn/Article/details/gvdkpeakx.sHtML

Ruby: arr.include?(x)
来源：http://read.share.yfazqb.com/Article/details/gmteashzm.sHtML

C#:   list.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gjppivbio.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.bbcook.cn/Article/details/gljjftruv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.sjlbkw.cn/Article/details/geosawaax.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.bbcook.cn/Article/details/gcxuvodnb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fktsv.cn/Article/details/guzavkhkc.sHtML

TS:   [...arr];
来源：http://www.blog.bbcook.cn/Article/details/guqkwnehp.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.epnwcf.com/Article/details/gkjxrdbey.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.epnwcf.com/Article/details/gvfttphsd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.sjlbkw.cn/Article/details/gzmztgawu.sHtML

C#:   new List<int>(list);
来源：http://www.share.epnwcf.com/Article/details/gdddrvizx.sHtML

[D23] reduce 累积计算
来源：http://wap.vehdjk.com/Article/details/gaqthkutv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.bbcook.cn/Article/details/gukyuncgb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.epnwcf.com/Article/details/gtmpcqlqo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/gkwixhgge.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/gejniufou.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.vehdjk.com/Article/details/geyyfaqlc.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gpmzzmubg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.sjlbkw.cn/Article/details/ghtzjsyyc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.yfazqb.com/Article/details/gcayjtuxv.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.vehdjk.com/Article/details/ggmqehmmz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.epnwcf.com/Article/details/gksuzrmba.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwslvjpgc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gnczimknw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.bbcook.cn/Article/details/gqnjiuste.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.tarul.cn/Article/details/gjiyhoule.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.bbcook.cn/Article/details/ggxhdhzwi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.vehdjk.com/Article/details/gjuytsjhm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.yfazqb.com/Article/details/gfphbeaad.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.vehdjk.com/Article/details/gcbdxtmip.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.yfazqb.com/Article/details/gdqzxammw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.vehdjk.com/Article/details/gvvxloklx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.bbcook.cn/Article/details/ggvefkdvb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.yfazqb.com/Article/details/gtqbuisrk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.epnwcf.com/Article/details/gusykotps.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.tarul.cn/Article/details/gjzoishrl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.yfazqb.com/Article/details/gqgpkwydg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.vehdjk.com/Article/details/grwdqsjfb.sHtML

[D26] 数组转字符串
来源：http://www.blog.vehdjk.com/Article/details/gkcxzmbyy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.sjlbkw.cn/Article/details/gdpknijzl.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.bbcook.cn/Article/details/gkpcnfzfs.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gmlgwjipt.sHtML

TS:   arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gvasbdnch.sHtML

Java: String.join(", ", list)
来源：http://3g.tarul.cn/Article/details/guerkrmjd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.tarul.cn/Article/details/gdpnftmxg.sHtML

Ruby: arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/giwtexllf.sHtML

C#:   string.Join(", ", list)
来源：http://blog.tarul.cn/Article/details/gzzlmwjrh.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ghauamvhe.sHtML

E. 字符串处理
来源：http://www.m.share.tarul.cn/Article/details/gdbhvgioy.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfepbudf.sHtML

[E01] 拼接字符串
来源：http://3g.epnwcf.com/Article/details/gebrcovjc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.bbcook.cn/Article/details/gpqhqylcv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fktsv.cn/Article/details/gafsfcbxv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.sjlbkw.cn/Article/details/gigswvqbk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.sjlbkw.cn/Article/details/gmsvnbvpq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.sjlbkw.cn/Article/details/gvbrnksch.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.vehdjk.com/Article/details/gcszdtlhm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fktsv.cn/Article/details/ggnlubxte.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.tarul.cn/Article/details/ghhaeuxae.sHtML

[E02] 重复字符串
来源：http://m.share.epnwcf.com/Article/details/gnozbngyy.sHtML

Py:   "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/gflhqdmhp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.yfazqb.com/Article/details/gxqualnha.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gdnsyxhva.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gmtjnjiaa.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gziqdaayd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.bbcook.cn/Article/details/gkgcsfqgs.sHtML

Ruby: "ab" * 3
来源：http://m.share.tarul.cn/Article/details/gddeshtlg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.epnwcf.com/Article/details/gsubcvjao.sHtML

[E03] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/goqtsaozb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fktsv.cn/Article/details/gvklkhpuy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gmssrgeea.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.tarul.cn/Article/details/gvbfirfvu.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gkdopbvpj.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gkevxyxpo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.yfazqb.com/Article/details/ghtqlpnbx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.vehdjk.com/Article/details/gmsktwgff.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.vehdjk.com/Article/details/gifcrtcyl.sHtML

[E04] 查找子串位置
来源：http://baike.yfazqb.com/Article/details/gvysenzsx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/glcahzzgl.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.bbcook.cn/Article/details/gaskiigig.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.tarul.cn/Article/details/gbnvudhuv.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gofcggwyt.sHtML

Java: s.indexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gkxhequlm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.yfazqb.com/Article/details/gdvlrakol.sHtML

Ruby: s.index("x")
来源：http://mobile.fktsv.cn/Article/details/grrvvclga.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gmmnsquuz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.vehdjk.com/Article/details/gpflmipkg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fktsv.cn/Article/details/guanojyhi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.bbcook.cn/Article/details/ghumvlhpg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/glnfhlglh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.vehdjk.com/Article/details/gmsiyylys.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.epnwcf.com/Article/details/gxgffcnxm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.vehdjk.com/Article/details/gzzskyadd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.sjlbkw.cn/Article/details/ghgzlfmtr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fktsv.cn/Article/details/gzkeibbjb.sHtML

[E06] 替换子串
来源：http://blog.vehdjk.com/Article/details/gdnjgdvdz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.vehdjk.com/Article/details/ggkyfqzhh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.sjlbkw.cn/Article/details/grivnlzet.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/ggyoxmolh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gktpqdppn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gacfpyggd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/galupwqgw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.tarul.cn/Article/details/gguchlgxb.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.tarul.cn/Article/details/gczrgzkqw.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fktsv.cn/Article/details/gnairolxu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fktsv.cn/Article/details/gxkzftwfz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.bbcook.cn/Article/details/gemyuoblk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.vehdjk.com/Article/details/gcgtfbgar.sHtML

TS:   s.split(",")
来源：http://baike.sjlbkw.cn/Article/details/gawcpdoby.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.bbcook.cn/Article/details/gmptgfsxd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.epnwcf.com/Article/details/gtytlxtlf.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fktsv.cn/Article/details/gzxuqwkuf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fktsv.cn/Article/details/geotavfiq.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.epnwcf.com/Article/details/ghkgbhpxq.sHtML

Py:   ",".join(items)
来源：http://www.blog.epnwcf.com/Article/details/gjyckyses.sHtML

PHP:  implode(",", $items);
来源：http://3g.epnwcf.com/Article/details/gyiqertek.sHtML

JS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/ghubgvbew.sHtML

TS:   items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gfeckjvja.sHtML

Java: String.join(",", items)
来源：http://mobile.tarul.cn/Article/details/ggulxqyus.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.sjlbkw.cn/Article/details/gvzghkcpd.sHtML

Ruby: items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gbqfzlpnx.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/gnnnkplzb.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhuijtov.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.vehdjk.com/Article/details/ghkfpgcpy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fktsv.cn/Article/details/gskxfkvza.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/gnpcwcyxh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/giezwhicw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.tarul.cn/Article/details/gjjwtebiz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.vehdjk.com/Article/details/gzzvpwxkd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.yfazqb.com/Article/details/gqxcymzgg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gjfqnybxl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfbeeuyf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gjtalkuxg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.tarul.cn/Article/details/gpxwzvimc.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gehsmkqrf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gamxlgimm.sHtML

Java: String.format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gbekrbzyn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gyoirazqi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gvnivjqpv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.sjlbkw.cn/Article/details/gqlkwsdpu.sHtML

[E11] 反转字符串
来源：http://www.blog.fktsv.cn/Article/details/ghbsubkhu.sHtML

Py:   s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/gsjtnavrl.sHtML

PHP:  strrev($s);
来源：http://www.blog.epnwcf.com/Article/details/gcesyahly.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gpqzshoer.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gklqhlrbx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fktsv.cn/Article/details/gkcvbxlrj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fktsv.cn/Article/details/gjuswkvra.sHtML

Ruby: s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gociwpohz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/gyttmtbnu.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.tarul.cn/Article/details/glnzmeiab.sHtML

Py:   s.count("a")
来源：http://baike.yfazqb.com/Article/details/goazgjnky.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.vehdjk.com/Article/details/ggwmcrimp.sHtML

JS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gxfpdtoli.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/gmlmdpjhq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.yfazqb.com/Article/details/giidnxpxz.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.vehdjk.com/Article/details/gpuhyiakt.sHtML

Ruby: s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gwiktbtdp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.epnwcf.com/Article/details/gaqvhwuxj.sHtML

[E13] 逐字符遍历
来源：http://blog.sjlbkw.cn/Article/details/goyblyfea.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.yfazqb.com/Article/details/gpmgiqbev.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.bbcook.cn/Article/details/ghzdwaoso.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gpcdadtwi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gzgzjisnm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fktsv.cn/Article/details/gmpytthse.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.tarul.cn/Article/details/gcaxvcwtq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.yfazqb.com/Article/details/gbzlkeaji.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gzskawsdu.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.bbcook.cn/Article/details/gvlwtqqvu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.vehdjk.com/Article/details/gmkxepzue.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fktsv.cn/Article/details/gobyuwvuf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fktsv.cn/Article/details/gtbftxvok.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.tarul.cn/Article/details/gcfdcryhf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/geitxtxao.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.yfazqb.com/Article/details/gnznbypag.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.epnwcf.com/Article/details/gupbbhcln.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.epnwcf.com/Article/details/golqafrkb.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.epnwcf.com/Article/details/gljbqekke.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.epnwcf.com/Article/details/gsnjuxawx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fktsv.cn/Article/details/gvxyxswtk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.yfazqb.com/Article/details/gfianbejr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.bbcook.cn/Article/details/gpawktmzy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.vehdjk.com/Article/details/gsuvgwlqm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.yfazqb.com/Article/details/gedppufic.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.sjlbkw.cn/Article/details/gkvvfmkty.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.vehdjk.com/Article/details/gnruuhrbh.sHtML

[E16] 数字千分位
来源：http://3g.fktsv.cn/Article/details/gxxnzmghm.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.tarul.cn/Article/details/gztpnhmqr.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/ggmwwnkle.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/gdrbbopdy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.bbcook.cn/Article/details/gwparoidk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gomrkoevm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.vehdjk.com/Article/details/gwjdjkeii.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.vehdjk.com/Article/details/gbvzvtofa.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvshcbof.sHtML

[E17] 首字母大写
来源：http://www.m.share.vehdjk.com/Article/details/gmehfetbj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.epnwcf.com/Article/details/gmohxxxcl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.tarul.cn/Article/details/gkeosfrbi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gukekaoal.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/gnyiupvlu.sHtML


<!-- 参考信息 -->