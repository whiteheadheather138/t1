代发 wailian999

[D19] 按字段分组
来源：http://baike.sjlbkw.cn/Article/details/glawxdqij.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.tarul.cn/Article/details/gemtfdxiy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.bbcook.cn/Article/details/gxzbghufg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.tarul.cn/Article/details/gviintucy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.vehdjk.com/Article/details/gbvbcizsd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.sjlbkw.cn/Article/details/gzubzyarv.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.tarul.cn/Article/details/gtxmhtzrg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fktsv.cn/Article/details/gwgmtfdjc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.vehdjk.com/Article/details/gcqgfradz.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.epnwcf.com/Article/details/gmacnokdj.sHtML

Py:   Counter(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtkxtqyu.sHtML

PHP:  array_count_values($arr);
来源：http://wap.epnwcf.com/Article/details/guvduuzgc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gfmggvsrk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/glflvllqa.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.vehdjk.com/Article/details/ggjnjlfly.sHtML

Go:   // 手写 map[T]int
来源：http://3g.tarul.cn/Article/details/gybuupjyd.sHtML

Ruby: arr.tally
来源：http://read.share.fktsv.cn/Article/details/gboeibsyj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.bbcook.cn/Article/details/ghmpfjpzl.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.yfazqb.com/Article/details/gisqkwlki.sHtML

Py:   x in arr
来源：http://3g.vehdjk.com/Article/details/gdxzeluzk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.sjlbkw.cn/Article/details/gwtfsbkah.sHtML

JS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gjtjctfli.sHtML

TS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gntucktnz.sHtML

Java: list.contains(x)
来源：http://3g.tarul.cn/Article/details/gftdvznge.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gyygigcoq.sHtML

Ruby: arr.include?(x)
来源：http://www.share.bbcook.cn/Article/details/getuoqgaw.sHtML

C#:   list.Contains(x)
来源：http://mobile.yfazqb.com/Article/details/gbrqvihej.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.yfazqb.com/Article/details/glvtcczhi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gfbuudynp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.tarul.cn/Article/details/gqjeebabd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.yfazqb.com/Article/details/gvvyyevll.sHtML

TS:   [...arr];
来源：http://www.share.epnwcf.com/Article/details/gbfqygeir.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.vehdjk.com/Article/details/ghkpyucka.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.yfazqb.com/Article/details/gbvtokxln.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.sjlbkw.cn/Article/details/gcpjirrpw.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fktsv.cn/Article/details/gpggejqbu.sHtML

[D23] reduce 累积计算
来源：http://wap.tarul.cn/Article/details/gaehlcysl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.tarul.cn/Article/details/gyuzfjmrb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.epnwcf.com/Article/details/gbrccbbwv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gpdqmkuam.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/gihkdeqel.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.vehdjk.com/Article/details/gosyzroza.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/gfkpgqxgm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.epnwcf.com/Article/details/gipwlzalb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.bbcook.cn/Article/details/gqiluwghx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.vehdjk.com/Article/details/gvhgekkme.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.tarul.cn/Article/details/gjiknrhqi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gecmeqzki.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fktsv.cn/Article/details/gebfcregn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.vehdjk.com/Article/details/goparaari.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.vehdjk.com/Article/details/gyykkwzfq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.sjlbkw.cn/Article/details/gviqarzmb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fktsv.cn/Article/details/gdufslzhv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.vehdjk.com/Article/details/gkpecbshm.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.vehdjk.com/Article/details/gvpqnlsus.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.vehdjk.com/Article/details/gvxqfnmse.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.sjlbkw.cn/Article/details/gzvfiryhy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fktsv.cn/Article/details/gtygprfgc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.epnwcf.com/Article/details/gjzxfoewj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/ggspsisdu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fktsv.cn/Article/details/gyoqjttmi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.epnwcf.com/Article/details/gpohudtvh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.tarul.cn/Article/details/gccjnocok.sHtML

[D26] 数组转字符串
来源：http://wap.fktsv.cn/Article/details/guqxitfbz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fktsv.cn/Article/details/gaitfmilx.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.vehdjk.com/Article/details/gaqfwrosq.sHtML

JS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/goyadmsoj.sHtML

TS:   arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/gaymomfjw.sHtML

Java: String.join(", ", list)
来源：http://mobile.bbcook.cn/Article/details/genokjkkj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.bbcook.cn/Article/details/gjqvhqnua.sHtML

Ruby: arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gotqaghhw.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gwzfdgyoj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpwzqjqvt.sHtML

E. 字符串处理
来源：http://blog.bbcook.cn/Article/details/gfotzkoth.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gpzgigcan.sHtML

[E01] 拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gwhuodvey.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.yfazqb.com/Article/details/gyxsdkfvl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.tarul.cn/Article/details/grtjwipyz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/gvuowjgff.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gvaqmdnpp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.bbcook.cn/Article/details/gktisllww.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.epnwcf.com/Article/details/gpdqgejpn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.tarul.cn/Article/details/gsulcsdqw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gvxzwhrkk.sHtML

[E02] 重复字符串
来源：http://www.share.sjlbkw.cn/Article/details/gsamupsky.sHtML

Py:   "ab" * 3
来源：http://m.share.tarul.cn/Article/details/gpofoypmn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.yfazqb.com/Article/details/ghtbqdcvq.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gdvhbjaxo.sHtML

TS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/gmisqgnwq.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gbrxkmknn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fktsv.cn/Article/details/gniivmtac.sHtML

Ruby: "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/ggicnxfsh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/gzvubioal.sHtML

[E03] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gvyhuutqs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.tarul.cn/Article/details/gfchzmkfb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gxpfkcqwq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gefnrtdef.sHtML

TS:   s.slice(1, 4)
来源：http://3g.vehdjk.com/Article/details/ggtvhpmpk.sHtML

Java: s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/grpcogsbv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.bbcook.cn/Article/details/glodwyxli.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.vehdjk.com/Article/details/gztfafrtp.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.sjlbkw.cn/Article/details/gstcpmjpd.sHtML

[E04] 查找子串位置
来源：http://baike.epnwcf.com/Article/details/gmyuetdto.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.tarul.cn/Article/details/gklufesxw.sHtML

PHP:  strpos($s, "x");
来源：http://baike.yfazqb.com/Article/details/gbimfhprk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fktsv.cn/Article/details/guezuipfs.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gslmwlyje.sHtML

Java: s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gujepzvvo.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.epnwcf.com/Article/details/gslhtmwvh.sHtML

Ruby: s.index("x")
来源：http://blog.yfazqb.com/Article/details/gisfrqeir.sHtML

C#:   s.IndexOf("x")
来源：http://wap.epnwcf.com/Article/details/gkfhxopwb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.yfazqb.com/Article/details/gwduhykdq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.bbcook.cn/Article/details/gkvxxjrih.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.sjlbkw.cn/Article/details/gbxjjyswq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gtrjhvggh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.bbcook.cn/Article/details/gcoidfmke.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gamkooius.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.vehdjk.com/Article/details/gpsffwdpi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fktsv.cn/Article/details/gjbuzlhwi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.epnwcf.com/Article/details/goqequevj.sHtML

[E06] 替换子串
来源：http://blog.yfazqb.com/Article/details/gdllkwsro.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/guoxngubf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.bbcook.cn/Article/details/gkbgrxoon.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/georqkdyy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gfcpnyevy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gqxsbtpze.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/gcwaxzohq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/ghkauwncv.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.yfazqb.com/Article/details/gzzflldmf.sHtML

[E07] 按分隔符拆分
来源：http://3g.epnwcf.com/Article/details/ghvyvetyu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.epnwcf.com/Article/details/gypinzdia.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.epnwcf.com/Article/details/gdkmeslyl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.sjlbkw.cn/Article/details/ggpilmiwz.sHtML

TS:   s.split(",")
来源：http://3g.tarul.cn/Article/details/gcrsoprqn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.vehdjk.com/Article/details/gnzglkfiy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.epnwcf.com/Article/details/gwhcjgecn.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.sjlbkw.cn/Article/details/gshisrtto.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.epnwcf.com/Article/details/gsyvodrar.sHtML

[E08] 数组按分隔符合并
来源：http://wap.tarul.cn/Article/details/ghkmqrnkt.sHtML

Py:   ",".join(items)
来源：http://baike.fktsv.cn/Article/details/gzljqlgqm.sHtML

PHP:  implode(",", $items);
来源：http://read.share.yfazqb.com/Article/details/gvwvbniwb.sHtML

JS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gigynykha.sHtML

TS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gpugoufqg.sHtML

Java: String.join(",", items)
来源：http://baike.tarul.cn/Article/details/gtmyjvsmj.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.tarul.cn/Article/details/gaieshybx.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gbackxlqd.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fktsv.cn/Article/details/gxwgmqmpj.sHtML

[E09] 去除所有空白字符
来源：http://blog.fktsv.cn/Article/details/gipsjxmuz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.vehdjk.com/Article/details/gzjmxzenw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.tarul.cn/Article/details/gublizkrg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gedjqtbzh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.vehdjk.com/Article/details/gwddkzcut.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gflyywhkp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.tarul.cn/Article/details/gpsojzrdr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.bbcook.cn/Article/details/gvfdfhrgf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.bbcook.cn/Article/details/gknipqacl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.tarul.cn/Article/details/guwxsmwkj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.vehdjk.com/Article/details/gfpvvtmae.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.bbcook.cn/Article/details/guzwwgxzb.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/ggqcpsotr.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fktsv.cn/Article/details/glcsfidcl.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gwusceqak.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gsywfvrfu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gnsmxgdfq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.epnwcf.com/Article/details/geedlugxy.sHtML

[E11] 反转字符串
来源：http://blog.fktsv.cn/Article/details/gclcxktxc.sHtML

Py:   s[::-1]
来源：http://blog.bbcook.cn/Article/details/gkpmlgnno.sHtML

PHP:  strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gsuztbuse.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/guspfqonr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gjhmaslxb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gtouodndv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.yfazqb.com/Article/details/gmanzzhzm.sHtML

Ruby: s.reverse
来源：http://3g.vehdjk.com/Article/details/gndukkdni.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/gsrnsqfog.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.tarul.cn/Article/details/gqxxnbfox.sHtML

Py:   s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gzswwdzlz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.sjlbkw.cn/Article/details/gazuwyqfz.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/gtopcgwds.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.sjlbkw.cn/Article/details/gtblirxzp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/giliczcol.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.yfazqb.com/Article/details/gysprvllg.sHtML

Ruby: s.count("a")
来源：http://www.m.share.epnwcf.com/Article/details/glqsptlwt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fktsv.cn/Article/details/gjjwkjflq.sHtML

[E13] 逐字符遍历
来源：http://3g.bbcook.cn/Article/details/gftytzgtl.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.tarul.cn/Article/details/gesyfwcjo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.sjlbkw.cn/Article/details/gutcafzpb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/grkbfcoyz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/grzhaaedm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.vehdjk.com/Article/details/ghvcqnxmo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.sjlbkw.cn/Article/details/gtvlidkup.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.epnwcf.com/Article/details/gonhsoxtg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.epnwcf.com/Article/details/gsrndzndr.sHtML

[E14] URL 编码与 Base64
来源：http://blog.vehdjk.com/Article/details/gnmtciqhe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.epnwcf.com/Article/details/gxcfzmqmj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.bbcook.cn/Article/details/gaoctojll.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fktsv.cn/Article/details/gaefokjiy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.epnwcf.com/Article/details/gllefvzwj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/ggkgcqiyv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.epnwcf.com/Article/details/ghocyaduq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.epnwcf.com/Article/details/gqjuylirs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.vehdjk.com/Article/details/gzaumdskb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.bbcook.cn/Article/details/gcblwackk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzhdlgeh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.tarul.cn/Article/details/gdbhdbbyo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.tarul.cn/Article/details/gfuwcdygz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.tarul.cn/Article/details/gesdtdsnj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.bbcook.cn/Article/details/gwzfruzmu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.bbcook.cn/Article/details/gkfpytdyn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.bbcook.cn/Article/details/gwqytxter.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.bbcook.cn/Article/details/gbbokugcz.sHtML

[E16] 数字千分位
来源：http://www.share.epnwcf.com/Article/details/gbkbesrxi.sHtML

Py:   f"{1234567:,}"
来源：http://3g.epnwcf.com/Article/details/gopmwtmgl.sHtML

PHP:  number_format(1234567);
来源：http://baike.tarul.cn/Article/details/gmynqdoci.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.vehdjk.com/Article/details/gucxxanxx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/gmviytwky.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.vehdjk.com/Article/details/gdjmzvixt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.tarul.cn/Article/details/gnxqfebob.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.sjlbkw.cn/Article/details/geewggqgj.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.epnwcf.com/Article/details/gzlirriad.sHtML

[E17] 首字母大写
来源：http://www.blog.epnwcf.com/Article/details/ghmgnlqvx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fktsv.cn/Article/details/gsjgwzmdp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.epnwcf.com/Article/details/gmxaeatvv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/girjxamjo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/gpacjcnfd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.vehdjk.com/Article/details/gfvmpijei.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.tarul.cn/Article/details/gxfxuihpe.sHtML

Ruby: s.capitalize
来源：http://mobile.sjlbkw.cn/Article/details/gzninbjoi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.bbcook.cn/Article/details/gqnohruse.sHtML

[E18] 模板占位符替换
来源：http://www.blog.tarul.cn/Article/details/gllqasmsl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.vehdjk.com/Article/details/glkmeqonh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.epnwcf.com/Article/details/ghqjnmnml.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gdsvcwrhn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gyfkfxvia.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gnqesqjsy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gfuywtvmx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.epnwcf.com/Article/details/gbqwnxlsi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fktsv.cn/Article/details/gsalbomnk.sHtML

[E19] 多行文本按行拆分
来源：http://blog.sjlbkw.cn/Article/details/ghejlwvhq.sHtML

Py:   s.splitlines()
来源：http://www.blog.vehdjk.com/Article/details/gxhpsikti.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fktsv.cn/Article/details/gqjrywuxd.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.vehdjk.com/Article/details/grmghslsx.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gllgmswpa.sHtML

Java: s.lines().toList()
来源：http://www.share.vehdjk.com/Article/details/gyahlabnh.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.sjlbkw.cn/Article/details/gvefojwui.sHtML

Ruby: s.lines
来源：http://mobile.vehdjk.com/Article/details/gtkufxvlz.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/ggguhtqsx.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.epnwcf.com/Article/details/gaehfzcrm.sHtML

Py:   if not s:
来源：http://read.share.yfazqb.com/Article/details/gryeasinw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.vehdjk.com/Article/details/gliqmrdig.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.tarul.cn/Article/details/gavijywyq.sHtML

TS:   if (s === "") {}
来源：http://mobile.bbcook.cn/Article/details/gyoyqbdym.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gjpdkexgx.sHtML

Go:   if s == "" {}
来源：http://3g.sjlbkw.cn/Article/details/gleerrovh.sHtML

Ruby: if s.empty?
来源：http://baike.fktsv.cn/Article/details/gbzvztnud.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.bbcook.cn/Article/details/gtwlysqty.sHtML

[E21] 超长截断加省略号
来源：http://www.share.bbcook.cn/Article/details/gkfyehvve.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.epnwcf.com/Article/details/gcviojdln.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gyylsqtcw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gznwazyym.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gfocfjlcw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gymfredpo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.bbcook.cn/Article/details/gpgbcniji.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gajjvjqpq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gapzqfpjy.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.yfazqb.com/Article/details/gnsulwltb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.epnwcf.com/Article/details/gpmrqdbxs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gpkzrlped.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gneavwbyq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/gxekgwzil.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.vehdjk.com/Article/details/gcsvzabom.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.yfazqb.com/Article/details/getsjpjbf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gzayynpsf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.epnwcf.com/Article/details/geamsjfgp.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gapgnzgih.sHtML

F. 文件与目录
来源：http://m.share.sjlbkw.cn/Article/details/gilbpokit.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gdnczvllf.sHtML

[F01] 读取整个文件
来源：http://www.blog.epnwcf.com/Article/details/ggihdavlp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.bbcook.cn/Article/details/gvmxqidvl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/ggrzzfhxk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fktsv.cn/Article/details/gbodbeitq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gjkvvylpz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/golbaoyyi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.yfazqb.com/Article/details/gmvhkkxgm.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gbespnhah.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/glerimwvc.sHtML

[F02] 逐行读取文件
来源：http://read.share.bbcook.cn/Article/details/gclwmzwds.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.sjlbkw.cn/Article/details/gfxweoxug.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.sjlbkw.cn/Article/details/gvzeyehky.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/grdpmgeuv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/gfdsgpkgj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/gmghqfgdg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.bbcook.cn/Article/details/ggexmcqoh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.epnwcf.com/Article/details/gxdcnshxw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.epnwcf.com/Article/details/gtcmviiov.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.tarul.cn/Article/details/gdiecbmzd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.tarul.cn/Article/details/gsvtokmgn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gofpcoztz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/gitbkufcf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gcchvrnaq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.yfazqb.com/Article/details/grtgzznbr.sHtML


<!-- 参考信息 -->