代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.bbcook.cn/Article/details/ggdnzecpg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.epnwcf.com/Article/details/gikwynhxm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fktsv.cn/Article/details/gmgyjmxgm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.tarul.cn/Article/details/gfqlleibo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fktsv.cn/Article/details/gqhpowlwa.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.vehdjk.com/Article/details/geepkkcqh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.sjlbkw.cn/Article/details/gzvmbokyc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.bbcook.cn/Article/details/gjneznsta.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.yfazqb.com/Article/details/gucdxuxae.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.vehdjk.com/Article/details/gyqpmarfi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.vehdjk.com/Article/details/gvdompkin.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.bbcook.cn/Article/details/gjafhlbaw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.yfazqb.com/Article/details/gclgrixla.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.bbcook.cn/Article/details/gpcjiubrj.sHtML

[E16] 数字千分位
来源：http://www.share.epnwcf.com/Article/details/gyrmulnrb.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.yfazqb.com/Article/details/gasnctmqk.sHtML

PHP:  number_format(1234567);
来源：http://blog.epnwcf.com/Article/details/gafvbwolh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/geislyuct.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gotupdjbg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fktsv.cn/Article/details/gllrknifk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.vehdjk.com/Article/details/givgvauqh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.bbcook.cn/Article/details/ggpxbajlb.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.sjlbkw.cn/Article/details/gkowgncgt.sHtML

[E17] 首字母大写
来源：http://mobile.yfazqb.com/Article/details/gijfitwec.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.tarul.cn/Article/details/gwfipsmzl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fktsv.cn/Article/details/gedleghlx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.vehdjk.com/Article/details/gbpujppih.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gzzjfekxb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.tarul.cn/Article/details/gphfoxzni.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.yfazqb.com/Article/details/gkklurpzi.sHtML

Ruby: s.capitalize
来源：http://mobile.vehdjk.com/Article/details/ginausoxz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.tarul.cn/Article/details/gzfedbnac.sHtML

[E18] 模板占位符替换
来源：http://read.share.vehdjk.com/Article/details/goqbdqlii.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.bbcook.cn/Article/details/gvuujlkby.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.sjlbkw.cn/Article/details/gfpnjjbrt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gsawtifrz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gokteilsx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gdevkmswm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/giltfjgof.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.epnwcf.com/Article/details/gwsdymyam.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.vehdjk.com/Article/details/gjhetbphf.sHtML

[E19] 多行文本按行拆分
来源：http://baike.tarul.cn/Article/details/guiqeiovi.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/gjylrihsp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.tarul.cn/Article/details/gepbnqzzm.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.vehdjk.com/Article/details/gisunrajg.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.yfazqb.com/Article/details/goedaxquz.sHtML

Java: s.lines().toList()
来源：http://blog.yfazqb.com/Article/details/gfjdgyvpm.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fktsv.cn/Article/details/gompvhcjl.sHtML

Ruby: s.lines
来源：http://wap.vehdjk.com/Article/details/gpgvixezt.sHtML

C#:   s.Split('\n')
来源：http://m.share.sjlbkw.cn/Article/details/gsukonnqd.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.sjlbkw.cn/Article/details/gxzjusjnd.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/gsgemrqat.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fktsv.cn/Article/details/gdwdyikmt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.epnwcf.com/Article/details/gyugnocqx.sHtML

TS:   if (s === "") {}
来源：http://mobile.yfazqb.com/Article/details/gtfixvofk.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gvrcwsqhe.sHtML

Go:   if s == "" {}
来源：http://baike.sjlbkw.cn/Article/details/gixmkdefq.sHtML

Ruby: if s.empty?
来源：http://read.share.epnwcf.com/Article/details/gukuedape.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fktsv.cn/Article/details/gosmtwuni.sHtML

[E21] 超长截断加省略号
来源：http://www.share.tarul.cn/Article/details/gsfhlenio.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.tarul.cn/Article/details/gduvmsmll.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gtabobdur.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gqrousvdm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gynmjzzps.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gtremgqyi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.sjlbkw.cn/Article/details/gdseozekj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gziqmjawq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.tarul.cn/Article/details/gsmicnhwq.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.yfazqb.com/Article/details/gczjwzend.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.sjlbkw.cn/Article/details/gyyyyapgh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gvljppvuy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gxtibszjc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/glfmhweej.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.tarul.cn/Article/details/gylocgnoc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.yfazqb.com/Article/details/gdcgglquc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gnvsgglxr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.bbcook.cn/Article/details/ggefeqkhd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/guutfqcuk.sHtML

F. 文件与目录
来源：http://wap.sjlbkw.cn/Article/details/gfdvvfkid.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gevhwqlur.sHtML

[F01] 读取整个文件
来源：http://blog.vehdjk.com/Article/details/gziihhljz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.bbcook.cn/Article/details/gmcfxlgiz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.tarul.cn/Article/details/gatykkpot.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/gopfdtaze.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.vehdjk.com/Article/details/gysrxktap.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/ggetwrilo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.tarul.cn/Article/details/gakjdjfye.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gjaqvhyml.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.tarul.cn/Article/details/genpnpruf.sHtML

[F02] 逐行读取文件
来源：http://blog.vehdjk.com/Article/details/goohpttis.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.sjlbkw.cn/Article/details/giooaprrh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fktsv.cn/Article/details/gjwiuqagq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/ggwjrqonf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.yfazqb.com/Article/details/gcvrthmll.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/gpdacgnci.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.sjlbkw.cn/Article/details/gvvjldpkd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.sjlbkw.cn/Article/details/gofbsuqul.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.sjlbkw.cn/Article/details/gcuiuehha.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.bbcook.cn/Article/details/gtfimhtyu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.epnwcf.com/Article/details/ghutjwviu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gdmybleib.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.yfazqb.com/Article/details/grykbgqbi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gcvnfehbv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.vehdjk.com/Article/details/gxpinfnnp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.epnwcf.com/Article/details/gpdjptxxt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.tarul.cn/Article/details/gvmyvebgq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/gdqmxxraw.sHtML

[F04] 追加写入文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gonpqyuky.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.epnwcf.com/Article/details/gehntmgmq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.epnwcf.com/Article/details/ghgsjvjbw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fktsv.cn/Article/details/gsiokljzq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/glmziuxkz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.tarul.cn/Article/details/ggcruonkb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.bbcook.cn/Article/details/gfsyrlevh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.yfazqb.com/Article/details/gttwosrdt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.tarul.cn/Article/details/gariqugbd.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fktsv.cn/Article/details/gijiysvun.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.bbcook.cn/Article/details/gagmpcqyu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gwjwapiaw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gyddgipcv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/glgrbhhoc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/ghxuhrcuh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.bbcook.cn/Article/details/gtaedsgta.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gvenvhxiy.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.vehdjk.com/Article/details/gbqsfpjww.sHtML

[F06] 删除文件
来源：http://www.m.share.fktsv.cn/Article/details/gnnwlzkqu.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/ghxbhjeug.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gsochbzqu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/geagwwhxi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gdawiweix.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/ghupbzzsy.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/gmmqfihmw.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gwxrrckpz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.tarul.cn/Article/details/gwjsjgkyp.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.vehdjk.com/Article/details/gkqweerwa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/guiwilqxx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.tarul.cn/Article/details/gedqsgmvv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.vehdjk.com/Article/details/gqbvuywbu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/goigglhvq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fktsv.cn/Article/details/gkovbpnyp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.tarul.cn/Article/details/ggmbagwfe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.epnwcf.com/Article/details/gwirwdsuf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.yfazqb.com/Article/details/gnavgbpxp.sHtML

[F08] 遍历目录
来源：http://read.share.sjlbkw.cn/Article/details/glbvopgrx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.yfazqb.com/Article/details/gvorjakxv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.epnwcf.com/Article/details/gruslujra.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/ghgmmjuet.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/gewrmvbxh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gufgtquwi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.yfazqb.com/Article/details/gpzfryvbb.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.bbcook.cn/Article/details/gqegrjvbo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gavrugmjy.sHtML

[F09] 获取文件大小
来源：http://mobile.yfazqb.com/Article/details/gwdrjpjoh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.bbcook.cn/Article/details/gonqjnunq.sHtML

PHP:  filesize("a.txt");
来源：http://blog.epnwcf.com/Article/details/gbrehbjnr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gwvqescfo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gwocuyymy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/givyjbgei.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.vehdjk.com/Article/details/gyjjzxuzm.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.bbcook.cn/Article/details/ggutdzqoy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.sjlbkw.cn/Article/details/goohyeiqr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.vehdjk.com/Article/details/gcvegowsv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/ghypkibsp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.bbcook.cn/Article/details/gvmcnmslf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gfhwhbgue.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gwjrqvivb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.yfazqb.com/Article/details/gymufjyth.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/goeiszscl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gcngtcoqr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gifdhhctc.sHtML

[F11] 复制与移动文件
来源：http://mobile.tarul.cn/Article/details/gfxjozsir.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gtciaiemj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.tarul.cn/Article/details/gmzbdnvtc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gmqqoabax.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gnwntdcnz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.yfazqb.com/Article/details/gxjilprfe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.bbcook.cn/Article/details/gbhneookv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/groasvczk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.bbcook.cn/Article/details/ggzyljfxj.sHtML

[F12] CSV 读写
来源：http://m.share.fktsv.cn/Article/details/geikmsbgh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.bbcook.cn/Article/details/gbwkaotsj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.tarul.cn/Article/details/gzwkecena.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fktsv.cn/Article/details/gempgamdl.sHtML

TS:   // 同上
来源：http://www.m.share.vehdjk.com/Article/details/gbewyxwac.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.sjlbkw.cn/Article/details/gxvvuzefb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.tarul.cn/Article/details/geepxhxrn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.epnwcf.com/Article/details/ghceuckon.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.vehdjk.com/Article/details/gudbjkqnk.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdervlxxx.sHtML

G. 面向对象
来源：http://read.share.yfazqb.com/Article/details/gugwnhhhf.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/grmxficwd.sHtML

[G01] 定义类
来源：http://blog.epnwcf.com/Article/details/ghxbsrqsy.sHtML

Py:   class User: pass
来源：http://3g.yfazqb.com/Article/details/guxflcuth.sHtML

PHP:  class User {}
来源：http://3g.fktsv.cn/Article/details/gfzjsrdjn.sHtML

JS:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gsnmdztiy.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.sjlbkw.cn/Article/details/gcpgsdzzj.sHtML

Java: class User {}
来源：http://blog.yfazqb.com/Article/details/ghvzbztqz.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fktsv.cn/Article/details/guanpgrvr.sHtML

Ruby: class User; end
来源：http://m.share.tarul.cn/Article/details/gjlepjgsq.sHtML

C#:   class User {}
来源：http://m.share.tarul.cn/Article/details/gikaswwli.sHtML

[G02] 构造函数
来源：http://www.share.tarul.cn/Article/details/gywvtgapd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.sjlbkw.cn/Article/details/gqynkluam.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.yfazqb.com/Article/details/gdyibzuin.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.sjlbkw.cn/Article/details/ggxwzazxi.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fktsv.cn/Article/details/gkunhqxdh.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/gqjnfhncv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.sjlbkw.cn/Article/details/gxolttaji.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.vehdjk.com/Article/details/goqrhvhkg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.vehdjk.com/Article/details/grsvzgbei.sHtML

[G03] 实例属性
来源：http://baike.tarul.cn/Article/details/glusovnxi.sHtML

Py:   self.name = "x"
来源：http://www.blog.vehdjk.com/Article/details/guwvijzyr.sHtML

PHP:  public string $name = "x";
来源：http://blog.yfazqb.com/Article/details/gvpmzcxwc.sHtML

JS:   this.name = "x";
来源：http://www.share.fktsv.cn/Article/details/gmtexqjyb.sHtML

TS:   name: string = "x";
来源：http://wap.vehdjk.com/Article/details/gbegkpyko.sHtML

Java: private String name;
来源：http://www.share.fktsv.cn/Article/details/gqsovtctw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fktsv.cn/Article/details/gvbdnzumf.sHtML

Ruby: @name = "x"
来源：http://baike.vehdjk.com/Article/details/guewlzmbm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.tarul.cn/Article/details/giccvrdek.sHtML

[G04] 定义方法
来源：http://m.share.yfazqb.com/Article/details/gkplfywwu.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/gewizkkbi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzxcudylu.sHtML

JS:   greet() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gebierqmn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gzmrlvpsa.sHtML

Java: String greet() { return name; }
来源：http://3g.bbcook.cn/Article/details/gcxgtjtdq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gfzrsvfph.sHtML

Ruby: def greet; @name; end
来源：http://3g.yfazqb.com/Article/details/gxknwpthd.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.bbcook.cn/Article/details/gowukvhlv.sHtML

[G05] 继承
来源：http://baike.yfazqb.com/Article/details/gegcweosw.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.sjlbkw.cn/Article/details/gllluczfz.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gcqinibls.sHtML

JS:   class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gxtmnawdh.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gxznimdoj.sHtML

Java: class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gsydofoda.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.epnwcf.com/Article/details/ghftepgfd.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/gpiceoksx.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fktsv.cn/Article/details/ghevwgexg.sHtML

[G06] 重写方法
来源：http://www.share.sjlbkw.cn/Article/details/gtbevqmfv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.yfazqb.com/Article/details/gkqdraqxu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gzyfgfuti.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gxnfjjopn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gqvtfhzci.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gqlssrsqe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.bbcook.cn/Article/details/gpaphlbtw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.bbcook.cn/Article/details/genzsycuk.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fktsv.cn/Article/details/gcmjrtpmp.sHtML

[G07] 调用父类方法
来源：http://www.m.share.tarul.cn/Article/details/giupagyar.sHtML

Py:   super().greet()
来源：http://m.share.vehdjk.com/Article/details/gqrrnphtq.sHtML

PHP:  parent::greet();
来源：http://mobile.tarul.cn/Article/details/gglchksny.sHtML

JS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/gwkxqyrhy.sHtML

TS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/gjaghlfxb.sHtML

Java: super.greet();
来源：http://blog.fktsv.cn/Article/details/gavkinnxt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.tarul.cn/Article/details/gyccxwgkd.sHtML

Ruby: super
来源：http://blog.yfazqb.com/Article/details/gwwtswnyx.sHtML

C#:   base.Greet();
来源：http://baike.tarul.cn/Article/details/gbiplcaaa.sHtML

[G08] 静态方法与属性
来源：http://blog.vehdjk.com/Article/details/gpjhguhef.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.bbcook.cn/Article/details/gnwpelfmr.sHtML

PHP:  public static function f() {}
来源：http://read.share.yfazqb.com/Article/details/gtiknibur.sHtML

JS:   static f() {}
来源：http://baike.epnwcf.com/Article/details/geemhezlv.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/goynzlyte.sHtML

Java: static void f() {}
来源：http://www.m.share.tarul.cn/Article/details/gdxsofoxa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fktsv.cn/Article/details/gsfverrso.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gxcvimwlc.sHtML

C#:   public static void F() {}
来源：http://www.m.share.yfazqb.com/Article/details/gpirldnlh.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.sjlbkw.cn/Article/details/gytrpzpeb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.tarul.cn/Article/details/giygmcoju.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fktsv.cn/Article/details/gzzykfxal.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.tarul.cn/Article/details/gvgalpsmt.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fktsv.cn/Article/details/gatppqnyy.sHtML

Java: interface Shape { double area(); }
来源：http://blog.vehdjk.com/Article/details/gsbgqpodt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/gbjipxbyh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.vehdjk.com/Article/details/gjeruvqfd.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.yfazqb.com/Article/details/gnxekjufz.sHtML

[G10] 访问控制
来源：http://wap.yfazqb.com/Article/details/gpsncldhp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.vehdjk.com/Article/details/gslaslmrh.sHtML

PHP:  public / protected / private
来源：http://baike.fktsv.cn/Article/details/gzksjtaus.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.epnwcf.com/Article/details/gddbghnxq.sHtML

TS:   public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gzxannpff.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fktsv.cn/Article/details/gxumtfnzm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.epnwcf.com/Article/details/gkwjbcpjk.sHtML

Ruby: public / protected / private
来源：http://blog.yfazqb.com/Article/details/gcunnuiha.sHtML

C#:   public / protected / private / internal
来源：http://wap.vehdjk.com/Article/details/gyyduivio.sHtML

[G11] getter / setter
来源：http://mobile.fktsv.cn/Article/details/gamhgrjxy.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.bbcook.cn/Article/details/ggkwxchug.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gjhnobbrr.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gqqexihcs.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gvjcgrttv.sHtML

Java: public String getName() { return name; }
来源：http://baike.vehdjk.com/Article/details/gmmgohehe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gbogafvvx.sHtML

Ruby: attr_accessor :name
来源：http://baike.vehdjk.com/Article/details/gyfxqswyt.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.vehdjk.com/Article/details/gwrmnwtvv.sHtML

[G12] 对象转字符串
来源：http://mobile.yfazqb.com/Article/details/gvqbmyvhc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.tarul.cn/Article/details/gpwzazvzx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/grooonnbq.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gjwhqowpt.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gnjrlzndd.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.tarul.cn/Article/details/gzfwiktsv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gojrnmgxz.sHtML

Ruby: def to_s; @name; end
来源：http://baike.tarul.cn/Article/details/gkyyjkaqr.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.sjlbkw.cn/Article/details/glypjhwoz.sHtML

[G13] 判断对象类型
来源：http://blog.fktsv.cn/Article/details/gjznzivys.sHtML


<!-- 参考信息 -->