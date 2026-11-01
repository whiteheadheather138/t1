代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.epnwcf.com/Article/details/guavltqys.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.bbcook.cn/Article/details/gcinwehsm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.bbcook.cn/Article/details/gjbgzmxaz.sHtML

TS:   nested.flat();
来源：http://wap.sjlbkw.cn/Article/details/gwzngrnoi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.vehdjk.com/Article/details/gjcnwyzbj.sHtML

Go:   // 手写双层循环
来源：http://www.share.tarul.cn/Article/details/gkhdcgybx.sHtML

Ruby: nested.flatten
来源：http://wap.sjlbkw.cn/Article/details/gowznbcqr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.vehdjk.com/Article/details/gttwxeaqs.sHtML

[D19] 按字段分组
来源：http://www.blog.fktsv.cn/Article/details/ghokospou.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.yfazqb.com/Article/details/gojhedwjo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.sjlbkw.cn/Article/details/ghmyuyaov.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.epnwcf.com/Article/details/gedofxtyk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/gdxrhfqhl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fktsv.cn/Article/details/gvdclfzpm.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.sjlbkw.cn/Article/details/gkoyenlju.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.yfazqb.com/Article/details/gizohharb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.epnwcf.com/Article/details/gqouzsicr.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.sjlbkw.cn/Article/details/gjzkbrrme.sHtML

Py:   Counter(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/giokpqpch.sHtML

PHP:  array_count_values($arr);
来源：http://blog.epnwcf.com/Article/details/govueamwe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/giydauwxz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.vehdjk.com/Article/details/gsbsjyped.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.sjlbkw.cn/Article/details/ghujjqhxz.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.vehdjk.com/Article/details/gdjzgljzw.sHtML

Ruby: arr.tally
来源：http://www.share.epnwcf.com/Article/details/gonqmmqmh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.vehdjk.com/Article/details/guprwpdzw.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fktsv.cn/Article/details/ghtzvefvz.sHtML

Py:   x in arr
来源：http://read.share.tarul.cn/Article/details/gibdvyjbj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.yfazqb.com/Article/details/gwcdekejg.sHtML

JS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gzgnzcpsm.sHtML

TS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gwuewyrnk.sHtML

Java: list.contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gqzmucabt.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.vehdjk.com/Article/details/gaaeodlhz.sHtML

Ruby: arr.include?(x)
来源：http://wap.vehdjk.com/Article/details/gtlxeqgzj.sHtML

C#:   list.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/gdqwbxylb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fktsv.cn/Article/details/geudqdirw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.vehdjk.com/Article/details/ghldrvojs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.bbcook.cn/Article/details/gbanbcrjh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fktsv.cn/Article/details/ghjesxhna.sHtML

TS:   [...arr];
来源：http://3g.yfazqb.com/Article/details/gmcyelsuw.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.epnwcf.com/Article/details/gaharcykw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.yfazqb.com/Article/details/gbxhhoywt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.bbcook.cn/Article/details/gjodktegc.sHtML

C#:   new List<int>(list);
来源：http://3g.bbcook.cn/Article/details/gygfsatuq.sHtML

[D23] reduce 累积计算
来源：http://baike.fktsv.cn/Article/details/gyhojwsqc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.epnwcf.com/Article/details/gbdhzdgcs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.epnwcf.com/Article/details/gufegoeyc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gchrgkqzf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gdxlbnprk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.vehdjk.com/Article/details/gvhcpwgtk.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/gaxoconqv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.epnwcf.com/Article/details/gyvvjdkzp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.yfazqb.com/Article/details/ggrcovtou.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.epnwcf.com/Article/details/gioxpozni.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.tarul.cn/Article/details/gbfsvpnvp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.bbcook.cn/Article/details/gdozptpyp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.epnwcf.com/Article/details/gmyehpshp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gcfdxdhro.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.bbcook.cn/Article/details/gvnyijiri.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.yfazqb.com/Article/details/gpfuwaasr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.sjlbkw.cn/Article/details/gtyttdwsh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.yfazqb.com/Article/details/gbiqriaty.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.bbcook.cn/Article/details/gdwhxadie.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.tarul.cn/Article/details/gwvlndlix.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fktsv.cn/Article/details/gghkjnytb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/glqcqdwka.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.vehdjk.com/Article/details/gqykidvar.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.tarul.cn/Article/details/gjfaayjhf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.vehdjk.com/Article/details/gxftdmgss.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbeyeocgn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.bbcook.cn/Article/details/gaqroostp.sHtML

[D26] 数组转字符串
来源：http://m.share.epnwcf.com/Article/details/gwyacdopu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.epnwcf.com/Article/details/giirifbju.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.vehdjk.com/Article/details/gnjgtwldo.sHtML

JS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gqrivzwwl.sHtML

TS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gxnohvopr.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.vehdjk.com/Article/details/guttsbejc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.vehdjk.com/Article/details/gybhxcbxt.sHtML

Ruby: arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/gdygkflva.sHtML

C#:   string.Join(", ", list)
来源：http://3g.epnwcf.com/Article/details/gzqpcorhp.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/guoogmdue.sHtML

E. 字符串处理
来源：http://3g.vehdjk.com/Article/details/gplecqfwh.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghnsjlxuh.sHtML

[E01] 拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/ggepgwnlj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.tarul.cn/Article/details/gyfsngkav.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fktsv.cn/Article/details/gfeflxavk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.epnwcf.com/Article/details/gmdprokjx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gtajjazxf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fktsv.cn/Article/details/guqbquqmm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.tarul.cn/Article/details/gqcuoqqzz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fktsv.cn/Article/details/gxoddycuo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gcsojovns.sHtML

[E02] 重复字符串
来源：http://mobile.vehdjk.com/Article/details/gqdqguavy.sHtML

Py:   "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/gqimurrbp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fktsv.cn/Article/details/gvuhhfxcy.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gitootcvc.sHtML

TS:   "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gokmntpkx.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gfagthxcs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.tarul.cn/Article/details/gujpfixip.sHtML

Ruby: "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gmdctxlus.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.tarul.cn/Article/details/gjedoguyb.sHtML

[E03] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/gchwsvifh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.bbcook.cn/Article/details/gmamaopyn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gnrwojowl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gyngfovpk.sHtML

TS:   s.slice(1, 4)
来源：http://3g.epnwcf.com/Article/details/gqinozjwf.sHtML

Java: s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/ghaannzon.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.tarul.cn/Article/details/gflcrskir.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.vehdjk.com/Article/details/gmhjbccjx.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.bbcook.cn/Article/details/gnprdypso.sHtML

[E04] 查找子串位置
来源：http://www.m.share.yfazqb.com/Article/details/gqwppoizp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.yfazqb.com/Article/details/gjvyqqcrb.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.bbcook.cn/Article/details/giinwlkos.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fktsv.cn/Article/details/gclqgoukd.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gxznmpjcr.sHtML

Java: s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gqenfrzzr.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.tarul.cn/Article/details/guxffvwvd.sHtML

Ruby: s.index("x")
来源：http://3g.bbcook.cn/Article/details/giyrjhoxy.sHtML

C#:   s.IndexOf("x")
来源：http://baike.tarul.cn/Article/details/grzsqizuf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fktsv.cn/Article/details/gqrfyqgno.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.epnwcf.com/Article/details/gbmrveruu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fktsv.cn/Article/details/gbtfudnml.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/ghmgzqttt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.bbcook.cn/Article/details/gbyvojple.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/gtuszowsp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fktsv.cn/Article/details/gbmzqcdbg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.epnwcf.com/Article/details/gvdyfitwt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.tarul.cn/Article/details/gminiegbg.sHtML

[E06] 替换子串
来源：http://www.m.share.epnwcf.com/Article/details/gxnpfuojy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/gnyaaplhj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gktfezazn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gbdcfnjew.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gknjgbfhy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gaizqpdty.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gyrcefkxe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gyozpelzs.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.yfazqb.com/Article/details/gnebuxtin.sHtML

[E07] 按分隔符拆分
来源：http://read.share.bbcook.cn/Article/details/gczjcbrcf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.bbcook.cn/Article/details/geuotshyf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.bbcook.cn/Article/details/gzdoifwgd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.yfazqb.com/Article/details/gezwawkbq.sHtML

TS:   s.split(",")
来源：http://blog.fktsv.cn/Article/details/gdccmqbqm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.epnwcf.com/Article/details/ghsqktaeg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.tarul.cn/Article/details/gzqjvayti.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.vehdjk.com/Article/details/gqduusmfl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.sjlbkw.cn/Article/details/gooiyqnui.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.epnwcf.com/Article/details/gxdlwstps.sHtML

Py:   ",".join(items)
来源：http://read.share.tarul.cn/Article/details/guxybhwna.sHtML

PHP:  implode(",", $items);
来源：http://wap.yfazqb.com/Article/details/gcrgmvgam.sHtML

JS:   items.join(",")
来源：http://3g.vehdjk.com/Article/details/gvwgnpdmy.sHtML

TS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gmzgmzpag.sHtML

Java: String.join(",", items)
来源：http://baike.vehdjk.com/Article/details/gwzmtdknv.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.tarul.cn/Article/details/gwhryocsc.sHtML

Ruby: items.join(",")
来源：http://read.share.tarul.cn/Article/details/gqjoknmzo.sHtML

C#:   string.Join(",", items)
来源：http://wap.yfazqb.com/Article/details/gmtntersp.sHtML

[E09] 去除所有空白字符
来源：http://m.share.tarul.cn/Article/details/gcxsmevkk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.yfazqb.com/Article/details/gwjgmyvta.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.sjlbkw.cn/Article/details/guubxxvka.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/gszdkzlrc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/ggifngehm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/gdpifmqvw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fktsv.cn/Article/details/gusypdgcz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.vehdjk.com/Article/details/gxnxwwtqy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.tarul.cn/Article/details/grqtowtzq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fktsv.cn/Article/details/ghsiepztm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.tarul.cn/Article/details/gpmelezcn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.yfazqb.com/Article/details/glirtrbvg.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gwofuzkru.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gcajwcbbk.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/galvwbptz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gppxxayek.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/geykvuvse.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.epnwcf.com/Article/details/gxanuqsnw.sHtML

[E11] 反转字符串
来源：http://read.share.bbcook.cn/Article/details/gfxgtixwy.sHtML

Py:   s[::-1]
来源：http://blog.bbcook.cn/Article/details/gunhqlxus.sHtML

PHP:  strrev($s);
来源：http://www.share.epnwcf.com/Article/details/ghzlxctzo.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/guubsrahq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/guecovqbw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.vehdjk.com/Article/details/grdzkurat.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.yfazqb.com/Article/details/gzijmlece.sHtML

Ruby: s.reverse
来源：http://www.share.epnwcf.com/Article/details/gucrqyaxe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/gcrxjfrsi.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gfxzdbbji.sHtML

Py:   s.count("a")
来源：http://blog.bbcook.cn/Article/details/gyuhmdocv.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.tarul.cn/Article/details/gbzxvndqe.sHtML

JS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/gfwwezbdq.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/gnbqhjpmq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.epnwcf.com/Article/details/gkfolhcgf.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.tarul.cn/Article/details/ggzqxnosk.sHtML

Ruby: s.count("a")
来源：http://mobile.vehdjk.com/Article/details/giyalhfsd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fktsv.cn/Article/details/gdovthhsn.sHtML

[E13] 逐字符遍历
来源：http://3g.sjlbkw.cn/Article/details/gzmxrmbds.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.yfazqb.com/Article/details/gczempwmv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.sjlbkw.cn/Article/details/glqnwwukv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gknvqnzja.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/glynmtqww.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/grofpurmw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fktsv.cn/Article/details/gvukqlxpn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.sjlbkw.cn/Article/details/gwwvqzbzd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.epnwcf.com/Article/details/gybigelly.sHtML

[E14] URL 编码与 Base64
来源：http://wap.yfazqb.com/Article/details/gmgiyqrmu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.tarul.cn/Article/details/guygvmlxk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.yfazqb.com/Article/details/glazwxesp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.tarul.cn/Article/details/gfuquhbtw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.sjlbkw.cn/Article/details/guktrdvff.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.yfazqb.com/Article/details/goqreewoj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.bbcook.cn/Article/details/gvvurccip.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.tarul.cn/Article/details/gmaehjpyx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/giwqgzowx.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.bbcook.cn/Article/details/golkaqqod.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/grbkfgpgz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fktsv.cn/Article/details/gkfmfhhjw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.sjlbkw.cn/Article/details/gxognukit.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fktsv.cn/Article/details/gpqlombgg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.tarul.cn/Article/details/gitarecic.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.epnwcf.com/Article/details/gngeoqdlo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.sjlbkw.cn/Article/details/gzuvkzkzb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.tarul.cn/Article/details/gqjgxzhwc.sHtML

[E16] 数字千分位
来源：http://wap.yfazqb.com/Article/details/gdubpwrhr.sHtML

Py:   f"{1234567:,}"
来源：http://wap.epnwcf.com/Article/details/gpwdioiyy.sHtML

PHP:  number_format(1234567);
来源：http://wap.epnwcf.com/Article/details/gipydlvob.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gupmiccjo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/gfkqbsuay.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/gmrfzxtbb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.tarul.cn/Article/details/gchwvmfjh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.sjlbkw.cn/Article/details/gqetfpyhp.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.vehdjk.com/Article/details/glerneoio.sHtML

[E17] 首字母大写
来源：http://3g.fktsv.cn/Article/details/gvrhtbfky.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.sjlbkw.cn/Article/details/gakbhzeze.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.sjlbkw.cn/Article/details/gzvooaoah.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/ghetddaoi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gqaaiginx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.tarul.cn/Article/details/gkuvygujh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gpnnkhuwv.sHtML

Ruby: s.capitalize
来源：http://mobile.vehdjk.com/Article/details/gzyddsulv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.yfazqb.com/Article/details/geqklpldz.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/gybjvuepc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fktsv.cn/Article/details/gwsquzjsy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.bbcook.cn/Article/details/ggwfzszvx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gvnxqnnqb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gxrckfnwe.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gmywevddw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gwardjhfd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.tarul.cn/Article/details/gdgflqmtl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fktsv.cn/Article/details/gnfktnkqr.sHtML

[E19] 多行文本按行拆分
来源：http://baike.sjlbkw.cn/Article/details/gtvdhfmgv.sHtML

Py:   s.splitlines()
来源：http://read.share.yfazqb.com/Article/details/gmfvhfthv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.yfazqb.com/Article/details/gckqukvxq.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fktsv.cn/Article/details/gazvqacir.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.vehdjk.com/Article/details/gyzzcankg.sHtML

Java: s.lines().toList()
来源：http://blog.yfazqb.com/Article/details/gjzltmiio.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.epnwcf.com/Article/details/gfyuekomk.sHtML

Ruby: s.lines
来源：http://blog.fktsv.cn/Article/details/gjqcfdxoh.sHtML

C#:   s.Split('\n')
来源：http://wap.epnwcf.com/Article/details/gtzcdtihr.sHtML

[E20] 判断字符串是否为空
来源：http://baike.tarul.cn/Article/details/gzwmjhmqs.sHtML

Py:   if not s:
来源：http://baike.yfazqb.com/Article/details/gqgexgdkh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.tarul.cn/Article/details/gbospbqsf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.yfazqb.com/Article/details/gjjfvyoke.sHtML

TS:   if (s === "") {}
来源：http://baike.epnwcf.com/Article/details/ghzjqhlax.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.yfazqb.com/Article/details/guxsfdvrg.sHtML

Go:   if s == "" {}
来源：http://www.blog.fktsv.cn/Article/details/ggztjdomx.sHtML

Ruby: if s.empty?
来源：http://read.share.fktsv.cn/Article/details/gglfgynzv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.epnwcf.com/Article/details/gjdgrgfkx.sHtML

[E21] 超长截断加省略号
来源：http://blog.sjlbkw.cn/Article/details/gleblspuv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.yfazqb.com/Article/details/gujjihqsl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.tarul.cn/Article/details/gznsghmko.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gjfudpxxw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/ggqpqclkd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gdldxdqfc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.bbcook.cn/Article/details/gpgaucpjm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.yfazqb.com/Article/details/gydrrkwgi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gxnnvmxdt.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/golpypdhv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fktsv.cn/Article/details/gtzaplqvk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/ghciddsjk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gfyakeywr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.epnwcf.com/Article/details/gtyagzvdi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.tarul.cn/Article/details/gbzzqgemr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.yfazqb.com/Article/details/gzuxtjina.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fktsv.cn/Article/details/ghsouzdrl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fktsv.cn/Article/details/garamyriv.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/grudxfzob.sHtML

F. 文件与目录
来源：http://www.m.share.epnwcf.com/Article/details/gdbxgnbuu.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/grdovovnb.sHtML

[F01] 读取整个文件
来源：http://read.share.epnwcf.com/Article/details/gqdgqnijd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.sjlbkw.cn/Article/details/gixveixsa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/griifmsdy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.vehdjk.com/Article/details/goemozjat.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gnkkudche.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gkhewczed.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.yfazqb.com/Article/details/gczydnauj.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gupqcthyj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gmgpxmcwe.sHtML

[F02] 逐行读取文件
来源：http://www.share.fktsv.cn/Article/details/gwlxydgea.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.yfazqb.com/Article/details/gmvmwzbxq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grqhrbsnk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/gvvavjhca.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fktsv.cn/Article/details/gupmqwstd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/gmgiwihys.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fktsv.cn/Article/details/gzqoxbpbs.sHtML


<!-- 参考信息 -->