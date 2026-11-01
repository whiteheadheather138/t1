代发 wailian999

[E06] 替换子串
来源：http://m.share.yfazqb.com/Article/details/gbtmgwlcp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fktsv.cn/Article/details/gekqolppw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fktsv.cn/Article/details/gkkomookg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gozsvchrs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gkazjetcw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/ghinzovhh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.bbcook.cn/Article/details/ghcorlhjv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.bbcook.cn/Article/details/giclrfxol.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gvnhtwxib.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.yfazqb.com/Article/details/gontqezrs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.yfazqb.com/Article/details/gkvcflqlz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gfpjybtzi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.yfazqb.com/Article/details/gjzbprrie.sHtML

TS:   s.split(",")
来源：http://m.share.tarul.cn/Article/details/gupfvijeo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fktsv.cn/Article/details/grieuvcuk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.tarul.cn/Article/details/gzrnotjpc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.tarul.cn/Article/details/gthluqfsj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.epnwcf.com/Article/details/gskqtwrjn.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fktsv.cn/Article/details/gllkijybc.sHtML

Py:   ",".join(items)
来源：http://wap.epnwcf.com/Article/details/gezceheci.sHtML

PHP:  implode(",", $items);
来源：http://blog.yfazqb.com/Article/details/gefcblmhg.sHtML

JS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gzfwxgrcg.sHtML

TS:   items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/glvifwhkp.sHtML

Java: String.join(",", items)
来源：http://baike.bbcook.cn/Article/details/gdphjbtyv.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.yfazqb.com/Article/details/gtpattynd.sHtML

Ruby: items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gstcronyw.sHtML

C#:   string.Join(",", items)
来源：http://m.share.bbcook.cn/Article/details/gnajbzhpq.sHtML

[E09] 去除所有空白字符
来源：http://baike.epnwcf.com/Article/details/glfcactna.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fktsv.cn/Article/details/guuflksgc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.epnwcf.com/Article/details/gkbgwlkym.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/gzvlqmmkx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/gyizzgqrj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.yfazqb.com/Article/details/gdeggscha.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.tarul.cn/Article/details/gxjtwfwee.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.epnwcf.com/Article/details/glyjqrvzm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gejnjbire.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.sjlbkw.cn/Article/details/gqrvfcmni.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/gqfcffmrq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.epnwcf.com/Article/details/gsjdfpykp.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gwbxtncix.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/glmwurqdp.sHtML

Java: String.format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gzcpjkcuu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gnszbaozd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gkkchyaxb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.yfazqb.com/Article/details/gnbitadng.sHtML

[E11] 反转字符串
来源：http://wap.bbcook.cn/Article/details/geepsytxj.sHtML

Py:   s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gswoitufk.sHtML

PHP:  strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/gclribgjs.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/ggtzwilxy.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gehzeqqwy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.bbcook.cn/Article/details/gzjcmaggm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.bbcook.cn/Article/details/gazpzfsmt.sHtML

Ruby: s.reverse
来源：http://3g.yfazqb.com/Article/details/gpitxbccs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gijvoryzl.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.tarul.cn/Article/details/gbbkkatee.sHtML

Py:   s.count("a")
来源：http://3g.tarul.cn/Article/details/gpyvqunpy.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.vehdjk.com/Article/details/gevzjioby.sHtML

JS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/ggatvzzwr.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gosiubjni.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/gioebmlvx.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.tarul.cn/Article/details/gnzzqlfix.sHtML

Ruby: s.count("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gccmlytzf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.tarul.cn/Article/details/gmqqqcqib.sHtML

[E13] 逐字符遍历
来源：http://wap.vehdjk.com/Article/details/gwrnyxgzh.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.sjlbkw.cn/Article/details/gmbupqpsm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.bbcook.cn/Article/details/gfraybwtv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/gqyfkjxhm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gutbpfoim.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.yfazqb.com/Article/details/guwjdmsmp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fktsv.cn/Article/details/gmxlrcwwm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.epnwcf.com/Article/details/gxujkxzel.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.epnwcf.com/Article/details/gdskljcqi.sHtML

[E14] URL 编码与 Base64
来源：http://wap.bbcook.cn/Article/details/gcgsvzber.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.yfazqb.com/Article/details/gmydwyjnd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.vehdjk.com/Article/details/garvxrotk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.vehdjk.com/Article/details/gupbowkhu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.yfazqb.com/Article/details/gerljaoce.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.tarul.cn/Article/details/gxsjnaywg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.epnwcf.com/Article/details/ghswrryww.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.tarul.cn/Article/details/gfumiwwnz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gfsjkfnzu.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.yfazqb.com/Article/details/goaznduyc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.bbcook.cn/Article/details/geenrkzvp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fktsv.cn/Article/details/ggyezkric.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.vehdjk.com/Article/details/glcwtggan.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.vehdjk.com/Article/details/gnpqqdjzy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.yfazqb.com/Article/details/gqlsjhxbf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.vehdjk.com/Article/details/gelbjqwlb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.bbcook.cn/Article/details/gqtdguwaa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.tarul.cn/Article/details/gbwqnnlza.sHtML

[E16] 数字千分位
来源：http://baike.epnwcf.com/Article/details/gvghjagol.sHtML

Py:   f"{1234567:,}"
来源：http://wap.sjlbkw.cn/Article/details/gljdnevhp.sHtML

PHP:  number_format(1234567);
来源：http://blog.bbcook.cn/Article/details/gjfjxkaiz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gfhwcaepu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/glvpmyayh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/gfactqdxk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.epnwcf.com/Article/details/gaunbrole.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.epnwcf.com/Article/details/gyqzejgib.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.sjlbkw.cn/Article/details/gzoojhfph.sHtML

[E17] 首字母大写
来源：http://3g.bbcook.cn/Article/details/gvsvkbkys.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.sjlbkw.cn/Article/details/gvyxfyrir.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.vehdjk.com/Article/details/gtyteudqz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/ggtgfogfe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gwavspmbj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.sjlbkw.cn/Article/details/gqsfqzcwt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.vehdjk.com/Article/details/gkynxoclq.sHtML

Ruby: s.capitalize
来源：http://wap.vehdjk.com/Article/details/gikuwqeuw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.sjlbkw.cn/Article/details/gyexshelb.sHtML

[E18] 模板占位符替换
来源：http://www.share.epnwcf.com/Article/details/geldtdyaz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.epnwcf.com/Article/details/gbrpcjmio.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.sjlbkw.cn/Article/details/gzwadecwx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/giwjljafi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gfgeybbrf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gdbmbevpo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gbmpnwrjz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.sjlbkw.cn/Article/details/gcxbuwgni.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.vehdjk.com/Article/details/gjbivjxyd.sHtML

[E19] 多行文本按行拆分
来源：http://blog.epnwcf.com/Article/details/gganosjoi.sHtML

Py:   s.splitlines()
来源：http://m.share.bbcook.cn/Article/details/gnywvnyiy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.vehdjk.com/Article/details/gitqvytzg.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.vehdjk.com/Article/details/gaveudumv.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gglxdcbeq.sHtML

Java: s.lines().toList()
来源：http://wap.fktsv.cn/Article/details/gcoesjdiu.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.yfazqb.com/Article/details/gjdrxotea.sHtML

Ruby: s.lines
来源：http://www.blog.sjlbkw.cn/Article/details/gvpkiziwa.sHtML

C#:   s.Split('\n')
来源：http://blog.bbcook.cn/Article/details/gycoiigwv.sHtML

[E20] 判断字符串是否为空
来源：http://wap.tarul.cn/Article/details/gavqodadj.sHtML

Py:   if not s:
来源：http://m.share.bbcook.cn/Article/details/gyletnxtl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.yfazqb.com/Article/details/gusfajssh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fktsv.cn/Article/details/ghlsojowk.sHtML

TS:   if (s === "") {}
来源：http://m.share.vehdjk.com/Article/details/gqnebqijd.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.bbcook.cn/Article/details/gzdsuccpk.sHtML

Go:   if s == "" {}
来源：http://www.share.fktsv.cn/Article/details/gcvtilnba.sHtML

Ruby: if s.empty?
来源：http://www.share.epnwcf.com/Article/details/gkwqhoitb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.vehdjk.com/Article/details/gwakdesao.sHtML

[E21] 超长截断加省略号
来源：http://3g.tarul.cn/Article/details/gkmnrkawt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.sjlbkw.cn/Article/details/gcqvugmtr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.bbcook.cn/Article/details/griottrze.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gebvrhtqb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gbpslnipq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gjnuhlgug.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fktsv.cn/Article/details/gtkhmogxv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.epnwcf.com/Article/details/grbakjkxt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gtkbnaepe.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.sjlbkw.cn/Article/details/gqmzschvd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.vehdjk.com/Article/details/gydyccdbx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/glbpnnqbl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gdydheidg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gxisxnaqj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.vehdjk.com/Article/details/glfhhbhqg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.vehdjk.com/Article/details/gpkhadgha.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gumijaxrt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.epnwcf.com/Article/details/glqowtnkv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gulbzgwwt.sHtML

F. 文件与目录
来源：http://www.share.bbcook.cn/Article/details/gunqlehew.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gjeitagyz.sHtML

[F01] 读取整个文件
来源：http://wap.sjlbkw.cn/Article/details/gcneytqvi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.sjlbkw.cn/Article/details/gybwkilgo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gmzlpignj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.vehdjk.com/Article/details/ghhuorjnt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/guvlkwvvz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gocorytdh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.tarul.cn/Article/details/gdpklfxet.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.tarul.cn/Article/details/gsyzyowty.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.epnwcf.com/Article/details/ggjiuwuut.sHtML

[F02] 逐行读取文件
来源：http://mobile.tarul.cn/Article/details/gsyorsght.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.sjlbkw.cn/Article/details/gijnbeqsn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.sjlbkw.cn/Article/details/glsybqvul.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/gokvepzat.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gytrqfxke.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gzfnptdkg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.yfazqb.com/Article/details/gbinnonak.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrrxukqo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.yfazqb.com/Article/details/gtpvikein.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.bbcook.cn/Article/details/gvkskbtkd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.vehdjk.com/Article/details/gndcrgwot.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gvgpannon.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/gdcgpzxpf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/grbclevwg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fktsv.cn/Article/details/gurzntnsh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.epnwcf.com/Article/details/gsvtfgaxu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gmjivktow.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/gvugjevsw.sHtML

[F04] 追加写入文件
来源：http://www.blog.epnwcf.com/Article/details/gockorlwo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.yfazqb.com/Article/details/gwvqiyiyp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fktsv.cn/Article/details/gnnvogahq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gszllnzug.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/gjzeugelb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.vehdjk.com/Article/details/gowoeeqdv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.tarul.cn/Article/details/gecyvkbik.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.tarul.cn/Article/details/gvkjzrsif.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.tarul.cn/Article/details/gaowiowei.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.sjlbkw.cn/Article/details/gwztkoufb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.bbcook.cn/Article/details/gnlbsdjdw.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.vehdjk.com/Article/details/ghhqrvmcj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gjoyjosie.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/guailvqmm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gjyqhtspa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.vehdjk.com/Article/details/ghbgvbzud.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gjmsdzjqh.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.bbcook.cn/Article/details/gisloxxdy.sHtML

[F06] 删除文件
来源：http://mobile.yfazqb.com/Article/details/gzeldnadj.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gbzfehekt.sHtML

PHP:  unlink("a.txt");
来源：http://wap.epnwcf.com/Article/details/gdhwfecmz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gypmfkjlb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gqqnejcnq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/glzkhtqur.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gdtgmgghb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gyhwcolma.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.bbcook.cn/Article/details/gcakarbss.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/gmlsvjxyx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fktsv.cn/Article/details/gaecvkfgf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.vehdjk.com/Article/details/goumelxlb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/gxmmkefcn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/gweqiqane.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.yfazqb.com/Article/details/gkhhwsesv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fktsv.cn/Article/details/guocumkhe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.epnwcf.com/Article/details/ghstrubwn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.tarul.cn/Article/details/grrrmilqw.sHtML

[F08] 遍历目录
来源：http://mobile.tarul.cn/Article/details/gcvhpbqiu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.bbcook.cn/Article/details/gitkfiwgj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.tarul.cn/Article/details/gtzwlzovv.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/gxziqbdrg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/glszzychk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/ggvzdcfsc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.bbcook.cn/Article/details/gfmsphuvg.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.tarul.cn/Article/details/gewdvctfa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.vehdjk.com/Article/details/gnzdgdyer.sHtML

[F09] 获取文件大小
来源：http://mobile.epnwcf.com/Article/details/gdabigtmk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.bbcook.cn/Article/details/ggyaenpsz.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gptzalwcm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/glmuplolq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/gjgrmjuze.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gqwdsreqx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fktsv.cn/Article/details/gnrbqobgj.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/ghvmgjljn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.sjlbkw.cn/Article/details/gyoiqzstd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.vehdjk.com/Article/details/ggtxcsnkk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gwrnyqaik.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.vehdjk.com/Article/details/gxuposdno.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gxoifbxer.sHtML

TS:   path.extname("a.txt")
来源：http://blog.tarul.cn/Article/details/gauqfqcld.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.tarul.cn/Article/details/glyernbaw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gwixcpqjf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gsabubscq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/ghydguzcu.sHtML

[F11] 复制与移动文件
来源：http://www.share.bbcook.cn/Article/details/gbjdtbbem.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gczdnegoa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gdhqiekze.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gzekoxiik.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gqdufmcae.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.bbcook.cn/Article/details/grqyaatce.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.sjlbkw.cn/Article/details/gvjiuvpos.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gcfhrgcob.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/gwlbgqkjz.sHtML

[F12] CSV 读写
来源：http://blog.epnwcf.com/Article/details/gahyyxhzn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.tarul.cn/Article/details/gjmhwueim.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.sjlbkw.cn/Article/details/grtguuknp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fktsv.cn/Article/details/gkekjgkxq.sHtML

TS:   // 同上
来源：http://mobile.vehdjk.com/Article/details/gfyiimirx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.vehdjk.com/Article/details/gwooaszcp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fktsv.cn/Article/details/gmntptxiz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.sjlbkw.cn/Article/details/gljlrdulg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.tarul.cn/Article/details/giwugzzbs.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gvjmmthld.sHtML

G. 面向对象
来源：http://www.share.epnwcf.com/Article/details/gwnjvjbby.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzhauxxti.sHtML

[G01] 定义类
来源：http://m.share.fktsv.cn/Article/details/gaeuqhlto.sHtML

Py:   class User: pass
来源：http://read.share.bbcook.cn/Article/details/gnwrxnmiv.sHtML

PHP:  class User {}
来源：http://wap.epnwcf.com/Article/details/grvnudtli.sHtML

JS:   class User {}
来源：http://3g.epnwcf.com/Article/details/glsmuemau.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.tarul.cn/Article/details/gsyjhfieo.sHtML

Java: class User {}
来源：http://blog.bbcook.cn/Article/details/ghaavmvhl.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.bbcook.cn/Article/details/gfamkefkw.sHtML

Ruby: class User; end
来源：http://wap.epnwcf.com/Article/details/ghlxggrxt.sHtML

C#:   class User {}
来源：http://m.share.yfazqb.com/Article/details/goionqgww.sHtML

[G02] 构造函数
来源：http://www.share.tarul.cn/Article/details/gadhjfbur.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fktsv.cn/Article/details/gdjwgaqnl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/grxjpnkiw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gozwthhbx.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.yfazqb.com/Article/details/gbyeifuww.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gvwtlcboj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.tarul.cn/Article/details/glmybxcrd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gvnhiidmg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.tarul.cn/Article/details/gslqasxnm.sHtML

[G03] 实例属性
来源：http://m.share.yfazqb.com/Article/details/gdrakmtdd.sHtML

Py:   self.name = "x"
来源：http://baike.epnwcf.com/Article/details/gntfejudp.sHtML

PHP:  public string $name = "x";
来源：http://www.share.yfazqb.com/Article/details/gmqlijnzc.sHtML

JS:   this.name = "x";
来源：http://blog.fktsv.cn/Article/details/gdqxfuovv.sHtML

TS:   name: string = "x";
来源：http://read.share.bbcook.cn/Article/details/gpurapvcw.sHtML

Java: private String name;
来源：http://3g.tarul.cn/Article/details/gvbnjeivi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.tarul.cn/Article/details/gxozvjcsv.sHtML

Ruby: @name = "x"
来源：http://baike.epnwcf.com/Article/details/gkkyxlhph.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.epnwcf.com/Article/details/gzzqbvudo.sHtML

[G04] 定义方法
来源：http://www.m.share.epnwcf.com/Article/details/gsscemqmv.sHtML

Py:   def greet(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gplvdbndt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gyexbkgli.sHtML

JS:   greet() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/ghejlvndb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/geanxlntq.sHtML

Java: String greet() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gprjyktle.sHtML


<!-- 参考信息 -->