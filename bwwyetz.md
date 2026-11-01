代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/gvpggolzb.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.yfazqb.com/Article/details/guheuybah.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.vehdjk.com/Article/details/ginkcnpwe.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.tarul.cn/Article/details/gewjopjsa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fktsv.cn/Article/details/gcmxsonmu.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.vehdjk.com/Article/details/gcffrpnmy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.vehdjk.com/Article/details/grgeuzblv.sHtML

TS:   nested.flat();
来源：http://mobile.fktsv.cn/Article/details/gnhykocnm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gakkjecrm.sHtML

Go:   // 手写双层循环
来源：http://wap.tarul.cn/Article/details/giientqej.sHtML

Ruby: nested.flatten
来源：http://read.share.yfazqb.com/Article/details/guqatbzgl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gkzkpenqd.sHtML

[D19] 按字段分组
来源：http://www.blog.fktsv.cn/Article/details/gchnkdunw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.bbcook.cn/Article/details/gycpzglnn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fktsv.cn/Article/details/gfyriytet.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fktsv.cn/Article/details/gwphmrqxl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.yfazqb.com/Article/details/gdgbcbypz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.epnwcf.com/Article/details/gsvdqcmit.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.yfazqb.com/Article/details/gifhxzayg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.epnwcf.com/Article/details/glzfcxvga.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.bbcook.cn/Article/details/gfbjdrbkp.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fktsv.cn/Article/details/gcnmeouto.sHtML

Py:   Counter(arr)
来源：http://m.share.epnwcf.com/Article/details/getbztocw.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fktsv.cn/Article/details/gpggnkmwo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.epnwcf.com/Article/details/gukcojcgu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/gbslvigac.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.vehdjk.com/Article/details/gggmirgho.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.yfazqb.com/Article/details/gdplmtfin.sHtML

Ruby: arr.tally
来源：http://3g.sjlbkw.cn/Article/details/grbxpwtxi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.epnwcf.com/Article/details/gbnheoilx.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.yfazqb.com/Article/details/gzdghvcsy.sHtML

Py:   x in arr
来源：http://www.share.yfazqb.com/Article/details/ggtbsufxh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.tarul.cn/Article/details/gttfsbtal.sHtML

JS:   arr.includes(x)
来源：http://www.share.vehdjk.com/Article/details/ghsoqcits.sHtML

TS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gksgbhywe.sHtML

Java: list.contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gaakyeokz.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fktsv.cn/Article/details/genefndal.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gbbmgykdo.sHtML

C#:   list.Contains(x)
来源：http://wap.yfazqb.com/Article/details/grnmldsri.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.vehdjk.com/Article/details/gnsgljavl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.yfazqb.com/Article/details/glbwiyjjj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.epnwcf.com/Article/details/gazdsttaw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbvtudra.sHtML

TS:   [...arr];
来源：http://blog.epnwcf.com/Article/details/gmjtabhst.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmdmlljq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fktsv.cn/Article/details/gnvzuwblh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.epnwcf.com/Article/details/giqugxcav.sHtML

C#:   new List<int>(list);
来源：http://mobile.fktsv.cn/Article/details/gjmhpfapj.sHtML

[D23] reduce 累积计算
来源：http://m.share.fktsv.cn/Article/details/gjtdqdcwv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.yfazqb.com/Article/details/gtgefcfkf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.epnwcf.com/Article/details/ggpirgdeh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.bbcook.cn/Article/details/ghcuzwkyx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fktsv.cn/Article/details/gmrdscnpl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.yfazqb.com/Article/details/gjhcpulnm.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/gfmxclmgs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.bbcook.cn/Article/details/gltjqpobq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.tarul.cn/Article/details/gdwguxodv.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.bbcook.cn/Article/details/goswolcad.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.yfazqb.com/Article/details/gzkdvvpuq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gfkdvatcm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.yfazqb.com/Article/details/gwpytjxdh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.tarul.cn/Article/details/gumstzfwg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.vehdjk.com/Article/details/gvvaacwxn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.yfazqb.com/Article/details/gsbguewwl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.tarul.cn/Article/details/gundgadkb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.yfazqb.com/Article/details/gmoapexax.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.sjlbkw.cn/Article/details/grufapsid.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.epnwcf.com/Article/details/girwapoae.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.tarul.cn/Article/details/gnekurayu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.epnwcf.com/Article/details/getkrjlzw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.bbcook.cn/Article/details/goioqvknl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.vehdjk.com/Article/details/gsfoykgnj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.yfazqb.com/Article/details/gvqqhwjmn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fktsv.cn/Article/details/gukcavaip.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.vehdjk.com/Article/details/goxxeoblk.sHtML

[D26] 数组转字符串
来源：http://mobile.epnwcf.com/Article/details/gnmauqvtt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.epnwcf.com/Article/details/gtbwofgrs.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gtlfclwmn.sHtML

JS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gusvyjltf.sHtML

TS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gqpvkadpy.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/ggneulqcj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fktsv.cn/Article/details/glqmtarwh.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gmdxlnefv.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.epnwcf.com/Article/details/gwmnkozxt.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gcludstyc.sHtML

E. 字符串处理
来源：http://www.m.share.fktsv.cn/Article/details/ghvowwawn.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gddrssokv.sHtML

[E01] 拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gdbecqily.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.yfazqb.com/Article/details/godfjzigg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.tarul.cn/Article/details/gnssksukh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/guywztnvz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.yfazqb.com/Article/details/gsbdzokjg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fktsv.cn/Article/details/gzyoyznop.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.vehdjk.com/Article/details/gzxlutmig.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.epnwcf.com/Article/details/gdvyixzwa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.tarul.cn/Article/details/gldzkkbim.sHtML

[E02] 重复字符串
来源：http://www.m.share.fktsv.cn/Article/details/gmprrfixz.sHtML

Py:   "ab" * 3
来源：http://wap.bbcook.cn/Article/details/ganutiqro.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.vehdjk.com/Article/details/gxmeahohj.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gkkywilsy.sHtML

TS:   "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/gfnxzgwtw.sHtML

Java: "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gmisbhwut.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.epnwcf.com/Article/details/gtljouiql.sHtML

Ruby: "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gflidvopf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fktsv.cn/Article/details/gsgimvgeu.sHtML

[E03] 截取子串
来源：http://wap.vehdjk.com/Article/details/guhdcltds.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.vehdjk.com/Article/details/gluxjgxdi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gzucvurvf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gzrpwsblj.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gqldojsms.sHtML

Java: s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/gbjhrgiio.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.vehdjk.com/Article/details/guynlqqyi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.bbcook.cn/Article/details/ghofouwor.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.sjlbkw.cn/Article/details/gmtasfbsl.sHtML

[E04] 查找子串位置
来源：http://wap.tarul.cn/Article/details/ghekygsju.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.sjlbkw.cn/Article/details/gtgucslvn.sHtML

PHP:  strpos($s, "x");
来源：http://baike.epnwcf.com/Article/details/gfjdhkddb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.yfazqb.com/Article/details/guwanpvzc.sHtML

TS:   s.indexOf("x")
来源：http://www.share.bbcook.cn/Article/details/glgofkjjc.sHtML

Java: s.indexOf("x")
来源：http://baike.tarul.cn/Article/details/gzuhsvimf.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fktsv.cn/Article/details/gzmsnwkym.sHtML

Ruby: s.index("x")
来源：http://read.share.tarul.cn/Article/details/ghcqgnsyw.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gcjgdovtz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fktsv.cn/Article/details/gpaehfrvq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.yfazqb.com/Article/details/ghqurifjj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.sjlbkw.cn/Article/details/gmejevhvh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.bbcook.cn/Article/details/gupqlqece.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.vehdjk.com/Article/details/gwwfhovsh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gegwwfawk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.sjlbkw.cn/Article/details/gsdpyzcce.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.bbcook.cn/Article/details/gphkchgjd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gqsonuesc.sHtML

[E06] 替换子串
来源：http://www.share.fktsv.cn/Article/details/gcwohunjy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/gyfzzmnmo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.vehdjk.com/Article/details/gvxcvnjyf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gluzwqkps.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gohkxpvmv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/giwbqdnqp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/gubfuixul.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gbwqvcitj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gjznnjqva.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.epnwcf.com/Article/details/glfvwytjm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.bbcook.cn/Article/details/gkpqzmowf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.bbcook.cn/Article/details/gckyplvkb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.yfazqb.com/Article/details/grnxyompv.sHtML

TS:   s.split(",")
来源：http://www.m.share.vehdjk.com/Article/details/gxviysuiz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.tarul.cn/Article/details/gkdjtyoky.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.tarul.cn/Article/details/gdbixabvy.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.vehdjk.com/Article/details/gdramvaqr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.epnwcf.com/Article/details/gdvyzqewa.sHtML

[E08] 数组按分隔符合并
来源：http://baike.vehdjk.com/Article/details/gycubewjb.sHtML

Py:   ",".join(items)
来源：http://www.blog.fktsv.cn/Article/details/gxfcaadel.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.vehdjk.com/Article/details/ggimzhval.sHtML

JS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gcrjahkgj.sHtML

TS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gljghgfbr.sHtML

Java: String.join(",", items)
来源：http://mobile.sjlbkw.cn/Article/details/gotnxhrht.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.bbcook.cn/Article/details/gxehmnxlk.sHtML

Ruby: items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gevstmugv.sHtML

C#:   string.Join(",", items)
来源：http://blog.fktsv.cn/Article/details/grrlcerid.sHtML

[E09] 去除所有空白字符
来源：http://baike.vehdjk.com/Article/details/ggpuvkngn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.sjlbkw.cn/Article/details/grrjhsoew.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.epnwcf.com/Article/details/gjhjszenr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gjctuedpz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gympsxkpa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/giatsidee.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.tarul.cn/Article/details/gyoyxyvaf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.tarul.cn/Article/details/gffykehml.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.tarul.cn/Article/details/gmdnkpunv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.epnwcf.com/Article/details/genfzexza.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gxjoirrfd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/gkvadhxvk.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/grvpnoaga.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gelgjvrbl.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gnekigpqd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gthzfnhcd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gpizxicmk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fktsv.cn/Article/details/geojnxkgn.sHtML

[E11] 反转字符串
来源：http://blog.epnwcf.com/Article/details/gsklbcbai.sHtML

Py:   s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/ghqdkpqtc.sHtML

PHP:  strrev($s);
来源：http://baike.tarul.cn/Article/details/gwlthqssa.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gtgzzzhij.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gricrxnix.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fktsv.cn/Article/details/gmjxljdzf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.yfazqb.com/Article/details/ggzoybdqk.sHtML

Ruby: s.reverse
来源：http://www.share.tarul.cn/Article/details/gthvvvdec.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gwcnrfzgo.sHtML

[E12] 统计某字符出现次数
来源：http://3g.yfazqb.com/Article/details/gzthwzvft.sHtML

Py:   s.count("a")
来源：http://baike.vehdjk.com/Article/details/gvvzvguji.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.sjlbkw.cn/Article/details/gxvxbbkuw.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/glzxtimet.sHtML

TS:   s.split("a").length - 1
来源：http://wap.bbcook.cn/Article/details/gyukxywwi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.yfazqb.com/Article/details/gieqffuyn.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.yfazqb.com/Article/details/gcrwciopj.sHtML

Ruby: s.count("a")
来源：http://wap.tarul.cn/Article/details/gjrahqltq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.bbcook.cn/Article/details/grtzxaimr.sHtML

[E13] 逐字符遍历
来源：http://baike.sjlbkw.cn/Article/details/glrydfxne.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.sjlbkw.cn/Article/details/gccvpzixe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.epnwcf.com/Article/details/gpkrttjsb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.bbcook.cn/Article/details/gyrmhjlom.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gmpwusyeo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.tarul.cn/Article/details/gdssxmghz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.tarul.cn/Article/details/gwamozdmu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.tarul.cn/Article/details/gvlyxwiuh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcpxdadf.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fktsv.cn/Article/details/gubevdhvz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fktsv.cn/Article/details/gujjmfuit.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.yfazqb.com/Article/details/gkhpofjic.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.bbcook.cn/Article/details/gvzuukoqt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fktsv.cn/Article/details/gbttpalmb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.yfazqb.com/Article/details/gcolrgqxx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.vehdjk.com/Article/details/gtvmnhdvx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.bbcook.cn/Article/details/guzoqnbdl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.bbcook.cn/Article/details/gntatsiro.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fktsv.cn/Article/details/gdjkmolna.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.bbcook.cn/Article/details/ggpqhtzcj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.bbcook.cn/Article/details/ggqnyqpto.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.bbcook.cn/Article/details/gnvdtsvbv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.epnwcf.com/Article/details/gzgnotbiw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.tarul.cn/Article/details/gjtrbyspy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.epnwcf.com/Article/details/gxclsejjv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.tarul.cn/Article/details/gemiqlgkv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.sjlbkw.cn/Article/details/gwixkhrci.sHtML

[E16] 数字千分位
来源：http://blog.sjlbkw.cn/Article/details/gfrvakaog.sHtML

Py:   f"{1234567:,}"
来源：http://baike.yfazqb.com/Article/details/gyvdltjbi.sHtML

PHP:  number_format(1234567);
来源：http://read.share.sjlbkw.cn/Article/details/gnzswpuki.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.sjlbkw.cn/Article/details/gybkmysmi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gvxuyvavt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gnxirigus.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.vehdjk.com/Article/details/gedijbydm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.bbcook.cn/Article/details/gbvsucoot.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fktsv.cn/Article/details/gvkrcoqwj.sHtML

[E17] 首字母大写
来源：http://wap.epnwcf.com/Article/details/gmjrwafwu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/gtqdrgdac.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.epnwcf.com/Article/details/gvubazacx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhckudky.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gteinlsgc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.sjlbkw.cn/Article/details/gxrzisirc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.sjlbkw.cn/Article/details/gajtqusdt.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/gpjbhcaik.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.tarul.cn/Article/details/githmevfx.sHtML

[E18] 模板占位符替换
来源：http://www.share.epnwcf.com/Article/details/ggrebzwas.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.bbcook.cn/Article/details/givfybcqs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.epnwcf.com/Article/details/gutgywmcd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/ghrdbytla.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gvpjddmvl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gaxkotxpx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.epnwcf.com/Article/details/gfdexipjs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.tarul.cn/Article/details/gkritcvhh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.bbcook.cn/Article/details/gninlxktd.sHtML

[E19] 多行文本按行拆分
来源：http://blog.sjlbkw.cn/Article/details/gzikymcrl.sHtML

Py:   s.splitlines()
来源：http://read.share.tarul.cn/Article/details/gluofrfyd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gqmvxwpqg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gjmjxybpp.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.bbcook.cn/Article/details/gcpjelelq.sHtML

Java: s.lines().toList()
来源：http://m.share.fktsv.cn/Article/details/gzhidaout.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.vehdjk.com/Article/details/gstlncftg.sHtML

Ruby: s.lines
来源：http://m.share.sjlbkw.cn/Article/details/gsffunivr.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.epnwcf.com/Article/details/ghrahdvcw.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.bbcook.cn/Article/details/gdbdbdexe.sHtML

Py:   if not s:
来源：http://read.share.vehdjk.com/Article/details/gyehcquoz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fktsv.cn/Article/details/gxwrdgzcc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.yfazqb.com/Article/details/gampddzhk.sHtML

TS:   if (s === "") {}
来源：http://read.share.yfazqb.com/Article/details/gqclnodou.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.sjlbkw.cn/Article/details/gpmajfuxw.sHtML

Go:   if s == "" {}
来源：http://www.blog.vehdjk.com/Article/details/gvxcficxu.sHtML

Ruby: if s.empty?
来源：http://read.share.yfazqb.com/Article/details/gxldcmwap.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.bbcook.cn/Article/details/grxijwxcr.sHtML

[E21] 超长截断加省略号
来源：http://wap.vehdjk.com/Article/details/gohuauitl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.vehdjk.com/Article/details/gbpkobhzh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gwdhaufgo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gwwuqhvmv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gkpcwtfcu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gsnukidpq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.tarul.cn/Article/details/giqggiqxp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/grfuupqla.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gmgjdsdoj.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.yfazqb.com/Article/details/gpcjzfjom.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.bbcook.cn/Article/details/gyfwmtpin.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gbqfpnzvr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/gahoclmhs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gxfhopkno.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.tarul.cn/Article/details/grrnmroap.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.vehdjk.com/Article/details/gmgppdety.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.epnwcf.com/Article/details/gceplqkhx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.yfazqb.com/Article/details/gsdtrhiul.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gtgwkcgyb.sHtML

F. 文件与目录
来源：http://blog.fktsv.cn/Article/details/gnmyzispq.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/grzewshwr.sHtML

[F01] 读取整个文件
来源：http://3g.sjlbkw.cn/Article/details/gkjozwjbt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.tarul.cn/Article/details/gzuuefdbg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gwgrliztp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.bbcook.cn/Article/details/gmxehdpjv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/ggiwlupre.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/ggytfdhqt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.tarul.cn/Article/details/ghplwhoep.sHtML

Ruby: File.read("a.txt")
来源：http://wap.yfazqb.com/Article/details/golwnmowo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.yfazqb.com/Article/details/gpinyjnnm.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fktsv.cn/Article/details/grtavjktc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fktsv.cn/Article/details/gwalwapbq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.tarul.cn/Article/details/gccsqrheo.sHtML


<!-- 参考信息 -->