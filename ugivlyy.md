代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.bbcook.cn/Article/details/gtshcgkae.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.sjlbkw.cn/Article/details/gnpqmitce.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.yfazqb.com/Article/details/gfrjxsaow.sHtML

TS:   nested.flat();
来源：http://blog.bbcook.cn/Article/details/gcnrenfve.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.epnwcf.com/Article/details/gcnsokimq.sHtML

Go:   // 手写双层循环
来源：http://www.share.vehdjk.com/Article/details/gpqoootlr.sHtML

Ruby: nested.flatten
来源：http://www.share.sjlbkw.cn/Article/details/grnqkpgsw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fktsv.cn/Article/details/glsgejowt.sHtML

[D19] 按字段分组
来源：http://read.share.sjlbkw.cn/Article/details/ggqsddzyx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.vehdjk.com/Article/details/gnylsmjuk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.tarul.cn/Article/details/ghuiozzpy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fktsv.cn/Article/details/gjnkcycdt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/gcbxdzfdo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.bbcook.cn/Article/details/gassvoqmm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.tarul.cn/Article/details/gcmlwvgjl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fktsv.cn/Article/details/gfmhauogb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.vehdjk.com/Article/details/gshgoncmx.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.yfazqb.com/Article/details/gfjgcctfq.sHtML

Py:   Counter(arr)
来源：http://read.share.bbcook.cn/Article/details/gyjploclt.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.yfazqb.com/Article/details/gyfchasol.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/gmnualevl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/ghosdcjgd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.yfazqb.com/Article/details/gzmxqqfiy.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fktsv.cn/Article/details/gbrxhxhxt.sHtML

Ruby: arr.tally
来源：http://www.m.share.fktsv.cn/Article/details/gkryvkchi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.sjlbkw.cn/Article/details/goagczgpa.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.vehdjk.com/Article/details/grjmwshny.sHtML

Py:   x in arr
来源：http://3g.tarul.cn/Article/details/gbumyidsa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.bbcook.cn/Article/details/giufkkxqj.sHtML

JS:   arr.includes(x)
来源：http://www.blog.vehdjk.com/Article/details/giqvbpqrh.sHtML

TS:   arr.includes(x)
来源：http://m.share.vehdjk.com/Article/details/grnicweac.sHtML

Java: list.contains(x)
来源：http://3g.tarul.cn/Article/details/gxscgqtoc.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/grvfxkyjg.sHtML

Ruby: arr.include?(x)
来源：http://3g.bbcook.cn/Article/details/gftrdqvrr.sHtML

C#:   list.Contains(x)
来源：http://3g.vehdjk.com/Article/details/gnwvwlvub.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.vehdjk.com/Article/details/ggtwnbuuu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/gvoahubne.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.sjlbkw.cn/Article/details/gnrjggtch.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.bbcook.cn/Article/details/grpxqdugk.sHtML

TS:   [...arr];
来源：http://3g.sjlbkw.cn/Article/details/gdzrcajsu.sHtML

Java: new ArrayList<>(list);
来源：http://blog.epnwcf.com/Article/details/gcbkvkduc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.tarul.cn/Article/details/gpolkpdkm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.sjlbkw.cn/Article/details/gcgqjhjgy.sHtML

C#:   new List<int>(list);
来源：http://wap.yfazqb.com/Article/details/gthweimkc.sHtML

[D23] reduce 累积计算
来源：http://3g.bbcook.cn/Article/details/gryndjdoj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.tarul.cn/Article/details/gkoshndao.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.epnwcf.com/Article/details/gspacjcph.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.vehdjk.com/Article/details/ghdslugjo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gzkcjfubs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.yfazqb.com/Article/details/gebvihcuv.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gprcgevdl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.yfazqb.com/Article/details/gtuyfqiov.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.epnwcf.com/Article/details/gtzsvvolf.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fktsv.cn/Article/details/gbusloptd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.vehdjk.com/Article/details/gpsabetci.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.yfazqb.com/Article/details/ghtmvfcdc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.tarul.cn/Article/details/ggtznqmlu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gyakqougv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.sjlbkw.cn/Article/details/grgdqnbfi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.bbcook.cn/Article/details/gujhaswlk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.vehdjk.com/Article/details/gqsltkibf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.epnwcf.com/Article/details/giniiikrb.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fktsv.cn/Article/details/ggwkskfuw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.yfazqb.com/Article/details/gscidnfgb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.sjlbkw.cn/Article/details/gqjzpioog.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.tarul.cn/Article/details/gxsgidsja.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.vehdjk.com/Article/details/gdpetzanz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.tarul.cn/Article/details/gbfdkajof.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.yfazqb.com/Article/details/gaarzimly.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.bbcook.cn/Article/details/gpniadtjx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.sjlbkw.cn/Article/details/gvahuovps.sHtML

[D26] 数组转字符串
来源：http://wap.fktsv.cn/Article/details/gjmfedrmo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.vehdjk.com/Article/details/gpfjlupew.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.tarul.cn/Article/details/gvrmbadef.sHtML

JS:   arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gppudlmqu.sHtML

TS:   arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gpqhdasdn.sHtML

Java: String.join(", ", list)
来源：http://m.share.bbcook.cn/Article/details/guzyemfsu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.bbcook.cn/Article/details/gmmonoiik.sHtML

Ruby: arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/giofjqlml.sHtML

C#:   string.Join(", ", list)
来源：http://baike.yfazqb.com/Article/details/gcaptfmvi.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghaqtudvs.sHtML

E. 字符串处理
来源：http://www.m.share.sjlbkw.cn/Article/details/goyrgrhqf.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gecvluddg.sHtML

[E01] 拼接字符串
来源：http://mobile.yfazqb.com/Article/details/gkrvghbvc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.vehdjk.com/Article/details/ggilpfyal.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.sjlbkw.cn/Article/details/gxgdrsulm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gmqdmtfyg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.yfazqb.com/Article/details/gmszvdjck.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.epnwcf.com/Article/details/gpwfxrjti.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.vehdjk.com/Article/details/gnvgmxdme.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.yfazqb.com/Article/details/gquleekvl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.epnwcf.com/Article/details/gedsyyaba.sHtML

[E02] 重复字符串
来源：http://m.share.tarul.cn/Article/details/gvizdvwrz.sHtML

Py:   "ab" * 3
来源：http://blog.sjlbkw.cn/Article/details/gauvefcwr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fktsv.cn/Article/details/gcflpbjwg.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/grykegvzm.sHtML

TS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gpmccyfcb.sHtML

Java: "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/gqxmksusx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fktsv.cn/Article/details/grwfvsisb.sHtML

Ruby: "ab" * 3
来源：http://read.share.yfazqb.com/Article/details/gucacfcca.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.tarul.cn/Article/details/gcfzwhltf.sHtML

[E03] 截取子串
来源：http://mobile.bbcook.cn/Article/details/gbvwdkxng.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.tarul.cn/Article/details/gzifxbxhi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/ghyqggxhb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gtopisewp.sHtML

TS:   s.slice(1, 4)
来源：http://baike.epnwcf.com/Article/details/gsbkzyzku.sHtML

Java: s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/gkviphimu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fktsv.cn/Article/details/glgrjojfm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.vehdjk.com/Article/details/gyagngnnr.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.vehdjk.com/Article/details/gdqsvaehp.sHtML

[E04] 查找子串位置
来源：http://baike.tarul.cn/Article/details/gfjvzhfkp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.bbcook.cn/Article/details/gfeyabuok.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.vehdjk.com/Article/details/gaddnmtjb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fktsv.cn/Article/details/goujabczp.sHtML

TS:   s.indexOf("x")
来源：http://3g.bbcook.cn/Article/details/ggyonbjsz.sHtML

Java: s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gyhguefeq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.sjlbkw.cn/Article/details/gectuzjnx.sHtML

Ruby: s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/gxhjxihcu.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gimfzsckn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fktsv.cn/Article/details/geolqgeul.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.yfazqb.com/Article/details/gxhhfiqni.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.tarul.cn/Article/details/gxclrozau.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gurtsoqou.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.vehdjk.com/Article/details/gpafcmxwe.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/gjgwpaotr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.epnwcf.com/Article/details/gajbsffpi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.epnwcf.com/Article/details/gzsqyygmo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gweiootwz.sHtML

[E06] 替换子串
来源：http://www.share.epnwcf.com/Article/details/gwvwonmnw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/gaobklsrl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.sjlbkw.cn/Article/details/gpikbzhwt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gsethxvpa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gmrrvtuwh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gpctrebdy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gzgorlimk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.vehdjk.com/Article/details/goesbghaj.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gytnwbpzw.sHtML

[E07] 按分隔符拆分
来源：http://blog.epnwcf.com/Article/details/goedmwsve.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.bbcook.cn/Article/details/grnywpsmv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/ghkgeukxi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fktsv.cn/Article/details/gznudljei.sHtML

TS:   s.split(",")
来源：http://www.m.share.yfazqb.com/Article/details/giuugcjky.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.sjlbkw.cn/Article/details/ginhshpjy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwbevqiw.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.tarul.cn/Article/details/gnzqjzmpu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fktsv.cn/Article/details/ggzqvssss.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.sjlbkw.cn/Article/details/gjmvendco.sHtML

Py:   ",".join(items)
来源：http://www.blog.yfazqb.com/Article/details/grebmyztu.sHtML

PHP:  implode(",", $items);
来源：http://baike.bbcook.cn/Article/details/gtqzdgrdf.sHtML

JS:   items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gzgpztkii.sHtML

TS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/gzprqkftq.sHtML

Java: String.join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gynosayad.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.vehdjk.com/Article/details/gaavipvsw.sHtML

Ruby: items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gttpwoyhg.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fktsv.cn/Article/details/grcrrokza.sHtML

[E09] 去除所有空白字符
来源：http://www.share.sjlbkw.cn/Article/details/guofioxne.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.bbcook.cn/Article/details/guvjbpgzh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.epnwcf.com/Article/details/gqulfuxpk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fktsv.cn/Article/details/gypausbcr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gsmbomroy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gxitiklri.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.tarul.cn/Article/details/gbdmlqqjk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.vehdjk.com/Article/details/gvcaegddf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.bbcook.cn/Article/details/gayzsuetl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.sjlbkw.cn/Article/details/glfjtjhsm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gpswqxvli.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.vehdjk.com/Article/details/gxakcmdxa.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gsqgcyjnx.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gthcnmctq.sHtML

Java: String.format("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/ghnnhpmab.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gvfjfygiv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/gbmjycgjn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.sjlbkw.cn/Article/details/gsnftmqnd.sHtML

[E11] 反转字符串
来源：http://baike.vehdjk.com/Article/details/gbyazdkeu.sHtML

Py:   s[::-1]
来源：http://mobile.epnwcf.com/Article/details/gkupzcysg.sHtML

PHP:  strrev($s);
来源：http://www.share.fktsv.cn/Article/details/gbenpwsyn.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gagykgebz.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gcsqtsjrx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.bbcook.cn/Article/details/gqcyfwhfz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.yfazqb.com/Article/details/gfuxuajns.sHtML

Ruby: s.reverse
来源：http://blog.vehdjk.com/Article/details/grvdijxcv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gjkvnbroe.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gcylfoadv.sHtML

Py:   s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/gunleronz.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.vehdjk.com/Article/details/gdkkigrkk.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gehahitmj.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gfrmhelde.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.sjlbkw.cn/Article/details/gexznefgi.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.bbcook.cn/Article/details/gwcrkjckv.sHtML

Ruby: s.count("a")
来源：http://www.blog.tarul.cn/Article/details/gtfoefwtv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.sjlbkw.cn/Article/details/ghqfqzajq.sHtML

[E13] 逐字符遍历
来源：http://read.share.sjlbkw.cn/Article/details/geqfxxizm.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.vehdjk.com/Article/details/geikkqinw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.tarul.cn/Article/details/gcpjudxmb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gadmqyhte.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.yfazqb.com/Article/details/giczbzomd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.vehdjk.com/Article/details/glqrswxbo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnszptpb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.bbcook.cn/Article/details/gfavvveez.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.bbcook.cn/Article/details/gxcludlwp.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcgesrdv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fktsv.cn/Article/details/gevqzetuk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.vehdjk.com/Article/details/gmhmsokvg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.epnwcf.com/Article/details/gpjtpubbs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.vehdjk.com/Article/details/glntffcbg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.tarul.cn/Article/details/gvaodrxam.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.epnwcf.com/Article/details/grlarhthe.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fktsv.cn/Article/details/gkegsvrsd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/glolqhqvw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.epnwcf.com/Article/details/gvtlsjjps.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.bbcook.cn/Article/details/gtwbeanjq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fktsv.cn/Article/details/gjnunfsht.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.epnwcf.com/Article/details/gzzhsigwd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.sjlbkw.cn/Article/details/ggqznbxoe.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.sjlbkw.cn/Article/details/gklneiibz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fktsv.cn/Article/details/gitjtwdrm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fktsv.cn/Article/details/gfdyqlqma.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.tarul.cn/Article/details/gbagyknfg.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/guvoldphy.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.bbcook.cn/Article/details/gkwugydjw.sHtML

PHP:  number_format(1234567);
来源：http://blog.yfazqb.com/Article/details/gjghxkyjd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.vehdjk.com/Article/details/gqzzncwqg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/gsyxutwar.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.sjlbkw.cn/Article/details/gtkzqaalk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.epnwcf.com/Article/details/gdkoefste.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.yfazqb.com/Article/details/gretevuhb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gayvkgfpl.sHtML

[E17] 首字母大写
来源：http://www.share.yfazqb.com/Article/details/gugxikitk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.sjlbkw.cn/Article/details/gphxkhzcl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.bbcook.cn/Article/details/gnzhsddpg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gusytqnkx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/gxnqnufoj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.epnwcf.com/Article/details/gwtowvwpz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.bbcook.cn/Article/details/ggyztrnsb.sHtML

Ruby: s.capitalize
来源：http://3g.vehdjk.com/Article/details/gfhyheuta.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.vehdjk.com/Article/details/gctkazulj.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxqlybfk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fktsv.cn/Article/details/gczuwnvyz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.epnwcf.com/Article/details/ggwzleihz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gmwicktuv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/ghognjmqo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.vehdjk.com/Article/details/ghhcgnffx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/giwyuizcm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.sjlbkw.cn/Article/details/gadknnvba.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fktsv.cn/Article/details/grunvmpep.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.yfazqb.com/Article/details/gikmueqrv.sHtML

Py:   s.splitlines()
来源：http://baike.vehdjk.com/Article/details/gyvzayfyh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.yfazqb.com/Article/details/gmkmyyyqu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gnottguiy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/ggudamols.sHtML

Java: s.lines().toList()
来源：http://blog.bbcook.cn/Article/details/gtnthrduj.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.vehdjk.com/Article/details/gmdlvbtyb.sHtML

Ruby: s.lines
来源：http://www.m.share.yfazqb.com/Article/details/glgatzphk.sHtML

C#:   s.Split('\n')
来源：http://read.share.bbcook.cn/Article/details/gzowafjaw.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.epnwcf.com/Article/details/gjuafrxaz.sHtML

Py:   if not s:
来源：http://baike.vehdjk.com/Article/details/ggmvlexmf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.sjlbkw.cn/Article/details/gsrglrzye.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.yfazqb.com/Article/details/gkxcuwxvd.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/gfpjpzghy.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gbzhcbwei.sHtML

Go:   if s == "" {}
来源：http://m.share.bbcook.cn/Article/details/gyfpgpyjn.sHtML

Ruby: if s.empty?
来源：http://m.share.yfazqb.com/Article/details/gvncmulfm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.bbcook.cn/Article/details/gfumuuhna.sHtML

[E21] 超长截断加省略号
来源：http://3g.bbcook.cn/Article/details/gahvjgxfk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.sjlbkw.cn/Article/details/gnvrrntiu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.tarul.cn/Article/details/galidqbfo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/grfpflvxt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gezcfeyvh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gbwdxvpvc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fktsv.cn/Article/details/grfsgslbo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/ggrxervpw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gmjzkdhem.sHtML

[E22] 字节长度与字符长度
来源：http://3g.tarul.cn/Article/details/gkhsprzel.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.sjlbkw.cn/Article/details/gwftuwohm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/ggmjnpudo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/ggeyuvdsy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/gbvxhaxrq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fktsv.cn/Article/details/grqahxrvr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.bbcook.cn/Article/details/gedaaxoqs.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.sjlbkw.cn/Article/details/gsvzcbthc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gslbmkfbt.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gsygjbiue.sHtML

F. 文件与目录
来源：http://blog.fktsv.cn/Article/details/gklhmqjve.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbzfuethq.sHtML

[F01] 读取整个文件
来源：http://m.share.bbcook.cn/Article/details/gywahatvr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.tarul.cn/Article/details/grbuiuoic.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.bbcook.cn/Article/details/gjeuoxoem.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.tarul.cn/Article/details/gotikgwcu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gdjyqmsru.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/ghnharrdx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.epnwcf.com/Article/details/gammahfkk.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gsumognqh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gatbfpvfo.sHtML

[F02] 逐行读取文件
来源：http://read.share.yfazqb.com/Article/details/gpqemdzsm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.tarul.cn/Article/details/gpxrttehy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fktsv.cn/Article/details/gglsqgams.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.vehdjk.com/Article/details/grlvzmgma.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gloqhzqdn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gtvtpfkig.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.tarul.cn/Article/details/gvboyukiq.sHtML


<!-- 参考信息 -->