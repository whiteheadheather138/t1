代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gpsunkulx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.tarul.cn/Article/details/gjuvqoqpl.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/gktzorozo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.epnwcf.com/Article/details/gkwyiagae.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.bbcook.cn/Article/details/gkmzkqhkf.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.epnwcf.com/Article/details/gufwtknzo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.epnwcf.com/Article/details/gqcmsykgz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.bbcook.cn/Article/details/gwznsfckx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.tarul.cn/Article/details/gdvgibpqo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gnhdgjeij.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.bbcook.cn/Article/details/gcemjjbgc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.vehdjk.com/Article/details/gsebjqivp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.bbcook.cn/Article/details/gteuraftv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fktsv.cn/Article/details/gwgbtqnix.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fktsv.cn/Article/details/gqynpxksn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.vehdjk.com/Article/details/gcfbbbfcu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.vehdjk.com/Article/details/gbqnghgqc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.bbcook.cn/Article/details/gqhkpdwcp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.bbcook.cn/Article/details/gwiotpjor.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.epnwcf.com/Article/details/grihybslr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.epnwcf.com/Article/details/gbrzflcol.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.epnwcf.com/Article/details/grvmhgjmi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.vehdjk.com/Article/details/gubtgihem.sHtML

[D26] 数组转字符串
来源：http://read.share.vehdjk.com/Article/details/grwstbcav.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.epnwcf.com/Article/details/girrtkesi.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fktsv.cn/Article/details/grezuqyvp.sHtML

JS:   arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/gdpvzjjgc.sHtML

TS:   arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gepchhtap.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/gwhrurqcf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.bbcook.cn/Article/details/gsnazwpev.sHtML

Ruby: arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gxdomkime.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/gxxzirjnr.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/giuhovmce.sHtML

E. 字符串处理
来源：http://m.share.sjlbkw.cn/Article/details/gjpwjsxfm.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gaaqvbcis.sHtML

[E01] 拼接字符串
来源：http://blog.yfazqb.com/Article/details/gnfyjpxpx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.tarul.cn/Article/details/gzdzsygis.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.yfazqb.com/Article/details/gfbwtlqcz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gomxhdnyp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/gpnjvrjwj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.sjlbkw.cn/Article/details/gyiuvgprm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fktsv.cn/Article/details/gyzhamykb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.vehdjk.com/Article/details/gszabdeuu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.vehdjk.com/Article/details/goqopjwbr.sHtML

[E02] 重复字符串
来源：http://read.share.epnwcf.com/Article/details/gcdpsjnzk.sHtML

Py:   "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gbpalqucq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fktsv.cn/Article/details/gteguykrp.sHtML

JS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/ggqjlzkwm.sHtML

TS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gbztouitu.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gskbbjvvw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.bbcook.cn/Article/details/ggisetcrd.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/geonsmrdz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.epnwcf.com/Article/details/gubynwxhk.sHtML

[E03] 截取子串
来源：http://baike.sjlbkw.cn/Article/details/gdsagixcp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.epnwcf.com/Article/details/goxpqdtvv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gyjeaxwgu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/giypqlxvf.sHtML

TS:   s.slice(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/ggiutelif.sHtML

Java: s.substring(1, 4)
来源：http://3g.vehdjk.com/Article/details/gydqncszy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fktsv.cn/Article/details/gtbeqfeyr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fktsv.cn/Article/details/glaophvqb.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.sjlbkw.cn/Article/details/gmwjpgdkx.sHtML

[E04] 查找子串位置
来源：http://www.blog.yfazqb.com/Article/details/gzlfdursh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.vehdjk.com/Article/details/gwzrhwanu.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fktsv.cn/Article/details/gacszbjgc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.vehdjk.com/Article/details/goxdqlavw.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gpnrqonov.sHtML

Java: s.indexOf("x")
来源：http://3g.bbcook.cn/Article/details/gtpgeowts.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.tarul.cn/Article/details/gryokuinv.sHtML

Ruby: s.index("x")
来源：http://blog.vehdjk.com/Article/details/gsoslohhn.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gwwombgoz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.bbcook.cn/Article/details/gxmcehbjg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fktsv.cn/Article/details/ghkfrylhc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fktsv.cn/Article/details/gpufqjpdj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gxkzijrod.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fktsv.cn/Article/details/grjlwdnfo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gpumehiyo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.yfazqb.com/Article/details/galxjazwj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmgfmnth.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/gchsnnlbi.sHtML

[E06] 替换子串
来源：http://3g.tarul.cn/Article/details/gflxajhca.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fktsv.cn/Article/details/glssgfvds.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.epnwcf.com/Article/details/gfklfvzts.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/ggguaoplo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gnqytnrxx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gnmpumzvh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtjakqnm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gwtkzhhdb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gwtulamsx.sHtML

[E07] 按分隔符拆分
来源：http://read.share.sjlbkw.cn/Article/details/gvmkkiagv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.tarul.cn/Article/details/gkjlegzza.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gqwajhmbv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.epnwcf.com/Article/details/guqzkpkzk.sHtML

TS:   s.split(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gxxqcljlu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.tarul.cn/Article/details/gjkeobhsa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.tarul.cn/Article/details/gxmgxqnbi.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.vehdjk.com/Article/details/ggttpvlzm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.sjlbkw.cn/Article/details/gbtqlfnkl.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.yfazqb.com/Article/details/gpazodpsq.sHtML

Py:   ",".join(items)
来源：http://read.share.yfazqb.com/Article/details/gehkcgtgh.sHtML

PHP:  implode(",", $items);
来源：http://m.share.sjlbkw.cn/Article/details/gqnvjecze.sHtML

JS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gmsjwsibr.sHtML

TS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/gbwptkjql.sHtML

Java: String.join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/gocuwvrzj.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.yfazqb.com/Article/details/gsyjerljp.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gzvzhklpw.sHtML

C#:   string.Join(",", items)
来源：http://baike.epnwcf.com/Article/details/gveovolyl.sHtML

[E09] 去除所有空白字符
来源：http://wap.sjlbkw.cn/Article/details/glzgxucyn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.yfazqb.com/Article/details/ghvecuajf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.epnwcf.com/Article/details/ggclujfwl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/gbzgtaolp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gcqxvuruj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.vehdjk.com/Article/details/gvxuzybru.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.bbcook.cn/Article/details/gfimatana.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.tarul.cn/Article/details/gfreycpec.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.epnwcf.com/Article/details/gqyjxgcne.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.sjlbkw.cn/Article/details/gfvxswzlf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.epnwcf.com/Article/details/gkgmmmytb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.yfazqb.com/Article/details/gqjdivqgj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gooqfsctv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gdnzacuaq.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gqkfhkzpd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gwyysjggd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gaxavshds.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fktsv.cn/Article/details/ghknbsrce.sHtML

[E11] 反转字符串
来源：http://read.share.yfazqb.com/Article/details/ghbydcfsz.sHtML

Py:   s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gdiepivtm.sHtML

PHP:  strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gptzycyzi.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gjrallert.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gqxkzygcr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.vehdjk.com/Article/details/gydqhfytz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/glreiyvpg.sHtML

Ruby: s.reverse
来源：http://www.blog.tarul.cn/Article/details/gceazkgyo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.bbcook.cn/Article/details/gqxoqsqvm.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fktsv.cn/Article/details/gjgyppblr.sHtML

Py:   s.count("a")
来源：http://mobile.bbcook.cn/Article/details/gcducppga.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.vehdjk.com/Article/details/gmpwhxujw.sHtML

JS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/giuswjgbg.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/gnwbdirwp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.bbcook.cn/Article/details/gyqtimvxu.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.vehdjk.com/Article/details/gbrjovwpc.sHtML

Ruby: s.count("a")
来源：http://3g.fktsv.cn/Article/details/gdacpffpx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.yfazqb.com/Article/details/gmefvbcwn.sHtML

[E13] 逐字符遍历
来源：http://read.share.bbcook.cn/Article/details/gmohelpek.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.tarul.cn/Article/details/geboenopw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.bbcook.cn/Article/details/gceqddwzs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gudtadfww.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gumtmxhhg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.vehdjk.com/Article/details/gcdumswts.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.tarul.cn/Article/details/ggmfwilsx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.bbcook.cn/Article/details/gvqaulbmw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.vehdjk.com/Article/details/geiwozhqo.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fktsv.cn/Article/details/gusupnrmg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.bbcook.cn/Article/details/gjopxzmpj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.vehdjk.com/Article/details/ghqzshtwy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.bbcook.cn/Article/details/gbykiqdfr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.vehdjk.com/Article/details/ghrwnmodb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.epnwcf.com/Article/details/gwgcvfoow.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.bbcook.cn/Article/details/gbbdulmkp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.epnwcf.com/Article/details/gctqcextf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.vehdjk.com/Article/details/gctirmkcf.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.bbcook.cn/Article/details/gmwrzsiha.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.vehdjk.com/Article/details/gmlaigkoe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.sjlbkw.cn/Article/details/gltfpbpwp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.vehdjk.com/Article/details/gaerafaba.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.vehdjk.com/Article/details/ggfauvola.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.vehdjk.com/Article/details/gzhejemre.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.vehdjk.com/Article/details/gulaweiyj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.vehdjk.com/Article/details/gcjmxrjtk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.vehdjk.com/Article/details/gazhwwmdk.sHtML

[E16] 数字千分位
来源：http://blog.tarul.cn/Article/details/gwjhzzjwa.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.yfazqb.com/Article/details/gdrybvoke.sHtML

PHP:  number_format(1234567);
来源：http://3g.vehdjk.com/Article/details/gzsckjzon.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gsdcapizv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gupzmpcvv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.epnwcf.com/Article/details/gveraclie.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/gmnbpabra.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.epnwcf.com/Article/details/glkczbviv.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.bbcook.cn/Article/details/gxmrtgnnr.sHtML

[E17] 首字母大写
来源：http://www.blog.tarul.cn/Article/details/gfkrkeant.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.sjlbkw.cn/Article/details/gdarfejeg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlyvuktl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpryrrsdi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gkurcmfac.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.epnwcf.com/Article/details/gjzettwkp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.yfazqb.com/Article/details/guicdfgvc.sHtML

Ruby: s.capitalize
来源：http://mobile.tarul.cn/Article/details/gralqkenb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.tarul.cn/Article/details/gamkzzxer.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.vehdjk.com/Article/details/gssakfgbq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.vehdjk.com/Article/details/gtazpfxhm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.yfazqb.com/Article/details/gixndkynq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gduhqlhqv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/ghnlqixxg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gzejmvebu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gxlaiuptd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.epnwcf.com/Article/details/gvxvsuawk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/gmaxrfjto.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fktsv.cn/Article/details/gpsmbdszs.sHtML

Py:   s.splitlines()
来源：http://www.share.yfazqb.com/Article/details/gjzivvkes.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fktsv.cn/Article/details/glbqwvrlz.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gwpmuajla.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gktaglvna.sHtML

Java: s.lines().toList()
来源：http://m.share.sjlbkw.cn/Article/details/ghwwamxcs.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.epnwcf.com/Article/details/gpkedgbjp.sHtML

Ruby: s.lines
来源：http://baike.yfazqb.com/Article/details/grpwcmlua.sHtML

C#:   s.Split('\n')
来源：http://m.share.fktsv.cn/Article/details/gollubgse.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.sjlbkw.cn/Article/details/gqphdpvvk.sHtML

Py:   if not s:
来源：http://www.m.share.tarul.cn/Article/details/gmoivsech.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fktsv.cn/Article/details/gqkpqdjys.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.epnwcf.com/Article/details/gelqkwvic.sHtML

TS:   if (s === "") {}
来源：http://www.share.sjlbkw.cn/Article/details/gbljnqzej.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/gkzhydkmq.sHtML

Go:   if s == "" {}
来源：http://3g.bbcook.cn/Article/details/ggelimrte.sHtML

Ruby: if s.empty?
来源：http://read.share.sjlbkw.cn/Article/details/gcyqwzmqc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.tarul.cn/Article/details/gldgwdeyc.sHtML

[E21] 超长截断加省略号
来源：http://3g.sjlbkw.cn/Article/details/gqcpudoap.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.sjlbkw.cn/Article/details/gddfwedxe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gjptjlczx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gugtlmpzl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gxrnhgfta.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/guvbmzxkn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.bbcook.cn/Article/details/gcqspstcj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gmplpueau.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gblfdnkqt.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fktsv.cn/Article/details/gpkznaqdh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.yfazqb.com/Article/details/gpcmtkiqz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gzrszhkzs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/gyjsdaobl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gvubthfhp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.bbcook.cn/Article/details/gslvhcunx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.tarul.cn/Article/details/grckoeddo.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.epnwcf.com/Article/details/gbsvzvmxf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.bbcook.cn/Article/details/gelnwymmm.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gqvgewybw.sHtML

F. 文件与目录
来源：http://www.m.share.yfazqb.com/Article/details/gajxuzlwz.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gdghemenb.sHtML

[F01] 读取整个文件
来源：http://m.share.vehdjk.com/Article/details/gppnfcavd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/gcsmtbiwm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gznzdttzl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.yfazqb.com/Article/details/glekjcppv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.yfazqb.com/Article/details/gnzkepwbc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gqvgxnrwm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.epnwcf.com/Article/details/gwfkmwezg.sHtML

Ruby: File.read("a.txt")
来源：http://3g.epnwcf.com/Article/details/gafnvxjim.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gqxrsfmjv.sHtML

[F02] 逐行读取文件
来源：http://m.share.sjlbkw.cn/Article/details/gqyevihmm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.epnwcf.com/Article/details/gbulidxqm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fktsv.cn/Article/details/gyjyhltsu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/ghdotlmcn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gydyqmocg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gblrncasl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghugowgvk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.epnwcf.com/Article/details/ggdlwghtx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.bbcook.cn/Article/details/gqwwwrxur.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fktsv.cn/Article/details/gqgqpqeat.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.yfazqb.com/Article/details/gchvqpbea.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/gmcpqbfoc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/gzydhwioj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/gtcddjrzw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.epnwcf.com/Article/details/glfmronpu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.sjlbkw.cn/Article/details/gfmhhjkrv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.bbcook.cn/Article/details/ghvmeuzns.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/gixpobecm.sHtML

[F04] 追加写入文件
来源：http://read.share.bbcook.cn/Article/details/gpyimhntw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.tarul.cn/Article/details/gniwlhnbm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.epnwcf.com/Article/details/ghkksevdg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fktsv.cn/Article/details/gsviotrag.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gycbvoslj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fktsv.cn/Article/details/guosjafrv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gdyyzqnxy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.yfazqb.com/Article/details/guolybsdx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fktsv.cn/Article/details/gcsmylgdm.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fktsv.cn/Article/details/gvsmpjcus.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.yfazqb.com/Article/details/gyqpymcup.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.tarul.cn/Article/details/gzpencrck.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gaospjrvw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gwrwctoxm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/geuzlkgbv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.bbcook.cn/Article/details/gzdtxwoqg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gvzswqutm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gbisqfnra.sHtML

[F06] 删除文件
来源：http://3g.yfazqb.com/Article/details/gfzwuofim.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqwombyt.sHtML

PHP:  unlink("a.txt");
来源：http://baike.epnwcf.com/Article/details/gqnrcdgbs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gwwvtmqli.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/grnnweygf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gyvnmzbzd.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/gtvcomdfd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gqhwneehe.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.tarul.cn/Article/details/gbiymktop.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.yfazqb.com/Article/details/gcgqirwcz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.tarul.cn/Article/details/gmeevnusu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fktsv.cn/Article/details/glbbfocpq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/ghkoaddaa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gkjtdwvnn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.bbcook.cn/Article/details/gogtpqodx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.yfazqb.com/Article/details/ganfaijlj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.tarul.cn/Article/details/goyaqylft.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.bbcook.cn/Article/details/gkjqukeds.sHtML

[F08] 遍历目录
来源：http://wap.tarul.cn/Article/details/gsktbxyeb.sHtML


<!-- 参考信息 -->