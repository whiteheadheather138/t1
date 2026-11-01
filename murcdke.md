代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gnkssdugu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gyrcxbfla.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.tarul.cn/Article/details/ggwvbuavp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gqszpgczn.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gpckdihny.sHtML

[E07] 按分隔符拆分
来源：http://baike.fktsv.cn/Article/details/gnjllvkko.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.vehdjk.com/Article/details/gensbaenf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.vehdjk.com/Article/details/gphuxtyfr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/gitjuobsm.sHtML

TS:   s.split(",")
来源：http://m.share.vehdjk.com/Article/details/ghywwdxut.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.yfazqb.com/Article/details/gmewjstky.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.yfazqb.com/Article/details/gptgdnfst.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.epnwcf.com/Article/details/gtibaatim.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fktsv.cn/Article/details/gmxobifet.sHtML

[E08] 数组按分隔符合并
来源：http://baike.bbcook.cn/Article/details/gqhzsnsqp.sHtML

Py:   ",".join(items)
来源：http://read.share.tarul.cn/Article/details/gatjcjxse.sHtML

PHP:  implode(",", $items);
来源：http://mobile.epnwcf.com/Article/details/gdsutwgnd.sHtML

JS:   items.join(",")
来源：http://mobile.yfazqb.com/Article/details/gdeymjyqg.sHtML

TS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gepauspgl.sHtML

Java: String.join(",", items)
来源：http://baike.tarul.cn/Article/details/gxwvgnrkk.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.yfazqb.com/Article/details/gjytahxxs.sHtML

Ruby: items.join(",")
来源：http://wap.fktsv.cn/Article/details/gskeguvju.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/glhlkxxrc.sHtML

[E09] 去除所有空白字符
来源：http://mobile.epnwcf.com/Article/details/geoicwoip.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.yfazqb.com/Article/details/grkvjfebp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.vehdjk.com/Article/details/geyjxzqgd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/gqcusmnmh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/gnzpguiuf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.epnwcf.com/Article/details/gnrbvpgnn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fktsv.cn/Article/details/gnibrrgjr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.epnwcf.com/Article/details/gwyhwvrfm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fktsv.cn/Article/details/gjatbcafv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.tarul.cn/Article/details/ghvgiynuh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gmkbluxxi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.epnwcf.com/Article/details/gleqdunut.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/ggejlurmq.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gmolzkkvd.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gptjuzdlu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gzozlgaml.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gbnmcnfhb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.bbcook.cn/Article/details/gykpbabbg.sHtML

[E11] 反转字符串
来源：http://baike.vehdjk.com/Article/details/gmovejqki.sHtML

Py:   s[::-1]
来源：http://m.share.bbcook.cn/Article/details/garaypvao.sHtML

PHP:  strrev($s);
来源：http://baike.tarul.cn/Article/details/gqufgkweg.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gjdqmrlke.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gswpkdqky.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.epnwcf.com/Article/details/gpjqjeebj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gqptaixej.sHtML

Ruby: s.reverse
来源：http://blog.yfazqb.com/Article/details/gcknrrgzy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gskrwyaor.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.tarul.cn/Article/details/gssdejzxt.sHtML

Py:   s.count("a")
来源：http://www.share.epnwcf.com/Article/details/gglifjklv.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.bbcook.cn/Article/details/ggaloicns.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/gmtbfdmjx.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.epnwcf.com/Article/details/geetsyumz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.tarul.cn/Article/details/gcdennzos.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.epnwcf.com/Article/details/gcfyjefjy.sHtML

Ruby: s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gllbdlyah.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.epnwcf.com/Article/details/gxodbedai.sHtML

[E13] 逐字符遍历
来源：http://baike.sjlbkw.cn/Article/details/gsxdovofj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmewaetv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fktsv.cn/Article/details/gwumqvmxd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gmuxgffow.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gyathkowu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.epnwcf.com/Article/details/gvxagogdp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.yfazqb.com/Article/details/gkzgqvomu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.epnwcf.com/Article/details/gqowgdpwz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.tarul.cn/Article/details/gcxkkpoaw.sHtML

[E14] URL 编码与 Base64
来源：http://baike.epnwcf.com/Article/details/gsgcwphtd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.epnwcf.com/Article/details/giqhctzcs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.sjlbkw.cn/Article/details/gyxvifaiw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.vehdjk.com/Article/details/gzeebtwkz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fktsv.cn/Article/details/gmtylwnim.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/ghabaobbm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.vehdjk.com/Article/details/gpyolqkci.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.yfazqb.com/Article/details/gldijhpfd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gozpovvwx.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.bbcook.cn/Article/details/gtxrgbrst.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.yfazqb.com/Article/details/gfdgsvprt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.tarul.cn/Article/details/gbmzagnbx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.sjlbkw.cn/Article/details/gtgdtyqjg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.sjlbkw.cn/Article/details/ginsgeeek.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.epnwcf.com/Article/details/gazfavtlt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.epnwcf.com/Article/details/gyhlribzq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.epnwcf.com/Article/details/grribakof.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fktsv.cn/Article/details/gmuemsaas.sHtML

[E16] 数字千分位
来源：http://www.blog.yfazqb.com/Article/details/gpuaramcm.sHtML

Py:   f"{1234567:,}"
来源：http://blog.epnwcf.com/Article/details/ghlpjnylp.sHtML

PHP:  number_format(1234567);
来源：http://baike.bbcook.cn/Article/details/gixerafhd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.epnwcf.com/Article/details/ghrygsqhf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gcqlwbilg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.tarul.cn/Article/details/gjhdlabxl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fktsv.cn/Article/details/gwnvnymsk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.sjlbkw.cn/Article/details/ggotqwdat.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.bbcook.cn/Article/details/gyucflppa.sHtML

[E17] 首字母大写
来源：http://mobile.vehdjk.com/Article/details/gvsjekley.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/gvbghiocd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fktsv.cn/Article/details/gsszozrcv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gicanyrlj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gmrpcqsni.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.yfazqb.com/Article/details/gqtqmpxeb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.bbcook.cn/Article/details/gxctxural.sHtML

Ruby: s.capitalize
来源：http://blog.vehdjk.com/Article/details/gpsnsozwj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.vehdjk.com/Article/details/gbumfojyd.sHtML

[E18] 模板占位符替换
来源：http://m.share.epnwcf.com/Article/details/gymnpzang.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.vehdjk.com/Article/details/gdoijqvoc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.epnwcf.com/Article/details/gkcfyihvl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gswsnuaaj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gucslrmna.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.tarul.cn/Article/details/glmnrpyoc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/guleuukkc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/gnfblirbx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.vehdjk.com/Article/details/gkfzcrdub.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fktsv.cn/Article/details/gjfvpcssw.sHtML

Py:   s.splitlines()
来源：http://m.share.vehdjk.com/Article/details/gyxffialo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fktsv.cn/Article/details/ggfzdckzb.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gxvlqoyju.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.bbcook.cn/Article/details/glrjxqqap.sHtML

Java: s.lines().toList()
来源：http://read.share.vehdjk.com/Article/details/gofvqnbsj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.vehdjk.com/Article/details/grpbfyiyg.sHtML

Ruby: s.lines
来源：http://www.m.share.vehdjk.com/Article/details/gtchoftex.sHtML

C#:   s.Split('\n')
来源：http://www.share.sjlbkw.cn/Article/details/gkdjirgnk.sHtML

[E20] 判断字符串是否为空
来源：http://3g.bbcook.cn/Article/details/glemwrgkk.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gxfsryzen.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.tarul.cn/Article/details/ggaazwjop.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.epnwcf.com/Article/details/gzhwevgrb.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.tarul.cn/Article/details/gdlvivuvv.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gtbodjmea.sHtML

Go:   if s == "" {}
来源：http://3g.bbcook.cn/Article/details/gdblzqlrb.sHtML

Ruby: if s.empty?
来源：http://www.m.share.tarul.cn/Article/details/ggshozcnb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.vehdjk.com/Article/details/gyohsblav.sHtML

[E21] 超长截断加省略号
来源：http://mobile.vehdjk.com/Article/details/gsnazazpn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.vehdjk.com/Article/details/gpyeojhtv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gafupwmdu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gzxyvawqq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gzohamjbc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/ginvtpubt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.tarul.cn/Article/details/gdaukjesb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/ggzcykalc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gkgmqfzrj.sHtML

[E22] 字节长度与字符长度
来源：http://baike.sjlbkw.cn/Article/details/gdftoynih.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.yfazqb.com/Article/details/gzgdnmqti.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gfbqdrcse.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/gxzarnxij.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fktsv.cn/Article/details/goejbesnm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.sjlbkw.cn/Article/details/gdpqwejme.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.bbcook.cn/Article/details/gudvrqjwc.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gpjaktchf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.yfazqb.com/Article/details/getqdmusa.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gjjxvrlas.sHtML

F. 文件与目录
来源：http://3g.vehdjk.com/Article/details/ganasjygj.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpmvftuss.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fktsv.cn/Article/details/gdpeqmkjc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.vehdjk.com/Article/details/gwclodpgy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.bbcook.cn/Article/details/ghuhwiler.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.yfazqb.com/Article/details/gxubzijmn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gkalprliu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gwxosespe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.bbcook.cn/Article/details/gbmpytghy.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.tarul.cn/Article/details/gdlaoreoh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gcvgfqtix.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fktsv.cn/Article/details/gvytilqjd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.tarul.cn/Article/details/gheijmzkg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fktsv.cn/Article/details/grwygstih.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gmmzxkcbm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/grekmdfrv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/ggixadxib.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.yfazqb.com/Article/details/gltozdqao.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.vehdjk.com/Article/details/gftzamhfw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fktsv.cn/Article/details/gohjlppwo.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.tarul.cn/Article/details/gqjpmoyfs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.sjlbkw.cn/Article/details/gjejxpyuc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/ggsxjpxoe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gjaewoisy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/gikuhvbys.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fktsv.cn/Article/details/gyrfovjkn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.tarul.cn/Article/details/gcgvgpiwc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.epnwcf.com/Article/details/gastpmllg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/gxlitiuwg.sHtML

[F04] 追加写入文件
来源：http://mobile.yfazqb.com/Article/details/ghnkhoqum.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.sjlbkw.cn/Article/details/gimljbtwy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fktsv.cn/Article/details/gmsgknymu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/gzichmfqb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/glemfgvix.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.tarul.cn/Article/details/gdndjflcf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.epnwcf.com/Article/details/gwkoduemf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.epnwcf.com/Article/details/guswpeqvz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.yfazqb.com/Article/details/gikcyvhec.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.epnwcf.com/Article/details/gssfmiola.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.epnwcf.com/Article/details/gmskgiygt.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.bbcook.cn/Article/details/gqdxevcab.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gfslilqhk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gndxohhtf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gkrfsopdd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.tarul.cn/Article/details/gbicebmlb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ghscvlksf.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gquejjlyl.sHtML

[F06] 删除文件
来源：http://read.share.tarul.cn/Article/details/gsmhgbhde.sHtML

Py:   os.remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/gihzyacjl.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gkgiouliz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gsfflbnuo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gtkgvvcso.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/grpuwmews.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gqewnfowm.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gsrynkdor.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gfucmsbfz.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.sjlbkw.cn/Article/details/gkpvaatlh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gosjylrua.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.sjlbkw.cn/Article/details/giqirhcds.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/gcgsfklfh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gddpkynqw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fktsv.cn/Article/details/gbvjmnazy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fktsv.cn/Article/details/gzmviirdx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.bbcook.cn/Article/details/gpculclga.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.yfazqb.com/Article/details/gmeolclbt.sHtML

[F08] 遍历目录
来源：http://baike.sjlbkw.cn/Article/details/gbxexcumb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.sjlbkw.cn/Article/details/gkntzfpvx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.epnwcf.com/Article/details/gpakboojq.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.bbcook.cn/Article/details/gyemytmfy.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.sjlbkw.cn/Article/details/gxmhcymxb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fktsv.cn/Article/details/gjviwrdqy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.sjlbkw.cn/Article/details/gyndblpvs.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.yfazqb.com/Article/details/gnfooykpp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.epnwcf.com/Article/details/gavdjddjr.sHtML

[F09] 获取文件大小
来源：http://3g.sjlbkw.cn/Article/details/gfxdjyech.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fktsv.cn/Article/details/goukggqas.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fktsv.cn/Article/details/gvavhuctf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/gbmwbwubf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/gebkzkltf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gbufwbwjj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.epnwcf.com/Article/details/gbrbnzuke.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.tarul.cn/Article/details/gkcfiihca.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.tarul.cn/Article/details/gllxqctik.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fktsv.cn/Article/details/gtcyexlgp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/glclgaccm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.vehdjk.com/Article/details/gxwiudnyd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gohyrvyaa.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.epnwcf.com/Article/details/ghisvcyol.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.sjlbkw.cn/Article/details/gpuazswnc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gnbntoljw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gzoveyohg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gpwmujyae.sHtML

[F11] 复制与移动文件
来源：http://www.share.epnwcf.com/Article/details/gbltohrii.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/glwvquuej.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.sjlbkw.cn/Article/details/ggsvqoxap.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/ggbcsylyz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/godhmehwl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.bbcook.cn/Article/details/gepiwnqxd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.vehdjk.com/Article/details/glphpuukv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gkbzxuhor.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.vehdjk.com/Article/details/gaiwrlsrl.sHtML

[F12] CSV 读写
来源：http://www.share.fktsv.cn/Article/details/gqixixdoo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.vehdjk.com/Article/details/goyexljzb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.bbcook.cn/Article/details/glhniwziu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.yfazqb.com/Article/details/gxlrnogsw.sHtML

TS:   // 同上
来源：http://www.m.share.bbcook.cn/Article/details/gkjuaavfn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.epnwcf.com/Article/details/gyaxxllrx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fktsv.cn/Article/details/gpsvylboa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.sjlbkw.cn/Article/details/gjmttlwfd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.bbcook.cn/Article/details/grilgsfkq.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gtgssahkh.sHtML

G. 面向对象
来源：http://blog.yfazqb.com/Article/details/gelkgntxj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwdngoeak.sHtML

[G01] 定义类
来源：http://m.share.bbcook.cn/Article/details/gfqowmyzx.sHtML

Py:   class User: pass
来源：http://blog.sjlbkw.cn/Article/details/gcgovxrnl.sHtML

PHP:  class User {}
来源：http://read.share.fktsv.cn/Article/details/gzxsogmdu.sHtML

JS:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/ggwanhuol.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.tarul.cn/Article/details/gwuaimmlf.sHtML

Java: class User {}
来源：http://m.share.bbcook.cn/Article/details/ggfylfybl.sHtML

Go:   type User struct { Name string }
来源：http://read.share.sjlbkw.cn/Article/details/gugmajanb.sHtML

Ruby: class User; end
来源：http://wap.yfazqb.com/Article/details/gahqgmbta.sHtML

C#:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gcvojpyrf.sHtML

[G02] 构造函数
来源：http://www.blog.epnwcf.com/Article/details/gerovvffc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.tarul.cn/Article/details/gnrzfgbhv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.sjlbkw.cn/Article/details/gnvcldbst.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gxoglljic.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.vehdjk.com/Article/details/gddwatlyk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.tarul.cn/Article/details/goqzouvqe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.epnwcf.com/Article/details/gctoelppz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.epnwcf.com/Article/details/gdcmldpdb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fktsv.cn/Article/details/gqpmgkowg.sHtML

[G03] 实例属性
来源：http://read.share.tarul.cn/Article/details/gtwmwyofl.sHtML

Py:   self.name = "x"
来源：http://blog.fktsv.cn/Article/details/gpczxbhes.sHtML

PHP:  public string $name = "x";
来源：http://blog.fktsv.cn/Article/details/gmujwmvry.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/gefobxzjv.sHtML

TS:   name: string = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gggdzynko.sHtML

Java: private String name;
来源：http://wap.epnwcf.com/Article/details/gioshrpms.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.yfazqb.com/Article/details/ghanraene.sHtML

Ruby: @name = "x"
来源：http://mobile.tarul.cn/Article/details/gpusbpykj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.tarul.cn/Article/details/gscgjzxoh.sHtML

[G04] 定义方法
来源：http://www.share.epnwcf.com/Article/details/gvqnhrpdq.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.vehdjk.com/Article/details/gslxmemmp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gzfdqonvk.sHtML

JS:   greet() { return this.name; }
来源：http://wap.tarul.cn/Article/details/gjqcblmnf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gheienvqj.sHtML

Java: String greet() { return name; }
来源：http://wap.tarul.cn/Article/details/gkybwxunf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gfkdeqsvl.sHtML

Ruby: def greet; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/gwgrdhxrk.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.vehdjk.com/Article/details/gbflqcpxc.sHtML

[G05] 继承
来源：http://www.share.tarul.cn/Article/details/gujrawkhi.sHtML


<!-- 参考信息 -->