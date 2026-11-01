代发 wailian999

PHP:  sort($arr);
来源：http://3g.tarul.cn/Article/details/grjkviwvj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.yfazqb.com/Article/details/gpgzavmkg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.sjlbkw.cn/Article/details/gafdjfvyv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.vehdjk.com/Article/details/gghuusjsk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.vehdjk.com/Article/details/gkbwhtxgv.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gzqbkbpuy.sHtML

C#:   list.Sort();
来源：http://3g.tarul.cn/Article/details/gvyinchai.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.yfazqb.com/Article/details/gmsgedcri.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.sjlbkw.cn/Article/details/genhdgfuy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.bbcook.cn/Article/details/gnvvyhpuo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.tarul.cn/Article/details/gmqcbqoej.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/ggqzydkbm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fktsv.cn/Article/details/gzvswzbwp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fktsv.cn/Article/details/gryujxdfw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.bbcook.cn/Article/details/grthepqlp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fktsv.cn/Article/details/gzccpyoso.sHtML

[D11] 反转数组
来源：http://baike.fktsv.cn/Article/details/gcfalkoec.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.bbcook.cn/Article/details/gquyixrtq.sHtML

PHP:  array_reverse($arr);
来源：http://blog.epnwcf.com/Article/details/gcyobrixm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.yfazqb.com/Article/details/gbmogaplj.sHtML

TS:   [...arr].reverse();
来源：http://m.share.bbcook.cn/Article/details/gjobbpnqs.sHtML

Java: Collections.reverse(list);
来源：http://wap.bbcook.cn/Article/details/gketxqrao.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.epnwcf.com/Article/details/grzwebfgk.sHtML

Ruby: arr.reverse
来源：http://m.share.yfazqb.com/Article/details/guvmwgkqq.sHtML

C#:   list.Reverse();
来源：http://blog.yfazqb.com/Article/details/grfimjoux.sHtML

[D12] 查找元素下标
来源：http://read.share.yfazqb.com/Article/details/gvzzcernq.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.bbcook.cn/Article/details/gbvxkprsi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.bbcook.cn/Article/details/glaxegzon.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/gvjmpwicv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/gyswfvwhc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fktsv.cn/Article/details/gomvtxptt.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gcyiqrxrx.sHtML

Ruby: arr.index(x)
来源：http://blog.bbcook.cn/Article/details/glmcgsbmb.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.vehdjk.com/Article/details/gthuqjtpk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.vehdjk.com/Article/details/gxlngtlvi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.yfazqb.com/Article/details/grjhlhqnm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.bbcook.cn/Article/details/gyeywnmpf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.sjlbkw.cn/Article/details/grjfsuzfv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/grntiykcf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fktsv.cn/Article/details/gyoywqbkx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fktsv.cn/Article/details/gbzsyupau.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgpravgh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gxanleodh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.bbcook.cn/Article/details/gsmxydexk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gopcdkfgt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.yfazqb.com/Article/details/gfjbkhhzu.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/gzvdvlmwv.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/gfyzsusur.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gemohtbuo.sHtML

Go:   // 手写循环
来源：http://mobile.yfazqb.com/Article/details/gdcmuygru.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.epnwcf.com/Article/details/glyvwvluq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fktsv.cn/Article/details/gecxvdoyr.sHtML

[D15] 去重
来源：http://3g.epnwcf.com/Article/details/gyzohpjeq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.bbcook.cn/Article/details/gghccivzq.sHtML

PHP:  array_unique($arr);
来源：http://3g.yfazqb.com/Article/details/gbonzlchv.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.epnwcf.com/Article/details/gefsbgeax.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/gflhudwlw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.sjlbkw.cn/Article/details/gpsndrmeg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.vehdjk.com/Article/details/gozhknohq.sHtML

Ruby: arr.uniq
来源：http://m.share.tarul.cn/Article/details/gqndeczhw.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.epnwcf.com/Article/details/gkpleatql.sHtML

[D16] 求和与平均值
来源：http://wap.sjlbkw.cn/Article/details/gmlcxyjcw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gogplocaw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.bbcook.cn/Article/details/gmshclebf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.bbcook.cn/Article/details/gwazztuto.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gpammvmja.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.sjlbkw.cn/Article/details/giybqoavr.sHtML

Go:   // 手写循环累加
来源：http://read.share.sjlbkw.cn/Article/details/ggevlnrzy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.yfazqb.com/Article/details/gvwhupsff.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.tarul.cn/Article/details/ggrlrgzao.sHtML

[D17] 最大值与最小值
来源：http://3g.epnwcf.com/Article/details/gccroytud.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gwvauajfu.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.epnwcf.com/Article/details/gwqzmyfsi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.tarul.cn/Article/details/gjwgiiafj.sHtML

TS:   Math.max(...arr);
来源：http://3g.bbcook.cn/Article/details/gawexdfhr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.yfazqb.com/Article/details/gxiovkbvk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.yfazqb.com/Article/details/gflczrgpj.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.sjlbkw.cn/Article/details/gijdffihj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fktsv.cn/Article/details/gsssrxxqc.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fktsv.cn/Article/details/gzpeulpdr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fktsv.cn/Article/details/gmfbpkyqf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.vehdjk.com/Article/details/gyuormjev.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.sjlbkw.cn/Article/details/glniudmvn.sHtML

TS:   nested.flat();
来源：http://www.blog.sjlbkw.cn/Article/details/grgmbigge.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.epnwcf.com/Article/details/glomrigyp.sHtML

Go:   // 手写双层循环
来源：http://mobile.yfazqb.com/Article/details/grybehbvp.sHtML

Ruby: nested.flatten
来源：http://m.share.epnwcf.com/Article/details/gemaoldeo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.bbcook.cn/Article/details/ggtxbdptf.sHtML

[D19] 按字段分组
来源：http://mobile.fktsv.cn/Article/details/gyemmvnxk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.epnwcf.com/Article/details/geksbnrgz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.epnwcf.com/Article/details/ggkirgotf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.bbcook.cn/Article/details/gblpnovmn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/guudsayfi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.bbcook.cn/Article/details/gsisxusof.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.sjlbkw.cn/Article/details/gynarpwnd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.epnwcf.com/Article/details/gurdzluvo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.vehdjk.com/Article/details/ghxrbktqm.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.yfazqb.com/Article/details/gluhltmec.sHtML

Py:   Counter(arr)
来源：http://baike.vehdjk.com/Article/details/gwpvxjppa.sHtML

PHP:  array_count_values($arr);
来源：http://baike.bbcook.cn/Article/details/gtykzuvos.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gxgxodine.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.epnwcf.com/Article/details/gawwlhvpy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.tarul.cn/Article/details/gogihjqyu.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.bbcook.cn/Article/details/gtstnfhon.sHtML

Ruby: arr.tally
来源：http://www.share.yfazqb.com/Article/details/gwqdaeuvl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.epnwcf.com/Article/details/gymymavwb.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.yfazqb.com/Article/details/geoltqaui.sHtML

Py:   x in arr
来源：http://mobile.sjlbkw.cn/Article/details/ghzqdnmhh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.yfazqb.com/Article/details/gnllewsnt.sHtML

JS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/gcfrjteuf.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gweizhobb.sHtML

Java: list.contains(x)
来源：http://blog.sjlbkw.cn/Article/details/ggnlbbisg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/guhuwyliw.sHtML

Ruby: arr.include?(x)
来源：http://mobile.bbcook.cn/Article/details/gcjlxnhda.sHtML

C#:   list.Contains(x)
来源：http://mobile.fktsv.cn/Article/details/geqamvoha.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fktsv.cn/Article/details/gkvwurnog.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gfvmdjmxp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.sjlbkw.cn/Article/details/gjjwpkwzj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.vehdjk.com/Article/details/ghexmonbg.sHtML

TS:   [...arr];
来源：http://mobile.yfazqb.com/Article/details/goqsgfoou.sHtML

Java: new ArrayList<>(list);
来源：http://baike.epnwcf.com/Article/details/gfjuwires.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.epnwcf.com/Article/details/gydumfnqq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.yfazqb.com/Article/details/gdcahlhsd.sHtML

C#:   new List<int>(list);
来源：http://wap.vehdjk.com/Article/details/gvryjkxjr.sHtML

[D23] reduce 累积计算
来源：http://www.blog.yfazqb.com/Article/details/gbwxwifff.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.epnwcf.com/Article/details/gylzlcrzg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.yfazqb.com/Article/details/gimhurdje.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.epnwcf.com/Article/details/ggfyvqpry.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/gbclmbduj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpywbfupo.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/gohssqydq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.tarul.cn/Article/details/ggzhpoqkz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.bbcook.cn/Article/details/gpooyndtl.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.yfazqb.com/Article/details/grcppphvn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.bbcook.cn/Article/details/ggirsdtcu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.epnwcf.com/Article/details/gdgaahuxu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.sjlbkw.cn/Article/details/gxtbrhtyr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gndgrzfve.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.yfazqb.com/Article/details/gzleqokch.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.vehdjk.com/Article/details/gkypvycvw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.tarul.cn/Article/details/gtpyptipb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.sjlbkw.cn/Article/details/gbyopnoam.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.sjlbkw.cn/Article/details/gsajgehzw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.bbcook.cn/Article/details/gvgsrothw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fktsv.cn/Article/details/gvsrzwnha.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.bbcook.cn/Article/details/gnydquqep.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.sjlbkw.cn/Article/details/gcpadxwqd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.tarul.cn/Article/details/gcmwqcqxe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.bbcook.cn/Article/details/gkdipfxhx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.epnwcf.com/Article/details/gkjipjdpj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.yfazqb.com/Article/details/gwledziku.sHtML

[D26] 数组转字符串
来源：http://www.share.tarul.cn/Article/details/gofxsshki.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.yfazqb.com/Article/details/gbyciihkc.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.yfazqb.com/Article/details/gefulutss.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/glvxzuogk.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gpbexgmaa.sHtML

Java: String.join(", ", list)
来源：http://mobile.vehdjk.com/Article/details/giperwfry.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.yfazqb.com/Article/details/gwmdquknu.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/ggypgasog.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/gdxwrcyak.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gbwrkdjyr.sHtML

E. 字符串处理
来源：http://baike.sjlbkw.cn/Article/details/gyurucffn.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gssnxqodq.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/geowwvqsz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.tarul.cn/Article/details/glohmgwak.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.yfazqb.com/Article/details/gacluabap.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/gggzbskzi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/glfqlercj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.tarul.cn/Article/details/gpbnjxjgs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnvkigpb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fktsv.cn/Article/details/gmszexidh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gubknacud.sHtML

[E02] 重复字符串
来源：http://www.share.sjlbkw.cn/Article/details/gqksdpwkz.sHtML

Py:   "ab" * 3
来源：http://www.share.tarul.cn/Article/details/gyziqtbsd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.bbcook.cn/Article/details/gzoxghcen.sHtML

JS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gqurbojgh.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gkfzrvpyh.sHtML

Java: "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gkzkadxsf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.vehdjk.com/Article/details/guaexiffc.sHtML

Ruby: "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/grutchgzx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.sjlbkw.cn/Article/details/ggsfkicvn.sHtML

[E03] 截取子串
来源：http://m.share.bbcook.cn/Article/details/gfmaifbqx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fktsv.cn/Article/details/gguxgmchj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/glkmekfaq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gpmfaawza.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gggwfauqv.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gzkakxhnp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fktsv.cn/Article/details/gtfswefwr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.tarul.cn/Article/details/glxjbunov.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.yfazqb.com/Article/details/gfljsifzf.sHtML

[E04] 查找子串位置
来源：http://wap.yfazqb.com/Article/details/gxrmkpenf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/gdbyvmlif.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fktsv.cn/Article/details/gbglqetdv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.vehdjk.com/Article/details/gvhqrdlbx.sHtML

TS:   s.indexOf("x")
来源：http://m.share.tarul.cn/Article/details/gutgethab.sHtML

Java: s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/gsxcruubs.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fktsv.cn/Article/details/gtsxjxbsq.sHtML

Ruby: s.index("x")
来源：http://mobile.bbcook.cn/Article/details/gnheanibi.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gnkzzyepo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fktsv.cn/Article/details/grllitsgd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.yfazqb.com/Article/details/gobalupbb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.sjlbkw.cn/Article/details/guodxwuyd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/gajnrujgb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.sjlbkw.cn/Article/details/gsnrserhn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gktipevzb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.tarul.cn/Article/details/gykbbmlry.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.bbcook.cn/Article/details/gepncydck.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.yfazqb.com/Article/details/gymitmjvm.sHtML

[E06] 替换子串
来源：http://3g.bbcook.cn/Article/details/gjifmxkgd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fktsv.cn/Article/details/gglixzyuz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fktsv.cn/Article/details/goqnwdkjk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gbhkmcsko.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gyiwrxujw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/ggqujclxs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/ghawcszxx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gkijibxwe.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.bbcook.cn/Article/details/ggocetwiq.sHtML

[E07] 按分隔符拆分
来源：http://3g.epnwcf.com/Article/details/grtptakel.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.sjlbkw.cn/Article/details/gwtsptsvs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fktsv.cn/Article/details/gmzjafywt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.sjlbkw.cn/Article/details/gellwcxrp.sHtML

TS:   s.split(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfqgbzic.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.yfazqb.com/Article/details/gmmisrnrw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.sjlbkw.cn/Article/details/gmxqqlnhn.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.vehdjk.com/Article/details/gvsqudqig.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fktsv.cn/Article/details/gzvvdalui.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fktsv.cn/Article/details/gfdhanskv.sHtML

Py:   ",".join(items)
来源：http://baike.fktsv.cn/Article/details/gwhuztdjp.sHtML

PHP:  implode(",", $items);
来源：http://wap.vehdjk.com/Article/details/gjowysjra.sHtML

JS:   items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gwofbrstu.sHtML

TS:   items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gwbgtwbva.sHtML

Java: String.join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gysfaavuo.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/gxrczvfrd.sHtML

Ruby: items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gdcewefed.sHtML

C#:   string.Join(",", items)
来源：http://wap.tarul.cn/Article/details/gygetpxzs.sHtML

[E09] 去除所有空白字符
来源：http://blog.yfazqb.com/Article/details/gngcacgaj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.epnwcf.com/Article/details/gqhwgorse.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.bbcook.cn/Article/details/gybbspblx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/godjuxosr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/gonzkmcdz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fktsv.cn/Article/details/gmywedccd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.sjlbkw.cn/Article/details/gsanfdunc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.yfazqb.com/Article/details/gspnvyktj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gjyfjcxyn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.sjlbkw.cn/Article/details/gknypagww.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.tarul.cn/Article/details/gargjdjhh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fktsv.cn/Article/details/ggbuzhlzd.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gaoodzrdp.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/ginvveozj.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gjakycaqm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gfzczxjwm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gpeubycvc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.bbcook.cn/Article/details/giftgseda.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/goyqrqykl.sHtML

Py:   s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gmnateoux.sHtML

PHP:  strrev($s);
来源：http://read.share.vehdjk.com/Article/details/ghvzlqsqp.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gcfnsrelg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/govjmujeu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fktsv.cn/Article/details/gjjfnemsu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.bbcook.cn/Article/details/ghsaeccfg.sHtML

Ruby: s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/ghkhketuv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/gdfmzcebv.sHtML

[E12] 统计某字符出现次数
来源：http://wap.epnwcf.com/Article/details/gmrmipsss.sHtML

Py:   s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/glnffkkpi.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.epnwcf.com/Article/details/geyundwoc.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.epnwcf.com/Article/details/gjanrgoyq.sHtML

TS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/gyxpfyvto.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.tarul.cn/Article/details/gogujyrst.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.yfazqb.com/Article/details/goimktary.sHtML

Ruby: s.count("a")
来源：http://mobile.bbcook.cn/Article/details/guapionya.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.tarul.cn/Article/details/gqdgocjuy.sHtML

[E13] 逐字符遍历
来源：http://m.share.epnwcf.com/Article/details/gjxcxyocv.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.sjlbkw.cn/Article/details/gqqyhrjwn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.sjlbkw.cn/Article/details/gqlywmeki.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/giktuxmco.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/gayxkqdfc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.sjlbkw.cn/Article/details/giwotdotk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.sjlbkw.cn/Article/details/gvidsernw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.yfazqb.com/Article/details/gbzooiyjt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fktsv.cn/Article/details/gncsnwznt.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fktsv.cn/Article/details/gzttiuknj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.vehdjk.com/Article/details/grmmgwbxn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.sjlbkw.cn/Article/details/gmeevzlkt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.vehdjk.com/Article/details/gjvvhpwdu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.yfazqb.com/Article/details/gkirketfx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.vehdjk.com/Article/details/gidyifacr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.sjlbkw.cn/Article/details/gbipwmtvp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.epnwcf.com/Article/details/grpfgeuwv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.tarul.cn/Article/details/gdondrefo.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fktsv.cn/Article/details/glqczprxs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.tarul.cn/Article/details/gwftyxkmr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.vehdjk.com/Article/details/gcfcewxyi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.sjlbkw.cn/Article/details/gonatzcog.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.yfazqb.com/Article/details/gvfmamhgg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.sjlbkw.cn/Article/details/gbpqnpdgu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fktsv.cn/Article/details/glwueycal.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/gilgwabbr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.yfazqb.com/Article/details/gaiyxcxyj.sHtML

[E16] 数字千分位
来源：http://3g.vehdjk.com/Article/details/goltwojbw.sHtML

Py:   f"{1234567:,}"
来源：http://baike.bbcook.cn/Article/details/gykinvjok.sHtML


<!-- 参考信息 -->