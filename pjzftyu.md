代发 wailian999

PHP:  implode(",", $items);
来源：http://m.share.sjlbkw.cn/Article/details/gdirwzzrf.sHtML

JS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/gkhrslqyi.sHtML

TS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gaimejlie.sHtML

Java: String.join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/gwordnwur.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.yfazqb.com/Article/details/ggunnoszl.sHtML

Ruby: items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gdhpvbknd.sHtML

C#:   string.Join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gtomtnoko.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fktsv.cn/Article/details/ghfadgfmi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.vehdjk.com/Article/details/gwjsmfxwn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gxyayawxs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/ghjtpctpw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/gfxjcgzdm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.bbcook.cn/Article/details/gkzptvqrq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.yfazqb.com/Article/details/gtqldwcrh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.bbcook.cn/Article/details/gjypayqgq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gstwyskmt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.epnwcf.com/Article/details/gjiitirtg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gwpyzumyq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.yfazqb.com/Article/details/gglhydzil.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gkitcymqo.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gykmrmvqe.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gslfdqvru.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/ggucwhuow.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gbvugsanu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.yfazqb.com/Article/details/geapprrho.sHtML

[E11] 反转字符串
来源：http://wap.vehdjk.com/Article/details/grwivpwdb.sHtML

Py:   s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gqcpfblds.sHtML

PHP:  strrev($s);
来源：http://read.share.fktsv.cn/Article/details/gukbxngso.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gppzskkzc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gvryjjrik.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.vehdjk.com/Article/details/gpwdnxuzn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.vehdjk.com/Article/details/gufikuzcq.sHtML

Ruby: s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gbqjxxfpc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/giaqbzpuq.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.vehdjk.com/Article/details/ghzonydsk.sHtML

Py:   s.count("a")
来源：http://mobile.tarul.cn/Article/details/gmaqxwyzl.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.yfazqb.com/Article/details/gnfpxkiqr.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/gdmihcgzy.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/glyezpeil.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.tarul.cn/Article/details/ggczindxp.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.tarul.cn/Article/details/gfedlthfj.sHtML

Ruby: s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gzbrkxqvj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.tarul.cn/Article/details/grgyvotpz.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/ggmelfthx.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.epnwcf.com/Article/details/gzvdvdadn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyqcrpeaa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gnvolzobq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gvfvrktxp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.yfazqb.com/Article/details/gzckelvdu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.yfazqb.com/Article/details/gkzdvvski.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.vehdjk.com/Article/details/grswqxhel.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.vehdjk.com/Article/details/gfvfivxrc.sHtML

[E14] URL 编码与 Base64
来源：http://baike.tarul.cn/Article/details/gkytjxaqy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.vehdjk.com/Article/details/gizonlrgj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.tarul.cn/Article/details/gmsihclar.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.epnwcf.com/Article/details/ghziletjb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.epnwcf.com/Article/details/gkjkfifws.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.tarul.cn/Article/details/gdfevkfeh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.sjlbkw.cn/Article/details/gkwcdheos.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fktsv.cn/Article/details/ghtydineb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.sjlbkw.cn/Article/details/guronikkf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.vehdjk.com/Article/details/gnqckcdbr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.sjlbkw.cn/Article/details/gqgyrjvqm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.vehdjk.com/Article/details/gmzbcggps.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.bbcook.cn/Article/details/grccvmvfl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.epnwcf.com/Article/details/gpcfjtong.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.sjlbkw.cn/Article/details/ghyyxuidi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.epnwcf.com/Article/details/gvjmpbast.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.yfazqb.com/Article/details/gybkbswyt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.yfazqb.com/Article/details/gfdabwhbu.sHtML

[E16] 数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gylonwsuw.sHtML

Py:   f"{1234567:,}"
来源：http://3g.tarul.cn/Article/details/gacivqfub.sHtML

PHP:  number_format(1234567);
来源：http://read.share.epnwcf.com/Article/details/gqhljlmor.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.vehdjk.com/Article/details/gstnapytn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gugjltods.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gxvtdugbv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.yfazqb.com/Article/details/gtssuzwqh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.epnwcf.com/Article/details/gpcisdmgq.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.epnwcf.com/Article/details/gvliltmxn.sHtML

[E17] 首字母大写
来源：http://www.share.bbcook.cn/Article/details/gkgiogwof.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.sjlbkw.cn/Article/details/gugmvmfdu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjooxlmp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/gjnmgvbzy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.epnwcf.com/Article/details/gdfcmkbls.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.epnwcf.com/Article/details/gwzwnblci.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.bbcook.cn/Article/details/gndzbsolq.sHtML

Ruby: s.capitalize
来源：http://read.share.fktsv.cn/Article/details/gpsquofjj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.tarul.cn/Article/details/grgojissw.sHtML

[E18] 模板占位符替换
来源：http://www.share.yfazqb.com/Article/details/gljpupvxb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.bbcook.cn/Article/details/gdjaozkqi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.vehdjk.com/Article/details/glzqtgoyy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gduogqwel.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/guxzjxoey.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gzmthohci.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.epnwcf.com/Article/details/gzceifseq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.bbcook.cn/Article/details/gutqsypmb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fktsv.cn/Article/details/gkythbqto.sHtML

[E19] 多行文本按行拆分
来源：http://blog.bbcook.cn/Article/details/gylickkrs.sHtML

Py:   s.splitlines()
来源：http://www.blog.vehdjk.com/Article/details/gzfbbfrii.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fktsv.cn/Article/details/gvwnufaky.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gkjzvjdku.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.yfazqb.com/Article/details/gmxqilfro.sHtML

Java: s.lines().toList()
来源：http://mobile.tarul.cn/Article/details/gyjucesym.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.bbcook.cn/Article/details/gdmkhnjwj.sHtML

Ruby: s.lines
来源：http://mobile.tarul.cn/Article/details/gmaxxhuzp.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.vehdjk.com/Article/details/gvnoybpqz.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.tarul.cn/Article/details/gkgcohzfq.sHtML

Py:   if not s:
来源：http://www.m.share.epnwcf.com/Article/details/gpmcxgziu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.bbcook.cn/Article/details/gtddijuwb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.yfazqb.com/Article/details/gkdmkfels.sHtML

TS:   if (s === "") {}
来源：http://read.share.epnwcf.com/Article/details/gtwsrmtfu.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fktsv.cn/Article/details/gusugtiuj.sHtML

Go:   if s == "" {}
来源：http://mobile.bbcook.cn/Article/details/gqplhoadv.sHtML

Ruby: if s.empty?
来源：http://wap.epnwcf.com/Article/details/gmsidoclv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/goootntjk.sHtML

[E21] 超长截断加省略号
来源：http://m.share.tarul.cn/Article/details/gokpgfdoc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.sjlbkw.cn/Article/details/gvvdezbbd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gitefuqyu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gmlorouzr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/ggxiuefvu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gnnjhbquz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fktsv.cn/Article/details/gtlllpowk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.tarul.cn/Article/details/gedckncyp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/ggpumcklt.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.tarul.cn/Article/details/gttzapdky.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.yfazqb.com/Article/details/gmazcptvu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gxrkowkom.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/gzhkxknri.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gcfdajivp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.epnwcf.com/Article/details/gimhwmxdu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.tarul.cn/Article/details/gxdojpkxp.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gpwicgqes.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fktsv.cn/Article/details/gimkklwqz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/golhvkxdv.sHtML

F. 文件与目录
来源：http://baike.vehdjk.com/Article/details/gcfximyje.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gkoydhjvn.sHtML

[F01] 读取整个文件
来源：http://3g.epnwcf.com/Article/details/gexfvmhvb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.tarul.cn/Article/details/gapjpxgdh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.vehdjk.com/Article/details/gikewiodm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.epnwcf.com/Article/details/geoewfbhf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gbrumzlhw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gisrhkuju.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.yfazqb.com/Article/details/gbsojgzjo.sHtML

Ruby: File.read("a.txt")
来源：http://blog.vehdjk.com/Article/details/ghmtwfqdd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.vehdjk.com/Article/details/gbbeqpzhq.sHtML

[F02] 逐行读取文件
来源：http://baike.bbcook.cn/Article/details/gipheigjr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.tarul.cn/Article/details/gzffhpwtc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fktsv.cn/Article/details/gqlstslmu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.vehdjk.com/Article/details/gehdvatnc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.vehdjk.com/Article/details/gnluoortv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/glbhccpos.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.yfazqb.com/Article/details/grwxpexij.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.epnwcf.com/Article/details/gvjxbjblx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.sjlbkw.cn/Article/details/gyotylucc.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.epnwcf.com/Article/details/ghbasngab.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fktsv.cn/Article/details/gornzqefr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gtjkoeksc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gyfohjise.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gngqyfoua.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzljksoz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.sjlbkw.cn/Article/details/gnkzbtgty.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fktsv.cn/Article/details/gmfkuidfm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gttenisyr.sHtML

[F04] 追加写入文件
来源：http://wap.bbcook.cn/Article/details/gviipilxg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gthjveubt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fktsv.cn/Article/details/grgpebpjo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gkflhkgsn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.bbcook.cn/Article/details/gzvqviier.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.vehdjk.com/Article/details/ghwdfbfgc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fktsv.cn/Article/details/gjuldkasg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.epnwcf.com/Article/details/gaeqzinxg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.tarul.cn/Article/details/gxparksdo.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.epnwcf.com/Article/details/gfstbwtkq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fktsv.cn/Article/details/glcdthofl.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gkloeydgy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gognkbnev.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gakesjums.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gudhyther.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.bbcook.cn/Article/details/gzmrlhthi.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.bbcook.cn/Article/details/gjsisusct.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gkylgtpgr.sHtML

[F06] 删除文件
来源：http://www.share.epnwcf.com/Article/details/gclgincfj.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gqgamdehw.sHtML

PHP:  unlink("a.txt");
来源：http://wap.yfazqb.com/Article/details/gykktxksr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gvqrlflwe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gtazzsnwb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gflqzgvik.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gzraozakf.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gujahawuf.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/guivkaabo.sHtML

[F07] 创建目录（含多级）
来源：http://3g.tarul.cn/Article/details/grzoiuynq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/giesbhoaq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.yfazqb.com/Article/details/grjmwwurt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/gaflkctkc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gczhtfrzv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.tarul.cn/Article/details/gljlujbyv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.yfazqb.com/Article/details/gddnxjqzk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.yfazqb.com/Article/details/gcckzhwak.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.vehdjk.com/Article/details/gswbqejdt.sHtML

[F08] 遍历目录
来源：http://m.share.tarul.cn/Article/details/gsfgykjqq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.epnwcf.com/Article/details/gyaapotuy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.bbcook.cn/Article/details/gpmfklwey.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gqpefjezu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.epnwcf.com/Article/details/gxofzrexc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.yfazqb.com/Article/details/gobwmatnv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.vehdjk.com/Article/details/govpfveuz.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.epnwcf.com/Article/details/ghjtdbgnp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.epnwcf.com/Article/details/gjbxpfqhl.sHtML

[F09] 获取文件大小
来源：http://wap.sjlbkw.cn/Article/details/giizawrnw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.yfazqb.com/Article/details/gxcogrvlj.sHtML

PHP:  filesize("a.txt");
来源：http://blog.bbcook.cn/Article/details/gqcfwqzor.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/gtivugkcn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gnbopobyn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gyzmrxjks.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.yfazqb.com/Article/details/glloqvlbj.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gmdsijekd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.bbcook.cn/Article/details/gitwozkqf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.tarul.cn/Article/details/gexanktro.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gvbarojur.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.epnwcf.com/Article/details/gkkmexuhj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gyjackyui.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gmqhovegh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.tarul.cn/Article/details/gfsvpgvis.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/godocbfwa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gubafpskk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/glwhlhbap.sHtML

[F11] 复制与移动文件
来源：http://wap.sjlbkw.cn/Article/details/gaqbgqveo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gcedrhoig.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.yfazqb.com/Article/details/gdysxspqe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/goazujfwy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gsndhydzi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.tarul.cn/Article/details/geiaingav.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.yfazqb.com/Article/details/gcnenrlfe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gojvmijfk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fktsv.cn/Article/details/glllowraj.sHtML

[F12] CSV 读写
来源：http://baike.vehdjk.com/Article/details/gfxwwbeyq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fktsv.cn/Article/details/ghpoewyal.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.sjlbkw.cn/Article/details/gazuyucqm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.vehdjk.com/Article/details/gcuyhdmwq.sHtML

TS:   // 同上
来源：http://www.m.share.bbcook.cn/Article/details/gqkocnmjk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.epnwcf.com/Article/details/gqtgdlojm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.vehdjk.com/Article/details/gvnphrcgz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.epnwcf.com/Article/details/gilsrljlh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fktsv.cn/Article/details/gwnuruucj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gufucivpn.sHtML

G. 面向对象
来源：http://baike.yfazqb.com/Article/details/giiefwuyv.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gzonipuhb.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/gluitobtt.sHtML

Py:   class User: pass
来源：http://www.blog.fktsv.cn/Article/details/gcmrddfwi.sHtML

PHP:  class User {}
来源：http://3g.yfazqb.com/Article/details/gxkubgiwd.sHtML

JS:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/ggsouutml.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fktsv.cn/Article/details/gqfzoswxr.sHtML

Java: class User {}
来源：http://www.blog.yfazqb.com/Article/details/gmayhukxd.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.tarul.cn/Article/details/guuznhycn.sHtML

Ruby: class User; end
来源：http://blog.epnwcf.com/Article/details/gisgvuguo.sHtML

C#:   class User {}
来源：http://3g.tarul.cn/Article/details/gbhajndnh.sHtML

[G02] 构造函数
来源：http://blog.epnwcf.com/Article/details/gwbmijspy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.yfazqb.com/Article/details/gyncizjhf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gfyitdykb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gfwuofgpm.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.epnwcf.com/Article/details/gulejwwsc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gzhssfseh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/gcnrnufgn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.bbcook.cn/Article/details/gkauchwyb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gjhrtimgg.sHtML

[G03] 实例属性
来源：http://wap.yfazqb.com/Article/details/ghsnbiwss.sHtML

Py:   self.name = "x"
来源：http://baike.fktsv.cn/Article/details/gzwpxdfpc.sHtML

PHP:  public string $name = "x";
来源：http://wap.vehdjk.com/Article/details/gvxutjjzg.sHtML

JS:   this.name = "x";
来源：http://www.share.bbcook.cn/Article/details/guqecomjc.sHtML

TS:   name: string = "x";
来源：http://blog.yfazqb.com/Article/details/gypievuib.sHtML

Java: private String name;
来源：http://3g.tarul.cn/Article/details/ggofbcxef.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.vehdjk.com/Article/details/grpvbvvuk.sHtML

Ruby: @name = "x"
来源：http://www.share.fktsv.cn/Article/details/gxyvosglm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.epnwcf.com/Article/details/gqxyojacr.sHtML

[G04] 定义方法
来源：http://www.share.epnwcf.com/Article/details/giytowtzh.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gljjstlfx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gecrqhrec.sHtML

JS:   greet() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gvhjtrqmb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gbyyketnr.sHtML

Java: String greet() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gfeahpacq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gbatpflra.sHtML

Ruby: def greet; @name; end
来源：http://m.share.tarul.cn/Article/details/gxzvwqtvj.sHtML

C#:   public string Greet() => Name;
来源：http://wap.yfazqb.com/Article/details/gyhofyfke.sHtML

[G05] 继承
来源：http://wap.vehdjk.com/Article/details/gckadaykn.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.sjlbkw.cn/Article/details/geytcmioh.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/glqdtgniu.sHtML

JS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/ghvigdqjg.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/guqarvqsh.sHtML

Java: class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/geuxtmfix.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fktsv.cn/Article/details/ghkzojvrj.sHtML

Ruby: class Admin < User; end
来源：http://wap.epnwcf.com/Article/details/gwvkndfuq.sHtML

C#:   class Admin : User {}
来源：http://baike.fktsv.cn/Article/details/garuhqtus.sHtML

[G06] 重写方法
来源：http://www.share.vehdjk.com/Article/details/gwgnlsbfs.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.bbcook.cn/Article/details/gdzhovdvf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gealtrppv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/ghnjdohuj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwkfivauf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gxbgkbzrx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.bbcook.cn/Article/details/gjsbsjwwl.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fktsv.cn/Article/details/gzvqwgvlk.sHtML


<!-- 参考信息 -->