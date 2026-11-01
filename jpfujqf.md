代发 wailian999

Java: String.join(", ", list)
来源：http://wap.bbcook.cn/Article/details/glbyzlllb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.tarul.cn/Article/details/gfpspkncc.sHtML

Ruby: arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gvwxkhggt.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/grstkdrta.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/grzmkfssl.sHtML

E. 字符串处理
来源：http://read.share.vehdjk.com/Article/details/geqhcykoe.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/goidzlhth.sHtML

[E01] 拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/glunotcwa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.yfazqb.com/Article/details/gtguihflf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.tarul.cn/Article/details/gtqobungt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/gebioaylg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/gmxcuqada.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.tarul.cn/Article/details/gbxkroetb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.vehdjk.com/Article/details/gvqkasjrf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.epnwcf.com/Article/details/gvvvzyshn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.vehdjk.com/Article/details/gpbrqcaqq.sHtML

[E02] 重复字符串
来源：http://www.share.sjlbkw.cn/Article/details/galvartmw.sHtML

Py:   "ab" * 3
来源：http://wap.tarul.cn/Article/details/gyiueovix.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fktsv.cn/Article/details/gyiochkqe.sHtML

JS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/glgottpil.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gevlqqzxj.sHtML

Java: "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/grvkgpcjx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.sjlbkw.cn/Article/details/ganheqfyk.sHtML

Ruby: "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gsoqdqzvc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.bbcook.cn/Article/details/gcngyuisz.sHtML

[E03] 截取子串
来源：http://read.share.bbcook.cn/Article/details/gccyzlxan.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.bbcook.cn/Article/details/gxnduzahq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gfocwqscu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gndehuqoh.sHtML

TS:   s.slice(1, 4)
来源：http://3g.tarul.cn/Article/details/gwtxcsqiw.sHtML

Java: s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/grnylydbd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.vehdjk.com/Article/details/gxbnmzkom.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.yfazqb.com/Article/details/gufxdksed.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.bbcook.cn/Article/details/gjqaqgwur.sHtML

[E04] 查找子串位置
来源：http://www.m.share.vehdjk.com/Article/details/gewcfnfqe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.yfazqb.com/Article/details/gbgjbujqi.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.vehdjk.com/Article/details/gdijinpvy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.bbcook.cn/Article/details/gwuvwubdo.sHtML

TS:   s.indexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gxuiffhlz.sHtML

Java: s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/grsfjmkdb.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.bbcook.cn/Article/details/gihiiovjr.sHtML

Ruby: s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/ghtlkbjnp.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gjhaolgpm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.bbcook.cn/Article/details/gflmssums.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fktsv.cn/Article/details/gglxppnhf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.bbcook.cn/Article/details/gppfjkdnx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gnnbfvjnq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fktsv.cn/Article/details/gytupmwxf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/gusrarbln.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.tarul.cn/Article/details/gradwfuzm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.epnwcf.com/Article/details/gfitbojgs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.tarul.cn/Article/details/gypxmtiqa.sHtML

[E06] 替换子串
来源：http://blog.yfazqb.com/Article/details/ghmxqskxs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/gfbxbiqgi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.vehdjk.com/Article/details/gjjdcsyrs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gyujxwklu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gkqurschg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/glnspyrpd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/ggjhqgypd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.tarul.cn/Article/details/gmmzfjjjt.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/geutmvidt.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fktsv.cn/Article/details/gxcxadjua.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.yfazqb.com/Article/details/gmolhcmkf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.vehdjk.com/Article/details/gdizgbpwf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.tarul.cn/Article/details/gnwfioocg.sHtML

TS:   s.split(",")
来源：http://3g.vehdjk.com/Article/details/gexlntopd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.bbcook.cn/Article/details/gzmprnvsw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.bbcook.cn/Article/details/gxmspcvyj.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.tarul.cn/Article/details/gotprgyar.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.bbcook.cn/Article/details/gdntpjora.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.epnwcf.com/Article/details/gtvcpfdgc.sHtML

Py:   ",".join(items)
来源：http://baike.vehdjk.com/Article/details/gcyngofqy.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.yfazqb.com/Article/details/gtgyvcwko.sHtML

JS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gtgeypyci.sHtML

TS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/gyltdufjv.sHtML

Java: String.join(",", items)
来源：http://baike.epnwcf.com/Article/details/gdvabtfqh.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.bbcook.cn/Article/details/grfbgomoe.sHtML

Ruby: items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gkphfloqi.sHtML

C#:   string.Join(",", items)
来源：http://read.share.vehdjk.com/Article/details/gxnbzczru.sHtML

[E09] 去除所有空白字符
来源：http://www.share.vehdjk.com/Article/details/gjhcfokxr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fktsv.cn/Article/details/gikihcxet.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gnksmxgvj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gbcfawjeh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gtzhddadn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gsgbuxxnt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.tarul.cn/Article/details/gvszhvrii.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fktsv.cn/Article/details/gyydypjoy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gterssvws.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fktsv.cn/Article/details/gjofuqyqg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/ghoyjgked.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.epnwcf.com/Article/details/grtfbunod.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gwuwysfad.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/ghsiwrear.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gkawzchut.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gigwzujyw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/ghyhelgmn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.sjlbkw.cn/Article/details/gljxjhuxl.sHtML

[E11] 反转字符串
来源：http://www.blog.vehdjk.com/Article/details/gcviuzeys.sHtML

Py:   s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gsryqwxkj.sHtML

PHP:  strrev($s);
来源：http://www.share.vehdjk.com/Article/details/ghmdmpvmz.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/garxibjrz.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gtzbnuhfd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.epnwcf.com/Article/details/gkkbvfjmn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.vehdjk.com/Article/details/gfkxggerc.sHtML

Ruby: s.reverse
来源：http://read.share.epnwcf.com/Article/details/gxnypswug.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/gwmtlvhug.sHtML

[E12] 统计某字符出现次数
来源：http://blog.sjlbkw.cn/Article/details/gipyyhfky.sHtML

Py:   s.count("a")
来源：http://m.share.yfazqb.com/Article/details/gottwodvz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.bbcook.cn/Article/details/giatsadiy.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gbqrsgusx.sHtML

TS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/gsgmpiyvz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.epnwcf.com/Article/details/gqpuwdcvw.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.epnwcf.com/Article/details/gvhkijfnk.sHtML

Ruby: s.count("a")
来源：http://blog.epnwcf.com/Article/details/gtdadwepf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.bbcook.cn/Article/details/guhvmjddk.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.epnwcf.com/Article/details/gfklqzdst.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fktsv.cn/Article/details/gtxpdoawe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.sjlbkw.cn/Article/details/gwnyvbqio.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.yfazqb.com/Article/details/gbrxcykhf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.vehdjk.com/Article/details/gyjqdvhmu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.tarul.cn/Article/details/gfqhtxadx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.bbcook.cn/Article/details/gvckfazfk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.sjlbkw.cn/Article/details/gtzlfoxwo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gccoxqfaj.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fktsv.cn/Article/details/ggggtwfbn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.epnwcf.com/Article/details/glxvyjatw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.epnwcf.com/Article/details/gwatfekzw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.sjlbkw.cn/Article/details/gkqlnkdmw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.vehdjk.com/Article/details/gqvjfrgiy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gfjcgmkhu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.yfazqb.com/Article/details/gjbfezakf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fktsv.cn/Article/details/gxcnjacjj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gilkarext.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.vehdjk.com/Article/details/gyytxqajg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.yfazqb.com/Article/details/grvhiifjw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.bbcook.cn/Article/details/gwgqeumjs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/grovvuudz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.yfazqb.com/Article/details/gcxcwlgab.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fktsv.cn/Article/details/gjsutbeht.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.epnwcf.com/Article/details/gijejuxyk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdfmiscj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.bbcook.cn/Article/details/grgaatdza.sHtML

[E16] 数字千分位
来源：http://www.share.sjlbkw.cn/Article/details/grpzocbny.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.tarul.cn/Article/details/gwojdtasv.sHtML

PHP:  number_format(1234567);
来源：http://blog.vehdjk.com/Article/details/gbiumcdmy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/gffqoueev.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.epnwcf.com/Article/details/gqkgoygor.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.vehdjk.com/Article/details/gcmdyanrt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.epnwcf.com/Article/details/goibybaut.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.yfazqb.com/Article/details/gnrjzmmew.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fktsv.cn/Article/details/gxwodpztj.sHtML

[E17] 首字母大写
来源：http://baike.bbcook.cn/Article/details/gyzzvncpl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fktsv.cn/Article/details/gbhnqewev.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.vehdjk.com/Article/details/ghxmbaqcb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/gspatxtfz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gypozknmb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.epnwcf.com/Article/details/gdonibcip.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.tarul.cn/Article/details/gkdftkutb.sHtML

Ruby: s.capitalize
来源：http://m.share.tarul.cn/Article/details/gxohcibpv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.sjlbkw.cn/Article/details/gtbfkaeid.sHtML

[E18] 模板占位符替换
来源：http://m.share.fktsv.cn/Article/details/goohundql.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.epnwcf.com/Article/details/gmyywfygm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.sjlbkw.cn/Article/details/gunlyrbuf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gwgbrxwbp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gwrvagoyc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/ghpflqxet.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/ggzfahtzv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.tarul.cn/Article/details/gpuzdyjal.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.tarul.cn/Article/details/gjtimbywk.sHtML

[E19] 多行文本按行拆分
来源：http://wap.bbcook.cn/Article/details/goshnztzh.sHtML

Py:   s.splitlines()
来源：http://mobile.epnwcf.com/Article/details/gudmhosuu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.tarul.cn/Article/details/glktpddbg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/gvnpvgimb.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gznizqqho.sHtML

Java: s.lines().toList()
来源：http://baike.bbcook.cn/Article/details/geeccqlgt.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.bbcook.cn/Article/details/gveclhgwu.sHtML

Ruby: s.lines
来源：http://baike.tarul.cn/Article/details/gpmrsyeuh.sHtML

C#:   s.Split('\n')
来源：http://www.blog.epnwcf.com/Article/details/gecjgypeb.sHtML

[E20] 判断字符串是否为空
来源：http://wap.vehdjk.com/Article/details/gkjiptini.sHtML

Py:   if not s:
来源：http://baike.vehdjk.com/Article/details/gryxfkvof.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.vehdjk.com/Article/details/gugjulrrz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.tarul.cn/Article/details/gpfllgpck.sHtML

TS:   if (s === "") {}
来源：http://blog.yfazqb.com/Article/details/gcsljofgg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/gkeiixfpv.sHtML

Go:   if s == "" {}
来源：http://read.share.vehdjk.com/Article/details/gcpnpxfqg.sHtML

Ruby: if s.empty?
来源：http://3g.bbcook.cn/Article/details/gjsfcqtco.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.tarul.cn/Article/details/gatjrzovx.sHtML

[E21] 超长截断加省略号
来源：http://baike.yfazqb.com/Article/details/gxdevnhid.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fktsv.cn/Article/details/ghinqqbnh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gbsjypnng.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gxhewebcq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gvawrirhn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/glnlhcdgb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.vehdjk.com/Article/details/gipbgpana.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gqlvyfhym.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gdtoixuge.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.epnwcf.com/Article/details/giezcfsac.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.tarul.cn/Article/details/gdptvhubd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gftkkefqj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.tarul.cn/Article/details/gvktaokde.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/gfpxdtccp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fktsv.cn/Article/details/geqeevfqh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.epnwcf.com/Article/details/gmyfxxawm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gxmdbrijq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.vehdjk.com/Article/details/gcdmxlawh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/guemyfvyf.sHtML

F. 文件与目录
来源：http://wap.yfazqb.com/Article/details/gnjtczyih.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gwzamkrrh.sHtML

[F01] 读取整个文件
来源：http://m.share.sjlbkw.cn/Article/details/gdjyduvcz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.yfazqb.com/Article/details/gvddptrud.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.tarul.cn/Article/details/gfkzzlsyd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.vehdjk.com/Article/details/gvkiptapr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.vehdjk.com/Article/details/grdduifzn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gebbizyoy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.epnwcf.com/Article/details/gcrmfibiw.sHtML

Ruby: File.read("a.txt")
来源：http://baike.vehdjk.com/Article/details/gbjnnwkst.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.tarul.cn/Article/details/gdkhpzuzh.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.tarul.cn/Article/details/gjulbvnki.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.tarul.cn/Article/details/gyinpynsj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.yfazqb.com/Article/details/gexrqfako.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/gypehhnmm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gilyfquxk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.vehdjk.com/Article/details/gimqcaqem.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.vehdjk.com/Article/details/gzullswdh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.vehdjk.com/Article/details/gfnhciqph.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fktsv.cn/Article/details/gdjtoujqq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.tarul.cn/Article/details/getzpoflq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.bbcook.cn/Article/details/gdfruauah.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gvhdrnwdd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/gyinfmbpm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gyqsckjob.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.bbcook.cn/Article/details/gjhinsxzf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fktsv.cn/Article/details/gdexxwpns.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.bbcook.cn/Article/details/grbodrhdy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/gxjhagntj.sHtML

[F04] 追加写入文件
来源：http://www.blog.yfazqb.com/Article/details/gncylepvv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.vehdjk.com/Article/details/guvnhkiwq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.tarul.cn/Article/details/gtaviuipe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/gewyyblbx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/ghvnsgtoq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.epnwcf.com/Article/details/gmfrujjus.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/gyqydyhtj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.sjlbkw.cn/Article/details/ghnpojryb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.vehdjk.com/Article/details/gnpeonbrg.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.bbcook.cn/Article/details/ghmxywmww.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fktsv.cn/Article/details/gozknpjso.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.tarul.cn/Article/details/gkiaxtyvh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gmsploqhp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gjlfzuonr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gutoikuhk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fktsv.cn/Article/details/grlaklicc.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gwybgdmmo.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fktsv.cn/Article/details/glxjyebfh.sHtML

[F06] 删除文件
来源：http://3g.bbcook.cn/Article/details/gzfpnexud.sHtML

Py:   os.remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gbopiirtn.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gtqktbtmg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gwqamirer.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gcjguwnuy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gmypuktqs.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gpptebqhj.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.bbcook.cn/Article/details/googwouuu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gnrxubkfv.sHtML

[F07] 创建目录（含多级）
来源：http://3g.epnwcf.com/Article/details/gulicfhce.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.vehdjk.com/Article/details/gktwnowee.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.tarul.cn/Article/details/gxzrgylyh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.epnwcf.com/Article/details/govcckniu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/gakouymxa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.bbcook.cn/Article/details/gjbpouykd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.yfazqb.com/Article/details/ghzpndxhx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.vehdjk.com/Article/details/gynjjrogq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fktsv.cn/Article/details/gpffjkjcg.sHtML

[F08] 遍历目录
来源：http://blog.epnwcf.com/Article/details/gbvrfkrfs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.vehdjk.com/Article/details/gnnloipgr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.tarul.cn/Article/details/guensxlds.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/gjrhoryhg.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/gtqruqbkb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fktsv.cn/Article/details/gqgozjabd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fktsv.cn/Article/details/ggkjrpwhu.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.yfazqb.com/Article/details/girumuawk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.vehdjk.com/Article/details/ggzlxmoha.sHtML

[F09] 获取文件大小
来源：http://www.share.epnwcf.com/Article/details/gnzeskfxq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.bbcook.cn/Article/details/gqgesvagb.sHtML

PHP:  filesize("a.txt");
来源：http://wap.tarul.cn/Article/details/gdcwsqfft.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/gaoqtszru.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fktsv.cn/Article/details/ghfqqbtkx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gmhznsimi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.tarul.cn/Article/details/giwahvnwu.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gxobymjif.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.vehdjk.com/Article/details/gncceoxuw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.epnwcf.com/Article/details/gpslrwqqr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gatddvnvp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.vehdjk.com/Article/details/guyidbusi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gmijjthks.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gyszgdbqx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.vehdjk.com/Article/details/gybdmjsyx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gaxmhihmc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/grtbeypym.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/giymftpin.sHtML

[F11] 复制与移动文件
来源：http://www.blog.vehdjk.com/Article/details/gmforlmum.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gajfeanvt.sHtML


<!-- 参考信息 -->