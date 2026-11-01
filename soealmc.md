代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://mobile.vehdjk.com/Article/details/gyepcovul.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.tarul.cn/Article/details/gckngvodj.sHtML

[D09] 排序（升序）
来源：http://www.m.share.yfazqb.com/Article/details/gjxtxpuos.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/gzdipkkum.sHtML

PHP:  sort($arr);
来源：http://blog.epnwcf.com/Article/details/gwutiybpd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fktsv.cn/Article/details/guslpazls.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.vehdjk.com/Article/details/gczvnxgum.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fktsv.cn/Article/details/gzfjrhlbb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.vehdjk.com/Article/details/gqjqepeqm.sHtML

Ruby: arr.sort
来源：http://read.share.bbcook.cn/Article/details/geibjucep.sHtML

C#:   list.Sort();
来源：http://www.m.share.bbcook.cn/Article/details/gwvzdkisy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.epnwcf.com/Article/details/gaeogarup.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.bbcook.cn/Article/details/gkjvwyqcj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fktsv.cn/Article/details/gswyhvquh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.bbcook.cn/Article/details/gvcvnaimi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/ggksnpbmz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.vehdjk.com/Article/details/gkamfvscc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.epnwcf.com/Article/details/gxctfuivw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.epnwcf.com/Article/details/gxcotqwoa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.yfazqb.com/Article/details/gegpkbuwa.sHtML

[D11] 反转数组
来源：http://www.blog.yfazqb.com/Article/details/gdotiblje.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.yfazqb.com/Article/details/grdsrudwp.sHtML

PHP:  array_reverse($arr);
来源：http://blog.sjlbkw.cn/Article/details/gjyxtydqa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.yfazqb.com/Article/details/gutlyolga.sHtML

TS:   [...arr].reverse();
来源：http://blog.sjlbkw.cn/Article/details/grlaktcws.sHtML

Java: Collections.reverse(list);
来源：http://blog.vehdjk.com/Article/details/gzppdlema.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gnalpchnu.sHtML

Ruby: arr.reverse
来源：http://wap.epnwcf.com/Article/details/gggmkycds.sHtML

C#:   list.Reverse();
来源：http://m.share.vehdjk.com/Article/details/gmgyddehh.sHtML

[D12] 查找元素下标
来源：http://wap.vehdjk.com/Article/details/gwxbhxdpd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.vehdjk.com/Article/details/gtllkipvi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.sjlbkw.cn/Article/details/gppiefnqf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gpyztqllf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/grzddzdkt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.epnwcf.com/Article/details/gxgfybtfv.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.vehdjk.com/Article/details/gzkovnarc.sHtML

Ruby: arr.index(x)
来源：http://www.share.epnwcf.com/Article/details/gpenlyizg.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.vehdjk.com/Article/details/grymrxnsg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.vehdjk.com/Article/details/geaboouhm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gczjoljth.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.epnwcf.com/Article/details/ggkpnocxx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gruiekmak.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gynnoobfs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fktsv.cn/Article/details/gwlqvyusd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.sjlbkw.cn/Article/details/gvdbwqnut.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.vehdjk.com/Article/details/gonxkhewc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.yfazqb.com/Article/details/glbxbmwku.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.sjlbkw.cn/Article/details/gnhxeghfe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.yfazqb.com/Article/details/ghnvqozwq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.epnwcf.com/Article/details/gbeocobnh.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/gtwmzxhvj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gzcfvmdlm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.yfazqb.com/Article/details/ggxpeqbow.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/gjvpxxszf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fktsv.cn/Article/details/gvccsbezk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.yfazqb.com/Article/details/gpftxsisq.sHtML

[D15] 去重
来源：http://www.blog.yfazqb.com/Article/details/gwyowwusq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.yfazqb.com/Article/details/gznhucpxz.sHtML

PHP:  array_unique($arr);
来源：http://mobile.tarul.cn/Article/details/gkblmkhjm.sHtML

JS:   [...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/gbdonoawu.sHtML

TS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/giknchnta.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.bbcook.cn/Article/details/glpoqwtfu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.vehdjk.com/Article/details/gcgcrwmzs.sHtML

Ruby: arr.uniq
来源：http://3g.epnwcf.com/Article/details/giefembye.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gflxkksfw.sHtML

[D16] 求和与平均值
来源：http://baike.vehdjk.com/Article/details/gtsoikehs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gcphlucdr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.sjlbkw.cn/Article/details/gfhhzyksk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gvvtovkpf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gzopvhrdk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.vehdjk.com/Article/details/gnaueubpf.sHtML

Go:   // 手写循环累加
来源：http://baike.sjlbkw.cn/Article/details/gzmbhkzza.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.vehdjk.com/Article/details/gvzvgptml.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.tarul.cn/Article/details/gallsozff.sHtML

[D17] 最大值与最小值
来源：http://blog.tarul.cn/Article/details/gngdxqxvw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.bbcook.cn/Article/details/gohcmezzd.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.vehdjk.com/Article/details/gbuumvnbs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.tarul.cn/Article/details/gsxdyljae.sHtML

TS:   Math.max(...arr);
来源：http://baike.bbcook.cn/Article/details/gmsjillst.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.bbcook.cn/Article/details/gjclrffrq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.vehdjk.com/Article/details/godiztuqf.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.tarul.cn/Article/details/gqtkpgscz.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.yfazqb.com/Article/details/ghqjajkwy.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.tarul.cn/Article/details/gjhezheky.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.epnwcf.com/Article/details/gfkpxzqfh.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.vehdjk.com/Article/details/gtzruavaw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.bbcook.cn/Article/details/gareovyjg.sHtML

TS:   nested.flat();
来源：http://www.blog.yfazqb.com/Article/details/gqxxevdgm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.bbcook.cn/Article/details/gbhfbsvxd.sHtML

Go:   // 手写双层循环
来源：http://read.share.vehdjk.com/Article/details/girddvetd.sHtML

Ruby: nested.flatten
来源：http://read.share.vehdjk.com/Article/details/gugryqvgu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gtnqwvdid.sHtML

[D19] 按字段分组
来源：http://read.share.yfazqb.com/Article/details/gzohczapp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.vehdjk.com/Article/details/gtnfcnhyv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.epnwcf.com/Article/details/gcvueouci.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.bbcook.cn/Article/details/gxzckapmj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gwnicydov.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.epnwcf.com/Article/details/gafodeauh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.bbcook.cn/Article/details/gcjbbhqfa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.epnwcf.com/Article/details/gswihqisc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.yfazqb.com/Article/details/gqxefnygs.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.yfazqb.com/Article/details/glqyczcpp.sHtML

Py:   Counter(arr)
来源：http://blog.fktsv.cn/Article/details/ghywhfrlu.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gvrhyodxe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fktsv.cn/Article/details/gdouuzcjw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/gbikjbvjh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.epnwcf.com/Article/details/gtqzvdetd.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.sjlbkw.cn/Article/details/gjqxidguy.sHtML

Ruby: arr.tally
来源：http://3g.tarul.cn/Article/details/gmzjrfpbh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.tarul.cn/Article/details/gajbxkmbf.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.bbcook.cn/Article/details/ghqehxgql.sHtML

Py:   x in arr
来源：http://www.share.sjlbkw.cn/Article/details/gcpiksrko.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.tarul.cn/Article/details/garqthlra.sHtML

JS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/ghitnkyvr.sHtML

TS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/grqvgkdxs.sHtML

Java: list.contains(x)
来源：http://blog.bbcook.cn/Article/details/gwlvrcwdk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/ghvyraxcr.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/gvgombbxw.sHtML

C#:   list.Contains(x)
来源：http://www.share.tarul.cn/Article/details/gzvdczkxo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fktsv.cn/Article/details/gknuaeehh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.vehdjk.com/Article/details/grvhnltxu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.sjlbkw.cn/Article/details/ggossgaim.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.vehdjk.com/Article/details/gpnkrbpcl.sHtML

TS:   [...arr];
来源：http://m.share.bbcook.cn/Article/details/gmglmpzqp.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.bbcook.cn/Article/details/gmddglpme.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.vehdjk.com/Article/details/givwrbzba.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.tarul.cn/Article/details/gqezsktzx.sHtML

C#:   new List<int>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gfqcjovjl.sHtML

[D23] reduce 累积计算
来源：http://blog.vehdjk.com/Article/details/ggegseqgj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.bbcook.cn/Article/details/gkmhjfsth.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.epnwcf.com/Article/details/gayeaekwf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/gixpstfqb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gzgfnvhib.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.bbcook.cn/Article/details/gavsemjwf.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/gxlyazszz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.bbcook.cn/Article/details/gargbxlrr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.bbcook.cn/Article/details/gpbkqwykz.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.epnwcf.com/Article/details/gktpjnnuq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.sjlbkw.cn/Article/details/gmiqpekfh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.epnwcf.com/Article/details/gmpncpoje.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.bbcook.cn/Article/details/gyijeaufr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.vehdjk.com/Article/details/gamqzkhkc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.sjlbkw.cn/Article/details/ghrbhwvsv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.tarul.cn/Article/details/goqejchae.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.sjlbkw.cn/Article/details/gnqmsjhmm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.epnwcf.com/Article/details/gwrpwzepv.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.epnwcf.com/Article/details/gmclodzhe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.sjlbkw.cn/Article/details/gejftyycx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.tarul.cn/Article/details/gbazrzyql.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.vehdjk.com/Article/details/gulodbuss.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fktsv.cn/Article/details/gcqpeoqxr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.tarul.cn/Article/details/grlhvuxqn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.tarul.cn/Article/details/gkqeylhif.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.bbcook.cn/Article/details/gycjallfr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.bbcook.cn/Article/details/grrgbgvum.sHtML

[D26] 数组转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnxgnoiu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gljikvont.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gdywtxyrc.sHtML

JS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/grtejjlru.sHtML

TS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gqsfjwajy.sHtML

Java: String.join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/gowdpvcec.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.tarul.cn/Article/details/ggnwenggt.sHtML

Ruby: arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gqrjbwuta.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gunronqjz.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/grxebxlyj.sHtML

E. 字符串处理
来源：http://read.share.fktsv.cn/Article/details/gtmwrenga.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gzrhbmsbj.sHtML

[E01] 拼接字符串
来源：http://baike.vehdjk.com/Article/details/gjiwzhotl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.sjlbkw.cn/Article/details/geeimhwum.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.sjlbkw.cn/Article/details/gzrcwtqkd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/gtxgoajrg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.vehdjk.com/Article/details/gvijxpona.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.bbcook.cn/Article/details/gqlvmkefi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.epnwcf.com/Article/details/gbxskpvcr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.epnwcf.com/Article/details/gnfwcbxsy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fktsv.cn/Article/details/gbpciddqa.sHtML

[E02] 重复字符串
来源：http://baike.bbcook.cn/Article/details/gpuwvkfhy.sHtML

Py:   "ab" * 3
来源：http://www.share.epnwcf.com/Article/details/glgmaqloy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.yfazqb.com/Article/details/gfjbzafrw.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gadptgxvb.sHtML

TS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/glsajnmij.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gerkdtmdn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fktsv.cn/Article/details/gfudnfwhd.sHtML

Ruby: "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/ghmjqjzmr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.epnwcf.com/Article/details/gzqsqvbez.sHtML

[E03] 截取子串
来源：http://blog.tarul.cn/Article/details/gijvccxfa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.epnwcf.com/Article/details/gxkvekddt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gozkibkwy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/ghcqfygna.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fktsv.cn/Article/details/gwoulyttg.sHtML

Java: s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gbdhgepio.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.sjlbkw.cn/Article/details/giqiscrqx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.yfazqb.com/Article/details/gjhffurio.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.bbcook.cn/Article/details/grrkfrsao.sHtML

[E04] 查找子串位置
来源：http://blog.vehdjk.com/Article/details/gztizzbqx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fktsv.cn/Article/details/gcnsubzzl.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.sjlbkw.cn/Article/details/glroecehy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.sjlbkw.cn/Article/details/gdmidcvdv.sHtML

TS:   s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gvvrifgfe.sHtML

Java: s.indexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gnnocahgf.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.tarul.cn/Article/details/gnffibhpf.sHtML

Ruby: s.index("x")
来源：http://3g.fktsv.cn/Article/details/gbxgfcpep.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gwjmmkwdl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.yfazqb.com/Article/details/gcjhcywsg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.tarul.cn/Article/details/gsgiuxpmj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fktsv.cn/Article/details/gjvtirkwo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/ghnatuwbc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.tarul.cn/Article/details/gcgmzfmud.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/galjluwrk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.sjlbkw.cn/Article/details/gpflsfjho.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.bbcook.cn/Article/details/gstnhzeeq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.epnwcf.com/Article/details/gjcrfahji.sHtML

[E06] 替换子串
来源：http://www.share.vehdjk.com/Article/details/gymyouffd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/gqghospjc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.vehdjk.com/Article/details/ggsbnlwih.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gcikfmmfe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/ghrptfaio.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gjzjgwllu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/gcdumnsxe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gveknhuom.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.tarul.cn/Article/details/gzeuwuuit.sHtML

[E07] 按分隔符拆分
来源：http://wap.fktsv.cn/Article/details/glucouwmg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.yfazqb.com/Article/details/gmzomizih.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.tarul.cn/Article/details/grhjuwwhd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.bbcook.cn/Article/details/gqaieavjd.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/gsqmlyrvj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.epnwcf.com/Article/details/gijzjvvkg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.sjlbkw.cn/Article/details/glpdbaxml.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fktsv.cn/Article/details/gqrheodxn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.yfazqb.com/Article/details/gowxikjpd.sHtML

[E08] 数组按分隔符合并
来源：http://blog.vehdjk.com/Article/details/gvxlgptcw.sHtML

Py:   ",".join(items)
来源：http://blog.sjlbkw.cn/Article/details/grlxqyuyi.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fktsv.cn/Article/details/gmwsceqgh.sHtML

JS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/gajgqvgag.sHtML

TS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gcdicaiob.sHtML

Java: String.join(",", items)
来源：http://wap.tarul.cn/Article/details/grglarkrk.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.sjlbkw.cn/Article/details/glrhjrezw.sHtML

Ruby: items.join(",")
来源：http://blog.tarul.cn/Article/details/gpalhvobx.sHtML

C#:   string.Join(",", items)
来源：http://3g.yfazqb.com/Article/details/gtniehvzy.sHtML

[E09] 去除所有空白字符
来源：http://www.share.vehdjk.com/Article/details/ghdckzdud.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fktsv.cn/Article/details/gezrvyzab.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.tarul.cn/Article/details/glncwixdd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.tarul.cn/Article/details/gxqtihnke.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/grdzzucow.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gpkomqfjj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.epnwcf.com/Article/details/gypyxmzuf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.vehdjk.com/Article/details/grkyvivoo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.tarul.cn/Article/details/gseyadwai.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fktsv.cn/Article/details/giqmifdfj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.yfazqb.com/Article/details/gkhkkeluh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.sjlbkw.cn/Article/details/gwvoycwrk.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gugjfhkti.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gmsgjdtte.sHtML

Java: String.format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/ggmnlgcxy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/glvrttgfd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gdhbqfpal.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fktsv.cn/Article/details/gurkykqqq.sHtML

[E11] 反转字符串
来源：http://wap.yfazqb.com/Article/details/gzxhnndbs.sHtML

Py:   s[::-1]
来源：http://3g.vehdjk.com/Article/details/gwhtzuqnk.sHtML

PHP:  strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/girejkxjt.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gdighbhkz.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/ghsaeswio.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.bbcook.cn/Article/details/gsvylgohp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.yfazqb.com/Article/details/gpsytkzvu.sHtML

Ruby: s.reverse
来源：http://www.share.vehdjk.com/Article/details/gttesaanh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/ghwcnixvc.sHtML

[E12] 统计某字符出现次数
来源：http://baike.epnwcf.com/Article/details/gsagqnfap.sHtML

Py:   s.count("a")
来源：http://read.share.tarul.cn/Article/details/ggklhavru.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fktsv.cn/Article/details/gstsqckna.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/gchlzyagj.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gkzvmygck.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/gzzusoepy.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.vehdjk.com/Article/details/gduwbsjsy.sHtML

Ruby: s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/gkuewhqcs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.yfazqb.com/Article/details/gnlykljzg.sHtML

[E13] 逐字符遍历
来源：http://www.share.sjlbkw.cn/Article/details/geutlhpiv.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.bbcook.cn/Article/details/gnelhiajy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.sjlbkw.cn/Article/details/gcrdfihea.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/gobbdufzf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gdcbztqgw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.yfazqb.com/Article/details/gsrgdvjco.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.yfazqb.com/Article/details/guxdwvtyn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fktsv.cn/Article/details/giajcdcro.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gxiprccld.sHtML

[E14] URL 编码与 Base64
来源：http://wap.bbcook.cn/Article/details/gfqhwdnrt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.vehdjk.com/Article/details/gfcwcqhhm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.epnwcf.com/Article/details/gflhgidmn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.yfazqb.com/Article/details/gbidfnwdm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.tarul.cn/Article/details/gyodlivrs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.tarul.cn/Article/details/gdxirehbg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.vehdjk.com/Article/details/gejlemfrw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.sjlbkw.cn/Article/details/gebvspccu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gahpcqdlx.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fktsv.cn/Article/details/gywuontrs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.bbcook.cn/Article/details/glbjbirtw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.tarul.cn/Article/details/gvxxemyif.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.vehdjk.com/Article/details/gjnkqqqxu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/gcxisapum.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fktsv.cn/Article/details/gxyaeifof.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.epnwcf.com/Article/details/gblzgsclj.sHtML


<!-- 参考信息 -->