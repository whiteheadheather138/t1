代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.vehdjk.com/Article/details/gelxuruhf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.bbcook.cn/Article/details/gnqobdgzf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.tarul.cn/Article/details/gvhyocsax.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.vehdjk.com/Article/details/gcnzqcfxe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.bbcook.cn/Article/details/geskbbwsv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fktsv.cn/Article/details/gasvbgczn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.vehdjk.com/Article/details/gffrdhkow.sHtML

[D26] 数组转字符串
来源：http://read.share.bbcook.cn/Article/details/ggyijnssf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.vehdjk.com/Article/details/gmpyezcyy.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fktsv.cn/Article/details/gqnfcfcnw.sHtML

JS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/ggkgsgsld.sHtML

TS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gcctmekdm.sHtML

Java: String.join(", ", list)
来源：http://wap.fktsv.cn/Article/details/graniozvh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.tarul.cn/Article/details/gvhaperli.sHtML

Ruby: arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gebjbmjsy.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.epnwcf.com/Article/details/gtzdqggok.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/griyqogyr.sHtML

E. 字符串处理
来源：http://www.blog.bbcook.cn/Article/details/gucyqpkuh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gseyqksfr.sHtML

[E01] 拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gamamgjya.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.yfazqb.com/Article/details/gqwiucwyu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.tarul.cn/Article/details/gmvtdtxjf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gtiulyqwz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gqauiojdu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.sjlbkw.cn/Article/details/gtxvfiysg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fktsv.cn/Article/details/gxmvxhucl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fktsv.cn/Article/details/geqlgybgu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.vehdjk.com/Article/details/grbjqtzux.sHtML

[E02] 重复字符串
来源：http://3g.tarul.cn/Article/details/gdrnpnafr.sHtML

Py:   "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gzrlnzhro.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.bbcook.cn/Article/details/gfnxpletp.sHtML

JS:   "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gbefhtbde.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gwxweajkb.sHtML

Java: "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gcshpibtq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.tarul.cn/Article/details/gfaxweawk.sHtML

Ruby: "ab" * 3
来源：http://wap.fktsv.cn/Article/details/ggplhjrhz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.epnwcf.com/Article/details/giwyqkaqu.sHtML

[E03] 截取子串
来源：http://m.share.vehdjk.com/Article/details/gvnxzqmul.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.vehdjk.com/Article/details/geaydgbgf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/grdgnkstv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gmdfnrlfr.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.tarul.cn/Article/details/gtzrwgevn.sHtML

Java: s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gobftudtg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fktsv.cn/Article/details/gxhglvyiu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.vehdjk.com/Article/details/gqbtdxglm.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.yfazqb.com/Article/details/gbipqjbqk.sHtML

[E04] 查找子串位置
来源：http://blog.epnwcf.com/Article/details/ghptbfsle.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/gcmuxtkrh.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.vehdjk.com/Article/details/gqrmldpho.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.vehdjk.com/Article/details/gcrjpozjc.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gfmmlvthz.sHtML

Java: s.indexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gxswjypqp.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/gwoymiisq.sHtML

Ruby: s.index("x")
来源：http://mobile.fktsv.cn/Article/details/gneaizzss.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fktsv.cn/Article/details/glwfgomml.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.epnwcf.com/Article/details/grxjqjeot.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fktsv.cn/Article/details/gemqnwvjn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.tarul.cn/Article/details/gblufupku.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.tarul.cn/Article/details/gdhrwghqq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.tarul.cn/Article/details/gifjeryoi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gacikeroe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.tarul.cn/Article/details/gtjwxbhan.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.vehdjk.com/Article/details/gipaivjmf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gztfadxfa.sHtML

[E06] 替换子串
来源：http://www.m.share.yfazqb.com/Article/details/ghhztkthm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.epnwcf.com/Article/details/glynytrnp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.tarul.cn/Article/details/gbfdawdkn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gzciolgvk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gfrsfvimb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gvxodjxfo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/gnpbpaorz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fktsv.cn/Article/details/gbdvkmief.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gqkksuugw.sHtML

[E07] 按分隔符拆分
来源：http://www.share.yfazqb.com/Article/details/gzuislhnq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.epnwcf.com/Article/details/goqqlaytd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gqgqkikgf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.sjlbkw.cn/Article/details/gfpuhorzh.sHtML

TS:   s.split(",")
来源：http://www.share.vehdjk.com/Article/details/gitoxpnai.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.yfazqb.com/Article/details/gggnstubq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.tarul.cn/Article/details/ggoppggpz.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.yfazqb.com/Article/details/gdztmhyrk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.vehdjk.com/Article/details/gkrnfvdio.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.epnwcf.com/Article/details/gxuqexayc.sHtML

Py:   ",".join(items)
来源：http://www.blog.tarul.cn/Article/details/gboduyzkr.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.sjlbkw.cn/Article/details/gantfqbte.sHtML

JS:   items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/gqnxrjjia.sHtML

TS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gsiyihcya.sHtML

Java: String.join(",", items)
来源：http://baike.yfazqb.com/Article/details/gziutqgea.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.tarul.cn/Article/details/grsprggyu.sHtML

Ruby: items.join(",")
来源：http://mobile.yfazqb.com/Article/details/gishwmwem.sHtML

C#:   string.Join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gobivdtec.sHtML

[E09] 去除所有空白字符
来源：http://baike.vehdjk.com/Article/details/gucrmqzlh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.sjlbkw.cn/Article/details/gjunxiqvb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fktsv.cn/Article/details/grpbzemfs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gbyohvrut.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gjqukmdcg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.sjlbkw.cn/Article/details/gvcizobkt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.tarul.cn/Article/details/ggmuyuuzg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.epnwcf.com/Article/details/gnipztzia.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.bbcook.cn/Article/details/gccrliexu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/gbckreyue.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/grbpxsdzp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/gvxgnpbsm.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gliftgjeq.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gcxnolbxi.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gljeqqhji.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gxwzuisih.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/guhjjgobb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.bbcook.cn/Article/details/gwqbdotth.sHtML

[E11] 反转字符串
来源：http://baike.bbcook.cn/Article/details/geazngrlf.sHtML

Py:   s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gwcndwdwi.sHtML

PHP:  strrev($s);
来源：http://read.share.yfazqb.com/Article/details/gmdtadebz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gcbnjwlnn.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gztmvcuch.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.sjlbkw.cn/Article/details/grlgtfhfz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.yfazqb.com/Article/details/ghotxiaiu.sHtML

Ruby: s.reverse
来源：http://read.share.vehdjk.com/Article/details/gwrvnimro.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/gpmzkmxos.sHtML

[E12] 统计某字符出现次数
来源：http://wap.vehdjk.com/Article/details/gtbvbbynf.sHtML

Py:   s.count("a")
来源：http://read.share.fktsv.cn/Article/details/gkjsmrbmn.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.yfazqb.com/Article/details/gwdrlqniy.sHtML

JS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/gvkxiikgg.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/grgmkyrbi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.bbcook.cn/Article/details/gvqugqtnp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.tarul.cn/Article/details/grajvbapk.sHtML

Ruby: s.count("a")
来源：http://m.share.fktsv.cn/Article/details/gsvpvzyhn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.sjlbkw.cn/Article/details/gsqueemkf.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.epnwcf.com/Article/details/gvdxhtdvc.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.sjlbkw.cn/Article/details/gedcdjwrr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.bbcook.cn/Article/details/guwceirdl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gxsxtmowj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.vehdjk.com/Article/details/guvbtiszd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gnlntqrmf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.tarul.cn/Article/details/gcbhiaauh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.tarul.cn/Article/details/gtjifnruq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.vehdjk.com/Article/details/guqtamhkb.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fktsv.cn/Article/details/gudgviraq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.tarul.cn/Article/details/gtuvsrpis.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.epnwcf.com/Article/details/gcxgatvcg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.epnwcf.com/Article/details/gvvsbdfzh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.epnwcf.com/Article/details/gjascvtzj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fktsv.cn/Article/details/gndxusenl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.epnwcf.com/Article/details/gooufunvn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fktsv.cn/Article/details/gvkqgzdxn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.epnwcf.com/Article/details/gzfajgwey.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.bbcook.cn/Article/details/gnpxbzqzd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.bbcook.cn/Article/details/gklytdiei.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fktsv.cn/Article/details/gbuxyrdlt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.vehdjk.com/Article/details/gehmjmfoc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.bbcook.cn/Article/details/gavthagdc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.epnwcf.com/Article/details/ghwoaslrl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.tarul.cn/Article/details/gitpxupoj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.vehdjk.com/Article/details/gzdcjduvi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fktsv.cn/Article/details/ghbnvlwxu.sHtML

[E16] 数字千分位
来源：http://www.blog.tarul.cn/Article/details/gsbervfem.sHtML

Py:   f"{1234567:,}"
来源：http://3g.vehdjk.com/Article/details/gyclxhowd.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.tarul.cn/Article/details/gmiewmyri.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gmphjcrcz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/gzeaxucxw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gqnlzgpsu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.vehdjk.com/Article/details/gmpyuvwpz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.vehdjk.com/Article/details/gqyqymxbl.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.sjlbkw.cn/Article/details/gyvsldqma.sHtML

[E17] 首字母大写
来源：http://wap.tarul.cn/Article/details/gvvcgoqfk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.bbcook.cn/Article/details/gtbzlfukr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.tarul.cn/Article/details/gpkceqbda.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/gtknbpjkc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/gwyyvarqm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.bbcook.cn/Article/details/gjrkfagdb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.epnwcf.com/Article/details/grcpvorls.sHtML

Ruby: s.capitalize
来源：http://3g.sjlbkw.cn/Article/details/gzmgnscts.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.yfazqb.com/Article/details/gqlqpbakx.sHtML

[E18] 模板占位符替换
来源：http://blog.vehdjk.com/Article/details/gbtwkgorg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.yfazqb.com/Article/details/gtajcdqio.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.bbcook.cn/Article/details/gypduegoi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/geuyvjaub.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gjrczgmkq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gjzhxitzd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.epnwcf.com/Article/details/gxqnughfv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fktsv.cn/Article/details/gjtjguofg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.epnwcf.com/Article/details/gsnupyoys.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.bbcook.cn/Article/details/gekgtvvjs.sHtML

Py:   s.splitlines()
来源：http://mobile.yfazqb.com/Article/details/gxgrehhdg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.vehdjk.com/Article/details/gtleytezp.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gwfzccojn.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/gtwdexpwl.sHtML

Java: s.lines().toList()
来源：http://blog.yfazqb.com/Article/details/gickzelod.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.epnwcf.com/Article/details/geokmfzli.sHtML

Ruby: s.lines
来源：http://www.share.fktsv.cn/Article/details/gypjalmyh.sHtML

C#:   s.Split('\n')
来源：http://baike.tarul.cn/Article/details/gjozjrswl.sHtML

[E20] 判断字符串是否为空
来源：http://wap.epnwcf.com/Article/details/gfeuczjnv.sHtML

Py:   if not s:
来源：http://www.share.yfazqb.com/Article/details/giqzkbvdc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fktsv.cn/Article/details/gibrtklch.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.tarul.cn/Article/details/gmvqdvpph.sHtML

TS:   if (s === "") {}
来源：http://baike.tarul.cn/Article/details/gayantnmi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/gvxcdfywu.sHtML

Go:   if s == "" {}
来源：http://www.share.bbcook.cn/Article/details/gohsghugb.sHtML

Ruby: if s.empty?
来源：http://baike.vehdjk.com/Article/details/geouioybk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fktsv.cn/Article/details/gcaiqdeuw.sHtML

[E21] 超长截断加省略号
来源：http://www.share.vehdjk.com/Article/details/gombwpdhb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.yfazqb.com/Article/details/gwqobqdti.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gzvjztigs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gkhcocwxx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gvaueeshl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gvxpdmsht.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.tarul.cn/Article/details/ghsayzbdc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gafwvgzvk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gifypgqqj.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.epnwcf.com/Article/details/gfszeqgnp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.bbcook.cn/Article/details/gmldobjls.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gqigfipom.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gvgqfkufi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gvikhhsmg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.bbcook.cn/Article/details/ggjcgnvfm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.vehdjk.com/Article/details/gujpleugh.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gnlrctcaj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.tarul.cn/Article/details/gzovoibhw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gomcgxehu.sHtML

F. 文件与目录
来源：http://m.share.bbcook.cn/Article/details/gmzwjbhro.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/glztxgagx.sHtML

[F01] 读取整个文件
来源：http://3g.yfazqb.com/Article/details/gfynvpmdx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/gaunozeel.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.bbcook.cn/Article/details/gjhtrgdlb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.tarul.cn/Article/details/gfvfsvsyf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gszgigqhi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gfnkswolu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.tarul.cn/Article/details/ghuoklvuv.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gzoewqrna.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.bbcook.cn/Article/details/ggrophvkr.sHtML

[F02] 逐行读取文件
来源：http://www.share.bbcook.cn/Article/details/gfsxspngj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.yfazqb.com/Article/details/giwdrdgby.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.vehdjk.com/Article/details/giwydahwc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fktsv.cn/Article/details/gqvpigfcr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/gibcjdzia.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gaxpwwbtc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.epnwcf.com/Article/details/gvyrpgbfs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.yfazqb.com/Article/details/gvoluurwm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fktsv.cn/Article/details/gfmybgxuu.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.epnwcf.com/Article/details/gubfagwkd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.tarul.cn/Article/details/gnyylcanc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gfvfbvpaq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/gviwqinnh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/gwzbswbna.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.bbcook.cn/Article/details/gmmejtbdy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.yfazqb.com/Article/details/ggzyzkwak.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.tarul.cn/Article/details/glcxojbff.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gduobhrwe.sHtML

[F04] 追加写入文件
来源：http://blog.bbcook.cn/Article/details/gtyrkivpr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.tarul.cn/Article/details/gqvqtvubh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fktsv.cn/Article/details/gyvzzporu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.epnwcf.com/Article/details/gnbntroog.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/gzgeuobks.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fktsv.cn/Article/details/gmajwiywg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.bbcook.cn/Article/details/gwfunshhn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.bbcook.cn/Article/details/gqougrkdi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fktsv.cn/Article/details/gvwupxtvu.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.tarul.cn/Article/details/gbjjzamli.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.tarul.cn/Article/details/gqdgbfgsa.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/guomwsxgp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gscanfalg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/ggoebdkpc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/ghykeipyn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.vehdjk.com/Article/details/gesbumtsi.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gcailahba.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gvokvtwem.sHtML

[F06] 删除文件
来源：http://mobile.fktsv.cn/Article/details/gcbwlwuhv.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gjuhkjnnc.sHtML

PHP:  unlink("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/genzelnak.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gfwcrkden.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gicicxukp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gfqymbmut.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/giyowzcfl.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.yfazqb.com/Article/details/gipnrgdjo.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.epnwcf.com/Article/details/ggxsjrmwp.sHtML

[F07] 创建目录（含多级）
来源：http://blog.sjlbkw.cn/Article/details/gfvziofou.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.bbcook.cn/Article/details/gscawugpj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fktsv.cn/Article/details/grdktxxos.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gwhkircno.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gerpajuaq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.epnwcf.com/Article/details/gewqdvbqi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.vehdjk.com/Article/details/gvhaljaxe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.sjlbkw.cn/Article/details/goqguymse.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.sjlbkw.cn/Article/details/gpbnkcfkf.sHtML

[F08] 遍历目录
来源：http://www.share.fktsv.cn/Article/details/gyysworot.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.tarul.cn/Article/details/gunxjvdzu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.epnwcf.com/Article/details/gyrzslwws.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/geyldsamz.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/govfymaip.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/gjslntrtc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.bbcook.cn/Article/details/gspdamuho.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.yfazqb.com/Article/details/gysemmgjz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gduvveoiv.sHtML

[F09] 获取文件大小
来源：http://baike.vehdjk.com/Article/details/ghfqpogka.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gjbtkmlmc.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gwvumfhga.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/gvxknmabz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/gyljsdptw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gumvknoty.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.yfazqb.com/Article/details/gtrujtvoy.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.epnwcf.com/Article/details/griofdkai.sHtML


<!-- 参考信息 -->