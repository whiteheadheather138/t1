代发 wailian999

TS:   [...arr].reverse();
来源：http://www.blog.bbcook.cn/Article/details/gqlckfrxl.sHtML

Java: Collections.reverse(list);
来源：http://wap.sjlbkw.cn/Article/details/gdjhyaqrf.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.sjlbkw.cn/Article/details/grmaqzzix.sHtML

Ruby: arr.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gqpbxtvfn.sHtML

C#:   list.Reverse();
来源：http://wap.tarul.cn/Article/details/gwoqmucim.sHtML

[D12] 查找元素下标
来源：http://www.m.share.epnwcf.com/Article/details/gmnqgvpya.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.yfazqb.com/Article/details/gjudzfkef.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gsdtideyh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.tarul.cn/Article/details/gbmiyzceb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gephiodys.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fktsv.cn/Article/details/gkdgatvvm.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gdrjhrudd.sHtML

Ruby: arr.index(x)
来源：http://baike.sjlbkw.cn/Article/details/guvmfjmur.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.yfazqb.com/Article/details/gsjrnjisv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.vehdjk.com/Article/details/gbpdsuktm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.tarul.cn/Article/details/gyylgfwba.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.tarul.cn/Article/details/gekwpwlqb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/glelcttpp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/gfbanlpnx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.vehdjk.com/Article/details/gusgfyjhg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.vehdjk.com/Article/details/ghdbmluum.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.tarul.cn/Article/details/gmbrzseaw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.vehdjk.com/Article/details/gdghhjwaa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.sjlbkw.cn/Article/details/gbowstreh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.bbcook.cn/Article/details/gnecologb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.tarul.cn/Article/details/gbgqjqdii.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gzvrxrkfu.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/gygiyqqek.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.tarul.cn/Article/details/gihnezpzg.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/gogebvqmq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gpgooquoo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gqqmlbphf.sHtML

[D15] 去重
来源：http://wap.fktsv.cn/Article/details/gjurujnvq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gpzkyjyda.sHtML

PHP:  array_unique($arr);
来源：http://wap.vehdjk.com/Article/details/guoqjxudo.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gzfmfwcxn.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gpctmxqhn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.tarul.cn/Article/details/gcvtczjku.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.tarul.cn/Article/details/gixaxtcyh.sHtML

Ruby: arr.uniq
来源：http://www.share.fktsv.cn/Article/details/gbwpiapjv.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.yfazqb.com/Article/details/gwartcqaz.sHtML

[D16] 求和与平均值
来源：http://read.share.bbcook.cn/Article/details/gctmclala.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.yfazqb.com/Article/details/gqybtxymp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.epnwcf.com/Article/details/gavxbueht.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/gbnvkukuu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gxmkmrcqd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.epnwcf.com/Article/details/gnndhuakv.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fktsv.cn/Article/details/grqzptjkw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.bbcook.cn/Article/details/gkppsfwua.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.tarul.cn/Article/details/gkahvdxuc.sHtML

[D17] 最大值与最小值
来源：http://m.share.vehdjk.com/Article/details/gmceteyff.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.epnwcf.com/Article/details/ghroevdse.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fktsv.cn/Article/details/gbjibqdxf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.yfazqb.com/Article/details/glsnytpjg.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fktsv.cn/Article/details/gfoukvzfg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.vehdjk.com/Article/details/gkcmovplu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fktsv.cn/Article/details/gawlrwpyr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fktsv.cn/Article/details/gadqwheqn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.sjlbkw.cn/Article/details/gykrbsryf.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.yfazqb.com/Article/details/grzonbgkk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.sjlbkw.cn/Article/details/ghtehqvfa.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.yfazqb.com/Article/details/gsxcyuclh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.bbcook.cn/Article/details/gmuvmsqov.sHtML

TS:   nested.flat();
来源：http://m.share.epnwcf.com/Article/details/gpnudjjyt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.yfazqb.com/Article/details/gfchlphay.sHtML

Go:   // 手写双层循环
来源：http://read.share.fktsv.cn/Article/details/gddxroeyi.sHtML

Ruby: nested.flatten
来源：http://blog.yfazqb.com/Article/details/gcdiklpnb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.tarul.cn/Article/details/gomkilqer.sHtML

[D19] 按字段分组
来源：http://3g.bbcook.cn/Article/details/giovcxhfe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.epnwcf.com/Article/details/glumalefz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.vehdjk.com/Article/details/gdlbpongm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.sjlbkw.cn/Article/details/glvhfngip.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.epnwcf.com/Article/details/gditinreg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.yfazqb.com/Article/details/gpnoublyu.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.yfazqb.com/Article/details/gdidxibak.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.yfazqb.com/Article/details/gqvyqhitz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.vehdjk.com/Article/details/gxjwjhydt.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.vehdjk.com/Article/details/gjtavlazi.sHtML

Py:   Counter(arr)
来源：http://blog.sjlbkw.cn/Article/details/gggxweyii.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gvajxjnnh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.vehdjk.com/Article/details/gqfbslwmp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.vehdjk.com/Article/details/gajafwqfj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.tarul.cn/Article/details/gxadhtqye.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.epnwcf.com/Article/details/gcwiaexka.sHtML

Ruby: arr.tally
来源：http://www.m.share.epnwcf.com/Article/details/grymcnyiq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.vehdjk.com/Article/details/gbblqrfga.sHtML

[D21] 判断是否包含某元素
来源：http://wap.sjlbkw.cn/Article/details/gmfgaxdoc.sHtML

Py:   x in arr
来源：http://baike.epnwcf.com/Article/details/gxqbqgvgs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fktsv.cn/Article/details/gqsbbanss.sHtML

JS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/grnyveqhp.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsurzcuxl.sHtML

Java: list.contains(x)
来源：http://mobile.epnwcf.com/Article/details/gzmkhveez.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gwmrdnszw.sHtML

Ruby: arr.include?(x)
来源：http://3g.vehdjk.com/Article/details/gkxflgovn.sHtML

C#:   list.Contains(x)
来源：http://read.share.fktsv.cn/Article/details/gmjeknwjn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.tarul.cn/Article/details/glrhylvsh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.epnwcf.com/Article/details/gmxodvypg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.vehdjk.com/Article/details/gmaqnpfqe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.vehdjk.com/Article/details/guzgvjmtf.sHtML

TS:   [...arr];
来源：http://blog.tarul.cn/Article/details/gkuscewir.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fktsv.cn/Article/details/gcttdmuyg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.yfazqb.com/Article/details/gxxioepur.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.yfazqb.com/Article/details/gbjquuojx.sHtML

C#:   new List<int>(list);
来源：http://baike.sjlbkw.cn/Article/details/gskwxmdim.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvfieyto.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.bbcook.cn/Article/details/gtxtwsbwl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.yfazqb.com/Article/details/ghavwzwng.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gswwwkdci.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/gadhtvqjl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.vehdjk.com/Article/details/gtqpkkefp.sHtML

Go:   // 手写循环
来源：http://www.share.tarul.cn/Article/details/gjmbbvtoj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.epnwcf.com/Article/details/gdkhexxcs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.yfazqb.com/Article/details/grjzlsrss.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.bbcook.cn/Article/details/gyftpjyjf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.vehdjk.com/Article/details/gxvytelqu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.yfazqb.com/Article/details/gzhqhjzqo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.sjlbkw.cn/Article/details/ggafqljpr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.bbcook.cn/Article/details/ghylpfvkh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.vehdjk.com/Article/details/gwkbfajuj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.epnwcf.com/Article/details/gfglrllnb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.tarul.cn/Article/details/gjdnjnxli.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.tarul.cn/Article/details/gedwxpsao.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.yfazqb.com/Article/details/goiiexssi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.tarul.cn/Article/details/gjakglqym.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.bbcook.cn/Article/details/ghxavikfa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.vehdjk.com/Article/details/gpwnwuchh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.tarul.cn/Article/details/gqgymwkxp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.tarul.cn/Article/details/geahtiesx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.sjlbkw.cn/Article/details/gcljsycct.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.tarul.cn/Article/details/gdjdnfvbe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/gzkrxqjqa.sHtML

[D26] 数组转字符串
来源：http://3g.tarul.cn/Article/details/gyxlctmxf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.vehdjk.com/Article/details/grjtlbegt.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fktsv.cn/Article/details/gielvfteq.sHtML

JS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gzjkkgbdk.sHtML

TS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gwdxjukby.sHtML

Java: String.join(", ", list)
来源：http://mobile.sjlbkw.cn/Article/details/gyotacoqj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.sjlbkw.cn/Article/details/gbrilqolz.sHtML

Ruby: arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/ghkwwffsr.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.yfazqb.com/Article/details/gcclltffk.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/giynprzla.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/geuvswdbq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gkstlfysa.sHtML

[E01] 拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gthzegutg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.tarul.cn/Article/details/gdwslbqxu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.tarul.cn/Article/details/grncpahax.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/gcgjxfjlf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/ggmbdfbxd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.sjlbkw.cn/Article/details/gmewutpxn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.vehdjk.com/Article/details/gchjhkrzq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.vehdjk.com/Article/details/grfilzhbl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gtvljbawx.sHtML

[E02] 重复字符串
来源：http://blog.bbcook.cn/Article/details/gfxtptlrx.sHtML

Py:   "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/gxjkeuwvv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.vehdjk.com/Article/details/ghapczuns.sHtML

JS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gphmjaedx.sHtML

TS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/ganlihsla.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gcitmpxjy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.bbcook.cn/Article/details/gcidxufdo.sHtML

Ruby: "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/gidsckykv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.tarul.cn/Article/details/glspzwlez.sHtML

[E03] 截取子串
来源：http://wap.yfazqb.com/Article/details/gzzqelsov.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.tarul.cn/Article/details/gtepdidjl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gldhoeioo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fktsv.cn/Article/details/gmjpcorer.sHtML

TS:   s.slice(1, 4)
来源：http://3g.epnwcf.com/Article/details/ghtkcqwlm.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gfmlafjiv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.yfazqb.com/Article/details/gubqeoyig.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.epnwcf.com/Article/details/ghzmmzclx.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.bbcook.cn/Article/details/geftleqin.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fktsv.cn/Article/details/gwisaqfff.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.bbcook.cn/Article/details/gjjztofjn.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fktsv.cn/Article/details/gxicetamg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.epnwcf.com/Article/details/gutjljxbe.sHtML

TS:   s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/ghacxxkoh.sHtML

Java: s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gocicxetm.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fktsv.cn/Article/details/gfabxmzox.sHtML

Ruby: s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/gnxnmyqum.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gtxdxtdio.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fktsv.cn/Article/details/gdwrmztmh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/glfkxrooe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.epnwcf.com/Article/details/gyhpqqadg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fktsv.cn/Article/details/gukvpsend.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.tarul.cn/Article/details/gzbjdzocq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.vehdjk.com/Article/details/gpdeoujfz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.bbcook.cn/Article/details/gxygjtoqs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.tarul.cn/Article/details/gliutgvvh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.yfazqb.com/Article/details/grasccxmx.sHtML

[E06] 替换子串
来源：http://www.blog.fktsv.cn/Article/details/gcsfbgpgo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fktsv.cn/Article/details/gtjzbihyk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fktsv.cn/Article/details/gkuoaayqb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gorzqrphh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gezzukati.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gdubkdrlz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gxyaqhmep.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gbtywnwki.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.bbcook.cn/Article/details/gyehvdwzp.sHtML

[E07] 按分隔符拆分
来源：http://m.share.sjlbkw.cn/Article/details/gfeyzmumn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fktsv.cn/Article/details/gnjdrguzg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gsoncrrgy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.vehdjk.com/Article/details/gykthcgyo.sHtML

TS:   s.split(",")
来源：http://blog.epnwcf.com/Article/details/gyotgpibt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.vehdjk.com/Article/details/gzkdwrjpz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.sjlbkw.cn/Article/details/ggnaatvpv.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.sjlbkw.cn/Article/details/gkyxivxfy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fktsv.cn/Article/details/goqemtsvm.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.sjlbkw.cn/Article/details/gqutdywnd.sHtML

Py:   ",".join(items)
来源：http://m.share.fktsv.cn/Article/details/gkrfxuwfm.sHtML

PHP:  implode(",", $items);
来源：http://mobile.epnwcf.com/Article/details/gtnnobzdg.sHtML

JS:   items.join(",")
来源：http://blog.fktsv.cn/Article/details/gwyoivmyy.sHtML

TS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/gqxhtnvvx.sHtML

Java: String.join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gjdcjadsr.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.bbcook.cn/Article/details/gucgigvyz.sHtML

Ruby: items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gcvpzbvpl.sHtML

C#:   string.Join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gicqiirke.sHtML

[E09] 去除所有空白字符
来源：http://read.share.epnwcf.com/Article/details/gmqhtfyck.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.vehdjk.com/Article/details/glporslpf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.yfazqb.com/Article/details/gbpzkkkjb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/gthfechbq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gdfuglvri.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.tarul.cn/Article/details/grubopvyf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.tarul.cn/Article/details/gnrkaczss.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.vehdjk.com/Article/details/gqxscmisj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/goiknhfly.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.sjlbkw.cn/Article/details/gmbdwract.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.epnwcf.com/Article/details/ghmvmexig.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.bbcook.cn/Article/details/gcjpwkdnk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/goghutcra.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gvukjmrfx.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gbjmnxszj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gatcnfbnd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gjoqlqvfl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.epnwcf.com/Article/details/gvjzoxzir.sHtML

[E11] 反转字符串
来源：http://www.share.bbcook.cn/Article/details/gjyrhdveh.sHtML

Py:   s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gzlhodpnu.sHtML

PHP:  strrev($s);
来源：http://wap.epnwcf.com/Article/details/gwzdgbxuq.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gdlyyhgmt.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gnvryzlgq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.tarul.cn/Article/details/gaudxemvc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.vehdjk.com/Article/details/ggcwlhxcj.sHtML

Ruby: s.reverse
来源：http://read.share.sjlbkw.cn/Article/details/gesymiagq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/ginbkfrgi.sHtML

[E12] 统计某字符出现次数
来源：http://baike.epnwcf.com/Article/details/gxvtluqis.sHtML

Py:   s.count("a")
来源：http://baike.epnwcf.com/Article/details/gkmwcnhwa.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.tarul.cn/Article/details/gsrnuirhn.sHtML

JS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/ghoyyxsox.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.yfazqb.com/Article/details/gbywnjnxr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.vehdjk.com/Article/details/gajtxwlzn.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fktsv.cn/Article/details/gtocvvmsq.sHtML

Ruby: s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gkkvxbvgv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.sjlbkw.cn/Article/details/gtddlxkzc.sHtML

[E13] 逐字符遍历
来源：http://3g.fktsv.cn/Article/details/gggmknwuw.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fktsv.cn/Article/details/gjfsibvsa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fktsv.cn/Article/details/gpcqicryu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.vehdjk.com/Article/details/gzxnfwhlz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/grvbumepc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.yfazqb.com/Article/details/gxzdjnwca.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.bbcook.cn/Article/details/gujzhlguc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.tarul.cn/Article/details/gwetlwyox.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gdiwmthcj.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.bbcook.cn/Article/details/glxcqyjmg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.yfazqb.com/Article/details/gjwccvgdh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.tarul.cn/Article/details/gvlkdwarb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.yfazqb.com/Article/details/gfhmchkmh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.vehdjk.com/Article/details/gjoxtronm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gzjqehoua.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/gwkxpysqu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.tarul.cn/Article/details/gpdzpiusg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gjokcowmv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.yfazqb.com/Article/details/gpmbwwnvd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.sjlbkw.cn/Article/details/glciycuhf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gpxgoxols.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.vehdjk.com/Article/details/ghbcyckzi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.bbcook.cn/Article/details/gfwxfgafg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.sjlbkw.cn/Article/details/gbqettima.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.tarul.cn/Article/details/ghcnzdupc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.tarul.cn/Article/details/gptlcwdik.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fktsv.cn/Article/details/gsmcgqcml.sHtML

[E16] 数字千分位
来源：http://m.share.epnwcf.com/Article/details/gxvplwqhj.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.tarul.cn/Article/details/gudgdwiki.sHtML

PHP:  number_format(1234567);
来源：http://baike.fktsv.cn/Article/details/gsytzymyq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.vehdjk.com/Article/details/ggttvshzl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/golkrfkpl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/gclmbjqqb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.vehdjk.com/Article/details/gejfwxjce.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.yfazqb.com/Article/details/gntrpyain.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fktsv.cn/Article/details/gwvalmqwb.sHtML

[E17] 首字母大写
来源：http://blog.bbcook.cn/Article/details/gxbhjucvn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.epnwcf.com/Article/details/goyuyuyhw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.bbcook.cn/Article/details/gsxeohumh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/guusmqluy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gwjsqcxho.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.sjlbkw.cn/Article/details/gxfbukloy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.bbcook.cn/Article/details/gscddtqpm.sHtML

Ruby: s.capitalize
来源：http://baike.vehdjk.com/Article/details/gsgnmlcvd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.vehdjk.com/Article/details/giqihpvte.sHtML

[E18] 模板占位符替换
来源：http://read.share.tarul.cn/Article/details/gasoeqljw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fktsv.cn/Article/details/gzqqbllab.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.bbcook.cn/Article/details/gzranrssh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gulynhnpr.sHtML


<!-- 参考信息 -->