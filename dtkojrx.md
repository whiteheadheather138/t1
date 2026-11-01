代发 wailian999

JS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gepkecnzq.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/grfpsujtr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.yfazqb.com/Article/details/gwsjavgqq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.tarul.cn/Article/details/gqlfolvji.sHtML

Ruby: s.reverse
来源：http://www.share.bbcook.cn/Article/details/gvsgwpxhh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gptfrzsut.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.vehdjk.com/Article/details/gwddgdffm.sHtML

Py:   s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gigcchype.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.bbcook.cn/Article/details/gfussnvbd.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/gkkmnwjcm.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/gbbkmfzfu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.bbcook.cn/Article/details/ggskyhfni.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.yfazqb.com/Article/details/ghapnkodr.sHtML

Ruby: s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gdhrvkdkr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.sjlbkw.cn/Article/details/gnjugpsno.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/gxjsmgldx.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.epnwcf.com/Article/details/gdmjrtnyb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.epnwcf.com/Article/details/gbgddhimm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gjvcwmrdd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.tarul.cn/Article/details/gkzcgkiyd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.yfazqb.com/Article/details/gbdytofpj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.vehdjk.com/Article/details/gdttibfzz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.tarul.cn/Article/details/gxbznqygm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.epnwcf.com/Article/details/gqjrrejkh.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.tarul.cn/Article/details/gtilttjsv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.sjlbkw.cn/Article/details/gsssjgazz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbzlsqjm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.bbcook.cn/Article/details/gpcwgqmbm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.sjlbkw.cn/Article/details/gprnwhynm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.epnwcf.com/Article/details/gahccrbpz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fktsv.cn/Article/details/gezsanbqf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fktsv.cn/Article/details/gpxnowhbq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.yfazqb.com/Article/details/gizqznbwz.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.vehdjk.com/Article/details/gvmesfciy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.tarul.cn/Article/details/gajqmawkj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.yfazqb.com/Article/details/gxpnztejn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.epnwcf.com/Article/details/gbxlxablq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/gezltdczi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.vehdjk.com/Article/details/gspwwzdzu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gtilltylo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fktsv.cn/Article/details/gwirsxgqf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fktsv.cn/Article/details/gwnferkwt.sHtML

[E16] 数字千分位
来源：http://m.share.vehdjk.com/Article/details/gpvmvrzon.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.yfazqb.com/Article/details/gbykorwcr.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fktsv.cn/Article/details/grfvqwugt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.bbcook.cn/Article/details/gvtdgdofs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/gwckbmwaa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.bbcook.cn/Article/details/gxakuwitk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fktsv.cn/Article/details/gaaghpbeb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.tarul.cn/Article/details/gnddjxkkg.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.tarul.cn/Article/details/gykcdoyrl.sHtML

[E17] 首字母大写
来源：http://m.share.epnwcf.com/Article/details/gacherusy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.vehdjk.com/Article/details/gzlccztba.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fktsv.cn/Article/details/gacbzhsxn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/giqvrqtiz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/getltkvsl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.bbcook.cn/Article/details/gimevkxyz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.sjlbkw.cn/Article/details/gvrilrgmv.sHtML

Ruby: s.capitalize
来源：http://blog.vehdjk.com/Article/details/gmofimjby.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fktsv.cn/Article/details/gxtmluazc.sHtML

[E18] 模板占位符替换
来源：http://read.share.bbcook.cn/Article/details/gynyfvonr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.vehdjk.com/Article/details/gwfxqglvl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fktsv.cn/Article/details/gffrxtqhs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gthxlnxrf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gcbbzzdli.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gkfmqvitd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gmzridfnq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.yfazqb.com/Article/details/gsjlirkkx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gctjqgxgw.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fktsv.cn/Article/details/gxwxkjlob.sHtML

Py:   s.splitlines()
来源：http://mobile.sjlbkw.cn/Article/details/ghxxfktrr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.tarul.cn/Article/details/gjerhdiqf.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.sjlbkw.cn/Article/details/gpuacqejp.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gmbxxoxpu.sHtML

Java: s.lines().toList()
来源：http://m.share.bbcook.cn/Article/details/gwbukmair.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmznfxga.sHtML

Ruby: s.lines
来源：http://mobile.bbcook.cn/Article/details/glpbcxsmr.sHtML

C#:   s.Split('\n')
来源：http://read.share.vehdjk.com/Article/details/gtuiicmre.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fktsv.cn/Article/details/geuajolpe.sHtML

Py:   if not s:
来源：http://mobile.fktsv.cn/Article/details/gawnbhcwh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fktsv.cn/Article/details/gwzayudjr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.epnwcf.com/Article/details/gvjimssdt.sHtML

TS:   if (s === "") {}
来源：http://mobile.sjlbkw.cn/Article/details/ggrliyvnn.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/gglftgsjm.sHtML

Go:   if s == "" {}
来源：http://www.m.share.tarul.cn/Article/details/ggsynqsrb.sHtML

Ruby: if s.empty?
来源：http://3g.epnwcf.com/Article/details/gniyhgbpg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.bbcook.cn/Article/details/gkywfohrc.sHtML

[E21] 超长截断加省略号
来源：http://m.share.bbcook.cn/Article/details/gwwmnczlb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fktsv.cn/Article/details/gvkawocga.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gffgahwuu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gpfxvuiii.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gejdkkzyv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/grbdgjfep.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.bbcook.cn/Article/details/gvisqexar.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gyuaiaain.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/ghvepeekt.sHtML

[E22] 字节长度与字符长度
来源：http://baike.tarul.cn/Article/details/ghbtyzahe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.epnwcf.com/Article/details/gnsammkko.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gwahghuew.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gtrcneyyp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/gkstzkjfy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.epnwcf.com/Article/details/ghrlugqcu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.bbcook.cn/Article/details/gwudhttvk.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.epnwcf.com/Article/details/guctlpsgb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.sjlbkw.cn/Article/details/glvifblnr.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnvfubkfp.sHtML

F. 文件与目录
来源：http://www.blog.vehdjk.com/Article/details/grybukkoz.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gexdvrdwa.sHtML

[F01] 读取整个文件
来源：http://3g.tarul.cn/Article/details/gjtzqaedz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fktsv.cn/Article/details/gfmaampge.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gnzwvqcvx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.bbcook.cn/Article/details/gofmalcjw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gvwqinbkg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gvqcwalfo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.sjlbkw.cn/Article/details/gznyyykqd.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gxsewqqsy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.tarul.cn/Article/details/ghvuuuwsj.sHtML

[F02] 逐行读取文件
来源：http://wap.yfazqb.com/Article/details/gjlsuojfv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.epnwcf.com/Article/details/gpmrwbnnn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.epnwcf.com/Article/details/goizdhjmw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/gqcylkfkz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gbjyccaon.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.bbcook.cn/Article/details/gularsxgw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.tarul.cn/Article/details/gatzdbrpc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.yfazqb.com/Article/details/gnluitino.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.epnwcf.com/Article/details/gkxbufild.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.tarul.cn/Article/details/gclbujctn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzyfhedd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gokcdensd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/glqbplpan.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gbstyjmgn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.bbcook.cn/Article/details/ghatryclm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/gvhhdyrqo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gbdwaelej.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gqbqzlgjn.sHtML

[F04] 追加写入文件
来源：http://blog.sjlbkw.cn/Article/details/gozjhqffu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.tarul.cn/Article/details/glfajxhap.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.yfazqb.com/Article/details/gntnejqgw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.tarul.cn/Article/details/ghpbfxdpd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/ghwqunbyr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.sjlbkw.cn/Article/details/gzoihjrwk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.yfazqb.com/Article/details/ghmcqqltj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.epnwcf.com/Article/details/goqzizvid.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.epnwcf.com/Article/details/gtgjqsybn.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.yfazqb.com/Article/details/gqptpypfi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.yfazqb.com/Article/details/gamhaagjc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gcpbvansb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/giommtxfh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gwnbjdlhe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/glucfazkf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.yfazqb.com/Article/details/gunsllsbs.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.epnwcf.com/Article/details/ginfflqgf.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.vehdjk.com/Article/details/gvhzcemzt.sHtML

[F06] 删除文件
来源：http://read.share.tarul.cn/Article/details/gogxwmdpg.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gdoutvazg.sHtML

PHP:  unlink("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gihcfknxr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/guffdydpj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gubdyhyrk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gdymhdurg.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gpomwgogd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.tarul.cn/Article/details/ggvofptjx.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gayfpuics.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.bbcook.cn/Article/details/glrqkhrej.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/grdkghmvp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.epnwcf.com/Article/details/gysblgqnm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/ggyegrmkd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gglegioyi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.epnwcf.com/Article/details/gomcurxis.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.epnwcf.com/Article/details/gcxxdqtcw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.sjlbkw.cn/Article/details/guzzvfnnb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/genewobbi.sHtML

[F08] 遍历目录
来源：http://www.share.sjlbkw.cn/Article/details/gvjlbvgzt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.bbcook.cn/Article/details/gysanndzg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.tarul.cn/Article/details/gwhqyluoq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gnxpdwbnp.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/grjefxdtd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gctohzedj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.bbcook.cn/Article/details/gzliyiemr.sHtML

Ruby: Dir.children("dir")
来源：http://baike.epnwcf.com/Article/details/gdjydbtbz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fktsv.cn/Article/details/gddjlwgtq.sHtML

[F09] 获取文件大小
来源：http://blog.epnwcf.com/Article/details/gnkhrdfwf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gktlhkccc.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gmfncfqzq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.vehdjk.com/Article/details/gwxpgzrnb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/gwbeqzayh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gobyceaqn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.sjlbkw.cn/Article/details/gphesyonq.sHtML

Ruby: File.size("a.txt")
来源：http://wap.epnwcf.com/Article/details/gsxmlejco.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.epnwcf.com/Article/details/grniuvuis.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fktsv.cn/Article/details/gwthfekxg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/grtewnyzf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gkxrvavlp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gbgkgjdkb.sHtML

TS:   path.extname("a.txt")
来源：http://baike.vehdjk.com/Article/details/gyrqpnvmg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fktsv.cn/Article/details/gliiawptt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gwguqvsjz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gizayycgs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gjcexlnaw.sHtML

[F11] 复制与移动文件
来源：http://read.share.epnwcf.com/Article/details/gwrbosxgf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gbgvmaqah.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fktsv.cn/Article/details/grwvyxwpp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/grjkakuko.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gonrgxywx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fktsv.cn/Article/details/geyesoxcp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.yfazqb.com/Article/details/gxafmjwlc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/ggadbqmcx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.epnwcf.com/Article/details/gohloldag.sHtML

[F12] CSV 读写
来源：http://www.m.share.bbcook.cn/Article/details/gwdvmfjdf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.bbcook.cn/Article/details/gzmundgla.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.epnwcf.com/Article/details/gsdfarvqp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.bbcook.cn/Article/details/gqbycauvy.sHtML

TS:   // 同上
来源：http://blog.epnwcf.com/Article/details/gdrjxoecs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.yfazqb.com/Article/details/ggjedngfz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fktsv.cn/Article/details/gssctdsjg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.tarul.cn/Article/details/gkkmppcza.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.sjlbkw.cn/Article/details/grtlhdqlc.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gcdkujtfi.sHtML

G. 面向对象
来源：http://blog.epnwcf.com/Article/details/grtgeumdo.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gsoxjjozv.sHtML

[G01] 定义类
来源：http://m.share.sjlbkw.cn/Article/details/gxrtuxtjp.sHtML

Py:   class User: pass
来源：http://wap.epnwcf.com/Article/details/gwvhblejn.sHtML

PHP:  class User {}
来源：http://www.blog.yfazqb.com/Article/details/gnovdniyi.sHtML

JS:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gfnhgshml.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.yfazqb.com/Article/details/gmhbrhctg.sHtML

Java: class User {}
来源：http://blog.epnwcf.com/Article/details/gxftcfzcc.sHtML

Go:   type User struct { Name string }
来源：http://3g.bbcook.cn/Article/details/gawavyawd.sHtML

Ruby: class User; end
来源：http://baike.yfazqb.com/Article/details/garphqyoc.sHtML

C#:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gyyuxihzd.sHtML

[G02] 构造函数
来源：http://3g.yfazqb.com/Article/details/gmswwkbfo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.bbcook.cn/Article/details/gmaqscydi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.epnwcf.com/Article/details/ggkvapusy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gpqnngjbc.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.epnwcf.com/Article/details/grfopujyw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gktkglulw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.vehdjk.com/Article/details/gzjnzkfhg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.vehdjk.com/Article/details/gfpkgvrub.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.bbcook.cn/Article/details/glvwelcsz.sHtML

[G03] 实例属性
来源：http://m.share.yfazqb.com/Article/details/grcymalmj.sHtML

Py:   self.name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/gtqxlwgbr.sHtML

PHP:  public string $name = "x";
来源：http://www.share.bbcook.cn/Article/details/gaxoykpcf.sHtML

JS:   this.name = "x";
来源：http://3g.bbcook.cn/Article/details/gazuprkkf.sHtML

TS:   name: string = "x";
来源：http://3g.vehdjk.com/Article/details/gnvnjdeti.sHtML

Java: private String name;
来源：http://mobile.vehdjk.com/Article/details/gjxtvxnfg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.sjlbkw.cn/Article/details/gndmduqhf.sHtML

Ruby: @name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gylmwnnyv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.bbcook.cn/Article/details/gtlvphhmv.sHtML

[G04] 定义方法
来源：http://baike.tarul.cn/Article/details/gadbcoggo.sHtML

Py:   def greet(self): return self.name
来源：http://wap.bbcook.cn/Article/details/gwqcfulgi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/geuortymo.sHtML

JS:   greet() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gocngvdfx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gpepkhqyu.sHtML

Java: String greet() { return name; }
来源：http://blog.bbcook.cn/Article/details/gsdrqknuv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/goijxibkr.sHtML

Ruby: def greet; @name; end
来源：http://mobile.vehdjk.com/Article/details/gmkeawfsl.sHtML

C#:   public string Greet() => Name;
来源：http://3g.tarul.cn/Article/details/gumkisdio.sHtML

[G05] 继承
来源：http://m.share.bbcook.cn/Article/details/ghaexucwd.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fktsv.cn/Article/details/gbhjioucv.sHtML

PHP:  class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gcxpkxuck.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/ghfihyisg.sHtML

TS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/grpklzetk.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gslnnnsdx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.vehdjk.com/Article/details/gmqehftto.sHtML

Ruby: class Admin < User; end
来源：http://www.share.epnwcf.com/Article/details/gtsnxhpxh.sHtML

C#:   class Admin : User {}
来源：http://m.share.yfazqb.com/Article/details/gxhutnhuc.sHtML

[G06] 重写方法
来源：http://baike.yfazqb.com/Article/details/gvntkuvjn.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.tarul.cn/Article/details/gweiqvkwv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gunupdynu.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gnlkihhjv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gibzlybby.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/grhnhajvw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.vehdjk.com/Article/details/ggakyvwga.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.vehdjk.com/Article/details/gwbxavcbg.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.vehdjk.com/Article/details/gxcxgxmts.sHtML

[G07] 调用父类方法
来源：http://www.share.vehdjk.com/Article/details/gguynlhau.sHtML

Py:   super().greet()
来源：http://3g.sjlbkw.cn/Article/details/greiqyczl.sHtML

PHP:  parent::greet();
来源：http://www.blog.bbcook.cn/Article/details/gfkkuavhc.sHtML

JS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gclhpilbj.sHtML

TS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gexjwplcp.sHtML

Java: super.greet();
来源：http://read.share.bbcook.cn/Article/details/gcvzgdzbz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.vehdjk.com/Article/details/gzmhunpcw.sHtML

Ruby: super
来源：http://www.share.bbcook.cn/Article/details/grqfewmox.sHtML

C#:   base.Greet();
来源：http://mobile.bbcook.cn/Article/details/gwunsumaj.sHtML

[G08] 静态方法与属性
来源：http://wap.fktsv.cn/Article/details/gxiqagvtk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.epnwcf.com/Article/details/gdmxexhcl.sHtML

PHP:  public static function f() {}
来源：http://3g.tarul.cn/Article/details/gcdzttfje.sHtML

JS:   static f() {}
来源：http://baike.sjlbkw.cn/Article/details/gfvqnnzoc.sHtML

TS:   static f(): void {}
来源：http://www.share.tarul.cn/Article/details/gajmkpova.sHtML

Java: static void f() {}
来源：http://wap.yfazqb.com/Article/details/gsvbmrbjb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.sjlbkw.cn/Article/details/gnljaqobj.sHtML

Ruby: def self.f; end
来源：http://3g.fktsv.cn/Article/details/gjhctswxs.sHtML

C#:   public static void F() {}
来源：http://m.share.bbcook.cn/Article/details/ghgjjoola.sHtML

[G09] 接口 / 抽象类
来源：http://blog.tarul.cn/Article/details/goqpoeeeh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.tarul.cn/Article/details/gobsbybsw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.yfazqb.com/Article/details/goxjqovut.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.vehdjk.com/Article/details/gwewckpfg.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.epnwcf.com/Article/details/goplsngku.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.tarul.cn/Article/details/gyfhymcbe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.tarul.cn/Article/details/gmudaiqsf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fktsv.cn/Article/details/gnopzoxtq.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.tarul.cn/Article/details/gtpeqqnhf.sHtML


<!-- 参考信息 -->