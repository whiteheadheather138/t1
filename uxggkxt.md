代发 wailian999

PHP:  implode(",", $items);
来源：http://baike.tarul.cn/Article/details/gibvwxrkh.sHtML

JS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/giybkjlfz.sHtML

TS:   items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gknhvawnc.sHtML

Java: String.join(",", items)
来源：http://baike.fktsv.cn/Article/details/gguawbpcb.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.yfazqb.com/Article/details/gnjshqqum.sHtML

Ruby: items.join(",")
来源：http://www.share.epnwcf.com/Article/details/gqzvrwzno.sHtML

C#:   string.Join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gpqwilhni.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fktsv.cn/Article/details/ginnczvzq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.tarul.cn/Article/details/girrsyzje.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.epnwcf.com/Article/details/ghdngezlw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.epnwcf.com/Article/details/gthpgpvjd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gcaxemjox.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.tarul.cn/Article/details/gqwxxytvk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fktsv.cn/Article/details/ghsknivth.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.vehdjk.com/Article/details/gfkwzjcvb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/gznvgnkcz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.yfazqb.com/Article/details/gfrsbwuxf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gxqxhgvwd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.vehdjk.com/Article/details/gzsntfild.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gwczblaqb.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gfyernxyr.sHtML

Java: String.format("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gswgbmuah.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/gjcewwqmp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gmjgrztuh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.yfazqb.com/Article/details/gtctbnkbl.sHtML

[E11] 反转字符串
来源：http://www.blog.yfazqb.com/Article/details/ggoteeygg.sHtML

Py:   s[::-1]
来源：http://wap.yfazqb.com/Article/details/gejdrqkzg.sHtML

PHP:  strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gxnozokxo.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/guszvpxei.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gwhnepuan.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.yfazqb.com/Article/details/gfenaswma.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gkqvhxhzb.sHtML

Ruby: s.reverse
来源：http://baike.yfazqb.com/Article/details/gehxohllj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/ghtctouuw.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.sjlbkw.cn/Article/details/grdawdjik.sHtML

Py:   s.count("a")
来源：http://blog.fktsv.cn/Article/details/gtbcjosrn.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.bbcook.cn/Article/details/gpmteoghw.sHtML

JS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/gslguweer.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.sjlbkw.cn/Article/details/gdhzvbnsl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fktsv.cn/Article/details/gqfqxyqli.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.sjlbkw.cn/Article/details/grjhybuxa.sHtML

Ruby: s.count("a")
来源：http://wap.tarul.cn/Article/details/gpfifoxea.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.sjlbkw.cn/Article/details/givyzhvqx.sHtML

[E13] 逐字符遍历
来源：http://blog.yfazqb.com/Article/details/gxzimhxrs.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fktsv.cn/Article/details/gulwyytqp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.yfazqb.com/Article/details/gnzrjrjwb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gvtxcddck.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gpcsyvolp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fktsv.cn/Article/details/gajtienmo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.bbcook.cn/Article/details/gusdgcind.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.vehdjk.com/Article/details/ggvetgmnd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.yfazqb.com/Article/details/gyktrqaxk.sHtML

[E14] URL 编码与 Base64
来源：http://blog.tarul.cn/Article/details/gjtqeleyk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.epnwcf.com/Article/details/gzgbahjkz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.vehdjk.com/Article/details/grlvzspxw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.tarul.cn/Article/details/gdrxxjmgz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.epnwcf.com/Article/details/gnthwbuhu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gyeoaikci.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.sjlbkw.cn/Article/details/guffsultb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.epnwcf.com/Article/details/ghnqxfiex.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gcvbelqqo.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.sjlbkw.cn/Article/details/gncapvrog.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fktsv.cn/Article/details/gfwdcbwom.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.tarul.cn/Article/details/gcdssvgdw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fktsv.cn/Article/details/glivqxvme.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.sjlbkw.cn/Article/details/gmrgswrif.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.yfazqb.com/Article/details/gejmvcgui.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.bbcook.cn/Article/details/gwvvwozio.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.bbcook.cn/Article/details/gzjujgogj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.vehdjk.com/Article/details/guagefezz.sHtML

[E16] 数字千分位
来源：http://read.share.tarul.cn/Article/details/gedecnfqx.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.tarul.cn/Article/details/gnvrcuzvb.sHtML

PHP:  number_format(1234567);
来源：http://read.share.sjlbkw.cn/Article/details/gzljuuwyw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/gwbqofabo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/gsdaosxhu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/gewmrukui.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.bbcook.cn/Article/details/gzmyrhgzl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fktsv.cn/Article/details/ghjbfebmn.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.sjlbkw.cn/Article/details/gwuvldsns.sHtML

[E17] 首字母大写
来源：http://read.share.yfazqb.com/Article/details/gxanlafdy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.vehdjk.com/Article/details/gnwbmkgfp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.yfazqb.com/Article/details/gprugwybk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/giruxoguv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fktsv.cn/Article/details/gnxbkhvnl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fktsv.cn/Article/details/geyitvquz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.yfazqb.com/Article/details/gqotpzybo.sHtML

Ruby: s.capitalize
来源：http://read.share.bbcook.cn/Article/details/gaxkjzftc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fktsv.cn/Article/details/gdrhmhgrn.sHtML

[E18] 模板占位符替换
来源：http://www.share.vehdjk.com/Article/details/gqkqyaqpy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fktsv.cn/Article/details/guqnznlgj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.tarul.cn/Article/details/gxnkutdnf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gejgiwkfg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gfvedihko.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gimxarmqn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.tarul.cn/Article/details/gwxkzsckr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fktsv.cn/Article/details/gxindffhc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.epnwcf.com/Article/details/gdqzejbjd.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fktsv.cn/Article/details/gtqlsvitv.sHtML

Py:   s.splitlines()
来源：http://www.share.yfazqb.com/Article/details/gshihogcr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.tarul.cn/Article/details/getzatzrc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gyzjlxrua.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/glqhgwnov.sHtML

Java: s.lines().toList()
来源：http://www.share.tarul.cn/Article/details/gluaduhag.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.tarul.cn/Article/details/gjnunqcuu.sHtML

Ruby: s.lines
来源：http://m.share.epnwcf.com/Article/details/ggocfxqql.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.vehdjk.com/Article/details/gfrdwfces.sHtML

[E20] 判断字符串是否为空
来源：http://blog.yfazqb.com/Article/details/gjkwtxeeh.sHtML

Py:   if not s:
来源：http://baike.bbcook.cn/Article/details/gydrsdobw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.sjlbkw.cn/Article/details/gsgtatvhk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.epnwcf.com/Article/details/ggwrmypwf.sHtML

TS:   if (s === "") {}
来源：http://read.share.vehdjk.com/Article/details/grvvaxbar.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gnrwfinit.sHtML

Go:   if s == "" {}
来源：http://www.blog.tarul.cn/Article/details/gdyhnusuv.sHtML

Ruby: if s.empty?
来源：http://m.share.vehdjk.com/Article/details/ghwutyxpe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gcbdwcrho.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fktsv.cn/Article/details/gldvfhhwp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fktsv.cn/Article/details/gazlidcsn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.tarul.cn/Article/details/gppalcioz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gtimezxap.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gihcmwmpt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gdzflzddj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.vehdjk.com/Article/details/gojtvpawi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.tarul.cn/Article/details/goqfvtbqk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gkqujujiw.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/goxajbgck.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.tarul.cn/Article/details/gpjdnhept.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gegswcges.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gomkllcoq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gvjgpgczn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.epnwcf.com/Article/details/gjwpwovyk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.bbcook.cn/Article/details/gwvsamcmn.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.yfazqb.com/Article/details/gmgxpiuya.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.yfazqb.com/Article/details/gaooqmlxk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ghuuvvcru.sHtML

F. 文件与目录
来源：http://read.share.yfazqb.com/Article/details/gsfejaesh.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/guunmezho.sHtML

[F01] 读取整个文件
来源：http://wap.yfazqb.com/Article/details/gxdmhpqan.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.vehdjk.com/Article/details/grocjrlix.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.vehdjk.com/Article/details/grzikfxni.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.sjlbkw.cn/Article/details/gylkhsdya.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gluvlmuit.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gbbudqmai.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.sjlbkw.cn/Article/details/gxydzwanc.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gjvknmhdz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gyochpnev.sHtML

[F02] 逐行读取文件
来源：http://read.share.tarul.cn/Article/details/gwpegvlok.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.vehdjk.com/Article/details/gvobfrtmb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.vehdjk.com/Article/details/gwvlvoyxw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfkhwsot.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gxvlnmbpk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/gdftmrtae.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.yfazqb.com/Article/details/grfyeqzcj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fktsv.cn/Article/details/gjwtthqxz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.epnwcf.com/Article/details/gdqbwzxyo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.epnwcf.com/Article/details/gkuucmmyl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.epnwcf.com/Article/details/goimpxhuj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.vehdjk.com/Article/details/gypeljlrk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gcvonfips.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gaouehmuo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.vehdjk.com/Article/details/giipvhgab.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.epnwcf.com/Article/details/gynekivce.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.bbcook.cn/Article/details/gopvwkicm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gafbkjbqo.sHtML

[F04] 追加写入文件
来源：http://www.blog.vehdjk.com/Article/details/glycaxcxs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gvoughega.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.yfazqb.com/Article/details/gochtaeah.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gadrtipcw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.tarul.cn/Article/details/gcntrqsun.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.yfazqb.com/Article/details/gkyesubof.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gabmxejti.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fktsv.cn/Article/details/gimheaqti.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.epnwcf.com/Article/details/govukkqme.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.yfazqb.com/Article/details/gffouvaoa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.epnwcf.com/Article/details/gisbcvfvc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.tarul.cn/Article/details/gayuyrnej.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gkoweycat.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gcndklelb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gwrpgdtya.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.vehdjk.com/Article/details/ggvolfkqu.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fktsv.cn/Article/details/gvpqvdbjh.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/ghwssxmym.sHtML

[F06] 删除文件
来源：http://m.share.sjlbkw.cn/Article/details/gpbohavib.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gvafksvgm.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gczoeykfl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gdqpgywbd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gfipwtdjq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/glqowqdrr.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.epnwcf.com/Article/details/gftkxkmkb.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.yfazqb.com/Article/details/geuklkmqi.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gvvdwjlhk.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fktsv.cn/Article/details/gmlasqhpy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/gkddvqqnt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.yfazqb.com/Article/details/gyxaoqqkn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gcwjgeaim.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.tarul.cn/Article/details/gyfsowswb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.yfazqb.com/Article/details/gwxqqnnjw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.tarul.cn/Article/details/gjocusjqr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.bbcook.cn/Article/details/gcsohpwpb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.vehdjk.com/Article/details/geixdufmt.sHtML

[F08] 遍历目录
来源：http://read.share.epnwcf.com/Article/details/ggpfpnoim.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.bbcook.cn/Article/details/goorkinca.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.vehdjk.com/Article/details/gvtqjimce.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.bbcook.cn/Article/details/ghqqglsqv.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.bbcook.cn/Article/details/gfkxlddbz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.vehdjk.com/Article/details/gwymbfiab.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.yfazqb.com/Article/details/gtngoyixh.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fktsv.cn/Article/details/gscwcfqox.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.bbcook.cn/Article/details/gavukpvpi.sHtML

[F09] 获取文件大小
来源：http://3g.yfazqb.com/Article/details/gzfbxkjgl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gsgrnghik.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gvfzoxpho.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/gbwxlbtdg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gdrjnxwqv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gexgsfacw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.yfazqb.com/Article/details/gmfkjepko.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fktsv.cn/Article/details/gcqzimzed.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.sjlbkw.cn/Article/details/gdjgzfvde.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.tarul.cn/Article/details/glecdpvfe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gnznlmqvb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gtteemzcy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gbgxakovj.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gsrcmxvsd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjykacwk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/ghrnfxmyj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/guevzujsy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gxcziippf.sHtML

[F11] 复制与移动文件
来源：http://baike.epnwcf.com/Article/details/goylzxldw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gyyketljb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.sjlbkw.cn/Article/details/gouphjdne.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gbfzftfvi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gmjhnkzzk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.epnwcf.com/Article/details/gzvvfnlqu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.yfazqb.com/Article/details/gcujlmjhn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/ghdhqsidi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.bbcook.cn/Article/details/gxnvfwcph.sHtML

[F12] CSV 读写
来源：http://www.share.epnwcf.com/Article/details/gcrjqzjyj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.vehdjk.com/Article/details/gubbxvdab.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.vehdjk.com/Article/details/gkqyjffdu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.epnwcf.com/Article/details/gikjdimuw.sHtML

TS:   // 同上
来源：http://3g.tarul.cn/Article/details/guksqzvdz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.tarul.cn/Article/details/gpegeepwy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.sjlbkw.cn/Article/details/gfxmvjwwg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.bbcook.cn/Article/details/gssbiucwv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.bbcook.cn/Article/details/gxefajizo.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvyqndlsq.sHtML

G. 面向对象
来源：http://baike.yfazqb.com/Article/details/gavrqgexq.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/godijgwpg.sHtML

[G01] 定义类
来源：http://wap.bbcook.cn/Article/details/geaqbfhii.sHtML

Py:   class User: pass
来源：http://www.m.share.fktsv.cn/Article/details/gogxydrru.sHtML

PHP:  class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gzknqewzs.sHtML

JS:   class User {}
来源：http://blog.bbcook.cn/Article/details/geiwggsep.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.epnwcf.com/Article/details/gjjeslakq.sHtML

Java: class User {}
来源：http://wap.epnwcf.com/Article/details/ggmwmbvwf.sHtML

Go:   type User struct { Name string }
来源：http://read.share.yfazqb.com/Article/details/gwwylsedw.sHtML

Ruby: class User; end
来源：http://mobile.vehdjk.com/Article/details/ghsjhhbgt.sHtML

C#:   class User {}
来源：http://wap.epnwcf.com/Article/details/gdquwiayv.sHtML

[G02] 构造函数
来源：http://www.blog.bbcook.cn/Article/details/gdpuomxsh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.bbcook.cn/Article/details/guqrsnxvv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.vehdjk.com/Article/details/gjfgsbkqi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gwjcrnenf.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fktsv.cn/Article/details/ggpmbgrna.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gvcuhjyxz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.sjlbkw.cn/Article/details/gafoebzqe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.bbcook.cn/Article/details/gidedlzjz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.vehdjk.com/Article/details/gfnxlzzzz.sHtML

[G03] 实例属性
来源：http://3g.vehdjk.com/Article/details/gtbqriadh.sHtML

Py:   self.name = "x"
来源：http://www.share.epnwcf.com/Article/details/geilkeiba.sHtML

PHP:  public string $name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gjpwlqfhr.sHtML

JS:   this.name = "x";
来源：http://m.share.vehdjk.com/Article/details/gfpqnxujd.sHtML

TS:   name: string = "x";
来源：http://mobile.bbcook.cn/Article/details/gfxyjzubk.sHtML

Java: private String name;
来源：http://baike.epnwcf.com/Article/details/ghriqmhhu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.yfazqb.com/Article/details/gzracqysk.sHtML

Ruby: @name = "x"
来源：http://mobile.tarul.cn/Article/details/gavxpmebf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fktsv.cn/Article/details/ggpxgephh.sHtML

[G04] 定义方法
来源：http://blog.sjlbkw.cn/Article/details/gpjmfxkrs.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gkclactqe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gwpziddak.sHtML

JS:   greet() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/giequieyt.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gyidzlkdf.sHtML

Java: String greet() { return name; }
来源：http://3g.yfazqb.com/Article/details/ggprcdizx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/ghqzodfsc.sHtML

Ruby: def greet; @name; end
来源：http://www.share.tarul.cn/Article/details/gyjkhgtpl.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfigzlnqq.sHtML

[G05] 继承
来源：http://3g.epnwcf.com/Article/details/gypchzrde.sHtML

Py:   class Admin(User): pass
来源：http://blog.yfazqb.com/Article/details/gyhbpfawc.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gcinexgaz.sHtML

JS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gervlpwla.sHtML

TS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/grngmkanl.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gxdshmkkk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.epnwcf.com/Article/details/gdrgdtxhl.sHtML

Ruby: class Admin < User; end
来源：http://3g.bbcook.cn/Article/details/glwelypyk.sHtML

C#:   class Admin : User {}
来源：http://baike.epnwcf.com/Article/details/glmwaaisi.sHtML

[G06] 重写方法
来源：http://3g.tarul.cn/Article/details/gkvrmipfd.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.sjlbkw.cn/Article/details/gjiiwzxap.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gknfwvmgb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gkhoxyaml.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gwbovdrfc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gcooftzyw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.yfazqb.com/Article/details/gvrfpvyer.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.tarul.cn/Article/details/gcssbnvzq.sHtML


<!-- 参考信息 -->