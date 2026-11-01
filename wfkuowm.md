代发 wailian999

[D19] 按字段分组
来源：http://blog.fktsv.cn/Article/details/gaplqqetu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.sjlbkw.cn/Article/details/gyucnxkab.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.bbcook.cn/Article/details/gkzqmwzva.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fktsv.cn/Article/details/globxcpwn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.yfazqb.com/Article/details/gwnteootd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.sjlbkw.cn/Article/details/guexsnieh.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.epnwcf.com/Article/details/gzpvxclcl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.yfazqb.com/Article/details/gojbovzeb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.vehdjk.com/Article/details/gjckhkgiu.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.sjlbkw.cn/Article/details/gkitbkdps.sHtML

Py:   Counter(arr)
来源：http://m.share.epnwcf.com/Article/details/gqszcxctr.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.vehdjk.com/Article/details/gywtlmaci.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.yfazqb.com/Article/details/guzdfhhgc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/gmghbynqm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.sjlbkw.cn/Article/details/gfkhsreli.sHtML

Go:   // 手写 map[T]int
来源：http://3g.vehdjk.com/Article/details/gfjfdkuai.sHtML

Ruby: arr.tally
来源：http://m.share.bbcook.cn/Article/details/gquekrqba.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.sjlbkw.cn/Article/details/gojeibswn.sHtML

[D21] 判断是否包含某元素
来源：http://wap.bbcook.cn/Article/details/gksecjkab.sHtML

Py:   x in arr
来源：http://baike.bbcook.cn/Article/details/gqpulasfr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.yfazqb.com/Article/details/gscvyedkc.sHtML

JS:   arr.includes(x)
来源：http://www.share.bbcook.cn/Article/details/gwibcukrd.sHtML

TS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gjbwrqkfi.sHtML

Java: list.contains(x)
来源：http://baike.epnwcf.com/Article/details/gsisjdxsq.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gkjevrlin.sHtML

Ruby: arr.include?(x)
来源：http://baike.epnwcf.com/Article/details/gepvchxkw.sHtML

C#:   list.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gfxpmpyyj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.tarul.cn/Article/details/gglavqblu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.sjlbkw.cn/Article/details/gwhdddyun.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.vehdjk.com/Article/details/gtspoagdm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.epnwcf.com/Article/details/gzalohwaz.sHtML

TS:   [...arr];
来源：http://baike.sjlbkw.cn/Article/details/gytfapnjr.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.vehdjk.com/Article/details/ggfrydpwm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fktsv.cn/Article/details/gydsxclae.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.vehdjk.com/Article/details/gkknvuucz.sHtML

C#:   new List<int>(list);
来源：http://wap.sjlbkw.cn/Article/details/gcmcbfxui.sHtML

[D23] reduce 累积计算
来源：http://blog.sjlbkw.cn/Article/details/gakgckama.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.bbcook.cn/Article/details/gsggihkkn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.tarul.cn/Article/details/gcmugpsve.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/guxovifqk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gczirputa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.bbcook.cn/Article/details/gjrgjkulr.sHtML

Go:   // 手写循环
来源：http://www.blog.yfazqb.com/Article/details/gmonypyoz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.tarul.cn/Article/details/gwzunoslz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.yfazqb.com/Article/details/gemozabvw.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fktsv.cn/Article/details/gtqirzrzs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.tarul.cn/Article/details/gguoyohfy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fktsv.cn/Article/details/gnzchlvtx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fktsv.cn/Article/details/gslqzaigt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gnzzdejkx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fktsv.cn/Article/details/gzuufwlhk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.yfazqb.com/Article/details/gbyfvexrn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.bbcook.cn/Article/details/gnausgghd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fktsv.cn/Article/details/gialthklu.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fktsv.cn/Article/details/gvajurrve.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.yfazqb.com/Article/details/gwbdmdcbh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.tarul.cn/Article/details/gvwmudnax.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.yfazqb.com/Article/details/gscoznksw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.yfazqb.com/Article/details/gvcvycnft.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.yfazqb.com/Article/details/ggofhbjxw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.yfazqb.com/Article/details/gbkctmsiz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.tarul.cn/Article/details/gyonwatbf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.bbcook.cn/Article/details/gzbarnzsf.sHtML

[D26] 数组转字符串
来源：http://blog.tarul.cn/Article/details/gzoekxroq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.yfazqb.com/Article/details/gekrbrcqw.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.bbcook.cn/Article/details/gnxbvoclk.sHtML

JS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gqbluqbiw.sHtML

TS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gntxhjqxr.sHtML

Java: String.join(", ", list)
来源：http://3g.epnwcf.com/Article/details/ghpnuyrsl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fktsv.cn/Article/details/gdhhyblkm.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gamrqnuaj.sHtML

C#:   string.Join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gugyfortz.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ghdjylfyg.sHtML

E. 字符串处理
来源：http://mobile.sjlbkw.cn/Article/details/gykyhbejq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glrtvnztl.sHtML

[E01] 拼接字符串
来源：http://baike.tarul.cn/Article/details/gknjpubkw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.epnwcf.com/Article/details/gvjywhlts.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.vehdjk.com/Article/details/ghsyprtbv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/gcfanemis.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/gijxwniiy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.epnwcf.com/Article/details/gnzzauzla.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.sjlbkw.cn/Article/details/ggmeifsej.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.bbcook.cn/Article/details/gwreypssv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fktsv.cn/Article/details/gaaqsmzjf.sHtML

[E02] 重复字符串
来源：http://wap.epnwcf.com/Article/details/ggjrhxxiq.sHtML

Py:   "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/gjwtdtewg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.tarul.cn/Article/details/ghivunxlb.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/gleoxvnin.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gkhxvffri.sHtML

Java: "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/ggollrrhw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.bbcook.cn/Article/details/gkddqlncd.sHtML

Ruby: "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/givedvghg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.yfazqb.com/Article/details/gobdhedun.sHtML

[E03] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/gufdfveww.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.yfazqb.com/Article/details/gqhgfjxuw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gpfzvdyyk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gzuokkjqz.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gyslemztf.sHtML

Java: s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/govrugyls.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fktsv.cn/Article/details/ggxbedbrw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fktsv.cn/Article/details/grfdsiuno.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.bbcook.cn/Article/details/gpxcrynuu.sHtML

[E04] 查找子串位置
来源：http://3g.epnwcf.com/Article/details/gnzceetjs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/gqdeagroc.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fktsv.cn/Article/details/gkkfxlkpd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.sjlbkw.cn/Article/details/gelzybjts.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gqpaomlln.sHtML

Java: s.indexOf("x")
来源：http://blog.vehdjk.com/Article/details/gqznqyton.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.epnwcf.com/Article/details/gxqjlkqbw.sHtML

Ruby: s.index("x")
来源：http://m.share.tarul.cn/Article/details/gymlpectq.sHtML

C#:   s.IndexOf("x")
来源：http://blog.yfazqb.com/Article/details/gajbhqbvf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.yfazqb.com/Article/details/gygkwkfcm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fktsv.cn/Article/details/gjginmnat.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.yfazqb.com/Article/details/gcymszzzt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.vehdjk.com/Article/details/gowjsvphr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.epnwcf.com/Article/details/gglhjsqwp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gcbaxusor.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.yfazqb.com/Article/details/gyayaoemj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fktsv.cn/Article/details/gzqntjvdc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gwzkdazws.sHtML

[E06] 替换子串
来源：http://3g.fktsv.cn/Article/details/gstfqladf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/gpektzuic.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.vehdjk.com/Article/details/gfavmcewf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gyvujsegr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gfnoalslm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gibkntccp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.tarul.cn/Article/details/gstyajtgy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/ggfbiyoeo.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gjdnilfcd.sHtML

[E07] 按分隔符拆分
来源：http://wap.tarul.cn/Article/details/gtpwdpxur.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.sjlbkw.cn/Article/details/gcwtluocp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.bbcook.cn/Article/details/gmpvioepo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.bbcook.cn/Article/details/gqzisncvj.sHtML

TS:   s.split(",")
来源：http://read.share.vehdjk.com/Article/details/glgdlzluy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fktsv.cn/Article/details/gsatvqroo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.bbcook.cn/Article/details/gbmahkwzx.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.yfazqb.com/Article/details/gifwmcptt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.vehdjk.com/Article/details/gvbcwhrmx.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.bbcook.cn/Article/details/gpavqfzmj.sHtML

Py:   ",".join(items)
来源：http://www.m.share.yfazqb.com/Article/details/ghfeajbbj.sHtML

PHP:  implode(",", $items);
来源：http://wap.epnwcf.com/Article/details/gpxskljtm.sHtML

JS:   items.join(",")
来源：http://mobile.tarul.cn/Article/details/gksbcoqep.sHtML

TS:   items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gucxoefyf.sHtML

Java: String.join(",", items)
来源：http://blog.fktsv.cn/Article/details/gbkiodewy.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.epnwcf.com/Article/details/ghtkqkkpw.sHtML

Ruby: items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gbiozvetw.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/gsabzqiyo.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.tarul.cn/Article/details/gmosovbtf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.epnwcf.com/Article/details/gxzcfdjhu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.vehdjk.com/Article/details/gtidfxive.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/gbajwihwo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.tarul.cn/Article/details/gnbjkdgby.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gisziwdix.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.bbcook.cn/Article/details/gdzzrziqj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.bbcook.cn/Article/details/gsmnngyko.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gdckiozrk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.epnwcf.com/Article/details/gcvatlmba.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fktsv.cn/Article/details/ghozrlfvr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.bbcook.cn/Article/details/ggnzkymyt.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/gqgjsfmvb.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gssizneas.sHtML

Java: String.format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gmwjfygkd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/guddrhivz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gfajafjsh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.epnwcf.com/Article/details/gdkjyluds.sHtML

[E11] 反转字符串
来源：http://www.share.vehdjk.com/Article/details/gfdukumnl.sHtML

Py:   s[::-1]
来源：http://3g.tarul.cn/Article/details/grlfvbhwq.sHtML

PHP:  strrev($s);
来源：http://3g.bbcook.cn/Article/details/gqctdorie.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/guztejtms.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/ggeadmuqv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.yfazqb.com/Article/details/gmlcehvhl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.tarul.cn/Article/details/gudxxaroc.sHtML

Ruby: s.reverse
来源：http://blog.bbcook.cn/Article/details/gkloefiyo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/giusdabvr.sHtML

[E12] 统计某字符出现次数
来源：http://blog.vehdjk.com/Article/details/gomrtrnag.sHtML

Py:   s.count("a")
来源：http://3g.yfazqb.com/Article/details/gmuwanqtp.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fktsv.cn/Article/details/gnthmajfr.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gvfpetaee.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/gqomxvxkf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fktsv.cn/Article/details/gjfqusnvs.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.tarul.cn/Article/details/gfyojxqze.sHtML

Ruby: s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gfpfgmbyz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.sjlbkw.cn/Article/details/gczskkgyq.sHtML

[E13] 逐字符遍历
来源：http://baike.bbcook.cn/Article/details/ggcskfgxm.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fktsv.cn/Article/details/gnctwktxr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.sjlbkw.cn/Article/details/gmfjtqxtl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gmujgxmfx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.tarul.cn/Article/details/gqnltmvbc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.vehdjk.com/Article/details/gvdgigqvn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.sjlbkw.cn/Article/details/gggquubdl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.tarul.cn/Article/details/guwyjepxv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fktsv.cn/Article/details/gqsasvmmq.sHtML

[E14] URL 编码与 Base64
来源：http://baike.tarul.cn/Article/details/gijtefwmd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.tarul.cn/Article/details/gphkoqrhz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.tarul.cn/Article/details/geppktasr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.yfazqb.com/Article/details/gzegdqkky.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.vehdjk.com/Article/details/gmfjofsfa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fktsv.cn/Article/details/gsdqfiiqo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fktsv.cn/Article/details/gmwaadknm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.epnwcf.com/Article/details/gfkdlcwmh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.bbcook.cn/Article/details/gexcpwyuc.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.epnwcf.com/Article/details/gcuqbdbvn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.vehdjk.com/Article/details/gchhptvdo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.vehdjk.com/Article/details/gelepqirh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.epnwcf.com/Article/details/gclqnmvvw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.bbcook.cn/Article/details/grerswzjf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.sjlbkw.cn/Article/details/ghmaejkve.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.epnwcf.com/Article/details/guvjytrwc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.sjlbkw.cn/Article/details/gjowfzaop.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.tarul.cn/Article/details/gjezjhtxj.sHtML

[E16] 数字千分位
来源：http://m.share.tarul.cn/Article/details/gsskssjjk.sHtML

Py:   f"{1234567:,}"
来源：http://3g.epnwcf.com/Article/details/gvsdxetts.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.bbcook.cn/Article/details/ggjeqqcch.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gtfwsjbah.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gwkfhktln.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.epnwcf.com/Article/details/gtxreieum.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.bbcook.cn/Article/details/gsfyujleh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.epnwcf.com/Article/details/grkvfsdiq.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.tarul.cn/Article/details/gtdkhkwsk.sHtML

[E17] 首字母大写
来源：http://blog.epnwcf.com/Article/details/gfaxmitfm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fktsv.cn/Article/details/guawgmwkc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.bbcook.cn/Article/details/glctnibih.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/guhsmequg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gpdcjvgmd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.vehdjk.com/Article/details/guegceddo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.yfazqb.com/Article/details/gyosnrpac.sHtML

Ruby: s.capitalize
来源：http://m.share.yfazqb.com/Article/details/gkzipicfi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.epnwcf.com/Article/details/gszkjvnnf.sHtML

[E18] 模板占位符替换
来源：http://read.share.sjlbkw.cn/Article/details/ggjrmpucs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.vehdjk.com/Article/details/gfnggecwn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fktsv.cn/Article/details/gltjcvnvi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gllwpsywp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gxauzfhyh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gxiwjkuko.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gqcwiyvbb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.sjlbkw.cn/Article/details/gvincbrvu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.sjlbkw.cn/Article/details/gbztujaur.sHtML

[E19] 多行文本按行拆分
来源：http://3g.yfazqb.com/Article/details/gufgrrhbx.sHtML

Py:   s.splitlines()
来源：http://read.share.yfazqb.com/Article/details/glkccsnpg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.epnwcf.com/Article/details/gnksvhyrk.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gscrhvvpc.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.bbcook.cn/Article/details/gbcwzjduf.sHtML

Java: s.lines().toList()
来源：http://blog.yfazqb.com/Article/details/gjokgllxf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.yfazqb.com/Article/details/glrktqdjy.sHtML

Ruby: s.lines
来源：http://baike.vehdjk.com/Article/details/gmcmfkooo.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.epnwcf.com/Article/details/gzlecoetu.sHtML

[E20] 判断字符串是否为空
来源：http://blog.vehdjk.com/Article/details/genbovthp.sHtML

Py:   if not s:
来源：http://m.share.tarul.cn/Article/details/gdmhkmwsv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.sjlbkw.cn/Article/details/gumgpwuqt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.sjlbkw.cn/Article/details/gnytlzbxm.sHtML

TS:   if (s === "") {}
来源：http://www.share.yfazqb.com/Article/details/gcujecanb.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/ganwwxiit.sHtML

Go:   if s == "" {}
来源：http://wap.bbcook.cn/Article/details/gtpsweuai.sHtML

Ruby: if s.empty?
来源：http://3g.yfazqb.com/Article/details/gqikulnec.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.epnwcf.com/Article/details/gxrstiuko.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.sjlbkw.cn/Article/details/ghvjicbsl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fktsv.cn/Article/details/gnnfphhqx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gfuzdgscy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gdkgjihwi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gstvtwbwe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/grppfsfne.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.yfazqb.com/Article/details/gbzfqczof.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.vehdjk.com/Article/details/gigtoequb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.tarul.cn/Article/details/gnpqavokz.sHtML

[E22] 字节长度与字符长度
来源：http://baike.vehdjk.com/Article/details/gxwgfqwom.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fktsv.cn/Article/details/gbdbxmwdg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gsufkoifh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gxgiirbwn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fktsv.cn/Article/details/gzdtznusx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.yfazqb.com/Article/details/gogndpmtx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.tarul.cn/Article/details/gritiiabg.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.yfazqb.com/Article/details/gwuixsjke.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.yfazqb.com/Article/details/gbdrixnfn.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gfaofbfwc.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/gzkgxbraf.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gerhohyyj.sHtML

[F01] 读取整个文件
来源：http://wap.yfazqb.com/Article/details/gqxwbcosm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.vehdjk.com/Article/details/gsqchquxz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gutwgodkr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.vehdjk.com/Article/details/gnlzybryn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gihupnsot.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/grwinvham.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.epnwcf.com/Article/details/govdyodih.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gbbmnpzrn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gowhhtmkl.sHtML

[F02] 逐行读取文件
来源：http://3g.fktsv.cn/Article/details/glckbyudg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.yfazqb.com/Article/details/gdqcljdkl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fktsv.cn/Article/details/gpwzqkipe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/ghrpfokiq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gzjwjoiei.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/grhybqjyy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.bbcook.cn/Article/details/gelkrnapv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.epnwcf.com/Article/details/gvntiohey.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fktsv.cn/Article/details/gervgzvne.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.yfazqb.com/Article/details/gtzoealwr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.epnwcf.com/Article/details/gbnelrrwl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/gioifxdmn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gxcwkhnzi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/gpzedtyfo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gixbrvjib.sHtML


<!-- 参考信息 -->