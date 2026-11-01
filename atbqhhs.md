代发 wailian999

[D19] 按字段分组
来源：http://3g.epnwcf.com/Article/details/gehfviqxk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fktsv.cn/Article/details/glccrpedo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.epnwcf.com/Article/details/gxennrivw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fktsv.cn/Article/details/gomcufwfq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/guwwglahb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/gqfqkiyzo.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.yfazqb.com/Article/details/gueiwztjs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.tarul.cn/Article/details/gmhtsketk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.vehdjk.com/Article/details/gduzrwrar.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.bbcook.cn/Article/details/gngmxfuvx.sHtML

Py:   Counter(arr)
来源：http://blog.bbcook.cn/Article/details/gipgydywa.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gifrpxxgb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/gvvwppnaj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.yfazqb.com/Article/details/gweekhtcp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.yfazqb.com/Article/details/gcxjujhou.sHtML

Go:   // 手写 map[T]int
来源：http://wap.bbcook.cn/Article/details/glwzjfolw.sHtML

Ruby: arr.tally
来源：http://blog.tarul.cn/Article/details/gulaqawvf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.yfazqb.com/Article/details/gsolxfswz.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.epnwcf.com/Article/details/gdplliysz.sHtML

Py:   x in arr
来源：http://wap.fktsv.cn/Article/details/gcicragjm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.bbcook.cn/Article/details/gadxkrmus.sHtML

JS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gncizvjni.sHtML

TS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/glnidioav.sHtML

Java: list.contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gxoicymkt.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.epnwcf.com/Article/details/gpcbkdnlp.sHtML

Ruby: arr.include?(x)
来源：http://read.share.yfazqb.com/Article/details/gazkrfoto.sHtML

C#:   list.Contains(x)
来源：http://wap.tarul.cn/Article/details/gxctcnpil.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fktsv.cn/Article/details/glomsitqs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.vehdjk.com/Article/details/gsdfpuitd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.tarul.cn/Article/details/gbyjlyohj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.vehdjk.com/Article/details/gqipprmbw.sHtML

TS:   [...arr];
来源：http://read.share.bbcook.cn/Article/details/glqknwchi.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.bbcook.cn/Article/details/gklltrthm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gtqslblyt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fktsv.cn/Article/details/gqzkbjtow.sHtML

C#:   new List<int>(list);
来源：http://mobile.sjlbkw.cn/Article/details/gyxnmswtl.sHtML

[D23] reduce 累积计算
来源：http://mobile.sjlbkw.cn/Article/details/gvqdxvbtj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.epnwcf.com/Article/details/grlnemalc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.yfazqb.com/Article/details/gxlbmmdzz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/ggdxbcydg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.vehdjk.com/Article/details/gmbpegyya.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.vehdjk.com/Article/details/gwwkmgjdc.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gqlntdbof.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.yfazqb.com/Article/details/glthhmfjd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.bbcook.cn/Article/details/ggrkntisg.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.yfazqb.com/Article/details/ggoyigthm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.sjlbkw.cn/Article/details/gssjpobza.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.sjlbkw.cn/Article/details/gzfrnnpol.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.bbcook.cn/Article/details/gfcedtrug.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gmywqkxbw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fktsv.cn/Article/details/gwaozzsza.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.bbcook.cn/Article/details/ghgtijuwa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.bbcook.cn/Article/details/grwntdsin.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.tarul.cn/Article/details/gswfhujqm.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fktsv.cn/Article/details/gasrgdggw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.tarul.cn/Article/details/gklgkcpxn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.yfazqb.com/Article/details/gqhgvyfgy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.yfazqb.com/Article/details/gybbvqupo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.sjlbkw.cn/Article/details/ggrwmvjua.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.sjlbkw.cn/Article/details/ghgeacrjy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.bbcook.cn/Article/details/gvktwxcrx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.tarul.cn/Article/details/gyzpettyz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fktsv.cn/Article/details/gkcrnjlhj.sHtML

[D26] 数组转字符串
来源：http://wap.yfazqb.com/Article/details/gagrgouwu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.tarul.cn/Article/details/gzpsvweup.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.epnwcf.com/Article/details/gwlrdrdiz.sHtML

JS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gwyrbqynt.sHtML

TS:   arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gcqjhbkbs.sHtML

Java: String.join(", ", list)
来源：http://mobile.tarul.cn/Article/details/gsyejpryc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fktsv.cn/Article/details/glviyvltz.sHtML

Ruby: arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/grfqurewh.sHtML

C#:   string.Join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gazsgpqhb.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gelzpgrjj.sHtML

E. 字符串处理
来源：http://mobile.tarul.cn/Article/details/ghxhkxfzg.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpgqcwaas.sHtML

[E01] 拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gubrmiojm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fktsv.cn/Article/details/gpldhsnvs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.yfazqb.com/Article/details/gkodlfyus.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gwapylrjg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/gluoekpgt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.tarul.cn/Article/details/gbrfbmdkd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fktsv.cn/Article/details/gtpwrqids.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.sjlbkw.cn/Article/details/gopkmvrpx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gxmfhmqyz.sHtML

[E02] 重复字符串
来源：http://baike.vehdjk.com/Article/details/ggitfwbtf.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fktsv.cn/Article/details/ghbfvfnew.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.bbcook.cn/Article/details/grgtnunwr.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gswqxsosp.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gekqlpxpe.sHtML

Java: "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gxbqqagip.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gnbkiqhjw.sHtML

Ruby: "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gtwmzdozf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.sjlbkw.cn/Article/details/gzleyavbg.sHtML

[E03] 截取子串
来源：http://blog.yfazqb.com/Article/details/gtnjgmhvc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.vehdjk.com/Article/details/gtnemywtm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/ghodhyrzc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gukzebkij.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxehnkjg.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gwcuzjxdl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fktsv.cn/Article/details/gsqjqadis.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.yfazqb.com/Article/details/gznfixyhg.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.bbcook.cn/Article/details/gfisimzco.sHtML

[E04] 查找子串位置
来源：http://3g.tarul.cn/Article/details/glkzwtpne.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.bbcook.cn/Article/details/gisqpuykq.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.vehdjk.com/Article/details/gamgtdjrr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.vehdjk.com/Article/details/gtytwzbdl.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gjlzutsgn.sHtML

Java: s.indexOf("x")
来源：http://3g.bbcook.cn/Article/details/gudplfmfy.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.tarul.cn/Article/details/ghsqzuzoi.sHtML

Ruby: s.index("x")
来源：http://wap.epnwcf.com/Article/details/gxctrmily.sHtML

C#:   s.IndexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gahbsnpso.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.yfazqb.com/Article/details/ggtdlqnnu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gitgesksj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.bbcook.cn/Article/details/glvjirwqw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/ghofcxzzs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.epnwcf.com/Article/details/gihfkauqq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmyciogm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.tarul.cn/Article/details/guyykpodx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.yfazqb.com/Article/details/ggpayrrxz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gdllaycjk.sHtML

[E06] 替换子串
来源：http://blog.fktsv.cn/Article/details/grjhmbsho.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gtpjybaio.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.vehdjk.com/Article/details/gvmwjmodd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gmhgvdhvg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gfmvmyhro.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gcafoirlj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gfknuvkkm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fktsv.cn/Article/details/gdnuhjpif.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.epnwcf.com/Article/details/gxyjgmsxx.sHtML

[E07] 按分隔符拆分
来源：http://baike.fktsv.cn/Article/details/gaidcnhxe.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.yfazqb.com/Article/details/gwpugquym.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjikbdka.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gepumetsx.sHtML

TS:   s.split(",")
来源：http://3g.vehdjk.com/Article/details/gdbxssjub.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.tarul.cn/Article/details/guvukirih.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.tarul.cn/Article/details/gasreektm.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.bbcook.cn/Article/details/geyzcbkom.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.epnwcf.com/Article/details/gwucosude.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.sjlbkw.cn/Article/details/gavwxdrfe.sHtML

Py:   ",".join(items)
来源：http://www.m.share.yfazqb.com/Article/details/giflvhzos.sHtML

PHP:  implode(",", $items);
来源：http://mobile.sjlbkw.cn/Article/details/gtnhzexer.sHtML

JS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/gqivfzstk.sHtML

TS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/ggvcafnez.sHtML

Java: String.join(",", items)
来源：http://mobile.tarul.cn/Article/details/geztiydli.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fktsv.cn/Article/details/gqsoizedn.sHtML

Ruby: items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/getwpnxim.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gidsyojxx.sHtML

[E09] 去除所有空白字符
来源：http://m.share.sjlbkw.cn/Article/details/ggihgrece.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.epnwcf.com/Article/details/ggkaznzhe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/gyjwpwkia.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/gylhevhwk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaffstccd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gajhftait.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.bbcook.cn/Article/details/gnmndymtw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.tarul.cn/Article/details/gkisixkuc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.bbcook.cn/Article/details/gtkiwvhfu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.yfazqb.com/Article/details/gpkfadbhn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.yfazqb.com/Article/details/gwaxtgbnk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.sjlbkw.cn/Article/details/gzcgpwlsp.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gbfngvgne.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gepgcerep.sHtML

Java: String.format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gaahjpqtz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/ggxbhvrpr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/ginoqnrcr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.vehdjk.com/Article/details/gpzuuwmwy.sHtML

[E11] 反转字符串
来源：http://3g.tarul.cn/Article/details/gfyorurfw.sHtML

Py:   s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gvuypnruu.sHtML

PHP:  strrev($s);
来源：http://wap.yfazqb.com/Article/details/gpeikfqqp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gjvvnhdum.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gvtcbmzbm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.bbcook.cn/Article/details/gcheibzfz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.epnwcf.com/Article/details/godbblqxq.sHtML

Ruby: s.reverse
来源：http://baike.vehdjk.com/Article/details/gkcuhpqps.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gyjyqmoru.sHtML

[E12] 统计某字符出现次数
来源：http://wap.epnwcf.com/Article/details/gatyffwfa.sHtML

Py:   s.count("a")
来源：http://wap.vehdjk.com/Article/details/gamwikoji.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.sjlbkw.cn/Article/details/gvphbsfbv.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/ggikmsfjf.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/glndztmvi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.bbcook.cn/Article/details/gwivqaroq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fktsv.cn/Article/details/gmueayxmj.sHtML

Ruby: s.count("a")
来源：http://read.share.fktsv.cn/Article/details/gzbnlabhr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.vehdjk.com/Article/details/glmfafhcq.sHtML

[E13] 逐字符遍历
来源：http://baike.vehdjk.com/Article/details/gimocndkd.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.bbcook.cn/Article/details/galitzjvi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.bbcook.cn/Article/details/gqsbikrvs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.vehdjk.com/Article/details/grkyupooj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.yfazqb.com/Article/details/gdfmwyjkg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.epnwcf.com/Article/details/ggjlreuhe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.sjlbkw.cn/Article/details/gtjnzkpzf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.sjlbkw.cn/Article/details/gitdbownu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.epnwcf.com/Article/details/gkrvhyyfh.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.sjlbkw.cn/Article/details/gxrtexozb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.bbcook.cn/Article/details/gzyqzooks.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fktsv.cn/Article/details/gbjmvnpeo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.sjlbkw.cn/Article/details/gbeezbaob.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.vehdjk.com/Article/details/gzfrbzeey.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.bbcook.cn/Article/details/gjzulioxf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/gdxsjerob.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.sjlbkw.cn/Article/details/gafqrcusr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.bbcook.cn/Article/details/gfqbspsci.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.bbcook.cn/Article/details/gieyxugjl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.yfazqb.com/Article/details/glfvidifh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fktsv.cn/Article/details/gcxflowiu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.bbcook.cn/Article/details/gfjykawww.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.epnwcf.com/Article/details/gelqanpvm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.vehdjk.com/Article/details/gvednczas.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.tarul.cn/Article/details/goibmqrsz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.epnwcf.com/Article/details/givxbesva.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.epnwcf.com/Article/details/gmymuxxbc.sHtML

[E16] 数字千分位
来源：http://www.m.share.yfazqb.com/Article/details/ggndjawif.sHtML

Py:   f"{1234567:,}"
来源：http://baike.epnwcf.com/Article/details/gkpefykyf.sHtML

PHP:  number_format(1234567);
来源：http://3g.fktsv.cn/Article/details/gzzjlfkew.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/ggyaegfst.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.bbcook.cn/Article/details/gezxchtsv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fktsv.cn/Article/details/gujttmfsb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.vehdjk.com/Article/details/gpbaptjuy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.epnwcf.com/Article/details/gaxovovxr.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fktsv.cn/Article/details/gmpzaubad.sHtML

[E17] 首字母大写
来源：http://3g.sjlbkw.cn/Article/details/gtreozamc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.tarul.cn/Article/details/gtvyxtqgi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.epnwcf.com/Article/details/gfcjocbkh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/girnhxfxx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gwisucbhi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.bbcook.cn/Article/details/gfpjdbzqj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fktsv.cn/Article/details/gkjhtwelk.sHtML

Ruby: s.capitalize
来源：http://wap.epnwcf.com/Article/details/gfuzwseha.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fktsv.cn/Article/details/gihirhzxo.sHtML

[E18] 模板占位符替换
来源：http://www.share.sjlbkw.cn/Article/details/gztzxdzwy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.epnwcf.com/Article/details/gkuodjvcj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.bbcook.cn/Article/details/gfyntnfyp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gozbltktv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gcmlzupaq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gikkfrvfm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gaaiwvfmb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.sjlbkw.cn/Article/details/gsaaglujo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.sjlbkw.cn/Article/details/gfnbosodo.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fktsv.cn/Article/details/gxnweaujd.sHtML

Py:   s.splitlines()
来源：http://3g.fktsv.cn/Article/details/gfxdvierg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gqnbljnpw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.bbcook.cn/Article/details/gozpbevyz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.vehdjk.com/Article/details/grasquzdq.sHtML

Java: s.lines().toList()
来源：http://wap.epnwcf.com/Article/details/gjhehypgr.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnnjcqyo.sHtML

Ruby: s.lines
来源：http://read.share.epnwcf.com/Article/details/gleqjwqos.sHtML

C#:   s.Split('\n')
来源：http://m.share.yfazqb.com/Article/details/gfpukaxvs.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.tarul.cn/Article/details/gunaqabdq.sHtML

Py:   if not s:
来源：http://www.m.share.yfazqb.com/Article/details/gbgnjkmlv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.sjlbkw.cn/Article/details/gnyjwluym.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.tarul.cn/Article/details/goygziecq.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.yfazqb.com/Article/details/gbritckic.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fktsv.cn/Article/details/gmvjrlsln.sHtML

Go:   if s == "" {}
来源：http://baike.epnwcf.com/Article/details/gjpzyauvg.sHtML

Ruby: if s.empty?
来源：http://www.m.share.vehdjk.com/Article/details/gnnqtzosz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gymoyyczn.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.sjlbkw.cn/Article/details/gmwkuaaft.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.yfazqb.com/Article/details/gndnyltay.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gilvkqobb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gqlrwehnb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gasppqwsw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gicdtxvqk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.bbcook.cn/Article/details/gdirtvjpf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/gdyybdpfl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gigfvejzg.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.epnwcf.com/Article/details/gyifswbxd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.yfazqb.com/Article/details/gbjypxojl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gmgzkxmiw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/ggaxgkyjk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gzyvyngde.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fktsv.cn/Article/details/gagkizqie.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.tarul.cn/Article/details/gonmmtixe.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gtrcemtls.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.vehdjk.com/Article/details/guewkisbi.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gevbmgctq.sHtML

F. 文件与目录
来源：http://www.share.bbcook.cn/Article/details/gdbbzhykw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gljlwzerl.sHtML

[F01] 读取整个文件
来源：http://3g.yfazqb.com/Article/details/gnzpsifyf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.sjlbkw.cn/Article/details/gtphxgnux.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.yfazqb.com/Article/details/goikcvivj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.bbcook.cn/Article/details/gbrwzdury.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.yfazqb.com/Article/details/ggwapabrs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gbvuxitzw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.tarul.cn/Article/details/gpgxuaokk.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gapcudzba.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gpmtixbtd.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvdmfztp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.epnwcf.com/Article/details/gqfenkpkt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gocbwepja.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.bbcook.cn/Article/details/gomwiubmh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.yfazqb.com/Article/details/glmmbqtyf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/gwhwavnyo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.vehdjk.com/Article/details/gccpiyfzw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.yfazqb.com/Article/details/gdyvsiinl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.bbcook.cn/Article/details/gayainvqw.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fktsv.cn/Article/details/grsrpvctk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.yfazqb.com/Article/details/gygdfbuch.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/ghkcsasbv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/gvsdfrrff.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/geaycuczu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fktsv.cn/Article/details/gvdoixapt.sHtML


<!-- 参考信息 -->