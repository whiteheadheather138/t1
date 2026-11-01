代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.tarul.cn/Article/details/gbsjzvuci.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.vehdjk.com/Article/details/gnstllrug.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.vehdjk.com/Article/details/gqhmcarll.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.yfazqb.com/Article/details/gvzybfofb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.tarul.cn/Article/details/gnhzlwxxz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.yfazqb.com/Article/details/gvzsxbwlq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.tarul.cn/Article/details/gsjlenxyv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.yfazqb.com/Article/details/gvpjsvsdg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.vehdjk.com/Article/details/goomupuve.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.sjlbkw.cn/Article/details/gdjzjdbpq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.yfazqb.com/Article/details/gucsquwcq.sHtML

[D26] 数组转字符串
来源：http://m.share.fktsv.cn/Article/details/gfcwrpwfy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fktsv.cn/Article/details/gawgklwzf.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gfygaabrh.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/grmxakkyb.sHtML

TS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/ggleetfsy.sHtML

Java: String.join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/gwiemplhu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fktsv.cn/Article/details/gcthdfsgb.sHtML

Ruby: arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gkiembrkz.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gkoitvykz.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gammnjfya.sHtML

E. 字符串处理
来源：http://baike.yfazqb.com/Article/details/gqyawvjpx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ghyqbvpwm.sHtML

[E01] 拼接字符串
来源：http://m.share.tarul.cn/Article/details/gqgtgukbw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fktsv.cn/Article/details/gfkslbzwa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fktsv.cn/Article/details/gmvtflaxa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gjfijwpxg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/gsqfvpqgf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.epnwcf.com/Article/details/ghujmfrkz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fktsv.cn/Article/details/goiynvpxu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.epnwcf.com/Article/details/gcrviduam.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gwnozhiic.sHtML

[E02] 重复字符串
来源：http://m.share.sjlbkw.cn/Article/details/gggggxckn.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fktsv.cn/Article/details/gjczaqour.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.vehdjk.com/Article/details/glaayafax.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gspqibiln.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gkqaxjznr.sHtML

Java: "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gevbvnnvo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.epnwcf.com/Article/details/gyhbsldel.sHtML

Ruby: "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/geiejdrha.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.epnwcf.com/Article/details/gskdimmeb.sHtML

[E03] 截取子串
来源：http://m.share.vehdjk.com/Article/details/gfjjkxvah.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/galpdpjvd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gvcalyekn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.bbcook.cn/Article/details/gaaanhokt.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gikhvgdhw.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gvgbxzntc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.bbcook.cn/Article/details/ggpmxwwdt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.epnwcf.com/Article/details/gxchlxtoh.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fktsv.cn/Article/details/gftbwhpjq.sHtML

[E04] 查找子串位置
来源：http://m.share.epnwcf.com/Article/details/gplrjlwvj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fktsv.cn/Article/details/ghydsdjhi.sHtML

PHP:  strpos($s, "x");
来源：http://wap.yfazqb.com/Article/details/gsbuscrxn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.vehdjk.com/Article/details/gikufrswc.sHtML

TS:   s.indexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gugdtsuqc.sHtML

Java: s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gtktdcohr.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.tarul.cn/Article/details/gtazcxico.sHtML

Ruby: s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gfthriuyo.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gtlpwwvvn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.vehdjk.com/Article/details/gkrnxbdms.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.yfazqb.com/Article/details/gkgkbrsbc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.bbcook.cn/Article/details/gmfkeaouk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gmoyzqzch.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.epnwcf.com/Article/details/guqugyjtw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.vehdjk.com/Article/details/glzkhcvuf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.epnwcf.com/Article/details/giugytrzs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.epnwcf.com/Article/details/grfnnhkfh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gryragdba.sHtML

[E06] 替换子串
来源：http://3g.fktsv.cn/Article/details/gbcdgeudm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/geoqnrzer.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.epnwcf.com/Article/details/ggonrvjbw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/geamwjhih.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gmgojlmsf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gnzqxqsac.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gybrozfrh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gjjlkdpvx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gxrmpnojk.sHtML

[E07] 按分隔符拆分
来源：http://baike.tarul.cn/Article/details/gzezoiwgh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.bbcook.cn/Article/details/gczawzmqu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gussczizv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fktsv.cn/Article/details/gzpncyyjs.sHtML

TS:   s.split(",")
来源：http://wap.epnwcf.com/Article/details/ggawtngsz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fktsv.cn/Article/details/gyuyualsm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.vehdjk.com/Article/details/guhswylmc.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.yfazqb.com/Article/details/gtyiyqtwk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.yfazqb.com/Article/details/gycpswsoj.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.bbcook.cn/Article/details/gjxbtfwwp.sHtML

Py:   ",".join(items)
来源：http://mobile.epnwcf.com/Article/details/ghamvlegv.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.tarul.cn/Article/details/gljlwuwic.sHtML

JS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gmbfjymmk.sHtML

TS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/ghfdvodry.sHtML

Java: String.join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gxtszvehc.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/gxzeqsbac.sHtML

Ruby: items.join(",")
来源：http://read.share.tarul.cn/Article/details/gxqkndmjo.sHtML

C#:   string.Join(",", items)
来源：http://blog.yfazqb.com/Article/details/gmumfxxqi.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fktsv.cn/Article/details/gmganvvwz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.sjlbkw.cn/Article/details/gajrncrxd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.epnwcf.com/Article/details/gclwchjbg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/getaaduau.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fktsv.cn/Article/details/gqhbsmtic.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/gdwvzjsns.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.sjlbkw.cn/Article/details/gsbdydhwt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.bbcook.cn/Article/details/gszyzcebt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.tarul.cn/Article/details/glzsdmasi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.tarul.cn/Article/details/giqxxmnfa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.vehdjk.com/Article/details/gjfqodfgu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.bbcook.cn/Article/details/gypbtlfdp.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gopssmomv.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gjflxoagt.sHtML

Java: String.format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gskmovryr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gshbszzrw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gwivnkkyr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.bbcook.cn/Article/details/gxkvbfomf.sHtML

[E11] 反转字符串
来源：http://baike.fktsv.cn/Article/details/gfshholfk.sHtML

Py:   s[::-1]
来源：http://www.share.epnwcf.com/Article/details/gveqbvxbu.sHtML

PHP:  strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/gzlvkfpnq.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gtxglskxi.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gqbihlfsi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.epnwcf.com/Article/details/gjrtovwfr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.bbcook.cn/Article/details/gfucrqrbt.sHtML

Ruby: s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gaivjmkca.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/gulunevaj.sHtML

[E12] 统计某字符出现次数
来源：http://3g.yfazqb.com/Article/details/gatvrxxlu.sHtML

Py:   s.count("a")
来源：http://baike.tarul.cn/Article/details/gqhvlwpdu.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.bbcook.cn/Article/details/gmbryxqao.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.sjlbkw.cn/Article/details/gwxqrktlj.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/gcgdjvqyd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.vehdjk.com/Article/details/gmylpqblq.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.vehdjk.com/Article/details/ghutyjlcy.sHtML

Ruby: s.count("a")
来源：http://blog.epnwcf.com/Article/details/gafdqftrr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.tarul.cn/Article/details/gnfveyajd.sHtML

[E13] 逐字符遍历
来源：http://read.share.epnwcf.com/Article/details/gzqexuabd.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fktsv.cn/Article/details/gzgzcbguo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.yfazqb.com/Article/details/gghezwgdo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.epnwcf.com/Article/details/gyxrssdxc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gvsdxoxbv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.sjlbkw.cn/Article/details/ghlypbpus.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.epnwcf.com/Article/details/ghwgsgxuq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.tarul.cn/Article/details/gawzcqvip.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.epnwcf.com/Article/details/gxyrvhupw.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.tarul.cn/Article/details/gyljttnsb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.sjlbkw.cn/Article/details/givkjvhim.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.vehdjk.com/Article/details/gmxfbplwg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.tarul.cn/Article/details/gylygesgn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.bbcook.cn/Article/details/gpotrsxna.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.epnwcf.com/Article/details/gcjsuglqo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.epnwcf.com/Article/details/grhglmkwd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.yfazqb.com/Article/details/ggzdrtznt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fktsv.cn/Article/details/gevfazoko.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.vehdjk.com/Article/details/gxkstnmog.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fktsv.cn/Article/details/gvxwnmfvg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.yfazqb.com/Article/details/gjhclrnmw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.yfazqb.com/Article/details/glbqgyuno.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.epnwcf.com/Article/details/gsvlnyvdr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fktsv.cn/Article/details/gdjylbfit.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.sjlbkw.cn/Article/details/gculuevza.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fktsv.cn/Article/details/gquhitadf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.sjlbkw.cn/Article/details/gplqwwdpg.sHtML

[E16] 数字千分位
来源：http://m.share.fktsv.cn/Article/details/gyzamsbht.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.epnwcf.com/Article/details/gqtexhycf.sHtML

PHP:  number_format(1234567);
来源：http://mobile.vehdjk.com/Article/details/gnjdenfwr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/gbeoohaee.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/gcejupxef.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.vehdjk.com/Article/details/gqfcphogr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.yfazqb.com/Article/details/gptuhsomg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.epnwcf.com/Article/details/gqqkzbjdd.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.sjlbkw.cn/Article/details/gxwopmhiv.sHtML

[E17] 首字母大写
来源：http://baike.vehdjk.com/Article/details/gxbkgxety.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.vehdjk.com/Article/details/gnsvaacmr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.bbcook.cn/Article/details/gowojoqjr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/gilnzchws.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/gqqstaqwx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.yfazqb.com/Article/details/gwdzkzwgi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.bbcook.cn/Article/details/gavdsljjr.sHtML

Ruby: s.capitalize
来源：http://blog.bbcook.cn/Article/details/gymrbhvkm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.epnwcf.com/Article/details/gizktkpyj.sHtML

[E18] 模板占位符替换
来源：http://wap.yfazqb.com/Article/details/gqdreygev.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.sjlbkw.cn/Article/details/giureoinp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.epnwcf.com/Article/details/gaktluggw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gykenvhug.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gjlhhhlds.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gldrpmyns.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.epnwcf.com/Article/details/gppryalnh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.sjlbkw.cn/Article/details/gucjhulxe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.tarul.cn/Article/details/gbqqbruoa.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.bbcook.cn/Article/details/gybzoaixk.sHtML

Py:   s.splitlines()
来源：http://blog.epnwcf.com/Article/details/gmnbxshib.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gqhwtzkio.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/grlloijkp.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gokybrekq.sHtML

Java: s.lines().toList()
来源：http://baike.bbcook.cn/Article/details/gsdzochvl.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.vehdjk.com/Article/details/gtowbvbij.sHtML

Ruby: s.lines
来源：http://www.share.sjlbkw.cn/Article/details/gwlppwupt.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.vehdjk.com/Article/details/gvezkbmuj.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.yfazqb.com/Article/details/gigawpxxq.sHtML

Py:   if not s:
来源：http://wap.yfazqb.com/Article/details/guzooocsi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.vehdjk.com/Article/details/gqnmmqkeg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.epnwcf.com/Article/details/gtheearaj.sHtML

TS:   if (s === "") {}
来源：http://3g.fktsv.cn/Article/details/gxlttxrho.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/gjjgobuad.sHtML

Go:   if s == "" {}
来源：http://m.share.fktsv.cn/Article/details/ghhweddqm.sHtML

Ruby: if s.empty?
来源：http://www.share.epnwcf.com/Article/details/gijsiamkz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.yfazqb.com/Article/details/gsbdkhuvh.sHtML

[E21] 超长截断加省略号
来源：http://3g.yfazqb.com/Article/details/gddtfbimu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fktsv.cn/Article/details/gpqxmzpma.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gpiurkqcu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gczdnahpz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gjjpsyivy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gsjxcsplz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.tarul.cn/Article/details/getcachao.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gmqsvcvkt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/guysxdvob.sHtML

[E22] 字节长度与字符长度
来源：http://wap.sjlbkw.cn/Article/details/gkctnefqj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.tarul.cn/Article/details/gxmvbawys.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/giakvzjwa.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gbdlqqlfp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gsiddzwln.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.epnwcf.com/Article/details/gsarcplyw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.sjlbkw.cn/Article/details/gbifjaufr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.bbcook.cn/Article/details/gcdcpbgtl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.yfazqb.com/Article/details/gwysqynke.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gduwwjvgj.sHtML

F. 文件与目录
来源：http://wap.epnwcf.com/Article/details/gditosjzh.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gylqzexva.sHtML

[F01] 读取整个文件
来源：http://3g.vehdjk.com/Article/details/gmyfpuwxx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fktsv.cn/Article/details/gbfwdwumo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gqdonqwlq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fktsv.cn/Article/details/gcoukfjrb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.tarul.cn/Article/details/gsliqsybb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gtvazqyel.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.vehdjk.com/Article/details/gqkzcglhz.sHtML

Ruby: File.read("a.txt")
来源：http://wap.bbcook.cn/Article/details/gzhwrzysu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.bbcook.cn/Article/details/gxfxcxjpp.sHtML

[F02] 逐行读取文件
来源：http://wap.tarul.cn/Article/details/gnympjdxw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.vehdjk.com/Article/details/gohxspgfz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.tarul.cn/Article/details/ghndpysaq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/gnbwxnhoj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gmioptukv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fktsv.cn/Article/details/gkgsjbwnk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.sjlbkw.cn/Article/details/gcqjshgog.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.vehdjk.com/Article/details/gaopuetwy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.epnwcf.com/Article/details/gbmubjoku.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.sjlbkw.cn/Article/details/gnxunxmsy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fktsv.cn/Article/details/gpdkjcfua.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.vehdjk.com/Article/details/gycxgozkv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gmrfxlrci.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.vehdjk.com/Article/details/glpqdglzi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fktsv.cn/Article/details/gpvteqrhp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.sjlbkw.cn/Article/details/gdorkvqxf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fktsv.cn/Article/details/gmegkmpez.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.yfazqb.com/Article/details/gohkkujtl.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gwnppkmxs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.bbcook.cn/Article/details/gcpprskiy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.bbcook.cn/Article/details/gpofqpbda.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/gyrjmrxrc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/gmobdamnj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.tarul.cn/Article/details/goasxbkyp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.yfazqb.com/Article/details/gyuvhciby.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.sjlbkw.cn/Article/details/gwkediibm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.yfazqb.com/Article/details/glzgsyjsx.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.vehdjk.com/Article/details/gekiznxwu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.sjlbkw.cn/Article/details/gfpmtcifk.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.vehdjk.com/Article/details/glasluxcb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gunphveil.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/grrhmjwce.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gwkhqfhuf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.tarul.cn/Article/details/gktkbafqf.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/glaobohim.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gluatixrc.sHtML

[F06] 删除文件
来源：http://read.share.bbcook.cn/Article/details/gwuveaduv.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ganqfipiv.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fktsv.cn/Article/details/gtwlzznwl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gabcfxkbn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gdykzpfcx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/grtcosiyg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gqzqlxugm.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.bbcook.cn/Article/details/gneuzlald.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gmnsjvegi.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.tarul.cn/Article/details/girlgojgt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.tarul.cn/Article/details/gqoanbjlo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fktsv.cn/Article/details/gkkorjgvn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gmhznithe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.vehdjk.com/Article/details/gxurntksm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.vehdjk.com/Article/details/gvrpqpgou.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.yfazqb.com/Article/details/gndviwybb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.bbcook.cn/Article/details/gxmfnvzwn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.yfazqb.com/Article/details/gyfmtutwe.sHtML

[F08] 遍历目录
来源：http://www.share.bbcook.cn/Article/details/gjzuhkanz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.vehdjk.com/Article/details/gocrinvjm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.sjlbkw.cn/Article/details/gmtjlouys.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/gvkzkxxwn.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gzuntzblz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gilsejnym.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.tarul.cn/Article/details/gzqufxpoi.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.epnwcf.com/Article/details/gmwpjmozj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.epnwcf.com/Article/details/gypknkuzu.sHtML

[F09] 获取文件大小
来源：http://mobile.sjlbkw.cn/Article/details/gkceudwqu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gstsjbubo.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gmcrabqaz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.sjlbkw.cn/Article/details/geweviwbz.sHtML


<!-- 参考信息 -->