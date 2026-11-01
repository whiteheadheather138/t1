代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.vehdjk.com/Article/details/gkybikudj.sHtML

[E03] 截取子串
来源：http://3g.fktsv.cn/Article/details/grzbcrspx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.bbcook.cn/Article/details/gzyzkovdm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gxogblqkk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gpdbihmcp.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gbufhdmka.sHtML

Java: s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gseaouopd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fktsv.cn/Article/details/gtawqeezg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.tarul.cn/Article/details/grmfulyhw.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.bbcook.cn/Article/details/gvzadjcnw.sHtML

[E04] 查找子串位置
来源：http://www.blog.vehdjk.com/Article/details/gdvpoohvb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fktsv.cn/Article/details/gruypazpz.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.sjlbkw.cn/Article/details/grjdywuid.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.bbcook.cn/Article/details/gcsaapwru.sHtML

TS:   s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/gomwggcvx.sHtML

Java: s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gzzbdpgdj.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.epnwcf.com/Article/details/gvikzexst.sHtML

Ruby: s.index("x")
来源：http://wap.sjlbkw.cn/Article/details/gllvcitsk.sHtML

C#:   s.IndexOf("x")
来源：http://3g.vehdjk.com/Article/details/gnaylapsb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.yfazqb.com/Article/details/gjuobwihl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.epnwcf.com/Article/details/gqyptcebe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.yfazqb.com/Article/details/gcycdokpj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/guibczfbq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.bbcook.cn/Article/details/gkwiyjujx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gteypxoka.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.vehdjk.com/Article/details/gtyzsokpw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.epnwcf.com/Article/details/ggbcijqki.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gmbrxpljo.sHtML

[E06] 替换子串
来源：http://wap.yfazqb.com/Article/details/gybfkkzck.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gjccixnve.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.epnwcf.com/Article/details/gqnaymlkg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gyprljhha.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gvxrzypik.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/glgkmroas.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/gnnxmnbly.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gtktllmzw.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gdiiqtsvy.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.tarul.cn/Article/details/gwvazlgyp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.vehdjk.com/Article/details/ghwgaxrha.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fktsv.cn/Article/details/gqwkwvwqr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fktsv.cn/Article/details/geuxqzyvw.sHtML

TS:   s.split(",")
来源：http://read.share.sjlbkw.cn/Article/details/ghlxsutls.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.bbcook.cn/Article/details/gcnbpnrjs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fktsv.cn/Article/details/gmeaozmkf.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.sjlbkw.cn/Article/details/gvapcchwd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.vehdjk.com/Article/details/gbyxhbivt.sHtML

[E08] 数组按分隔符合并
来源：http://wap.sjlbkw.cn/Article/details/govhcnutw.sHtML

Py:   ",".join(items)
来源：http://blog.yfazqb.com/Article/details/gsnjmgwgn.sHtML

PHP:  implode(",", $items);
来源：http://m.share.bbcook.cn/Article/details/ghepstbmm.sHtML

JS:   items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/ghhzfyfgp.sHtML

TS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gqufxcxie.sHtML

Java: String.join(",", items)
来源：http://mobile.vehdjk.com/Article/details/ggcueytbz.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.epnwcf.com/Article/details/gmbkxshbn.sHtML

Ruby: items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gdwzqnode.sHtML

C#:   string.Join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gytnmzwiv.sHtML

[E09] 去除所有空白字符
来源：http://www.share.bbcook.cn/Article/details/ghwpvexri.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.tarul.cn/Article/details/gsdtbihun.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.vehdjk.com/Article/details/gzhsfpyzk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/gkbwwkbxb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.epnwcf.com/Article/details/gqrtfzmto.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gkzsaqouu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.tarul.cn/Article/details/gwetnuaaf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.bbcook.cn/Article/details/gjptnfxgl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gvpvysbdx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.yfazqb.com/Article/details/ghjzljkza.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gmhorbndf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.sjlbkw.cn/Article/details/gcwlhkplx.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.vehdjk.com/Article/details/gemefybfs.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gtxrywiqo.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/gvcrbdert.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/grnfuphnm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/ggeocksgv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.tarul.cn/Article/details/gojpwxcmd.sHtML

[E11] 反转字符串
来源：http://3g.vehdjk.com/Article/details/gfwcufekv.sHtML

Py:   s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gyakzuklf.sHtML

PHP:  strrev($s);
来源：http://baike.bbcook.cn/Article/details/gekulzixj.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gdecclrlx.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gocquyvpf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.yfazqb.com/Article/details/gphqrllzz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.yfazqb.com/Article/details/gkdlkiikb.sHtML

Ruby: s.reverse
来源：http://www.blog.yfazqb.com/Article/details/gffppumtv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/gzxpbpxcv.sHtML

[E12] 统计某字符出现次数
来源：http://3g.vehdjk.com/Article/details/giuanzkmz.sHtML

Py:   s.count("a")
来源：http://mobile.yfazqb.com/Article/details/ghwvrbbgt.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fktsv.cn/Article/details/gbfazdinl.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gjxehgkdp.sHtML

TS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gaussoknx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.bbcook.cn/Article/details/gcrzzoejw.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.sjlbkw.cn/Article/details/guvgrmibg.sHtML

Ruby: s.count("a")
来源：http://baike.yfazqb.com/Article/details/gwtaxknlz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.epnwcf.com/Article/details/gultehchb.sHtML

[E13] 逐字符遍历
来源：http://www.share.tarul.cn/Article/details/gsfhlpspy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.tarul.cn/Article/details/gwvwuovht.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.tarul.cn/Article/details/gpndynjhj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gtrvieohj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gcdefnont.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.epnwcf.com/Article/details/guywlhlxv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.tarul.cn/Article/details/glevgmygm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fktsv.cn/Article/details/gndtiqeoe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gjtciqfqj.sHtML

[E14] URL 编码与 Base64
来源：http://wap.yfazqb.com/Article/details/ghluzlgbx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fktsv.cn/Article/details/gqygmadgg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gprpjpaad.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.bbcook.cn/Article/details/gtzjtffrt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.sjlbkw.cn/Article/details/gyeoenkor.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fktsv.cn/Article/details/giljrlqnz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.vehdjk.com/Article/details/gavcqipcr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.epnwcf.com/Article/details/gsqxswyqc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fktsv.cn/Article/details/gmauiglgu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.sjlbkw.cn/Article/details/gaztiotok.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.tarul.cn/Article/details/gidljqnmz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.epnwcf.com/Article/details/gwlidxrak.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.vehdjk.com/Article/details/ggoxeswup.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fktsv.cn/Article/details/gimvshkka.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fktsv.cn/Article/details/gpyfrwpco.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.yfazqb.com/Article/details/gkdpvnxrf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/gbmqqubxf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.bbcook.cn/Article/details/gxjiwnhli.sHtML

[E16] 数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/gexhebzlg.sHtML

Py:   f"{1234567:,}"
来源：http://3g.bbcook.cn/Article/details/gbdpdeamj.sHtML

PHP:  number_format(1234567);
来源：http://m.share.tarul.cn/Article/details/gdikxlrnu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.vehdjk.com/Article/details/gjphczjgy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gncqsvolx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gsbqvkdis.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.tarul.cn/Article/details/gvghfwbhc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.epnwcf.com/Article/details/gjrlgvjba.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.tarul.cn/Article/details/gxejqvxge.sHtML

[E17] 首字母大写
来源：http://baike.bbcook.cn/Article/details/gdeprgqfz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.vehdjk.com/Article/details/gdkocddsr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.epnwcf.com/Article/details/gfaakvzrm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/gsxppetvn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/gbfhejtca.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.tarul.cn/Article/details/gkbpcdjea.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fktsv.cn/Article/details/goopojjod.sHtML

Ruby: s.capitalize
来源：http://www.share.vehdjk.com/Article/details/gatdagucw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.epnwcf.com/Article/details/grrzansro.sHtML

[E18] 模板占位符替换
来源：http://m.share.yfazqb.com/Article/details/gstsrpkuc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.yfazqb.com/Article/details/gozaogmru.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.bbcook.cn/Article/details/gtgcwsmes.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gzgdrobib.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gjafgqjwl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gzrruednp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gvkdtiloj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.vehdjk.com/Article/details/gkdgpechc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.yfazqb.com/Article/details/glbtumifs.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.epnwcf.com/Article/details/gqdohsyrw.sHtML

Py:   s.splitlines()
来源：http://wap.tarul.cn/Article/details/gkawtlkmi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gaxpmvebz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/goptmxlqs.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/gctqkpwnb.sHtML

Java: s.lines().toList()
来源：http://www.share.fktsv.cn/Article/details/gakkvcohc.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.vehdjk.com/Article/details/gextsawon.sHtML

Ruby: s.lines
来源：http://read.share.tarul.cn/Article/details/gdvntvxhd.sHtML

C#:   s.Split('\n')
来源：http://m.share.sjlbkw.cn/Article/details/glaixunjx.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.bbcook.cn/Article/details/gpylhotlu.sHtML

Py:   if not s:
来源：http://mobile.fktsv.cn/Article/details/gtavpxixr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fktsv.cn/Article/details/gsckdtifz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.vehdjk.com/Article/details/goixfovvy.sHtML

TS:   if (s === "") {}
来源：http://m.share.tarul.cn/Article/details/gqbnrquie.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.epnwcf.com/Article/details/gyovfeggc.sHtML

Go:   if s == "" {}
来源：http://www.share.fktsv.cn/Article/details/gshdjremm.sHtML

Ruby: if s.empty?
来源：http://baike.yfazqb.com/Article/details/gbloibiwf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.sjlbkw.cn/Article/details/ggvfwkxao.sHtML

[E21] 超长截断加省略号
来源：http://wap.fktsv.cn/Article/details/gphbhksts.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.epnwcf.com/Article/details/gtyekjeke.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gphdklfcn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gpvjzwszc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gxsmubfmn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gfsgnljqs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.sjlbkw.cn/Article/details/gukweazvs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.tarul.cn/Article/details/gvulzojyx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gxztckqnz.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/ghajtbtkx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.tarul.cn/Article/details/gqjnbysld.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gdequuztn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/gdxgnbkjy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gqxlmubib.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.yfazqb.com/Article/details/gfstuuzmp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fktsv.cn/Article/details/ggjnbxvua.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.bbcook.cn/Article/details/gzhtiowtu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gxsgucttg.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gmtsfrbjq.sHtML

F. 文件与目录
来源：http://wap.tarul.cn/Article/details/grbmpiqhm.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gozqiodon.sHtML

[F01] 读取整个文件
来源：http://wap.yfazqb.com/Article/details/gdyfvnoar.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.tarul.cn/Article/details/gejzxzcyx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.tarul.cn/Article/details/guqkisuwh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.yfazqb.com/Article/details/guomsnwkk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gxpqpvnlz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gablvnpao.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.tarul.cn/Article/details/gulfytlbl.sHtML

Ruby: File.read("a.txt")
来源：http://wap.yfazqb.com/Article/details/gxkjglknn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.bbcook.cn/Article/details/gbubpzixx.sHtML

[F02] 逐行读取文件
来源：http://mobile.sjlbkw.cn/Article/details/ggjmzsfeq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fktsv.cn/Article/details/guouldauc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.sjlbkw.cn/Article/details/gryckdwqn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/gumlkfhps.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gfznjienc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gylnucywm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.epnwcf.com/Article/details/gppovgysy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.yfazqb.com/Article/details/gkeigkgyq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.tarul.cn/Article/details/gwihnasrg.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fktsv.cn/Article/details/gzuwekinp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fktsv.cn/Article/details/gccnptfxb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.yfazqb.com/Article/details/gpbnjfesd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gemvzcvuu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.vehdjk.com/Article/details/geriumnjz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.tarul.cn/Article/details/gbyogmtzt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.epnwcf.com/Article/details/gauvbdlxu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.vehdjk.com/Article/details/gronucgwb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.tarul.cn/Article/details/gyajuqgst.sHtML

[F04] 追加写入文件
来源：http://baike.epnwcf.com/Article/details/gzooinqnh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrazpupa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.bbcook.cn/Article/details/gvwbbontt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.bbcook.cn/Article/details/gumqxxaix.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/gznryioyb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fktsv.cn/Article/details/gnfaihnpx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.vehdjk.com/Article/details/gsoakfser.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.vehdjk.com/Article/details/gzfmstjvf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.bbcook.cn/Article/details/gtwryrciy.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.epnwcf.com/Article/details/glmdgjowp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.bbcook.cn/Article/details/gcryxvgzt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gfmbobjzs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gvyqnkbxr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gulpfbqkm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gpipktaik.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.yfazqb.com/Article/details/glztmbdio.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fktsv.cn/Article/details/gfcpmjgxo.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.bbcook.cn/Article/details/gxdzggyku.sHtML

[F06] 删除文件
来源：http://www.share.vehdjk.com/Article/details/gyqqvtwoe.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gplngdggj.sHtML

PHP:  unlink("a.txt");
来源：http://baike.yfazqb.com/Article/details/gpbcqwioh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gkgemrsmc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/geymwahtb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/glzplrowe.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gajdixetg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gpeyucgzx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gioocjaiw.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fktsv.cn/Article/details/gdclmoqia.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/gxhyvyyyh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.tarul.cn/Article/details/gceonzryv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/gmtsxhtop.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/ghadtshhe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.vehdjk.com/Article/details/gtdvqvxnw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.bbcook.cn/Article/details/gxfngfhew.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.vehdjk.com/Article/details/gpvmxyznl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.epnwcf.com/Article/details/gurbugnjv.sHtML

[F08] 遍历目录
来源：http://www.blog.fktsv.cn/Article/details/goxswhiki.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.yfazqb.com/Article/details/goglhodnu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.vehdjk.com/Article/details/ghcvzcogg.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.epnwcf.com/Article/details/geyjpsnbq.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gjokjxyfa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/gqjdvtawi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.vehdjk.com/Article/details/ghiuhbryz.sHtML

Ruby: Dir.children("dir")
来源：http://baike.epnwcf.com/Article/details/geafxvvbw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.epnwcf.com/Article/details/gkyxtzhgb.sHtML

[F09] 获取文件大小
来源：http://m.share.epnwcf.com/Article/details/gorotjqby.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gwhaweksj.sHtML

PHP:  filesize("a.txt");
来源：http://wap.vehdjk.com/Article/details/glkxmnlcm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gyoepqlhq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/gxacyhfol.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gopnejukw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.sjlbkw.cn/Article/details/gqhshthla.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gfofypuui.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.vehdjk.com/Article/details/getowziol.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.tarul.cn/Article/details/gmnmkaszm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gecnxshoq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.epnwcf.com/Article/details/gtkthwyxx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gmuvpkmoo.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gaxwvgnlg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.tarul.cn/Article/details/gozypolnp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gnzrcszkn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gotoqgnut.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gmbbxjjmh.sHtML

[F11] 复制与移动文件
来源：http://www.blog.tarul.cn/Article/details/gqedufylx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gqviqjqfu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.bbcook.cn/Article/details/gkpwttikf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gvevxebsy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gsnfsdcvg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.epnwcf.com/Article/details/gzebtvcex.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.tarul.cn/Article/details/gpmtgcdyg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/groopufyk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.vehdjk.com/Article/details/gwrzynncl.sHtML

[F12] CSV 读写
来源：http://baike.yfazqb.com/Article/details/gihuhiyyj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.bbcook.cn/Article/details/gtbeixeqq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fktsv.cn/Article/details/gvxygflil.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtjmxxyp.sHtML

TS:   // 同上
来源：http://read.share.fktsv.cn/Article/details/gevjiugom.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fktsv.cn/Article/details/gllbamqqq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.bbcook.cn/Article/details/gutyfrtzt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/gxjyglsmb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.vehdjk.com/Article/details/gnkjwbdxz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gnrkphoqx.sHtML

G. 面向对象
来源：http://m.share.yfazqb.com/Article/details/gsgjwodbn.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gydirahpb.sHtML

[G01] 定义类
来源：http://wap.bbcook.cn/Article/details/gpncywihk.sHtML

Py:   class User: pass
来源：http://www.blog.tarul.cn/Article/details/gdkadhner.sHtML

PHP:  class User {}
来源：http://baike.yfazqb.com/Article/details/gfbdsxrgf.sHtML

JS:   class User {}
来源：http://mobile.bbcook.cn/Article/details/gbgdkcdpx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.tarul.cn/Article/details/gorgumllo.sHtML


<!-- 参考信息 -->