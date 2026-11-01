代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.bbcook.cn/Article/details/gadjzzctg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.tarul.cn/Article/details/gmdveabvk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.bbcook.cn/Article/details/gdzyfeqzx.sHtML

[D26] 数组转字符串
来源：http://m.share.tarul.cn/Article/details/gxjqupbvy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fktsv.cn/Article/details/gipkhzlxc.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.sjlbkw.cn/Article/details/gbtwxmizz.sHtML

JS:   arr.join(", ")
来源：http://baike.fktsv.cn/Article/details/gwihketul.sHtML

TS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gcczefaln.sHtML

Java: String.join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gbizoiuuj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.vehdjk.com/Article/details/gubcmzqkr.sHtML

Ruby: arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gcptkbvdp.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.vehdjk.com/Article/details/gtembxric.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gmcaihrkm.sHtML

E. 字符串处理
来源：http://blog.bbcook.cn/Article/details/gqepshmom.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gordmcpjg.sHtML

[E01] 拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/ghpsaxizh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.yfazqb.com/Article/details/gyxpdeskc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fktsv.cn/Article/details/gabanffdi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.epnwcf.com/Article/details/gopuefekd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gfwvbxfqg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.vehdjk.com/Article/details/gwryivbqy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.tarul.cn/Article/details/gxnzytgoy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fktsv.cn/Article/details/ghqgymqqx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.tarul.cn/Article/details/gilrbyoxb.sHtML

[E02] 重复字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gnrrqwneg.sHtML

Py:   "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gsjiprbff.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gwoobbcul.sHtML

JS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gokhycquz.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gzfjqhsxq.sHtML

Java: "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/geypckjfa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.epnwcf.com/Article/details/gtpgbdftg.sHtML

Ruby: "ab" * 3
来源：http://m.share.tarul.cn/Article/details/gwkzmfyoj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.epnwcf.com/Article/details/gjjgjsrqy.sHtML

[E03] 截取子串
来源：http://baike.yfazqb.com/Article/details/gazndbxrv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.yfazqb.com/Article/details/gwkqjddsy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/guwkoesix.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gsipnjwta.sHtML

TS:   s.slice(1, 4)
来源：http://3g.bbcook.cn/Article/details/gidvtbkfh.sHtML

Java: s.substring(1, 4)
来源：http://wap.epnwcf.com/Article/details/gvhqaygmz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.tarul.cn/Article/details/ginaomozo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.vehdjk.com/Article/details/gymimccsg.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.bbcook.cn/Article/details/gskpttgba.sHtML

[E04] 查找子串位置
来源：http://baike.sjlbkw.cn/Article/details/geshhrunv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fktsv.cn/Article/details/gqcalhcdj.sHtML

PHP:  strpos($s, "x");
来源：http://blog.sjlbkw.cn/Article/details/ggsvrxqfw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fktsv.cn/Article/details/glwyuanen.sHtML

TS:   s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/gzwbhcvpm.sHtML

Java: s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gkuqduzae.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.bbcook.cn/Article/details/gwwqlwsez.sHtML

Ruby: s.index("x")
来源：http://3g.vehdjk.com/Article/details/gjmgtsstm.sHtML

C#:   s.IndexOf("x")
来源：http://blog.epnwcf.com/Article/details/gsajiyhqq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.bbcook.cn/Article/details/gxephzsus.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.epnwcf.com/Article/details/ggybwsjip.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.bbcook.cn/Article/details/gtygoaxgk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gevbbdnab.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fktsv.cn/Article/details/gpfynekmt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gvektcrdf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fktsv.cn/Article/details/ghibmeuwc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.vehdjk.com/Article/details/gnntsinki.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.tarul.cn/Article/details/gmpymlrmv.sHtML

[E06] 替换子串
来源：http://mobile.epnwcf.com/Article/details/gvmkhcjop.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.tarul.cn/Article/details/gkkrgzlmo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/guxlxvzas.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/ghqjlbfdy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gntnnmhdm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gwebwmdbn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.tarul.cn/Article/details/gqwpgfwoj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gysobmybi.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.tarul.cn/Article/details/goayutjlc.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.yfazqb.com/Article/details/gbcfqhwtq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.epnwcf.com/Article/details/gsckwknpk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.epnwcf.com/Article/details/gdbmjkjwx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.bbcook.cn/Article/details/gfkzyatmj.sHtML

TS:   s.split(",")
来源：http://baike.yfazqb.com/Article/details/gamxzucvh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.vehdjk.com/Article/details/gbngylvvm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.yfazqb.com/Article/details/gihdmagjw.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.sjlbkw.cn/Article/details/gtyqlogfw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.vehdjk.com/Article/details/gouilfwbr.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.sjlbkw.cn/Article/details/gkxnkttnu.sHtML

Py:   ",".join(items)
来源：http://baike.tarul.cn/Article/details/gzbswgpvk.sHtML

PHP:  implode(",", $items);
来源：http://www.share.yfazqb.com/Article/details/ggineiity.sHtML

JS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/gxucgwqmw.sHtML

TS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gardafejy.sHtML

Java: String.join(",", items)
来源：http://mobile.bbcook.cn/Article/details/gfqfniyvf.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.vehdjk.com/Article/details/gxjktzqio.sHtML

Ruby: items.join(",")
来源：http://wap.yfazqb.com/Article/details/glsyssphx.sHtML

C#:   string.Join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gqjivimer.sHtML

[E09] 去除所有空白字符
来源：http://baike.epnwcf.com/Article/details/gviqcgzde.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.bbcook.cn/Article/details/ghjqfaifk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.tarul.cn/Article/details/gbjaxzhns.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/gdlvzmqcy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.bbcook.cn/Article/details/gnrkwflep.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.epnwcf.com/Article/details/ggzqymfyb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fktsv.cn/Article/details/gqfifbktc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.vehdjk.com/Article/details/glywgckbe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.bbcook.cn/Article/details/ggffpmrlm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.tarul.cn/Article/details/ggcoojarz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gittfznwa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.tarul.cn/Article/details/grhixrqqw.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gdpigwxnc.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/genyifjyg.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gjlxkmbgq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/garguyuic.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gzbhdfxwu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.yfazqb.com/Article/details/gxevxpkld.sHtML

[E11] 反转字符串
来源：http://www.blog.epnwcf.com/Article/details/gjkgkrhdb.sHtML

Py:   s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/gimodytxu.sHtML

PHP:  strrev($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsgbslkk.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gtibiiifo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gebamqyar.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.tarul.cn/Article/details/gxqrscuoe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.tarul.cn/Article/details/gttedodkj.sHtML

Ruby: s.reverse
来源：http://mobile.bbcook.cn/Article/details/gvppvavke.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/glcycuogd.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.sjlbkw.cn/Article/details/gwsvjjicw.sHtML

Py:   s.count("a")
来源：http://read.share.tarul.cn/Article/details/gswlimytz.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.epnwcf.com/Article/details/gctxpiglf.sHtML

JS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/gmowfgprq.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gqlhccmtm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.yfazqb.com/Article/details/gynyxydla.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.tarul.cn/Article/details/gjutlqquo.sHtML

Ruby: s.count("a")
来源：http://www.m.share.tarul.cn/Article/details/gshgdrkvz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.yfazqb.com/Article/details/gpxrcwvyu.sHtML

[E13] 逐字符遍历
来源：http://3g.sjlbkw.cn/Article/details/gtehlcazf.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.tarul.cn/Article/details/gmvtbpjou.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.yfazqb.com/Article/details/gywcceith.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.yfazqb.com/Article/details/ggtvswtvp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.epnwcf.com/Article/details/gxhbkksue.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gafbmzwxi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.yfazqb.com/Article/details/gtbbuowzu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.yfazqb.com/Article/details/gzodfxwlv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.yfazqb.com/Article/details/gbpwmtgga.sHtML

[E14] URL 编码与 Base64
来源：http://blog.yfazqb.com/Article/details/gkahimknt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.epnwcf.com/Article/details/gszcmenkr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.sjlbkw.cn/Article/details/gxlickdfd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.epnwcf.com/Article/details/glqyfvgvs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.epnwcf.com/Article/details/giaslkhaf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.tarul.cn/Article/details/gjmbbjdyy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.sjlbkw.cn/Article/details/gjrxkeyhv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.yfazqb.com/Article/details/gqjxfmrxd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gwyyofplp.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.yfazqb.com/Article/details/grgpfpili.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.bbcook.cn/Article/details/gwexwgqvj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fktsv.cn/Article/details/gfwskzgsj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.sjlbkw.cn/Article/details/glnryejxr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fktsv.cn/Article/details/gnvdtdiyy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.sjlbkw.cn/Article/details/gcigvnkis.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.epnwcf.com/Article/details/gxjaqijxn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.vehdjk.com/Article/details/gpvbrphxf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fktsv.cn/Article/details/gjwtoslwa.sHtML

[E16] 数字千分位
来源：http://blog.bbcook.cn/Article/details/gaczxsnnm.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.vehdjk.com/Article/details/gqthhhkkb.sHtML

PHP:  number_format(1234567);
来源：http://baike.fktsv.cn/Article/details/gxyqhshuk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/guywbshuj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/gsuuusrre.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/gieqtzdbr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.bbcook.cn/Article/details/gdcpujrcj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.bbcook.cn/Article/details/gwklnloyr.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.epnwcf.com/Article/details/giavjclzb.sHtML

[E17] 首字母大写
来源：http://read.share.vehdjk.com/Article/details/gqlrhszhp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.bbcook.cn/Article/details/gwuuvwgcy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.yfazqb.com/Article/details/ggrgfuqhl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/guaghvuca.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.epnwcf.com/Article/details/guqeewkei.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.epnwcf.com/Article/details/gqhqottkl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fktsv.cn/Article/details/gfvbpjkhz.sHtML

Ruby: s.capitalize
来源：http://blog.fktsv.cn/Article/details/gocmyteif.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.yfazqb.com/Article/details/gkshptjrt.sHtML

[E18] 模板占位符替换
来源：http://www.share.sjlbkw.cn/Article/details/gonttlysq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.vehdjk.com/Article/details/grhxzxmbd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.yfazqb.com/Article/details/gupbrpfui.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gzjxwraoz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gqzltertb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gdpvgqpuj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gjoxwezyp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fktsv.cn/Article/details/gwbklvjzw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gsiiemquv.sHtML

[E19] 多行文本按行拆分
来源：http://3g.bbcook.cn/Article/details/gjmekvejc.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/gmfcluyim.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.bbcook.cn/Article/details/gxpjtdmrj.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gcssotfzv.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/glivcvaxr.sHtML

Java: s.lines().toList()
来源：http://www.share.epnwcf.com/Article/details/gyznlsnxu.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.tarul.cn/Article/details/glczijuzr.sHtML

Ruby: s.lines
来源：http://read.share.yfazqb.com/Article/details/gvzeadbji.sHtML

C#:   s.Split('\n')
来源：http://www.blog.yfazqb.com/Article/details/gtgzeskay.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.tarul.cn/Article/details/gkpoogffe.sHtML

Py:   if not s:
来源：http://read.share.epnwcf.com/Article/details/gvnhlmytd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.bbcook.cn/Article/details/guoqkelqh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.vehdjk.com/Article/details/gxoewhcjy.sHtML

TS:   if (s === "") {}
来源：http://read.share.yfazqb.com/Article/details/gudrendsz.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gmarbthsi.sHtML

Go:   if s == "" {}
来源：http://3g.yfazqb.com/Article/details/gjpzmrgrw.sHtML

Ruby: if s.empty?
来源：http://read.share.epnwcf.com/Article/details/gqomkurab.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.yfazqb.com/Article/details/gnefggtmf.sHtML

[E21] 超长截断加省略号
来源：http://read.share.vehdjk.com/Article/details/gngwrpxez.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.bbcook.cn/Article/details/gqblyfibc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gwpddiqwq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/ghxvtawvu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gosfdotmj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gknwzjfig.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.vehdjk.com/Article/details/gdddhisaj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gmmiwvoer.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gbllxczuh.sHtML

[E22] 字节长度与字符长度
来源：http://3g.bbcook.cn/Article/details/gvqtrpzft.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.bbcook.cn/Article/details/gdzcalust.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gyxjmmifb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/geozivnng.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gzkqamvuw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.epnwcf.com/Article/details/gqrrhglvd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.bbcook.cn/Article/details/gieqtvach.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gsezgworx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.tarul.cn/Article/details/gcwbgvmos.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gjmcnfucg.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/gohczqmma.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gfxtaxtwf.sHtML

[F01] 读取整个文件
来源：http://blog.yfazqb.com/Article/details/gwplaqrny.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.tarul.cn/Article/details/germzfaiv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gmekmxkht.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.tarul.cn/Article/details/gxflobkki.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gwcjybudp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/geanrmquq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.vehdjk.com/Article/details/glncpukqw.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gwcyzupch.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gvzrgadtw.sHtML

[F02] 逐行读取文件
来源：http://m.share.tarul.cn/Article/details/gmcmbgrzb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.yfazqb.com/Article/details/gtpfbqcju.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.epnwcf.com/Article/details/gwcxqfrnx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/gcihdyevp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gfmhbkoms.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/gkptgfguz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.bbcook.cn/Article/details/gpovrwqed.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.tarul.cn/Article/details/guhdmzrab.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fktsv.cn/Article/details/gncnxbsjm.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.bbcook.cn/Article/details/gbxnwdrpq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.vehdjk.com/Article/details/gizzusjxb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.yfazqb.com/Article/details/gkwxqwjdj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gjlxnsuez.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gpvmgepkx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.epnwcf.com/Article/details/guedxgrrd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.vehdjk.com/Article/details/glnubqfaw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.epnwcf.com/Article/details/gviulzxdk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gtjdmqelw.sHtML

[F04] 追加写入文件
来源：http://mobile.vehdjk.com/Article/details/gcuhcgezy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.tarul.cn/Article/details/gnqlxstxh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fktsv.cn/Article/details/gbuhlbrcn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/guuwpvosa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/gwrhlkjwa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fktsv.cn/Article/details/gmuicfvrf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gfnkgpbkw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fktsv.cn/Article/details/grqxuuyyw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.epnwcf.com/Article/details/gfeheiesy.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fktsv.cn/Article/details/ghpjldfmd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.bbcook.cn/Article/details/goozcbbgt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gaoxahton.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gtfzjmagn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/govakjxfc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gwuofbvzy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.epnwcf.com/Article/details/gvthdvosq.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gtzuaasgz.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gzbpyctzz.sHtML

[F06] 删除文件
来源：http://www.m.share.epnwcf.com/Article/details/geezobmkz.sHtML

Py:   os.remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gluexcmkg.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gtcpdoajw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gtqgyymjq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gqaryxwgv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gysvrfwgb.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gdhmwtysp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.tarul.cn/Article/details/ghxajzhyb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/ggideuqzd.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fktsv.cn/Article/details/gaskvxhzm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gusmipjtx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.vehdjk.com/Article/details/ghpckuiyt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gxkvsyasx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gdxmmjyzu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fktsv.cn/Article/details/gzfljxzja.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.sjlbkw.cn/Article/details/gvjpihpci.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.tarul.cn/Article/details/gfjncejtd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.yfazqb.com/Article/details/gyfazxqzx.sHtML

[F08] 遍历目录
来源：http://www.m.share.tarul.cn/Article/details/gaefduirp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.sjlbkw.cn/Article/details/gvaqjdfut.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.bbcook.cn/Article/details/gjnbkwknt.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gksqjrdpg.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gkcvcrfqn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/gzktehhsk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.vehdjk.com/Article/details/gnbrqrvmv.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.yfazqb.com/Article/details/gzhdrgpak.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.vehdjk.com/Article/details/ggxjibgoa.sHtML

[F09] 获取文件大小
来源：http://3g.vehdjk.com/Article/details/gnhifxrfw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gpgftjwij.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gyxbxabdz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/ghaypdilf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/gimvcctxl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gzgoilpxi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.sjlbkw.cn/Article/details/gjuulhrgm.sHtML

Ruby: File.size("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gaqvbwoin.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.epnwcf.com/Article/details/gvjjfxnob.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.bbcook.cn/Article/details/gxwdkcdhx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gmdstedrr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.epnwcf.com/Article/details/gfhbzectg.sHtML


<!-- 参考信息 -->