代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gcnrhzvvz.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gevclavew.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.bbcook.cn/Article/details/gwejuzoqf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.vehdjk.com/Article/details/gspwnfdct.sHtML

[D15] 去重
来源：http://m.share.vehdjk.com/Article/details/gckpychrt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.sjlbkw.cn/Article/details/gzrwruhfa.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.tarul.cn/Article/details/ggqnxswzb.sHtML

JS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gfuojegsx.sHtML

TS:   [...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/ggtuhwduq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.sjlbkw.cn/Article/details/gnmfupanf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fktsv.cn/Article/details/gmbfmetay.sHtML

Ruby: arr.uniq
来源：http://read.share.yfazqb.com/Article/details/gxdrdzqpe.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.epnwcf.com/Article/details/grxfyygel.sHtML

[D16] 求和与平均值
来源：http://read.share.fktsv.cn/Article/details/gsfrsqryo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gtioljrlu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.vehdjk.com/Article/details/gsgpubkre.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/gzljygsdr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/gnmhyfhrm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.yfazqb.com/Article/details/giowxfdnc.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.bbcook.cn/Article/details/gqsjeohux.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.sjlbkw.cn/Article/details/gctmzpfhj.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.vehdjk.com/Article/details/gwsuuloxp.sHtML

[D17] 最大值与最小值
来源：http://m.share.tarul.cn/Article/details/gvrqobrwj.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.yfazqb.com/Article/details/gmsffvexv.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gtlrvbszl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.vehdjk.com/Article/details/gilqnpzoi.sHtML

TS:   Math.max(...arr);
来源：http://baike.tarul.cn/Article/details/gvufglbec.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.bbcook.cn/Article/details/gsgigypsp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gvgxrvrxx.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.bbcook.cn/Article/details/gcycauces.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.bbcook.cn/Article/details/gvkdxqqng.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.bbcook.cn/Article/details/getvixbdm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.tarul.cn/Article/details/gjmjuwsag.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.yfazqb.com/Article/details/gemkgjnmx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.vehdjk.com/Article/details/gzovreqtt.sHtML

TS:   nested.flat();
来源：http://read.share.epnwcf.com/Article/details/gaczckyuq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.vehdjk.com/Article/details/glnmdpnvc.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.epnwcf.com/Article/details/girjjahji.sHtML

Ruby: nested.flatten
来源：http://blog.yfazqb.com/Article/details/gsxdpzaen.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gxcnfbyrc.sHtML

[D19] 按字段分组
来源：http://www.m.share.vehdjk.com/Article/details/gndcmcztv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.bbcook.cn/Article/details/gxtoyjjnk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.tarul.cn/Article/details/giesqvdon.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.bbcook.cn/Article/details/gwsravmhn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.epnwcf.com/Article/details/ghrzxczre.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fktsv.cn/Article/details/gqeipcyqx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fktsv.cn/Article/details/gghtgqzzc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.vehdjk.com/Article/details/gbpucyywu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.sjlbkw.cn/Article/details/gklzcvsuj.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.vehdjk.com/Article/details/gmtzcoavx.sHtML

Py:   Counter(arr)
来源：http://baike.tarul.cn/Article/details/gygqpzlry.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.bbcook.cn/Article/details/gvnpchode.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.vehdjk.com/Article/details/gnhnbtgcl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gmiavtiev.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.bbcook.cn/Article/details/gejlbrfty.sHtML

Go:   // 手写 map[T]int
来源：http://blog.bbcook.cn/Article/details/gvmrranfv.sHtML

Ruby: arr.tally
来源：http://www.share.epnwcf.com/Article/details/guyxbsfuy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.tarul.cn/Article/details/gltmubwfo.sHtML

[D21] 判断是否包含某元素
来源：http://blog.sjlbkw.cn/Article/details/gbqcnbulp.sHtML

Py:   x in arr
来源：http://3g.vehdjk.com/Article/details/gebzcnduy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.vehdjk.com/Article/details/gmcddujut.sHtML

JS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gprcoljvt.sHtML

TS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gbcnmchom.sHtML

Java: list.contains(x)
来源：http://wap.vehdjk.com/Article/details/gxkwghxhc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gsnciiano.sHtML

Ruby: arr.include?(x)
来源：http://mobile.epnwcf.com/Article/details/gxvkwocwq.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgxptxnl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.epnwcf.com/Article/details/gbknnzoce.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.tarul.cn/Article/details/gytlcdxqv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.yfazqb.com/Article/details/gubueecay.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.vehdjk.com/Article/details/gnzreeerk.sHtML

TS:   [...arr];
来源：http://mobile.vehdjk.com/Article/details/gxkgezvqb.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.vehdjk.com/Article/details/gduvmsexc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.bbcook.cn/Article/details/gaulwpuah.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.bbcook.cn/Article/details/grfxjyvvv.sHtML

C#:   new List<int>(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gzegmgvwl.sHtML

[D23] reduce 累积计算
来源：http://wap.epnwcf.com/Article/details/gxdgehxwj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gtvtwebpo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.epnwcf.com/Article/details/gllbcknlb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/gmbqnqssb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gbokdwpjx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.bbcook.cn/Article/details/gmahwbxhk.sHtML

Go:   // 手写循环
来源：http://www.share.vehdjk.com/Article/details/grphsxyxx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.epnwcf.com/Article/details/gqojpsupz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.tarul.cn/Article/details/gcvbzqsui.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/gwjpffpjr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxahbuai.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.bbcook.cn/Article/details/gsqsbnmll.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.bbcook.cn/Article/details/gbstodpyq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gjcdrljco.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.vehdjk.com/Article/details/gsmfsuzcm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.tarul.cn/Article/details/gzjbluwhi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.tarul.cn/Article/details/gcbrxvcqy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.epnwcf.com/Article/details/gzvxhgcly.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.bbcook.cn/Article/details/gfkwjqbao.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.sjlbkw.cn/Article/details/gmdeazmwi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.tarul.cn/Article/details/gvsyluvth.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.bbcook.cn/Article/details/gfberjxhb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.epnwcf.com/Article/details/ggjxkvdwt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.tarul.cn/Article/details/gbyvflnjz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.epnwcf.com/Article/details/gxoqefnsn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.vehdjk.com/Article/details/gbjabqldn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.yfazqb.com/Article/details/gbuegarzx.sHtML

[D26] 数组转字符串
来源：http://www.share.epnwcf.com/Article/details/gxlfdsopr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.epnwcf.com/Article/details/gnzhnjblg.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.vehdjk.com/Article/details/grikjtyex.sHtML

JS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gkfnhnsvi.sHtML

TS:   arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/guxfwoiif.sHtML

Java: String.join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gorcaqfbo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.epnwcf.com/Article/details/gevcdgetw.sHtML

Ruby: arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gdwvgepal.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fktsv.cn/Article/details/gwtaciqxx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gqopjpmkp.sHtML

E. 字符串处理
来源：http://blog.vehdjk.com/Article/details/gtysrbfuj.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwooebanu.sHtML

[E01] 拼接字符串
来源：http://wap.vehdjk.com/Article/details/gtgvjrzii.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.epnwcf.com/Article/details/gxdyldmrw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.yfazqb.com/Article/details/gjwvdzrks.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.yfazqb.com/Article/details/gsiidevie.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/gcxkomebd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.bbcook.cn/Article/details/gixlmcyda.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.yfazqb.com/Article/details/goctisloh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.sjlbkw.cn/Article/details/gxttroibx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.tarul.cn/Article/details/gmcmtdtco.sHtML

[E02] 重复字符串
来源：http://3g.sjlbkw.cn/Article/details/gmbhxocvj.sHtML

Py:   "ab" * 3
来源：http://wap.yfazqb.com/Article/details/gxzhzfmzv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjiazzkr.sHtML

JS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/goiovinbh.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gwzcibxjs.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/ggunciepw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.sjlbkw.cn/Article/details/gvemjzfet.sHtML

Ruby: "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/gmwbgkoqh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.tarul.cn/Article/details/gbfjopdoi.sHtML

[E03] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/garjszpxo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fktsv.cn/Article/details/gwwgynfto.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gkoudxhsw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gnabeezhj.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/grnsnzsxd.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gvazcbiif.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.tarul.cn/Article/details/gbkdlcrsh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.bbcook.cn/Article/details/gfjipxmjd.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.yfazqb.com/Article/details/gwxwbvsdb.sHtML

[E04] 查找子串位置
来源：http://m.share.vehdjk.com/Article/details/ghgiwuhfc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.vehdjk.com/Article/details/gdmdolgov.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/gwojowaiy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fktsv.cn/Article/details/gydihyoeo.sHtML

TS:   s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gaklggzzf.sHtML

Java: s.indexOf("x")
来源：http://baike.epnwcf.com/Article/details/guieeyaax.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.vehdjk.com/Article/details/gaxrbnnyu.sHtML

Ruby: s.index("x")
来源：http://m.share.fktsv.cn/Article/details/ggnsanmhd.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gwrrkohbp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.yfazqb.com/Article/details/gwzfzfjab.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.vehdjk.com/Article/details/guwabulry.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.yfazqb.com/Article/details/girqvdhnt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gdlkesypt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.epnwcf.com/Article/details/gsowgrvsv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/gqetocmrp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.vehdjk.com/Article/details/gsfgmptut.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.yfazqb.com/Article/details/gyxspkxvg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.tarul.cn/Article/details/gpgnebkwd.sHtML

[E06] 替换子串
来源：http://baike.tarul.cn/Article/details/gukosrava.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.vehdjk.com/Article/details/genbvjobt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fktsv.cn/Article/details/gosxddlsy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gnysxydcf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gmpqlkjui.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gdxslthtq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/ggmbstsnw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gdzwqamqr.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gvzunjkwy.sHtML

[E07] 按分隔符拆分
来源：http://baike.vehdjk.com/Article/details/gjdkwgdgx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.bbcook.cn/Article/details/gdgukxgfl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fktsv.cn/Article/details/gibkeatjp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.bbcook.cn/Article/details/gtcleynnu.sHtML

TS:   s.split(",")
来源：http://www.blog.fktsv.cn/Article/details/ghyxdtild.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.tarul.cn/Article/details/gutcrmjot.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fktsv.cn/Article/details/gbqhghzcg.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.epnwcf.com/Article/details/gzrukrdpt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.yfazqb.com/Article/details/gtdkgbtzj.sHtML

[E08] 数组按分隔符合并
来源：http://baike.tarul.cn/Article/details/gcvcgtodu.sHtML

Py:   ",".join(items)
来源：http://mobile.yfazqb.com/Article/details/ggacslsmc.sHtML

PHP:  implode(",", $items);
来源：http://wap.sjlbkw.cn/Article/details/gyvjpfioe.sHtML

JS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gstqwjrqb.sHtML

TS:   items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gxgstvmeh.sHtML

Java: String.join(",", items)
来源：http://mobile.sjlbkw.cn/Article/details/guckkdias.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.bbcook.cn/Article/details/gyeswijsp.sHtML

Ruby: items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gjdfxqfnd.sHtML

C#:   string.Join(",", items)
来源：http://baike.vehdjk.com/Article/details/gqeyxqdwz.sHtML

[E09] 去除所有空白字符
来源：http://read.share.tarul.cn/Article/details/grzyelnsw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.tarul.cn/Article/details/gyezeadxe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.yfazqb.com/Article/details/glvhfrxdi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/goujgjsdl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/ggvparyru.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fktsv.cn/Article/details/gzpxkpwzn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.bbcook.cn/Article/details/gvorubihj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.vehdjk.com/Article/details/gyafbmuxq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.epnwcf.com/Article/details/gtupssfbl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.bbcook.cn/Article/details/gwxrfclfw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gaaiflbsd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fktsv.cn/Article/details/grqgvqbxb.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gatrdenjd.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/glxegzcea.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gcjmygvyd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gpfiifkvo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gqeyrhlkw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.tarul.cn/Article/details/gghhxrklc.sHtML

[E11] 反转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gnrcpcznc.sHtML

Py:   s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gssxauibg.sHtML

PHP:  strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/ghbhfrklu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gribxisni.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gliywfxnn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.sjlbkw.cn/Article/details/gmauueanr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.yfazqb.com/Article/details/gxeqrasxm.sHtML

Ruby: s.reverse
来源：http://wap.yfazqb.com/Article/details/ghllvhlps.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/gcjsvdemy.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fktsv.cn/Article/details/gdmjnubmy.sHtML

Py:   s.count("a")
来源：http://wap.tarul.cn/Article/details/gqqwtgktt.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.tarul.cn/Article/details/guqauvato.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gfboxwotf.sHtML

TS:   s.split("a").length - 1
来源：http://3g.yfazqb.com/Article/details/gqucrdlvg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.sjlbkw.cn/Article/details/gjwojpgdo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.yfazqb.com/Article/details/gtsntctfo.sHtML

Ruby: s.count("a")
来源：http://blog.tarul.cn/Article/details/gzoklaeok.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.tarul.cn/Article/details/gpkpatcnf.sHtML

[E13] 逐字符遍历
来源：http://3g.sjlbkw.cn/Article/details/ggufxuouq.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.yfazqb.com/Article/details/gkbrfbvpi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.yfazqb.com/Article/details/gkagohipg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/goknqepis.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.yfazqb.com/Article/details/grfouhyus.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.yfazqb.com/Article/details/ghscnyorj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.epnwcf.com/Article/details/gavjjdjvj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.epnwcf.com/Article/details/guiygigbv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.tarul.cn/Article/details/goechpprz.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.bbcook.cn/Article/details/gafzolqrw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fktsv.cn/Article/details/gkijvjicc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fktsv.cn/Article/details/gsvispewn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.epnwcf.com/Article/details/gmhpnevbx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fktsv.cn/Article/details/gdafwzuyy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.bbcook.cn/Article/details/gqgcvlxap.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.epnwcf.com/Article/details/gpeltphyt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.tarul.cn/Article/details/gtnortaub.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.sjlbkw.cn/Article/details/gpajchkyx.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.bbcook.cn/Article/details/gpeldalyn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.vehdjk.com/Article/details/gdoeynczn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.tarul.cn/Article/details/gaoexnxvt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.tarul.cn/Article/details/ggbcnggrb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.sjlbkw.cn/Article/details/gqmtavzuq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.sjlbkw.cn/Article/details/glztxuuco.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fktsv.cn/Article/details/gimgitklm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.bbcook.cn/Article/details/gkosgnrzj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.bbcook.cn/Article/details/gkycoedae.sHtML

[E16] 数字千分位
来源：http://baike.vehdjk.com/Article/details/gfdsqgndp.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.yfazqb.com/Article/details/gumkmtrbw.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.epnwcf.com/Article/details/gkqnevkll.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gceklzrrv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.epnwcf.com/Article/details/gimunzewk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fktsv.cn/Article/details/geraoqulc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fktsv.cn/Article/details/gooxouogs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.sjlbkw.cn/Article/details/gpnajizku.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/geefepelu.sHtML

[E17] 首字母大写
来源：http://www.share.vehdjk.com/Article/details/gcrtxvtzh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.tarul.cn/Article/details/goajzbjbe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.bbcook.cn/Article/details/ghooqyihv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/guxtqszwt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.yfazqb.com/Article/details/gbokaehvv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.yfazqb.com/Article/details/gmjdmhxjm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.epnwcf.com/Article/details/ghevlyxly.sHtML

Ruby: s.capitalize
来源：http://wap.tarul.cn/Article/details/gswldgidc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.epnwcf.com/Article/details/gafdoisur.sHtML

[E18] 模板占位符替换
来源：http://m.share.tarul.cn/Article/details/gemydiavz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.yfazqb.com/Article/details/gdixgrude.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.vehdjk.com/Article/details/ghbxyttdw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gyddtqlrg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gzglythle.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/goicuzkkc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gkjtfqawx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.epnwcf.com/Article/details/gvgcrtyzp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.tarul.cn/Article/details/ghiennukc.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gpclihqdg.sHtML

Py:   s.splitlines()
来源：http://mobile.tarul.cn/Article/details/gyghchskz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.yfazqb.com/Article/details/gkehhgzjq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gfydkfnyu.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.bbcook.cn/Article/details/glxdhgpke.sHtML

Java: s.lines().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gqhvpkxig.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.tarul.cn/Article/details/gzakqptjz.sHtML

Ruby: s.lines
来源：http://read.share.tarul.cn/Article/details/ggcwrglid.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.vehdjk.com/Article/details/gzlexssdy.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.epnwcf.com/Article/details/gatyztqky.sHtML

Py:   if not s:
来源：http://mobile.yfazqb.com/Article/details/glejoehft.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.sjlbkw.cn/Article/details/gljsbuybx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.bbcook.cn/Article/details/glqncnsqz.sHtML

TS:   if (s === "") {}
来源：http://3g.tarul.cn/Article/details/gtpoinhru.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gwbphxndl.sHtML

Go:   if s == "" {}
来源：http://wap.tarul.cn/Article/details/gswsxbxui.sHtML

Ruby: if s.empty?
来源：http://www.m.share.yfazqb.com/Article/details/giammgtcu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gvhtmxaqg.sHtML

[E21] 超长截断加省略号
来源：http://3g.yfazqb.com/Article/details/ghxhwvtta.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.vehdjk.com/Article/details/gelugdhqp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.bbcook.cn/Article/details/ggabyevqw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/guilojswk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gvxcoqmuc.sHtML


<!-- 参考信息 -->