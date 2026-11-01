代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gdreivhym.sHtML

[D08] 合并两个数组
来源：http://m.share.fktsv.cn/Article/details/gystrcvfi.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.bbcook.cn/Article/details/gvvcprzuk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.epnwcf.com/Article/details/gxdwmnveh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.vehdjk.com/Article/details/gyrjfnivj.sHtML

TS:   [...a, ...b];
来源：http://mobile.yfazqb.com/Article/details/gjzjvlyag.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.epnwcf.com/Article/details/gaqtlmvzk.sHtML

Go:   append(a, b...)
来源：http://mobile.yfazqb.com/Article/details/gpgqdpkxo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.yfazqb.com/Article/details/gmrlyaayi.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/ganmpsrat.sHtML

[D09] 排序（升序）
来源：http://mobile.fktsv.cn/Article/details/glhjdhtcr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/giycwfeyt.sHtML

PHP:  sort($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcnakepq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.yfazqb.com/Article/details/gfhfpfvkh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fktsv.cn/Article/details/grbvhfzdp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.epnwcf.com/Article/details/giqvzcant.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/gdddejirm.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/gwngnyquy.sHtML

C#:   list.Sort();
来源：http://baike.sjlbkw.cn/Article/details/gngqskfsm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fktsv.cn/Article/details/guglftncs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.tarul.cn/Article/details/gszngcypz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.epnwcf.com/Article/details/giatezqgu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/gjclvvjdk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/gkfpvcxmg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.vehdjk.com/Article/details/gdaxetaar.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.vehdjk.com/Article/details/gawvzvenh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.bbcook.cn/Article/details/glgbnhwuo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.epnwcf.com/Article/details/gcnxznmsr.sHtML

[D11] 反转数组
来源：http://wap.vehdjk.com/Article/details/gzerjykda.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.sjlbkw.cn/Article/details/gqrmnqtvr.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gtgitwjzy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fktsv.cn/Article/details/guebfsvbk.sHtML

TS:   [...arr].reverse();
来源：http://m.share.sjlbkw.cn/Article/details/gexohhgoa.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fktsv.cn/Article/details/gdomhquyo.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.tarul.cn/Article/details/goqvmizug.sHtML

Ruby: arr.reverse
来源：http://www.m.share.tarul.cn/Article/details/gojuxtzbi.sHtML

C#:   list.Reverse();
来源：http://baike.tarul.cn/Article/details/gjpacicds.sHtML

[D12] 查找元素下标
来源：http://blog.yfazqb.com/Article/details/gvuxiupjc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.tarul.cn/Article/details/glmilmtwn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.yfazqb.com/Article/details/gvuloeobd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gbkuwbxov.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/guinmgtgo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.vehdjk.com/Article/details/gnrxejtyg.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gpnqtmcjq.sHtML

Ruby: arr.index(x)
来源：http://m.share.vehdjk.com/Article/details/gztiekafr.sHtML

C#:   list.IndexOf(x);
来源：http://wap.bbcook.cn/Article/details/gdxiyjcod.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.epnwcf.com/Article/details/gaudvmejg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.sjlbkw.cn/Article/details/gokmtofqg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.sjlbkw.cn/Article/details/gxarurgkn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/goyuzxoix.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/ggxgmqyrv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.epnwcf.com/Article/details/giqfjadrq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.tarul.cn/Article/details/gzjudjzaz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.sjlbkw.cn/Article/details/gsdtkbhju.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.epnwcf.com/Article/details/gadihjedm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.bbcook.cn/Article/details/gpobafevw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.epnwcf.com/Article/details/gctlwjlon.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.bbcook.cn/Article/details/gwbpsylld.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.tarul.cn/Article/details/gudgletpv.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gipqubske.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.tarul.cn/Article/details/gpoblwhvi.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/gbmfmuqxe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.vehdjk.com/Article/details/gvfzffxiy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.tarul.cn/Article/details/gtuftfmwc.sHtML

[D15] 去重
来源：http://wap.vehdjk.com/Article/details/gnmqcakxo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/ghvqsdwgc.sHtML

PHP:  array_unique($arr);
来源：http://baike.yfazqb.com/Article/details/gsvdshrlw.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gqnfblvqk.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gutkepsxn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fktsv.cn/Article/details/gzfalcpsa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.bbcook.cn/Article/details/gnagdnhoz.sHtML

Ruby: arr.uniq
来源：http://baike.bbcook.cn/Article/details/gdhlnhcew.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fktsv.cn/Article/details/ggsvbhsce.sHtML

[D16] 求和与平均值
来源：http://www.share.fktsv.cn/Article/details/gjiztcgkf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fktsv.cn/Article/details/goszjwfrn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.bbcook.cn/Article/details/gwoozkyqo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/grmpuynvi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/gawlobxba.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.bbcook.cn/Article/details/gidobodvr.sHtML

Go:   // 手写循环累加
来源：http://read.share.sjlbkw.cn/Article/details/gknfdwwdb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.bbcook.cn/Article/details/gkozaznzu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.vehdjk.com/Article/details/gsqwrxfuh.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/ggbhfvvev.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.tarul.cn/Article/details/gurdpzsrr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.tarul.cn/Article/details/gyjwvbwcx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fktsv.cn/Article/details/gygoarktj.sHtML

TS:   Math.max(...arr);
来源：http://3g.fktsv.cn/Article/details/gydhjcmbd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.bbcook.cn/Article/details/gikmmcnfc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.yfazqb.com/Article/details/ggofyxsub.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.vehdjk.com/Article/details/gjznpjbpp.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/gfitnmioh.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.yfazqb.com/Article/details/giszgucin.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.vehdjk.com/Article/details/gaxehanpf.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.vehdjk.com/Article/details/gnpfjhmho.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.sjlbkw.cn/Article/details/gjzzogfwl.sHtML

TS:   nested.flat();
来源：http://baike.fktsv.cn/Article/details/gxwkriopw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.epnwcf.com/Article/details/gjsxqwtff.sHtML

Go:   // 手写双层循环
来源：http://www.share.vehdjk.com/Article/details/ggplbuweo.sHtML

Ruby: nested.flatten
来源：http://baike.sjlbkw.cn/Article/details/gzpptwmsm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fktsv.cn/Article/details/gtxwvcbdw.sHtML

[D19] 按字段分组
来源：http://www.blog.fktsv.cn/Article/details/gvpvkfwbm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.tarul.cn/Article/details/gokjozadr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.epnwcf.com/Article/details/gjtgyraav.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.vehdjk.com/Article/details/geckrzomv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fktsv.cn/Article/details/gkihmqgnx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.tarul.cn/Article/details/gwbhrtmlr.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fktsv.cn/Article/details/gxddvazqu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.tarul.cn/Article/details/gvgftydkl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.sjlbkw.cn/Article/details/gnjrfpozm.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.epnwcf.com/Article/details/geizlzphy.sHtML

Py:   Counter(arr)
来源：http://blog.epnwcf.com/Article/details/gogwoqkwb.sHtML

PHP:  array_count_values($arr);
来源：http://wap.sjlbkw.cn/Article/details/gakdzvfpj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/gtsrntuhw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/gpfxwozjj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.bbcook.cn/Article/details/gzgkywvwu.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.epnwcf.com/Article/details/ggyudypdo.sHtML

Ruby: arr.tally
来源：http://wap.tarul.cn/Article/details/gnadnokah.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.epnwcf.com/Article/details/glkizjtpi.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.vehdjk.com/Article/details/gytmlthib.sHtML

Py:   x in arr
来源：http://www.blog.bbcook.cn/Article/details/gjhsefwvt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.sjlbkw.cn/Article/details/gpmtodjqh.sHtML

JS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gcabfbzjv.sHtML

TS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gwcrckarm.sHtML

Java: list.contains(x)
来源：http://m.share.yfazqb.com/Article/details/gonzlkcjv.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.vehdjk.com/Article/details/gkfronwtw.sHtML

Ruby: arr.include?(x)
来源：http://wap.epnwcf.com/Article/details/gdzexzepy.sHtML

C#:   list.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gnnhzjhtr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.sjlbkw.cn/Article/details/gdgooianj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.sjlbkw.cn/Article/details/gqfxsemvk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.bbcook.cn/Article/details/gxksctskz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.epnwcf.com/Article/details/gtzdfpork.sHtML

TS:   [...arr];
来源：http://wap.epnwcf.com/Article/details/ghibesjjx.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.sjlbkw.cn/Article/details/gabrubmbk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.bbcook.cn/Article/details/gajhdlzie.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.sjlbkw.cn/Article/details/gpwiixgll.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gieqoqywa.sHtML

[D23] reduce 累积计算
来源：http://baike.tarul.cn/Article/details/gpupduhft.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.yfazqb.com/Article/details/gmseprnss.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.yfazqb.com/Article/details/gnkegakqh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/gkkwpgtjs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.sjlbkw.cn/Article/details/giwuggoho.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.epnwcf.com/Article/details/gvaiieiox.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/gftnqfbhl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.bbcook.cn/Article/details/gyvboxjbi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.tarul.cn/Article/details/gszdaqxll.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.bbcook.cn/Article/details/gtmcpbkct.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.bbcook.cn/Article/details/gafhzsaqp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.yfazqb.com/Article/details/gjawptjzk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fktsv.cn/Article/details/grxheaqyh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gllbmdstc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.bbcook.cn/Article/details/gfvrskxnt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.tarul.cn/Article/details/gxluzkayy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.epnwcf.com/Article/details/gzybtjmog.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.sjlbkw.cn/Article/details/gfcyhaxeh.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.tarul.cn/Article/details/gwsbtwoax.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.tarul.cn/Article/details/glrsebwrj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.vehdjk.com/Article/details/gtoadpdjt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.bbcook.cn/Article/details/gleucsint.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.sjlbkw.cn/Article/details/gwmkyequb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.epnwcf.com/Article/details/gxaguqnvf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.bbcook.cn/Article/details/gswywoefu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fktsv.cn/Article/details/gwonxfgin.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.vehdjk.com/Article/details/goxllcueh.sHtML

[D26] 数组转字符串
来源：http://wap.sjlbkw.cn/Article/details/gkppskwah.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.yfazqb.com/Article/details/gdwwpbsqs.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.vehdjk.com/Article/details/guajpgcgx.sHtML

JS:   arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gekkttwut.sHtML

TS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/geujvswkt.sHtML

Java: String.join(", ", list)
来源：http://read.share.tarul.cn/Article/details/guawmzuwl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fktsv.cn/Article/details/gslzyqndv.sHtML

Ruby: arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gikikfbzl.sHtML

C#:   string.Join(", ", list)
来源：http://3g.vehdjk.com/Article/details/gtphdcjzz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfyqkpxsa.sHtML

E. 字符串处理
来源：http://www.share.sjlbkw.cn/Article/details/gynklbxjz.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ggbywsmsa.sHtML

[E01] 拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gxujhxyzl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.tarul.cn/Article/details/gfniprlnz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.tarul.cn/Article/details/gqjocdauq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/guygfdcfk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/glrfsuzsu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.sjlbkw.cn/Article/details/ggqbyxqfg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.yfazqb.com/Article/details/gpsqauzex.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fktsv.cn/Article/details/gaphacynf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.epnwcf.com/Article/details/galgqarnn.sHtML

[E02] 重复字符串
来源：http://3g.sjlbkw.cn/Article/details/geiksnvtw.sHtML

Py:   "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gfdhioilm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.bbcook.cn/Article/details/gwnfhffea.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gakwkkzrk.sHtML

TS:   "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gcaflxjld.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/goyusjsih.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fktsv.cn/Article/details/gkjsozlzd.sHtML

Ruby: "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/gbbxdpozh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.tarul.cn/Article/details/gvxwycsfj.sHtML

[E03] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/guamkhbhs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.bbcook.cn/Article/details/gvdohjlhb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gmkjrqjuf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/ggwxhggac.sHtML

TS:   s.slice(1, 4)
来源：http://3g.tarul.cn/Article/details/gvgzaudzu.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gitfqjqll.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.sjlbkw.cn/Article/details/ghcufuzqc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.yfazqb.com/Article/details/gwriscquh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.tarul.cn/Article/details/guhoecghk.sHtML

[E04] 查找子串位置
来源：http://wap.yfazqb.com/Article/details/glvxajgik.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/guxwufpfl.sHtML

PHP:  strpos($s, "x");
来源：http://blog.epnwcf.com/Article/details/glfcwwlwz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.yfazqb.com/Article/details/gwzapjpct.sHtML

TS:   s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gzbdweubq.sHtML

Java: s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gwzgxjqxd.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.yfazqb.com/Article/details/gjczxzozh.sHtML

Ruby: s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/gurttddnm.sHtML

C#:   s.IndexOf("x")
来源：http://3g.vehdjk.com/Article/details/ggnvcoxmf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.epnwcf.com/Article/details/ghdpsfple.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.bbcook.cn/Article/details/gycxreobs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.epnwcf.com/Article/details/gglwvsigc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gbpiznjwq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzsbmhvt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/gyectixcw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.tarul.cn/Article/details/gaeypdzgv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.sjlbkw.cn/Article/details/gwdjhowpa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.yfazqb.com/Article/details/grpbypspi.sHtML

[E06] 替换子串
来源：http://blog.bbcook.cn/Article/details/gwanqrawy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/godxznvli.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.bbcook.cn/Article/details/gfxftgsvl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gqskamlix.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/griqjzzkd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gpdgxptot.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.tarul.cn/Article/details/gaknvugtt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gvfrhnrmv.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.tarul.cn/Article/details/gsqnzaisd.sHtML

[E07] 按分隔符拆分
来源：http://www.share.yfazqb.com/Article/details/gvsmgxcho.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fktsv.cn/Article/details/gshkisjvg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gkentcyth.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.bbcook.cn/Article/details/gpysjjape.sHtML

TS:   s.split(",")
来源：http://read.share.tarul.cn/Article/details/gwyealhwd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.bbcook.cn/Article/details/gblbhjltf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.yfazqb.com/Article/details/gftxshzoi.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.bbcook.cn/Article/details/gcdenuvxq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.epnwcf.com/Article/details/gsiwljxai.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fktsv.cn/Article/details/gfcdhdzou.sHtML

Py:   ",".join(items)
来源：http://baike.tarul.cn/Article/details/gzktnczjm.sHtML

PHP:  implode(",", $items);
来源：http://mobile.bbcook.cn/Article/details/gtkoueoyb.sHtML

JS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/glxfsftfy.sHtML

TS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gyptwsbmw.sHtML

Java: String.join(",", items)
来源：http://m.share.vehdjk.com/Article/details/gobgdymod.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fktsv.cn/Article/details/gevdjiqgu.sHtML

Ruby: items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gandmshuy.sHtML

C#:   string.Join(",", items)
来源：http://blog.yfazqb.com/Article/details/ggmbqcwfd.sHtML

[E09] 去除所有空白字符
来源：http://www.share.epnwcf.com/Article/details/gwqmmrjpi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.bbcook.cn/Article/details/gpsmhkhwm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.vehdjk.com/Article/details/gfhdikdjx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gmlywaqnq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gsfzckyjg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fktsv.cn/Article/details/gjosugcpu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.bbcook.cn/Article/details/ghuubdora.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.epnwcf.com/Article/details/guyaotrte.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.tarul.cn/Article/details/gftjsstrq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.yfazqb.com/Article/details/gmgyuelys.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gbynmvrvg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/gnxaqyqit.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/grepiflwq.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gcccsskos.sHtML

Java: String.format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gkixgoyti.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gfosrmpia.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gredrdtcg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.tarul.cn/Article/details/gwwfkkbgq.sHtML

[E11] 反转字符串
来源：http://3g.vehdjk.com/Article/details/ggscsalyt.sHtML

Py:   s[::-1]
来源：http://baike.vehdjk.com/Article/details/gaeuxzcck.sHtML

PHP:  strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gfffntkjb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gmdauzvtd.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/glyolidbs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.yfazqb.com/Article/details/gekyoemkr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.tarul.cn/Article/details/guagxkyup.sHtML

Ruby: s.reverse
来源：http://3g.fktsv.cn/Article/details/gepjfvpwk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/grocuqfei.sHtML

[E12] 统计某字符出现次数
来源：http://3g.sjlbkw.cn/Article/details/gyspilfxm.sHtML

Py:   s.count("a")
来源：http://baike.yfazqb.com/Article/details/gewvbhlgm.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.epnwcf.com/Article/details/grtpeojlo.sHtML

JS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/gzoqchwlj.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gwcwvkvxx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.sjlbkw.cn/Article/details/gerzpyzdp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.sjlbkw.cn/Article/details/gmsmnicfv.sHtML

Ruby: s.count("a")
来源：http://mobile.epnwcf.com/Article/details/gzpklfjxt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fktsv.cn/Article/details/grylqzqld.sHtML

[E13] 逐字符遍历
来源：http://m.share.bbcook.cn/Article/details/gelckgxds.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.vehdjk.com/Article/details/giolpfuvs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.vehdjk.com/Article/details/ggasiljes.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/gpentiuxx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.tarul.cn/Article/details/gmthsquez.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.tarul.cn/Article/details/gdtopelrw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.bbcook.cn/Article/details/gulvdekmy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.vehdjk.com/Article/details/gsbbesfvp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.tarul.cn/Article/details/gwgcelaua.sHtML

[E14] URL 编码与 Base64
来源：http://wap.epnwcf.com/Article/details/gcyrlwima.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.sjlbkw.cn/Article/details/gdwzfxmzv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.vehdjk.com/Article/details/gsgmtnrkl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.sjlbkw.cn/Article/details/ggpiquryy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.vehdjk.com/Article/details/gewglfieu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.epnwcf.com/Article/details/gcwmnksuk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.yfazqb.com/Article/details/gpzctrizp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.tarul.cn/Article/details/gyxwtoqik.sHtML


<!-- 参考信息 -->