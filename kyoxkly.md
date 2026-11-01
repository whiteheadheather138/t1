代发 wailian999

Ruby: arr.tally
来源：http://blog.fktsv.cn/Article/details/gwlhpzafe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.epnwcf.com/Article/details/grylgkhza.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.yfazqb.com/Article/details/gpulcjktl.sHtML

Py:   x in arr
来源：http://blog.epnwcf.com/Article/details/glsjuxyyi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.sjlbkw.cn/Article/details/gllkgnrpj.sHtML

JS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/gtgaalehy.sHtML

TS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/gfbqhvfoi.sHtML

Java: list.contains(x)
来源：http://wap.bbcook.cn/Article/details/gasferyok.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fktsv.cn/Article/details/gjwmxzbqn.sHtML

Ruby: arr.include?(x)
来源：http://mobile.yfazqb.com/Article/details/gbbysawjx.sHtML

C#:   list.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gesqmjfuz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.epnwcf.com/Article/details/gyhahujci.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.yfazqb.com/Article/details/gnfciujjj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fktsv.cn/Article/details/gtejudhxn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.sjlbkw.cn/Article/details/gdhohuhrw.sHtML

TS:   [...arr];
来源：http://www.share.fktsv.cn/Article/details/gkiqkvlym.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.yfazqb.com/Article/details/gybqxgiqq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.vehdjk.com/Article/details/gamxmikzo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.bbcook.cn/Article/details/gwoictjpg.sHtML

C#:   new List<int>(list);
来源：http://read.share.bbcook.cn/Article/details/gzmhivuwn.sHtML

[D23] reduce 累积计算
来源：http://wap.fktsv.cn/Article/details/guhhksowh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.epnwcf.com/Article/details/gxsnwvyst.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.epnwcf.com/Article/details/gedmomxox.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/gcgwkywzo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gzkdojmfc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.yfazqb.com/Article/details/gooqgdmfg.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/ggwnkjiry.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.vehdjk.com/Article/details/grzqxrryd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.bbcook.cn/Article/details/geybqsxgg.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.yfazqb.com/Article/details/geeavvyok.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.epnwcf.com/Article/details/gjjagvkdu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.sjlbkw.cn/Article/details/gmvrxirkv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gdcdboduk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gjvqpehkf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/gfqdyluic.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.bbcook.cn/Article/details/gpccudltw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fktsv.cn/Article/details/gvxcbmfxt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.tarul.cn/Article/details/gkpvjuidn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.yfazqb.com/Article/details/gasrbdqza.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzumfuiv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fktsv.cn/Article/details/gzsupgeod.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.epnwcf.com/Article/details/ghjfreuov.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.sjlbkw.cn/Article/details/gyglkpcqo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.tarul.cn/Article/details/gbmbzlyub.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.epnwcf.com/Article/details/geyexkvnm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.bbcook.cn/Article/details/ggmkqtyit.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.bbcook.cn/Article/details/gurxlgzse.sHtML

[D26] 数组转字符串
来源：http://mobile.yfazqb.com/Article/details/gfyukkgrm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.sjlbkw.cn/Article/details/gqtuovdxl.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.yfazqb.com/Article/details/gndpxnfag.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gnkatatqy.sHtML

TS:   arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gajyumwep.sHtML

Java: String.join(", ", list)
来源：http://baike.bbcook.cn/Article/details/ghpnzrnaq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.epnwcf.com/Article/details/gipchyqhg.sHtML

Ruby: arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gtbyedbgb.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.yfazqb.com/Article/details/gwboejarn.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtmhhzymv.sHtML

E. 字符串处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gsslybqnd.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gmyheagfw.sHtML

[E01] 拼接字符串
来源：http://3g.epnwcf.com/Article/details/gbzvmpvqx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.tarul.cn/Article/details/gsoxwrkrv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fktsv.cn/Article/details/glhsrjfgp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gvhqdfpzy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/ggmmlyjot.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.yfazqb.com/Article/details/gazhesevy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.yfazqb.com/Article/details/gkpimpnmg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.sjlbkw.cn/Article/details/gwrkagyjm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gtvqklihn.sHtML

[E02] 重复字符串
来源：http://www.blog.tarul.cn/Article/details/ggnbaaivq.sHtML

Py:   "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/gxbnczvnh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.epnwcf.com/Article/details/gqosrrnhh.sHtML

JS:   "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/ghdzdlcrm.sHtML

TS:   "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/geoqinong.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gamgyndai.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.vehdjk.com/Article/details/ghjbdohkh.sHtML

Ruby: "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/gvfmniqow.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.vehdjk.com/Article/details/gudoiyltj.sHtML

[E03] 截取子串
来源：http://baike.vehdjk.com/Article/details/gmvebqfhl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.yfazqb.com/Article/details/gxspsxfav.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gbfpshcxq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.tarul.cn/Article/details/gfafalbug.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fktsv.cn/Article/details/gmpzjxieo.sHtML

Java: s.substring(1, 4)
来源：http://3g.fktsv.cn/Article/details/gbhramxix.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.bbcook.cn/Article/details/guzkihrvc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.vehdjk.com/Article/details/gxtoovimj.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.vehdjk.com/Article/details/geoprnqxj.sHtML

[E04] 查找子串位置
来源：http://baike.epnwcf.com/Article/details/gkbniwxev.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.tarul.cn/Article/details/gjrmphutb.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fktsv.cn/Article/details/gnogtompm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.tarul.cn/Article/details/gilmshecm.sHtML

TS:   s.indexOf("x")
来源：http://baike.tarul.cn/Article/details/gifebyzed.sHtML

Java: s.indexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gyqszuuhe.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.vehdjk.com/Article/details/gjsrfgdjo.sHtML

Ruby: s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/gghdhhuyg.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gtgmxssrb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.yfazqb.com/Article/details/gkrhdiqes.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.tarul.cn/Article/details/guoqosqce.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fktsv.cn/Article/details/gleuugmyp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.yfazqb.com/Article/details/guepbzpsb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.sjlbkw.cn/Article/details/gdofjloxc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/gcyteablg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.yfazqb.com/Article/details/ghnoxkcex.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.bbcook.cn/Article/details/ghqqudzay.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/glswbunxf.sHtML

[E06] 替换子串
来源：http://baike.vehdjk.com/Article/details/gplltucwy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.tarul.cn/Article/details/gxqybcpis.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.bbcook.cn/Article/details/gfjloytkz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/govxunqam.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gnlhabnwg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/glbqrgxaq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gkhtomnik.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/ghkrplgkb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gikhzeepi.sHtML

[E07] 按分隔符拆分
来源：http://www.share.vehdjk.com/Article/details/gsxixyzsi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.bbcook.cn/Article/details/gtcaazzth.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gdiadvnnn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gemptcccg.sHtML

TS:   s.split(",")
来源：http://baike.vehdjk.com/Article/details/gjrewmkfn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.tarul.cn/Article/details/gcxkipnwx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.bbcook.cn/Article/details/gfokkrzsg.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.bbcook.cn/Article/details/gmoqyowze.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.bbcook.cn/Article/details/gnzwkfrln.sHtML

[E08] 数组按分隔符合并
来源：http://3g.yfazqb.com/Article/details/gvpcqtfki.sHtML

Py:   ",".join(items)
来源：http://3g.yfazqb.com/Article/details/gzwndcjxr.sHtML

PHP:  implode(",", $items);
来源：http://m.share.vehdjk.com/Article/details/grcleydps.sHtML

JS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/guuxghbyt.sHtML

TS:   items.join(",")
来源：http://blog.fktsv.cn/Article/details/gwuvjgnrj.sHtML

Java: String.join(",", items)
来源：http://blog.fktsv.cn/Article/details/gerbbibgf.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.yfazqb.com/Article/details/glxhheoew.sHtML

Ruby: items.join(",")
来源：http://wap.epnwcf.com/Article/details/glmbtdcdb.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.yfazqb.com/Article/details/ghsnjnuam.sHtML

[E09] 去除所有空白字符
来源：http://wap.yfazqb.com/Article/details/gfkvjouye.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.epnwcf.com/Article/details/gbalhmgva.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.bbcook.cn/Article/details/ghvrfnvzo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.vehdjk.com/Article/details/gxkfeselv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/gdjerzmxn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.bbcook.cn/Article/details/goxkhmurg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.epnwcf.com/Article/details/gefrzmrmn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fktsv.cn/Article/details/gziiptnjx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fktsv.cn/Article/details/ghkmgiaop.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.epnwcf.com/Article/details/grmklrqjr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gjswamyao.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.bbcook.cn/Article/details/gyjsbhtpl.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gmwkdurpa.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/glyhweedj.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gaionnefq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gtaybunjn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gtrivszda.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.sjlbkw.cn/Article/details/gvpyripch.sHtML

[E11] 反转字符串
来源：http://mobile.fktsv.cn/Article/details/gyoqjgmqa.sHtML

Py:   s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gqxgeokuk.sHtML

PHP:  strrev($s);
来源：http://mobile.bbcook.cn/Article/details/gekjzfnfq.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gdcsgbtro.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/glmzfhnzw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.tarul.cn/Article/details/gfguqdudg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.bbcook.cn/Article/details/gxgtawrvj.sHtML

Ruby: s.reverse
来源：http://mobile.epnwcf.com/Article/details/gaoyigozk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gvqesybuv.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.tarul.cn/Article/details/gnnvnhnlk.sHtML

Py:   s.count("a")
来源：http://read.share.fktsv.cn/Article/details/gzfqjgzki.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fktsv.cn/Article/details/gqsbqnrmv.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gqufjasgy.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.yfazqb.com/Article/details/gihgrtmuc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.bbcook.cn/Article/details/gftgreojq.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.yfazqb.com/Article/details/gmaiowdnc.sHtML

Ruby: s.count("a")
来源：http://mobile.tarul.cn/Article/details/gtkmxvboh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.sjlbkw.cn/Article/details/gfouatqyi.sHtML

[E13] 逐字符遍历
来源：http://wap.bbcook.cn/Article/details/gogzuazwv.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.sjlbkw.cn/Article/details/gcpqlyvro.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fktsv.cn/Article/details/gaywygbtu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/gymrnoqva.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gihxcyipf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.tarul.cn/Article/details/gxwsxqhas.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.yfazqb.com/Article/details/gvqtudlju.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.epnwcf.com/Article/details/gxierhwrq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gqiflkxrc.sHtML

[E14] URL 编码与 Base64
来源：http://wap.sjlbkw.cn/Article/details/goqbxztnq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.epnwcf.com/Article/details/gvkcxdybe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gleyhxmtg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.yfazqb.com/Article/details/glizscdig.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.vehdjk.com/Article/details/ghnregxjh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/guvkejngu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.tarul.cn/Article/details/grkdgznic.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.vehdjk.com/Article/details/govwdfoua.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.epnwcf.com/Article/details/gwhektasg.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.tarul.cn/Article/details/gkdamvdxl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.sjlbkw.cn/Article/details/gmwatncpc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.yfazqb.com/Article/details/ggimgpjjx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.bbcook.cn/Article/details/gpqkjozex.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fktsv.cn/Article/details/ghxrugkwu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.vehdjk.com/Article/details/gbftqlszi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.bbcook.cn/Article/details/grzdylefi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.yfazqb.com/Article/details/gyghotgjf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.tarul.cn/Article/details/gzpxdcrqm.sHtML

[E16] 数字千分位
来源：http://baike.yfazqb.com/Article/details/gbbmingva.sHtML

Py:   f"{1234567:,}"
来源：http://blog.yfazqb.com/Article/details/gxhytgojq.sHtML

PHP:  number_format(1234567);
来源：http://www.share.epnwcf.com/Article/details/gflusvlus.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gjbldzils.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gzosjysqt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.bbcook.cn/Article/details/ghqfchnen.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.tarul.cn/Article/details/gtkupeokg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.vehdjk.com/Article/details/gfdawnzyo.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fktsv.cn/Article/details/gqqjtbnys.sHtML

[E17] 首字母大写
来源：http://wap.bbcook.cn/Article/details/gdegrpaaj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.bbcook.cn/Article/details/gbhjxuprn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fktsv.cn/Article/details/gxgxunkiu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gmqrnprqh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fktsv.cn/Article/details/gsvhmkfap.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/gihwwikhf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.tarul.cn/Article/details/goovbnrrt.sHtML

Ruby: s.capitalize
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkyhnexe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.vehdjk.com/Article/details/gnnicgcfc.sHtML

[E18] 模板占位符替换
来源：http://www.blog.tarul.cn/Article/details/gxjmqijsz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.vehdjk.com/Article/details/gtioqlfza.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.epnwcf.com/Article/details/gibeljhuz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/ggexedxvb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gvmgiqxdx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gqapsuqyn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.yfazqb.com/Article/details/gabhfqrrw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.tarul.cn/Article/details/gsovqlslq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.epnwcf.com/Article/details/gfpfeedyp.sHtML

[E19] 多行文本按行拆分
来源：http://3g.yfazqb.com/Article/details/gzoxgojfl.sHtML

Py:   s.splitlines()
来源：http://mobile.fktsv.cn/Article/details/gdhbunhyc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/ghytvpact.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.yfazqb.com/Article/details/gcoiogzjr.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.epnwcf.com/Article/details/gobeswyiv.sHtML

Java: s.lines().toList()
来源：http://wap.sjlbkw.cn/Article/details/gkanbvsuw.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.epnwcf.com/Article/details/gvwnvggxe.sHtML

Ruby: s.lines
来源：http://baike.fktsv.cn/Article/details/gqeyrwktq.sHtML

C#:   s.Split('\n')
来源：http://baike.sjlbkw.cn/Article/details/gehhzucnp.sHtML

[E20] 判断字符串是否为空
来源：http://blog.sjlbkw.cn/Article/details/ghybutuyz.sHtML

Py:   if not s:
来源：http://blog.fktsv.cn/Article/details/gierxqxof.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fktsv.cn/Article/details/gkhkduwyo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.vehdjk.com/Article/details/grulyhgpd.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.bbcook.cn/Article/details/gigbkkeyr.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gamawcmub.sHtML

Go:   if s == "" {}
来源：http://baike.yfazqb.com/Article/details/gzbgdldza.sHtML

Ruby: if s.empty?
来源：http://wap.vehdjk.com/Article/details/giztfheta.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.vehdjk.com/Article/details/grmuplato.sHtML

[E21] 超长截断加省略号
来源：http://www.share.yfazqb.com/Article/details/gczrjlwqn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.yfazqb.com/Article/details/gpumjvsys.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gjvshattw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/ggbiewjcg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/grctwvpkd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gveteygxg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.sjlbkw.cn/Article/details/gevkunynq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gugpalzjs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.bbcook.cn/Article/details/gaasdodxr.sHtML

[E22] 字节长度与字符长度
来源：http://3g.tarul.cn/Article/details/ggalijrki.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.yfazqb.com/Article/details/ginhyieog.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gdjmkxchp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gzwqkhzkl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fktsv.cn/Article/details/glmbewziw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.epnwcf.com/Article/details/gzcaodegf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.bbcook.cn/Article/details/gknmmgptq.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.yfazqb.com/Article/details/gvuwltqqu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fktsv.cn/Article/details/gqiflgvez.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjryzmxbo.sHtML

F. 文件与目录
来源：http://mobile.epnwcf.com/Article/details/gaohcxefw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gsbulbkjr.sHtML

[F01] 读取整个文件
来源：http://m.share.tarul.cn/Article/details/ghzpubiql.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fktsv.cn/Article/details/gflyldbee.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gtoogvimv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fktsv.cn/Article/details/gtucyxqkf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.tarul.cn/Article/details/giuthltia.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gdbycmbud.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.bbcook.cn/Article/details/gurluejnq.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gwoekbvrw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.yfazqb.com/Article/details/ggoytozkf.sHtML

[F02] 逐行读取文件
来源：http://read.share.epnwcf.com/Article/details/gpctqrrqa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.vehdjk.com/Article/details/gohrrblqa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.vehdjk.com/Article/details/gfuuccvzy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/ggqmvdfag.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gwleqovkg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gtfqozlta.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.vehdjk.com/Article/details/ggfrveoen.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.bbcook.cn/Article/details/gwjgbvqxm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.tarul.cn/Article/details/gcybktjrz.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fktsv.cn/Article/details/gpfvoemss.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.epnwcf.com/Article/details/gryyzcvft.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.sjlbkw.cn/Article/details/gyecsvtbv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gsbkwbejn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gsrihznxv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.epnwcf.com/Article/details/gjwrbtqow.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.yfazqb.com/Article/details/gagxbbjdc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.sjlbkw.cn/Article/details/guzhnocpq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gzswssxoz.sHtML

[F04] 追加写入文件
来源：http://www.m.share.sjlbkw.cn/Article/details/giipmmnzq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.yfazqb.com/Article/details/gxskdaolz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fktsv.cn/Article/details/guwxzxjpr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gnrqixwud.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gtbbpporv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.bbcook.cn/Article/details/gqsqtmhbm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.epnwcf.com/Article/details/gokaulfub.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.yfazqb.com/Article/details/gfixykoeq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.tarul.cn/Article/details/gthmrvwaz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjpmtqef.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.yfazqb.com/Article/details/gxhikiekd.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.epnwcf.com/Article/details/gtwmyqbnq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gkwussdpw.sHtML


<!-- 参考信息 -->