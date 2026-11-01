代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.sjlbkw.cn/Article/details/ghkfkfgyh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.bbcook.cn/Article/details/gwrkbawnf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.bbcook.cn/Article/details/gsvcrkvgi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/gvmxsyqah.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.yfazqb.com/Article/details/gvomvejnp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.epnwcf.com/Article/details/gvpxmfxqi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.epnwcf.com/Article/details/gcimwzbbs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fktsv.cn/Article/details/gaqmvydsf.sHtML

[D11] 反转数组
来源：http://m.share.fktsv.cn/Article/details/gxifliyfc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.vehdjk.com/Article/details/gffflaxkx.sHtML

PHP:  array_reverse($arr);
来源：http://blog.tarul.cn/Article/details/ginkttlyo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.bbcook.cn/Article/details/gpftraldx.sHtML

TS:   [...arr].reverse();
来源：http://wap.yfazqb.com/Article/details/gcpkvasdh.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.tarul.cn/Article/details/gjlowuwap.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.vehdjk.com/Article/details/gqxqnzntc.sHtML

Ruby: arr.reverse
来源：http://read.share.sjlbkw.cn/Article/details/gqaqorkgq.sHtML

C#:   list.Reverse();
来源：http://baike.epnwcf.com/Article/details/ghdtddsuh.sHtML

[D12] 查找元素下标
来源：http://m.share.fktsv.cn/Article/details/gzjhqdcrr.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.epnwcf.com/Article/details/gjtushvil.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gqoujyyim.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/gnczucayn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gzaoyfjqc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fktsv.cn/Article/details/gwybzvbal.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.epnwcf.com/Article/details/ganfocrgt.sHtML

Ruby: arr.index(x)
来源：http://blog.tarul.cn/Article/details/gfwvdvnkm.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.epnwcf.com/Article/details/gkmdcdluc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.vehdjk.com/Article/details/gxihayocm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.bbcook.cn/Article/details/gtbyysbnf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.sjlbkw.cn/Article/details/gvnmusfhe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/goxbbcqmt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/gchnvskvp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/grnlhkuzf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.tarul.cn/Article/details/gupdwnyvq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.vehdjk.com/Article/details/gsbsydrjr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gtiucbwau.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fktsv.cn/Article/details/goxonaslo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.vehdjk.com/Article/details/grpplnhcs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.vehdjk.com/Article/details/gtwchtlai.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.vehdjk.com/Article/details/gxayoldvr.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gwvxymtxi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.epnwcf.com/Article/details/gishhuxbr.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gfanmpygg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.yfazqb.com/Article/details/gnutedcpz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.epnwcf.com/Article/details/goyofrvgs.sHtML

[D15] 去重
来源：http://www.blog.vehdjk.com/Article/details/gvewzrvgj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gpptlzkmt.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.vehdjk.com/Article/details/goesfwfwm.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/giyfejvmv.sHtML

TS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/glbdixhyt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.bbcook.cn/Article/details/gxpnsdlez.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.bbcook.cn/Article/details/ggnglkfjx.sHtML

Ruby: arr.uniq
来源：http://baike.epnwcf.com/Article/details/gpfucmvvl.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.epnwcf.com/Article/details/gcjuzvcie.sHtML

[D16] 求和与平均值
来源：http://baike.bbcook.cn/Article/details/gjdmstljs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.bbcook.cn/Article/details/gjzwyomsv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.vehdjk.com/Article/details/goisqjoeu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/gmflvxdna.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.bbcook.cn/Article/details/gzvzwvtiv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.vehdjk.com/Article/details/gybsrklie.sHtML

Go:   // 手写循环累加
来源：http://read.share.vehdjk.com/Article/details/gqjxocfxy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.vehdjk.com/Article/details/gxqzxocil.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.vehdjk.com/Article/details/giigucxiu.sHtML

[D17] 最大值与最小值
来源：http://baike.sjlbkw.cn/Article/details/gijlnshin.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gmezjpnrs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.tarul.cn/Article/details/gyielluga.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.yfazqb.com/Article/details/gyrgbfjkt.sHtML

TS:   Math.max(...arr);
来源：http://3g.sjlbkw.cn/Article/details/gjymzlfgy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.sjlbkw.cn/Article/details/gsyafcjbd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.vehdjk.com/Article/details/gbpymusto.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.epnwcf.com/Article/details/ggnmqrtyk.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.vehdjk.com/Article/details/glkljyloa.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.bbcook.cn/Article/details/glscgcpyo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.epnwcf.com/Article/details/gwcfxnleb.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.yfazqb.com/Article/details/gwdosnqwj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fktsv.cn/Article/details/gcugibspy.sHtML

TS:   nested.flat();
来源：http://baike.bbcook.cn/Article/details/gyxpjiast.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gvrpwdwzj.sHtML

Go:   // 手写双层循环
来源：http://mobile.sjlbkw.cn/Article/details/gjtleqdeu.sHtML

Ruby: nested.flatten
来源：http://www.blog.bbcook.cn/Article/details/gqixzbjvu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fktsv.cn/Article/details/gpfsoytcs.sHtML

[D19] 按字段分组
来源：http://www.share.fktsv.cn/Article/details/gyfndkcsw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.sjlbkw.cn/Article/details/gjkzbgjbh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.bbcook.cn/Article/details/gzirvkvbd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.sjlbkw.cn/Article/details/gxommmplm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/gszyhdnzt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/gecheyzzh.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.vehdjk.com/Article/details/gjscldife.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.vehdjk.com/Article/details/gcforssgc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.sjlbkw.cn/Article/details/gevoubrjx.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.yfazqb.com/Article/details/gnghalbyd.sHtML

Py:   Counter(arr)
来源：http://baike.vehdjk.com/Article/details/guioyfpns.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gcdoyvfnt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/gssynanmj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gsuzjdfzg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.bbcook.cn/Article/details/getakfcls.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.epnwcf.com/Article/details/gdxxlznjj.sHtML

Ruby: arr.tally
来源：http://baike.tarul.cn/Article/details/gwrlndneo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.bbcook.cn/Article/details/gtmxllxak.sHtML

[D21] 判断是否包含某元素
来源：http://wap.bbcook.cn/Article/details/gcemnnluo.sHtML

Py:   x in arr
来源：http://www.blog.tarul.cn/Article/details/grhieelqj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/glhhpbnws.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gofmyudak.sHtML

TS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/geqpemisi.sHtML

Java: list.contains(x)
来源：http://m.share.yfazqb.com/Article/details/ghhjfvjpc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gfaxffocp.sHtML

Ruby: arr.include?(x)
来源：http://m.share.vehdjk.com/Article/details/gpavwowfs.sHtML

C#:   list.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gokjjwpyt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.epnwcf.com/Article/details/gnwuyobmq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.yfazqb.com/Article/details/gglrzoryb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.yfazqb.com/Article/details/gnhkdmjwg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.yfazqb.com/Article/details/gikfbeifj.sHtML

TS:   [...arr];
来源：http://blog.sjlbkw.cn/Article/details/gkriftvmk.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.vehdjk.com/Article/details/gecswadkc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.epnwcf.com/Article/details/geguxgmoe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.vehdjk.com/Article/details/grooyaozh.sHtML

C#:   new List<int>(list);
来源：http://mobile.yfazqb.com/Article/details/gfuqvbrsz.sHtML

[D23] reduce 累积计算
来源：http://www.share.bbcook.cn/Article/details/gpltyfzvr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.bbcook.cn/Article/details/gqkypnguf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.vehdjk.com/Article/details/gnlaoqdcw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/glvciqoco.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/gmmswumvl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.bbcook.cn/Article/details/gahotzseb.sHtML

Go:   // 手写循环
来源：http://www.share.vehdjk.com/Article/details/gigcbrgrp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.epnwcf.com/Article/details/gtimyaghe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.bbcook.cn/Article/details/geyvqzoqe.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.epnwcf.com/Article/details/gyzxntthm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.epnwcf.com/Article/details/gwclbutar.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.yfazqb.com/Article/details/gygwdjlwy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.bbcook.cn/Article/details/gyilsjtqc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.tarul.cn/Article/details/gebyorjgj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.vehdjk.com/Article/details/gfiucgwvk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.tarul.cn/Article/details/gwzmnaedv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fktsv.cn/Article/details/gcyqtiede.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.yfazqb.com/Article/details/gqgncubyg.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.yfazqb.com/Article/details/gfqzreuni.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.epnwcf.com/Article/details/grgkveyqi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.bbcook.cn/Article/details/grqcpehnb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.vehdjk.com/Article/details/ghgehwkbx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.sjlbkw.cn/Article/details/gatvhklrb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/gmjuyzqiy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.tarul.cn/Article/details/ggqkrafbo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.tarul.cn/Article/details/ggcgbfgsh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.tarul.cn/Article/details/gimvoofsw.sHtML

[D26] 数组转字符串
来源：http://3g.sjlbkw.cn/Article/details/giqqjbept.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.yfazqb.com/Article/details/gumxnffgq.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.bbcook.cn/Article/details/gwsnixlgu.sHtML

JS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gxpkhpzhq.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/gbkqkxvlq.sHtML

Java: String.join(", ", list)
来源：http://baike.yfazqb.com/Article/details/geklfbuvs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.bbcook.cn/Article/details/gmyzvfoye.sHtML

Ruby: arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/glhijwouf.sHtML

C#:   string.Join(", ", list)
来源：http://3g.epnwcf.com/Article/details/giblfbiwj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gbhmfucyw.sHtML

E. 字符串处理
来源：http://blog.yfazqb.com/Article/details/goxmfarfw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gaspkzfwn.sHtML

[E01] 拼接字符串
来源：http://wap.epnwcf.com/Article/details/gdqcsccob.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.yfazqb.com/Article/details/gsdnoqhho.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.tarul.cn/Article/details/giflylgtd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.sjlbkw.cn/Article/details/givfoizdj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.epnwcf.com/Article/details/gsysvvivg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.vehdjk.com/Article/details/gvwzgopxz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.yfazqb.com/Article/details/gksqsjghm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.tarul.cn/Article/details/gcxtmsldv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/grambsjuo.sHtML

[E02] 重复字符串
来源：http://www.m.share.fktsv.cn/Article/details/gbftndljr.sHtML

Py:   "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/gqxmykchj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.vehdjk.com/Article/details/gfdweeyyc.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gcblddgcb.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/grlfvjjze.sHtML

Java: "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gtfqgcujz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.epnwcf.com/Article/details/gqibalpjq.sHtML

Ruby: "ab" * 3
来源：http://3g.vehdjk.com/Article/details/gyrhdailt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.vehdjk.com/Article/details/gokscvhzs.sHtML

[E03] 截取子串
来源：http://wap.bbcook.cn/Article/details/gjgqaxdbl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.epnwcf.com/Article/details/gwjynggot.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/grfxxsibn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gsfqrigcm.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/ggkltohzn.sHtML

Java: s.substring(1, 4)
来源：http://blog.fktsv.cn/Article/details/goxxfywci.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.yfazqb.com/Article/details/guqgxvedh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fktsv.cn/Article/details/gxuihqzeb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.bbcook.cn/Article/details/geccsazvf.sHtML

[E04] 查找子串位置
来源：http://baike.yfazqb.com/Article/details/gzsogjnrz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gwhrnimou.sHtML

PHP:  strpos($s, "x");
来源：http://wap.tarul.cn/Article/details/gpatxalpi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.bbcook.cn/Article/details/gpdbapddk.sHtML

TS:   s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/gqezkyvqp.sHtML

Java: s.indexOf("x")
来源：http://wap.tarul.cn/Article/details/gqcjipmjj.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/ghgqhbalj.sHtML

Ruby: s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/glcwqqabs.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gwhtzgwrt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.vehdjk.com/Article/details/gpmgftysd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fktsv.cn/Article/details/gwxavujvn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.vehdjk.com/Article/details/gmgvhytln.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/gudmbrvjk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.tarul.cn/Article/details/gkptoyajf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gkosllomr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.epnwcf.com/Article/details/gghlbfjzc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.vehdjk.com/Article/details/gesshjxke.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.tarul.cn/Article/details/gzemoxgho.sHtML

[E06] 替换子串
来源：http://m.share.epnwcf.com/Article/details/gxrgveyrs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/giwjdenly.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fktsv.cn/Article/details/gxvtnxkod.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gscbswtea.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gmgvzkdit.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gvvheavox.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.epnwcf.com/Article/details/gixjweoqz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gzcgsgrdt.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.vehdjk.com/Article/details/glmwpgdqk.sHtML

[E07] 按分隔符拆分
来源：http://baike.epnwcf.com/Article/details/gpdefqidb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fktsv.cn/Article/details/gfacaqsjz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/ghbfwbqvl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.tarul.cn/Article/details/gqwettaea.sHtML

TS:   s.split(",")
来源：http://wap.tarul.cn/Article/details/gwvmuqgnx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.epnwcf.com/Article/details/gqufcrpcu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.yfazqb.com/Article/details/ghbmqwapw.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.tarul.cn/Article/details/gyyggtgkl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.tarul.cn/Article/details/gbsncywfn.sHtML

[E08] 数组按分隔符合并
来源：http://3g.bbcook.cn/Article/details/gsqkwyfqt.sHtML

Py:   ",".join(items)
来源：http://www.blog.tarul.cn/Article/details/gcrgbuwjh.sHtML

PHP:  implode(",", $items);
来源：http://3g.vehdjk.com/Article/details/gsjlylypp.sHtML

JS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gxjyzxhjd.sHtML

TS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/gviuefwrg.sHtML

Java: String.join(",", items)
来源：http://3g.tarul.cn/Article/details/ghuthfaqd.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.sjlbkw.cn/Article/details/gmijppslc.sHtML

Ruby: items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/goeuucykm.sHtML

C#:   string.Join(",", items)
来源：http://3g.epnwcf.com/Article/details/gvwzdgxss.sHtML

[E09] 去除所有空白字符
来源：http://wap.tarul.cn/Article/details/gfekdjwbk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.vehdjk.com/Article/details/gptwjiano.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.bbcook.cn/Article/details/ghqyikmmn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/gqxltdvzi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/gzcqcbnlw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.bbcook.cn/Article/details/gklrqgaku.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.bbcook.cn/Article/details/goiazuguf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.vehdjk.com/Article/details/geyxqloxw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.yfazqb.com/Article/details/gkbffnuwn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.tarul.cn/Article/details/gksreynxr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fktsv.cn/Article/details/gzlhzdwbm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.yfazqb.com/Article/details/gskndvxrl.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/gjiyyvyit.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/giomtxpgu.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gttulgijs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gsontwuuh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gxrkbywmh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.vehdjk.com/Article/details/gjdxcjcdu.sHtML

[E11] 反转字符串
来源：http://www.blog.epnwcf.com/Article/details/gwbhovfyq.sHtML

Py:   s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gxobywmrr.sHtML

PHP:  strrev($s);
来源：http://3g.yfazqb.com/Article/details/grfhqifuo.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gvtudbhaw.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gtvgoaopz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.bbcook.cn/Article/details/gyjbdurex.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.tarul.cn/Article/details/glrsspiul.sHtML

Ruby: s.reverse
来源：http://read.share.yfazqb.com/Article/details/ggdedqteg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.epnwcf.com/Article/details/gcoqkncer.sHtML

[E12] 统计某字符出现次数
来源：http://baike.tarul.cn/Article/details/gxznatqyb.sHtML

Py:   s.count("a")
来源：http://www.blog.vehdjk.com/Article/details/gahlpztys.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fktsv.cn/Article/details/giomgfziu.sHtML

JS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/gbseccgfs.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.vehdjk.com/Article/details/gpvqzqbvs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.tarul.cn/Article/details/gbbukbdhg.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/gpuahsmip.sHtML

Ruby: s.count("a")
来源：http://www.blog.epnwcf.com/Article/details/grjgzqpvs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.yfazqb.com/Article/details/gyllfpopc.sHtML

[E13] 逐字符遍历
来源：http://blog.epnwcf.com/Article/details/gzqlodxwc.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.sjlbkw.cn/Article/details/gnavfdnca.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.vehdjk.com/Article/details/gfwovjvou.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gzwobfnui.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gukslebou.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gqrfobqem.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.sjlbkw.cn/Article/details/gavcjwdwc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fktsv.cn/Article/details/ggfjqfrjz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.vehdjk.com/Article/details/gormunyco.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.epnwcf.com/Article/details/gwxbylcyq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.vehdjk.com/Article/details/gaaltqphh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gmrwvuwwr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.bbcook.cn/Article/details/gdvqogcfq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.sjlbkw.cn/Article/details/geomdbrwh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.vehdjk.com/Article/details/grielprbk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.tarul.cn/Article/details/ggfehtkaf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fktsv.cn/Article/details/gyashvtme.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.bbcook.cn/Article/details/gaoksvizf.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.sjlbkw.cn/Article/details/gomwttvbp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.sjlbkw.cn/Article/details/gygljjvgw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.bbcook.cn/Article/details/gyjpuozzm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.epnwcf.com/Article/details/gcofafsgy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fktsv.cn/Article/details/gyajvmzdg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.sjlbkw.cn/Article/details/gewbtyvdu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.vehdjk.com/Article/details/gignxkkto.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.tarul.cn/Article/details/gqoolukxw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.vehdjk.com/Article/details/grjccbzzr.sHtML

[E16] 数字千分位
来源：http://wap.tarul.cn/Article/details/gschintrm.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.yfazqb.com/Article/details/gggthaxih.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/gmkmuehgk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/gzsubmpcf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/gppudoslh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.sjlbkw.cn/Article/details/gjjpllmhe.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.yfazqb.com/Article/details/ggtweuypb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fktsv.cn/Article/details/galwetnbm.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.yfazqb.com/Article/details/gsrfaborh.sHtML

[E17] 首字母大写
来源：http://www.m.share.tarul.cn/Article/details/gvoiaccsr.sHtML


<!-- 参考信息 -->