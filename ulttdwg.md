代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.m.share.tarul.cn/Article/details/gfuzejrni.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.epnwcf.com/Article/details/gnbztbeql.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.epnwcf.com/Article/details/gtplykvzs.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gminwjwgh.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.vehdjk.com/Article/details/gtwuhseld.sHtML

Java: list.subList(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gldvwjkce.sHtML

Go:   arr[1:4]
来源：http://baike.sjlbkw.cn/Article/details/gouceqrfl.sHtML

Ruby: arr[1, 3]
来源：http://wap.yfazqb.com/Article/details/grbvdeend.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.bbcook.cn/Article/details/gzccvjdxr.sHtML

[D08] 合并两个数组
来源：http://m.share.tarul.cn/Article/details/gvfmtsnno.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.tarul.cn/Article/details/gqkpiryla.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.vehdjk.com/Article/details/gadmalrqn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.bbcook.cn/Article/details/ggbiblobp.sHtML

TS:   [...a, ...b];
来源：http://baike.epnwcf.com/Article/details/gjgcxrfnx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.vehdjk.com/Article/details/gwuypuvvd.sHtML

Go:   append(a, b...)
来源：http://www.share.sjlbkw.cn/Article/details/gkxgrrkqi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.yfazqb.com/Article/details/gkrwqsxyy.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.epnwcf.com/Article/details/gmzjrxhnq.sHtML

[D09] 排序（升序）
来源：http://3g.sjlbkw.cn/Article/details/glummsvwd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/gamqdxkan.sHtML

PHP:  sort($arr);
来源：http://read.share.vehdjk.com/Article/details/gyrvhmxrd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.vehdjk.com/Article/details/gkdecafqo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.yfazqb.com/Article/details/gtpnaqdsh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.sjlbkw.cn/Article/details/gwcfckzja.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gthqhdgkx.sHtML

Ruby: arr.sort
来源：http://read.share.yfazqb.com/Article/details/gddqgkvyp.sHtML

C#:   list.Sort();
来源：http://www.share.vehdjk.com/Article/details/gzxpgqcnw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.vehdjk.com/Article/details/gjsoesxyq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.yfazqb.com/Article/details/grhmillim.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.tarul.cn/Article/details/grqfyshie.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/gbnvoclpk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.vehdjk.com/Article/details/grsshapiw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.epnwcf.com/Article/details/geyfefhyl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.vehdjk.com/Article/details/gbykwfwbn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxzifkqw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.tarul.cn/Article/details/gnpivagof.sHtML

[D11] 反转数组
来源：http://read.share.tarul.cn/Article/details/gwwrlryxt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.epnwcf.com/Article/details/gsmkhmwar.sHtML

PHP:  array_reverse($arr);
来源：http://wap.bbcook.cn/Article/details/gqygrnjsn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.bbcook.cn/Article/details/gmlwyscra.sHtML

TS:   [...arr].reverse();
来源：http://blog.yfazqb.com/Article/details/gptfdcluf.sHtML

Java: Collections.reverse(list);
来源：http://3g.yfazqb.com/Article/details/gwqtdjqaj.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.vehdjk.com/Article/details/gixnipayf.sHtML

Ruby: arr.reverse
来源：http://wap.bbcook.cn/Article/details/gjtyuvgji.sHtML

C#:   list.Reverse();
来源：http://www.m.share.yfazqb.com/Article/details/gsiriddeg.sHtML

[D12] 查找元素下标
来源：http://read.share.yfazqb.com/Article/details/gmimylycq.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.vehdjk.com/Article/details/gwxaqoblu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.vehdjk.com/Article/details/ghffmcvko.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.vehdjk.com/Article/details/gnpwnesod.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.epnwcf.com/Article/details/gvqyjgynd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.tarul.cn/Article/details/gtqlaezvd.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fktsv.cn/Article/details/gvjqnhsiv.sHtML

Ruby: arr.index(x)
来源：http://www.share.sjlbkw.cn/Article/details/gelrpwffc.sHtML

C#:   list.IndexOf(x);
来源：http://blog.sjlbkw.cn/Article/details/gkbydbdfp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.vehdjk.com/Article/details/gsgsegmxs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.vehdjk.com/Article/details/gmlqxfgzn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.sjlbkw.cn/Article/details/gtmasdkpp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gnbyxgpnq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/gfqjaetmh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fktsv.cn/Article/details/gxzpnrvdq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.tarul.cn/Article/details/gwpcayvue.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fktsv.cn/Article/details/gemhpbuaz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.yfazqb.com/Article/details/ggbzpcljz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.tarul.cn/Article/details/gykcxajzn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.yfazqb.com/Article/details/gwlnakxjo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.tarul.cn/Article/details/goumsgykb.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/gprvplxmz.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/gyhtficai.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.bbcook.cn/Article/details/gdkkngkiv.sHtML

Go:   // 手写循环
来源：http://3g.sjlbkw.cn/Article/details/gihphitzi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.epnwcf.com/Article/details/ghmsiguqj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcoluoxl.sHtML

[D15] 去重
来源：http://baike.bbcook.cn/Article/details/guzrhunsn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.epnwcf.com/Article/details/gmnbidfun.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.yfazqb.com/Article/details/ggzuwddmr.sHtML

JS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gxzqvelbm.sHtML

TS:   [...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/giwqkwvkt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.tarul.cn/Article/details/gdcqsdsiy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.vehdjk.com/Article/details/gvjduiwsz.sHtML

Ruby: arr.uniq
来源：http://www.blog.sjlbkw.cn/Article/details/gizemuvag.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.bbcook.cn/Article/details/ghshszpoa.sHtML

[D16] 求和与平均值
来源：http://www.m.share.epnwcf.com/Article/details/gzljudpzl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gntgxgiyb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.epnwcf.com/Article/details/gcrszerqz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/govbuqite.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/glpagxdkn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.yfazqb.com/Article/details/gqdfbytwg.sHtML

Go:   // 手写循环累加
来源：http://baike.tarul.cn/Article/details/gpqyzcllz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.vehdjk.com/Article/details/grxwaksyp.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.bbcook.cn/Article/details/ghspemdsx.sHtML

[D17] 最大值与最小值
来源：http://www.share.vehdjk.com/Article/details/gvnsegesh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gzhwumalq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.tarul.cn/Article/details/gvedltrld.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.vehdjk.com/Article/details/gyfwavosi.sHtML

TS:   Math.max(...arr);
来源：http://mobile.yfazqb.com/Article/details/gepkgtfqj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.epnwcf.com/Article/details/gtavujqvm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gteaqduib.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/guphjimit.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.tarul.cn/Article/details/gsvwfcmxi.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fktsv.cn/Article/details/gjpbbwcpb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fktsv.cn/Article/details/glskirqwr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.tarul.cn/Article/details/gvrusxvhu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fktsv.cn/Article/details/gdlmtgilq.sHtML

TS:   nested.flat();
来源：http://blog.tarul.cn/Article/details/gdffnvrgy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.bbcook.cn/Article/details/geircbzpv.sHtML

Go:   // 手写双层循环
来源：http://baike.vehdjk.com/Article/details/gbjaeveiy.sHtML

Ruby: nested.flatten
来源：http://www.share.tarul.cn/Article/details/gcswbjkcg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.vehdjk.com/Article/details/gqstdgbyw.sHtML

[D19] 按字段分组
来源：http://www.blog.sjlbkw.cn/Article/details/grtthqxod.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fktsv.cn/Article/details/gxowlalkp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.vehdjk.com/Article/details/gpnnoxfjf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.yfazqb.com/Article/details/gbzkxybjt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.vehdjk.com/Article/details/gdfeytebs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.vehdjk.com/Article/details/gjpkxxggq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fktsv.cn/Article/details/gbiwxwhyw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.epnwcf.com/Article/details/getnwpkxw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.epnwcf.com/Article/details/gpftxsymk.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.sjlbkw.cn/Article/details/gsdkaqwvf.sHtML

Py:   Counter(arr)
来源：http://www.share.yfazqb.com/Article/details/gjqgjsrta.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.yfazqb.com/Article/details/gjjbidevo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gcwaiccey.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.yfazqb.com/Article/details/gwhkwiauy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.epnwcf.com/Article/details/gmmouqxiv.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.yfazqb.com/Article/details/gfqcaeepw.sHtML

Ruby: arr.tally
来源：http://www.blog.epnwcf.com/Article/details/gzsltfveb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.yfazqb.com/Article/details/ggbhixjhn.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.epnwcf.com/Article/details/gaadxchyd.sHtML

Py:   x in arr
来源：http://mobile.sjlbkw.cn/Article/details/gxvqcxfne.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.bbcook.cn/Article/details/gktmcyceh.sHtML

JS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/gzcdktbvf.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gywegyrai.sHtML

Java: list.contains(x)
来源：http://blog.vehdjk.com/Article/details/gszdkhlsi.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gfugslkwh.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.yfazqb.com/Article/details/googsphci.sHtML

C#:   list.Contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gohkzikni.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.yfazqb.com/Article/details/gqyhuscia.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gkqyncdbn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.tarul.cn/Article/details/gaomcfqum.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gvcltojrg.sHtML

TS:   [...arr];
来源：http://read.share.bbcook.cn/Article/details/gsfmyqqbr.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fktsv.cn/Article/details/gipwwacgo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.sjlbkw.cn/Article/details/ggzsyabyc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fktsv.cn/Article/details/gsqncewfe.sHtML

C#:   new List<int>(list);
来源：http://blog.epnwcf.com/Article/details/gexmzcjqi.sHtML

[D23] reduce 累积计算
来源：http://read.share.tarul.cn/Article/details/grerulnls.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.epnwcf.com/Article/details/gnsrwhhwg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gztbznlnc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/guknwuwik.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gkmbunoya.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsltefwqf.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/gvbiilmro.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.tarul.cn/Article/details/ghigzotmn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.vehdjk.com/Article/details/gbvsbanxz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.epnwcf.com/Article/details/glvumibds.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.sjlbkw.cn/Article/details/gfjkixrip.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.yfazqb.com/Article/details/gsyitabvo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.epnwcf.com/Article/details/gmmivmkby.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gdgtmznnj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.bbcook.cn/Article/details/ggfjxwaal.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fktsv.cn/Article/details/gppurzdpa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.bbcook.cn/Article/details/glnokdjrp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.bbcook.cn/Article/details/gdbitdclx.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.vehdjk.com/Article/details/gbnwryznz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.bbcook.cn/Article/details/gsdxczfvm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.yfazqb.com/Article/details/gepjbqfrl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.yfazqb.com/Article/details/gqnyuhnht.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.tarul.cn/Article/details/gfdtzttpb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.vehdjk.com/Article/details/gyvvbdjiw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fktsv.cn/Article/details/gcazrvvmo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.epnwcf.com/Article/details/ggggyblam.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.bbcook.cn/Article/details/graydlund.sHtML

[D26] 数组转字符串
来源：http://3g.fktsv.cn/Article/details/gffnzmogn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.sjlbkw.cn/Article/details/gknlufyfc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.bbcook.cn/Article/details/gkimtcwmh.sHtML

JS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/glwohrdny.sHtML

TS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gkppognja.sHtML

Java: String.join(", ", list)
来源：http://baike.sjlbkw.cn/Article/details/gomwszhke.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fktsv.cn/Article/details/gvffrqykv.sHtML

Ruby: arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gilnotquo.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gltmgdxst.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtfpfmpuz.sHtML

E. 字符串处理
来源：http://www.m.share.epnwcf.com/Article/details/gksqvxskc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxtxdqrkx.sHtML

[E01] 拼接字符串
来源：http://baike.yfazqb.com/Article/details/gzptfuyeu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.vehdjk.com/Article/details/glacsvxee.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.tarul.cn/Article/details/gqvlvmihi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gdvbtgkuc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/graadodor.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.vehdjk.com/Article/details/gpskszwgq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.vehdjk.com/Article/details/gpmvbgyyl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.yfazqb.com/Article/details/gsofidyuu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gskvmruwr.sHtML

[E02] 重复字符串
来源：http://baike.bbcook.cn/Article/details/gmviyqokd.sHtML

Py:   "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gytaabuhz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.sjlbkw.cn/Article/details/gzxccywyw.sHtML

JS:   "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gvlrttrpl.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gsqqwzswv.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/goczkxcmz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.tarul.cn/Article/details/gvsznfcxt.sHtML

Ruby: "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/gjcsuezns.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.bbcook.cn/Article/details/ghstaowhn.sHtML

[E03] 截取子串
来源：http://mobile.tarul.cn/Article/details/gbqrocuib.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.vehdjk.com/Article/details/gpmunqulr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/griyixwzg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gheyfworb.sHtML

TS:   s.slice(1, 4)
来源：http://3g.vehdjk.com/Article/details/gvfnseqph.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gyzzottdg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.epnwcf.com/Article/details/gxhugfsgn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.tarul.cn/Article/details/ganrjdfzb.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.yfazqb.com/Article/details/gqoxqgohc.sHtML

[E04] 查找子串位置
来源：http://blog.vehdjk.com/Article/details/gftewqxuy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.yfazqb.com/Article/details/gpjjtnpbr.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.tarul.cn/Article/details/gtwvqlryg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.tarul.cn/Article/details/grhndexmw.sHtML

TS:   s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gephqxwsx.sHtML

Java: s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gaqbgbjhg.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fktsv.cn/Article/details/gueofxxwk.sHtML

Ruby: s.index("x")
来源：http://baike.fktsv.cn/Article/details/glfnkzblx.sHtML

C#:   s.IndexOf("x")
来源：http://baike.yfazqb.com/Article/details/gwfgzkjpr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.epnwcf.com/Article/details/glozbedus.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.epnwcf.com/Article/details/gkaybpkaz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.vehdjk.com/Article/details/gbingbodp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.yfazqb.com/Article/details/gwlrkgeeb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.epnwcf.com/Article/details/gsmsivhce.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gdfhxorcv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.tarul.cn/Article/details/glelibjji.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.tarul.cn/Article/details/grxeswuam.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.tarul.cn/Article/details/grodhqfbn.sHtML

[E06] 替换子串
来源：http://read.share.fktsv.cn/Article/details/ggrmerhjt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gkjtrgwwu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.epnwcf.com/Article/details/gtqizkkak.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/ggviisepx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gnstazmee.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gnlzbdowo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.epnwcf.com/Article/details/gtymgfumn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gyrcrhvwx.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gdpqaitah.sHtML

[E07] 按分隔符拆分
来源：http://mobile.vehdjk.com/Article/details/grpvgmcvj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.tarul.cn/Article/details/gtbsvcpjq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.vehdjk.com/Article/details/gqzufjobe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fktsv.cn/Article/details/gpwpicyvm.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/glcpnpluq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fktsv.cn/Article/details/gbqgmnklj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.tarul.cn/Article/details/githzbbzv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.bbcook.cn/Article/details/gippuedtf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.sjlbkw.cn/Article/details/gvxwdhfkp.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.vehdjk.com/Article/details/gaduutllq.sHtML

Py:   ",".join(items)
来源：http://www.m.share.epnwcf.com/Article/details/giawswmlc.sHtML

PHP:  implode(",", $items);
来源：http://mobile.tarul.cn/Article/details/grrlwmgab.sHtML

JS:   items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gysjhrcjt.sHtML

TS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/gelxkbbyt.sHtML

Java: String.join(",", items)
来源：http://m.share.vehdjk.com/Article/details/gmihxszhx.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.yfazqb.com/Article/details/gkwgmhcdh.sHtML

Ruby: items.join(",")
来源：http://baike.yfazqb.com/Article/details/gooixwujg.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gocywimba.sHtML

[E09] 去除所有空白字符
来源：http://baike.bbcook.cn/Article/details/gtsqgqyeu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fktsv.cn/Article/details/gmfjumyrn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fktsv.cn/Article/details/griikxwvb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gnkfedyji.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/gewseuznz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.yfazqb.com/Article/details/gzkuowbeb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.yfazqb.com/Article/details/gyisitliy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.bbcook.cn/Article/details/giumortgn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.bbcook.cn/Article/details/glurblyso.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.sjlbkw.cn/Article/details/gcfalbvkv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.tarul.cn/Article/details/gceivgmoq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.epnwcf.com/Article/details/gpojgvmgc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gupfxpouy.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/galdjdtsf.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gxinpxqnr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gdqbumdrt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/ggzjfphye.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.sjlbkw.cn/Article/details/glmypqvah.sHtML

[E11] 反转字符串
来源：http://mobile.tarul.cn/Article/details/gnzsqazyy.sHtML

Py:   s[::-1]
来源：http://m.share.tarul.cn/Article/details/gxwedwxfn.sHtML

PHP:  strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gtdrccpjm.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gzgthzjbo.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gtzjtadfm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fktsv.cn/Article/details/ghrnfwzgf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fktsv.cn/Article/details/gnvhbndfa.sHtML

Ruby: s.reverse
来源：http://baike.fktsv.cn/Article/details/gszraqvmz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/gssihlvih.sHtML

[E12] 统计某字符出现次数
来源：http://3g.vehdjk.com/Article/details/gttusqhgd.sHtML

Py:   s.count("a")
来源：http://blog.fktsv.cn/Article/details/gnlddkjnp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.vehdjk.com/Article/details/gyspuhmay.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/gsdepgcin.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/gxwodnufp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.epnwcf.com/Article/details/gezxwvfiv.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.tarul.cn/Article/details/gjxkktied.sHtML

Ruby: s.count("a")
来源：http://mobile.tarul.cn/Article/details/gudeomudh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhcjtgzx.sHtML

[E13] 逐字符遍历
来源：http://mobile.sjlbkw.cn/Article/details/gyrasowrz.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.bbcook.cn/Article/details/gjeoynxzs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.vehdjk.com/Article/details/ghxbufvjc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/gdxdgobzr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gftnlwetd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.vehdjk.com/Article/details/ggvufsknq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.bbcook.cn/Article/details/gqjocnzkd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.bbcook.cn/Article/details/gofcegcld.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/ghcltocpn.sHtML


<!-- 参考信息 -->