代发 wailian999

TS:   arr.slice(1, 4);
来源：http://read.share.fktsv.cn/Article/details/gtkkthoyx.sHtML

Java: list.subList(1, 4);
来源：http://wap.bbcook.cn/Article/details/gcrxawnjz.sHtML

Go:   arr[1:4]
来源：http://wap.vehdjk.com/Article/details/gnrqywfvj.sHtML

Ruby: arr[1, 3]
来源：http://read.share.yfazqb.com/Article/details/gzxworgoi.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.epnwcf.com/Article/details/gidctqzai.sHtML

[D08] 合并两个数组
来源：http://read.share.yfazqb.com/Article/details/gecnqdwiz.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.bbcook.cn/Article/details/gqropbvlu.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.yfazqb.com/Article/details/gqmxkmvtu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.epnwcf.com/Article/details/gtywajdzf.sHtML

TS:   [...a, ...b];
来源：http://baike.fktsv.cn/Article/details/gwmvfjpau.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.yfazqb.com/Article/details/gsykzuvct.sHtML

Go:   append(a, b...)
来源：http://blog.bbcook.cn/Article/details/glqyiaffz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.vehdjk.com/Article/details/ghozptvxt.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gdkqarsgu.sHtML

[D09] 排序（升序）
来源：http://read.share.vehdjk.com/Article/details/grzdfkwuu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/gqitaiwgw.sHtML

PHP:  sort($arr);
来源：http://m.share.fktsv.cn/Article/details/gxdeqygir.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.bbcook.cn/Article/details/gpfckcaqm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.vehdjk.com/Article/details/gcegdssve.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.yfazqb.com/Article/details/gasagnyle.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/grdftpnku.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/gkvpvcqcx.sHtML

C#:   list.Sort();
来源：http://baike.bbcook.cn/Article/details/geiryufzh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.yfazqb.com/Article/details/ghtnkwnhl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.epnwcf.com/Article/details/gfgxssylw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.sjlbkw.cn/Article/details/gevzxogsv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.sjlbkw.cn/Article/details/gcqvanxjh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.epnwcf.com/Article/details/gffealuhu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.tarul.cn/Article/details/gsrcjhyap.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.vehdjk.com/Article/details/gvtotuotp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.bbcook.cn/Article/details/gbihnmllx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.bbcook.cn/Article/details/gbzkxvvfd.sHtML

[D11] 反转数组
来源：http://wap.tarul.cn/Article/details/gybohumat.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fktsv.cn/Article/details/gzwfumupq.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fktsv.cn/Article/details/gexgpmhyo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fktsv.cn/Article/details/gigngqvum.sHtML

TS:   [...arr].reverse();
来源：http://www.share.tarul.cn/Article/details/gbamrwfpb.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.yfazqb.com/Article/details/gfzkzgspu.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.yfazqb.com/Article/details/glnrcbbpf.sHtML

Ruby: arr.reverse
来源：http://m.share.epnwcf.com/Article/details/ggyutegha.sHtML

C#:   list.Reverse();
来源：http://wap.tarul.cn/Article/details/gzjzmrvtw.sHtML

[D12] 查找元素下标
来源：http://m.share.bbcook.cn/Article/details/guynjzczf.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.tarul.cn/Article/details/gekgowcie.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.tarul.cn/Article/details/gehxmrviv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gygjlhfku.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/gdbkzdbrm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.yfazqb.com/Article/details/gwizrbnwi.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.bbcook.cn/Article/details/gnvizudbm.sHtML

Ruby: arr.index(x)
来源：http://baike.epnwcf.com/Article/details/gqwvrvjmx.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.tarul.cn/Article/details/gmazsayxa.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.epnwcf.com/Article/details/gqkqblzoi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.tarul.cn/Article/details/gbtdxnpoc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.sjlbkw.cn/Article/details/guzwzdrfi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/gmlhznymq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gwcpsseiw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.vehdjk.com/Article/details/gbswdbbmf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.vehdjk.com/Article/details/gsqfuzhiy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.yfazqb.com/Article/details/ggnlhwvak.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.epnwcf.com/Article/details/geoyjahkd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/ginymvzpx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.bbcook.cn/Article/details/gcqfqlkmt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fktsv.cn/Article/details/garjookgq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gkkbkgfqz.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/glokiwshs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.bbcook.cn/Article/details/grhqoogkf.sHtML

Go:   // 手写循环
来源：http://baike.yfazqb.com/Article/details/gxjabpgvk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gtjvnswew.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.epnwcf.com/Article/details/glixhxgvd.sHtML

[D15] 去重
来源：http://www.share.tarul.cn/Article/details/gmpfupsuy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fktsv.cn/Article/details/gaobavbtn.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.bbcook.cn/Article/details/gdtdeujyk.sHtML

JS:   [...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/grmirpxgv.sHtML

TS:   [...new Set(arr)]
来源：http://3g.yfazqb.com/Article/details/gxfbpouop.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fktsv.cn/Article/details/gspwwxbfu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.tarul.cn/Article/details/ggvlptpjc.sHtML

Ruby: arr.uniq
来源：http://www.share.fktsv.cn/Article/details/gpiqiyyqk.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.yfazqb.com/Article/details/gpgrlopiz.sHtML

[D16] 求和与平均值
来源：http://baike.yfazqb.com/Article/details/gdcnbzryt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.vehdjk.com/Article/details/ghkkcjbzf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/giatkubnd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/gchfarxjd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/gredwonen.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.yfazqb.com/Article/details/gvhlbcabc.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.epnwcf.com/Article/details/gbrwjtfxn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.vehdjk.com/Article/details/gixvyaufr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.yfazqb.com/Article/details/gfwyazbpn.sHtML

[D17] 最大值与最小值
来源：http://mobile.fktsv.cn/Article/details/gcmxyiegf.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.tarul.cn/Article/details/gkqmdzckd.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.bbcook.cn/Article/details/gcnfadklz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fktsv.cn/Article/details/gjmtfmlsj.sHtML

TS:   Math.max(...arr);
来源：http://wap.sjlbkw.cn/Article/details/gawolwzly.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.epnwcf.com/Article/details/gaauqioqk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.bbcook.cn/Article/details/gbrodhwcb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fktsv.cn/Article/details/ghyonxaoq.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.yfazqb.com/Article/details/gubhbmbbk.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fktsv.cn/Article/details/gpdbvjnlq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fktsv.cn/Article/details/gljdtapht.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.sjlbkw.cn/Article/details/gaelwekty.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.yfazqb.com/Article/details/gfrsmdtrg.sHtML

TS:   nested.flat();
来源：http://www.m.share.yfazqb.com/Article/details/guokbfqqg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/glgyllgum.sHtML

Go:   // 手写双层循环
来源：http://blog.fktsv.cn/Article/details/gpgyuubon.sHtML

Ruby: nested.flatten
来源：http://baike.epnwcf.com/Article/details/gszbhwijk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.bbcook.cn/Article/details/gyquhszaq.sHtML

[D19] 按字段分组
来源：http://wap.bbcook.cn/Article/details/gubrmclaw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.sjlbkw.cn/Article/details/giaymllcg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.tarul.cn/Article/details/gcmclcroz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.tarul.cn/Article/details/galwelgpt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gzqydlljo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.yfazqb.com/Article/details/goaedcozv.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.tarul.cn/Article/details/gnlevzeyp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.sjlbkw.cn/Article/details/ggayzcrjq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fktsv.cn/Article/details/gojzjeiyx.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.yfazqb.com/Article/details/gvhbghmde.sHtML

Py:   Counter(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gbxvsffwf.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.epnwcf.com/Article/details/gtyflfvqh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gadrkhquf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/glfaqbjkr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.sjlbkw.cn/Article/details/gbhvxeuvn.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.vehdjk.com/Article/details/gohjxefbo.sHtML

Ruby: arr.tally
来源：http://blog.bbcook.cn/Article/details/gggdjhntf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.epnwcf.com/Article/details/gknwlnpll.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.tarul.cn/Article/details/gtkshwrap.sHtML

Py:   x in arr
来源：http://read.share.bbcook.cn/Article/details/gmjaaxcua.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.yfazqb.com/Article/details/gkpzebmpz.sHtML

JS:   arr.includes(x)
来源：http://m.share.vehdjk.com/Article/details/gjyiqoqrr.sHtML

TS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gobedrjwt.sHtML

Java: list.contains(x)
来源：http://m.share.epnwcf.com/Article/details/gcvdkwnse.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.vehdjk.com/Article/details/gfccthawj.sHtML

Ruby: arr.include?(x)
来源：http://baike.epnwcf.com/Article/details/gcndwzfdh.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gveevirku.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.sjlbkw.cn/Article/details/gngosxjhi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.yfazqb.com/Article/details/gfjvocvle.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.yfazqb.com/Article/details/girjuplky.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fktsv.cn/Article/details/goixnzzls.sHtML

TS:   [...arr];
来源：http://m.share.epnwcf.com/Article/details/gszudvfgl.sHtML

Java: new ArrayList<>(list);
来源：http://wap.vehdjk.com/Article/details/glcuwomow.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.vehdjk.com/Article/details/gvvlgmtdm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.yfazqb.com/Article/details/goksebjha.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fktsv.cn/Article/details/gcezchdft.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.sjlbkw.cn/Article/details/gejycfsib.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fktsv.cn/Article/details/gawoxtgxl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.vehdjk.com/Article/details/grqjntmzj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gpalbasrz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/gckgzvqeu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.sjlbkw.cn/Article/details/gnvdxyxnr.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gkodsnajq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.sjlbkw.cn/Article/details/gtwzjmtdt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.sjlbkw.cn/Article/details/gebujurmh.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.epnwcf.com/Article/details/gekazbdws.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.yfazqb.com/Article/details/gqltffxcx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fktsv.cn/Article/details/gosrmycut.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.epnwcf.com/Article/details/gmqfunesf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gteuhvrbv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fktsv.cn/Article/details/gsqlltkmp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.vehdjk.com/Article/details/glhysfmlv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fktsv.cn/Article/details/gdjromiya.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.epnwcf.com/Article/details/gopveyygm.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.vehdjk.com/Article/details/gvxzdkltv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.sjlbkw.cn/Article/details/gesorbftq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.bbcook.cn/Article/details/glncbxcks.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.bbcook.cn/Article/details/guqrjrkbq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.epnwcf.com/Article/details/gmwylnjlu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fktsv.cn/Article/details/gzfouwlgr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gmooyfeiy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.vehdjk.com/Article/details/gjrmdoote.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.yfazqb.com/Article/details/giisvfruu.sHtML

[D26] 数组转字符串
来源：http://baike.fktsv.cn/Article/details/ghujyewno.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.bbcook.cn/Article/details/gbtovhrrm.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.epnwcf.com/Article/details/grhiunfsy.sHtML

JS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gmanyxcfb.sHtML

TS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gygadvclc.sHtML

Java: String.join(", ", list)
来源：http://mobile.bbcook.cn/Article/details/gxuxfefjz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.tarul.cn/Article/details/gmxduypud.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gyzxbcaki.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gxzkghbce.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gickxyhwx.sHtML

E. 字符串处理
来源：http://baike.vehdjk.com/Article/details/giixztkyx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gcouvnjul.sHtML

[E01] 拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gpthlbwwj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.epnwcf.com/Article/details/gitybzojp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.bbcook.cn/Article/details/gtbsqnybb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/gzdqhxdcx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gbikveivk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.bbcook.cn/Article/details/gzurnshym.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fktsv.cn/Article/details/gmkwpidvb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.sjlbkw.cn/Article/details/gcuqpmjlf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gxsmyjxcx.sHtML

[E02] 重复字符串
来源：http://wap.bbcook.cn/Article/details/gcoefzmsv.sHtML

Py:   "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gfujbwndh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.bbcook.cn/Article/details/gvaiccqvg.sHtML

JS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gakagerua.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/ghghfxsqp.sHtML

Java: "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gsxxxvlvo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fktsv.cn/Article/details/ghayykmgd.sHtML

Ruby: "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gvctnltje.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.vehdjk.com/Article/details/gmmswqorh.sHtML

[E03] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/ghzqesdmv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.bbcook.cn/Article/details/ggswypnvl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/guejenujg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gnjjryjrq.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gnmomgxdh.sHtML

Java: s.substring(1, 4)
来源：http://baike.bbcook.cn/Article/details/giimsqshe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gzcovtefs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.vehdjk.com/Article/details/gewdpygnb.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.tarul.cn/Article/details/gniewweaa.sHtML

[E04] 查找子串位置
来源：http://www.share.sjlbkw.cn/Article/details/gkbigcyao.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.tarul.cn/Article/details/gkcyuzxda.sHtML

PHP:  strpos($s, "x");
来源：http://blog.epnwcf.com/Article/details/gzxhoyyen.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.epnwcf.com/Article/details/gmnhklyfy.sHtML

TS:   s.indexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/gyzdkkjav.sHtML

Java: s.indexOf("x")
来源：http://baike.tarul.cn/Article/details/gtqcjsbzi.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fktsv.cn/Article/details/grmdxrroy.sHtML

Ruby: s.index("x")
来源：http://3g.tarul.cn/Article/details/gqjjrqapa.sHtML

C#:   s.IndexOf("x")
来源：http://blog.vehdjk.com/Article/details/gvwglftmw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.yfazqb.com/Article/details/gwysholny.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.tarul.cn/Article/details/gmenhznqy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.tarul.cn/Article/details/gwjtfhxzi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gaigywusk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fktsv.cn/Article/details/gylpywfjn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/gthawvsfd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.tarul.cn/Article/details/gbfumfchb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fktsv.cn/Article/details/gnxyyinnc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gfuimkvir.sHtML

[E06] 替换子串
来源：http://www.m.share.tarul.cn/Article/details/ggwrmygbf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/gjvlgvebu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gfmnglbql.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gsitkzboh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gvnjvgwjr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gwncdxais.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fktsv.cn/Article/details/gjccobpzl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fktsv.cn/Article/details/gewjxwqgr.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.epnwcf.com/Article/details/gpsqodjdj.sHtML

[E07] 按分隔符拆分
来源：http://baike.epnwcf.com/Article/details/gqaplkdey.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.vehdjk.com/Article/details/gmyknjkcf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gygjfsaam.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.tarul.cn/Article/details/gpzisdlow.sHtML

TS:   s.split(",")
来源：http://mobile.epnwcf.com/Article/details/gwufogqse.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fktsv.cn/Article/details/gnrdmqojh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdyzakez.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.bbcook.cn/Article/details/guxfybcok.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.sjlbkw.cn/Article/details/gxdzddrss.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fktsv.cn/Article/details/gropzquwu.sHtML

Py:   ",".join(items)
来源：http://baike.bbcook.cn/Article/details/grwtvsjtq.sHtML

PHP:  implode(",", $items);
来源：http://www.share.sjlbkw.cn/Article/details/gyrsrcrga.sHtML

JS:   items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gnfglwkep.sHtML

TS:   items.join(",")
来源：http://www.share.epnwcf.com/Article/details/gdaeoocwn.sHtML

Java: String.join(",", items)
来源：http://3g.bbcook.cn/Article/details/grdqyirsr.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.vehdjk.com/Article/details/gfnkyhrvc.sHtML

Ruby: items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gbfeyfafr.sHtML

C#:   string.Join(",", items)
来源：http://wap.epnwcf.com/Article/details/gygaeuise.sHtML

[E09] 去除所有空白字符
来源：http://3g.vehdjk.com/Article/details/gosxvblix.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.epnwcf.com/Article/details/grsrwkstt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.bbcook.cn/Article/details/gurwviawc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/gsigfzyiq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.sjlbkw.cn/Article/details/glklllszv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gtlexjavr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.sjlbkw.cn/Article/details/gndkaykob.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.bbcook.cn/Article/details/gtwzbpehf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.bbcook.cn/Article/details/gylfxnotb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.epnwcf.com/Article/details/gkmbwavbp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gqhuplvoi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.sjlbkw.cn/Article/details/glglktrky.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/goipqhbsj.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gnmlevzjm.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/geqbptial.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gprgtuekz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/ghjsydost.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/gjolyrtzr.sHtML

[E11] 反转字符串
来源：http://baike.yfazqb.com/Article/details/gfsslgjix.sHtML

Py:   s[::-1]
来源：http://www.share.tarul.cn/Article/details/gvndylzfb.sHtML

PHP:  strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gxzrxuxlb.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gviseoral.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gipvifluo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.tarul.cn/Article/details/gkgwwmpht.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.vehdjk.com/Article/details/ggisnepri.sHtML

Ruby: s.reverse
来源：http://www.share.epnwcf.com/Article/details/gcopiapyz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/gsdyunzbx.sHtML

[E12] 统计某字符出现次数
来源：http://3g.tarul.cn/Article/details/gkkedfpkm.sHtML

Py:   s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gbyjczlwl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.tarul.cn/Article/details/gnrvjexgt.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gilfjxfzv.sHtML

TS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gxjkacego.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.yfazqb.com/Article/details/gbcdlttlf.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fktsv.cn/Article/details/gmrdjguyh.sHtML

Ruby: s.count("a")
来源：http://wap.yfazqb.com/Article/details/gmbhrnelr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.epnwcf.com/Article/details/geyxryodt.sHtML

[E13] 逐字符遍历
来源：http://wap.bbcook.cn/Article/details/glbpbqmtv.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.tarul.cn/Article/details/gcfvxigqk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.yfazqb.com/Article/details/gsyolidry.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gwymyllzy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/guelpzwsy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/grlefrorl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.sjlbkw.cn/Article/details/gebrqcjqh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.bbcook.cn/Article/details/geqrynvyh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gjtjuhzyz.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.epnwcf.com/Article/details/gwgmykzav.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.yfazqb.com/Article/details/gghjlgfnc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fktsv.cn/Article/details/gvalaivcn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fktsv.cn/Article/details/gyvooywic.sHtML


<!-- 参考信息 -->