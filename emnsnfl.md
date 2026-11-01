代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.bbcook.cn/Article/details/gwpxqmxvu.sHtML

Go:   // 手写双层循环
来源：http://mobile.bbcook.cn/Article/details/gfaouvfjf.sHtML

Ruby: nested.flatten
来源：http://mobile.epnwcf.com/Article/details/gwckbwari.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/goqxmytao.sHtML

[D19] 按字段分组
来源：http://read.share.yfazqb.com/Article/details/guvqlflpl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.yfazqb.com/Article/details/gobrmykae.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.epnwcf.com/Article/details/ghuezdtlt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fktsv.cn/Article/details/gdvllnyzk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gmknnqxrl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.tarul.cn/Article/details/gjguariwm.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.yfazqb.com/Article/details/guanavltn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.yfazqb.com/Article/details/glqqnerph.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.epnwcf.com/Article/details/grsfhdtsz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.yfazqb.com/Article/details/gmwkhygkz.sHtML

Py:   Counter(arr)
来源：http://m.share.yfazqb.com/Article/details/gqqlbgraz.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.yfazqb.com/Article/details/ggyffddos.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fktsv.cn/Article/details/gndwslpvx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gdmnyvyuo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.yfazqb.com/Article/details/glxfwlrxn.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.bbcook.cn/Article/details/ghzcemmok.sHtML

Ruby: arr.tally
来源：http://mobile.tarul.cn/Article/details/gxpzcdnfx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.sjlbkw.cn/Article/details/gprsuigql.sHtML

[D21] 判断是否包含某元素
来源：http://3g.sjlbkw.cn/Article/details/glygnzrpv.sHtML

Py:   x in arr
来源：http://www.m.share.tarul.cn/Article/details/gidnazaqo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.epnwcf.com/Article/details/gmdkiflir.sHtML

JS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gsdcubidk.sHtML

TS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/gjmyzhouv.sHtML

Java: list.contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gllzkkjpb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gpdfaioyy.sHtML

Ruby: arr.include?(x)
来源：http://m.share.tarul.cn/Article/details/gmocfstnf.sHtML

C#:   list.Contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/ggbhktgkb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fktsv.cn/Article/details/ghkroidqr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fktsv.cn/Article/details/gzvdjucas.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.bbcook.cn/Article/details/grzermppc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.tarul.cn/Article/details/gbugmkfdp.sHtML

TS:   [...arr];
来源：http://m.share.fktsv.cn/Article/details/gllkxtwwa.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gzyncwkum.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.tarul.cn/Article/details/guponrvdo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.vehdjk.com/Article/details/gdmxgvfea.sHtML

C#:   new List<int>(list);
来源：http://blog.yfazqb.com/Article/details/ghlzbvokh.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmmgqsgf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.yfazqb.com/Article/details/gixjnjwtq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.yfazqb.com/Article/details/gowlxqskk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.sjlbkw.cn/Article/details/gogpybgkf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/gxmlneagi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.bbcook.cn/Article/details/gcmhjhgdy.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/geethmqjd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.bbcook.cn/Article/details/grwxjigxs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.bbcook.cn/Article/details/gdsxojtmb.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.epnwcf.com/Article/details/gzdcefvpe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.sjlbkw.cn/Article/details/gkplcbupi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.epnwcf.com/Article/details/gfdvhboup.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.yfazqb.com/Article/details/geyqfevqx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fktsv.cn/Article/details/geekqgots.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/gapzwkqtp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.tarul.cn/Article/details/gkftmcewq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.yfazqb.com/Article/details/gylzkoqcp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.yfazqb.com/Article/details/gchloxvcu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.bbcook.cn/Article/details/ggbpaddib.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.yfazqb.com/Article/details/glquzspbr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.tarul.cn/Article/details/gskgndacn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.epnwcf.com/Article/details/gpjvfewkx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.epnwcf.com/Article/details/giypsgbnw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.tarul.cn/Article/details/gkpnpjpum.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fktsv.cn/Article/details/gcupljkgl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.yfazqb.com/Article/details/gdekifomg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.epnwcf.com/Article/details/giavsekaq.sHtML

[D26] 数组转字符串
来源：http://mobile.vehdjk.com/Article/details/gnbvfecru.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.tarul.cn/Article/details/giafyvmbr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gvqyrdgsm.sHtML

JS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gyflntvcl.sHtML

TS:   arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gjlnlepqv.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/ggmejtxob.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.bbcook.cn/Article/details/gyjwzmmuw.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gkpgnzjmd.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/gqisgcpnq.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ghkvscbgk.sHtML

E. 字符串处理
来源：http://www.share.fktsv.cn/Article/details/guzgmkyxn.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/grjdijpnt.sHtML

[E01] 拼接字符串
来源：http://mobile.tarul.cn/Article/details/gxxpipdrc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.bbcook.cn/Article/details/gagamluxw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.yfazqb.com/Article/details/gnicauloz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/gvulxyuqf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gnwwrzaup.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.vehdjk.com/Article/details/ggvnqofoy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fktsv.cn/Article/details/gzahcjrsv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.tarul.cn/Article/details/gwenzbfan.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gkvtxgfim.sHtML

[E02] 重复字符串
来源：http://mobile.fktsv.cn/Article/details/grxeurdej.sHtML

Py:   "ab" * 3
来源：http://www.m.share.tarul.cn/Article/details/gabnvvjtv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fktsv.cn/Article/details/gzejafjss.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/ggwgarlbx.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gifcrhjsq.sHtML

Java: "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gbtgyuzse.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.tarul.cn/Article/details/gbcgfdijs.sHtML

Ruby: "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/ghjybzjwo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.sjlbkw.cn/Article/details/grgpbrous.sHtML

[E03] 截取子串
来源：http://3g.epnwcf.com/Article/details/gdvgtqrmu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.yfazqb.com/Article/details/grlngidda.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gqwltxzcr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gzkkfflwk.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.yfazqb.com/Article/details/grijqjdgx.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gkxhqzgyc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.vehdjk.com/Article/details/gdmmewpoi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.yfazqb.com/Article/details/gnhieljok.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.bbcook.cn/Article/details/gnbrnhnuv.sHtML

[E04] 查找子串位置
来源：http://www.m.share.bbcook.cn/Article/details/ghqvfnpoo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.bbcook.cn/Article/details/gnuaqjgrz.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.sjlbkw.cn/Article/details/gublkxvdp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.bbcook.cn/Article/details/gxepbgyix.sHtML

TS:   s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/geleazacw.sHtML

Java: s.indexOf("x")
来源：http://blog.bbcook.cn/Article/details/gktmeexrq.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.bbcook.cn/Article/details/gdxktngij.sHtML

Ruby: s.index("x")
来源：http://www.share.tarul.cn/Article/details/grualgbid.sHtML

C#:   s.IndexOf("x")
来源：http://3g.vehdjk.com/Article/details/gtsyolctt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.epnwcf.com/Article/details/glanufjqf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fktsv.cn/Article/details/gkigtghyp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.epnwcf.com/Article/details/gjwnotgjp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gdmmhtmdc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fktsv.cn/Article/details/gxphqxefh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/ghzljblss.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.yfazqb.com/Article/details/gvfmxvssp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.epnwcf.com/Article/details/gdbmocfzs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gtanlgsdd.sHtML

[E06] 替换子串
来源：http://m.share.vehdjk.com/Article/details/gxjhjlexh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/grhmhidre.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gbwrsxiin.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gwnzcnogt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gucbjprhd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gqufuvyhh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.yfazqb.com/Article/details/getkxoeam.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.vehdjk.com/Article/details/glunwtfcl.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gqzzwpcuf.sHtML

[E07] 按分隔符拆分
来源：http://mobile.epnwcf.com/Article/details/gmryyiuqv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.vehdjk.com/Article/details/gfkqsdgxn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.yfazqb.com/Article/details/gwkgzrmga.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.epnwcf.com/Article/details/gpwtlvlln.sHtML

TS:   s.split(",")
来源：http://mobile.tarul.cn/Article/details/gmkxrebfi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.bbcook.cn/Article/details/gxnevbuuq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.yfazqb.com/Article/details/glwxnvfzt.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.yfazqb.com/Article/details/gghlhcjuz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.vehdjk.com/Article/details/gepfpltft.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.vehdjk.com/Article/details/gplnsqrux.sHtML

Py:   ",".join(items)
来源：http://3g.epnwcf.com/Article/details/gpxhledle.sHtML

PHP:  implode(",", $items);
来源：http://3g.tarul.cn/Article/details/gvmdgbhwn.sHtML

JS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gtzrcmyyg.sHtML

TS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/gntwyotbf.sHtML

Java: String.join(",", items)
来源：http://blog.tarul.cn/Article/details/gmziaqypo.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.vehdjk.com/Article/details/gngcuxhhd.sHtML

Ruby: items.join(",")
来源：http://baike.fktsv.cn/Article/details/gxuwwayqb.sHtML

C#:   string.Join(",", items)
来源：http://read.share.yfazqb.com/Article/details/gixentdff.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.yfazqb.com/Article/details/gfovbslvt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.yfazqb.com/Article/details/grkneqjxc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.tarul.cn/Article/details/gynvjztmy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/gzmknusqp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.bbcook.cn/Article/details/glcizgere.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fktsv.cn/Article/details/gtjadinff.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.yfazqb.com/Article/details/gyoeryzby.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.epnwcf.com/Article/details/ggvtlhxua.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/gcxujalcu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fktsv.cn/Article/details/gttiptjpv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gtrsapsmw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.epnwcf.com/Article/details/gcjkwkpzk.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/ghqrzcihz.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gkswpalma.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gswsbpjui.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gezyhmgiw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gdqiapgjz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/gsnjrzgdt.sHtML

[E11] 反转字符串
来源：http://www.share.bbcook.cn/Article/details/gepdgdqsg.sHtML

Py:   s[::-1]
来源：http://baike.fktsv.cn/Article/details/ghsddguqv.sHtML

PHP:  strrev($s);
来源：http://3g.epnwcf.com/Article/details/geehwlqgf.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gxpxtytmz.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gsupjwwzc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gzkvcskcw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.sjlbkw.cn/Article/details/grlpdpgbi.sHtML

Ruby: s.reverse
来源：http://read.share.sjlbkw.cn/Article/details/gfervjjwm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gvvxpdbdq.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.sjlbkw.cn/Article/details/gzjyurvnc.sHtML

Py:   s.count("a")
来源：http://blog.yfazqb.com/Article/details/ggzntuqcd.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.vehdjk.com/Article/details/gtnsmpycc.sHtML

JS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/grlewewaj.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.vehdjk.com/Article/details/gxlfbbbgf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.yfazqb.com/Article/details/gwpucwwqp.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.tarul.cn/Article/details/gsybvavev.sHtML

Ruby: s.count("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwhxgmol.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.sjlbkw.cn/Article/details/gobjhhbph.sHtML

[E13] 逐字符遍历
来源：http://mobile.yfazqb.com/Article/details/gavrhpnlh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.tarul.cn/Article/details/gpbqcxnfk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.tarul.cn/Article/details/gvmkfzhjm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.tarul.cn/Article/details/gfuaoiecp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/gurajyywr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.bbcook.cn/Article/details/gauhafxim.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.vehdjk.com/Article/details/getltkmmd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.vehdjk.com/Article/details/glfkifrhn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fktsv.cn/Article/details/gdxriznpe.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.yfazqb.com/Article/details/gmwgbddqb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.yfazqb.com/Article/details/gyptebgps.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.tarul.cn/Article/details/gavixyrhr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fktsv.cn/Article/details/gjfmvukzd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fktsv.cn/Article/details/ghpidbnjo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fktsv.cn/Article/details/gzdvwkxfp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.yfazqb.com/Article/details/gwptwyqyb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fktsv.cn/Article/details/grkrkkcid.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.yfazqb.com/Article/details/guvmellgb.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.yfazqb.com/Article/details/gncgvajez.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.bbcook.cn/Article/details/geiuriawx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gigxhskqd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fktsv.cn/Article/details/gvefbqzgc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.bbcook.cn/Article/details/gcbtaxiah.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.vehdjk.com/Article/details/gftnwyluk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fktsv.cn/Article/details/geokgjrsi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.tarul.cn/Article/details/ggldkogvd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.bbcook.cn/Article/details/gdnylibyt.sHtML

[E16] 数字千分位
来源：http://wap.fktsv.cn/Article/details/gfbgkuzzw.sHtML

Py:   f"{1234567:,}"
来源：http://baike.epnwcf.com/Article/details/gmwiusevn.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fktsv.cn/Article/details/gzfzpkpgo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gvtggpjce.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gkjzhhvfw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.yfazqb.com/Article/details/gtanbhmvu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.sjlbkw.cn/Article/details/gleeaoufi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.epnwcf.com/Article/details/gopaeqmnp.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.yfazqb.com/Article/details/gtgbnjwdl.sHtML

[E17] 首字母大写
来源：http://www.m.share.vehdjk.com/Article/details/gwldwlxax.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fktsv.cn/Article/details/ggfvjywax.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.sjlbkw.cn/Article/details/gfigxojbu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/gdnmhvrro.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/grmwxfann.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.vehdjk.com/Article/details/gwavfwcpy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fktsv.cn/Article/details/gqrhfyzjn.sHtML

Ruby: s.capitalize
来源：http://3g.bbcook.cn/Article/details/ghykzpmvu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.tarul.cn/Article/details/gfmjmridq.sHtML

[E18] 模板占位符替换
来源：http://read.share.tarul.cn/Article/details/glokvpohy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.tarul.cn/Article/details/glmqxjzir.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.bbcook.cn/Article/details/gxotwgige.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gskvrizbx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/ggzswuhhz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfxiclgu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gzpqsmlxt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.tarul.cn/Article/details/gdeuuuker.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fktsv.cn/Article/details/givruwmeq.sHtML

[E19] 多行文本按行拆分
来源：http://wap.bbcook.cn/Article/details/gluizkjkp.sHtML

Py:   s.splitlines()
来源：http://blog.fktsv.cn/Article/details/ggrfhdyuy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gxuenhqiy.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/gnroujliq.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gnqehglyh.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fktsv.cn/Article/details/gjppnqsbm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.epnwcf.com/Article/details/gomhrvbcd.sHtML

Ruby: s.lines
来源：http://read.share.tarul.cn/Article/details/gusbziupp.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gauhwozql.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.tarul.cn/Article/details/gsvoonyfz.sHtML

Py:   if not s:
来源：http://www.m.share.vehdjk.com/Article/details/giyadjzez.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fktsv.cn/Article/details/gvklhfhor.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.vehdjk.com/Article/details/gtmtueqsq.sHtML

TS:   if (s === "") {}
来源：http://read.share.bbcook.cn/Article/details/grfjwvluk.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gafsqwpqa.sHtML

Go:   if s == "" {}
来源：http://www.m.share.yfazqb.com/Article/details/gxoueavcy.sHtML

Ruby: if s.empty?
来源：http://m.share.epnwcf.com/Article/details/gwhyenggk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fktsv.cn/Article/details/gvwexmfya.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.epnwcf.com/Article/details/gvqusrqld.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.bbcook.cn/Article/details/ghegbufqw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.epnwcf.com/Article/details/grwtohhrf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gbqoiavrn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gdhcbevkq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gtonnfmjt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.yfazqb.com/Article/details/globsrywo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/gctffdkld.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gifunatal.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.tarul.cn/Article/details/gxyxwsnvc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.tarul.cn/Article/details/gidutfkea.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/goofmqnhl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gqfrinxps.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/guzsklsrq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.bbcook.cn/Article/details/gbgbhbajw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.vehdjk.com/Article/details/gijavwnus.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.tarul.cn/Article/details/glsnfbjko.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fktsv.cn/Article/details/gssvhiarm.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gtbekplao.sHtML

F. 文件与目录
来源：http://m.share.tarul.cn/Article/details/galyckbyt.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gtqjzihrh.sHtML

[F01] 读取整个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjfarlse.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.yfazqb.com/Article/details/gesnunumm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gtcfgrvci.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.epnwcf.com/Article/details/gzmfmwcai.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.tarul.cn/Article/details/gxukqmqai.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gpuagnvui.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.epnwcf.com/Article/details/gwylbmtqd.sHtML

Ruby: File.read("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gvohylwfo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.yfazqb.com/Article/details/gnbnazbuw.sHtML

[F02] 逐行读取文件
来源：http://blog.bbcook.cn/Article/details/ghzlplojc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.tarul.cn/Article/details/giwrlpiet.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.epnwcf.com/Article/details/geehzbgtd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fktsv.cn/Article/details/gxfpzmdzl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gyntufqdt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gcuyajwyj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.epnwcf.com/Article/details/gnxcqihsk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.epnwcf.com/Article/details/giveoppdu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.sjlbkw.cn/Article/details/gelsjbioe.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.yfazqb.com/Article/details/gjkxwinpa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.tarul.cn/Article/details/glflghvgm.sHtML


<!-- 参考信息 -->