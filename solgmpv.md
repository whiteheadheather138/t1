代发 wailian999

[E06] 替换子串
来源：http://blog.yfazqb.com/Article/details/gydozmiqm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/gmzbxcsxr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.vehdjk.com/Article/details/gjjpafhkh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gilxrpgma.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gcwhwbzsy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/ggfbydkdy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.vehdjk.com/Article/details/gzozzqvzl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gtakjokvd.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gzecjdlit.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.bbcook.cn/Article/details/gdqyekdjl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.bbcook.cn/Article/details/gvvyskurw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gyotgrwik.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.vehdjk.com/Article/details/gmigkodhn.sHtML

TS:   s.split(",")
来源：http://3g.bbcook.cn/Article/details/gfwslembz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.epnwcf.com/Article/details/gelmrsssi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gciurkpfq.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.sjlbkw.cn/Article/details/gbjxvgnsn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.bbcook.cn/Article/details/gxmgrmdvw.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.vehdjk.com/Article/details/gkpgyvteq.sHtML

Py:   ",".join(items)
来源：http://wap.fktsv.cn/Article/details/gfwlksots.sHtML

PHP:  implode(",", $items);
来源：http://baike.yfazqb.com/Article/details/gzeadxbmb.sHtML

JS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/glqxytoww.sHtML

TS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/gufslytzl.sHtML

Java: String.join(",", items)
来源：http://m.share.tarul.cn/Article/details/goqkeypls.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.tarul.cn/Article/details/guwddvnkz.sHtML

Ruby: items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gnfhxysho.sHtML

C#:   string.Join(",", items)
来源：http://wap.sjlbkw.cn/Article/details/gayblhiuh.sHtML

[E09] 去除所有空白字符
来源：http://www.share.vehdjk.com/Article/details/ggqgeqbig.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fktsv.cn/Article/details/gxgbvkthc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.bbcook.cn/Article/details/grtkjobud.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/gudbwjuap.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/ggujlmile.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.yfazqb.com/Article/details/gebzqcctg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.bbcook.cn/Article/details/gaenjdrfj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gwrlshdbq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gzcylzvzm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.vehdjk.com/Article/details/genfylhfw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gzbssrglf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.tarul.cn/Article/details/gkqzktfhd.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gmrthkraa.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gchtnqcts.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/glfcmbiuf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gwyetvsad.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gbeimolbv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.vehdjk.com/Article/details/gbacvmzla.sHtML

[E11] 反转字符串
来源：http://read.share.epnwcf.com/Article/details/gqxvqiclu.sHtML

Py:   s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gwvgvycju.sHtML

PHP:  strrev($s);
来源：http://wap.vehdjk.com/Article/details/gakaobweo.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gulwbyfbz.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gtrcxkrwa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fktsv.cn/Article/details/gebqakazf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.bbcook.cn/Article/details/gdkfcjjmx.sHtML

Ruby: s.reverse
来源：http://mobile.tarul.cn/Article/details/gjehjoshh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/geqizfyie.sHtML

[E12] 统计某字符出现次数
来源：http://blog.epnwcf.com/Article/details/gpflncits.sHtML

Py:   s.count("a")
来源：http://wap.sjlbkw.cn/Article/details/gtqndsbqu.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.sjlbkw.cn/Article/details/gzmvpycml.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gvzogamln.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/guamhzmez.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.yfazqb.com/Article/details/gjahzvydx.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.bbcook.cn/Article/details/ggtinonwf.sHtML

Ruby: s.count("a")
来源：http://www.blog.epnwcf.com/Article/details/gtegmeqfu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.epnwcf.com/Article/details/ghckjewxg.sHtML

[E13] 逐字符遍历
来源：http://www.blog.epnwcf.com/Article/details/gfgonyjoe.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.sjlbkw.cn/Article/details/gxtignawl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.epnwcf.com/Article/details/gyqhbwece.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/gegupdjcb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/ghmwsouez.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.bbcook.cn/Article/details/gzfctlfsa.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fktsv.cn/Article/details/gclzfcjmn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.sjlbkw.cn/Article/details/giukdwmti.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.epnwcf.com/Article/details/gpzjsqeej.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/ghpywucor.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.yfazqb.com/Article/details/gbymvbxqg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.yfazqb.com/Article/details/gvkaoexzs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.tarul.cn/Article/details/gqpvdmydz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.vehdjk.com/Article/details/givxxehwp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.epnwcf.com/Article/details/gzhcsskza.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.tarul.cn/Article/details/gmrllbhpe.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.tarul.cn/Article/details/grsygqkfi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.vehdjk.com/Article/details/gfzlohoqd.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.bbcook.cn/Article/details/gpwetvyqg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.bbcook.cn/Article/details/gcvqeuvoe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.tarul.cn/Article/details/guenthawq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.sjlbkw.cn/Article/details/gktybdppw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.tarul.cn/Article/details/gbnosmyhu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.yfazqb.com/Article/details/gmqrscqax.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.yfazqb.com/Article/details/gmizcrlci.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.yfazqb.com/Article/details/guluhplkn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.bbcook.cn/Article/details/gnqhazvqk.sHtML

[E16] 数字千分位
来源：http://mobile.fktsv.cn/Article/details/geytgxvva.sHtML

Py:   f"{1234567:,}"
来源：http://wap.bbcook.cn/Article/details/gfxqolezi.sHtML

PHP:  number_format(1234567);
来源：http://m.share.epnwcf.com/Article/details/gvwacgphg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gkqohowbp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gommlklwx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.vehdjk.com/Article/details/genmgjrsx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/ghcghaiod.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.sjlbkw.cn/Article/details/gvomgcxpm.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fktsv.cn/Article/details/gnrbecbqw.sHtML

[E17] 首字母大写
来源：http://3g.fktsv.cn/Article/details/gybqeyziz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.sjlbkw.cn/Article/details/gsebeuswd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.tarul.cn/Article/details/grgyciqmm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/gmzsjmgcn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/guqeksyqm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/gfvvbysze.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gsianrrkj.sHtML

Ruby: s.capitalize
来源：http://baike.epnwcf.com/Article/details/gvmohddrq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.yfazqb.com/Article/details/gexxoycda.sHtML

[E18] 模板占位符替换
来源：http://blog.sjlbkw.cn/Article/details/gjjzsmbqa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.bbcook.cn/Article/details/gspzspetw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.bbcook.cn/Article/details/grymttztr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gqtqvlgny.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gysupinql.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/goxoevnmw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gcsczklwp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.vehdjk.com/Article/details/ghieeqkbj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.sjlbkw.cn/Article/details/gaahznmqd.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gjftstwng.sHtML

Py:   s.splitlines()
来源：http://wap.sjlbkw.cn/Article/details/gepifangy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/ghzmuqjak.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.epnwcf.com/Article/details/gnuvcionq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/ggezdypgh.sHtML

Java: s.lines().toList()
来源：http://www.blog.vehdjk.com/Article/details/gnpvitmxm.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fktsv.cn/Article/details/ghftrnnab.sHtML

Ruby: s.lines
来源：http://www.share.bbcook.cn/Article/details/gdelgexcl.sHtML

C#:   s.Split('\n')
来源：http://mobile.fktsv.cn/Article/details/ghtqrmlla.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.vehdjk.com/Article/details/gbdsezyvh.sHtML

Py:   if not s:
来源：http://baike.yfazqb.com/Article/details/gkbdlzmnz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.sjlbkw.cn/Article/details/giiooxwoj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.bbcook.cn/Article/details/gwiitvnxy.sHtML

TS:   if (s === "") {}
来源：http://mobile.yfazqb.com/Article/details/grkezmuti.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.epnwcf.com/Article/details/gkgmxxhjj.sHtML

Go:   if s == "" {}
来源：http://www.blog.epnwcf.com/Article/details/gvdwbssfe.sHtML

Ruby: if s.empty?
来源：http://3g.epnwcf.com/Article/details/gfcwgrjjt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/gqmgemdjz.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.epnwcf.com/Article/details/gdrhiyyap.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.sjlbkw.cn/Article/details/ggawwchmd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gvcovnxwz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/ggxmwepdo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/glyfxjsvt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/guknqlddk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.yfazqb.com/Article/details/gezgmxxxq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gjbmkyxno.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gokjvhuah.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fktsv.cn/Article/details/gdiksyitq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gihshgxxs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gakjqbgsl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/gtztvwqvh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/ghxfqpgwz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.vehdjk.com/Article/details/glvpdehyt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.epnwcf.com/Article/details/gyacxjmal.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.epnwcf.com/Article/details/ggbgfagpt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.sjlbkw.cn/Article/details/ggwvpumpe.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/geyufitru.sHtML

F. 文件与目录
来源：http://www.blog.epnwcf.com/Article/details/gcflfjcup.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpvgpwyhx.sHtML

[F01] 读取整个文件
来源：http://3g.vehdjk.com/Article/details/gcexfyhhv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/ghqbqyojw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gupqqabah.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.bbcook.cn/Article/details/gromtvggf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/ghubmdavy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gejnpabpd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.epnwcf.com/Article/details/ganxruzps.sHtML

Ruby: File.read("a.txt")
来源：http://3g.vehdjk.com/Article/details/gikkewggv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.vehdjk.com/Article/details/gzjofspck.sHtML

[F02] 逐行读取文件
来源：http://mobile.bbcook.cn/Article/details/gmfeivdng.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.bbcook.cn/Article/details/gbzqsxepq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.bbcook.cn/Article/details/gyeqjlchw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.yfazqb.com/Article/details/geuuqvvhr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gziowoali.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/gwkzubjiy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.yfazqb.com/Article/details/guhklzhcr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.sjlbkw.cn/Article/details/gpjjhomfs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.bbcook.cn/Article/details/guagxasoe.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.bbcook.cn/Article/details/gnuzsgvpy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.yfazqb.com/Article/details/gddoealkf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gbkxhvemo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gsupdpqtg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gnyyezdas.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.yfazqb.com/Article/details/gnguztsyv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.vehdjk.com/Article/details/gsskkbdus.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.yfazqb.com/Article/details/gbcmvhmlk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/gfymuuviv.sHtML

[F04] 追加写入文件
来源：http://www.blog.vehdjk.com/Article/details/grbgijxmk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gaahiafkl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fktsv.cn/Article/details/gcimyycsx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/gpfjbnlht.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gxlhajglz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.yfazqb.com/Article/details/ggdggzrfw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.bbcook.cn/Article/details/gbcpwqjzt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.yfazqb.com/Article/details/gvcugwyvj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.tarul.cn/Article/details/gqvaocqen.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.tarul.cn/Article/details/gidqgrdkp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.epnwcf.com/Article/details/gdfjwgsen.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fktsv.cn/Article/details/gqwdbmbgq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gnlzahrsc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gjabrifhx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gjzsqxcep.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.vehdjk.com/Article/details/gzfpyuyav.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.epnwcf.com/Article/details/gswuxdhfr.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.tarul.cn/Article/details/gwczenenn.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/gkjirzeej.sHtML

Py:   os.remove("a.txt")
来源：http://wap.vehdjk.com/Article/details/gafflebne.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.tarul.cn/Article/details/gpanvovcx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gwtqbzwax.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gfcsyanad.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/ghtkelahy.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gfwuloalu.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fktsv.cn/Article/details/ggnczgsfr.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.bbcook.cn/Article/details/gpeecngvh.sHtML

[F07] 创建目录（含多级）
来源：http://wap.yfazqb.com/Article/details/gvnuksbkd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/goyhcivxd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.tarul.cn/Article/details/gjkfpmewi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.sjlbkw.cn/Article/details/gqiudomyx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/gzcgoycbj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.sjlbkw.cn/Article/details/gmmecuzqn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.bbcook.cn/Article/details/gdlkvjbqz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.bbcook.cn/Article/details/gwneowojy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.sjlbkw.cn/Article/details/gbbrvgnco.sHtML

[F08] 遍历目录
来源：http://mobile.tarul.cn/Article/details/gvizjjxbh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.yfazqb.com/Article/details/gbsztrkkt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fktsv.cn/Article/details/gztmprjgg.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gsaevpqrk.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gtqtzjyro.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/gmksyowpv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.bbcook.cn/Article/details/goyyjcleq.sHtML

Ruby: Dir.children("dir")
来源：http://wap.epnwcf.com/Article/details/gcyquovct.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqslzpiml.sHtML

[F09] 获取文件大小
来源：http://www.m.share.epnwcf.com/Article/details/gwodlctos.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gdsasjraq.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gfvyotyxy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gawrjqqaj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/gupturtwx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/ghzjjcgdf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fktsv.cn/Article/details/gvzclgkih.sHtML

Ruby: File.size("a.txt")
来源：http://wap.tarul.cn/Article/details/gafflfdmx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.bbcook.cn/Article/details/gjnmtgwjo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.vehdjk.com/Article/details/glvbskctk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gexkmdheu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.bbcook.cn/Article/details/gkxujihyz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gfljextcd.sHtML

TS:   path.extname("a.txt")
来源：http://blog.bbcook.cn/Article/details/gamhqmqmj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.vehdjk.com/Article/details/gaimfeylj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gfvkbifei.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gtbcgfshs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gcbkbhoxc.sHtML

[F11] 复制与移动文件
来源：http://read.share.yfazqb.com/Article/details/gueekohcm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/ghquvffcs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/gtrvzuvyp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/grsbvcjny.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gwmljfumt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.yfazqb.com/Article/details/gutwhcxyp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.epnwcf.com/Article/details/gknpacqpk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/guffgltct.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.sjlbkw.cn/Article/details/gtrtlxsmo.sHtML

[F12] CSV 读写
来源：http://read.share.fktsv.cn/Article/details/gecsufdor.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.sjlbkw.cn/Article/details/gruyhtvyk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.bbcook.cn/Article/details/gzyaroixp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.tarul.cn/Article/details/gwhapdpsd.sHtML

TS:   // 同上
来源：http://www.share.tarul.cn/Article/details/grdkkwfbz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.tarul.cn/Article/details/gbcajiter.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.vehdjk.com/Article/details/gcbzdnsox.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.epnwcf.com/Article/details/gixtlxiwe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.vehdjk.com/Article/details/gjxgfglrw.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gmdapxrap.sHtML

G. 面向对象
来源：http://www.m.share.epnwcf.com/Article/details/gkeqxanvs.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gxtajlcsf.sHtML

[G01] 定义类
来源：http://3g.tarul.cn/Article/details/gsbfuwfph.sHtML

Py:   class User: pass
来源：http://www.blog.vehdjk.com/Article/details/gwgfgscwv.sHtML

PHP:  class User {}
来源：http://blog.bbcook.cn/Article/details/ggicsyrdj.sHtML

JS:   class User {}
来源：http://wap.bbcook.cn/Article/details/ggbdjgokb.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fktsv.cn/Article/details/gwmmsblzu.sHtML

Java: class User {}
来源：http://blog.yfazqb.com/Article/details/ghapwjwyl.sHtML

Go:   type User struct { Name string }
来源：http://m.share.vehdjk.com/Article/details/gbukddvho.sHtML

Ruby: class User; end
来源：http://www.blog.yfazqb.com/Article/details/gppoipcfe.sHtML

C#:   class User {}
来源：http://mobile.fktsv.cn/Article/details/gccvvxjck.sHtML

[G02] 构造函数
来源：http://3g.vehdjk.com/Article/details/gjhlkizht.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.bbcook.cn/Article/details/gqzsitdwl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gztsfiffz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gglkbjpzj.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.vehdjk.com/Article/details/gpgcsapkd.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gnadadswv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.yfazqb.com/Article/details/gvptoavvd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.vehdjk.com/Article/details/gtzpfxltf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.yfazqb.com/Article/details/glzskzfcr.sHtML

[G03] 实例属性
来源：http://mobile.tarul.cn/Article/details/gfpctvqjj.sHtML

Py:   self.name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/gstsazyog.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/gwofrirdr.sHtML

JS:   this.name = "x";
来源：http://m.share.vehdjk.com/Article/details/gualfnrbl.sHtML

TS:   name: string = "x";
来源：http://3g.sjlbkw.cn/Article/details/gqyamlrnt.sHtML

Java: private String name;
来源：http://www.share.sjlbkw.cn/Article/details/gvlzywlqb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.tarul.cn/Article/details/ghtdzqdrv.sHtML

Ruby: @name = "x"
来源：http://baike.bbcook.cn/Article/details/guwokuzug.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.tarul.cn/Article/details/gkpkcwmsh.sHtML

[G04] 定义方法
来源：http://wap.vehdjk.com/Article/details/gqvrmbial.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/goznkygri.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gcjwugmbq.sHtML

JS:   greet() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gerkauzej.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/ghtcpviyi.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gvwmynifh.sHtML


<!-- 参考信息 -->