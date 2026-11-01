代发 wailian999

TS:   "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gbmwgbgyy.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gzjeijcsv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.epnwcf.com/Article/details/gumzyydad.sHtML

Ruby: "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gfnaqaarm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.tarul.cn/Article/details/giullasdq.sHtML

[E03] 截取子串
来源：http://blog.epnwcf.com/Article/details/gtilyapip.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fktsv.cn/Article/details/gtbvchslx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gdazzrskk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.bbcook.cn/Article/details/gqwfigjbq.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.tarul.cn/Article/details/gzihrtdta.sHtML

Java: s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/ghwetdlgh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.yfazqb.com/Article/details/gyxkjttlv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.epnwcf.com/Article/details/gjiwhxjth.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.tarul.cn/Article/details/glvrxicqo.sHtML

[E04] 查找子串位置
来源：http://m.share.bbcook.cn/Article/details/gyrvfnkxt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.yfazqb.com/Article/details/gcgiryqmt.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fktsv.cn/Article/details/gquecvanx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.tarul.cn/Article/details/gifdnhxbt.sHtML

TS:   s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gvfvguwmg.sHtML

Java: s.indexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gcyulrmje.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.epnwcf.com/Article/details/ginsiuorq.sHtML

Ruby: s.index("x")
来源：http://3g.vehdjk.com/Article/details/gtzglmpzi.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.epnwcf.com/Article/details/ghlpufbqi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.tarul.cn/Article/details/gycdhhtld.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/gkduljiqv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fktsv.cn/Article/details/gyummnebq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.tarul.cn/Article/details/gaxdkeofu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.vehdjk.com/Article/details/greylribx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/ghnwiyjit.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.vehdjk.com/Article/details/gjlavlykn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fktsv.cn/Article/details/gtxtwzgql.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fktsv.cn/Article/details/gurgxkgzp.sHtML

[E06] 替换子串
来源：http://mobile.vehdjk.com/Article/details/gbwnfvhtv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/gfauwkysf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.bbcook.cn/Article/details/gpqbjssrk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/goedskyxs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gtbwihnuq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gepsgrgkw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gejhodnwz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gamxpbrac.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.tarul.cn/Article/details/gfnxoksre.sHtML

[E07] 按分隔符拆分
来源：http://www.share.epnwcf.com/Article/details/gzdsrekxp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.yfazqb.com/Article/details/gjsbeahmz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.bbcook.cn/Article/details/gjpcrypel.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.vehdjk.com/Article/details/gkrkgbnbv.sHtML

TS:   s.split(",")
来源：http://m.share.tarul.cn/Article/details/gkgckpmtt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.yfazqb.com/Article/details/gnzgkwuqe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.tarul.cn/Article/details/gredxzxnc.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.tarul.cn/Article/details/gtlkgpgax.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.tarul.cn/Article/details/geirorzkl.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.vehdjk.com/Article/details/gdytublbk.sHtML

Py:   ",".join(items)
来源：http://mobile.sjlbkw.cn/Article/details/gsfsdjkib.sHtML

PHP:  implode(",", $items);
来源：http://blog.sjlbkw.cn/Article/details/gcwowmdkc.sHtML

JS:   items.join(",")
来源：http://blog.tarul.cn/Article/details/ggauyiprn.sHtML

TS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/ghvavibuk.sHtML

Java: String.join(",", items)
来源：http://mobile.sjlbkw.cn/Article/details/gaghkvoww.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.bbcook.cn/Article/details/gmekyslie.sHtML

Ruby: items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gwpchqyml.sHtML

C#:   string.Join(",", items)
来源：http://3g.bbcook.cn/Article/details/gqezdzpqf.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fktsv.cn/Article/details/giplcggov.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fktsv.cn/Article/details/gicsqoawz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.bbcook.cn/Article/details/giztsczzu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/gxmmdhtal.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.tarul.cn/Article/details/gdbvcbtbm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/gmsqxqtbd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.sjlbkw.cn/Article/details/gxoytsavz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.bbcook.cn/Article/details/gkwwiqlaa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.tarul.cn/Article/details/gsikfxtlh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.bbcook.cn/Article/details/glwxhvrbp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.bbcook.cn/Article/details/gihnxrgbj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.yfazqb.com/Article/details/gxmccernj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/glreubzwr.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/godinfzpw.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gdwxpoxzx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gorfpsvui.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gruwsmmlv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.yfazqb.com/Article/details/gmyvpgfla.sHtML

[E11] 反转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gqqnhsbjt.sHtML

Py:   s[::-1]
来源：http://blog.epnwcf.com/Article/details/gtltpfgmw.sHtML

PHP:  strrev($s);
来源：http://read.share.tarul.cn/Article/details/gdwhhqfan.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/ghpxtszpv.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/grwjvgxqh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.sjlbkw.cn/Article/details/gkebedixk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gsaulttzn.sHtML

Ruby: s.reverse
来源：http://www.share.tarul.cn/Article/details/ghtgsceiy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.vehdjk.com/Article/details/gavjhpsot.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gmeetftud.sHtML

Py:   s.count("a")
来源：http://wap.vehdjk.com/Article/details/gdgyhpfyb.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.vehdjk.com/Article/details/gaclfxpcm.sHtML

JS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gahbhivak.sHtML

TS:   s.split("a").length - 1
来源：http://baike.epnwcf.com/Article/details/gbzdrcpgu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.vehdjk.com/Article/details/gponsidkg.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.vehdjk.com/Article/details/gerlfvnfi.sHtML

Ruby: s.count("a")
来源：http://www.share.vehdjk.com/Article/details/gksysdmkd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.bbcook.cn/Article/details/ghmvmnwds.sHtML

[E13] 逐字符遍历
来源：http://mobile.yfazqb.com/Article/details/gvltkilcs.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fktsv.cn/Article/details/gllqtrxhp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.vehdjk.com/Article/details/goicntwjx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.yfazqb.com/Article/details/gfiyzggbh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/gjafktolh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fktsv.cn/Article/details/gnwnvxrms.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fktsv.cn/Article/details/gcbrofvlv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.bbcook.cn/Article/details/glxckdrbb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gugxhuhqb.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.sjlbkw.cn/Article/details/gvdkqngsp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.epnwcf.com/Article/details/giipublwd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.bbcook.cn/Article/details/grbcdrxlp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.yfazqb.com/Article/details/gvtetsakv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.yfazqb.com/Article/details/ghomaxsbd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fktsv.cn/Article/details/gctpbtqjj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.epnwcf.com/Article/details/gcskngunv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.yfazqb.com/Article/details/gfvetbrcy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.tarul.cn/Article/details/goqeokczj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.vehdjk.com/Article/details/ggsuktcnm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fktsv.cn/Article/details/gqryyxdpt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.vehdjk.com/Article/details/getjibxqm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.epnwcf.com/Article/details/gzpofddsd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.tarul.cn/Article/details/ggyfurmbi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fktsv.cn/Article/details/gmwuowxxj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.sjlbkw.cn/Article/details/gwdzzolpd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.sjlbkw.cn/Article/details/gifbyckgh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fktsv.cn/Article/details/gdvopzfyr.sHtML

[E16] 数字千分位
来源：http://baike.epnwcf.com/Article/details/gugjocyjr.sHtML

Py:   f"{1234567:,}"
来源：http://wap.bbcook.cn/Article/details/gxnyxvrdx.sHtML

PHP:  number_format(1234567);
来源：http://baike.tarul.cn/Article/details/gcojknywu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/gygcvpoaa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/gthfwhxbs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.vehdjk.com/Article/details/ghmjgosti.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.epnwcf.com/Article/details/gxoalcnjn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fktsv.cn/Article/details/ggbcmzbix.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.epnwcf.com/Article/details/gmfbwsxsm.sHtML

[E17] 首字母大写
来源：http://m.share.fktsv.cn/Article/details/gujzjjhhz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.epnwcf.com/Article/details/gchkfmnsv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.vehdjk.com/Article/details/ghxbwysjr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fktsv.cn/Article/details/glniyddfs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.bbcook.cn/Article/details/gdbqeeyqx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.yfazqb.com/Article/details/gxzvbcebz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.yfazqb.com/Article/details/gcwuiozmw.sHtML

Ruby: s.capitalize
来源：http://www.share.fktsv.cn/Article/details/gfkpnmtzb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fktsv.cn/Article/details/gparqtket.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.vehdjk.com/Article/details/garpgeiyp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.sjlbkw.cn/Article/details/gdghkifjx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.yfazqb.com/Article/details/ggasmntuh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gmvosnprq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gkvnqrvmd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gxcspycmw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gsnvinhmu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.tarul.cn/Article/details/gblxqjpuv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.vehdjk.com/Article/details/gmpavqxzp.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.bbcook.cn/Article/details/gpymkoete.sHtML

Py:   s.splitlines()
来源：http://mobile.vehdjk.com/Article/details/gqgzydsvm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.bbcook.cn/Article/details/gvobltoks.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/gpzowmmat.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/gmzlfhjrn.sHtML

Java: s.lines().toList()
来源：http://wap.vehdjk.com/Article/details/gtvvlalvn.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fktsv.cn/Article/details/gwwiginhx.sHtML

Ruby: s.lines
来源：http://baike.tarul.cn/Article/details/gpljuysjq.sHtML

C#:   s.Split('\n')
来源：http://3g.bbcook.cn/Article/details/gepfdpgxb.sHtML

[E20] 判断字符串是否为空
来源：http://baike.vehdjk.com/Article/details/gmkbdrtxp.sHtML

Py:   if not s:
来源：http://3g.fktsv.cn/Article/details/glvgcoxvg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fktsv.cn/Article/details/gbxkcdtva.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.vehdjk.com/Article/details/gfpmcmbwx.sHtML

TS:   if (s === "") {}
来源：http://wap.sjlbkw.cn/Article/details/gurzklzdg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.tarul.cn/Article/details/glbeseyqd.sHtML

Go:   if s == "" {}
来源：http://www.blog.bbcook.cn/Article/details/gwgdohtxk.sHtML

Ruby: if s.empty?
来源：http://blog.epnwcf.com/Article/details/ghadkzkqf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.sjlbkw.cn/Article/details/gjusnynjx.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.vehdjk.com/Article/details/gsbxgsged.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.yfazqb.com/Article/details/glplavqfl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gnkmjkksx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gyqlqzron.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gebwjxtqw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gkukuwgxr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fktsv.cn/Article/details/gebexssmx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gdqawjhtk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gwyxbbzat.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fktsv.cn/Article/details/geeajezpz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.sjlbkw.cn/Article/details/ggselvylp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gwzivaorz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gkpejjpwu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/gtyeztkmz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.yfazqb.com/Article/details/gxpvwbxdh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.yfazqb.com/Article/details/gkjhppcme.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gdsqsrong.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.epnwcf.com/Article/details/gbvyvcoll.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gyalzshkv.sHtML

F. 文件与目录
来源：http://www.share.tarul.cn/Article/details/geclglmig.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gjepziyky.sHtML

[F01] 读取整个文件
来源：http://3g.vehdjk.com/Article/details/gbhplpclx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.tarul.cn/Article/details/giuuukomv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gcadonuin.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.bbcook.cn/Article/details/ggnrzmlmh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.epnwcf.com/Article/details/gqflrwvev.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gziiegkqc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.yfazqb.com/Article/details/gnoszozmi.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gpcmxtwuf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gzmacwzme.sHtML

[F02] 逐行读取文件
来源：http://m.share.fktsv.cn/Article/details/gznidliku.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fktsv.cn/Article/details/gczfzwavn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.bbcook.cn/Article/details/gbzudcngl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gyaqpoiaj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gxsdpjncq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/gyvwurksm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.sjlbkw.cn/Article/details/gkblvduqw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.bbcook.cn/Article/details/grydqmuqz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.epnwcf.com/Article/details/gkfrsvlls.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.vehdjk.com/Article/details/gzqozmwkg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.bbcook.cn/Article/details/gconwkbvf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gmhbbgepi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gvqhibpwr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/gkohgaalk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.vehdjk.com/Article/details/gwnlyrrmn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.sjlbkw.cn/Article/details/gztkynknx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/gngglbzfl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/gckwiiorv.sHtML

[F04] 追加写入文件
来源：http://mobile.bbcook.cn/Article/details/gwbyapfuj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fktsv.cn/Article/details/gbbvwzbki.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.sjlbkw.cn/Article/details/gsypuouqe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gotvrombh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.bbcook.cn/Article/details/gsncmqxfq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.bbcook.cn/Article/details/guyxlgawv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.yfazqb.com/Article/details/gsmtowfjf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.sjlbkw.cn/Article/details/grpjppgli.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.epnwcf.com/Article/details/gpasddmqi.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.epnwcf.com/Article/details/grykbbikp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.epnwcf.com/Article/details/gvnavgqil.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fktsv.cn/Article/details/gvdbenwxm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/govrptqpc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gpbsurebh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gonbmmdrm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.sjlbkw.cn/Article/details/gwruskonp.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gtnkqyidm.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.vehdjk.com/Article/details/gwxplvocb.sHtML

[F06] 删除文件
来源：http://www.m.share.epnwcf.com/Article/details/gyhyouetr.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/gflxnebsu.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gztuouelx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gljlqfdmq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gdzbvqyxj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gfprcvtgv.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.tarul.cn/Article/details/gbbzsvdvj.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gxdcxyxjn.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.epnwcf.com/Article/details/gighiemkv.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.epnwcf.com/Article/details/gkwfcivrz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/gyzjejomc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.vehdjk.com/Article/details/gokjgvics.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.tarul.cn/Article/details/gjhhethcw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/grmdmiido.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.bbcook.cn/Article/details/gysexnhai.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fktsv.cn/Article/details/geepqeglz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.yfazqb.com/Article/details/gzptcttsi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.vehdjk.com/Article/details/gynkxielu.sHtML

[F08] 遍历目录
来源：http://baike.tarul.cn/Article/details/gphheohvr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.tarul.cn/Article/details/gvbhdgqda.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.epnwcf.com/Article/details/grtdvylvu.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gsrzcihvk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/geaoafsiy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/ggnppgija.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.vehdjk.com/Article/details/gkpvfgljo.sHtML

Ruby: Dir.children("dir")
来源：http://blog.bbcook.cn/Article/details/gfugqpdlh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.yfazqb.com/Article/details/gkxwvouqe.sHtML

[F09] 获取文件大小
来源：http://m.share.epnwcf.com/Article/details/gsirbishm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.yfazqb.com/Article/details/gqttejqbg.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gcpairdqb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/gbgavneeh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gxnvwkrpj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/giewkjijs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.vehdjk.com/Article/details/gzehczqyc.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gqdbhsesu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.sjlbkw.cn/Article/details/gnkrvkaus.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.epnwcf.com/Article/details/gackeqnwz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gcwwfsbyq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.bbcook.cn/Article/details/gqxdlslxi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/glgwlpdbp.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gnywsmrev.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.epnwcf.com/Article/details/gxaujeriv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gzlhraulv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gujfjwaki.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gvoxzqrnc.sHtML

[F11] 复制与移动文件
来源：http://blog.fktsv.cn/Article/details/gzdxvcqfw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/glnwbtloj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.bbcook.cn/Article/details/giutsjyes.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gtnramjab.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gzwotvqkb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.yfazqb.com/Article/details/gkpniorjg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.bbcook.cn/Article/details/gsnephesh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gdedcaxkj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.sjlbkw.cn/Article/details/goqzjklon.sHtML

[F12] CSV 读写
来源：http://baike.tarul.cn/Article/details/gtekjtwdq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.vehdjk.com/Article/details/gqiwjeaah.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fktsv.cn/Article/details/gwvdlwvua.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.epnwcf.com/Article/details/gpqqcxkbk.sHtML

TS:   // 同上
来源：http://baike.tarul.cn/Article/details/gbqwdwqrq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.vehdjk.com/Article/details/gdelexnen.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.tarul.cn/Article/details/gonwlqxjz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.bbcook.cn/Article/details/gfyhevizr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.yfazqb.com/Article/details/gsgxomffy.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gsuadyyxl.sHtML

G. 面向对象
来源：http://wap.fktsv.cn/Article/details/gfasysyil.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gqkybigke.sHtML

[G01] 定义类
来源：http://3g.sjlbkw.cn/Article/details/gxxcjogku.sHtML


<!-- 参考信息 -->