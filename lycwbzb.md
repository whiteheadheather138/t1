代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://wap.epnwcf.com/Article/details/gaqajcikd.sHtML

JS:   arr.includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gvsnnfyzx.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gnbbcargo.sHtML

Java: list.contains(x)
来源：http://baike.sjlbkw.cn/Article/details/ggovicpad.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.vehdjk.com/Article/details/ghjrlgwqx.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/gooyrdzsp.sHtML

C#:   list.Contains(x)
来源：http://m.share.vehdjk.com/Article/details/gxuyalorq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.tarul.cn/Article/details/ggbusowin.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.yfazqb.com/Article/details/gsyvjouza.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.bbcook.cn/Article/details/ggrxfbymv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.epnwcf.com/Article/details/gpbmkbpak.sHtML

TS:   [...arr];
来源：http://blog.yfazqb.com/Article/details/gkfnghief.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fktsv.cn/Article/details/geyccnjdj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fktsv.cn/Article/details/gzhkxntfy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.vehdjk.com/Article/details/gpqrxzkkp.sHtML

C#:   new List<int>(list);
来源：http://baike.vehdjk.com/Article/details/gypiwgbde.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.sjlbkw.cn/Article/details/gimrwubzf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.tarul.cn/Article/details/gwcdpeubk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.vehdjk.com/Article/details/gscyufbkv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.vehdjk.com/Article/details/gqlylkiyh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/gutnkjrmv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.vehdjk.com/Article/details/gqzqrevbc.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/gdqbzqupv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.yfazqb.com/Article/details/grbtcpxzp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.vehdjk.com/Article/details/gyxolijrn.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.yfazqb.com/Article/details/gkjtgaian.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gkkrrjqrv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.yfazqb.com/Article/details/glwfsmokw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gdnldthne.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gqscbzesx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.epnwcf.com/Article/details/gjyvidiba.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.vehdjk.com/Article/details/gdufquhca.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.sjlbkw.cn/Article/details/grhmcwuvd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.sjlbkw.cn/Article/details/gnzraudcb.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.bbcook.cn/Article/details/gmafzrpds.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.bbcook.cn/Article/details/gdxsbdwus.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fktsv.cn/Article/details/gwinfqdtz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.sjlbkw.cn/Article/details/gabasupzz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.yfazqb.com/Article/details/gigwtpqgj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.yfazqb.com/Article/details/gxonpqusx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.sjlbkw.cn/Article/details/gbycwydyn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.yfazqb.com/Article/details/gxfsduflu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.bbcook.cn/Article/details/gfhhqyetq.sHtML

[D26] 数组转字符串
来源：http://blog.bbcook.cn/Article/details/gnhpxmwdu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.tarul.cn/Article/details/gkyzuyizn.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.bbcook.cn/Article/details/gdvqwrelm.sHtML

JS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gcvcycyiv.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gssoglpvo.sHtML

Java: String.join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gmqqmlcjz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.yfazqb.com/Article/details/goiozpkjh.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gixluyxno.sHtML

C#:   string.Join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gxhxzunvi.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gqswnncxg.sHtML

E. 字符串处理
来源：http://www.m.share.tarul.cn/Article/details/glgnbwgdx.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/godrgdoub.sHtML

[E01] 拼接字符串
来源：http://wap.epnwcf.com/Article/details/gskftexcm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.yfazqb.com/Article/details/glimmcafr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.vehdjk.com/Article/details/gvdtzqzxl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/gbrsqjydn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gfpwraesx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.bbcook.cn/Article/details/gscwfszos.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvtsemdw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.bbcook.cn/Article/details/gidmsxjob.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.bbcook.cn/Article/details/gzmcojtuu.sHtML

[E02] 重复字符串
来源：http://wap.tarul.cn/Article/details/grnffepfb.sHtML

Py:   "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/gejykqcqc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.yfazqb.com/Article/details/gnvhdbiyr.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gutyfwlka.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gmtwkrcxk.sHtML

Java: "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gmtwohtbl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.bbcook.cn/Article/details/gnqtlsjug.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/gbphuekkq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.tarul.cn/Article/details/gezgarwlq.sHtML

[E03] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/gyzgkspfj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.yfazqb.com/Article/details/gdpsoocfm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/glulrvrnk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/giwqcffvg.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gqtdrendy.sHtML

Java: s.substring(1, 4)
来源：http://wap.epnwcf.com/Article/details/gamllrmig.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.yfazqb.com/Article/details/glvtwdcbg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.tarul.cn/Article/details/gdceaawvu.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.sjlbkw.cn/Article/details/ghbctcfbu.sHtML

[E04] 查找子串位置
来源：http://baike.epnwcf.com/Article/details/gcwlgmtjl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.bbcook.cn/Article/details/gctudpljv.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fktsv.cn/Article/details/gnucqfkth.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fktsv.cn/Article/details/gxohobmbx.sHtML

TS:   s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gvkvhkqer.sHtML

Java: s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/govjouxlz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.yfazqb.com/Article/details/gghrtgikj.sHtML

Ruby: s.index("x")
来源：http://3g.fktsv.cn/Article/details/grrmcvafb.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.epnwcf.com/Article/details/gqtolrkbo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.sjlbkw.cn/Article/details/gkqhubpdx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.tarul.cn/Article/details/gfabvabxj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.vehdjk.com/Article/details/gdfhjvbqo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.bbcook.cn/Article/details/gdeveqrjq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gbzxrbonf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.bbcook.cn/Article/details/gvkacodmz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fktsv.cn/Article/details/glujajyax.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.vehdjk.com/Article/details/gbeytldgq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gwqaxbmky.sHtML

[E06] 替换子串
来源：http://wap.tarul.cn/Article/details/gbawkrnty.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/gnimtjxwk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.vehdjk.com/Article/details/grqydirop.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gucuxsemf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gkgofsieh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gkcrtxwqc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.yfazqb.com/Article/details/geprlmlkx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gmxuvhayj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/guesyrdnz.sHtML

[E07] 按分隔符拆分
来源：http://read.share.bbcook.cn/Article/details/gosufnnke.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.tarul.cn/Article/details/gjnpqpodk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gfqpgojxm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.tarul.cn/Article/details/gloxzywfy.sHtML

TS:   s.split(",")
来源：http://blog.vehdjk.com/Article/details/gjiaymtyx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.epnwcf.com/Article/details/gzvlffzmn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fktsv.cn/Article/details/gzdedtfpp.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.vehdjk.com/Article/details/gayergqvd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.yfazqb.com/Article/details/geybusqtc.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.vehdjk.com/Article/details/gbjyzzbci.sHtML

Py:   ",".join(items)
来源：http://wap.vehdjk.com/Article/details/gpwgcoabe.sHtML

PHP:  implode(",", $items);
来源：http://3g.tarul.cn/Article/details/gbazlntbm.sHtML

JS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gujpkjwqt.sHtML

TS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/glgdeiudz.sHtML

Java: String.join(",", items)
来源：http://blog.vehdjk.com/Article/details/gjnklmmtl.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.sjlbkw.cn/Article/details/ggnubgljf.sHtML

Ruby: items.join(",")
来源：http://www.share.fktsv.cn/Article/details/ghunufwmj.sHtML

C#:   string.Join(",", items)
来源：http://m.share.yfazqb.com/Article/details/godqtrtqb.sHtML

[E09] 去除所有空白字符
来源：http://wap.tarul.cn/Article/details/gmjeplrxi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.vehdjk.com/Article/details/gfyenuqsh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.tarul.cn/Article/details/gjkdysudq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/gzpfvhpgi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/gvhwhbjxt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.epnwcf.com/Article/details/gixwyyate.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.yfazqb.com/Article/details/gusveebpt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fktsv.cn/Article/details/gdvgfefke.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.bbcook.cn/Article/details/gvgfcahxp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fktsv.cn/Article/details/gghnnfpwg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.epnwcf.com/Article/details/gpsucuunw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.bbcook.cn/Article/details/gjjwvljdy.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/giukfrtni.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gdmznidku.sHtML

Java: String.format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gplrstzrr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gewweqjep.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/grsgsxtjf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fktsv.cn/Article/details/gyygcnfls.sHtML

[E11] 反转字符串
来源：http://blog.sjlbkw.cn/Article/details/gdkgzhesd.sHtML

Py:   s[::-1]
来源：http://wap.fktsv.cn/Article/details/gnooloojw.sHtML

PHP:  strrev($s);
来源：http://mobile.bbcook.cn/Article/details/glewirkki.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gbazusyca.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/glpocgjzg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.vehdjk.com/Article/details/gysklnska.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.sjlbkw.cn/Article/details/gqttcpjzo.sHtML

Ruby: s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gblcyforv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gtkdnrnsp.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.vehdjk.com/Article/details/gpqmstqvn.sHtML

Py:   s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gtedakeag.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.sjlbkw.cn/Article/details/gvuioxmke.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/gzvbkiols.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gpnparrko.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.yfazqb.com/Article/details/gqjdbwtws.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.tarul.cn/Article/details/gqcccovjo.sHtML

Ruby: s.count("a")
来源：http://baike.sjlbkw.cn/Article/details/gonsydvpp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.tarul.cn/Article/details/gnmsusbyb.sHtML

[E13] 逐字符遍历
来源：http://3g.tarul.cn/Article/details/geqpwglva.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.epnwcf.com/Article/details/gwbcgalhh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.tarul.cn/Article/details/golcgpcku.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/gsdyxkjdi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gefviyvce.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.vehdjk.com/Article/details/gmdmedpdo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.vehdjk.com/Article/details/gpsowgoeo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.sjlbkw.cn/Article/details/ghpegmpct.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.bbcook.cn/Article/details/gzhwxjdbj.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.bbcook.cn/Article/details/gucuprtfk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.bbcook.cn/Article/details/gzrxofggw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fktsv.cn/Article/details/gxiybpqxo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fktsv.cn/Article/details/gzqabhngu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.bbcook.cn/Article/details/gxxyzudjm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.epnwcf.com/Article/details/glangrmnv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.vehdjk.com/Article/details/gchkgblmg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fktsv.cn/Article/details/glfriycnu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.yfazqb.com/Article/details/gqzitkvja.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.vehdjk.com/Article/details/gdyfklxva.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.sjlbkw.cn/Article/details/gcpswxbub.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.bbcook.cn/Article/details/gdttepjrj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.sjlbkw.cn/Article/details/ggytbutxx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.yfazqb.com/Article/details/gkwwlgccj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.vehdjk.com/Article/details/glzaagtnx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.bbcook.cn/Article/details/gaqtvfpdy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.bbcook.cn/Article/details/ggsbjzzqt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.yfazqb.com/Article/details/gdxrwzqkl.sHtML

[E16] 数字千分位
来源：http://3g.epnwcf.com/Article/details/guhvndvgi.sHtML

Py:   f"{1234567:,}"
来源：http://wap.sjlbkw.cn/Article/details/gyuggsqya.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.tarul.cn/Article/details/guichfnfw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/gckehhmqr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/gkrupideb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.tarul.cn/Article/details/grechkgfk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.yfazqb.com/Article/details/gkuurxpmc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.vehdjk.com/Article/details/gjzvnbizy.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fktsv.cn/Article/details/gpuirvrir.sHtML

[E17] 首字母大写
来源：http://www.share.tarul.cn/Article/details/ghqvafqfx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.sjlbkw.cn/Article/details/gyaxphvph.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.bbcook.cn/Article/details/gcngcookf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/gfdiulcwm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/gjbgwrhup.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.tarul.cn/Article/details/gzhcnqyzt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.tarul.cn/Article/details/gapvybgjs.sHtML

Ruby: s.capitalize
来源：http://www.share.tarul.cn/Article/details/gwhiiweah.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.sjlbkw.cn/Article/details/ggtphoneh.sHtML

[E18] 模板占位符替换
来源：http://blog.bbcook.cn/Article/details/gxhqppgzo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.vehdjk.com/Article/details/grksckwup.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.epnwcf.com/Article/details/gevprolpz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gaerlrkwe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gphbfrmlc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gwnuxtoni.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.tarul.cn/Article/details/gklrhoufj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.sjlbkw.cn/Article/details/gaxonjnyq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fktsv.cn/Article/details/gbyekxmjp.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.vehdjk.com/Article/details/gorbfrivz.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/gvfpgqbxl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.yfazqb.com/Article/details/gxnewgkhx.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/gjhtvjyzw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gldqjwhdw.sHtML

Java: s.lines().toList()
来源：http://3g.sjlbkw.cn/Article/details/gkzyjuyny.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.bbcook.cn/Article/details/grffjzgxv.sHtML

Ruby: s.lines
来源：http://read.share.epnwcf.com/Article/details/gqftdacpu.sHtML

C#:   s.Split('\n')
来源：http://read.share.epnwcf.com/Article/details/geddoddmh.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.vehdjk.com/Article/details/gdclrfkkh.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/ggnsoxvkm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.epnwcf.com/Article/details/gonlcbttn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.tarul.cn/Article/details/gnzfhduop.sHtML

TS:   if (s === "") {}
来源：http://read.share.yfazqb.com/Article/details/govjoggqz.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gtvuewtli.sHtML

Go:   if s == "" {}
来源：http://mobile.yfazqb.com/Article/details/gessjxzfy.sHtML

Ruby: if s.empty?
来源：http://www.m.share.bbcook.cn/Article/details/gkqgobmsx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.bbcook.cn/Article/details/gkjwyeeua.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.epnwcf.com/Article/details/gakxohvai.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.bbcook.cn/Article/details/ggnznwctx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gicdezmaj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/grfwkdrgn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gpfbciadz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gqmedlefb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.yfazqb.com/Article/details/gaurtfwvu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gtbdkjlul.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/goozpsvml.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.sjlbkw.cn/Article/details/gartcdfnv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gpasabuyy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gjozjkkqc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gmmheiibo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.epnwcf.com/Article/details/gepddxmte.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/grttzawko.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fktsv.cn/Article/details/grdihhscz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.tarul.cn/Article/details/gtupswykb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.yfazqb.com/Article/details/gcaghhulr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqhzefglz.sHtML

F. 文件与目录
来源：http://www.blog.tarul.cn/Article/details/gbjvwttwe.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gijvuknic.sHtML

[F01] 读取整个文件
来源：http://wap.yfazqb.com/Article/details/gukaoupmh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.sjlbkw.cn/Article/details/glnjlfsky.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gsrcwftlq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fktsv.cn/Article/details/gojtrpcyj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/ggzjrfcor.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gzraxiuso.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.sjlbkw.cn/Article/details/gakgtfadr.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gkgimdhuj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.vehdjk.com/Article/details/ggyfmgale.sHtML

[F02] 逐行读取文件
来源：http://wap.yfazqb.com/Article/details/gwfnxgjaw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.yfazqb.com/Article/details/gxtshiocv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.epnwcf.com/Article/details/gedhounwi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fktsv.cn/Article/details/gmidrdkrg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/gyyksncdb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/ggpdvwwhf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.bbcook.cn/Article/details/gqhiuzovq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.vehdjk.com/Article/details/gbgvbjhyf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fktsv.cn/Article/details/gzyrjpseo.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.vehdjk.com/Article/details/gkjkbqoxn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.epnwcf.com/Article/details/gvtzvybai.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gttxyezsc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gygjjsksa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/gnxhzoxal.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.bbcook.cn/Article/details/gtnmahspo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzmzeire.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.epnwcf.com/Article/details/gwflakpur.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/gifydzauw.sHtML

[F04] 追加写入文件
来源：http://m.share.sjlbkw.cn/Article/details/gqgnavwti.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.epnwcf.com/Article/details/gusufixlr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.sjlbkw.cn/Article/details/geugkumvm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/ghrcyupvp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/gmxilnono.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fktsv.cn/Article/details/gsjawgbnh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.bbcook.cn/Article/details/gkpmuvrlr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.epnwcf.com/Article/details/gznisyfhj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.vehdjk.com/Article/details/goxdxbojl.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.tarul.cn/Article/details/ggunwulkd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.sjlbkw.cn/Article/details/gbkccnxau.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gtzcawivr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gjkilzqzn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gwpuzjqtj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gktyibuqy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.sjlbkw.cn/Article/details/gnnebsiag.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gqrbthbqr.sHtML


<!-- 参考信息 -->