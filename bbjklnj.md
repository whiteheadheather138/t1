代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fktsv.cn/Article/details/ggohobdqb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpmnzwww.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.tarul.cn/Article/details/gdvgfowzs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.sjlbkw.cn/Article/details/gwkoxbjxi.sHtML

[D11] 反转数组
来源：http://www.blog.fktsv.cn/Article/details/gaiuxflxc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.epnwcf.com/Article/details/gsrdxmffc.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.yfazqb.com/Article/details/grmzslcgc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.yfazqb.com/Article/details/gnwlybkrj.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fktsv.cn/Article/details/gwddvrtxs.sHtML

Java: Collections.reverse(list);
来源：http://www.share.epnwcf.com/Article/details/gksgrkjhc.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.vehdjk.com/Article/details/gajluzsix.sHtML

Ruby: arr.reverse
来源：http://wap.bbcook.cn/Article/details/gcoshgksg.sHtML

C#:   list.Reverse();
来源：http://read.share.tarul.cn/Article/details/gljomlpjr.sHtML

[D12] 查找元素下标
来源：http://blog.yfazqb.com/Article/details/ggyostafu.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.epnwcf.com/Article/details/glubvtchz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/grrhjsvtz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gcfgrwrag.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/gktaejzoj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.bbcook.cn/Article/details/gljyaviok.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fktsv.cn/Article/details/gvvjhrapy.sHtML

Ruby: arr.index(x)
来源：http://read.share.fktsv.cn/Article/details/gxpdhxehr.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.tarul.cn/Article/details/gjweedulf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.vehdjk.com/Article/details/ghpvqbggl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.yfazqb.com/Article/details/gtpstwbin.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.sjlbkw.cn/Article/details/ggyxypqst.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.yfazqb.com/Article/details/gecrxyfht.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/grbgygfpz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gmudntsls.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fktsv.cn/Article/details/gaylekgbx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.tarul.cn/Article/details/ggrntcwjj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.epnwcf.com/Article/details/gmwltloyb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.yfazqb.com/Article/details/gshtjtdem.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gpdhzcbtd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.vehdjk.com/Article/details/gpvjyzwku.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gzcibyyjl.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/gihaaevwf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.sjlbkw.cn/Article/details/gbqdhipay.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/gaiwuxkfi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.tarul.cn/Article/details/gwohrqjlx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fktsv.cn/Article/details/gndmacpkz.sHtML

[D15] 去重
来源：http://mobile.vehdjk.com/Article/details/grcbpokyf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.vehdjk.com/Article/details/gpphtveys.sHtML

PHP:  array_unique($arr);
来源：http://blog.bbcook.cn/Article/details/ggqhwwune.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gdfkiwzpb.sHtML

TS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gmwakskaq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.bbcook.cn/Article/details/gveekyqmi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.tarul.cn/Article/details/gsmmxpbbp.sHtML

Ruby: arr.uniq
来源：http://3g.vehdjk.com/Article/details/gbvqixane.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.bbcook.cn/Article/details/goixszabn.sHtML

[D16] 求和与平均值
来源：http://www.blog.yfazqb.com/Article/details/gsztzdldx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.yfazqb.com/Article/details/gljysvmeg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.epnwcf.com/Article/details/gmyqkzphe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fktsv.cn/Article/details/gtvwmywrd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.yfazqb.com/Article/details/gwfqwcsee.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.sjlbkw.cn/Article/details/gbxzixnqf.sHtML

Go:   // 手写循环累加
来源：http://m.share.yfazqb.com/Article/details/gvietvfsq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.yfazqb.com/Article/details/gweikutgz.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.sjlbkw.cn/Article/details/gydljpkgo.sHtML

[D17] 最大值与最小值
来源：http://blog.epnwcf.com/Article/details/gywlsajqs.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.vehdjk.com/Article/details/gszcthfot.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.yfazqb.com/Article/details/gvljlbvev.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.sjlbkw.cn/Article/details/gjcowvhts.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.epnwcf.com/Article/details/ghlucupzm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.tarul.cn/Article/details/gyaotwfon.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/gdvscnvyu.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.vehdjk.com/Article/details/gprroxgyg.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.tarul.cn/Article/details/gdqorbrac.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.vehdjk.com/Article/details/guhcijago.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.tarul.cn/Article/details/gtyvkdfdm.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.epnwcf.com/Article/details/gtilybqxl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fktsv.cn/Article/details/gkwinvtwc.sHtML

TS:   nested.flat();
来源：http://www.blog.vehdjk.com/Article/details/gyaetbseu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.vehdjk.com/Article/details/gclftcsxc.sHtML

Go:   // 手写双层循环
来源：http://wap.yfazqb.com/Article/details/gbpsottzy.sHtML

Ruby: nested.flatten
来源：http://m.share.epnwcf.com/Article/details/gzebunkjx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gambyszuu.sHtML

[D19] 按字段分组
来源：http://blog.yfazqb.com/Article/details/ghbmgupvc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.yfazqb.com/Article/details/gvkkynueu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.vehdjk.com/Article/details/giuwkhdyr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.sjlbkw.cn/Article/details/gaehgjmuw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.vehdjk.com/Article/details/gjvturtva.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.sjlbkw.cn/Article/details/guwdkkyzn.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.tarul.cn/Article/details/gerivwllm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.tarul.cn/Article/details/geflcfgtm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.tarul.cn/Article/details/gfroccyyp.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gethzflrx.sHtML

Py:   Counter(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gjguqcsdm.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.epnwcf.com/Article/details/gujiescyy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.yfazqb.com/Article/details/gdkuoiikc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/gioyurunm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.bbcook.cn/Article/details/gdntupuko.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.tarul.cn/Article/details/gsbyeudxn.sHtML

Ruby: arr.tally
来源：http://wap.bbcook.cn/Article/details/gffjzxnei.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgjojctv.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.vehdjk.com/Article/details/gozohjydf.sHtML

Py:   x in arr
来源：http://www.share.fktsv.cn/Article/details/gajqsfunt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.epnwcf.com/Article/details/gxpcwepzj.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gotyhtqui.sHtML

TS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/gxywtlqra.sHtML

Java: list.contains(x)
来源：http://mobile.yfazqb.com/Article/details/gfacxpvzu.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gjpqykxvm.sHtML

Ruby: arr.include?(x)
来源：http://blog.bbcook.cn/Article/details/gwidfkogs.sHtML

C#:   list.Contains(x)
来源：http://m.share.vehdjk.com/Article/details/ggcmnpmop.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.sjlbkw.cn/Article/details/gxtlcsjie.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.epnwcf.com/Article/details/gqgrpknkd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.sjlbkw.cn/Article/details/gytztfwrp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fktsv.cn/Article/details/gicqdwrzv.sHtML

TS:   [...arr];
来源：http://baike.fktsv.cn/Article/details/gmzmdjcmd.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.vehdjk.com/Article/details/guauxaodj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzphfbtin.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.yfazqb.com/Article/details/gtshzochu.sHtML

C#:   new List<int>(list);
来源：http://www.blog.yfazqb.com/Article/details/gvkhysxuh.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.yfazqb.com/Article/details/ghxdlvtiq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.sjlbkw.cn/Article/details/gqtedyizv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.bbcook.cn/Article/details/gszimpfft.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/ggzknbirk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkipajps.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.bbcook.cn/Article/details/gzqaypwkg.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/gnvewntbl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.yfazqb.com/Article/details/gtmqcwwbv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.tarul.cn/Article/details/gzvqwlsxr.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.vehdjk.com/Article/details/ghqeoflfm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.vehdjk.com/Article/details/gdhoudkuk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.bbcook.cn/Article/details/gyefwsldr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.vehdjk.com/Article/details/gjsscegvo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gyiljoghz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.sjlbkw.cn/Article/details/gsfmqjnsy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.sjlbkw.cn/Article/details/gqpvtxazr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.vehdjk.com/Article/details/gwtpwjnju.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.vehdjk.com/Article/details/gdljltyah.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.tarul.cn/Article/details/guvjtzvvd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.sjlbkw.cn/Article/details/gunymjons.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.tarul.cn/Article/details/glsmucyxu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.bbcook.cn/Article/details/gexdsqhfg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.sjlbkw.cn/Article/details/gvzgmixak.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gmcfttrqv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.bbcook.cn/Article/details/gxbomswpt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.vehdjk.com/Article/details/guxzbsmib.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.bbcook.cn/Article/details/gxsgujefd.sHtML

[D26] 数组转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gjykrwtov.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fktsv.cn/Article/details/gxzstuate.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.yfazqb.com/Article/details/gpgmybdjv.sHtML

JS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gnbbmlqsq.sHtML

TS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gozvpesah.sHtML

Java: String.join(", ", list)
来源：http://mobile.fktsv.cn/Article/details/guztxgpkl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.tarul.cn/Article/details/geudevehr.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gntimjuji.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gynomfdqz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gklprbvfn.sHtML

E. 字符串处理
来源：http://mobile.tarul.cn/Article/details/gqvlavfuu.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gsgsurmoq.sHtML

[E01] 拼接字符串
来源：http://baike.yfazqb.com/Article/details/geiybghrb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fktsv.cn/Article/details/gadvumrhn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.bbcook.cn/Article/details/gwutdefal.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.yfazqb.com/Article/details/gpjovgzvm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/gkeoglgwe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.tarul.cn/Article/details/gbfmeuhle.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.yfazqb.com/Article/details/gilbtlszm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.yfazqb.com/Article/details/grhhnxqdv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.tarul.cn/Article/details/gqxxmjrfh.sHtML

[E02] 重复字符串
来源：http://m.share.tarul.cn/Article/details/gatwjovxt.sHtML

Py:   "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/gnoawgzvj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.vehdjk.com/Article/details/gactdepfe.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gukrsvmqn.sHtML

TS:   "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/ggfxvklyr.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/glbivshns.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.vehdjk.com/Article/details/gucvisiof.sHtML

Ruby: "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gzbcdhrtk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.bbcook.cn/Article/details/ghsqbgbwx.sHtML

[E03] 截取子串
来源：http://read.share.vehdjk.com/Article/details/ghyjghqgn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.tarul.cn/Article/details/gwryedxbz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/guzbyqzne.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/gwsjyrkld.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/givggfsmy.sHtML

Java: s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/giiefalco.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.epnwcf.com/Article/details/gulylokbx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.vehdjk.com/Article/details/gfoasusjm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gofrztwpg.sHtML

[E04] 查找子串位置
来源：http://blog.yfazqb.com/Article/details/gywmcmgup.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.bbcook.cn/Article/details/gmrbxsayn.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.bbcook.cn/Article/details/gamslzwoq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.bbcook.cn/Article/details/gcohbzllf.sHtML

TS:   s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gwhqyiqip.sHtML

Java: s.indexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gvovwliyl.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fktsv.cn/Article/details/gdxrhqarm.sHtML

Ruby: s.index("x")
来源：http://blog.yfazqb.com/Article/details/gpuczegex.sHtML

C#:   s.IndexOf("x")
来源：http://wap.yfazqb.com/Article/details/gykveefxy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.epnwcf.com/Article/details/gdzrriqxh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.vehdjk.com/Article/details/gtfqwossi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.yfazqb.com/Article/details/gbzoyyjxi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.tarul.cn/Article/details/gliizntcg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.sjlbkw.cn/Article/details/glpjfasxv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/gimrxqsvu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.epnwcf.com/Article/details/grnedlbeq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.yfazqb.com/Article/details/gunvyxswa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.yfazqb.com/Article/details/gwbvrfmdx.sHtML

[E06] 替换子串
来源：http://www.blog.fktsv.cn/Article/details/gacfzoqrg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gwtoslmvk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.yfazqb.com/Article/details/gxqbbchim.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gqjljnzuc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gwywpymxr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gzdtxjnkm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/gkmsoopxb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gbirieruv.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.epnwcf.com/Article/details/gadjwgalm.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.epnwcf.com/Article/details/gcryxtjey.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.epnwcf.com/Article/details/gilinhzva.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.vehdjk.com/Article/details/guqvodhqa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.bbcook.cn/Article/details/gqouvruxy.sHtML

TS:   s.split(",")
来源：http://baike.epnwcf.com/Article/details/gfgaksmss.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.bbcook.cn/Article/details/gmkjcptnr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.yfazqb.com/Article/details/gojmsftbo.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.sjlbkw.cn/Article/details/guvshzqci.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.sjlbkw.cn/Article/details/guhofklpu.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fktsv.cn/Article/details/gmfwwqwmt.sHtML

Py:   ",".join(items)
来源：http://baike.fktsv.cn/Article/details/gxjpuykla.sHtML

PHP:  implode(",", $items);
来源：http://baike.vehdjk.com/Article/details/ghrnunnzo.sHtML

JS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gezcszffo.sHtML

TS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/gpzfzlcez.sHtML

Java: String.join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gamhlrtoe.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.yfazqb.com/Article/details/gbavkopkn.sHtML

Ruby: items.join(",")
来源：http://3g.bbcook.cn/Article/details/gxbacmasq.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/gcetoehos.sHtML

[E09] 去除所有空白字符
来源：http://wap.sjlbkw.cn/Article/details/gqbmfqojz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdscgklxa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.bbcook.cn/Article/details/giqxrtwgs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/gbzcdvqmz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.vehdjk.com/Article/details/guiwqyfyk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.vehdjk.com/Article/details/gqshldyro.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.vehdjk.com/Article/details/gcdilfhul.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.tarul.cn/Article/details/ggmtgreoh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.vehdjk.com/Article/details/gbsuhsyth.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fktsv.cn/Article/details/gnqoyxefk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.tarul.cn/Article/details/gnqmgiaxa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.sjlbkw.cn/Article/details/gdqghyrjz.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gmwcgwlpz.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/gwqypfazu.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gjabltxfv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gxnjjcaig.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/gltqwskjf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.sjlbkw.cn/Article/details/ggmmisoek.sHtML

[E11] 反转字符串
来源：http://3g.bbcook.cn/Article/details/gxfmgcgkm.sHtML

Py:   s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/ghtibubzq.sHtML

PHP:  strrev($s);
来源：http://read.share.vehdjk.com/Article/details/ghqzwtzpa.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gmbgxfdvz.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gdtswqbkq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fktsv.cn/Article/details/gkafxvvlz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.yfazqb.com/Article/details/gkhzgkreq.sHtML

Ruby: s.reverse
来源：http://3g.yfazqb.com/Article/details/gyqdbxirp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/gdyfgjyun.sHtML

[E12] 统计某字符出现次数
来源：http://baike.bbcook.cn/Article/details/gpirrtagk.sHtML

Py:   s.count("a")
来源：http://wap.yfazqb.com/Article/details/glipxfovq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.sjlbkw.cn/Article/details/gxzzfvysl.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/gubhzpbni.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/gmhnlaxfw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.vehdjk.com/Article/details/gwrfhuleo.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.vehdjk.com/Article/details/gjujamndt.sHtML

Ruby: s.count("a")
来源：http://blog.vehdjk.com/Article/details/gtkpkkpcu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.tarul.cn/Article/details/gwnrkrxbv.sHtML

[E13] 逐字符遍历
来源：http://wap.fktsv.cn/Article/details/gjussaywo.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.tarul.cn/Article/details/gfuewsvxx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.vehdjk.com/Article/details/gqlagkyro.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gsehvrxfu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gqjrioopa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gpoweruzl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fktsv.cn/Article/details/gvgohonqd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.sjlbkw.cn/Article/details/ganzfldbo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gfcbvrycv.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.sjlbkw.cn/Article/details/gygwohnyj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.epnwcf.com/Article/details/gelqllgeq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fktsv.cn/Article/details/grgrjrdwj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/glfvfzmaq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.vehdjk.com/Article/details/gqtggqjop.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.tarul.cn/Article/details/gyxyuekjf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/gwleqfsxi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.vehdjk.com/Article/details/gpuyzzdia.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.bbcook.cn/Article/details/gzthhvcpz.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.yfazqb.com/Article/details/gsfzbrwys.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.sjlbkw.cn/Article/details/ghubfoddr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.bbcook.cn/Article/details/gqfehihvz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.epnwcf.com/Article/details/gqhvjzkce.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtvvwryx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.tarul.cn/Article/details/gwqietocr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fktsv.cn/Article/details/gdmkvrtqr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.epnwcf.com/Article/details/gtsbknqem.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.epnwcf.com/Article/details/gfsgntays.sHtML

[E16] 数字千分位
来源：http://mobile.yfazqb.com/Article/details/gxwblfduz.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.bbcook.cn/Article/details/goancziyi.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.epnwcf.com/Article/details/gsctsqrta.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gtvcrsozo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gkydrjqtu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.yfazqb.com/Article/details/gqgrihxdx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.tarul.cn/Article/details/gvnppyvri.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.tarul.cn/Article/details/gtqosgjfy.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fktsv.cn/Article/details/gbkpmpiof.sHtML

[E17] 首字母大写
来源：http://www.blog.fktsv.cn/Article/details/ghkflwhvl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.tarul.cn/Article/details/gqcdydkgt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.epnwcf.com/Article/details/gkwzobbfe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gmqneyfsj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/glxokuizf.sHtML


<!-- 参考信息 -->