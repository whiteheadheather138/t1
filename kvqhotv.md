代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.yfazqb.com/Article/details/gfsxkfzym.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.sjlbkw.cn/Article/details/gasccdvmg.sHtML

Go:   // 手写循环
来源：http://www.share.vehdjk.com/Article/details/gcmsgdovg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.epnwcf.com/Article/details/gnmmlhqby.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fktsv.cn/Article/details/gmpuavgef.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.vehdjk.com/Article/details/gfxevqrpx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.bbcook.cn/Article/details/gqspfxvyv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.bbcook.cn/Article/details/gppyafivx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.yfazqb.com/Article/details/geffllden.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gjcwgwvai.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/gxjcoanhj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.yfazqb.com/Article/details/gzlakirtq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.bbcook.cn/Article/details/gupdsvqeo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.sjlbkw.cn/Article/details/ggkhpooco.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.epnwcf.com/Article/details/gcgwspwax.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fktsv.cn/Article/details/griioxqco.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.epnwcf.com/Article/details/gtowdudcs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhkzebvf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.vehdjk.com/Article/details/gyixdyajj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.tarul.cn/Article/details/gmffrvwvu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.tarul.cn/Article/details/guihalebs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.bbcook.cn/Article/details/gorsedydv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.vehdjk.com/Article/details/gpvuzujmq.sHtML

[D26] 数组转字符串
来源：http://mobile.bbcook.cn/Article/details/gyxjcvtju.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fktsv.cn/Article/details/gfptlrirr.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fktsv.cn/Article/details/gbonlcbps.sHtML

JS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gcokdeiia.sHtML

TS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gbyssujwj.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gouptvacl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.yfazqb.com/Article/details/gsxnvxlle.sHtML

Ruby: arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gxhjzfgim.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gexyylijp.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gazklftgw.sHtML

E. 字符串处理
来源：http://m.share.tarul.cn/Article/details/goeweorna.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gikvarefk.sHtML

[E01] 拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/goiabnujt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.bbcook.cn/Article/details/gyuzqrgkc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fktsv.cn/Article/details/glpqvzsmu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/gkbquzfhc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/gjkxavnvz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.epnwcf.com/Article/details/gqvhqzmrg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.epnwcf.com/Article/details/gvfhmosve.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.bbcook.cn/Article/details/gqxuranft.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.vehdjk.com/Article/details/gqqltffsu.sHtML

[E02] 重复字符串
来源：http://wap.yfazqb.com/Article/details/gtswrznod.sHtML

Py:   "ab" * 3
来源：http://wap.epnwcf.com/Article/details/ghrljdyei.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.vehdjk.com/Article/details/gdvylrcmg.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gggrqaerp.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gqkwcpdle.sHtML

Java: "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/groaoqctt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fktsv.cn/Article/details/gvnrrlfaa.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/glzlgcwzq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.tarul.cn/Article/details/gywqtkvnt.sHtML

[E03] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/ghneaqzdx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.epnwcf.com/Article/details/gjciorsic.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gfefjykdk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gokmvdpwi.sHtML

TS:   s.slice(1, 4)
来源：http://3g.bbcook.cn/Article/details/gtboyqlzr.sHtML

Java: s.substring(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/gxhfibimb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fktsv.cn/Article/details/glphkvuey.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fktsv.cn/Article/details/gskhzahbt.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.yfazqb.com/Article/details/gygupallb.sHtML

[E04] 查找子串位置
来源：http://www.m.share.tarul.cn/Article/details/gcjxssjdt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.vehdjk.com/Article/details/geqcoudmo.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.tarul.cn/Article/details/gxkujrmmc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.tarul.cn/Article/details/gwlzcygcp.sHtML

TS:   s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gktqampyn.sHtML

Java: s.indexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gorfcfydm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.tarul.cn/Article/details/gqltigkgz.sHtML

Ruby: s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/gowbsqtjj.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gltaxwkll.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fktsv.cn/Article/details/gsmhkppym.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.tarul.cn/Article/details/gzbwhettb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.yfazqb.com/Article/details/gsgyggywb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.vehdjk.com/Article/details/gfgknvlra.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.epnwcf.com/Article/details/gywpdnnky.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gjxiursoa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.epnwcf.com/Article/details/giqfhtfgf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.vehdjk.com/Article/details/gffupwrkv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.yfazqb.com/Article/details/guvnhdigc.sHtML

[E06] 替换子串
来源：http://read.share.bbcook.cn/Article/details/glhqxebkb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/ghdurykik.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fktsv.cn/Article/details/gtsyllrvl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gbkgovrbw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gakxcixgb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/garzlfioi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/ghevssbnq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.tarul.cn/Article/details/geaoyzsve.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.vehdjk.com/Article/details/gesbjrazq.sHtML

[E07] 按分隔符拆分
来源：http://mobile.yfazqb.com/Article/details/gfihokvru.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fktsv.cn/Article/details/gjpxbtkjp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.bbcook.cn/Article/details/grbugornk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.tarul.cn/Article/details/gwwkpjjfq.sHtML

TS:   s.split(",")
来源：http://wap.bbcook.cn/Article/details/glpyoumuv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.epnwcf.com/Article/details/glmfwxhuk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fktsv.cn/Article/details/glmskdmze.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.bbcook.cn/Article/details/gqxgkrbvy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.vehdjk.com/Article/details/giihxkiic.sHtML

[E08] 数组按分隔符合并
来源：http://baike.yfazqb.com/Article/details/gucziexnm.sHtML

Py:   ",".join(items)
来源：http://3g.vehdjk.com/Article/details/gfanzhwnr.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.sjlbkw.cn/Article/details/ggwenashh.sHtML

JS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/grzfzutwx.sHtML

TS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/gbzwsjtyo.sHtML

Java: String.join(",", items)
来源：http://www.m.share.yfazqb.com/Article/details/gmocxqabp.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fktsv.cn/Article/details/gjayysbsr.sHtML

Ruby: items.join(",")
来源：http://www.share.yfazqb.com/Article/details/ghxcvefhj.sHtML

C#:   string.Join(",", items)
来源：http://mobile.vehdjk.com/Article/details/gqsxhdgpb.sHtML

[E09] 去除所有空白字符
来源：http://mobile.bbcook.cn/Article/details/gvfmswuqr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.tarul.cn/Article/details/gidsemhsb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.yfazqb.com/Article/details/gflsrklqg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fktsv.cn/Article/details/gmyxyqwcg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fktsv.cn/Article/details/gbrmhqvug.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.tarul.cn/Article/details/gixnkvdnx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.vehdjk.com/Article/details/garwlkfyd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.yfazqb.com/Article/details/gfvbtpmbl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.vehdjk.com/Article/details/gvppundvs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.bbcook.cn/Article/details/gapsvhwss.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/ggwjtaepa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.tarul.cn/Article/details/grbsmgmda.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gtobctmal.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/glnatkxzs.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/ggnktiizb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gjdfkqzhq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gmztdjaud.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.epnwcf.com/Article/details/gykdkocsm.sHtML

[E11] 反转字符串
来源：http://read.share.tarul.cn/Article/details/gwxdwpihk.sHtML

Py:   s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gvafjsuwf.sHtML

PHP:  strrev($s);
来源：http://wap.bbcook.cn/Article/details/gafthjddu.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gmdkdjmbq.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/ggvfrgvwi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fktsv.cn/Article/details/gavlygnep.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.vehdjk.com/Article/details/gdsasfoga.sHtML

Ruby: s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gwwlkzpvg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/gqkjmrpfw.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.yfazqb.com/Article/details/gexvihsfi.sHtML

Py:   s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gpobnrlah.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.tarul.cn/Article/details/gqkcazayp.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/gqkcfzhvk.sHtML

TS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/ghxtgcsuj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.bbcook.cn/Article/details/gnzbnkssm.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.vehdjk.com/Article/details/gynxliaty.sHtML

Ruby: s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gsvlwwycp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.vehdjk.com/Article/details/gkzsqycqt.sHtML

[E13] 逐字符遍历
来源：http://wap.sjlbkw.cn/Article/details/gcefmijpi.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.tarul.cn/Article/details/gcxgyzjaz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.yfazqb.com/Article/details/gjiebpiqn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.yfazqb.com/Article/details/gtrcachex.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/gwvexaplt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fktsv.cn/Article/details/gxnvaskrg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.bbcook.cn/Article/details/gcrukttfs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.vehdjk.com/Article/details/gzlepbxqy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gigquyjsj.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.sjlbkw.cn/Article/details/guairfjfz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.bbcook.cn/Article/details/ghndjumux.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fktsv.cn/Article/details/gcutrjljb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.bbcook.cn/Article/details/gymmjwuja.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.vehdjk.com/Article/details/gfklostyn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.sjlbkw.cn/Article/details/glyazyuxz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.epnwcf.com/Article/details/glkadixur.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fktsv.cn/Article/details/gmmknfjjp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fktsv.cn/Article/details/gykwdgxhg.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.bbcook.cn/Article/details/gcnzapgcf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fktsv.cn/Article/details/gbwzefrwb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.vehdjk.com/Article/details/glimisxpl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.epnwcf.com/Article/details/grsnmukyo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.vehdjk.com/Article/details/gojqmpeum.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.vehdjk.com/Article/details/gcwyoiesj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fktsv.cn/Article/details/gkuajucww.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fktsv.cn/Article/details/gjzciqwcv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fktsv.cn/Article/details/ggkgkjqlj.sHtML

[E16] 数字千分位
来源：http://mobile.fktsv.cn/Article/details/gmieycqtb.sHtML

Py:   f"{1234567:,}"
来源：http://blog.tarul.cn/Article/details/gpakjceoy.sHtML

PHP:  number_format(1234567);
来源：http://wap.tarul.cn/Article/details/geejaiztr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fktsv.cn/Article/details/gxwweucls.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/ggswgqodc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.tarul.cn/Article/details/ggkfjuxxn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.epnwcf.com/Article/details/gkxtbsmiz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.sjlbkw.cn/Article/details/guhwvwsyc.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.yfazqb.com/Article/details/gsyrfxlob.sHtML

[E17] 首字母大写
来源：http://3g.epnwcf.com/Article/details/gnwyhppce.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.yfazqb.com/Article/details/gcfyjdoca.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.vehdjk.com/Article/details/ghhgzsyrp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.tarul.cn/Article/details/ghnnvusbm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gzujfnsas.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.epnwcf.com/Article/details/gnpjjajgp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.tarul.cn/Article/details/gqixdxayq.sHtML

Ruby: s.capitalize
来源：http://read.share.tarul.cn/Article/details/gsywaasgh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.vehdjk.com/Article/details/gjtzmtubc.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.bbcook.cn/Article/details/gxncooqou.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.sjlbkw.cn/Article/details/gfncwaptr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.vehdjk.com/Article/details/gpqqucxko.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gcpvyztgo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gulmkvuew.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/grzqxddnl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fktsv.cn/Article/details/gzxurhegy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.epnwcf.com/Article/details/gaggfwbxu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.bbcook.cn/Article/details/gcliyzdij.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.bbcook.cn/Article/details/gktfruomg.sHtML

Py:   s.splitlines()
来源：http://3g.bbcook.cn/Article/details/gozudohyu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.yfazqb.com/Article/details/gxfqslgod.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/gggedujjj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/guwnlorki.sHtML

Java: s.lines().toList()
来源：http://3g.fktsv.cn/Article/details/gsduyfbje.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.vehdjk.com/Article/details/gucrzbokl.sHtML

Ruby: s.lines
来源：http://www.share.epnwcf.com/Article/details/gftundtyj.sHtML

C#:   s.Split('\n')
来源：http://mobile.tarul.cn/Article/details/garneexnv.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.tarul.cn/Article/details/gakmpbjcr.sHtML

Py:   if not s:
来源：http://3g.epnwcf.com/Article/details/gbaxagwsq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.vehdjk.com/Article/details/glgnqttre.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.sjlbkw.cn/Article/details/gxmzvsxzg.sHtML

TS:   if (s === "") {}
来源：http://www.share.sjlbkw.cn/Article/details/gwkcvjfuw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gbimdmxil.sHtML

Go:   if s == "" {}
来源：http://baike.bbcook.cn/Article/details/goxaalahj.sHtML

Ruby: if s.empty?
来源：http://mobile.yfazqb.com/Article/details/glckkzzin.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.epnwcf.com/Article/details/ghnkibhlw.sHtML

[E21] 超长截断加省略号
来源：http://read.share.bbcook.cn/Article/details/glzelghnv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.bbcook.cn/Article/details/gekgyubmk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gmciuzcui.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gjnthikhd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gbauekuze.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/goyjvfkjl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.yfazqb.com/Article/details/gamdrlkwi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.bbcook.cn/Article/details/giavmvyva.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gbgkjxjtc.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.vehdjk.com/Article/details/gfesszbvl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.epnwcf.com/Article/details/gtjbcvahn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gnszksddy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gczxadeti.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gvinafvbx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gkseoxqcf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.bbcook.cn/Article/details/gwcmxrtzq.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.epnwcf.com/Article/details/gtmuwpuve.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.tarul.cn/Article/details/gqntdqxko.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gsqaeiywj.sHtML

F. 文件与目录
来源：http://www.share.tarul.cn/Article/details/glrngxfun.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gmisazdne.sHtML

[F01] 读取整个文件
来源：http://m.share.tarul.cn/Article/details/gkatmqkfs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.tarul.cn/Article/details/gepqgnoel.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gacczoksj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.tarul.cn/Article/details/ghynimqhc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gpkfnwzpq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/geiwymikd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.yfazqb.com/Article/details/gdsuorixx.sHtML

Ruby: File.read("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gskvnhqze.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.yfazqb.com/Article/details/gfxnlfzxv.sHtML

[F02] 逐行读取文件
来源：http://3g.fktsv.cn/Article/details/gnsokapom.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.sjlbkw.cn/Article/details/geykpthki.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.tarul.cn/Article/details/gvhyhbmej.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/gnjzhhmwa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/gkrfgqpiy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/gvvsbiltv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.yfazqb.com/Article/details/gdlsdfchf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.sjlbkw.cn/Article/details/gildkxnbx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.tarul.cn/Article/details/gzjqdctju.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.yfazqb.com/Article/details/gdaiwpqum.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.vehdjk.com/Article/details/gilswlhrl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.epnwcf.com/Article/details/gamecvdlz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/geuxakdha.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gkzxzljjr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.epnwcf.com/Article/details/gntlcloty.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.bbcook.cn/Article/details/gpqslwjxh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.yfazqb.com/Article/details/ggyyvajey.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gttjttrdm.sHtML

[F04] 追加写入文件
来源：http://baike.yfazqb.com/Article/details/gpvqihkub.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.vehdjk.com/Article/details/gdjkkijjm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fktsv.cn/Article/details/ghejzbzfu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gtupsufky.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/ghxqmoube.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.epnwcf.com/Article/details/gagiyihkw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.yfazqb.com/Article/details/gcmdppcfi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.sjlbkw.cn/Article/details/gfkuumitc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.vehdjk.com/Article/details/gyipjiquz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.yfazqb.com/Article/details/gmhcgvahc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fktsv.cn/Article/details/gzfhyawgz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gedrnkmpy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/grqzhsemf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gtldqciqc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gljmzfzxa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.tarul.cn/Article/details/gwgvdetbg.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.tarul.cn/Article/details/gdikjejtk.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gaxykbgxm.sHtML

[F06] 删除文件
来源：http://www.share.epnwcf.com/Article/details/glfzhwhob.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gwpvcsdpj.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdkuxpgg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gbemrwany.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gttqrukpn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/geuficoyt.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fktsv.cn/Article/details/ghvuszubz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gikfmkacf.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.bbcook.cn/Article/details/gmzretfqh.sHtML

[F07] 创建目录（含多级）
来源：http://wap.yfazqb.com/Article/details/gnvmccpiq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/ggiyalihd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.sjlbkw.cn/Article/details/giriymngn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/gfqilazee.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gmhvuczro.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.bbcook.cn/Article/details/gsilvodnt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.tarul.cn/Article/details/gyndziaip.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.vehdjk.com/Article/details/gvkbypqff.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.epnwcf.com/Article/details/gevlzrmjq.sHtML

[F08] 遍历目录
来源：http://www.blog.yfazqb.com/Article/details/gynnjqpgb.sHtML


<!-- 参考信息 -->