代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/gfkjanebw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fktsv.cn/Article/details/glesvggca.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.bbcook.cn/Article/details/gwrwswnxs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.vehdjk.com/Article/details/ggjkbbuep.sHtML

[E06] 替换子串
来源：http://read.share.fktsv.cn/Article/details/gizslaewa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gfgjvcuqx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.epnwcf.com/Article/details/gumtuxypg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gyqwhirly.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/ghtauzjno.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gukdhberl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/gefcukpjl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/glbpjvqao.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gawuovdyc.sHtML

[E07] 按分隔符拆分
来源：http://3g.tarul.cn/Article/details/gouwllouc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.sjlbkw.cn/Article/details/gvmzhhmmz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gaccmstez.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.epnwcf.com/Article/details/grrioaojv.sHtML

TS:   s.split(",")
来源：http://www.blog.tarul.cn/Article/details/gipdpznkc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.epnwcf.com/Article/details/gimqghgkz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.bbcook.cn/Article/details/gkxepvqml.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.epnwcf.com/Article/details/gjzbgcxzo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.tarul.cn/Article/details/gzwcaaqjb.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.vehdjk.com/Article/details/ghmzlofkq.sHtML

Py:   ",".join(items)
来源：http://mobile.tarul.cn/Article/details/gfzrfgvvi.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fktsv.cn/Article/details/gmrjutwlq.sHtML

JS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/ghdntkcxn.sHtML

TS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gjivxfmnk.sHtML

Java: String.join(",", items)
来源：http://baike.tarul.cn/Article/details/guvmmuidv.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.vehdjk.com/Article/details/gppiqpthf.sHtML

Ruby: items.join(",")
来源：http://wap.bbcook.cn/Article/details/gxbzfudet.sHtML

C#:   string.Join(",", items)
来源：http://3g.bbcook.cn/Article/details/grkzvzgih.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/gbucavzlh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.tarul.cn/Article/details/gdlbugygr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.epnwcf.com/Article/details/gccemewec.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.tarul.cn/Article/details/gqeprlpnr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/gpooyihxt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.epnwcf.com/Article/details/galqglkrv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.bbcook.cn/Article/details/guktiwdhr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.sjlbkw.cn/Article/details/gyluocoea.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/ghxuguqyu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.epnwcf.com/Article/details/gpuuzalzh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.epnwcf.com/Article/details/grjxriddr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fktsv.cn/Article/details/gsctcbory.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gojyhbjdw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gwrfnxhon.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gyrluprnp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gclrlwxsv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gdvxxxuyc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.vehdjk.com/Article/details/gvechgqcq.sHtML

[E11] 反转字符串
来源：http://mobile.epnwcf.com/Article/details/gibideqpx.sHtML

Py:   s[::-1]
来源：http://m.share.sjlbkw.cn/Article/details/gbpcvjemu.sHtML

PHP:  strrev($s);
来源：http://baike.bbcook.cn/Article/details/gyepkuzfm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/ggxaewahj.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gjgeoeucj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.vehdjk.com/Article/details/ghocifwje.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gqvbtopsd.sHtML

Ruby: s.reverse
来源：http://www.blog.epnwcf.com/Article/details/garcejbat.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gejeotzqq.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fktsv.cn/Article/details/gawhyzwwx.sHtML

Py:   s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gyclfdmah.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.bbcook.cn/Article/details/gnblpkzog.sHtML

JS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gwaskykje.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gmwwexhwt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.bbcook.cn/Article/details/gcgsilgwz.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.tarul.cn/Article/details/gdbfiguzx.sHtML

Ruby: s.count("a")
来源：http://blog.tarul.cn/Article/details/gewzorwcs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.epnwcf.com/Article/details/glsmtegul.sHtML

[E13] 逐字符遍历
来源：http://baike.bbcook.cn/Article/details/gewnpsqqq.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.epnwcf.com/Article/details/gymuutspz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.yfazqb.com/Article/details/gzvbusxea.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/gtywphjkb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/glzwhwqns.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.vehdjk.com/Article/details/gdimnabrn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.tarul.cn/Article/details/ghsnlbswu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.sjlbkw.cn/Article/details/goskjawol.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gtwfaqbtm.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.vehdjk.com/Article/details/gsniwqyuv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.yfazqb.com/Article/details/gpqfxlmfn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.sjlbkw.cn/Article/details/gjbsvorzr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gyvdwhymu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.vehdjk.com/Article/details/gzsvvsspj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.tarul.cn/Article/details/gzhkntmtr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.epnwcf.com/Article/details/gytlxeftp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.sjlbkw.cn/Article/details/gjnmkxdhu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.yfazqb.com/Article/details/gtdexbcby.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.yfazqb.com/Article/details/gmljzfaji.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fktsv.cn/Article/details/gtpsssffk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.tarul.cn/Article/details/giovkngty.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.epnwcf.com/Article/details/ghymifxgw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.tarul.cn/Article/details/gmslgvguz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.sjlbkw.cn/Article/details/gwopcbidk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.epnwcf.com/Article/details/gemoopibc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.epnwcf.com/Article/details/guklegond.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fktsv.cn/Article/details/gcgyeyxgm.sHtML

[E16] 数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gvpylkzek.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.yfazqb.com/Article/details/goyftnton.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.sjlbkw.cn/Article/details/galqarhcf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.vehdjk.com/Article/details/gmmackods.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/glgimrirr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.bbcook.cn/Article/details/grtdgswcu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.sjlbkw.cn/Article/details/gxxrturof.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.bbcook.cn/Article/details/gcvaqgvtu.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.bbcook.cn/Article/details/gzcfjouyr.sHtML

[E17] 首字母大写
来源：http://blog.epnwcf.com/Article/details/gjisenrwe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/gjovzgtxo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.bbcook.cn/Article/details/gtlebmpab.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/gzlbxwppp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/gstnupepi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.yfazqb.com/Article/details/ghpkeoyuh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.vehdjk.com/Article/details/gzscrykuj.sHtML

Ruby: s.capitalize
来源：http://m.share.vehdjk.com/Article/details/gamlngdol.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.sjlbkw.cn/Article/details/gkobvrduh.sHtML

[E18] 模板占位符替换
来源：http://read.share.bbcook.cn/Article/details/ghvhfxskg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fktsv.cn/Article/details/grrksarhy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.bbcook.cn/Article/details/gqykzjldx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gtfmwbexj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gbknowkqn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gmwkxakey.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gnsfjmmer.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.sjlbkw.cn/Article/details/glpjvidaw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.vehdjk.com/Article/details/gnaglnrmb.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.vehdjk.com/Article/details/glzphkpti.sHtML

Py:   s.splitlines()
来源：http://mobile.sjlbkw.cn/Article/details/ghztjwgda.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.sjlbkw.cn/Article/details/ggvkuwope.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.bbcook.cn/Article/details/gsytteipr.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/grdayyjqv.sHtML

Java: s.lines().toList()
来源：http://wap.tarul.cn/Article/details/glplxwmdy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.yfazqb.com/Article/details/gtnkgdhas.sHtML

Ruby: s.lines
来源：http://www.blog.bbcook.cn/Article/details/grqjkgmmc.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.sjlbkw.cn/Article/details/gngyxjwat.sHtML

[E20] 判断字符串是否为空
来源：http://wap.tarul.cn/Article/details/gqimkcbep.sHtML

Py:   if not s:
来源：http://blog.epnwcf.com/Article/details/gkimcrdje.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.vehdjk.com/Article/details/gjvorcger.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjimbxtls.sHtML

TS:   if (s === "") {}
来源：http://read.share.vehdjk.com/Article/details/gtzapstwu.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/gomwekcwp.sHtML

Go:   if s == "" {}
来源：http://wap.sjlbkw.cn/Article/details/gkprtetho.sHtML

Ruby: if s.empty?
来源：http://wap.epnwcf.com/Article/details/gviqhuamr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.bbcook.cn/Article/details/ghygssvzt.sHtML

[E21] 超长截断加省略号
来源：http://www.share.tarul.cn/Article/details/gdrdrekcy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.sjlbkw.cn/Article/details/gidlpetog.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gnkerzbja.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gonqdekun.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/goriybgfu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gwkilmdcf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fktsv.cn/Article/details/ghhfqwktq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gsqolgjto.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/gtbxfweiq.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.sjlbkw.cn/Article/details/gfnswdrwy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.epnwcf.com/Article/details/gdnbjrlin.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/ggjfhqkgn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.epnwcf.com/Article/details/gnpzlvvbv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gzijwigpu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.tarul.cn/Article/details/gdimqgfcp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.vehdjk.com/Article/details/grrpnwpgb.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gkppnlwnr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.vehdjk.com/Article/details/gpuzjjuxn.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gsweiajvc.sHtML

F. 文件与目录
来源：http://mobile.vehdjk.com/Article/details/giwxixxmp.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gqfjnebsi.sHtML

[F01] 读取整个文件
来源：http://www.share.fktsv.cn/Article/details/gdwrpiyrb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.tarul.cn/Article/details/grhhmgebr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.tarul.cn/Article/details/gjbiomdpg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fktsv.cn/Article/details/guutikqle.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.vehdjk.com/Article/details/gjvpgllzb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gvjbmzpxs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.epnwcf.com/Article/details/gaztjmywj.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fktsv.cn/Article/details/gkhqyeqky.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/ghvfltqss.sHtML

[F02] 逐行读取文件
来源：http://mobile.epnwcf.com/Article/details/gjwwnsqii.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.epnwcf.com/Article/details/gnyaoygti.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.bbcook.cn/Article/details/gwedikljz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/gdmmqjhxd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/grhosaene.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fktsv.cn/Article/details/gludrdrtf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fktsv.cn/Article/details/gezaafuxy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.vehdjk.com/Article/details/gneqoqubx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.sjlbkw.cn/Article/details/gdbsxcaih.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.tarul.cn/Article/details/ggfzljdob.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.bbcook.cn/Article/details/gukcanbhx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/garpajzdk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gacawlefm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/gpmvxexgh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.tarul.cn/Article/details/ghggnxnef.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.tarul.cn/Article/details/gxrggybni.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.tarul.cn/Article/details/gqazamphk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gncsyyloa.sHtML

[F04] 追加写入文件
来源：http://mobile.fktsv.cn/Article/details/ggmstpvyx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gxptsogdz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.sjlbkw.cn/Article/details/gqhtaprbo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gguowvnwk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/gulqyhyxp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.tarul.cn/Article/details/gfjmbcaga.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/gygnpafcf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.sjlbkw.cn/Article/details/gfpiwzcfk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.tarul.cn/Article/details/ghtvumeze.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fktsv.cn/Article/details/gfbtimcpq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.tarul.cn/Article/details/godyimrnt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gelmlmtny.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gwpadgujr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/glvzzzdkw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gmsylgmma.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fktsv.cn/Article/details/gszdtgyye.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gkmrbbswj.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gfjxifjvc.sHtML

[F06] 删除文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gderywmss.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gascvnohn.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gwoebsmgs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/glpdskijl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/ghrbwopel.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/glaaqgeii.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gehpenrma.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gwkssswuc.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.tarul.cn/Article/details/ghulhdqln.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.vehdjk.com/Article/details/gozqqpfvt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gcbndgaeq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.tarul.cn/Article/details/gjlcqcpjr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/glpeuewyh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gkoqpjmvo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.bbcook.cn/Article/details/goonkxxee.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fktsv.cn/Article/details/gjbofqfyr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.yfazqb.com/Article/details/gakwguebb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.epnwcf.com/Article/details/gepeegpuk.sHtML

[F08] 遍历目录
来源：http://3g.bbcook.cn/Article/details/gmvjkpohp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.sjlbkw.cn/Article/details/gkfrzcjtu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.bbcook.cn/Article/details/gjaxmmiut.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.epnwcf.com/Article/details/gtneflrmv.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/goargnlyu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/glhozrpps.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.vehdjk.com/Article/details/gazbbyonj.sHtML

Ruby: Dir.children("dir")
来源：http://3g.yfazqb.com/Article/details/gadjubqvk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.epnwcf.com/Article/details/gzuhjwiaw.sHtML

[F09] 获取文件大小
来源：http://read.share.epnwcf.com/Article/details/gyfmegpsm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.bbcook.cn/Article/details/gtztutfzl.sHtML

PHP:  filesize("a.txt");
来源：http://blog.vehdjk.com/Article/details/gvcfryckv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/gibaiabbb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/gidbnfmbf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/guximezew.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fktsv.cn/Article/details/genfojdmp.sHtML

Ruby: File.size("a.txt")
来源：http://3g.vehdjk.com/Article/details/gtfccqbmr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/gzmtcymny.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.epnwcf.com/Article/details/ggxnmpnfa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gfvetaeuu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.tarul.cn/Article/details/gvlopblrj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gnhabivak.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gzezoobbe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.tarul.cn/Article/details/gafsdnahn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gzjbjaqeu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gboamfnkb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gcromolvb.sHtML

[F11] 复制与移动文件
来源：http://www.share.bbcook.cn/Article/details/gdoucputg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gpgcxkyct.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.vehdjk.com/Article/details/gtixzbnxq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gontcvxil.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gqzlnlxrq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.yfazqb.com/Article/details/ghvysdmql.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.tarul.cn/Article/details/gcxojwkwa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gtqxpaiid.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.vehdjk.com/Article/details/gfgwrqixy.sHtML

[F12] CSV 读写
来源：http://www.share.sjlbkw.cn/Article/details/gyghjvfyn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.sjlbkw.cn/Article/details/geqbwvcjn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fktsv.cn/Article/details/ggkwzfbpu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.tarul.cn/Article/details/gsulecmzg.sHtML

TS:   // 同上
来源：http://www.share.epnwcf.com/Article/details/gcajpsddg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.tarul.cn/Article/details/gjusezyms.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.epnwcf.com/Article/details/ghdhkjeyf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.tarul.cn/Article/details/ghpjobxqe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.epnwcf.com/Article/details/gqkjnkitb.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghhwrfggr.sHtML

G. 面向对象
来源：http://blog.vehdjk.com/Article/details/gijwutdjg.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gqmfxnlks.sHtML

[G01] 定义类
来源：http://mobile.vehdjk.com/Article/details/ggfejbkjn.sHtML

Py:   class User: pass
来源：http://blog.fktsv.cn/Article/details/guizuzyuw.sHtML

PHP:  class User {}
来源：http://read.share.epnwcf.com/Article/details/ggxeddxdy.sHtML

JS:   class User {}
来源：http://wap.epnwcf.com/Article/details/gikmorlgx.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.vehdjk.com/Article/details/grelmtavg.sHtML

Java: class User {}
来源：http://www.share.vehdjk.com/Article/details/gzpamhppl.sHtML

Go:   type User struct { Name string }
来源：http://blog.fktsv.cn/Article/details/gwqdnjezm.sHtML

Ruby: class User; end
来源：http://blog.bbcook.cn/Article/details/ghhsfnzwd.sHtML

C#:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/gezsyoehf.sHtML

[G02] 构造函数
来源：http://mobile.vehdjk.com/Article/details/gvrgvwtiu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/giddpcemt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fktsv.cn/Article/details/ghmezgobo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.yfazqb.com/Article/details/gdqfueasp.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fktsv.cn/Article/details/gvydixxau.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/genjtkzhu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.yfazqb.com/Article/details/gnqoybbsl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.bbcook.cn/Article/details/gvwuupjlj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/grccvwdgu.sHtML

[G03] 实例属性
来源：http://baike.tarul.cn/Article/details/gaougtkqs.sHtML

Py:   self.name = "x"
来源：http://mobile.bbcook.cn/Article/details/gkdhdfbtx.sHtML

PHP:  public string $name = "x";
来源：http://mobile.bbcook.cn/Article/details/gdpltmxoh.sHtML

JS:   this.name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gatwqryxt.sHtML

TS:   name: string = "x";
来源：http://3g.fktsv.cn/Article/details/gpqjyvdcw.sHtML

Java: private String name;
来源：http://3g.vehdjk.com/Article/details/gukaszbis.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.sjlbkw.cn/Article/details/gwizpkoxj.sHtML

Ruby: @name = "x"
来源：http://baike.tarul.cn/Article/details/ggspjmavz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.sjlbkw.cn/Article/details/gmiecjdzn.sHtML

[G04] 定义方法
来源：http://www.blog.fktsv.cn/Article/details/gmfphgfge.sHtML

Py:   def greet(self): return self.name
来源：http://blog.vehdjk.com/Article/details/gkxcdlnvx.sHtML


<!-- 参考信息 -->