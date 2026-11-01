代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.epnwcf.com/Article/details/glevrrhzr.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.tarul.cn/Article/details/gsqzitxan.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.sjlbkw.cn/Article/details/gllqmzsgm.sHtML

TS:   nested.flat();
来源：http://read.share.fktsv.cn/Article/details/gnvgzwhcp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.epnwcf.com/Article/details/gtodukyvl.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fktsv.cn/Article/details/gztxjfwkq.sHtML

Ruby: nested.flatten
来源：http://www.m.share.vehdjk.com/Article/details/gqdietdcs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.vehdjk.com/Article/details/gpaehkzuw.sHtML

[D19] 按字段分组
来源：http://www.blog.yfazqb.com/Article/details/gmznguqya.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.sjlbkw.cn/Article/details/glasfcpkc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fktsv.cn/Article/details/gmsyjxpmr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.vehdjk.com/Article/details/grrmdanth.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/ggcnbrcjh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.tarul.cn/Article/details/gizitymbn.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.tarul.cn/Article/details/gkkpxnrmw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.bbcook.cn/Article/details/gmxlcjbso.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.tarul.cn/Article/details/gjoqbnxss.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.bbcook.cn/Article/details/gbtwlhoci.sHtML

Py:   Counter(arr)
来源：http://www.share.fktsv.cn/Article/details/gupckshpz.sHtML

PHP:  array_count_values($arr);
来源：http://wap.vehdjk.com/Article/details/gbtrwqylv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/gpxllvnfy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gmxydkbkn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fktsv.cn/Article/details/gcvduxkti.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.yfazqb.com/Article/details/ggvopwwfp.sHtML

Ruby: arr.tally
来源：http://3g.tarul.cn/Article/details/ggjttdmwl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.bbcook.cn/Article/details/gftdhunfp.sHtML

[D21] 判断是否包含某元素
来源：http://blog.vehdjk.com/Article/details/gaqmjhpdb.sHtML

Py:   x in arr
来源：http://m.share.epnwcf.com/Article/details/gqqvuctkh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.sjlbkw.cn/Article/details/guewiymgf.sHtML

JS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gaeoxzkth.sHtML

TS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gdnarhrtk.sHtML

Java: list.contains(x)
来源：http://www.m.share.tarul.cn/Article/details/ghxfcjdur.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fktsv.cn/Article/details/gzzmnvphp.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.sjlbkw.cn/Article/details/getmlhpmz.sHtML

C#:   list.Contains(x)
来源：http://mobile.yfazqb.com/Article/details/gswyqbsat.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.yfazqb.com/Article/details/gwnjaomct.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.yfazqb.com/Article/details/gijtvknzc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.vehdjk.com/Article/details/garhsvtrn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.tarul.cn/Article/details/gstsnhyjy.sHtML

TS:   [...arr];
来源：http://www.blog.sjlbkw.cn/Article/details/grvwhxqiv.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fktsv.cn/Article/details/gtzjnaglc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.tarul.cn/Article/details/gniocdwjw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fktsv.cn/Article/details/gicjcwxdz.sHtML

C#:   new List<int>(list);
来源：http://baike.bbcook.cn/Article/details/gssykkfkf.sHtML

[D23] reduce 累积计算
来源：http://blog.yfazqb.com/Article/details/gejwfslvd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.sjlbkw.cn/Article/details/ghcbsuxqc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.bbcook.cn/Article/details/gmfywqxlk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gszdoxbtl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/gvoefaruz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.sjlbkw.cn/Article/details/gaihcvivw.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/gfcqipvbx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.vehdjk.com/Article/details/gfbswlolp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fktsv.cn/Article/details/gpjhxsvki.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.tarul.cn/Article/details/gjoijotss.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.yfazqb.com/Article/details/gmhkzklsw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fktsv.cn/Article/details/gkihivvhv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.tarul.cn/Article/details/gjxfjmhvv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.yfazqb.com/Article/details/ggxvvtrue.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.bbcook.cn/Article/details/gwalalxmj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.epnwcf.com/Article/details/gatraidbh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.bbcook.cn/Article/details/gbsctisht.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.bbcook.cn/Article/details/gevjxumow.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.sjlbkw.cn/Article/details/gbdvxaxal.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.yfazqb.com/Article/details/gbjwizajc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fktsv.cn/Article/details/glsgofzdp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.bbcook.cn/Article/details/givzhjqde.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.bbcook.cn/Article/details/gmtpvoroi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.yfazqb.com/Article/details/girsheooy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.yfazqb.com/Article/details/gcqkalsgz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fktsv.cn/Article/details/gkyjrzqmw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.yfazqb.com/Article/details/gdgnijspo.sHtML

[D26] 数组转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gkwugilsp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.epnwcf.com/Article/details/gsrachdtf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gapaaptse.sHtML

JS:   arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gyqznlkdy.sHtML

TS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gcgfjpsfu.sHtML

Java: String.join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gmmskwbhu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.bbcook.cn/Article/details/gdbzugrwt.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gmhlpjabs.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fktsv.cn/Article/details/gzqkevard.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gljkvotfe.sHtML

E. 字符串处理
来源：http://wap.sjlbkw.cn/Article/details/gykuzchpu.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gyprkhftt.sHtML

[E01] 拼接字符串
来源：http://wap.tarul.cn/Article/details/gcauibpvq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.tarul.cn/Article/details/guxhweqel.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.vehdjk.com/Article/details/gbcpghyrn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/gylyxlazj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/gzmkddigk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.epnwcf.com/Article/details/gggclbajv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fktsv.cn/Article/details/ghrjlpapz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.bbcook.cn/Article/details/ghxzjtqfb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fktsv.cn/Article/details/gbcooysfc.sHtML

[E02] 重复字符串
来源：http://www.share.sjlbkw.cn/Article/details/grcrgujtc.sHtML

Py:   "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gevqjdoxi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.epnwcf.com/Article/details/geokhzzoi.sHtML

JS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gjzgmdxre.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gttdxpvsj.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gywuqjwnb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.sjlbkw.cn/Article/details/gdbpbjigv.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.tarul.cn/Article/details/gjnxjgshs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.bbcook.cn/Article/details/gcdbbttuu.sHtML

[E03] 截取子串
来源：http://wap.epnwcf.com/Article/details/ghxvjtcmx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fktsv.cn/Article/details/gmuqdwmpb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gfimtwkhn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gdcudxrlh.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gfcferstc.sHtML

Java: s.substring(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gnrzpjmlc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fktsv.cn/Article/details/gbpokumkr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.yfazqb.com/Article/details/gjsoqwivp.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.tarul.cn/Article/details/gqwabhxyt.sHtML

[E04] 查找子串位置
来源：http://read.share.epnwcf.com/Article/details/gjhdgljxe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.bbcook.cn/Article/details/gsiiwqjal.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fktsv.cn/Article/details/gvvsccjye.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.yfazqb.com/Article/details/gxmzuanfd.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gnwgdrsyi.sHtML

Java: s.indexOf("x")
来源：http://3g.tarul.cn/Article/details/guopjgfol.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.yfazqb.com/Article/details/gvhfkydqs.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gbihavsxk.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.tarul.cn/Article/details/gqpjvjadr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.tarul.cn/Article/details/gtuenpccx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fktsv.cn/Article/details/grxxewpnt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.epnwcf.com/Article/details/gkpemijvg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gbjvguxlj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.tarul.cn/Article/details/gaahlfrau.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fktsv.cn/Article/details/gfgsuwaex.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fktsv.cn/Article/details/ggixscauh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.yfazqb.com/Article/details/golkmcybi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gffrkswae.sHtML

[E06] 替换子串
来源：http://mobile.fktsv.cn/Article/details/gejrgeobo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gbwnggbzb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.tarul.cn/Article/details/gaegtqrvv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/grhjmsira.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gmjxhrqsg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/glgttirgf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gnsovttjk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gumycgncm.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gqztfharo.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/gwnpbxgzp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.bbcook.cn/Article/details/gxohjfefb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.bbcook.cn/Article/details/gckdztmiy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.epnwcf.com/Article/details/gvlgspvid.sHtML

TS:   s.split(",")
来源：http://mobile.sjlbkw.cn/Article/details/gqnlfybfy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fktsv.cn/Article/details/gnhuyfauy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.bbcook.cn/Article/details/gdljkkyrg.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.tarul.cn/Article/details/gwcfrtmdd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.bbcook.cn/Article/details/gpwwjfjdm.sHtML

[E08] 数组按分隔符合并
来源：http://wap.vehdjk.com/Article/details/gayomyutm.sHtML

Py:   ",".join(items)
来源：http://baike.vehdjk.com/Article/details/ggbbuhjde.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.yfazqb.com/Article/details/gmbsuvjpp.sHtML

JS:   items.join(",")
来源：http://3g.bbcook.cn/Article/details/gyqrvktbv.sHtML

TS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gkvrcxinn.sHtML

Java: String.join(",", items)
来源：http://www.m.share.epnwcf.com/Article/details/gkxwakftm.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.epnwcf.com/Article/details/gwtjrnajw.sHtML

Ruby: items.join(",")
来源：http://read.share.bbcook.cn/Article/details/ghadygneh.sHtML

C#:   string.Join(",", items)
来源：http://baike.vehdjk.com/Article/details/ghdlharhj.sHtML

[E09] 去除所有空白字符
来源：http://m.share.bbcook.cn/Article/details/gajpvbupc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.yfazqb.com/Article/details/gdcxbamiv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.tarul.cn/Article/details/gkvhmqntw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.vehdjk.com/Article/details/goffhqejh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/gorlkidxn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.tarul.cn/Article/details/gviipinlf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.yfazqb.com/Article/details/grbvkpobh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.epnwcf.com/Article/details/gfzdavisq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.epnwcf.com/Article/details/grrrlqudx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.tarul.cn/Article/details/gxijqlcxx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.epnwcf.com/Article/details/gxwdublxh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.epnwcf.com/Article/details/gcgqzyjxj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gxefuctpw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/ggqgutwne.sHtML

Java: String.format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gnwpejuiz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gzdofttoc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gjrdjhddg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fktsv.cn/Article/details/gpayexiso.sHtML

[E11] 反转字符串
来源：http://www.blog.tarul.cn/Article/details/gtkfmatuh.sHtML

Py:   s[::-1]
来源：http://m.share.vehdjk.com/Article/details/gaergorjs.sHtML

PHP:  strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gatqbjzhi.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gwbzczgzj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gvicijbqw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.vehdjk.com/Article/details/gbaqltofb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.vehdjk.com/Article/details/grqvrdtxx.sHtML

Ruby: s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gjyrrrero.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/gayyprfeo.sHtML

[E12] 统计某字符出现次数
来源：http://blog.yfazqb.com/Article/details/gcjkgrzxd.sHtML

Py:   s.count("a")
来源：http://wap.bbcook.cn/Article/details/gmkciujvz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.vehdjk.com/Article/details/guwkkfwgc.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/gkjxdjfax.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdrpzoiz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fktsv.cn/Article/details/gthnxsbew.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.sjlbkw.cn/Article/details/gjblnuayy.sHtML

Ruby: s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/gimnlzrig.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.vehdjk.com/Article/details/ggngsgfyk.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.bbcook.cn/Article/details/ghnbbsblq.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.epnwcf.com/Article/details/gneeiwqmw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.epnwcf.com/Article/details/gvbehtucq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gdtnojrqd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/ggifpefts.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.epnwcf.com/Article/details/gvlheavhr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.vehdjk.com/Article/details/gtzsgebuj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.yfazqb.com/Article/details/grsehrhjf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.bbcook.cn/Article/details/gkkzoyqxe.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fktsv.cn/Article/details/gdkfcjkbu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fktsv.cn/Article/details/gjxklhbix.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.vehdjk.com/Article/details/gdpaffrsw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.sjlbkw.cn/Article/details/gfmyepfxu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fktsv.cn/Article/details/gipcdovwr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.vehdjk.com/Article/details/ginpuwkyw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/gevyicsll.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.bbcook.cn/Article/details/gkzsaueny.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.epnwcf.com/Article/details/gnquxipqa.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.yfazqb.com/Article/details/gjmavuvka.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.vehdjk.com/Article/details/gbtutffrv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gehxvmdwv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fktsv.cn/Article/details/gkirncyzw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.tarul.cn/Article/details/gnidkiivx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.bbcook.cn/Article/details/gpoidsrul.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.tarul.cn/Article/details/gggljyvlm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.vehdjk.com/Article/details/gxmtoowkd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.bbcook.cn/Article/details/gppjrxagt.sHtML

[E16] 数字千分位
来源：http://m.share.bbcook.cn/Article/details/gxfgktmbz.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.yfazqb.com/Article/details/gthglqkcy.sHtML

PHP:  number_format(1234567);
来源：http://wap.vehdjk.com/Article/details/gnfvbdgsy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/gshnenumj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gshwnhxjd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gjkmfcgzo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fktsv.cn/Article/details/gohczqkdt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.epnwcf.com/Article/details/gksdaiqpi.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.tarul.cn/Article/details/gapsxgime.sHtML

[E17] 首字母大写
来源：http://wap.tarul.cn/Article/details/gjmpjcbde.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fktsv.cn/Article/details/galqxotyq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.vehdjk.com/Article/details/ginhwflit.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.tarul.cn/Article/details/gxeztbnmm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fktsv.cn/Article/details/ggapayxnb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.tarul.cn/Article/details/gbzdbptqb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.vehdjk.com/Article/details/gwrqudpsl.sHtML

Ruby: s.capitalize
来源：http://3g.bbcook.cn/Article/details/gxoiougcn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.epnwcf.com/Article/details/gyclrpvrh.sHtML

[E18] 模板占位符替换
来源：http://m.share.tarul.cn/Article/details/gxrwtiqev.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.epnwcf.com/Article/details/glqfvxejp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.epnwcf.com/Article/details/gjofkanut.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/gjmjqlyda.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.tarul.cn/Article/details/gonlvbzkj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gvzrswbhq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gxrfolfnk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.epnwcf.com/Article/details/guluzosxt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.tarul.cn/Article/details/gxookcwio.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fktsv.cn/Article/details/gxfbqqecy.sHtML

Py:   s.splitlines()
来源：http://3g.vehdjk.com/Article/details/gxmtesbng.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gwtceurjd.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gzyckymbm.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.yfazqb.com/Article/details/gicmlszfw.sHtML

Java: s.lines().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gadnntxcj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.yfazqb.com/Article/details/gahmqrjvf.sHtML

Ruby: s.lines
来源：http://www.share.vehdjk.com/Article/details/gthewyvrg.sHtML

C#:   s.Split('\n')
来源：http://m.share.bbcook.cn/Article/details/gkzujpvjl.sHtML

[E20] 判断字符串是否为空
来源：http://3g.vehdjk.com/Article/details/gxxmpbpld.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/glddcpxpg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fktsv.cn/Article/details/gzjrgnsar.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.bbcook.cn/Article/details/gcpsokefs.sHtML

TS:   if (s === "") {}
来源：http://blog.tarul.cn/Article/details/ggrfijkws.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/gqllaoaxe.sHtML

Go:   if s == "" {}
来源：http://m.share.fktsv.cn/Article/details/gflxjtjry.sHtML

Ruby: if s.empty?
来源：http://www.m.share.sjlbkw.cn/Article/details/gensqysmf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gbujwjqpk.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.sjlbkw.cn/Article/details/gcounxbta.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.yfazqb.com/Article/details/gedwzaylr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gqrykswgx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gbzwigtjs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/ggqyohtnx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gkrwvntia.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.bbcook.cn/Article/details/gebjkiutt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gzgjzlftw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gxsokbfqm.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fktsv.cn/Article/details/gnczmrbbi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/grcverwwo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gmzpgppdy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gahaqgvrc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/gpuxnehbf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.bbcook.cn/Article/details/gbuilhcad.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.yfazqb.com/Article/details/gyrcmzobm.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.bbcook.cn/Article/details/gggissjxx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.tarul.cn/Article/details/gyoumfxgp.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggknwrasa.sHtML

F. 文件与目录
来源：http://www.m.share.epnwcf.com/Article/details/gyarwhexr.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gvanuphmi.sHtML

[F01] 读取整个文件
来源：http://3g.vehdjk.com/Article/details/gxqznysoa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.yfazqb.com/Article/details/gsuozmwdc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gdbynwvlv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.vehdjk.com/Article/details/gmedpwfwl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gnmzjrqje.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gnqniedbx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.bbcook.cn/Article/details/gtjpeksii.sHtML

Ruby: File.read("a.txt")
来源：http://3g.epnwcf.com/Article/details/gimqeubxm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.yfazqb.com/Article/details/gszipmkoy.sHtML

[F02] 逐行读取文件
来源：http://3g.bbcook.cn/Article/details/gymrluohm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.epnwcf.com/Article/details/grpmnyekh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.yfazqb.com/Article/details/ggtlsvraq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.yfazqb.com/Article/details/gjewciuap.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/grqucmucd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/gttgwbqfn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.sjlbkw.cn/Article/details/gmnfpnqnc.sHtML


<!-- 参考信息 -->