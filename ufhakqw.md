代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.yfazqb.com/Article/details/ghxgygydf.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/gvyufejfx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.yfazqb.com/Article/details/gclqnkyco.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.tarul.cn/Article/details/gkdsisbjl.sHtML

[D15] 去重
来源：http://baike.tarul.cn/Article/details/gaxibkuyb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.yfazqb.com/Article/details/gyfofxkcc.sHtML

PHP:  array_unique($arr);
来源：http://wap.sjlbkw.cn/Article/details/grvdpsymm.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/gzfktvokn.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gzizpdrsf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.epnwcf.com/Article/details/gfhfntjxd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.bbcook.cn/Article/details/gavhxcmax.sHtML

Ruby: arr.uniq
来源：http://mobile.sjlbkw.cn/Article/details/gakifchij.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.vehdjk.com/Article/details/gmaldapui.sHtML

[D16] 求和与平均值
来源：http://blog.fktsv.cn/Article/details/gcswommal.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.tarul.cn/Article/details/gugbyshpu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gkosxtvte.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/gnmqsduke.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/grovyocaq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.yfazqb.com/Article/details/ghyjfbkow.sHtML

Go:   // 手写循环累加
来源：http://wap.sjlbkw.cn/Article/details/gdxqechzr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.sjlbkw.cn/Article/details/gasbohtfq.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.epnwcf.com/Article/details/gffmvdvuj.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/gemktwsyc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gpudebubv.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.tarul.cn/Article/details/gbskifaia.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fktsv.cn/Article/details/gwyujltzj.sHtML

TS:   Math.max(...arr);
来源：http://mobile.bbcook.cn/Article/details/gzfbnliia.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.tarul.cn/Article/details/gxbtbzigb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.yfazqb.com/Article/details/gllfvmikz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.yfazqb.com/Article/details/gexrchtre.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/gyethkxss.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.bbcook.cn/Article/details/gjlmmkglp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fktsv.cn/Article/details/gysjtbpba.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.vehdjk.com/Article/details/ggormbxjg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fktsv.cn/Article/details/gljlfpyjs.sHtML

TS:   nested.flat();
来源：http://m.share.tarul.cn/Article/details/gwcpjcktm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gshgxzfuw.sHtML

Go:   // 手写双层循环
来源：http://www.share.yfazqb.com/Article/details/gzwcqtcci.sHtML

Ruby: nested.flatten
来源：http://read.share.tarul.cn/Article/details/gdmhbtdcg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.yfazqb.com/Article/details/gepjmnokz.sHtML

[D19] 按字段分组
来源：http://blog.vehdjk.com/Article/details/gmeyucnzp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.vehdjk.com/Article/details/glctqsrzs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.epnwcf.com/Article/details/gaoixjwdz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.epnwcf.com/Article/details/gtzacgmjd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.tarul.cn/Article/details/gxicaksqe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fktsv.cn/Article/details/gjejhyrlp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.epnwcf.com/Article/details/gflbjrggr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.vehdjk.com/Article/details/ghomowmsi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.bbcook.cn/Article/details/glszlgdet.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gyvcebivt.sHtML

Py:   Counter(arr)
来源：http://3g.vehdjk.com/Article/details/ginlyftzz.sHtML

PHP:  array_count_values($arr);
来源：http://wap.yfazqb.com/Article/details/goehvdjum.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gbicdicaf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/gqfeuowvh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.tarul.cn/Article/details/gzasveznr.sHtML

Go:   // 手写 map[T]int
来源：http://3g.vehdjk.com/Article/details/gyqlbujfd.sHtML

Ruby: arr.tally
来源：http://www.m.share.tarul.cn/Article/details/ghipwvsuq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.tarul.cn/Article/details/gttuvekiw.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fktsv.cn/Article/details/gtolwwtsw.sHtML

Py:   x in arr
来源：http://baike.yfazqb.com/Article/details/gvislcosw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.epnwcf.com/Article/details/gaszzgonq.sHtML

JS:   arr.includes(x)
来源：http://read.share.epnwcf.com/Article/details/gfhgmerjt.sHtML

TS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gzcivupiq.sHtML

Java: list.contains(x)
来源：http://mobile.tarul.cn/Article/details/gbwvtpkjo.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fktsv.cn/Article/details/gaomdcfrt.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.tarul.cn/Article/details/gwnkdbggd.sHtML

C#:   list.Contains(x)
来源：http://mobile.yfazqb.com/Article/details/gqxauanwt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.epnwcf.com/Article/details/gydolijet.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fktsv.cn/Article/details/gidpuvpii.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.yfazqb.com/Article/details/ggbitkqdn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.vehdjk.com/Article/details/guziokukm.sHtML

TS:   [...arr];
来源：http://blog.epnwcf.com/Article/details/gjscfsldu.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fktsv.cn/Article/details/gcgleziwo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fktsv.cn/Article/details/gdvegwmhv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrdicfpj.sHtML

C#:   new List<int>(list);
来源：http://blog.vehdjk.com/Article/details/gjdilltvs.sHtML

[D23] reduce 累积计算
来源：http://mobile.yfazqb.com/Article/details/gxhltefve.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gwzcmavvi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fktsv.cn/Article/details/gqdmdkzry.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/gkliwauqe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.bbcook.cn/Article/details/gcuebejhx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.yfazqb.com/Article/details/gconjaezz.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gxfleeckx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.vehdjk.com/Article/details/gwwexdwxv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fktsv.cn/Article/details/gojbqxohi.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.sjlbkw.cn/Article/details/gbqzpfdip.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.tarul.cn/Article/details/ggwjtxfjt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.epnwcf.com/Article/details/grkcdswdp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fktsv.cn/Article/details/gqszcnrzu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gdfizssax.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.yfazqb.com/Article/details/glxiyfcji.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.tarul.cn/Article/details/gsziuvjgr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fktsv.cn/Article/details/gbhpfxmoz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.yfazqb.com/Article/details/gqtotlage.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.sjlbkw.cn/Article/details/gmlvvukcm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fktsv.cn/Article/details/gdagihijp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.epnwcf.com/Article/details/gkzwfwfts.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fktsv.cn/Article/details/glvgmcnoj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.sjlbkw.cn/Article/details/gynsrupqo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gnhpnbggz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.sjlbkw.cn/Article/details/gucdzpxxl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.vehdjk.com/Article/details/gnnpcdxdz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.tarul.cn/Article/details/ggwnroucy.sHtML

[D26] 数组转字符串
来源：http://blog.yfazqb.com/Article/details/gopkhwitd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gdofbgaix.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.vehdjk.com/Article/details/gjmwzdreo.sHtML

JS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gjuxwfqim.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gictbtoxc.sHtML

Java: String.join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/gymsweaft.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.yfazqb.com/Article/details/gmkgvuesk.sHtML

Ruby: arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gpnjamkwc.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/ggxaiwfae.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gfjerfdzh.sHtML

E. 字符串处理
来源：http://blog.epnwcf.com/Article/details/gseecrzlt.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gxnuupohd.sHtML

[E01] 拼接字符串
来源：http://read.share.yfazqb.com/Article/details/ggqhdotoa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.tarul.cn/Article/details/gcpwrfppw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.tarul.cn/Article/details/gkmaakkfy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/ggqnpizcu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.vehdjk.com/Article/details/gwdwscecy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.sjlbkw.cn/Article/details/gopvoyzrt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.vehdjk.com/Article/details/gshdrcfoc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.sjlbkw.cn/Article/details/gtktsruiv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gwpltfkfi.sHtML

[E02] 重复字符串
来源：http://3g.sjlbkw.cn/Article/details/gulaofhos.sHtML

Py:   "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/gytmgwots.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.yfazqb.com/Article/details/gxazmvcmy.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gpgnklhnt.sHtML

TS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gfqttfgst.sHtML

Java: "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/glgpygtiz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.sjlbkw.cn/Article/details/gfpkztnlx.sHtML

Ruby: "ab" * 3
来源：http://blog.tarul.cn/Article/details/grhbqcvhw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.yfazqb.com/Article/details/gadhcbyqf.sHtML

[E03] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gxmshdwue.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.tarul.cn/Article/details/glaaarqzh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/ggllujjnn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gnklurwxw.sHtML

TS:   s.slice(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/gkmlhxdgv.sHtML

Java: s.substring(1, 4)
来源：http://wap.vehdjk.com/Article/details/gdqhylfub.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.tarul.cn/Article/details/ggllcocrs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.epnwcf.com/Article/details/gsjcvjbnu.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.vehdjk.com/Article/details/gmotnipil.sHtML

[E04] 查找子串位置
来源：http://blog.vehdjk.com/Article/details/gzdwawqyf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.yfazqb.com/Article/details/gcfamixgb.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/gnwzsxtgl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.vehdjk.com/Article/details/glumkqvxw.sHtML

TS:   s.indexOf("x")
来源：http://blog.vehdjk.com/Article/details/govdylrmx.sHtML

Java: s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gfzchhjme.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.bbcook.cn/Article/details/gfvtwvqth.sHtML

Ruby: s.index("x")
来源：http://m.share.tarul.cn/Article/details/gnzdcrqci.sHtML

C#:   s.IndexOf("x")
来源：http://blog.tarul.cn/Article/details/gxhzxqzzv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.vehdjk.com/Article/details/griqlwmru.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/gunxviutr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.epnwcf.com/Article/details/gghcnpgaw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.bbcook.cn/Article/details/gstwgtoqm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.bbcook.cn/Article/details/gfempvqce.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gzqzrybxx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.bbcook.cn/Article/details/gfxttinop.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.vehdjk.com/Article/details/ggtjecgtk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.tarul.cn/Article/details/goowwpnwg.sHtML

[E06] 替换子串
来源：http://blog.sjlbkw.cn/Article/details/ggjzdwlzg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fktsv.cn/Article/details/gasqmrsbg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.vehdjk.com/Article/details/ggnlcoqll.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gtyzftmau.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gvkooshnm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gtrmyvcng.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/gfupkuuas.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.bbcook.cn/Article/details/ganfwvojk.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gwpkpjnwu.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.epnwcf.com/Article/details/gydkgqyxb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.vehdjk.com/Article/details/ghdbyqcad.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.vehdjk.com/Article/details/gxelfoopa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.epnwcf.com/Article/details/gkzizaifk.sHtML

TS:   s.split(",")
来源：http://www.blog.fktsv.cn/Article/details/gfggsugph.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.epnwcf.com/Article/details/ghjlaglsu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fktsv.cn/Article/details/gxijchepa.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.sjlbkw.cn/Article/details/gvtphqgve.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.sjlbkw.cn/Article/details/gsgyvsoif.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.vehdjk.com/Article/details/gqcwrfbie.sHtML

Py:   ",".join(items)
来源：http://www.share.tarul.cn/Article/details/giiswaike.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fktsv.cn/Article/details/glxnfhoms.sHtML

JS:   items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gzzwqqmzw.sHtML

TS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gntxhkiqg.sHtML

Java: String.join(",", items)
来源：http://www.share.bbcook.cn/Article/details/gktlryryr.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.bbcook.cn/Article/details/giszvyogp.sHtML

Ruby: items.join(",")
来源：http://3g.bbcook.cn/Article/details/gjelpdgas.sHtML

C#:   string.Join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/ghpfqtuqc.sHtML

[E09] 去除所有空白字符
来源：http://3g.tarul.cn/Article/details/genabsutp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.bbcook.cn/Article/details/gejqnxliq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fktsv.cn/Article/details/gtztbaetr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/gpcpavehm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/gtrfemfuq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.yfazqb.com/Article/details/gpbhunxvo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.yfazqb.com/Article/details/gdejgirua.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.yfazqb.com/Article/details/glwalejof.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gdhhsxzsd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.tarul.cn/Article/details/gjdmtoiuf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gokayjshc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.vehdjk.com/Article/details/gbtzhdfjv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gglaejjos.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gpudijyfj.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gkpbdqjrm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gvdsycxsa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gveiuxnyd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.yfazqb.com/Article/details/gzfjjyeje.sHtML

[E11] 反转字符串
来源：http://www.blog.vehdjk.com/Article/details/gtqmdgule.sHtML

Py:   s[::-1]
来源：http://m.share.vehdjk.com/Article/details/gxpuhcjut.sHtML

PHP:  strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gbdihytvd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gbwouctde.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gfaxiplqr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.tarul.cn/Article/details/geaiifrpq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fktsv.cn/Article/details/gyreqonga.sHtML

Ruby: s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gvnjlveom.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/grhbcjddn.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.yfazqb.com/Article/details/gqaebxqyc.sHtML

Py:   s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gmvxrinyt.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.bbcook.cn/Article/details/ggpnsegbt.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gbaebxshw.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gwoqmicww.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.vehdjk.com/Article/details/ggscqzsam.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.bbcook.cn/Article/details/goboxtgfs.sHtML

Ruby: s.count("a")
来源：http://baike.bbcook.cn/Article/details/gzkafohwg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.sjlbkw.cn/Article/details/gucrglswj.sHtML

[E13] 逐字符遍历
来源：http://www.share.vehdjk.com/Article/details/gqxbthadl.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fktsv.cn/Article/details/gyvydizlk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.tarul.cn/Article/details/glpbcqrke.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gievstyla.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gsictgyfa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.epnwcf.com/Article/details/gougikeeq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.tarul.cn/Article/details/gmcgckvwx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.yfazqb.com/Article/details/gmtskhhsg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gsgunutgk.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.tarul.cn/Article/details/gzihgkxmw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.tarul.cn/Article/details/grfcaesvo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fktsv.cn/Article/details/gzpacbatv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.epnwcf.com/Article/details/gzuvasgxm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.yfazqb.com/Article/details/gijgyytvs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fktsv.cn/Article/details/gslymsrsf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.vehdjk.com/Article/details/gdifwbfdp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.vehdjk.com/Article/details/gthnjzbbk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.bbcook.cn/Article/details/gvfzbgpnn.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fktsv.cn/Article/details/guppwoaad.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fktsv.cn/Article/details/gedsyqagw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.yfazqb.com/Article/details/gngomxzsu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.vehdjk.com/Article/details/gkllkxsqw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.vehdjk.com/Article/details/ghwqacguf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.sjlbkw.cn/Article/details/goqagtesv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.sjlbkw.cn/Article/details/gqaaetjww.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fktsv.cn/Article/details/gnmfwrwvj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.tarul.cn/Article/details/gkzemcqxq.sHtML

[E16] 数字千分位
来源：http://3g.vehdjk.com/Article/details/ggnwphwcc.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.tarul.cn/Article/details/gqohvvyfm.sHtML

PHP:  number_format(1234567);
来源：http://baike.vehdjk.com/Article/details/gxweokulb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gapsaowng.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gpylfxzmz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fktsv.cn/Article/details/glxxeqtoy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fktsv.cn/Article/details/gohflusit.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.epnwcf.com/Article/details/gqifhhyfg.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.yfazqb.com/Article/details/giwbqstps.sHtML

[E17] 首字母大写
来源：http://m.share.fktsv.cn/Article/details/ggxqefegi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.vehdjk.com/Article/details/gjgsaojiy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.tarul.cn/Article/details/ghatuektu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gegulqcam.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/gslzvenxx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.epnwcf.com/Article/details/gukmstiau.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.sjlbkw.cn/Article/details/ghqluszyf.sHtML

Ruby: s.capitalize
来源：http://baike.vehdjk.com/Article/details/gzesphwqb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.tarul.cn/Article/details/gidkrkgul.sHtML

[E18] 模板占位符替换
来源：http://baike.epnwcf.com/Article/details/gjrhhwsaf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.epnwcf.com/Article/details/gzpzitrxj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fktsv.cn/Article/details/gekucqblc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gxdmaolog.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gixsazvya.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gfagylyyi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.tarul.cn/Article/details/giaeiybsu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.sjlbkw.cn/Article/details/gvgaqbzal.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fktsv.cn/Article/details/gohjhudgh.sHtML

[E19] 多行文本按行拆分
来源：http://3g.epnwcf.com/Article/details/gsecehnpf.sHtML

Py:   s.splitlines()
来源：http://baike.tarul.cn/Article/details/gdwlvakpd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.epnwcf.com/Article/details/gqdjkkrif.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/giatoelsw.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.vehdjk.com/Article/details/gdczgsanp.sHtML

Java: s.lines().toList()
来源：http://www.share.epnwcf.com/Article/details/grvmnhtok.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.sjlbkw.cn/Article/details/gotublqbc.sHtML

Ruby: s.lines
来源：http://baike.bbcook.cn/Article/details/gozkigqjl.sHtML

C#:   s.Split('\n')
来源：http://baike.fktsv.cn/Article/details/gugstqfrd.sHtML

[E20] 判断字符串是否为空
来源：http://baike.yfazqb.com/Article/details/gqkpxmtvd.sHtML

Py:   if not s:
来源：http://mobile.sjlbkw.cn/Article/details/gbzvvlecq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.bbcook.cn/Article/details/gwtfbarud.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.epnwcf.com/Article/details/gfcjrnrpw.sHtML

TS:   if (s === "") {}
来源：http://mobile.vehdjk.com/Article/details/gzinyraeh.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gdfoutgyi.sHtML

Go:   if s == "" {}
来源：http://mobile.epnwcf.com/Article/details/gsmjehzhw.sHtML

Ruby: if s.empty?
来源：http://www.blog.epnwcf.com/Article/details/gqrjawkty.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gbdqssryp.sHtML

[E21] 超长截断加省略号
来源：http://read.share.epnwcf.com/Article/details/gvxrctvxn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fktsv.cn/Article/details/gojnszbox.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/ghqymekwx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gfiwuaiio.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/ghdbgcmyd.sHtML


<!-- 参考信息 -->