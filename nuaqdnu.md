代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.vehdjk.com/Article/details/goldylddb.sHtML

[E03] 截取子串
来源：http://3g.tarul.cn/Article/details/ginvmfltl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.bbcook.cn/Article/details/glyybfzgm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gaxdoxivh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/gtegehcwy.sHtML

TS:   s.slice(1, 4)
来源：http://3g.epnwcf.com/Article/details/gycwmzipi.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gvgniobgs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.vehdjk.com/Article/details/gulyaagpg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.yfazqb.com/Article/details/gefqgfgea.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.bbcook.cn/Article/details/gwklvkbyt.sHtML

[E04] 查找子串位置
来源：http://read.share.fktsv.cn/Article/details/gutrpeoeo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.tarul.cn/Article/details/glirlisab.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.epnwcf.com/Article/details/gazzwwnfy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.epnwcf.com/Article/details/gixxlbrbj.sHtML

TS:   s.indexOf("x")
来源：http://mobile.bbcook.cn/Article/details/giovegwoe.sHtML

Java: s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gwcwfrvpf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.tarul.cn/Article/details/gcjhzxloq.sHtML

Ruby: s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gefqhgjxn.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gpuorhxxd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.bbcook.cn/Article/details/gbstivbku.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.yfazqb.com/Article/details/gilachfqi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.sjlbkw.cn/Article/details/ghwnzrkqj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gdcuyrqbq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.epnwcf.com/Article/details/gbttaawwr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gnngbwrjh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.tarul.cn/Article/details/ggcbetyrd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.sjlbkw.cn/Article/details/guwzwjvet.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.bbcook.cn/Article/details/glpmizcxs.sHtML

[E06] 替换子串
来源：http://baike.fktsv.cn/Article/details/ggqxnmwvo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.yfazqb.com/Article/details/gnkwrnkrm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.bbcook.cn/Article/details/gysedbayh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gdautbern.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/glclfdecc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/ggyfnxzax.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/gyjvbncyz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.vehdjk.com/Article/details/gugtztaku.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gbbwnsony.sHtML

[E07] 按分隔符拆分
来源：http://read.share.bbcook.cn/Article/details/gtbcjtwro.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.vehdjk.com/Article/details/gzkdwdisd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gcsejnyzi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fktsv.cn/Article/details/gnettbjms.sHtML

TS:   s.split(",")
来源：http://read.share.epnwcf.com/Article/details/gvicctoak.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.vehdjk.com/Article/details/gcebhumky.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.epnwcf.com/Article/details/gbivyxdma.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.vehdjk.com/Article/details/ggwprwwkt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.sjlbkw.cn/Article/details/gvhlmvtwb.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.vehdjk.com/Article/details/glpqwnefv.sHtML

Py:   ",".join(items)
来源：http://wap.sjlbkw.cn/Article/details/gghpscmkm.sHtML

PHP:  implode(",", $items);
来源：http://wap.bbcook.cn/Article/details/gthcidnaz.sHtML

JS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/gjcdrffxb.sHtML

TS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gpmaxntag.sHtML

Java: String.join(",", items)
来源：http://wap.epnwcf.com/Article/details/gzcwxcqox.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.bbcook.cn/Article/details/gnpfueuaw.sHtML

Ruby: items.join(",")
来源：http://baike.tarul.cn/Article/details/ghenbzsmw.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/gjwuwfmzk.sHtML

[E09] 去除所有空白字符
来源：http://wap.bbcook.cn/Article/details/gmzzlduxq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.sjlbkw.cn/Article/details/gojvrdbpg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gnvphivwa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/gucwmjixw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/goryxcidx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.epnwcf.com/Article/details/giejwcsei.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.sjlbkw.cn/Article/details/gvkhdqxvs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.epnwcf.com/Article/details/ghevzkqys.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gzdctbfuq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.epnwcf.com/Article/details/gtlebwrvt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.bbcook.cn/Article/details/gddltpkqa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fktsv.cn/Article/details/gvbsxhqrw.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/ggrlnmuia.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gvmyclppb.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/gerbyvhcp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gjwgchukk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/giwrccsll.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.tarul.cn/Article/details/gmmakouhc.sHtML

[E11] 反转字符串
来源：http://www.share.vehdjk.com/Article/details/ggeiebnjt.sHtML

Py:   s[::-1]
来源：http://www.share.bbcook.cn/Article/details/gxkxfkqzz.sHtML

PHP:  strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gvcvasces.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/glztwqkap.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gyeeypbsp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.epnwcf.com/Article/details/gwxweqyle.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fktsv.cn/Article/details/gebwmppft.sHtML

Ruby: s.reverse
来源：http://www.blog.epnwcf.com/Article/details/gblykszfj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/geeewjmez.sHtML

[E12] 统计某字符出现次数
来源：http://3g.yfazqb.com/Article/details/gocingknf.sHtML

Py:   s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/gzzeupojo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.vehdjk.com/Article/details/gaabdneft.sHtML

JS:   s.split("a").length - 1
来源：http://baike.epnwcf.com/Article/details/gadokoprs.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/gqxcpwisb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.bbcook.cn/Article/details/gckonnjqi.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.sjlbkw.cn/Article/details/gnoutycrw.sHtML

Ruby: s.count("a")
来源：http://mobile.fktsv.cn/Article/details/ggcmzrbaf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.bbcook.cn/Article/details/gwetbwqbz.sHtML

[E13] 逐字符遍历
来源：http://wap.vehdjk.com/Article/details/gtkwsxdos.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.bbcook.cn/Article/details/gyzxspojb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.sjlbkw.cn/Article/details/gjswfoxpo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/guyaagcag.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/gavbfgtfw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fktsv.cn/Article/details/glvptagjk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.vehdjk.com/Article/details/gyrzjyjki.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.bbcook.cn/Article/details/gyocgzbae.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fktsv.cn/Article/details/ggzwbssaq.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fktsv.cn/Article/details/gixhbjgav.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.yfazqb.com/Article/details/gsmmpkhnm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.epnwcf.com/Article/details/guzzzlznd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fktsv.cn/Article/details/gourfilmc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.bbcook.cn/Article/details/gribvoxpq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.vehdjk.com/Article/details/giopivtzb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.yfazqb.com/Article/details/gfxxshprb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.bbcook.cn/Article/details/gikxsqsya.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.epnwcf.com/Article/details/gswbabeps.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.sjlbkw.cn/Article/details/godjvyipa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.vehdjk.com/Article/details/gwydzihqy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fktsv.cn/Article/details/gmxueluwa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/geuwcyxpy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/gmdtjxfto.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.vehdjk.com/Article/details/gpdracgkq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.vehdjk.com/Article/details/gsryphwpt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.bbcook.cn/Article/details/gkapbwhcb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.vehdjk.com/Article/details/gfvjverkh.sHtML

[E16] 数字千分位
来源：http://baike.tarul.cn/Article/details/gfmjkrzng.sHtML

Py:   f"{1234567:,}"
来源：http://wap.bbcook.cn/Article/details/gjpvtpiee.sHtML

PHP:  number_format(1234567);
来源：http://blog.yfazqb.com/Article/details/gkheuyfqo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/grxycstpu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gcpqggzhp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.vehdjk.com/Article/details/gyjwiyyat.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.epnwcf.com/Article/details/gxqweorpv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.tarul.cn/Article/details/gmcptopgs.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fktsv.cn/Article/details/gwmbyeyaq.sHtML

[E17] 首字母大写
来源：http://m.share.bbcook.cn/Article/details/gohffwphk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.bbcook.cn/Article/details/ggruseanw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.sjlbkw.cn/Article/details/gtzpcjhyg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gbncujfqx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gfptlbvmu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fktsv.cn/Article/details/gsvjlykek.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gheumfszh.sHtML

Ruby: s.capitalize
来源：http://wap.yfazqb.com/Article/details/gbpscznby.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.bbcook.cn/Article/details/gljewmpze.sHtML

[E18] 模板占位符替换
来源：http://m.share.yfazqb.com/Article/details/gjpvyyefs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.yfazqb.com/Article/details/gtowyrquy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.sjlbkw.cn/Article/details/gtdjgqfsb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gztyabfwq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gzlbhqaim.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/glpvbplku.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gmavjbevy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.vehdjk.com/Article/details/guiiumerc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.yfazqb.com/Article/details/gactcfhgg.sHtML

[E19] 多行文本按行拆分
来源：http://blog.vehdjk.com/Article/details/gcxebivyz.sHtML

Py:   s.splitlines()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfcmgtgl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.vehdjk.com/Article/details/gxrjxshtp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gkcomicvt.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.bbcook.cn/Article/details/gizlcaftg.sHtML

Java: s.lines().toList()
来源：http://m.share.bbcook.cn/Article/details/gxsyenoty.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.vehdjk.com/Article/details/gygsvhswu.sHtML

Ruby: s.lines
来源：http://wap.yfazqb.com/Article/details/gyhmbcvct.sHtML

C#:   s.Split('\n')
来源：http://m.share.fktsv.cn/Article/details/gukuikzzl.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.bbcook.cn/Article/details/geleonqff.sHtML

Py:   if not s:
来源：http://3g.tarul.cn/Article/details/gcmzfdgbl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.vehdjk.com/Article/details/glwznssko.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gekfudiwn.sHtML

TS:   if (s === "") {}
来源：http://3g.bbcook.cn/Article/details/gkuehmfrb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gacfihelc.sHtML

Go:   if s == "" {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzklaybwo.sHtML

Ruby: if s.empty?
来源：http://www.blog.fktsv.cn/Article/details/gvbipcluv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fktsv.cn/Article/details/gbebuzadw.sHtML

[E21] 超长截断加省略号
来源：http://blog.yfazqb.com/Article/details/gnxwpqmdp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.sjlbkw.cn/Article/details/gtgayynxk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fktsv.cn/Article/details/gfscirrmt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gzjtwbteh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gzcsmtefu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gwbsfbzad.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.vehdjk.com/Article/details/gzszymhij.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.tarul.cn/Article/details/gqlmgeamh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gvyypbukq.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/gxbgwybwo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fktsv.cn/Article/details/gcomevsgz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gshbgkble.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gsmvirxvt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gjfkmceug.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.tarul.cn/Article/details/gkvjlibhn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.bbcook.cn/Article/details/goryncrka.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gwegtacua.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.tarul.cn/Article/details/gitrxnxgx.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghhojyfzy.sHtML

F. 文件与目录
来源：http://3g.yfazqb.com/Article/details/gbqowgblw.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grcxjjzsd.sHtML

[F01] 读取整个文件
来源：http://wap.tarul.cn/Article/details/gbqxowvpb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.vehdjk.com/Article/details/grlsdgiym.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gkwxedmfl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.vehdjk.com/Article/details/gorrzufsm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fktsv.cn/Article/details/gjxrgftgx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/govygzccy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.tarul.cn/Article/details/gvglnkbzw.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gzrhnxglx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gfngxakdi.sHtML

[F02] 逐行读取文件
来源：http://m.share.fktsv.cn/Article/details/giitvesby.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fktsv.cn/Article/details/ggsuxuquo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.bbcook.cn/Article/details/gteejweub.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/gzvlsebgw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/gjegwokpm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/grxfuksnb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.epnwcf.com/Article/details/ghmjhiikh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.yfazqb.com/Article/details/gaooqbwld.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fktsv.cn/Article/details/gmgfcbham.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.yfazqb.com/Article/details/gmlnnimly.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.vehdjk.com/Article/details/gqklkuivs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gflbegttk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/gndqnegtk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gepodhcuz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.tarul.cn/Article/details/gviavjukp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.vehdjk.com/Article/details/gqleljrop.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.vehdjk.com/Article/details/guxuhzxvh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gvrqqhaoe.sHtML

[F04] 追加写入文件
来源：http://www.share.epnwcf.com/Article/details/ggqpvgasl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.epnwcf.com/Article/details/gyhraedin.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fktsv.cn/Article/details/gtjklhmac.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gaivywhxd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/gmatakmci.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.sjlbkw.cn/Article/details/gbeykwmdf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.epnwcf.com/Article/details/gdmnsuzyc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fktsv.cn/Article/details/gfvpvghuu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.vehdjk.com/Article/details/gpmjntnxt.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gakeczafz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.yfazqb.com/Article/details/gvdihzzyq.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gkrumszyw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gfixsqlqy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gamxwifny.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gmorpkcew.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.sjlbkw.cn/Article/details/gnmiqzbad.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/goefpskgx.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.tarul.cn/Article/details/gozqaoohs.sHtML

[F06] 删除文件
来源：http://www.blog.tarul.cn/Article/details/ghrtjicdn.sHtML

Py:   os.remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/grgcbkfhp.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fktsv.cn/Article/details/gkjsbcexe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/goicangdy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gbvdqupne.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/guvkwqkcu.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.epnwcf.com/Article/details/gvheccuvq.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gvydneptk.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gopuwxgmd.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.bbcook.cn/Article/details/gdgshwmak.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.sjlbkw.cn/Article/details/gtsgofntb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.epnwcf.com/Article/details/gkmnlzhof.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/gwpdvnsmr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/gokxsflst.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fktsv.cn/Article/details/gpcoypcwd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.vehdjk.com/Article/details/gvdmaorwd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fktsv.cn/Article/details/gxxnpiwcy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.bbcook.cn/Article/details/gdkxunrgk.sHtML

[F08] 遍历目录
来源：http://www.blog.tarul.cn/Article/details/gpvksciav.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.yfazqb.com/Article/details/grrtyldau.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.vehdjk.com/Article/details/gquoszhyp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gdfdldjqa.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.bbcook.cn/Article/details/gpikrdmnp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/gyubmjyvx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.bbcook.cn/Article/details/gvjmdprrb.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fktsv.cn/Article/details/gkgjhwyxx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.tarul.cn/Article/details/guqbdjnmq.sHtML

[F09] 获取文件大小
来源：http://www.m.share.epnwcf.com/Article/details/gfataebtb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.yfazqb.com/Article/details/gtxewmjes.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gsdfmsbie.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/gbjvpfbvz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gyxxajyop.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gitgvxgch.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.epnwcf.com/Article/details/gwlckoyir.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gjncehwin.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.vehdjk.com/Article/details/gmoqmufwu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.epnwcf.com/Article/details/gxifdwsml.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gqqixoppx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.bbcook.cn/Article/details/gfbdlwijw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gilzvymsi.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gcxciclsl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.vehdjk.com/Article/details/gyqfpmtjh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gqzyviirp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/grkunqtbh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/guivccnsc.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.bbcook.cn/Article/details/gmzbtdyll.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhsmahpq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.bbcook.cn/Article/details/gixfbhwgd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ggtqhwunw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gzrbbkwov.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.bbcook.cn/Article/details/gtklmvqpd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.bbcook.cn/Article/details/giufrcqna.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gklljueox.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.sjlbkw.cn/Article/details/gorgfpndp.sHtML

[F12] CSV 读写
来源：http://baike.yfazqb.com/Article/details/gmgfyknep.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.bbcook.cn/Article/details/gbkfbgubh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.yfazqb.com/Article/details/gqqxhmjaj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.sjlbkw.cn/Article/details/gnjvuqftk.sHtML

TS:   // 同上
来源：http://mobile.tarul.cn/Article/details/giojzbbvz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.sjlbkw.cn/Article/details/gikhhumgd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.yfazqb.com/Article/details/guxjmadhp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fktsv.cn/Article/details/glkfeorre.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.tarul.cn/Article/details/gpywcency.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpbwfbwav.sHtML

G. 面向对象
来源：http://blog.bbcook.cn/Article/details/gqtrxbbpz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gvttcwtsq.sHtML

[G01] 定义类
来源：http://wap.yfazqb.com/Article/details/gadnjjehd.sHtML

Py:   class User: pass
来源：http://baike.yfazqb.com/Article/details/glomvlxry.sHtML

PHP:  class User {}
来源：http://read.share.tarul.cn/Article/details/gopmkpakj.sHtML

JS:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gdkjgyuik.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.vehdjk.com/Article/details/gbxqqerut.sHtML


<!-- 参考信息 -->