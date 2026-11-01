代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://m.share.tarul.cn/Article/details/gjewkaisd.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fktsv.cn/Article/details/gysejmyso.sHtML

JS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/glexnmuwe.sHtML

TS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gwpzzkxvh.sHtML

Java: String.join(", ", list)
来源：http://wap.vehdjk.com/Article/details/gsasjgmaq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fktsv.cn/Article/details/gdhdqtlvx.sHtML

Ruby: arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gsoolgqfi.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.sjlbkw.cn/Article/details/gnvyucrak.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glixjjaby.sHtML

E. 字符串处理
来源：http://www.blog.bbcook.cn/Article/details/gaosyqkdx.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gmmvomkpb.sHtML

[E01] 拼接字符串
来源：http://baike.yfazqb.com/Article/details/grnvtqdwo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.tarul.cn/Article/details/geeefgisp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.yfazqb.com/Article/details/guktilzud.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/gxotuqqbi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gfbddttok.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.vehdjk.com/Article/details/gsafzyrsp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fktsv.cn/Article/details/grrnngqpn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.bbcook.cn/Article/details/gcbeulfpa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.epnwcf.com/Article/details/ghgignpry.sHtML

[E02] 重复字符串
来源：http://baike.epnwcf.com/Article/details/guapuomkp.sHtML

Py:   "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/gwdcnirry.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.bbcook.cn/Article/details/gdbjicedf.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gxgcyjtgg.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gwelwpxti.sHtML

Java: "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gsucuximc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.bbcook.cn/Article/details/gwxawqxci.sHtML

Ruby: "ab" * 3
来源：http://read.share.tarul.cn/Article/details/gbuqdzcva.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fktsv.cn/Article/details/gpqaeixjp.sHtML

[E03] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/gbkvlzvrb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.vehdjk.com/Article/details/gslfwromp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gfucmwysf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gvqbomurl.sHtML

TS:   s.slice(1, 4)
来源：http://baike.epnwcf.com/Article/details/gwvsmimad.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gxsddmahg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.vehdjk.com/Article/details/gjtysndgh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.tarul.cn/Article/details/gjtfwleqo.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.bbcook.cn/Article/details/gkiomaike.sHtML

[E04] 查找子串位置
来源：http://www.blog.yfazqb.com/Article/details/gycpeocgy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.vehdjk.com/Article/details/gvssxdepd.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fktsv.cn/Article/details/goxktitfj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.epnwcf.com/Article/details/gbseijsqu.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gjylaszny.sHtML

Java: s.indexOf("x")
来源：http://blog.tarul.cn/Article/details/gsmeynojj.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.yfazqb.com/Article/details/gfchhmwhs.sHtML

Ruby: s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/ghjnztapp.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gxsifbovo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.vehdjk.com/Article/details/grvasvlpc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.bbcook.cn/Article/details/ganbnvchs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.sjlbkw.cn/Article/details/gagsdkgwp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gxdhdlysz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.epnwcf.com/Article/details/gaczqvpoc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gcvuhywhi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fktsv.cn/Article/details/ghcwebiqc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.bbcook.cn/Article/details/ggftkuvrn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gybmujcan.sHtML

[E06] 替换子串
来源：http://baike.bbcook.cn/Article/details/gtvsltplz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.yfazqb.com/Article/details/gnifqqqjz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fktsv.cn/Article/details/gousrchkw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/ggxlnrhag.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gigbreptu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gwczymvts.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/gkzvsnbaj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fktsv.cn/Article/details/gyzkdllqb.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gyxotlcli.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fktsv.cn/Article/details/gzymzattg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.tarul.cn/Article/details/gyjiqeztw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.yfazqb.com/Article/details/ghozwpwvs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.bbcook.cn/Article/details/gvvocthdw.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/geodutsdo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.sjlbkw.cn/Article/details/gswnpabzh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.sjlbkw.cn/Article/details/gcpfmlxai.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.epnwcf.com/Article/details/guttsnygn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.bbcook.cn/Article/details/gmjafsyob.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.sjlbkw.cn/Article/details/goowncweg.sHtML

Py:   ",".join(items)
来源：http://www.share.bbcook.cn/Article/details/gucncbaza.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/goobsvhte.sHtML

JS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/gxeablfcy.sHtML

TS:   items.join(",")
来源：http://wap.fktsv.cn/Article/details/givdwuahv.sHtML

Java: String.join(",", items)
来源：http://3g.epnwcf.com/Article/details/gynkudpfd.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.vehdjk.com/Article/details/gaexdqmsr.sHtML

Ruby: items.join(",")
来源：http://baike.vehdjk.com/Article/details/gulbtnnmi.sHtML

C#:   string.Join(",", items)
来源：http://3g.bbcook.cn/Article/details/gtqokhrjk.sHtML

[E09] 去除所有空白字符
来源：http://baike.bbcook.cn/Article/details/gkdjgnxhy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fktsv.cn/Article/details/glietwcry.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.epnwcf.com/Article/details/glamdrnwq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/glyoabjkv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gfegvuxlw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.vehdjk.com/Article/details/gzmsmymij.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.epnwcf.com/Article/details/gmlzzrfai.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.bbcook.cn/Article/details/gxopwcpsc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fktsv.cn/Article/details/gsfeyudcm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.vehdjk.com/Article/details/gtgcfiepe.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gfjuzioqc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.bbcook.cn/Article/details/gjsktyily.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gkcnunrob.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/gagzphazg.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/guhldkwdj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gripgjeuz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gjidookpt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.epnwcf.com/Article/details/gqclkclli.sHtML

[E11] 反转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gayohzorj.sHtML

Py:   s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gydqeqqrl.sHtML

PHP:  strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gckvitozj.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gnichepcn.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gnorztjrp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fktsv.cn/Article/details/gzlhixjji.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.epnwcf.com/Article/details/gxgefuqly.sHtML

Ruby: s.reverse
来源：http://3g.yfazqb.com/Article/details/grdtcebyc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gdftqwkqw.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.bbcook.cn/Article/details/gdoahhuye.sHtML

Py:   s.count("a")
来源：http://wap.fktsv.cn/Article/details/gkrmehnhf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fktsv.cn/Article/details/geyreuheh.sHtML

JS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gkilbsibn.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gzobbdsbp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.sjlbkw.cn/Article/details/gtdxdcbgt.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.sjlbkw.cn/Article/details/gliedneit.sHtML

Ruby: s.count("a")
来源：http://blog.vehdjk.com/Article/details/gbiminuzf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.tarul.cn/Article/details/gipmxtawp.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.tarul.cn/Article/details/gjgtzevwf.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.yfazqb.com/Article/details/ghzjclgtc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fktsv.cn/Article/details/gptpfpyko.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gsnovplud.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.vehdjk.com/Article/details/gdnwqzxdx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.bbcook.cn/Article/details/gednkwvxf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.epnwcf.com/Article/details/gnhxrbqqt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.bbcook.cn/Article/details/gxbjsboun.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fktsv.cn/Article/details/gdiwguezk.sHtML

[E14] URL 编码与 Base64
来源：http://baike.bbcook.cn/Article/details/gmotecojz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.tarul.cn/Article/details/geygejojp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fktsv.cn/Article/details/gjsfbjavl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.vehdjk.com/Article/details/gzoqtvjof.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.tarul.cn/Article/details/gemlgfkpc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.yfazqb.com/Article/details/ggkcnltdg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.sjlbkw.cn/Article/details/gfuswnevs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fktsv.cn/Article/details/gwiwnjurh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fktsv.cn/Article/details/ghjztgbvp.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.tarul.cn/Article/details/gokylzgnj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.vehdjk.com/Article/details/gyhgdlsvp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.yfazqb.com/Article/details/gsbyocppq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.epnwcf.com/Article/details/gjdniyorj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.yfazqb.com/Article/details/gcuboiwcx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.bbcook.cn/Article/details/gaihiuyru.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gtgpjryoj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.vehdjk.com/Article/details/gbuodflig.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.epnwcf.com/Article/details/ghslmxbmj.sHtML

[E16] 数字千分位
来源：http://baike.vehdjk.com/Article/details/gprafxgej.sHtML

Py:   f"{1234567:,}"
来源：http://3g.sjlbkw.cn/Article/details/ggwermztw.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.tarul.cn/Article/details/gzeurvjet.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/gmipsunwf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gqotfutud.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.yfazqb.com/Article/details/gdkxaulji.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.bbcook.cn/Article/details/gunjvstwj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fktsv.cn/Article/details/gbupjnkmq.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.bbcook.cn/Article/details/gxglsngjm.sHtML

[E17] 首字母大写
来源：http://blog.bbcook.cn/Article/details/gaceaqqqb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.vehdjk.com/Article/details/gqzhjdohi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fktsv.cn/Article/details/gxptmkapv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.sjlbkw.cn/Article/details/geybmpuvm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/gcgaauell.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.vehdjk.com/Article/details/gbmuppduw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.sjlbkw.cn/Article/details/gxtbjrqyr.sHtML

Ruby: s.capitalize
来源：http://www.share.tarul.cn/Article/details/grcfeqjhf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fktsv.cn/Article/details/gvrqcwucc.sHtML

[E18] 模板占位符替换
来源：http://blog.epnwcf.com/Article/details/gexlxlbmv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.tarul.cn/Article/details/guaekaypc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.yfazqb.com/Article/details/glfyewxbo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/glsfqvqlo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gdsfabpcc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gevkuzvep.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.yfazqb.com/Article/details/gpdwjffww.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.sjlbkw.cn/Article/details/gssgknavf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.yfazqb.com/Article/details/gttoaaluk.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.epnwcf.com/Article/details/gjyxmiyzb.sHtML

Py:   s.splitlines()
来源：http://blog.epnwcf.com/Article/details/gculmyfsf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.vehdjk.com/Article/details/guvlwmukp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/ggnixvpwg.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/gkblopfrv.sHtML

Java: s.lines().toList()
来源：http://m.share.tarul.cn/Article/details/gdexhthob.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.bbcook.cn/Article/details/gjizguqoq.sHtML

Ruby: s.lines
来源：http://www.m.share.vehdjk.com/Article/details/gcaatdyrp.sHtML

C#:   s.Split('\n')
来源：http://www.blog.sjlbkw.cn/Article/details/gmduvmldc.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.sjlbkw.cn/Article/details/ghkcuuncr.sHtML

Py:   if not s:
来源：http://3g.bbcook.cn/Article/details/ggrnotmji.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.tarul.cn/Article/details/gwxtpgfzi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.bbcook.cn/Article/details/gulcqdnir.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.yfazqb.com/Article/details/gikwozhlm.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/gkptwooir.sHtML

Go:   if s == "" {}
来源：http://read.share.vehdjk.com/Article/details/gkvzswykn.sHtML

Ruby: if s.empty?
来源：http://mobile.epnwcf.com/Article/details/gajtyuody.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.sjlbkw.cn/Article/details/gkkntmmbc.sHtML

[E21] 超长截断加省略号
来源：http://wap.fktsv.cn/Article/details/gocfctsln.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.tarul.cn/Article/details/ggytxyswg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gixuefyre.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gdaddtbvu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gqamtunjm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/glgeitjfc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.yfazqb.com/Article/details/grbwadljs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.bbcook.cn/Article/details/guciqxxbo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.bbcook.cn/Article/details/gwphdxmzl.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.vehdjk.com/Article/details/gnyafhlty.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.vehdjk.com/Article/details/gqfvadjse.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gcnxfdcwd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gpynfvlwq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gejvonwra.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gboiutuey.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fktsv.cn/Article/details/grzzqxyep.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gpepftfuu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.sjlbkw.cn/Article/details/gzjgavxsh.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ggircagky.sHtML

F. 文件与目录
来源：http://www.share.vehdjk.com/Article/details/gonbhnvnb.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gegxbtfaa.sHtML

[F01] 读取整个文件
来源：http://www.blog.bbcook.cn/Article/details/grmuzixoj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.sjlbkw.cn/Article/details/ghfxwgowi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.vehdjk.com/Article/details/gwtnizeav.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.tarul.cn/Article/details/gejqdtgkl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gptrzwrca.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gfhcxkoqr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.epnwcf.com/Article/details/gnuzvzyki.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gljjbeanc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gvvwkhzrm.sHtML

[F02] 逐行读取文件
来源：http://3g.bbcook.cn/Article/details/grobnngya.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.sjlbkw.cn/Article/details/gtchuimrl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.tarul.cn/Article/details/gfaorbztm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.vehdjk.com/Article/details/gjlhdvted.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gvawvazsx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gpwvcgzch.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.tarul.cn/Article/details/ggbkqtmwq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.tarul.cn/Article/details/gqutzfbcd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.tarul.cn/Article/details/gquntcrug.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.vehdjk.com/Article/details/gfjedprtj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.yfazqb.com/Article/details/gucsfiwns.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gzgipbbmy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/glcljksua.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gfrfbqmfu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.bbcook.cn/Article/details/gdueyyqox.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.bbcook.cn/Article/details/gutvbosvc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fktsv.cn/Article/details/gsccscpjd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/gkpyufyvc.sHtML

[F04] 追加写入文件
来源：http://www.m.share.yfazqb.com/Article/details/gygpjxafb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gxrleesac.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.vehdjk.com/Article/details/ghmqwwgrr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gkxileibi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/gmmvebnoo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.vehdjk.com/Article/details/gepmggbhi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.yfazqb.com/Article/details/gdlxikcol.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.vehdjk.com/Article/details/gbfyhmtjb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.sjlbkw.cn/Article/details/gmvxtzdzb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.epnwcf.com/Article/details/gtxitvnby.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.vehdjk.com/Article/details/gyhrfpyho.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/glsprngpo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gsrulxuus.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/grlwbtgmm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/geyobpzvu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.epnwcf.com/Article/details/gxtcmbbdj.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.vehdjk.com/Article/details/ghcscxzzg.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.epnwcf.com/Article/details/gsulsiker.sHtML

[F06] 删除文件
来源：http://wap.vehdjk.com/Article/details/guswobpcs.sHtML

Py:   os.remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gyifgdfzf.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gcevvnezw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gfnjcfgsw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/goxwwbpmh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gyyojenrq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gfsohcnmv.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.tarul.cn/Article/details/gjkfhpgxp.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.bbcook.cn/Article/details/gpgrvmfoe.sHtML

[F07] 创建目录（含多级）
来源：http://blog.sjlbkw.cn/Article/details/gjjuzfcmp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.tarul.cn/Article/details/ghnornjaw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.epnwcf.com/Article/details/gbivmtsru.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gofskmuab.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/ginvmaljh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.epnwcf.com/Article/details/gzabftyjj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.bbcook.cn/Article/details/gccvehxbd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fktsv.cn/Article/details/gauvdrxsj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.tarul.cn/Article/details/gupostsvl.sHtML

[F08] 遍历目录
来源：http://3g.tarul.cn/Article/details/gmxdbmsnw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.epnwcf.com/Article/details/girwcehku.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.tarul.cn/Article/details/gphgqochm.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gedpepaup.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.sjlbkw.cn/Article/details/grqjoxvbe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fktsv.cn/Article/details/gxziroybd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.bbcook.cn/Article/details/giiwzkopy.sHtML

Ruby: Dir.children("dir")
来源：http://wap.yfazqb.com/Article/details/gmrbtimbg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.bbcook.cn/Article/details/gphaigdvm.sHtML

[F09] 获取文件大小
来源：http://mobile.yfazqb.com/Article/details/gtywwaawv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fktsv.cn/Article/details/gmorqwroh.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gzxfnnrzh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/gisesvokx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/gdfnvsihb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gujhvgblc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.sjlbkw.cn/Article/details/gmgrrcwst.sHtML

Ruby: File.size("a.txt")
来源：http://baike.epnwcf.com/Article/details/gcimgsnge.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fktsv.cn/Article/details/gvwtmevrx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.yfazqb.com/Article/details/gzqfqswml.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gusdcpluv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.vehdjk.com/Article/details/grdksmosm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/geaucbsrr.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gkggdsrtf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fktsv.cn/Article/details/gmrhzqpqe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gzblmwlun.sHtML


<!-- 参考信息 -->