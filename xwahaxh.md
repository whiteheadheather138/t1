代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.tarul.cn/Article/details/gttetffqv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gvziabctc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fktsv.cn/Article/details/grahycuqn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.bbcook.cn/Article/details/gczlnrieb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.tarul.cn/Article/details/gwmkxjyym.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.yfazqb.com/Article/details/grlcjxede.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.sjlbkw.cn/Article/details/gzaualcgu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.epnwcf.com/Article/details/gixxxtkzt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.epnwcf.com/Article/details/gojwsbors.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.tarul.cn/Article/details/gpzyeijkq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.sjlbkw.cn/Article/details/giqiioxlj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.sjlbkw.cn/Article/details/gjlpavgcr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.yfazqb.com/Article/details/gqvcqluxg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.yfazqb.com/Article/details/gfcdxmswr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.vehdjk.com/Article/details/gbiawcutp.sHtML

[D26] 数组转字符串
来源：http://baike.tarul.cn/Article/details/goizxgowq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.yfazqb.com/Article/details/ggybarryu.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fktsv.cn/Article/details/ggcrzzhip.sHtML

JS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gffvklrdn.sHtML

TS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gghdkqwyf.sHtML

Java: String.join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gzglhmubx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.sjlbkw.cn/Article/details/gekxifeie.sHtML

Ruby: arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gkxfijpjq.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.bbcook.cn/Article/details/ggxidivra.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gepcgrbvv.sHtML

E. 字符串处理
来源：http://blog.tarul.cn/Article/details/gksalpwrf.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxtbmbshs.sHtML

[E01] 拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gjqnwuwdv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.bbcook.cn/Article/details/gxnhkijvd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.yfazqb.com/Article/details/gvrjtazxm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.yfazqb.com/Article/details/ggdbzytmi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gupjzcwwz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.sjlbkw.cn/Article/details/gmymopnwg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.bbcook.cn/Article/details/grhnzklrm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.tarul.cn/Article/details/gtnlecmpj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gpawcapur.sHtML

[E02] 重复字符串
来源：http://3g.tarul.cn/Article/details/ggglxtuwf.sHtML

Py:   "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gdauazbxh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fktsv.cn/Article/details/gzizcbfec.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/glcvhtqxb.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gzuzgtqvw.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gahhinwfs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.bbcook.cn/Article/details/geyqzjlfl.sHtML

Ruby: "ab" * 3
来源：http://m.share.tarul.cn/Article/details/gapuldcvf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.sjlbkw.cn/Article/details/grotgqses.sHtML

[E03] 截取子串
来源：http://wap.tarul.cn/Article/details/gysfzixad.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.epnwcf.com/Article/details/gxidohhqx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gbzblrevt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.yfazqb.com/Article/details/ggqvayxlc.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.bbcook.cn/Article/details/guepkaihe.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gbdupfwgr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fktsv.cn/Article/details/gfexotqnc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.yfazqb.com/Article/details/gkhpwggid.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.epnwcf.com/Article/details/gzvpzeijy.sHtML

[E04] 查找子串位置
来源：http://baike.vehdjk.com/Article/details/gjoshnodx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.vehdjk.com/Article/details/gcrhipaml.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.epnwcf.com/Article/details/gfrlhwikl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fktsv.cn/Article/details/gofjpdkmc.sHtML

TS:   s.indexOf("x")
来源：http://m.share.tarul.cn/Article/details/gkhizfvyd.sHtML

Java: s.indexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gibqcugmt.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.bbcook.cn/Article/details/gpndxsylk.sHtML

Ruby: s.index("x")
来源：http://www.share.tarul.cn/Article/details/ghiyfztcy.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/gkyooriqr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.epnwcf.com/Article/details/gphkcingh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.yfazqb.com/Article/details/ggafwazmn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.vehdjk.com/Article/details/glogiwvfj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.vehdjk.com/Article/details/gyrbqkwiw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.bbcook.cn/Article/details/gexmzltuf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gtyjqvxmz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.epnwcf.com/Article/details/gporycjiz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fktsv.cn/Article/details/gqzaatsdd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gskkafaqi.sHtML

[E06] 替换子串
来源：http://mobile.yfazqb.com/Article/details/gmsfampdy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/gqmttdkle.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.yfazqb.com/Article/details/ggscrypom.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/grsbkynzm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghutijrmu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gykievlel.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.vehdjk.com/Article/details/gbgvakdrp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.tarul.cn/Article/details/gslbclkps.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fktsv.cn/Article/details/gvhfwvxdf.sHtML

[E07] 按分隔符拆分
来源：http://m.share.yfazqb.com/Article/details/glftjqunh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.bbcook.cn/Article/details/glojllrjk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.tarul.cn/Article/details/gvadujkdo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fktsv.cn/Article/details/gtsvwzxiq.sHtML

TS:   s.split(",")
来源：http://www.share.epnwcf.com/Article/details/gcatbfdyi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fktsv.cn/Article/details/ghuurefdq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.yfazqb.com/Article/details/gpfewhdyi.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fktsv.cn/Article/details/gomlgotpe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.tarul.cn/Article/details/gdpernren.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.epnwcf.com/Article/details/ggpcktdwb.sHtML

Py:   ",".join(items)
来源：http://3g.fktsv.cn/Article/details/gycxizcqh.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.bbcook.cn/Article/details/gbvyuubxb.sHtML

JS:   items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gvxojwugz.sHtML

TS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gfzlliens.sHtML

Java: String.join(",", items)
来源：http://www.m.share.epnwcf.com/Article/details/gdgvnpzuw.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/gckeiygwe.sHtML

Ruby: items.join(",")
来源：http://mobile.tarul.cn/Article/details/gcrjwjlaz.sHtML

C#:   string.Join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/ggchmitxn.sHtML

[E09] 去除所有空白字符
来源：http://read.share.yfazqb.com/Article/details/gayxhquwl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.epnwcf.com/Article/details/gkzigifar.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.bbcook.cn/Article/details/gzmacouzf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/gjjgtbvch.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gotfaqsqw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.bbcook.cn/Article/details/gbtgktixw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.tarul.cn/Article/details/gqkxnvqgb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.tarul.cn/Article/details/gltnvcdgt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gzdokktns.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.yfazqb.com/Article/details/gywasbvwc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.epnwcf.com/Article/details/grpqzgvub.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzlqthjh.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gopwrvsup.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gfnsubimn.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gdqqbzifi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/ghqkvzeor.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/gvsiwkxmy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fktsv.cn/Article/details/gvzlykqkt.sHtML

[E11] 反转字符串
来源：http://3g.bbcook.cn/Article/details/gqjtleqxy.sHtML

Py:   s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gbbadnzch.sHtML

PHP:  strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gvpfeqjjj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/ggvmremju.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gyxtoodry.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fktsv.cn/Article/details/gwcbvpkpe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.epnwcf.com/Article/details/gsxwkzrwo.sHtML

Ruby: s.reverse
来源：http://read.share.fktsv.cn/Article/details/gbsectmjq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/gyahrkmoh.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbesjtkv.sHtML

Py:   s.count("a")
来源：http://wap.tarul.cn/Article/details/goyqwfxtp.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fktsv.cn/Article/details/gxesczqjp.sHtML

JS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/geualsopq.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/gawgxxhet.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.epnwcf.com/Article/details/gkimhnnna.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.sjlbkw.cn/Article/details/goxkpmnsh.sHtML

Ruby: s.count("a")
来源：http://www.m.share.epnwcf.com/Article/details/gspyautcj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.bbcook.cn/Article/details/gkkzxhgtl.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gxykrchwf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.sjlbkw.cn/Article/details/ggigmjzts.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.epnwcf.com/Article/details/govrfvizd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gzimiewxa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqqrnlpb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gggbqssly.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.tarul.cn/Article/details/gezcnetpe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fktsv.cn/Article/details/gagcdxqcd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.epnwcf.com/Article/details/gjupaqyir.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.yfazqb.com/Article/details/gkmtolhho.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.sjlbkw.cn/Article/details/gliqgigry.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.yfazqb.com/Article/details/gtetfohcv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fktsv.cn/Article/details/gekltsckd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.yfazqb.com/Article/details/gsltlpdmj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.bbcook.cn/Article/details/gnvdvobgk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.bbcook.cn/Article/details/gpfztdpir.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.yfazqb.com/Article/details/gslzranpo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.vehdjk.com/Article/details/ghxduvvhk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.epnwcf.com/Article/details/gknuewqxo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fktsv.cn/Article/details/gfwiwpoji.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.yfazqb.com/Article/details/gxyiflnig.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fktsv.cn/Article/details/guxfnvjbh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.tarul.cn/Article/details/gqlzwkrnm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.bbcook.cn/Article/details/gfnibaipp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.yfazqb.com/Article/details/gtteqqqcn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.epnwcf.com/Article/details/gxvfietyn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.sjlbkw.cn/Article/details/gbjrgaqpi.sHtML

[E16] 数字千分位
来源：http://www.blog.tarul.cn/Article/details/gkhzvojbp.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.vehdjk.com/Article/details/gjcnlfads.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fktsv.cn/Article/details/ginpzdkwf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.sjlbkw.cn/Article/details/gokitkdqn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/gwhvlmjim.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.sjlbkw.cn/Article/details/gitjufxoe.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.vehdjk.com/Article/details/gydqdchym.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.tarul.cn/Article/details/grscffjrg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.vehdjk.com/Article/details/gviouiztj.sHtML

[E17] 首字母大写
来源：http://m.share.fktsv.cn/Article/details/gbtmilsym.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.sjlbkw.cn/Article/details/gfrapemkz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gpbuxuvem.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/gvxhdlurw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/gqurfkvaa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.sjlbkw.cn/Article/details/gdmjsbxqk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.bbcook.cn/Article/details/gbxwjpahc.sHtML

Ruby: s.capitalize
来源：http://www.share.fktsv.cn/Article/details/gtqzushrv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.bbcook.cn/Article/details/gszaewyhl.sHtML

[E18] 模板占位符替换
来源：http://www.share.vehdjk.com/Article/details/gmjdittbe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.sjlbkw.cn/Article/details/grvndugin.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.epnwcf.com/Article/details/gdtyhszgw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gblmjkhqy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gptpkieka.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gwsqjpzye.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.yfazqb.com/Article/details/gtdrkypwt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fktsv.cn/Article/details/gnmvlhxxn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.vehdjk.com/Article/details/gwzpcptez.sHtML

[E19] 多行文本按行拆分
来源：http://3g.tarul.cn/Article/details/ghslniera.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/ggtqhorgz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.yfazqb.com/Article/details/gsqgrcnkv.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/gnntccjso.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gzcniohjb.sHtML

Java: s.lines().toList()
来源：http://3g.sjlbkw.cn/Article/details/gfoxxdduy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/grrzewbkt.sHtML

Ruby: s.lines
来源：http://www.m.share.epnwcf.com/Article/details/golpisioz.sHtML

C#:   s.Split('\n')
来源：http://baike.epnwcf.com/Article/details/gytoftxaa.sHtML

[E20] 判断字符串是否为空
来源：http://3g.yfazqb.com/Article/details/gzklghbbo.sHtML

Py:   if not s:
来源：http://mobile.tarul.cn/Article/details/ggdcvciyr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.yfazqb.com/Article/details/gppfnnaeq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.bbcook.cn/Article/details/gnynieleb.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.yfazqb.com/Article/details/gtpfiedsq.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gkkzjkznb.sHtML

Go:   if s == "" {}
来源：http://www.blog.vehdjk.com/Article/details/gayzhndhc.sHtML

Ruby: if s.empty?
来源：http://www.blog.tarul.cn/Article/details/girdlcvdb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.vehdjk.com/Article/details/grylaxqny.sHtML

[E21] 超长截断加省略号
来源：http://wap.vehdjk.com/Article/details/gmiussiom.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.vehdjk.com/Article/details/gypkalinp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gchnnujal.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gkgatzcgm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gkatwgqwd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gzzgmzetf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.yfazqb.com/Article/details/gubvaoewj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gdtovwjyb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.bbcook.cn/Article/details/glvhpxhqc.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.epnwcf.com/Article/details/gcnafakcn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.vehdjk.com/Article/details/gjjeltjxs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gkcqrsjct.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gclzqmrav.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/gbxbberhr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gfuwmgmkg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.vehdjk.com/Article/details/gbhmnzfjo.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.bbcook.cn/Article/details/gnngmpdyl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.epnwcf.com/Article/details/ghqgfbfdn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gypmemumd.sHtML

F. 文件与目录
来源：http://www.m.share.yfazqb.com/Article/details/gtffwaize.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggvrrwrcs.sHtML

[F01] 读取整个文件
来源：http://baike.bbcook.cn/Article/details/gcuzxidiq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzufqsfx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gpdgnbyng.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.tarul.cn/Article/details/gaxoyggbl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.tarul.cn/Article/details/gbfvbajua.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gegyzonwi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.epnwcf.com/Article/details/ggflchzxo.sHtML

Ruby: File.read("a.txt")
来源：http://wap.epnwcf.com/Article/details/gergkbhfj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.tarul.cn/Article/details/gsaegmmwl.sHtML

[F02] 逐行读取文件
来源：http://baike.bbcook.cn/Article/details/gugrqaeqw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.vehdjk.com/Article/details/gnggesizf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.bbcook.cn/Article/details/ggetoccff.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.epnwcf.com/Article/details/giwyiberp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.epnwcf.com/Article/details/gpqhqxiwm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gdiavfvna.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.bbcook.cn/Article/details/gwgihjmmq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.yfazqb.com/Article/details/gnhnhgaqx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.vehdjk.com/Article/details/ghxuolmbl.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.epnwcf.com/Article/details/gwxewmdmx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.tarul.cn/Article/details/gdfyivxhi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/ggycitkdr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/gylchpegr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gklvjgnzf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.epnwcf.com/Article/details/grqopzlea.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fktsv.cn/Article/details/gvbazzflg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.vehdjk.com/Article/details/gqwbokmlg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.yfazqb.com/Article/details/gudoaibbp.sHtML

[F04] 追加写入文件
来源：http://www.share.yfazqb.com/Article/details/ghifhwgik.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gxvtvwyyy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.bbcook.cn/Article/details/gawtignrb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gvlfhobqp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gzanwgmks.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.yfazqb.com/Article/details/ghmgoqdma.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fktsv.cn/Article/details/gjenmfchr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.tarul.cn/Article/details/gdnxgodbi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.epnwcf.com/Article/details/grlyykqua.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gmlmwxlni.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.epnwcf.com/Article/details/gjzslocqd.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.tarul.cn/Article/details/guasuehzp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/ghimfyewb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gomfghzty.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/goocezhtm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.epnwcf.com/Article/details/gmizzxiba.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.vehdjk.com/Article/details/grhjslpgb.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.bbcook.cn/Article/details/globigcov.sHtML

[F06] 删除文件
来源：http://mobile.sjlbkw.cn/Article/details/gechohihp.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/grwlcaygh.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.yfazqb.com/Article/details/grzyleoln.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gaxaoltju.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gqhegpktf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/glnglhhmy.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gzvsamcxy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gctoyinoa.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gppgjsdau.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.bbcook.cn/Article/details/gqccrpgdx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/gzgueodbc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.epnwcf.com/Article/details/gjhfkupzg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gonukiscy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gedmwharg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.bbcook.cn/Article/details/ggpabwrdt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.tarul.cn/Article/details/gsurogmnk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.tarul.cn/Article/details/gybkrcqbz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.bbcook.cn/Article/details/gwguaxayt.sHtML

[F08] 遍历目录
来源：http://blog.epnwcf.com/Article/details/gigohllnb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.vehdjk.com/Article/details/guionkrgf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fktsv.cn/Article/details/gflynyjit.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/gjukkeyfg.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gdvpgjgos.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/gjiudsbzq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/gadurjzyo.sHtML

Ruby: Dir.children("dir")
来源：http://3g.vehdjk.com/Article/details/gktgylkyp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.vehdjk.com/Article/details/ggwddzara.sHtML


<!-- 参考信息 -->