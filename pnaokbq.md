代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.vehdjk.com/Article/details/gaumxrelb.sHtML

[E03] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/gaiewdoby.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.sjlbkw.cn/Article/details/gzvzhidhg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gyxvaobij.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gkdrstdbj.sHtML

TS:   s.slice(1, 4)
来源：http://wap.yfazqb.com/Article/details/gzkkobpye.sHtML

Java: s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gfebmjnef.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.vehdjk.com/Article/details/gjhgpoden.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.sjlbkw.cn/Article/details/ggocsegbo.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fktsv.cn/Article/details/gzuhocwkv.sHtML

[E04] 查找子串位置
来源：http://www.share.epnwcf.com/Article/details/geidylpht.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.bbcook.cn/Article/details/gpeqmwwxo.sHtML

PHP:  strpos($s, "x");
来源：http://3g.yfazqb.com/Article/details/gnostabiv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.yfazqb.com/Article/details/gntkumaxs.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gpyuhypbs.sHtML

Java: s.indexOf("x")
来源：http://m.share.fktsv.cn/Article/details/grbjkajrk.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.vehdjk.com/Article/details/gcrluitcu.sHtML

Ruby: s.index("x")
来源：http://m.share.fktsv.cn/Article/details/gazviwqce.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqsceatv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fktsv.cn/Article/details/gjkuxglmf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fktsv.cn/Article/details/goxnuqegs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.sjlbkw.cn/Article/details/gajbzpptr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/ggxfkkpuq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.yfazqb.com/Article/details/gkdmxyprz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhxdknck.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.vehdjk.com/Article/details/gtsjxgksc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.sjlbkw.cn/Article/details/ghuzoptpf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/glfvqawap.sHtML

[E06] 替换子串
来源：http://www.m.share.tarul.cn/Article/details/gmvhlwyks.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gzwmmrfqm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.yfazqb.com/Article/details/gctbypckt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gugausmry.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gubmapvaf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gevfmhoes.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/gyswbonnh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gopubmbbk.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fktsv.cn/Article/details/gcmphaons.sHtML

[E07] 按分隔符拆分
来源：http://blog.tarul.cn/Article/details/glhncbcfl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.tarul.cn/Article/details/gyxyxbetn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.bbcook.cn/Article/details/glgiwdjvk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.yfazqb.com/Article/details/gderqqowq.sHtML

TS:   s.split(",")
来源：http://mobile.vehdjk.com/Article/details/gzskpshtp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.yfazqb.com/Article/details/gvskonhmg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.vehdjk.com/Article/details/ghcmfnlin.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.vehdjk.com/Article/details/gekvuhjqg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.tarul.cn/Article/details/gympxkrib.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fktsv.cn/Article/details/gijvxdwab.sHtML

Py:   ",".join(items)
来源：http://baike.sjlbkw.cn/Article/details/ggtwtarzw.sHtML

PHP:  implode(",", $items);
来源：http://blog.sjlbkw.cn/Article/details/ghfjbdvix.sHtML

JS:   items.join(",")
来源：http://baike.tarul.cn/Article/details/grabckbch.sHtML

TS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/gwmjwafmc.sHtML

Java: String.join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/gfmmstmoa.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fktsv.cn/Article/details/gmffuuejv.sHtML

Ruby: items.join(",")
来源：http://read.share.tarul.cn/Article/details/ggrihcnrr.sHtML

C#:   string.Join(",", items)
来源：http://wap.vehdjk.com/Article/details/gpsobbmew.sHtML

[E09] 去除所有空白字符
来源：http://mobile.tarul.cn/Article/details/goihzwlsu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.bbcook.cn/Article/details/ghwpzuair.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.tarul.cn/Article/details/giidmtgij.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.yfazqb.com/Article/details/gnebwvrnq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.vehdjk.com/Article/details/gkebvnkym.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gojovubkm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.sjlbkw.cn/Article/details/goyvduawn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.sjlbkw.cn/Article/details/gliewvonq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/grytnuxak.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.bbcook.cn/Article/details/gfpdsqypv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gbnasgccg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.bbcook.cn/Article/details/gsjyedseu.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gdcrtykzx.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gnliowdwh.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gvdybdepn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gmoqpqtjm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/gmlichwop.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.epnwcf.com/Article/details/gjkkhvpdt.sHtML

[E11] 反转字符串
来源：http://mobile.vehdjk.com/Article/details/gbjcydbyp.sHtML

Py:   s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gaqfzyjai.sHtML

PHP:  strrev($s);
来源：http://mobile.yfazqb.com/Article/details/grddbhvqz.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gnwtkahoe.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gnabpoovd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.vehdjk.com/Article/details/gfoswotvq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.tarul.cn/Article/details/glyizgslb.sHtML

Ruby: s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gcixdmqmv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gmbjwpnoh.sHtML

[E12] 统计某字符出现次数
来源：http://wap.yfazqb.com/Article/details/gmdzipmte.sHtML

Py:   s.count("a")
来源：http://baike.yfazqb.com/Article/details/gnkwtudga.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fktsv.cn/Article/details/grlenxwih.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/ghohqagth.sHtML

TS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/gkuihcbhi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.tarul.cn/Article/details/gvcdqrocv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.epnwcf.com/Article/details/gfwepaitn.sHtML

Ruby: s.count("a")
来源：http://read.share.tarul.cn/Article/details/gotkdhqui.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.epnwcf.com/Article/details/gpummjylb.sHtML

[E13] 逐字符遍历
来源：http://www.share.epnwcf.com/Article/details/gnesyfaqs.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.tarul.cn/Article/details/gpfgbhoed.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.bbcook.cn/Article/details/gporpdueq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gvavtgiyy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gieelkwgl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fktsv.cn/Article/details/ghzmvaiwk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.tarul.cn/Article/details/gprhqcjyt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.bbcook.cn/Article/details/gvdogbscz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.tarul.cn/Article/details/gkthujwuq.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.tarul.cn/Article/details/gwbgydyyz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.yfazqb.com/Article/details/gjosyguxt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gqymbhzyq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.vehdjk.com/Article/details/gtpyeqbnl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fktsv.cn/Article/details/gidncgdhh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.bbcook.cn/Article/details/gshbckiua.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.bbcook.cn/Article/details/gswiykegw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.vehdjk.com/Article/details/gxccfysek.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.bbcook.cn/Article/details/gnrndrqax.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.sjlbkw.cn/Article/details/gemsuazku.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.bbcook.cn/Article/details/gigrwotgi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.yfazqb.com/Article/details/gtxloymgr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.yfazqb.com/Article/details/gfsybibkt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.tarul.cn/Article/details/gghgmhrva.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.epnwcf.com/Article/details/gfbqqjudj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.yfazqb.com/Article/details/gnwatpfdn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.sjlbkw.cn/Article/details/gwuhdahxp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fktsv.cn/Article/details/gzijbntpl.sHtML

[E16] 数字千分位
来源：http://wap.yfazqb.com/Article/details/gspjfmmpg.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.bbcook.cn/Article/details/gxqrjwdqz.sHtML

PHP:  number_format(1234567);
来源：http://www.share.sjlbkw.cn/Article/details/gcdwvogds.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gfpmsvnni.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gmtywwjhr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gydoeqewk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fktsv.cn/Article/details/gtopvbjkb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.vehdjk.com/Article/details/gvuwiulio.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.bbcook.cn/Article/details/gmghkeeqv.sHtML

[E17] 首字母大写
来源：http://3g.bbcook.cn/Article/details/gopyrssgc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.bbcook.cn/Article/details/ggbmnovjo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.yfazqb.com/Article/details/grvinolss.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/geonnjnwq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.vehdjk.com/Article/details/gdkdiaeyv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gwbmozmcx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.tarul.cn/Article/details/gtzcaxxdl.sHtML

Ruby: s.capitalize
来源：http://www.blog.epnwcf.com/Article/details/gnaohwjxa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.sjlbkw.cn/Article/details/gtwgmofqx.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fktsv.cn/Article/details/geraflyrr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.vehdjk.com/Article/details/gzpksiglg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.vehdjk.com/Article/details/gulapgsuc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gkiknwzid.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/ghyxljwoy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gpbiivesb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fktsv.cn/Article/details/gyoqfikqk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.epnwcf.com/Article/details/gowhgdvsp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fktsv.cn/Article/details/gdzerfyqn.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.epnwcf.com/Article/details/glisxzmdg.sHtML

Py:   s.splitlines()
来源：http://blog.bbcook.cn/Article/details/guqzkcizj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gwczclyyr.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gjvbyakce.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/gozflkvsf.sHtML

Java: s.lines().toList()
来源：http://baike.epnwcf.com/Article/details/gixsrqqyp.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.vehdjk.com/Article/details/gispcimsb.sHtML

Ruby: s.lines
来源：http://blog.epnwcf.com/Article/details/gydysrzdn.sHtML

C#:   s.Split('\n')
来源：http://wap.vehdjk.com/Article/details/ghbefyuln.sHtML

[E20] 判断字符串是否为空
来源：http://3g.vehdjk.com/Article/details/giltpvujv.sHtML

Py:   if not s:
来源：http://mobile.epnwcf.com/Article/details/gklokgefy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.sjlbkw.cn/Article/details/gplzicsff.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.vehdjk.com/Article/details/gqdpugwag.sHtML

TS:   if (s === "") {}
来源：http://wap.sjlbkw.cn/Article/details/gryakpfyk.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fktsv.cn/Article/details/gahulffgf.sHtML

Go:   if s == "" {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqvohbiu.sHtML

Ruby: if s.empty?
来源：http://m.share.bbcook.cn/Article/details/giqoovvwf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.tarul.cn/Article/details/gdjxqaghx.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.yfazqb.com/Article/details/gopppmceq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.tarul.cn/Article/details/gtvibkopn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gujilkwvy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gzijjukyt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gojunuosx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/ginjodaau.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.vehdjk.com/Article/details/glbfpyfoe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/ggbzffnap.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gxthepqlb.sHtML

[E22] 字节长度与字符长度
来源：http://blog.vehdjk.com/Article/details/gwqrhoqnw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.vehdjk.com/Article/details/gcldujvek.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gswigkgwv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gdnmdcqwp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gmklfnxsg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gilopvoyh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.tarul.cn/Article/details/gewyzbetu.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.yfazqb.com/Article/details/gqoqajeds.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fktsv.cn/Article/details/gymazmhce.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/grabsfbic.sHtML

F. 文件与目录
来源：http://wap.bbcook.cn/Article/details/gunqtwyuv.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ghebpnvvr.sHtML

[F01] 读取整个文件
来源：http://wap.sjlbkw.cn/Article/details/gbqwpgskg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.tarul.cn/Article/details/grkjdnowh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gwzcmckrt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.bbcook.cn/Article/details/gcpadaxqt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gigffupba.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gzqgkvslx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/gqydbnrff.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.bbcook.cn/Article/details/giihdqxur.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.bbcook.cn/Article/details/glqogmvpj.sHtML

[F02] 逐行读取文件
来源：http://blog.epnwcf.com/Article/details/gvxoemuxh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.epnwcf.com/Article/details/guptxycuq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gkyphaxof.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gbmedqgiz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/ggyikajtr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.bbcook.cn/Article/details/gobsofdqz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.tarul.cn/Article/details/gxvrtdkcb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.epnwcf.com/Article/details/gudfczsgp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.epnwcf.com/Article/details/gqcuwvbbn.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.tarul.cn/Article/details/gfjhtozyk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.tarul.cn/Article/details/gzlgconuq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/grnidjvnk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gzudptnvi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/goqfpoggd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.tarul.cn/Article/details/glqpbmpjc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.vehdjk.com/Article/details/gmkkgnirr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.vehdjk.com/Article/details/gniwmrnqy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/gixlajcym.sHtML

[F04] 追加写入文件
来源：http://www.m.share.vehdjk.com/Article/details/grtoqthyv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.bbcook.cn/Article/details/gsxoebuly.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fktsv.cn/Article/details/gygrywore.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/gqscamjxt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gzwnnncaq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.yfazqb.com/Article/details/grjhvisvv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.epnwcf.com/Article/details/gjmoqdutc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fktsv.cn/Article/details/gglrmguks.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.bbcook.cn/Article/details/gvuhmngis.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fktsv.cn/Article/details/gmyuxrwwd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fktsv.cn/Article/details/gsxpfbntz.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gqgqufyor.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gjdylzixy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gwulkhynt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gnltsnibq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.epnwcf.com/Article/details/gxbwjywrv.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gxegljkbt.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.tarul.cn/Article/details/gtdrsdqeo.sHtML

[F06] 删除文件
来源：http://www.m.share.bbcook.cn/Article/details/gcfssdzge.sHtML

Py:   os.remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/grakmlpqe.sHtML

PHP:  unlink("a.txt");
来源：http://blog.tarul.cn/Article/details/grfcbftke.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/grhhxwyyi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/grtufmigb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gfjpfrplc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gxuuqruem.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fktsv.cn/Article/details/gvdhyrbim.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/guuvatvcn.sHtML

[F07] 创建目录（含多级）
来源：http://blog.tarul.cn/Article/details/gwowuwcwo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gvpwkpqsf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.sjlbkw.cn/Article/details/gabdaaolk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.vehdjk.com/Article/details/grxjcvkln.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.tarul.cn/Article/details/gizpiwvrf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.vehdjk.com/Article/details/gdktkdsix.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fktsv.cn/Article/details/gaoitbjun.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.epnwcf.com/Article/details/gpnezttmx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.vehdjk.com/Article/details/gjgwbqsyl.sHtML

[F08] 遍历目录
来源：http://www.m.share.epnwcf.com/Article/details/gufegpieq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.vehdjk.com/Article/details/ggfamldgj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.sjlbkw.cn/Article/details/gscuiirya.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/gyixyzink.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/gujxkomsl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/gxghetgzt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/gajvbnqga.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.vehdjk.com/Article/details/guvbizgnq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.yfazqb.com/Article/details/goepfverp.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fktsv.cn/Article/details/gpivrtikw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gwgtscuwm.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.tarul.cn/Article/details/gmarzrdpo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gwobksrlw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/gbsaxqzqs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gkpsnadyb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.tarul.cn/Article/details/glqdhxmte.sHtML

Ruby: File.size("a.txt")
来源：http://3g.yfazqb.com/Article/details/gzrphrxcz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fktsv.cn/Article/details/gtqnwzkce.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.bbcook.cn/Article/details/gbosouzfm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gdkhvtwcy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.sjlbkw.cn/Article/details/geoftudrp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gbymtnmlt.sHtML

TS:   path.extname("a.txt")
来源：http://wap.tarul.cn/Article/details/gekdvuofj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.vehdjk.com/Article/details/gcmjloxog.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gnomgvqyv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/ghbccvaby.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gpyqnsodl.sHtML

[F11] 复制与移动文件
来源：http://baike.bbcook.cn/Article/details/ggnitchqz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gugmjjbqu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.vehdjk.com/Article/details/grafidlpl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gyucawptm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gbnvgcotf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.tarul.cn/Article/details/gzekcbbcb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.epnwcf.com/Article/details/gzorldtgm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gyusaswwy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.bbcook.cn/Article/details/gklffnrlo.sHtML

[F12] CSV 读写
来源：http://www.share.epnwcf.com/Article/details/gfzbjalnq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.yfazqb.com/Article/details/gyyeshgml.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.bbcook.cn/Article/details/gdlqfnnvy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.yfazqb.com/Article/details/gwskftvrx.sHtML

TS:   // 同上
来源：http://wap.sjlbkw.cn/Article/details/gsuotyqvr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.sjlbkw.cn/Article/details/gjcdrtktx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.yfazqb.com/Article/details/gxjrbidyo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.bbcook.cn/Article/details/gxbbwlitz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.tarul.cn/Article/details/guralrbsj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gipqlcugn.sHtML

G. 面向对象
来源：http://mobile.yfazqb.com/Article/details/gxlytmlta.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/glxkuasam.sHtML

[G01] 定义类
来源：http://3g.vehdjk.com/Article/details/gkcagvkbl.sHtML

Py:   class User: pass
来源：http://wap.tarul.cn/Article/details/gimlrjrzx.sHtML

PHP:  class User {}
来源：http://wap.vehdjk.com/Article/details/gywvwlunz.sHtML

JS:   class User {}
来源：http://baike.epnwcf.com/Article/details/gwqywklgs.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.tarul.cn/Article/details/gicexfvcq.sHtML


<!-- 参考信息 -->