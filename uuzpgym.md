代发 wailian999

Ruby: arr.tally
来源：http://www.share.yfazqb.com/Article/details/gespjltpj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fktsv.cn/Article/details/gpwcbvvbf.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.tarul.cn/Article/details/gzzxrshyl.sHtML

Py:   x in arr
来源：http://read.share.fktsv.cn/Article/details/gjjksriyo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fktsv.cn/Article/details/gzbpmidxv.sHtML

JS:   arr.includes(x)
来源：http://wap.yfazqb.com/Article/details/ghtfomcib.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gdgpdleqk.sHtML

Java: list.contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/ghyamrjuj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gimjcdfgh.sHtML

Ruby: arr.include?(x)
来源：http://baike.fktsv.cn/Article/details/gnpbknrla.sHtML

C#:   list.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gxibwnwir.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.yfazqb.com/Article/details/gakncipok.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gdyxrzlgi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.tarul.cn/Article/details/gqxaqctke.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.vehdjk.com/Article/details/gkwdejdjc.sHtML

TS:   [...arr];
来源：http://baike.bbcook.cn/Article/details/gobjevrix.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.epnwcf.com/Article/details/gjabpfjdx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlagjduy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.vehdjk.com/Article/details/gjigugeda.sHtML

C#:   new List<int>(list);
来源：http://baike.epnwcf.com/Article/details/gmiwytyow.sHtML

[D23] reduce 累积计算
来源：http://wap.bbcook.cn/Article/details/genzlrmdh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.vehdjk.com/Article/details/ginztedaf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.vehdjk.com/Article/details/gknywuugj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gfcktljgo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gcoegwrpq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.sjlbkw.cn/Article/details/gngmstncn.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/gpozbtusm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.epnwcf.com/Article/details/gotzdgpvz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.sjlbkw.cn/Article/details/gtbjnbzdt.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.sjlbkw.cn/Article/details/gxpkhcyfa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.yfazqb.com/Article/details/ghpsldgvk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fktsv.cn/Article/details/gcjwmuwfw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fktsv.cn/Article/details/gwibjlbnh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gjxpmquxn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.epnwcf.com/Article/details/gnmncnojw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.sjlbkw.cn/Article/details/gstvwyvvz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.tarul.cn/Article/details/gutihowdy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.vehdjk.com/Article/details/gufddebtj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.epnwcf.com/Article/details/gkallujfm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.bbcook.cn/Article/details/goxeayvyv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.yfazqb.com/Article/details/gsdbiicig.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gmtuezghr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.tarul.cn/Article/details/gykmuvxxq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gygopprvs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.bbcook.cn/Article/details/gacgqvdtw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.sjlbkw.cn/Article/details/gkrqbrcgk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.tarul.cn/Article/details/gxcsusdnk.sHtML

[D26] 数组转字符串
来源：http://www.share.epnwcf.com/Article/details/gdjrpmizk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.bbcook.cn/Article/details/gcveslfhi.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.vehdjk.com/Article/details/gvdpckiwy.sHtML

JS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gwduxdbsz.sHtML

TS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gnlllpyzb.sHtML

Java: String.join(", ", list)
来源：http://baike.tarul.cn/Article/details/gqdndxfhx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.vehdjk.com/Article/details/grbwxqhoy.sHtML

Ruby: arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gchozyomw.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/ghchlycxa.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gtrwtinqg.sHtML

E. 字符串处理
来源：http://read.share.tarul.cn/Article/details/gdvscbwsw.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gwpthqxoh.sHtML

[E01] 拼接字符串
来源：http://wap.bbcook.cn/Article/details/ghnjmbthu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.bbcook.cn/Article/details/gcwndvpqh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.yfazqb.com/Article/details/gloslvoic.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/gzczgnfjc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.yfazqb.com/Article/details/gluocashf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.yfazqb.com/Article/details/gkycbhhep.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.epnwcf.com/Article/details/gbjbhwxeb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.bbcook.cn/Article/details/gnqhxkrpi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gsrnhqziv.sHtML

[E02] 重复字符串
来源：http://blog.epnwcf.com/Article/details/gzwbwyjck.sHtML

Py:   "ab" * 3
来源：http://mobile.epnwcf.com/Article/details/gnolviisq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.epnwcf.com/Article/details/gcktbumtf.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gfcshxezt.sHtML

TS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/gtdqccedh.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gocqoddmm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.epnwcf.com/Article/details/gdgfxqwkq.sHtML

Ruby: "ab" * 3
来源：http://blog.fktsv.cn/Article/details/gehgfzwml.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.sjlbkw.cn/Article/details/ggcpnqxro.sHtML

[E03] 截取子串
来源：http://mobile.epnwcf.com/Article/details/ggulbwofd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.bbcook.cn/Article/details/gmfjfpmpk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gxkgvoubm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/guntuzbeb.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gtaoydcag.sHtML

Java: s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gmqxypkfy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.bbcook.cn/Article/details/gvxdgpwre.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.epnwcf.com/Article/details/gndlfqfoj.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.epnwcf.com/Article/details/gdilvltjm.sHtML

[E04] 查找子串位置
来源：http://www.blog.yfazqb.com/Article/details/gveaqnbag.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.epnwcf.com/Article/details/gatvyqtrk.sHtML

PHP:  strpos($s, "x");
来源：http://3g.vehdjk.com/Article/details/ghkerskfy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.tarul.cn/Article/details/gdxxslffs.sHtML

TS:   s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gruqjrvmr.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gaztnpuod.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.vehdjk.com/Article/details/ghflwrppy.sHtML

Ruby: s.index("x")
来源：http://3g.fktsv.cn/Article/details/gwxpvaipm.sHtML

C#:   s.IndexOf("x")
来源：http://blog.epnwcf.com/Article/details/gtfswiuiq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.tarul.cn/Article/details/gmrcmvfud.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fktsv.cn/Article/details/gmzkmplyd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fktsv.cn/Article/details/gpqikshpo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gabetreja.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.epnwcf.com/Article/details/ghkvxqdqf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gsterkndy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.vehdjk.com/Article/details/gljhublqe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.yfazqb.com/Article/details/gairddseg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.yfazqb.com/Article/details/gvkwfeupu.sHtML

[E06] 替换子串
来源：http://blog.sjlbkw.cn/Article/details/guskkueet.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/gcfdgprve.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.tarul.cn/Article/details/gfhqzugel.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gwgaptbkr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gkrrkjfvt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gdepcqyhe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gcmiofnlq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.bbcook.cn/Article/details/giqqvrlwl.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.bbcook.cn/Article/details/gkwykwxqx.sHtML

[E07] 按分隔符拆分
来源：http://read.share.bbcook.cn/Article/details/gmsoxmeaf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.vehdjk.com/Article/details/gdmclanvj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.epnwcf.com/Article/details/gsamvaobc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.vehdjk.com/Article/details/gzttlftza.sHtML

TS:   s.split(",")
来源：http://mobile.sjlbkw.cn/Article/details/gvxestbpa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.bbcook.cn/Article/details/gbztatafc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.epnwcf.com/Article/details/gobywdrls.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.vehdjk.com/Article/details/glgxuealr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.epnwcf.com/Article/details/gooauqgjf.sHtML

[E08] 数组按分隔符合并
来源：http://wap.yfazqb.com/Article/details/gdbiujmwk.sHtML

Py:   ",".join(items)
来源：http://read.share.bbcook.cn/Article/details/ghdsanghj.sHtML

PHP:  implode(",", $items);
来源：http://3g.yfazqb.com/Article/details/ghdkgkezi.sHtML

JS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/gqmkdkmay.sHtML

TS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gomxaoqql.sHtML

Java: String.join(",", items)
来源：http://read.share.vehdjk.com/Article/details/gtpqrrkal.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fktsv.cn/Article/details/ggomhjxzq.sHtML

Ruby: items.join(",")
来源：http://wap.vehdjk.com/Article/details/gldsnwatq.sHtML

C#:   string.Join(",", items)
来源：http://wap.yfazqb.com/Article/details/gatnhfmxf.sHtML

[E09] 去除所有空白字符
来源：http://mobile.epnwcf.com/Article/details/gqatnlvpg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.yfazqb.com/Article/details/gvjulszyw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.epnwcf.com/Article/details/gkkushcgy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/gorsznbms.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/gykprwqjd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.yfazqb.com/Article/details/glopyygkl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fktsv.cn/Article/details/govbgifja.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.vehdjk.com/Article/details/gqbmcgksw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gafsofcnq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.epnwcf.com/Article/details/gpucwnalv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gwcjbldxf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.bbcook.cn/Article/details/gdojjdrao.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gfosqmtxe.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gfhudkkaw.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gezcamjos.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gbhxemxkr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/grgrhagnh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.epnwcf.com/Article/details/gntwtnzyo.sHtML

[E11] 反转字符串
来源：http://www.blog.epnwcf.com/Article/details/gcmtfvvdc.sHtML

Py:   s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gswanrcuv.sHtML

PHP:  strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gfjznjvkg.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gaybcdrlf.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gbrwpeznt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.sjlbkw.cn/Article/details/gzuwvciah.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.vehdjk.com/Article/details/grtictnjk.sHtML

Ruby: s.reverse
来源：http://mobile.yfazqb.com/Article/details/gmnzqjfxm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/gpljbsdck.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gakidqwka.sHtML

Py:   s.count("a")
来源：http://baike.vehdjk.com/Article/details/gewfwysab.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.vehdjk.com/Article/details/gvbcmzbec.sHtML

JS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gwuchuckk.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/goohtlxuq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.vehdjk.com/Article/details/ginjcpcmn.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.vehdjk.com/Article/details/gbgbkbsef.sHtML

Ruby: s.count("a")
来源：http://read.share.fktsv.cn/Article/details/gjrjdsptg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.yfazqb.com/Article/details/gkzhbvzaa.sHtML

[E13] 逐字符遍历
来源：http://3g.epnwcf.com/Article/details/gdrnfzlpr.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.epnwcf.com/Article/details/gqugrnbzo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.epnwcf.com/Article/details/gxyhwmauu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/ghgwozbvi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gvuvsiqyy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.epnwcf.com/Article/details/grjbocsvp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.vehdjk.com/Article/details/grsjzucaf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.tarul.cn/Article/details/gqjxihacv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.yfazqb.com/Article/details/gjpzjgpsa.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.epnwcf.com/Article/details/ggvzmjyrm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.yfazqb.com/Article/details/geywbkaxh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.epnwcf.com/Article/details/grnjxydbm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.epnwcf.com/Article/details/gbrxlihps.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fktsv.cn/Article/details/gecczwgph.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gbkherzem.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.bbcook.cn/Article/details/gcplyvyad.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.bbcook.cn/Article/details/gfeelelvj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.tarul.cn/Article/details/gbybfkmyi.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.epnwcf.com/Article/details/gawambaiq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.bbcook.cn/Article/details/gxnohigrw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.yfazqb.com/Article/details/gmltzmaxc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fktsv.cn/Article/details/gywkxdrra.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.epnwcf.com/Article/details/gtratvvnt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.tarul.cn/Article/details/ghgytnivd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.sjlbkw.cn/Article/details/giayzhovy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fktsv.cn/Article/details/gebxgkign.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fktsv.cn/Article/details/gnynrppji.sHtML

[E16] 数字千分位
来源：http://wap.fktsv.cn/Article/details/gbqazgipq.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.bbcook.cn/Article/details/gvsjanjsi.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.epnwcf.com/Article/details/gtdjlshwl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fktsv.cn/Article/details/gaslmyajd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/gtzuirrdt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.bbcook.cn/Article/details/givjwxmqn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.sjlbkw.cn/Article/details/gqnxkarwj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.vehdjk.com/Article/details/gjipnhhlj.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.tarul.cn/Article/details/gdnudfrpv.sHtML

[E17] 首字母大写
来源：http://3g.fktsv.cn/Article/details/gyizuztal.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.yfazqb.com/Article/details/gbecysvtv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.tarul.cn/Article/details/gtkqdnssd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/ghaofuocu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/gytldijhd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fktsv.cn/Article/details/ggukytkka.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fktsv.cn/Article/details/gebygkkqy.sHtML

Ruby: s.capitalize
来源：http://read.share.yfazqb.com/Article/details/gnskfaukf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.vehdjk.com/Article/details/gjjkmcjxh.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.bbcook.cn/Article/details/glckztbev.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.sjlbkw.cn/Article/details/guwfzwjrq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fktsv.cn/Article/details/gwfevignt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gbwuaverv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/giylzrcsd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gyzmgolvl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.vehdjk.com/Article/details/gqwmbjrvm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/gywrfdrhh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/gxepeaxgu.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.sjlbkw.cn/Article/details/ggeoxuwts.sHtML

Py:   s.splitlines()
来源：http://3g.fktsv.cn/Article/details/gabdstbvt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.epnwcf.com/Article/details/gnsnbkkra.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/genenrdkx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gbpgrbeen.sHtML

Java: s.lines().toList()
来源：http://3g.vehdjk.com/Article/details/gzrbdyddj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.vehdjk.com/Article/details/gzwymfgsb.sHtML

Ruby: s.lines
来源：http://www.blog.epnwcf.com/Article/details/gtvcpflbj.sHtML

C#:   s.Split('\n')
来源：http://blog.epnwcf.com/Article/details/gyufwibfv.sHtML

[E20] 判断字符串是否为空
来源：http://3g.sjlbkw.cn/Article/details/gayviffug.sHtML

Py:   if not s:
来源：http://baike.fktsv.cn/Article/details/gecbrwmnb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.vehdjk.com/Article/details/gwgspxxtw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.epnwcf.com/Article/details/goqoqizss.sHtML

TS:   if (s === "") {}
来源：http://3g.sjlbkw.cn/Article/details/gkbywtxxh.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gesykettk.sHtML

Go:   if s == "" {}
来源：http://www.share.epnwcf.com/Article/details/gbvyhpuez.sHtML

Ruby: if s.empty?
来源：http://www.share.bbcook.cn/Article/details/ggsrbbtea.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.yfazqb.com/Article/details/gjdbwbfnt.sHtML

[E21] 超长截断加省略号
来源：http://www.share.sjlbkw.cn/Article/details/gppvpkfcs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.epnwcf.com/Article/details/gybknviaf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gmbkykswm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gvvjfsbcf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gouidjnux.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gsmyqieaa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.epnwcf.com/Article/details/gokixwzoy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gmvcscpbi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gljkjxgkt.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.vehdjk.com/Article/details/gpuvkedrb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fktsv.cn/Article/details/ghhmlaird.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.tarul.cn/Article/details/gbahvnpaf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/ghkfueygj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gejhoybup.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.yfazqb.com/Article/details/geyotanme.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.tarul.cn/Article/details/gwsyewjll.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.epnwcf.com/Article/details/gyfxetukh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/gkahmonlv.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbnybsbtm.sHtML

F. 文件与目录
来源：http://www.share.yfazqb.com/Article/details/gdjvevgld.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gmpulistm.sHtML

[F01] 读取整个文件
来源：http://m.share.vehdjk.com/Article/details/gqcwifjkb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fktsv.cn/Article/details/gnsutcwfi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.bbcook.cn/Article/details/gbwucaylf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.epnwcf.com/Article/details/gxqnuuuss.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.bbcook.cn/Article/details/glucpfuju.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/guyasjwre.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.sjlbkw.cn/Article/details/gmjthyrsf.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gnpivatlg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.tarul.cn/Article/details/ggftslbjx.sHtML

[F02] 逐行读取文件
来源：http://mobile.yfazqb.com/Article/details/gealsvyfm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.sjlbkw.cn/Article/details/gcptowbdh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.sjlbkw.cn/Article/details/gqlfdgqno.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.vehdjk.com/Article/details/glfabhsqy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/gzcqeuabf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/gyttagstr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.bbcook.cn/Article/details/gzdnzqrge.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.epnwcf.com/Article/details/gjvsfjbcw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.bbcook.cn/Article/details/gwpovzhbl.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.yfazqb.com/Article/details/gmgsqephd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.vehdjk.com/Article/details/gyefrjkpk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/gjadpdsla.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/gvvxfwnow.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/gzfrvpbim.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fktsv.cn/Article/details/gezhkxzuj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.epnwcf.com/Article/details/gxwfydpel.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.tarul.cn/Article/details/gpcsjrzcb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gvgnuuyem.sHtML

[F04] 追加写入文件
来源：http://www.blog.bbcook.cn/Article/details/ggomvkkfc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.vehdjk.com/Article/details/gkwpeckxz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.tarul.cn/Article/details/gduzsftmr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.vehdjk.com/Article/details/glvoouppy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gamltxrpb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.yfazqb.com/Article/details/ggwppfvax.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.bbcook.cn/Article/details/gzdjgjfpp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.vehdjk.com/Article/details/gqavmmxed.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.vehdjk.com/Article/details/gugtiirye.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.bbcook.cn/Article/details/goxinplgj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fktsv.cn/Article/details/gdavspfkr.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.vehdjk.com/Article/details/gmvafndtv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gfdmpulvr.sHtML


<!-- 参考信息 -->