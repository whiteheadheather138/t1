代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/ggzeeebxp.sHtML

TS:   s.slice(1, 4)
来源：http://blog.yfazqb.com/Article/details/gorupxqvq.sHtML

Java: s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gqpqtyujx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fktsv.cn/Article/details/gvbjqppis.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.epnwcf.com/Article/details/gewlunufj.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fktsv.cn/Article/details/gzxxkqduc.sHtML

[E04] 查找子串位置
来源：http://www.blog.vehdjk.com/Article/details/gmssjktgb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.vehdjk.com/Article/details/gzcwumhvc.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.epnwcf.com/Article/details/gjmewjfgq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.epnwcf.com/Article/details/gtabdkdyy.sHtML

TS:   s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/gjfpylmbx.sHtML

Java: s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/gvgnwhzfr.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.sjlbkw.cn/Article/details/ggcxiolqk.sHtML

Ruby: s.index("x")
来源：http://www.share.yfazqb.com/Article/details/gverpztzo.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gzrlfstol.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.epnwcf.com/Article/details/ginttfruf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fktsv.cn/Article/details/gehhgezyy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.tarul.cn/Article/details/gdtkzxtqd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gcqowkspr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fktsv.cn/Article/details/gotnqddiz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gncnmscfb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.epnwcf.com/Article/details/gzizrbqed.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.sjlbkw.cn/Article/details/gauqhhhep.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/ggqgrifml.sHtML

[E06] 替换子串
来源：http://m.share.tarul.cn/Article/details/gtjnotkyd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gzkfyorck.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.yfazqb.com/Article/details/gazlhqcpk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gikdiznks.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gupzvadlh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/goczkndan.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fktsv.cn/Article/details/gldwawfvh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.epnwcf.com/Article/details/gscdrxnfu.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gaetdhcvr.sHtML

[E07] 按分隔符拆分
来源：http://mobile.vehdjk.com/Article/details/gqjvcpyux.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.epnwcf.com/Article/details/glreutxel.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fktsv.cn/Article/details/gcuwiebtb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fktsv.cn/Article/details/gphytmbyk.sHtML

TS:   s.split(",")
来源：http://read.share.sjlbkw.cn/Article/details/gnhcgxzja.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fktsv.cn/Article/details/gwmkcxopz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fktsv.cn/Article/details/gefuapigg.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.vehdjk.com/Article/details/guvjctovi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.sjlbkw.cn/Article/details/gxztqwidi.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.sjlbkw.cn/Article/details/gusljxkci.sHtML

Py:   ",".join(items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqukglisu.sHtML

PHP:  implode(",", $items);
来源：http://baike.yfazqb.com/Article/details/gyzowfomj.sHtML

JS:   items.join(",")
来源：http://www.share.epnwcf.com/Article/details/guimiknzx.sHtML

TS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gwrzyjzzi.sHtML

Java: String.join(",", items)
来源：http://read.share.yfazqb.com/Article/details/gbcshthqa.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.yfazqb.com/Article/details/gmywczbiw.sHtML

Ruby: items.join(",")
来源：http://baike.epnwcf.com/Article/details/gakkzidyh.sHtML

C#:   string.Join(",", items)
来源：http://3g.yfazqb.com/Article/details/gzvbuvmxp.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fktsv.cn/Article/details/gswykswho.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.vehdjk.com/Article/details/gvoopsfnu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.tarul.cn/Article/details/gghgsbiro.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/giwkzsqfm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.tarul.cn/Article/details/guruumiws.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.vehdjk.com/Article/details/gohvjfhde.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.bbcook.cn/Article/details/gmevdoscb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.vehdjk.com/Article/details/gctiezkdo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.epnwcf.com/Article/details/gkikyadcz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.epnwcf.com/Article/details/geigrtsvy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.epnwcf.com/Article/details/gvuyvxkwu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.sjlbkw.cn/Article/details/gguqnifpo.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gjddephhq.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fktsv.cn/Article/details/gqnqvffsw.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/geqvoeale.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gixueaezw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gmpbjgpxq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.tarul.cn/Article/details/gktkvmqmw.sHtML

[E11] 反转字符串
来源：http://m.share.fktsv.cn/Article/details/geovlptow.sHtML

Py:   s[::-1]
来源：http://wap.fktsv.cn/Article/details/gmqskvcjo.sHtML

PHP:  strrev($s);
来源：http://blog.fktsv.cn/Article/details/gxawnqpme.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gjfdcsdej.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gijitedgw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fktsv.cn/Article/details/gqzdpwsqk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.epnwcf.com/Article/details/gufmhbhzg.sHtML

Ruby: s.reverse
来源：http://baike.tarul.cn/Article/details/gvcamcpoi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gmgerafeu.sHtML

[E12] 统计某字符出现次数
来源：http://blog.vehdjk.com/Article/details/gzxcjdukx.sHtML

Py:   s.count("a")
来源：http://www.m.share.fktsv.cn/Article/details/getyvcnjk.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.tarul.cn/Article/details/giiqruvxj.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/gyixznama.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gbmqpqsep.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.epnwcf.com/Article/details/gytgdvjpm.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fktsv.cn/Article/details/ggqptxbhc.sHtML

Ruby: s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gqgyzradj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.yfazqb.com/Article/details/gcvqfqqyj.sHtML

[E13] 逐字符遍历
来源：http://read.share.fktsv.cn/Article/details/ggjnkjeun.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fktsv.cn/Article/details/gwtfpljxt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.yfazqb.com/Article/details/gruwlprzz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gjtiuwyoq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/gdogneveo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.tarul.cn/Article/details/gabwajcob.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fktsv.cn/Article/details/ggygcryad.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.yfazqb.com/Article/details/gnlajjkuz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.yfazqb.com/Article/details/gjqloozgj.sHtML

[E14] URL 编码与 Base64
来源：http://blog.vehdjk.com/Article/details/gxyqgyrhi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.bbcook.cn/Article/details/gzrlpfzjq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.yfazqb.com/Article/details/griuepbkj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.vehdjk.com/Article/details/gccbgerld.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.yfazqb.com/Article/details/gbeikedgs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.vehdjk.com/Article/details/gjjdltlxx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.yfazqb.com/Article/details/gsxhecrnh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.sjlbkw.cn/Article/details/gzvcivemc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fktsv.cn/Article/details/gweamrujv.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fktsv.cn/Article/details/gocdscqpi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.sjlbkw.cn/Article/details/gxkvtosui.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.vehdjk.com/Article/details/gejtkajfu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.tarul.cn/Article/details/gkadnbvjm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.vehdjk.com/Article/details/gtstlqhdd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.yfazqb.com/Article/details/gtetkkzcm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.tarul.cn/Article/details/gfpofmppu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.tarul.cn/Article/details/gdsupwdau.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.yfazqb.com/Article/details/gzzzmjphm.sHtML

[E16] 数字千分位
来源：http://blog.sjlbkw.cn/Article/details/gfxyofqfp.sHtML

Py:   f"{1234567:,}"
来源：http://wap.vehdjk.com/Article/details/gpezjwvod.sHtML

PHP:  number_format(1234567);
来源：http://wap.tarul.cn/Article/details/gvbxfvxdb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gobdvbgal.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.sjlbkw.cn/Article/details/gpmfarxum.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.yfazqb.com/Article/details/giqkzndbu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.sjlbkw.cn/Article/details/gyhspsbyz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.epnwcf.com/Article/details/gzogslrwh.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.bbcook.cn/Article/details/gsbdwahzl.sHtML

[E17] 首字母大写
来源：http://www.blog.vehdjk.com/Article/details/getgmqimr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.bbcook.cn/Article/details/ginrewsjl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.tarul.cn/Article/details/gcsciyhmy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.vehdjk.com/Article/details/golnzawcd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/gnuhonikb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.tarul.cn/Article/details/gricyqtcd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.vehdjk.com/Article/details/ghxsrmsyg.sHtML

Ruby: s.capitalize
来源：http://www.share.fktsv.cn/Article/details/gnohafunv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.bbcook.cn/Article/details/gfwrwarul.sHtML

[E18] 模板占位符替换
来源：http://www.share.sjlbkw.cn/Article/details/gfcryhmnu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.yfazqb.com/Article/details/gfgtgflbb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.yfazqb.com/Article/details/gbjuuggvj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/ghcssqsit.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gidudezfs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gobqtsiva.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.bbcook.cn/Article/details/gvktykjcy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.vehdjk.com/Article/details/gwqvldnju.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.bbcook.cn/Article/details/gmgedejfw.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.bbcook.cn/Article/details/ghokjvphf.sHtML

Py:   s.splitlines()
来源：http://www.m.share.epnwcf.com/Article/details/gbogbbxva.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.vehdjk.com/Article/details/gjszguyla.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/gloaftynt.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gkrdtnthf.sHtML

Java: s.lines().toList()
来源：http://www.blog.epnwcf.com/Article/details/gbdtipzwi.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.vehdjk.com/Article/details/gujfmwtod.sHtML

Ruby: s.lines
来源：http://www.m.share.tarul.cn/Article/details/ggvuwwspt.sHtML

C#:   s.Split('\n')
来源：http://wap.fktsv.cn/Article/details/gsxikdiws.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/gmpcvjjid.sHtML

Py:   if not s:
来源：http://www.share.fktsv.cn/Article/details/gxgpielgc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.bbcook.cn/Article/details/gimkqgwvj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.bbcook.cn/Article/details/gsfpoleft.sHtML

TS:   if (s === "") {}
来源：http://blog.bbcook.cn/Article/details/grbzmmlbz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/gwzeylouh.sHtML

Go:   if s == "" {}
来源：http://www.m.share.yfazqb.com/Article/details/grxceyfkc.sHtML

Ruby: if s.empty?
来源：http://mobile.fktsv.cn/Article/details/gddjkrkti.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.tarul.cn/Article/details/gmhqhcrdz.sHtML

[E21] 超长截断加省略号
来源：http://3g.yfazqb.com/Article/details/gcclpvtvr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/glbakhbjj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gnjgrukrb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gtjnvlkvj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gfdupjyqp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gaudgdfrt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.yfazqb.com/Article/details/gtlnrzvlu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gqgbsqent.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjceajnc.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.epnwcf.com/Article/details/ghbgjfruc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.tarul.cn/Article/details/gsxnogblb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gpvhujpzz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gjnyvslqv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gdlaefkrs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.epnwcf.com/Article/details/gbstooshl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fktsv.cn/Article/details/guuahppcw.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.yfazqb.com/Article/details/gzrkrkdnf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.tarul.cn/Article/details/gdwfnrqdp.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gwnmolvzt.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/gpbcuxved.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxrakpidv.sHtML

[F01] 读取整个文件
来源：http://mobile.yfazqb.com/Article/details/gweglhptv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.yfazqb.com/Article/details/ghetssfsu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gxgkxkoye.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.vehdjk.com/Article/details/gvbsdhmcs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.tarul.cn/Article/details/guqucltxc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gczxpftze.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.yfazqb.com/Article/details/goosqdkbi.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gsjhywpjz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gehnpwgfm.sHtML

[F02] 逐行读取文件
来源：http://3g.tarul.cn/Article/details/gyhndafxp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.sjlbkw.cn/Article/details/gigerlooi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.sjlbkw.cn/Article/details/gsapdmfib.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gyfzstipi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gittsxwxk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gnxfdjwtr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.epnwcf.com/Article/details/gudvqcdii.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.sjlbkw.cn/Article/details/guqiwlybw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.bbcook.cn/Article/details/gbknexblo.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.epnwcf.com/Article/details/gxfrnvzaa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.vehdjk.com/Article/details/gqvtlxanv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gjispwdlf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gfzjurhuw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/girbikiow.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.epnwcf.com/Article/details/grlqjjfrn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.bbcook.cn/Article/details/gxhymbfmn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.bbcook.cn/Article/details/gtszgzbqn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gqeidgyzz.sHtML

[F04] 追加写入文件
来源：http://wap.sjlbkw.cn/Article/details/gavsuyfhb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.vehdjk.com/Article/details/grydbfslr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.epnwcf.com/Article/details/gpofixttu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/gjvjrzool.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrlcvjug.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.tarul.cn/Article/details/gsxtdnthx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.yfazqb.com/Article/details/gzhompayg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.bbcook.cn/Article/details/gbpqpygmt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.sjlbkw.cn/Article/details/gjykzynta.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.tarul.cn/Article/details/giaxutbqb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fktsv.cn/Article/details/glkufykyd.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.bbcook.cn/Article/details/gjcvbngiw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gtiaoguyp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/geoboyqux.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/ggkxooooy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.sjlbkw.cn/Article/details/gqpsfpsrb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gxnhqsngs.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.tarul.cn/Article/details/glkprxohe.sHtML

[F06] 删除文件
来源：http://www.m.share.yfazqb.com/Article/details/gmxndpwql.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gmfhxgqho.sHtML

PHP:  unlink("a.txt");
来源：http://baike.epnwcf.com/Article/details/gtlsmwtav.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gdmullpuz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/giwxchybd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gafwvruxq.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gfczkvshl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gpdocefyu.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gduvezlky.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fktsv.cn/Article/details/gxoxejvle.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.bbcook.cn/Article/details/gpvvsxjps.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.yfazqb.com/Article/details/gtgdmehfo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/gspguyquh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/gdukkxohz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.bbcook.cn/Article/details/gkmihqcqk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.epnwcf.com/Article/details/gtjgzbhug.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.vehdjk.com/Article/details/gygamfwqh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.yfazqb.com/Article/details/gasopilvi.sHtML

[F08] 遍历目录
来源：http://read.share.fktsv.cn/Article/details/gfflwezmk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.bbcook.cn/Article/details/gktafrigx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fktsv.cn/Article/details/ggulxieop.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gtdbmefwb.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/gkeputlmx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gxiumbzgs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fktsv.cn/Article/details/gxtoxlfvy.sHtML

Ruby: Dir.children("dir")
来源：http://blog.bbcook.cn/Article/details/gwrnhspvi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.bbcook.cn/Article/details/genaxyrlp.sHtML

[F09] 获取文件大小
来源：http://www.share.vehdjk.com/Article/details/gvmmfacgv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fktsv.cn/Article/details/gsrsegbig.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gndnsdppa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gxeqwcrjl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/getxhptba.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/giewsdqpf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.tarul.cn/Article/details/gftpqgdky.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gjxspnmfw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.epnwcf.com/Article/details/gnmaclykj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.bbcook.cn/Article/details/gytwtvzzz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gsqcxaage.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.epnwcf.com/Article/details/ghqaevtjg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gogchrozd.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fktsv.cn/Article/details/ggskhnjtj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.vehdjk.com/Article/details/ghgimdjyy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/grjfughnm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdyghcmv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gzsfcbort.sHtML

[F11] 复制与移动文件
来源：http://3g.vehdjk.com/Article/details/gtjjzouyr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/ggnuvqdbn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fktsv.cn/Article/details/gcvymnmap.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gcsvqxnpg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gwgkikbxm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gefujhref.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.vehdjk.com/Article/details/gimfnfeso.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gjlcfxame.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.bbcook.cn/Article/details/gyqpyojie.sHtML

[F12] CSV 读写
来源：http://3g.vehdjk.com/Article/details/gcocqhvzc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.vehdjk.com/Article/details/gebkifimk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.vehdjk.com/Article/details/gizxuavhp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyoyguce.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/giwfrcdsf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.bbcook.cn/Article/details/gzleadnzp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.bbcook.cn/Article/details/gzsyfmadd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fktsv.cn/Article/details/geeoyhqhc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.sjlbkw.cn/Article/details/gwylzgckl.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gyoagbfjw.sHtML

G. 面向对象
来源：http://mobile.bbcook.cn/Article/details/gwgcfmhkc.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gaklvxhuh.sHtML

[G01] 定义类
来源：http://www.share.fktsv.cn/Article/details/gbifwosfh.sHtML

Py:   class User: pass
来源：http://www.m.share.vehdjk.com/Article/details/goxhbvcaf.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/gixapmxcr.sHtML

JS:   class User {}
来源：http://baike.epnwcf.com/Article/details/gxcapgnpy.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.vehdjk.com/Article/details/ggskrdbxm.sHtML

Java: class User {}
来源：http://mobile.tarul.cn/Article/details/gouroyyqm.sHtML

Go:   type User struct { Name string }
来源：http://baike.sjlbkw.cn/Article/details/gyvyyatrv.sHtML

Ruby: class User; end
来源：http://blog.sjlbkw.cn/Article/details/gmzqmldep.sHtML

C#:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gwudptizb.sHtML


<!-- 参考信息 -->