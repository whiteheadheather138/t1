代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.tarul.cn/Article/details/ggnbwxiaa.sHtML

TS:   [...a, ...b];
来源：http://www.share.fktsv.cn/Article/details/gmlodwoup.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.vehdjk.com/Article/details/gpateojbb.sHtML

Go:   append(a, b...)
来源：http://blog.epnwcf.com/Article/details/gvcioiouo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.bbcook.cn/Article/details/ganateqmi.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.tarul.cn/Article/details/ggsmqlggc.sHtML

[D09] 排序（升序）
来源：http://mobile.vehdjk.com/Article/details/gtzmuhdhx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gpeafsxtg.sHtML

PHP:  sort($arr);
来源：http://blog.sjlbkw.cn/Article/details/gumhuzeju.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.epnwcf.com/Article/details/golnhvdhq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.bbcook.cn/Article/details/glewlulyc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbuogfxqv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/gyobjhnow.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/gocbhdvwz.sHtML

C#:   list.Sort();
来源：http://mobile.bbcook.cn/Article/details/gopzumefa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.epnwcf.com/Article/details/gtzpjrndy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.epnwcf.com/Article/details/glemvdbqr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.epnwcf.com/Article/details/gsohkvqhp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/ghozxsabj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fktsv.cn/Article/details/ghtqgxvty.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.epnwcf.com/Article/details/guluodckq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.tarul.cn/Article/details/gtpljxvua.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.vehdjk.com/Article/details/gdvfmujvh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.epnwcf.com/Article/details/gvfspkyiz.sHtML

[D11] 反转数组
来源：http://m.share.vehdjk.com/Article/details/gsikcbaqu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.tarul.cn/Article/details/gneaiopgz.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fktsv.cn/Article/details/ghojvpmuu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.epnwcf.com/Article/details/glprnfjvj.sHtML

TS:   [...arr].reverse();
来源：http://www.share.yfazqb.com/Article/details/gepgtsgdl.sHtML

Java: Collections.reverse(list);
来源：http://baike.yfazqb.com/Article/details/gagpaztwe.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.tarul.cn/Article/details/grzqsunoi.sHtML

Ruby: arr.reverse
来源：http://blog.tarul.cn/Article/details/gbxpyelzu.sHtML

C#:   list.Reverse();
来源：http://3g.sjlbkw.cn/Article/details/gbzfwcbcx.sHtML

[D12] 查找元素下标
来源：http://m.share.fktsv.cn/Article/details/gekdhkjcc.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.tarul.cn/Article/details/gefrkocxr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.sjlbkw.cn/Article/details/gdcjcfqcl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/gaulbvnwq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gmnqupqjm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.vehdjk.com/Article/details/gqlkvjyve.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gvehcovca.sHtML

Ruby: arr.index(x)
来源：http://wap.tarul.cn/Article/details/gyaczmyte.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.bbcook.cn/Article/details/gjppidvuh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.vehdjk.com/Article/details/gauqsvtxs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.vehdjk.com/Article/details/gttszasie.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.tarul.cn/Article/details/gpnmixqmz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/gnbxrdszf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/gelpaizek.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.tarul.cn/Article/details/gztmqxpzb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.tarul.cn/Article/details/giyfebmwn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.epnwcf.com/Article/details/gwpvzeuza.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.yfazqb.com/Article/details/glqbmopqb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.yfazqb.com/Article/details/glqicaytm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.epnwcf.com/Article/details/gagwpavdr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.epnwcf.com/Article/details/gmavmaftn.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gznhimkxs.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.vehdjk.com/Article/details/gcegrdwpl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.epnwcf.com/Article/details/gyvzlfnlr.sHtML

Go:   // 手写循环
来源：http://www.m.share.vehdjk.com/Article/details/govpdojiy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gnewtnoot.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.yfazqb.com/Article/details/gvsvpjgzv.sHtML

[D15] 去重
来源：http://baike.epnwcf.com/Article/details/gdousmact.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/gushtitjq.sHtML

PHP:  array_unique($arr);
来源：http://3g.vehdjk.com/Article/details/gjiwkbqza.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/ghnisufso.sHtML

TS:   [...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gxijquiet.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.sjlbkw.cn/Article/details/gsxjyvquu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.sjlbkw.cn/Article/details/ghmcwulmc.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fktsv.cn/Article/details/ggeuoleff.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gvhupqhwv.sHtML

[D16] 求和与平均值
来源：http://blog.fktsv.cn/Article/details/gcpmkckbo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fktsv.cn/Article/details/gqapwhgwe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.tarul.cn/Article/details/gciugdper.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.yfazqb.com/Article/details/gmqseixjo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.bbcook.cn/Article/details/gebekrhvw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fktsv.cn/Article/details/gwltfimqp.sHtML

Go:   // 手写循环累加
来源：http://www.share.sjlbkw.cn/Article/details/ggykhijzq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fktsv.cn/Article/details/gzigbniyl.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.epnwcf.com/Article/details/gtjtcvhvj.sHtML

[D17] 最大值与最小值
来源：http://read.share.bbcook.cn/Article/details/gxhraantc.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fktsv.cn/Article/details/gbecnjabk.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.bbcook.cn/Article/details/ggquizshi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.yfazqb.com/Article/details/gqsawwxql.sHtML

TS:   Math.max(...arr);
来源：http://baike.tarul.cn/Article/details/gylyvoelu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.epnwcf.com/Article/details/gcispzlwk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.tarul.cn/Article/details/gqouppdoj.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.vehdjk.com/Article/details/glvjnvrdy.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.tarul.cn/Article/details/gczhvxuve.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.bbcook.cn/Article/details/gpczgwbhb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.vehdjk.com/Article/details/gfslyycbi.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.tarul.cn/Article/details/gssfcmyst.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.yfazqb.com/Article/details/gakszasph.sHtML

TS:   nested.flat();
来源：http://read.share.sjlbkw.cn/Article/details/gtbyuagbg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fktsv.cn/Article/details/ghoxqkedd.sHtML

Go:   // 手写双层循环
来源：http://m.share.yfazqb.com/Article/details/gaeqtaueu.sHtML

Ruby: nested.flatten
来源：http://wap.bbcook.cn/Article/details/gomhqeshx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.yfazqb.com/Article/details/gqhvnlmuz.sHtML

[D19] 按字段分组
来源：http://read.share.epnwcf.com/Article/details/gyqyrhusm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fktsv.cn/Article/details/gchibcpls.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhlitaxa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.sjlbkw.cn/Article/details/gupxivinj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/gusdkaajn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.sjlbkw.cn/Article/details/gveikqxky.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.yfazqb.com/Article/details/gxclblvkq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fktsv.cn/Article/details/gbzgvwpkw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fktsv.cn/Article/details/gqeneclkz.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.epnwcf.com/Article/details/gxamxfhsr.sHtML

Py:   Counter(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gqcpnulkw.sHtML

PHP:  array_count_values($arr);
来源：http://baike.vehdjk.com/Article/details/gxearlzxt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/giytpcvmj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.bbcook.cn/Article/details/gmjbkaskg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.bbcook.cn/Article/details/gsoejryxu.sHtML

Go:   // 手写 map[T]int
来源：http://wap.epnwcf.com/Article/details/giworjxti.sHtML

Ruby: arr.tally
来源：http://www.m.share.vehdjk.com/Article/details/gcyoqkmti.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.bbcook.cn/Article/details/gevaaekhg.sHtML

[D21] 判断是否包含某元素
来源：http://wap.tarul.cn/Article/details/grvxbpptx.sHtML

Py:   x in arr
来源：http://wap.fktsv.cn/Article/details/gnrkpnsgf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fktsv.cn/Article/details/gragqroqf.sHtML

JS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/gqvrrqqjv.sHtML

TS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/gkhkxqswr.sHtML

Java: list.contains(x)
来源：http://read.share.tarul.cn/Article/details/gqmsmovxx.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gjaqzayrn.sHtML

Ruby: arr.include?(x)
来源：http://wap.yfazqb.com/Article/details/gnyxjiakb.sHtML

C#:   list.Contains(x)
来源：http://wap.vehdjk.com/Article/details/grhwoolgj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.yfazqb.com/Article/details/ggkmtqmzz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.yfazqb.com/Article/details/gshkyphev.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.vehdjk.com/Article/details/gltztogwb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.sjlbkw.cn/Article/details/gbblmjuyw.sHtML

TS:   [...arr];
来源：http://read.share.tarul.cn/Article/details/gnspsxmwz.sHtML

Java: new ArrayList<>(list);
来源：http://baike.yfazqb.com/Article/details/gzdgegsyf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.yfazqb.com/Article/details/guaqrwjgx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.bbcook.cn/Article/details/gfohwwdqn.sHtML

C#:   new List<int>(list);
来源：http://mobile.vehdjk.com/Article/details/gvmnhiimu.sHtML

[D23] reduce 累积计算
来源：http://3g.epnwcf.com/Article/details/gitfculdq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fktsv.cn/Article/details/glzmpcokj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.epnwcf.com/Article/details/gvthgfdfb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/gjgatwxpo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/gnjglkgxm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fktsv.cn/Article/details/gsncqmani.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gbevqjdvw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.bbcook.cn/Article/details/gezfqnxkg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.yfazqb.com/Article/details/gppacobaq.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fktsv.cn/Article/details/gfwjqucnd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fktsv.cn/Article/details/gpnmnkqcg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.sjlbkw.cn/Article/details/gerjpbkor.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/ggbxiehcs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.bbcook.cn/Article/details/gmerunhwn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.bbcook.cn/Article/details/gcwiitcze.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fktsv.cn/Article/details/gbariqflm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.tarul.cn/Article/details/gffbwqzfa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.tarul.cn/Article/details/goziebums.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.yfazqb.com/Article/details/gohwbhswh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.epnwcf.com/Article/details/gxfrxjdxz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.epnwcf.com/Article/details/gnacrlbxy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.epnwcf.com/Article/details/ggyaxnnki.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.bbcook.cn/Article/details/gluhbewpo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.sjlbkw.cn/Article/details/gnhudusaw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.tarul.cn/Article/details/gygimpwbb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.bbcook.cn/Article/details/ghtnxwprc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.tarul.cn/Article/details/gghzefcbb.sHtML

[D26] 数组转字符串
来源：http://m.share.fktsv.cn/Article/details/gtuabskzn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/ggkfxkjgd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.epnwcf.com/Article/details/gxdhaqhsg.sHtML

JS:   arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gmqhnpccm.sHtML

TS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gzlisaxvy.sHtML

Java: String.join(", ", list)
来源：http://wap.bbcook.cn/Article/details/gvuyjekmp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.tarul.cn/Article/details/gpjqgshhw.sHtML

Ruby: arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/gafaofyzy.sHtML

C#:   string.Join(", ", list)
来源：http://blog.sjlbkw.cn/Article/details/ggchqzaoe.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gttgqgwnl.sHtML

E. 字符串处理
来源：http://www.m.share.vehdjk.com/Article/details/gxqjakudn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ggyygiqgq.sHtML

[E01] 拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gatgrsrdt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.tarul.cn/Article/details/ggizehtmk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.vehdjk.com/Article/details/gszxfzwiy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gpctptfvg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gxjhvffxs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.tarul.cn/Article/details/gtklasnvv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.tarul.cn/Article/details/grvbpgvui.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.epnwcf.com/Article/details/gyvsrfrxy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.epnwcf.com/Article/details/ggpcdpdbm.sHtML

[E02] 重复字符串
来源：http://www.m.share.fktsv.cn/Article/details/gafnayqtq.sHtML

Py:   "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/ggnwdyprq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.epnwcf.com/Article/details/gxrfnknfq.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/gmdnsttzy.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gxeshxvpm.sHtML

Java: "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gykkudzrw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.sjlbkw.cn/Article/details/ghzgakqtj.sHtML

Ruby: "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gxhtbxoqj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.vehdjk.com/Article/details/gwkifflma.sHtML

[E03] 截取子串
来源：http://3g.sjlbkw.cn/Article/details/gxigutqzl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.sjlbkw.cn/Article/details/gtjqfkjyx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gszhmugsf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gimipgzks.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gwrnsbjcl.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gkmikhmsa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.sjlbkw.cn/Article/details/gfjlgpcmo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fktsv.cn/Article/details/gmxpwpmot.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fktsv.cn/Article/details/glsgunhqt.sHtML

[E04] 查找子串位置
来源：http://read.share.fktsv.cn/Article/details/gzxjjbdlh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.bbcook.cn/Article/details/gxuhvwxam.sHtML

PHP:  strpos($s, "x");
来源：http://wap.vehdjk.com/Article/details/gjzbyrjkt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fktsv.cn/Article/details/gwmjrkjzy.sHtML

TS:   s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gwhqzzxwr.sHtML

Java: s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gitelxdml.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.bbcook.cn/Article/details/golotvbhd.sHtML

Ruby: s.index("x")
来源：http://baike.tarul.cn/Article/details/gcdxosabi.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gelqgqcuf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fktsv.cn/Article/details/gfojgwruk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fktsv.cn/Article/details/gnttcmfcz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fktsv.cn/Article/details/gfriuklbf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.vehdjk.com/Article/details/gwvdezngy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.bbcook.cn/Article/details/grtbdrgci.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.yfazqb.com/Article/details/gejonwllf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.sjlbkw.cn/Article/details/gvqnkykpp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.tarul.cn/Article/details/gpwavwgzz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/goayuynkj.sHtML

[E06] 替换子串
来源：http://www.m.share.yfazqb.com/Article/details/gkvilffmo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gdagkpzwe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.yfazqb.com/Article/details/gortxirhk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gtdfzcmko.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gyrfqkvck.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gdvxcryrz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.yfazqb.com/Article/details/gernveopx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gllevyygd.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gqrsszdqs.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fktsv.cn/Article/details/gygetdqwm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.tarul.cn/Article/details/gpizdyyqo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gavlrbwfj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.sjlbkw.cn/Article/details/gdqzolysm.sHtML

TS:   s.split(",")
来源：http://wap.yfazqb.com/Article/details/gaofnrvcd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.epnwcf.com/Article/details/glxspmvvs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.yfazqb.com/Article/details/gpmmsqjmz.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.yfazqb.com/Article/details/gmzbhdhci.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.vehdjk.com/Article/details/gyfoxqhdf.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.sjlbkw.cn/Article/details/govxzqwms.sHtML

Py:   ",".join(items)
来源：http://www.blog.epnwcf.com/Article/details/gmvfkncke.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fktsv.cn/Article/details/gjivpbirp.sHtML

JS:   items.join(",")
来源：http://3g.vehdjk.com/Article/details/gdklupfjx.sHtML

TS:   items.join(",")
来源：http://wap.fktsv.cn/Article/details/gtyygifbq.sHtML

Java: String.join(",", items)
来源：http://mobile.tarul.cn/Article/details/gmnryltpa.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.tarul.cn/Article/details/gnwtvzenj.sHtML

Ruby: items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gpgjkwkgh.sHtML

C#:   string.Join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gypqwbwsr.sHtML

[E09] 去除所有空白字符
来源：http://www.share.tarul.cn/Article/details/gxgduqypz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fktsv.cn/Article/details/gsvlocmnk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.epnwcf.com/Article/details/gixgdxecy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/gpuzdszfc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/gjsqfceac.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.tarul.cn/Article/details/geznneleo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.bbcook.cn/Article/details/ghjzhxtyh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fktsv.cn/Article/details/glcxpfoac.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gfasfqcar.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.tarul.cn/Article/details/gudvrtuho.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gdyqgfdly.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fktsv.cn/Article/details/gkenwxtvs.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gbwhpcslh.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gpffqxjex.sHtML

Java: String.format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gydtsysmt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gnpbpuvkw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gbntduupm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.yfazqb.com/Article/details/gjlomkkam.sHtML

[E11] 反转字符串
来源：http://wap.tarul.cn/Article/details/gksppncqy.sHtML

Py:   s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gsdytseix.sHtML

PHP:  strrev($s);
来源：http://mobile.tarul.cn/Article/details/gvbqkxcgv.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gyjhkebge.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gegfclext.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fktsv.cn/Article/details/gknthqanq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.yfazqb.com/Article/details/gaqfcutix.sHtML

Ruby: s.reverse
来源：http://m.share.tarul.cn/Article/details/gsirtodgi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/gajncaeny.sHtML

[E12] 统计某字符出现次数
来源：http://3g.vehdjk.com/Article/details/gteolubta.sHtML

Py:   s.count("a")
来源：http://baike.bbcook.cn/Article/details/greyugryo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfanreydd.sHtML

JS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/ghnrazcyt.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.epnwcf.com/Article/details/gmavpbcdh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fktsv.cn/Article/details/ggxsguldz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.vehdjk.com/Article/details/gvhovzwcp.sHtML

Ruby: s.count("a")
来源：http://3g.vehdjk.com/Article/details/gchnfrugh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.vehdjk.com/Article/details/gglmsgwnj.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/gfqgfcblr.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.bbcook.cn/Article/details/gldxpmxxg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.epnwcf.com/Article/details/gjsvfpcvz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/guirakrsw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gkniyxxie.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.tarul.cn/Article/details/gytyxkkwk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.vehdjk.com/Article/details/grnbjgjrk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.vehdjk.com/Article/details/grqdrokdb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.tarul.cn/Article/details/gsqrwwekj.sHtML

[E14] URL 编码与 Base64
来源：http://3g.yfazqb.com/Article/details/gmckcdvrj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.sjlbkw.cn/Article/details/grjlcccqv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.bbcook.cn/Article/details/gdgtawcnc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.yfazqb.com/Article/details/gbpcvxllj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.yfazqb.com/Article/details/gdxewgrbq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.bbcook.cn/Article/details/gcwfqkloo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.tarul.cn/Article/details/gljblwpst.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.epnwcf.com/Article/details/gckcejzhl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.tarul.cn/Article/details/gljvzxyqt.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.epnwcf.com/Article/details/gcwbxrbyg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.epnwcf.com/Article/details/gtdtwpgiv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.sjlbkw.cn/Article/details/gyjjazlrz.sHtML


<!-- 参考信息 -->