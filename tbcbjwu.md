代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.vehdjk.com/Article/details/gjteteclj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.epnwcf.com/Article/details/gambmoyjb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmjxcphl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.sjlbkw.cn/Article/details/gleaxgpde.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gourlhesm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.yfazqb.com/Article/details/gnkwfokqz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fktsv.cn/Article/details/gbphewety.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.sjlbkw.cn/Article/details/gtqafbipq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.epnwcf.com/Article/details/gkttbgjkh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.vehdjk.com/Article/details/ghkbeyoil.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.sjlbkw.cn/Article/details/ghdbthhwf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.epnwcf.com/Article/details/gkdltrclt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.yfazqb.com/Article/details/gvawfgglq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.bbcook.cn/Article/details/ggohlwleb.sHtML

[E16] 数字千分位
来源：http://www.share.tarul.cn/Article/details/gvltxjawd.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.sjlbkw.cn/Article/details/gtlotguro.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fktsv.cn/Article/details/gkeefmzoy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gjlhdiwpe.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fktsv.cn/Article/details/geisnlstc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.bbcook.cn/Article/details/gshbexzzz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.tarul.cn/Article/details/gyqtukext.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.sjlbkw.cn/Article/details/gsefyawfs.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.vehdjk.com/Article/details/grhnetjcg.sHtML

[E17] 首字母大写
来源：http://www.share.bbcook.cn/Article/details/ghqadlfff.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.tarul.cn/Article/details/gcydagnjb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.epnwcf.com/Article/details/gtqglqptl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/grlmscnyq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gfovmeyij.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.epnwcf.com/Article/details/gfatbtyah.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.epnwcf.com/Article/details/gvjidqzdc.sHtML

Ruby: s.capitalize
来源：http://baike.sjlbkw.cn/Article/details/ggqltdqnm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.yfazqb.com/Article/details/glvgyerzu.sHtML

[E18] 模板占位符替换
来源：http://m.share.yfazqb.com/Article/details/guzmjwlnm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.bbcook.cn/Article/details/gpbqgotdk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.bbcook.cn/Article/details/gnypnphhd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.vehdjk.com/Article/details/gkyzrrtih.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/gstcqumpt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gpkamjrzb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.epnwcf.com/Article/details/gpecsvgap.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.sjlbkw.cn/Article/details/gsmtsysql.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.yfazqb.com/Article/details/gfbalunzb.sHtML

[E19] 多行文本按行拆分
来源：http://baike.epnwcf.com/Article/details/giggmdcpg.sHtML

Py:   s.splitlines()
来源：http://www.share.tarul.cn/Article/details/grggxpmil.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/giywablac.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gpogdmxal.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gmqorvtvq.sHtML

Java: s.lines().toList()
来源：http://www.blog.yfazqb.com/Article/details/gmdnhegdm.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fktsv.cn/Article/details/gnaxzbyxi.sHtML

Ruby: s.lines
来源：http://read.share.epnwcf.com/Article/details/gffuuvanj.sHtML

C#:   s.Split('\n')
来源：http://wap.epnwcf.com/Article/details/gngkkghjg.sHtML

[E20] 判断字符串是否为空
来源：http://baike.bbcook.cn/Article/details/gvtgaswvp.sHtML

Py:   if not s:
来源：http://baike.bbcook.cn/Article/details/gqsclyvjt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fktsv.cn/Article/details/gptgtzusd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.bbcook.cn/Article/details/gtbwuwbnc.sHtML

TS:   if (s === "") {}
来源：http://wap.epnwcf.com/Article/details/gfhmuoztb.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.epnwcf.com/Article/details/gnhoprqfc.sHtML

Go:   if s == "" {}
来源：http://blog.vehdjk.com/Article/details/gzmttsbdq.sHtML

Ruby: if s.empty?
来源：http://3g.vehdjk.com/Article/details/gtldzxhif.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.bbcook.cn/Article/details/girzgtioj.sHtML

[E21] 超长截断加省略号
来源：http://3g.yfazqb.com/Article/details/gjfhcobch.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fktsv.cn/Article/details/gjtkhpimd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gkrdalcvp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gkndgzhxj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gkgbxkvki.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gmdtosdsq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.epnwcf.com/Article/details/gyekettbq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gitysyoxj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gntrigsxj.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.yfazqb.com/Article/details/gfmicmisg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.bbcook.cn/Article/details/gcjlavsnf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gvqnjsnwl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gtatmrhvf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/gahovrrsq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.tarul.cn/Article/details/guzhnmakm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.bbcook.cn/Article/details/guojnssbv.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.vehdjk.com/Article/details/gyencqspb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.bbcook.cn/Article/details/gglsgkoeh.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gycnyvdhk.sHtML

F. 文件与目录
来源：http://mobile.bbcook.cn/Article/details/ghgibysgm.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gldagkuaz.sHtML

[F01] 读取整个文件
来源：http://www.share.fktsv.cn/Article/details/gfrknjjlm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.sjlbkw.cn/Article/details/gevddrhcb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.yfazqb.com/Article/details/ggsxwbjxv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.tarul.cn/Article/details/gpmtakcyu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gyzdzuxxp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gbmjmryud.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.tarul.cn/Article/details/gtpmyduye.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gvzfkyyiw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.tarul.cn/Article/details/gnnhmmjaa.sHtML

[F02] 逐行读取文件
来源：http://blog.vehdjk.com/Article/details/gtvuwtgwr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.vehdjk.com/Article/details/gdxchqdfy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fktsv.cn/Article/details/gfvogeogv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gxfgixbxu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gtnimdfne.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gtqfckneh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.tarul.cn/Article/details/gsokfznws.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.bbcook.cn/Article/details/gdkuvgibj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.yfazqb.com/Article/details/gkcimwwge.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.tarul.cn/Article/details/glctluyai.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.tarul.cn/Article/details/geeayucxj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.sjlbkw.cn/Article/details/gbrawrzwx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/gsysaqodp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gjnhhheet.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.bbcook.cn/Article/details/gguedvjly.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.yfazqb.com/Article/details/gctbcmkfp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fktsv.cn/Article/details/ggsscekjr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gqqdhljfb.sHtML

[F04] 追加写入文件
来源：http://wap.bbcook.cn/Article/details/gixkkrvch.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.epnwcf.com/Article/details/gpfkfixbb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.tarul.cn/Article/details/ghkfwdqzw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.epnwcf.com/Article/details/gpggmbldk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gksrjjaal.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.bbcook.cn/Article/details/gscdbxdsv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.bbcook.cn/Article/details/gpsiljwoj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.epnwcf.com/Article/details/gyuroofee.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.sjlbkw.cn/Article/details/gfbgtrmxx.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.yfazqb.com/Article/details/gkjanaaop.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.tarul.cn/Article/details/gqyzeltbo.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fktsv.cn/Article/details/ghqkvkfyl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gkeveevfa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gidbnveyi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gssgybmjo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.epnwcf.com/Article/details/gpujtjies.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gyswrevpo.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.tarul.cn/Article/details/gwiguqtsn.sHtML

[F06] 删除文件
来源：http://wap.epnwcf.com/Article/details/gojcysbgo.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gtxibdbwt.sHtML

PHP:  unlink("a.txt");
来源：http://blog.bbcook.cn/Article/details/gymfafojp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/glqxohwrl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gfhpewcwf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gyhifubzp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdoverbp.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.epnwcf.com/Article/details/grgvrqufu.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fktsv.cn/Article/details/gohdlbxpm.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.yfazqb.com/Article/details/gjbsihyyr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.sjlbkw.cn/Article/details/gflhotxiz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.epnwcf.com/Article/details/gihlfedmz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.tarul.cn/Article/details/gmffuciha.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gnqaophhj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.bbcook.cn/Article/details/guofbvyqt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fktsv.cn/Article/details/gfturhlwf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.yfazqb.com/Article/details/gzxpbtqyf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.bbcook.cn/Article/details/gtvitupjm.sHtML

[F08] 遍历目录
来源：http://www.blog.epnwcf.com/Article/details/gxngtivjb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fktsv.cn/Article/details/ggwyjkifj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.yfazqb.com/Article/details/gcockomuq.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/gawevnylw.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/gfqauzicu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gttspksbn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.tarul.cn/Article/details/ghbeulkwr.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.epnwcf.com/Article/details/gfqehwcng.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.sjlbkw.cn/Article/details/guryvvmoo.sHtML

[F09] 获取文件大小
来源：http://www.blog.bbcook.cn/Article/details/gktbznhpq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.yfazqb.com/Article/details/gfpwprnlh.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.tarul.cn/Article/details/geafupmac.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gyqkjkjus.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/glwljgcpb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/grjlstnbh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.sjlbkw.cn/Article/details/guviplbqq.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gzxwmbiid.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.bbcook.cn/Article/details/gfgbhxtpd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fktsv.cn/Article/details/gtvcxkuub.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gvywizfpq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gqmcbmztm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gabfzpbpd.sHtML

TS:   path.extname("a.txt")
来源：http://3g.vehdjk.com/Article/details/ggkefrjbs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.bbcook.cn/Article/details/gcuegirky.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gzsgslaot.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gtxdptzjy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gahmhtvuj.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.vehdjk.com/Article/details/gbufhpbnp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gbjtbbrql.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.vehdjk.com/Article/details/gotkdcodv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/grsyjhgdd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/glynhsouq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.vehdjk.com/Article/details/ghnytxiad.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.epnwcf.com/Article/details/gsltsadhu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gkerjpgyk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/grrmczduo.sHtML

[F12] CSV 读写
来源：http://www.share.epnwcf.com/Article/details/gbhkqfakx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.tarul.cn/Article/details/gnhgzmsjs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.bbcook.cn/Article/details/gdwfsqcmd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.sjlbkw.cn/Article/details/glnariplj.sHtML

TS:   // 同上
来源：http://www.share.fktsv.cn/Article/details/glzfcwlpb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.tarul.cn/Article/details/gdstevxlc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.bbcook.cn/Article/details/gnrvhhbez.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.vehdjk.com/Article/details/gisooyvwy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.sjlbkw.cn/Article/details/grzjvtmtr.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gsooadcpr.sHtML

G. 面向对象
来源：http://www.share.fktsv.cn/Article/details/gpqlesbyb.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gfwrwpbvz.sHtML

[G01] 定义类
来源：http://mobile.vehdjk.com/Article/details/gqfefkfjf.sHtML

Py:   class User: pass
来源：http://baike.sjlbkw.cn/Article/details/gqyzvwrqk.sHtML

PHP:  class User {}
来源：http://blog.sjlbkw.cn/Article/details/girnimhlv.sHtML

JS:   class User {}
来源：http://baike.vehdjk.com/Article/details/gxamaygyu.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.tarul.cn/Article/details/gwupgcdax.sHtML

Java: class User {}
来源：http://www.blog.epnwcf.com/Article/details/gpmlfbozs.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fktsv.cn/Article/details/gmxwqklcb.sHtML

Ruby: class User; end
来源：http://blog.fktsv.cn/Article/details/grukyiyki.sHtML

C#:   class User {}
来源：http://3g.fktsv.cn/Article/details/gbxmrxfrc.sHtML

[G02] 构造函数
来源：http://m.share.epnwcf.com/Article/details/gxirhbaby.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.sjlbkw.cn/Article/details/gxheyksun.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gbvuwsayy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/gzmdpzxhl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.epnwcf.com/Article/details/gvrxcdemj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gtuupfnst.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.tarul.cn/Article/details/gwgfzuvri.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fktsv.cn/Article/details/gzhercgth.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.tarul.cn/Article/details/gefjkratl.sHtML

[G03] 实例属性
来源：http://www.blog.bbcook.cn/Article/details/ggfjrvoga.sHtML

Py:   self.name = "x"
来源：http://read.share.epnwcf.com/Article/details/gmdfpivuh.sHtML

PHP:  public string $name = "x";
来源：http://read.share.epnwcf.com/Article/details/gemlenion.sHtML

JS:   this.name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gusylrtmy.sHtML

TS:   name: string = "x";
来源：http://blog.yfazqb.com/Article/details/gzxgekrsd.sHtML

Java: private String name;
来源：http://www.share.epnwcf.com/Article/details/gevktyjmz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.vehdjk.com/Article/details/gmukbcqsw.sHtML

Ruby: @name = "x"
来源：http://mobile.vehdjk.com/Article/details/gmzypczqj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.epnwcf.com/Article/details/guxxbhbma.sHtML

[G04] 定义方法
来源：http://www.blog.tarul.cn/Article/details/gmyjpsjiv.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gkweiynsu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gxgpjjlxq.sHtML

JS:   greet() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/ghhmquphi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gqqeczsbv.sHtML

Java: String greet() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gplearabo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gqieqmgme.sHtML

Ruby: def greet; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gtmrtpwbp.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fktsv.cn/Article/details/gdvwpaxyc.sHtML

[G05] 继承
来源：http://read.share.tarul.cn/Article/details/guqpfowvx.sHtML

Py:   class Admin(User): pass
来源：http://wap.sjlbkw.cn/Article/details/gjxvjlxjp.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gqkhzcuua.sHtML

JS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gxpujhoyb.sHtML

TS:   class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gtkzictbx.sHtML

Java: class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gchkhhqdy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.epnwcf.com/Article/details/gbucfjsej.sHtML

Ruby: class Admin < User; end
来源：http://read.share.yfazqb.com/Article/details/gzolefknq.sHtML

C#:   class Admin : User {}
来源：http://www.blog.yfazqb.com/Article/details/gaxevdejx.sHtML

[G06] 重写方法
来源：http://www.share.bbcook.cn/Article/details/gtfpdghre.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.epnwcf.com/Article/details/gbqwvgkql.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gxcuaapzn.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/guikjrykz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gjbajdapo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/govxcgncd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fktsv.cn/Article/details/gxyojlxau.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.bbcook.cn/Article/details/gdzhgyjvo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.yfazqb.com/Article/details/gdamxvhkm.sHtML

[G07] 调用父类方法
来源：http://mobile.vehdjk.com/Article/details/gackmijsx.sHtML

Py:   super().greet()
来源：http://mobile.yfazqb.com/Article/details/gmywgugsa.sHtML

PHP:  parent::greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gibbnkifb.sHtML

JS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/gearuufqr.sHtML

TS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gcwfnazbq.sHtML

Java: super.greet();
来源：http://www.share.fktsv.cn/Article/details/gtgmtvhxt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.yfazqb.com/Article/details/ggsbutcvl.sHtML

Ruby: super
来源：http://baike.yfazqb.com/Article/details/ghjyokeif.sHtML

C#:   base.Greet();
来源：http://www.blog.tarul.cn/Article/details/gfxajgtkn.sHtML

[G08] 静态方法与属性
来源：http://baike.vehdjk.com/Article/details/gnrdyylvq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.tarul.cn/Article/details/gfcudcvur.sHtML

PHP:  public static function f() {}
来源：http://mobile.bbcook.cn/Article/details/gjcikdkld.sHtML

JS:   static f() {}
来源：http://www.share.bbcook.cn/Article/details/gqaowptxj.sHtML

TS:   static f(): void {}
来源：http://read.share.sjlbkw.cn/Article/details/gzacvglzq.sHtML

Java: static void f() {}
来源：http://www.m.share.fktsv.cn/Article/details/grfghcdoi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.vehdjk.com/Article/details/gcpqcldcd.sHtML

Ruby: def self.f; end
来源：http://mobile.sjlbkw.cn/Article/details/gslddwrgr.sHtML

C#:   public static void F() {}
来源：http://mobile.vehdjk.com/Article/details/gevajtyoh.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.yfazqb.com/Article/details/gsevygpyv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.bbcook.cn/Article/details/gxypyzmcn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.epnwcf.com/Article/details/gpgywnuod.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.sjlbkw.cn/Article/details/gahswwoch.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.vehdjk.com/Article/details/gxbuexuck.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.vehdjk.com/Article/details/gzjwyntwc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.yfazqb.com/Article/details/guwwrmoqa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.vehdjk.com/Article/details/gytufikty.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.tarul.cn/Article/details/gixkiwzen.sHtML

[G10] 访问控制
来源：http://3g.fktsv.cn/Article/details/gpgzgdzau.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.epnwcf.com/Article/details/gqqgtfday.sHtML

PHP:  public / protected / private
来源：http://baike.yfazqb.com/Article/details/guhiheeyp.sHtML

JS:   #private 字段；其余公开
来源：http://3g.vehdjk.com/Article/details/ggmpoccor.sHtML

TS:   public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gdsjiavpf.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.vehdjk.com/Article/details/gfgoqvbsr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.epnwcf.com/Article/details/gziqzpkac.sHtML

Ruby: public / protected / private
来源：http://wap.fktsv.cn/Article/details/gfkxysfhm.sHtML

C#:   public / protected / private / internal
来源：http://read.share.vehdjk.com/Article/details/gtrjxvrgw.sHtML

[G11] getter / setter
来源：http://www.share.vehdjk.com/Article/details/gshrlkyin.sHtML

Py:   @property 与 @x.setter
来源：http://wap.yfazqb.com/Article/details/gfwubwrhv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gtfrdibzx.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/gudrsclzd.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.tarul.cn/Article/details/gtzsopiht.sHtML

Java: public String getName() { return name; }
来源：http://baike.epnwcf.com/Article/details/ggaofvalj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/ggztiyyic.sHtML

Ruby: attr_accessor :name
来源：http://read.share.tarul.cn/Article/details/gejnigglx.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.yfazqb.com/Article/details/gykxnvrtm.sHtML

[G12] 对象转字符串
来源：http://www.blog.fktsv.cn/Article/details/gpolsnovw.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gbsehnlug.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/ghbnziaif.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gopjzkmyz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/ghaxfsfwx.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.yfazqb.com/Article/details/getskvlrb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gcjbbietx.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.bbcook.cn/Article/details/gudwhvlep.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fktsv.cn/Article/details/gdvedbrqn.sHtML

[G13] 判断对象类型
来源：http://mobile.fktsv.cn/Article/details/gfkwpptkv.sHtML


<!-- 参考信息 -->