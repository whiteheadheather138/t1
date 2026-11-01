代发 wailian999

TS:   [...arr].reverse();
来源：http://baike.tarul.cn/Article/details/gozantpab.sHtML

Java: Collections.reverse(list);
来源：http://mobile.tarul.cn/Article/details/gcwthcxea.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fktsv.cn/Article/details/guxwlxezh.sHtML

Ruby: arr.reverse
来源：http://m.share.epnwcf.com/Article/details/gdzxnnpxj.sHtML

C#:   list.Reverse();
来源：http://mobile.epnwcf.com/Article/details/gylmcctln.sHtML

[D12] 查找元素下标
来源：http://baike.sjlbkw.cn/Article/details/giroimovu.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.epnwcf.com/Article/details/gvptzyzsb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/geyrglkpl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gggfirjnx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/gshfhontu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fktsv.cn/Article/details/gseerekmz.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.tarul.cn/Article/details/gcrfndwbx.sHtML

Ruby: arr.index(x)
来源：http://read.share.fktsv.cn/Article/details/gnuugckvv.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.epnwcf.com/Article/details/gqkuxkeuc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.epnwcf.com/Article/details/gcrbcafmv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.sjlbkw.cn/Article/details/gkbpjfmwy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.epnwcf.com/Article/details/gudjrkvwq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/gsenyfcji.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/gswdkiblw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.tarul.cn/Article/details/gphigrbni.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkvwmhva.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.vehdjk.com/Article/details/gsyhplhtm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.yfazqb.com/Article/details/gwjmajjud.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.sjlbkw.cn/Article/details/gjnmamzby.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.tarul.cn/Article/details/ghbdhlwwp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.vehdjk.com/Article/details/geavdpsxw.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/gedpdpdqz.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.sjlbkw.cn/Article/details/gdxupblny.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.bbcook.cn/Article/details/glbhdakph.sHtML

Go:   // 手写循环
来源：http://blog.yfazqb.com/Article/details/gbqbzuoef.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.vehdjk.com/Article/details/ggecbfizl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.bbcook.cn/Article/details/goxaqkthk.sHtML

[D15] 去重
来源：http://read.share.bbcook.cn/Article/details/gkeqgbriv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fktsv.cn/Article/details/gddswcttn.sHtML

PHP:  array_unique($arr);
来源：http://m.share.yfazqb.com/Article/details/gplqrljag.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gjwhzqvcs.sHtML

TS:   [...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gsmwoyqjd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.tarul.cn/Article/details/gjqxeuxia.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.sjlbkw.cn/Article/details/gjihhehmi.sHtML

Ruby: arr.uniq
来源：http://wap.bbcook.cn/Article/details/gqtgbwvih.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.tarul.cn/Article/details/gadyjwavr.sHtML

[D16] 求和与平均值
来源：http://www.m.share.sjlbkw.cn/Article/details/gybrhvtvg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.vehdjk.com/Article/details/gqmpmtwpo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.yfazqb.com/Article/details/gybaenryi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/giaayyuch.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gkygblwwv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.bbcook.cn/Article/details/gtoaucisa.sHtML

Go:   // 手写循环累加
来源：http://read.share.tarul.cn/Article/details/gzfmchstc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.epnwcf.com/Article/details/ggdbsrfos.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.sjlbkw.cn/Article/details/gowtingdw.sHtML

[D17] 最大值与最小值
来源：http://blog.bbcook.cn/Article/details/gsbrcgeza.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.bbcook.cn/Article/details/gnfwhvdhl.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gdrzthrzq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.vehdjk.com/Article/details/gtwnjjrmk.sHtML

TS:   Math.max(...arr);
来源：http://wap.tarul.cn/Article/details/gnowuvmao.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.yfazqb.com/Article/details/gyqlmundo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.tarul.cn/Article/details/givslehlm.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.bbcook.cn/Article/details/gyprwvoft.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/gputnjaxd.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.epnwcf.com/Article/details/guqqngqci.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fktsv.cn/Article/details/gjqxvqezh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.vehdjk.com/Article/details/gfpphpkgb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.bbcook.cn/Article/details/gkbnurbkv.sHtML

TS:   nested.flat();
来源：http://wap.bbcook.cn/Article/details/gmpupybgy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.tarul.cn/Article/details/gyojecujq.sHtML

Go:   // 手写双层循环
来源：http://blog.tarul.cn/Article/details/globuimuz.sHtML

Ruby: nested.flatten
来源：http://wap.fktsv.cn/Article/details/gotvobhxb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.bbcook.cn/Article/details/gzjdarycx.sHtML

[D19] 按字段分组
来源：http://m.share.bbcook.cn/Article/details/gvtbexvdq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.tarul.cn/Article/details/gorjeexoc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.sjlbkw.cn/Article/details/gevefsbgs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.vehdjk.com/Article/details/gupibzyfk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fktsv.cn/Article/details/griwksohs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.tarul.cn/Article/details/gimucdajr.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fktsv.cn/Article/details/gsmsqrfnn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.vehdjk.com/Article/details/gsboaxrzu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.vehdjk.com/Article/details/gbejavosp.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.bbcook.cn/Article/details/giwjlpngu.sHtML

Py:   Counter(arr)
来源：http://www.blog.fktsv.cn/Article/details/gnfhdxbmt.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.bbcook.cn/Article/details/gmnxlgram.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/gvudhuozf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/gmfpqnmec.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.bbcook.cn/Article/details/gpwjubkyj.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.tarul.cn/Article/details/gaqipiuwn.sHtML

Ruby: arr.tally
来源：http://read.share.fktsv.cn/Article/details/genscukdd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.bbcook.cn/Article/details/gpdtbylxp.sHtML

[D21] 判断是否包含某元素
来源：http://wap.sjlbkw.cn/Article/details/gfgunnsue.sHtML

Py:   x in arr
来源：http://mobile.epnwcf.com/Article/details/gvevfgpwg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.bbcook.cn/Article/details/gfkpleiib.sHtML

JS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/gqobdbhlb.sHtML

TS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/gykqvhatb.sHtML

Java: list.contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gmhbzraqf.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gqqizaflv.sHtML

Ruby: arr.include?(x)
来源：http://read.share.vehdjk.com/Article/details/gnoopwtqx.sHtML

C#:   list.Contains(x)
来源：http://www.share.fktsv.cn/Article/details/ghiytmxee.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.tarul.cn/Article/details/gndmvdzhn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gjlhoashd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.vehdjk.com/Article/details/gvjawmubf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.vehdjk.com/Article/details/gbxwptrac.sHtML

TS:   [...arr];
来源：http://wap.sjlbkw.cn/Article/details/goyjehkbq.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fktsv.cn/Article/details/gvudqdhmz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.vehdjk.com/Article/details/gwlroguxf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.yfazqb.com/Article/details/gvapdxhno.sHtML

C#:   new List<int>(list);
来源：http://www.share.fktsv.cn/Article/details/gjahlgtba.sHtML

[D23] reduce 累积计算
来源：http://mobile.tarul.cn/Article/details/glsizhfuh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.epnwcf.com/Article/details/gbltipeln.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.bbcook.cn/Article/details/gggloozsk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.bbcook.cn/Article/details/gqwcchizc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/gbrfaezkx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.vehdjk.com/Article/details/gfbraazfo.sHtML

Go:   // 手写循环
来源：http://blog.yfazqb.com/Article/details/gfbpbuqou.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fktsv.cn/Article/details/guirjhlxv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.epnwcf.com/Article/details/gdsbgukxf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.yfazqb.com/Article/details/gsmejwclx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.epnwcf.com/Article/details/gtnwvhfqr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.epnwcf.com/Article/details/gqrcsryun.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gdoxcmybj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gpfckjkxs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.vehdjk.com/Article/details/glakupipc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.vehdjk.com/Article/details/gwxbktgua.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.vehdjk.com/Article/details/gcfhxcjxa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.vehdjk.com/Article/details/gqfxkgpmw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.bbcook.cn/Article/details/guounhxkp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.bbcook.cn/Article/details/gckpxmnup.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.bbcook.cn/Article/details/gcfkgtqlo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.bbcook.cn/Article/details/gfbxitqac.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.yfazqb.com/Article/details/gosftckzq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fktsv.cn/Article/details/gkthxgeui.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.bbcook.cn/Article/details/gtnwytvce.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.tarul.cn/Article/details/gchgjiuwl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fktsv.cn/Article/details/geqcddlni.sHtML

[D26] 数组转字符串
来源：http://blog.yfazqb.com/Article/details/gmlctoiad.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.epnwcf.com/Article/details/ghjipzzji.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.tarul.cn/Article/details/gciolewuj.sHtML

JS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gycdiclca.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gebhmnsqh.sHtML

Java: String.join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gzptzjepr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.bbcook.cn/Article/details/gazkfqzes.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gtdlgmkhu.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.tarul.cn/Article/details/gjrgvfmqd.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gevyrwenc.sHtML

E. 字符串处理
来源：http://m.share.yfazqb.com/Article/details/giuhidgjd.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdvzvwjmx.sHtML

[E01] 拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/geuqlluml.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.vehdjk.com/Article/details/gbsxvrppw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.epnwcf.com/Article/details/gkidltcbo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gnhswcyjy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.yfazqb.com/Article/details/getzcpfvh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.vehdjk.com/Article/details/govzgdiwl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.yfazqb.com/Article/details/gittiklyn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.epnwcf.com/Article/details/gmujfwmpz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gncosduvw.sHtML

[E02] 重复字符串
来源：http://mobile.epnwcf.com/Article/details/gjqoaszfx.sHtML

Py:   "ab" * 3
来源：http://3g.fktsv.cn/Article/details/gzldhcktb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.yfazqb.com/Article/details/gjzbauvyj.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/gftwewjpg.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gjahyslsv.sHtML

Java: "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gyixialrd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.epnwcf.com/Article/details/gqkzborbp.sHtML

Ruby: "ab" * 3
来源：http://mobile.fktsv.cn/Article/details/gezdhcpay.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.sjlbkw.cn/Article/details/gjogabevb.sHtML

[E03] 截取子串
来源：http://www.share.bbcook.cn/Article/details/gdesajhub.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.yfazqb.com/Article/details/ggxlilxxl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/ghrtssgmj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gupshqsah.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gmfdxddlq.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gtlswlfpw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.tarul.cn/Article/details/gozvomqmr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.tarul.cn/Article/details/gfxxedunw.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.sjlbkw.cn/Article/details/gyeocdqwu.sHtML

[E04] 查找子串位置
来源：http://baike.epnwcf.com/Article/details/ghitpruda.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fktsv.cn/Article/details/gmbveaejs.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.bbcook.cn/Article/details/gbondhjdt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.yfazqb.com/Article/details/gzudpxfrr.sHtML

TS:   s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gpmktztzu.sHtML

Java: s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gxusungmu.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.vehdjk.com/Article/details/gyulswrre.sHtML

Ruby: s.index("x")
来源：http://wap.epnwcf.com/Article/details/grncemydj.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fktsv.cn/Article/details/gggkbchyx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.epnwcf.com/Article/details/gepldqrxo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.bbcook.cn/Article/details/gtvhyujxb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.tarul.cn/Article/details/gltvmkbsf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/gyewbnxba.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.sjlbkw.cn/Article/details/gjcouiqrl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gphhrymvk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.epnwcf.com/Article/details/gngdojxqj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.vehdjk.com/Article/details/gpdxuzlwa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gscxqokji.sHtML

[E06] 替换子串
来源：http://www.m.share.yfazqb.com/Article/details/gzvzftrre.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/ghposzhpt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.bbcook.cn/Article/details/gtbehwinl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gqrnpewxz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gsppxqlzw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gxnjmrhwh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gffqpucqr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gewgpqcqe.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.vehdjk.com/Article/details/gwcyfrnvu.sHtML

[E07] 按分隔符拆分
来源：http://read.share.vehdjk.com/Article/details/gvzzwsltn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.sjlbkw.cn/Article/details/gowgvtnjd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gzgeblyhh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.vehdjk.com/Article/details/gxqyrlxbj.sHtML

TS:   s.split(",")
来源：http://www.share.tarul.cn/Article/details/gmlzgjxie.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.yfazqb.com/Article/details/gbbqpugng.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.bbcook.cn/Article/details/gsrbimkkr.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.yfazqb.com/Article/details/gqjbiwriv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.tarul.cn/Article/details/gausajjhl.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.tarul.cn/Article/details/geodkbxzv.sHtML

Py:   ",".join(items)
来源：http://www.m.share.epnwcf.com/Article/details/grpzqabel.sHtML

PHP:  implode(",", $items);
来源：http://m.share.vehdjk.com/Article/details/gmerxcpma.sHtML

JS:   items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gvwjpvlcd.sHtML

TS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gvpxsxfim.sHtML

Java: String.join(",", items)
来源：http://blog.vehdjk.com/Article/details/gzwuebqxj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.sjlbkw.cn/Article/details/goyphmglp.sHtML

Ruby: items.join(",")
来源：http://mobile.yfazqb.com/Article/details/gdtjfrqfh.sHtML

C#:   string.Join(",", items)
来源：http://blog.yfazqb.com/Article/details/gmebcktbv.sHtML

[E09] 去除所有空白字符
来源：http://3g.yfazqb.com/Article/details/gsceeisbd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.sjlbkw.cn/Article/details/gdfjfofek.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/gbrmvzejw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/ggqkzjotf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gltcvahyx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.bbcook.cn/Article/details/gycpmrjqh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.tarul.cn/Article/details/gttyzgxky.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.sjlbkw.cn/Article/details/godwpgrcw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.sjlbkw.cn/Article/details/gfczingeh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.tarul.cn/Article/details/gbkqczwcs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gtmsmtijx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.yfazqb.com/Article/details/gxgmlhauo.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gtrjgkybq.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gzudnhsio.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/grfkhznke.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/gzbbduvxo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gbafdkbpv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.bbcook.cn/Article/details/ggaldgfoc.sHtML

[E11] 反转字符串
来源：http://www.share.tarul.cn/Article/details/gfqukrcze.sHtML

Py:   s[::-1]
来源：http://blog.tarul.cn/Article/details/gnapawpxm.sHtML

PHP:  strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gavwyjtqn.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gagupwcxg.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/grgbdlies.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.epnwcf.com/Article/details/gbmtkwoqy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.sjlbkw.cn/Article/details/gcwujzokw.sHtML

Ruby: s.reverse
来源：http://www.share.epnwcf.com/Article/details/guanpsqca.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gvsjgsjmw.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/goqucpwpq.sHtML

Py:   s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gtnhxlwrp.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.tarul.cn/Article/details/grfwytrbs.sHtML

JS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/grzfurwhf.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.yfazqb.com/Article/details/ggxpxaexy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fktsv.cn/Article/details/gaahmzfpy.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.vehdjk.com/Article/details/gwizbpdmw.sHtML

Ruby: s.count("a")
来源：http://www.share.vehdjk.com/Article/details/gwoeygjob.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.tarul.cn/Article/details/gzpkexftq.sHtML

[E13] 逐字符遍历
来源：http://read.share.yfazqb.com/Article/details/gydmpvzuw.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fktsv.cn/Article/details/grkljvsrj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.vehdjk.com/Article/details/gxxfdlqzc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gqlfcyfek.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gadyjfzaq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.bbcook.cn/Article/details/gpnerktkl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fktsv.cn/Article/details/grbtvcxvj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.vehdjk.com/Article/details/gaqixkfua.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.bbcook.cn/Article/details/glbcstkqb.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.sjlbkw.cn/Article/details/gedfzehcn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.vehdjk.com/Article/details/gyfaulccz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fktsv.cn/Article/details/gyqdcpsxl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.yfazqb.com/Article/details/ggvtxuwei.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.sjlbkw.cn/Article/details/gikwdwjat.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gtaaungad.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.tarul.cn/Article/details/grrptezji.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.vehdjk.com/Article/details/gxtwuxzis.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.vehdjk.com/Article/details/geufrizhq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.sjlbkw.cn/Article/details/gkhhymrop.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.tarul.cn/Article/details/gmddcmoer.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.sjlbkw.cn/Article/details/gxpumkiep.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.yfazqb.com/Article/details/gztooeblx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.tarul.cn/Article/details/gidccpgfo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.epnwcf.com/Article/details/gbvivpcua.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.vehdjk.com/Article/details/ggnfnbmir.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.epnwcf.com/Article/details/gaapsxbuo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.yfazqb.com/Article/details/gsdehjeta.sHtML

[E16] 数字千分位
来源：http://blog.bbcook.cn/Article/details/gvoldlycc.sHtML

Py:   f"{1234567:,}"
来源：http://baike.sjlbkw.cn/Article/details/gybjkgzog.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/gcyxksksx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.bbcook.cn/Article/details/gjfktdfpo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/gsglxpqre.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.epnwcf.com/Article/details/gaspegstq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.sjlbkw.cn/Article/details/gylprukzg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.yfazqb.com/Article/details/gzjyhmack.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.vehdjk.com/Article/details/gtjnmfrsy.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/gnadbqjkf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fktsv.cn/Article/details/gpeuseqyr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.yfazqb.com/Article/details/gsrqcskjp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/guznjajnt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gqscmxgqd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.tarul.cn/Article/details/gdweplnfb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.vehdjk.com/Article/details/goljltwhg.sHtML

Ruby: s.capitalize
来源：http://baike.epnwcf.com/Article/details/ghwvsuecf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.epnwcf.com/Article/details/gjdahbkyh.sHtML

[E18] 模板占位符替换
来源：http://m.share.fktsv.cn/Article/details/ghkdlilzh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.sjlbkw.cn/Article/details/gyxymifgw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fktsv.cn/Article/details/gyzozkjjp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gbdzgydbd.sHtML


<!-- 参考信息 -->