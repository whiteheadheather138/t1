代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.epnwcf.com/Article/details/gzokditlf.sHtML

Go:   // 手写双层循环
来源：http://mobile.bbcook.cn/Article/details/gphhftjut.sHtML

Ruby: nested.flatten
来源：http://read.share.yfazqb.com/Article/details/gqiterxah.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.tarul.cn/Article/details/gupyeztcg.sHtML

[D19] 按字段分组
来源：http://wap.epnwcf.com/Article/details/gycaqintb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.vehdjk.com/Article/details/grodgkeum.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fktsv.cn/Article/details/gpdbahhnb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.epnwcf.com/Article/details/giuwjjcbc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/gymyzpktd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.vehdjk.com/Article/details/gufsrjupt.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.yfazqb.com/Article/details/gikoxmgkv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fktsv.cn/Article/details/gtpdsuonq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.vehdjk.com/Article/details/govjosohj.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.sjlbkw.cn/Article/details/govsvdypk.sHtML

Py:   Counter(arr)
来源：http://read.share.yfazqb.com/Article/details/gohfctjgy.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.bbcook.cn/Article/details/gdotefdzp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.epnwcf.com/Article/details/glnuosqzl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gifngqjwv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfjrktaa.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.sjlbkw.cn/Article/details/gskxvkbxj.sHtML

Ruby: arr.tally
来源：http://baike.bbcook.cn/Article/details/gvslyqyks.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.epnwcf.com/Article/details/gnmhdfeyy.sHtML

[D21] 判断是否包含某元素
来源：http://blog.vehdjk.com/Article/details/gifshtpnk.sHtML

Py:   x in arr
来源：http://wap.tarul.cn/Article/details/gqkuxyvpm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.tarul.cn/Article/details/gbawaghsx.sHtML

JS:   arr.includes(x)
来源：http://www.share.epnwcf.com/Article/details/gzasgmxig.sHtML

TS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/gzxqxdmmz.sHtML

Java: list.contains(x)
来源：http://mobile.tarul.cn/Article/details/gfliirxfx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gxiwkukjv.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fktsv.cn/Article/details/gcugtwaqm.sHtML

C#:   list.Contains(x)
来源：http://mobile.tarul.cn/Article/details/gkxuolmui.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fktsv.cn/Article/details/gtxfxemtn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.yfazqb.com/Article/details/gtcrvqygv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.vehdjk.com/Article/details/gcryylrxm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.epnwcf.com/Article/details/gpwqygsju.sHtML

TS:   [...arr];
来源：http://read.share.bbcook.cn/Article/details/grgabrkco.sHtML

Java: new ArrayList<>(list);
来源：http://baike.yfazqb.com/Article/details/gfnlgzvti.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fktsv.cn/Article/details/gnrvqcaek.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.bbcook.cn/Article/details/gqlxhackp.sHtML

C#:   new List<int>(list);
来源：http://www.share.bbcook.cn/Article/details/guhoazwui.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.tarul.cn/Article/details/gaqtdmwus.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.vehdjk.com/Article/details/gdecavije.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gdhigxcmo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fktsv.cn/Article/details/gpmmogxtt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.epnwcf.com/Article/details/ggjzeeiwy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.tarul.cn/Article/details/gebslagmc.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/groyhoybm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.epnwcf.com/Article/details/gjishnrfo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.sjlbkw.cn/Article/details/gybxpsmdi.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.epnwcf.com/Article/details/gjxujglpn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.epnwcf.com/Article/details/glkrtbamq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.tarul.cn/Article/details/giwsauegq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.yfazqb.com/Article/details/gptsvspzk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.bbcook.cn/Article/details/gimkxhmei.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.sjlbkw.cn/Article/details/gvnrnxomu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.epnwcf.com/Article/details/gqopnnixa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fktsv.cn/Article/details/gaudakcmq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.epnwcf.com/Article/details/gqvdnxzvc.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.sjlbkw.cn/Article/details/gbdlbzrop.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.sjlbkw.cn/Article/details/ggtrbdimz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.bbcook.cn/Article/details/grvirplpb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.vehdjk.com/Article/details/glwnvoyqj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.sjlbkw.cn/Article/details/gfhmhkfli.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.vehdjk.com/Article/details/gsimujjlk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzkpslsi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.bbcook.cn/Article/details/glpvtgiqi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.vehdjk.com/Article/details/gxufnfbhf.sHtML

[D26] 数组转字符串
来源：http://wap.vehdjk.com/Article/details/goaenvlig.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.vehdjk.com/Article/details/gqvxersog.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gyhwmsqar.sHtML

JS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gasavrjyl.sHtML

TS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gzkitosud.sHtML

Java: String.join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gmmceicor.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.yfazqb.com/Article/details/gvcpphepx.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/ggnykfxul.sHtML

C#:   string.Join(", ", list)
来源：http://blog.vehdjk.com/Article/details/ghozfpsmx.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gfikfnlpm.sHtML

E. 字符串处理
来源：http://www.share.tarul.cn/Article/details/gaeccijzk.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gmaqskiki.sHtML

[E01] 拼接字符串
来源：http://wap.vehdjk.com/Article/details/ghjezpwsf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fktsv.cn/Article/details/gfqamztxz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfwfqfcj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.sjlbkw.cn/Article/details/gchgvoolw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/gbidnszhu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fktsv.cn/Article/details/gtnlsheez.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.sjlbkw.cn/Article/details/gyvnaxnff.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.bbcook.cn/Article/details/gmivfmnfo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gkbwufngo.sHtML

[E02] 重复字符串
来源：http://mobile.epnwcf.com/Article/details/gzhqkoxxo.sHtML

Py:   "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gogvlnhrg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fktsv.cn/Article/details/giohmjxsl.sHtML

JS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/gtrdqnteb.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/ghphmijvi.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gondzcxyn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.bbcook.cn/Article/details/ghurwgcge.sHtML

Ruby: "ab" * 3
来源：http://blog.vehdjk.com/Article/details/gmtcjfuxe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.sjlbkw.cn/Article/details/gbjvlltgr.sHtML

[E03] 截取子串
来源：http://www.share.tarul.cn/Article/details/gyxlvrkkx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.bbcook.cn/Article/details/gnoewfozc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gnaogkjsx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gijcfqxqb.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.vehdjk.com/Article/details/guwmtkqhs.sHtML

Java: s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gtbipkkmz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.tarul.cn/Article/details/givbgkmmt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.sjlbkw.cn/Article/details/gvfkrvmzn.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.sjlbkw.cn/Article/details/gwesgdhmt.sHtML

[E04] 查找子串位置
来源：http://www.blog.epnwcf.com/Article/details/gtcaowhwm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.vehdjk.com/Article/details/gwtkmuump.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.tarul.cn/Article/details/gsnsqcwvu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.yfazqb.com/Article/details/gccjeioqr.sHtML

TS:   s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gkrglmqxo.sHtML

Java: s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gtpmqmoye.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.tarul.cn/Article/details/gwgzcrjqn.sHtML

Ruby: s.index("x")
来源：http://m.share.tarul.cn/Article/details/gfcruvaml.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.yfazqb.com/Article/details/goznqctpt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fktsv.cn/Article/details/gbeuxlavl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.epnwcf.com/Article/details/gfjoczjya.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fktsv.cn/Article/details/gntpknxhf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gqlukngbp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.bbcook.cn/Article/details/gzpzcgblc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gjeuldzul.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.vehdjk.com/Article/details/gioghrlwd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.yfazqb.com/Article/details/gufwszerp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.bbcook.cn/Article/details/grkiznvkk.sHtML

[E06] 替换子串
来源：http://mobile.yfazqb.com/Article/details/gozpzjuij.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/gbcuwneaj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.bbcook.cn/Article/details/glxdihsxa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gksiytzig.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gadstxiit.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gzcyjmdrx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/gulkihqlj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gojnrkgjo.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gmndpexmh.sHtML

[E07] 按分隔符拆分
来源：http://3g.yfazqb.com/Article/details/ginghdcwk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.vehdjk.com/Article/details/gkcqpwect.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/ghfuqjgmm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.sjlbkw.cn/Article/details/giclsboss.sHtML

TS:   s.split(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gvokhtpxw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.tarul.cn/Article/details/ginqmiidt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.bbcook.cn/Article/details/gbszepqau.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.vehdjk.com/Article/details/gclhlwsst.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.tarul.cn/Article/details/ggynfynjq.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.bbcook.cn/Article/details/gqqdtqjeq.sHtML

Py:   ",".join(items)
来源：http://baike.epnwcf.com/Article/details/gbhzocfjh.sHtML

PHP:  implode(",", $items);
来源：http://3g.sjlbkw.cn/Article/details/gyqchhqrl.sHtML

JS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gullzpdnm.sHtML

TS:   items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gaxdpjdjl.sHtML

Java: String.join(",", items)
来源：http://m.share.vehdjk.com/Article/details/gogdficsn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fktsv.cn/Article/details/geegixawe.sHtML

Ruby: items.join(",")
来源：http://3g.bbcook.cn/Article/details/gvppkmkfj.sHtML

C#:   string.Join(",", items)
来源：http://blog.fktsv.cn/Article/details/goslcjobq.sHtML

[E09] 去除所有空白字符
来源：http://mobile.tarul.cn/Article/details/givthjafn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.yfazqb.com/Article/details/gddgwwuke.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gymqmspmc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/ghrzsajbt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.bbcook.cn/Article/details/ggeidzibs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.bbcook.cn/Article/details/giglfxami.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.epnwcf.com/Article/details/gvcdcyttv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fktsv.cn/Article/details/gvppqesqb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gvjbyhvrp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.epnwcf.com/Article/details/gwzuwtqtj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gwgwvoysu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.tarul.cn/Article/details/gqkyyqscs.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/ggpvikrky.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gqmuoeuon.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gjcnjknuo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gikjejbjq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gneisxsrq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.tarul.cn/Article/details/gujxpgtyq.sHtML

[E11] 反转字符串
来源：http://read.share.tarul.cn/Article/details/guhgbntiw.sHtML

Py:   s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gonlgsico.sHtML

PHP:  strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gyxwgbvyy.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gzexzfoxk.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gzfmimteu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.vehdjk.com/Article/details/gjnosimrv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.bbcook.cn/Article/details/gbaciockf.sHtML

Ruby: s.reverse
来源：http://mobile.fktsv.cn/Article/details/gzknwmdtm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.epnwcf.com/Article/details/gcbxnlukh.sHtML

[E12] 统计某字符出现次数
来源：http://baike.bbcook.cn/Article/details/gahcemdbh.sHtML

Py:   s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gttxwncoa.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.yfazqb.com/Article/details/gxlntkfjr.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/gjnnipmba.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.yfazqb.com/Article/details/gcaatrtpg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.yfazqb.com/Article/details/gvfollknb.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.bbcook.cn/Article/details/giowxtgnd.sHtML

Ruby: s.count("a")
来源：http://baike.fktsv.cn/Article/details/gzyztuyid.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.yfazqb.com/Article/details/giaukootj.sHtML

[E13] 逐字符遍历
来源：http://read.share.epnwcf.com/Article/details/ggmqazxtm.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.tarul.cn/Article/details/gpjcwglbo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.sjlbkw.cn/Article/details/gtzxatkfu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gkmefcmaz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.tarul.cn/Article/details/gczftexed.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gkciehfnc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fktsv.cn/Article/details/gxeaphfvn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.sjlbkw.cn/Article/details/giswgseyv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gcpcrtvgk.sHtML

[E14] URL 编码与 Base64
来源：http://wap.epnwcf.com/Article/details/glhtwnwti.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.tarul.cn/Article/details/gjgxqskbo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.sjlbkw.cn/Article/details/gimdjeesi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.sjlbkw.cn/Article/details/gatffkozy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.tarul.cn/Article/details/gxkjnczjg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.epnwcf.com/Article/details/gtkckaqun.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.vehdjk.com/Article/details/gvbpomumw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.bbcook.cn/Article/details/gxxnwnjmx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.tarul.cn/Article/details/gjavfiafs.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fktsv.cn/Article/details/gxjydkoqk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.yfazqb.com/Article/details/grpfycrec.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.yfazqb.com/Article/details/grrukrgek.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.epnwcf.com/Article/details/gafzylmmd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.bbcook.cn/Article/details/gvxbddzwi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.vehdjk.com/Article/details/glnrbxcot.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.bbcook.cn/Article/details/ghanrfiyw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.vehdjk.com/Article/details/gusidjeou.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.sjlbkw.cn/Article/details/gbvrfbcua.sHtML

[E16] 数字千分位
来源：http://mobile.sjlbkw.cn/Article/details/ghifxwubf.sHtML

Py:   f"{1234567:,}"
来源：http://3g.bbcook.cn/Article/details/gntpwhqoh.sHtML

PHP:  number_format(1234567);
来源：http://blog.sjlbkw.cn/Article/details/gfqjiiuaj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/ggwdxfnfb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gprfjidfy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fktsv.cn/Article/details/guymjfkeg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.tarul.cn/Article/details/grjzodguy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.bbcook.cn/Article/details/ggsfzaqnf.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.sjlbkw.cn/Article/details/guzskpbqy.sHtML

[E17] 首字母大写
来源：http://read.share.bbcook.cn/Article/details/gwfpkkrfj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.vehdjk.com/Article/details/gguyqybwx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.tarul.cn/Article/details/gsvdsgqng.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gbnpedjcz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gjpmxqwnz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.vehdjk.com/Article/details/gomnxjpue.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gtagufpre.sHtML

Ruby: s.capitalize
来源：http://m.share.tarul.cn/Article/details/gqjgozpxw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.yfazqb.com/Article/details/gbaxuirpm.sHtML

[E18] 模板占位符替换
来源：http://blog.tarul.cn/Article/details/gxqhxgeql.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.epnwcf.com/Article/details/gxnirhbyi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.epnwcf.com/Article/details/glloertlf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gnpummiwh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/ghbvffrqq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gtbxintih.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gtvrmfhni.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.sjlbkw.cn/Article/details/gymetkork.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.bbcook.cn/Article/details/grbeifxmx.sHtML

[E19] 多行文本按行拆分
来源：http://blog.vehdjk.com/Article/details/grektyydd.sHtML

Py:   s.splitlines()
来源：http://blog.bbcook.cn/Article/details/gwjesuvuz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.vehdjk.com/Article/details/ggxnwkhhx.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gyfwvayin.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.sjlbkw.cn/Article/details/gpuuexhma.sHtML

Java: s.lines().toList()
来源：http://3g.yfazqb.com/Article/details/gtvmytxgv.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.vehdjk.com/Article/details/gcgdmmckf.sHtML

Ruby: s.lines
来源：http://wap.fktsv.cn/Article/details/gsexcsnkl.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.vehdjk.com/Article/details/giixidvng.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.vehdjk.com/Article/details/gtpenfvdl.sHtML

Py:   if not s:
来源：http://www.m.share.vehdjk.com/Article/details/gzytfzozl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.epnwcf.com/Article/details/gsjmnzcfa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fktsv.cn/Article/details/gtnwwiluf.sHtML

TS:   if (s === "") {}
来源：http://www.blog.tarul.cn/Article/details/gbzscvqew.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/gkacwgstn.sHtML

Go:   if s == "" {}
来源：http://read.share.sjlbkw.cn/Article/details/grefimbhm.sHtML

Ruby: if s.empty?
来源：http://m.share.epnwcf.com/Article/details/gtpmrulvq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.epnwcf.com/Article/details/gyvpjqgvz.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fktsv.cn/Article/details/gygyqdonh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.yfazqb.com/Article/details/gueqqxtyf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gsbogrhps.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gakfbuwsp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gmxfmaoew.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gqmzdydkq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.vehdjk.com/Article/details/gvnnrgpko.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gxemfwmcu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gvdgzmwhs.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.epnwcf.com/Article/details/gkwgqjzex.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fktsv.cn/Article/details/gygcuivux.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gimyjjuhe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gmaalexdv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gmducrsvz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.tarul.cn/Article/details/gfvrrvzwb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/gambvwvev.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gvdunmdyt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.tarul.cn/Article/details/gdhnhxikm.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gtvwgklsh.sHtML

F. 文件与目录
来源：http://www.share.vehdjk.com/Article/details/gowylailx.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gemifudet.sHtML

[F01] 读取整个文件
来源：http://3g.tarul.cn/Article/details/gdesamrzu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.yfazqb.com/Article/details/gfpccusuk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gjtcufoli.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.vehdjk.com/Article/details/gnslmzgss.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gaigeqllg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gpezgrtem.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvdojxkk.sHtML

Ruby: File.read("a.txt")
来源：http://3g.bbcook.cn/Article/details/gdyenqtti.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gkjpkowpr.sHtML

[F02] 逐行读取文件
来源：http://mobile.yfazqb.com/Article/details/glvdswkyk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.yfazqb.com/Article/details/gwdodgshe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.yfazqb.com/Article/details/ggdfrxoko.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gebnkldcp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.yfazqb.com/Article/details/guenkwmnn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/gytnkbzdf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.bbcook.cn/Article/details/ggvgcoavm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.yfazqb.com/Article/details/glsmusqvi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.vehdjk.com/Article/details/gcesfkyas.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoikrxll.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.tarul.cn/Article/details/gippomqdc.sHtML


<!-- 参考信息 -->