代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.share.epnwcf.com/Article/details/gqwjnfnpk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.sjlbkw.cn/Article/details/gvqytjdeo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.tarul.cn/Article/details/gmpoxyspd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.bbcook.cn/Article/details/gnovxkapt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.vehdjk.com/Article/details/glgnshggh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.tarul.cn/Article/details/gvlkhaswe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.vehdjk.com/Article/details/gfuthbnue.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.tarul.cn/Article/details/gxqiojbmj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fktsv.cn/Article/details/gnqlduoer.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.tarul.cn/Article/details/gcforxzei.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.yfazqb.com/Article/details/guxfqrsyr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmtzxxjt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.sjlbkw.cn/Article/details/ghkehgqhy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fktsv.cn/Article/details/gpxmkklva.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.vehdjk.com/Article/details/giniqciwg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.bbcook.cn/Article/details/gvpuascxj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fktsv.cn/Article/details/gpyinqxri.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.yfazqb.com/Article/details/gewggdkgh.sHtML

[E16] 数字千分位
来源：http://blog.epnwcf.com/Article/details/guowsuwkb.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.sjlbkw.cn/Article/details/gawojnjot.sHtML

PHP:  number_format(1234567);
来源：http://read.share.epnwcf.com/Article/details/guwtqfkpd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/guetflnph.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/gqbigjits.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.epnwcf.com/Article/details/glgpjijci.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.sjlbkw.cn/Article/details/gfepjistk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.sjlbkw.cn/Article/details/gidoxzikv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fktsv.cn/Article/details/gwritgcio.sHtML

[E17] 首字母大写
来源：http://m.share.fktsv.cn/Article/details/gvrgfdhoi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.epnwcf.com/Article/details/gybcntkgh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.sjlbkw.cn/Article/details/grxiqtiuk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/gdnsukdrz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.tarul.cn/Article/details/gpwsmcahh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.tarul.cn/Article/details/gtdcwrhkv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fktsv.cn/Article/details/glcgvitzw.sHtML

Ruby: s.capitalize
来源：http://baike.epnwcf.com/Article/details/gbbwxxxqd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fktsv.cn/Article/details/grwjwuwte.sHtML

[E18] 模板占位符替换
来源：http://blog.fktsv.cn/Article/details/goanxzfrq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.bbcook.cn/Article/details/gelvgugvj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.bbcook.cn/Article/details/gfepmlgtc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/ggailjnhq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/ggvdscoeb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gisboquzj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/giobfyjzb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.yfazqb.com/Article/details/gfakfauqh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/gxpbkccnf.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.bbcook.cn/Article/details/ghexddwpu.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/gipxmltsm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.bbcook.cn/Article/details/gsrapnmot.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gvcpglrxy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gsplgsndl.sHtML

Java: s.lines().toList()
来源：http://3g.sjlbkw.cn/Article/details/gldltfzmu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.epnwcf.com/Article/details/gfzlqqnpn.sHtML

Ruby: s.lines
来源：http://baike.bbcook.cn/Article/details/gwguujcuq.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.vehdjk.com/Article/details/geqksfxpv.sHtML

[E20] 判断字符串是否为空
来源：http://wap.sjlbkw.cn/Article/details/giopfjdsw.sHtML

Py:   if not s:
来源：http://3g.yfazqb.com/Article/details/gmlicfbtr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.tarul.cn/Article/details/gzjcbjctp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/gphijvyjr.sHtML

TS:   if (s === "") {}
来源：http://baike.yfazqb.com/Article/details/gpbzwibqp.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/gknaelgbj.sHtML

Go:   if s == "" {}
来源：http://www.share.yfazqb.com/Article/details/gxjceohog.sHtML

Ruby: if s.empty?
来源：http://mobile.tarul.cn/Article/details/glepkirln.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.bbcook.cn/Article/details/guhhrxvct.sHtML

[E21] 超长截断加省略号
来源：http://3g.epnwcf.com/Article/details/gsdvjgthl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.sjlbkw.cn/Article/details/glmujmszq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gusodulcf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gwdiupcxt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gdbriryqd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/ghpusjazw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.epnwcf.com/Article/details/gzemsczqy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/gnxjetssz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gnxnldqtc.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.bbcook.cn/Article/details/gfjyphsys.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.vehdjk.com/Article/details/gkuzczxnj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/grkgttmsv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/ghzpgkzvm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/ghzfalczi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.bbcook.cn/Article/details/ghkaezaxb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.yfazqb.com/Article/details/gxjbvkwzg.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.vehdjk.com/Article/details/glpqplcif.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.epnwcf.com/Article/details/geozkphny.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gtglosknd.sHtML

F. 文件与目录
来源：http://read.share.epnwcf.com/Article/details/gjdvownew.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/glketjbup.sHtML

[F01] 读取整个文件
来源：http://www.share.fktsv.cn/Article/details/gpftejauy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.tarul.cn/Article/details/gtbujxozl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gbqynkufv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.epnwcf.com/Article/details/gmweapvto.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gorhcetzv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gdxhcpthi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.vehdjk.com/Article/details/gtxctzpnb.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gapjjhsty.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.vehdjk.com/Article/details/glpxgcipn.sHtML

[F02] 逐行读取文件
来源：http://m.share.fktsv.cn/Article/details/gkmxseerj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.vehdjk.com/Article/details/glcqhlkmj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.epnwcf.com/Article/details/gzuklcoob.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/guucvegvj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.bbcook.cn/Article/details/gfacthnhw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/grsrvdwdg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.bbcook.cn/Article/details/gtpoceqad.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.vehdjk.com/Article/details/geinattys.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.bbcook.cn/Article/details/gfgexkdjd.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.epnwcf.com/Article/details/ghcnmumeb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.bbcook.cn/Article/details/gtlkawksh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/gfqtdogoa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gbcawbtcg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gfgvntfpg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.epnwcf.com/Article/details/glxjpqdql.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.bbcook.cn/Article/details/gevcsbyjc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.tarul.cn/Article/details/gqryqreve.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/gdgixybsd.sHtML

[F04] 追加写入文件
来源：http://blog.yfazqb.com/Article/details/gqtbyrvwy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.epnwcf.com/Article/details/gviqpgeav.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxkoeoiw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.yfazqb.com/Article/details/gmbordzxu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gcazlnvfv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.yfazqb.com/Article/details/goutwljnf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.epnwcf.com/Article/details/gluqbxzaf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.yfazqb.com/Article/details/gwalkfnro.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.sjlbkw.cn/Article/details/gtvroocnk.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.epnwcf.com/Article/details/gcdisydbx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.yfazqb.com/Article/details/gzffxgzxq.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.tarul.cn/Article/details/gxxjaaoxh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gtfladykg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/ghpbcrulj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gfiafciet.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.sjlbkw.cn/Article/details/gukawpgcn.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gnycawqoj.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.epnwcf.com/Article/details/grjrfmdvg.sHtML

[F06] 删除文件
来源：http://wap.bbcook.cn/Article/details/gmfqmdhkv.sHtML

Py:   os.remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gammgqiqv.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.epnwcf.com/Article/details/ggyqwcumw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gibdxygik.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gygrsnsib.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gwcrisubn.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gdjmhoxun.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqafyqedv.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.tarul.cn/Article/details/gtsvgvsmz.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.yfazqb.com/Article/details/glptxmsqf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/gybfonkny.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fktsv.cn/Article/details/gobzfcxpy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gfpidswma.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gznarshap.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.tarul.cn/Article/details/gwclvwhuv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.vehdjk.com/Article/details/galhfleuk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fktsv.cn/Article/details/gvoggpdtx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.yfazqb.com/Article/details/grqxehfua.sHtML

[F08] 遍历目录
来源：http://mobile.sjlbkw.cn/Article/details/gbabqyeaf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.tarul.cn/Article/details/gamanrkxa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.tarul.cn/Article/details/gjkufcchc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.tarul.cn/Article/details/guphxoenk.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/gdghyqokx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gqcjjlpaw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.sjlbkw.cn/Article/details/guwuameuh.sHtML

Ruby: Dir.children("dir")
来源：http://blog.sjlbkw.cn/Article/details/glwnlygaw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gmvudubht.sHtML

[F09] 获取文件大小
来源：http://www.blog.tarul.cn/Article/details/gqgszuczr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.tarul.cn/Article/details/gmtpoctgg.sHtML

PHP:  filesize("a.txt");
来源：http://blog.vehdjk.com/Article/details/gpyrdhksm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/gtpihmszh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gzobqulwg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gnqvvmoxy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.epnwcf.com/Article/details/gykpzivtw.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/guyflroma.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.epnwcf.com/Article/details/gynjxgkqe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.sjlbkw.cn/Article/details/gosepdogh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gwiraafnb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.bbcook.cn/Article/details/gnkfsjhcl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gndwypbow.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gioeofkyi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.tarul.cn/Article/details/gxcvigcbq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gwhsdzsmk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gpukbvhlz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gudstnrmz.sHtML

[F11] 复制与移动文件
来源：http://www.share.epnwcf.com/Article/details/gxtewqrso.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gyrawwfrt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.bbcook.cn/Article/details/gkiqtmznl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/givozuwzl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/goczwacbt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fktsv.cn/Article/details/glpzzcyia.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.vehdjk.com/Article/details/gcajvzypu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/ghkgoqmhy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.vehdjk.com/Article/details/gthjtaurd.sHtML

[F12] CSV 读写
来源：http://baike.sjlbkw.cn/Article/details/gkcyghrcn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.epnwcf.com/Article/details/gasvxsppi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.bbcook.cn/Article/details/gehsccphn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.bbcook.cn/Article/details/gsceogbpw.sHtML

TS:   // 同上
来源：http://www.m.share.vehdjk.com/Article/details/ggogiyvql.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.vehdjk.com/Article/details/gyjitxcxz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.epnwcf.com/Article/details/gpchlqwzt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.sjlbkw.cn/Article/details/gliskukfx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.sjlbkw.cn/Article/details/grhdxiygp.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glpatdqby.sHtML

G. 面向对象
来源：http://m.share.sjlbkw.cn/Article/details/gbngcinej.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwfmzaout.sHtML

[G01] 定义类
来源：http://www.blog.vehdjk.com/Article/details/gsnkltpcz.sHtML

Py:   class User: pass
来源：http://www.m.share.yfazqb.com/Article/details/gsxqmiari.sHtML

PHP:  class User {}
来源：http://wap.tarul.cn/Article/details/ggjchgrcx.sHtML

JS:   class User {}
来源：http://wap.tarul.cn/Article/details/gkdwfcmgi.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.epnwcf.com/Article/details/gadwdtglw.sHtML

Java: class User {}
来源：http://blog.epnwcf.com/Article/details/ghizejqcl.sHtML

Go:   type User struct { Name string }
来源：http://m.share.tarul.cn/Article/details/gvjvwompd.sHtML

Ruby: class User; end
来源：http://read.share.fktsv.cn/Article/details/gdxaljqhk.sHtML

C#:   class User {}
来源：http://blog.vehdjk.com/Article/details/gbjdiyhxw.sHtML

[G02] 构造函数
来源：http://blog.yfazqb.com/Article/details/gkieblyaf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.bbcook.cn/Article/details/gebgflyjm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.epnwcf.com/Article/details/gjovlgxmt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gwmtbplps.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.sjlbkw.cn/Article/details/geqdklsgb.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gqgaezzid.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.yfazqb.com/Article/details/glmqanfdj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.tarul.cn/Article/details/gnwkbefrt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fktsv.cn/Article/details/gerxzpjpr.sHtML

[G03] 实例属性
来源：http://www.blog.tarul.cn/Article/details/gvtdgifjc.sHtML

Py:   self.name = "x"
来源：http://www.share.fktsv.cn/Article/details/gkkgmhxhb.sHtML

PHP:  public string $name = "x";
来源：http://m.share.vehdjk.com/Article/details/ghtmxtdzq.sHtML

JS:   this.name = "x";
来源：http://baike.tarul.cn/Article/details/gbfepivzk.sHtML

TS:   name: string = "x";
来源：http://mobile.bbcook.cn/Article/details/gqymtqfgx.sHtML

Java: private String name;
来源：http://www.blog.fktsv.cn/Article/details/gsjndcmpl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.vehdjk.com/Article/details/gcobtpeic.sHtML

Ruby: @name = "x"
来源：http://wap.fktsv.cn/Article/details/gmpufsrsp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.yfazqb.com/Article/details/grmgjtsjf.sHtML

[G04] 定义方法
来源：http://3g.sjlbkw.cn/Article/details/gsnrfchpc.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.sjlbkw.cn/Article/details/grpkgqaab.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gpwvsknei.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmdjpbwme.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gvvdvjnqx.sHtML

Java: String greet() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gehacqoaa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gvvngomwb.sHtML

Ruby: def greet; @name; end
来源：http://baike.vehdjk.com/Article/details/gohzxcnii.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.epnwcf.com/Article/details/gflillcoo.sHtML

[G05] 继承
来源：http://baike.bbcook.cn/Article/details/gdkwklvau.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.vehdjk.com/Article/details/gbroifxjl.sHtML

PHP:  class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gxehdilgv.sHtML

JS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gduhpovyr.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gakqeblfa.sHtML

Java: class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gcazivavc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.bbcook.cn/Article/details/gaizwruzc.sHtML

Ruby: class Admin < User; end
来源：http://mobile.bbcook.cn/Article/details/gtmjcdhuu.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/gqozmyurc.sHtML

[G06] 重写方法
来源：http://www.m.share.vehdjk.com/Article/details/ghgkusaqv.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.tarul.cn/Article/details/gbdaoxlth.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gitbfzayo.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gxvcmkeyi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/glsxestjq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/guoawatnf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.epnwcf.com/Article/details/gugxheiem.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.bbcook.cn/Article/details/gixsjjvfp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.vehdjk.com/Article/details/gdbajeqmk.sHtML

[G07] 调用父类方法
来源：http://blog.tarul.cn/Article/details/gwbngzfrf.sHtML

Py:   super().greet()
来源：http://mobile.fktsv.cn/Article/details/gpxizkovv.sHtML

PHP:  parent::greet();
来源：http://m.share.epnwcf.com/Article/details/gylyqmzlh.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gmlkbahmk.sHtML

TS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/gginxqubi.sHtML

Java: super.greet();
来源：http://baike.bbcook.cn/Article/details/gkomuxxyl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fktsv.cn/Article/details/gyrtxtdiq.sHtML

Ruby: super
来源：http://baike.vehdjk.com/Article/details/giiwskdub.sHtML

C#:   base.Greet();
来源：http://www.m.share.bbcook.cn/Article/details/geooyoeai.sHtML

[G08] 静态方法与属性
来源：http://mobile.yfazqb.com/Article/details/gfnowghtt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.tarul.cn/Article/details/gunxkbptx.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/gnykjzvmh.sHtML

JS:   static f() {}
来源：http://m.share.tarul.cn/Article/details/gpopywcgb.sHtML

TS:   static f(): void {}
来源：http://www.m.share.tarul.cn/Article/details/goidgctfw.sHtML

Java: static void f() {}
来源：http://www.share.yfazqb.com/Article/details/gswqiptmn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.yfazqb.com/Article/details/gjzepipyi.sHtML

Ruby: def self.f; end
来源：http://baike.bbcook.cn/Article/details/gsmrmljig.sHtML

C#:   public static void F() {}
来源：http://m.share.bbcook.cn/Article/details/gvoroepas.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.epnwcf.com/Article/details/ghctoixum.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.vehdjk.com/Article/details/gdyagbfwe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.epnwcf.com/Article/details/gfgcggfgh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fktsv.cn/Article/details/gyxsueadb.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fktsv.cn/Article/details/gomyaxzht.sHtML

Java: interface Shape { double area(); }
来源：http://3g.sjlbkw.cn/Article/details/glwivzoer.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.tarul.cn/Article/details/gbfslwuqp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fktsv.cn/Article/details/gftmsiyzj.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.epnwcf.com/Article/details/geaneugcw.sHtML

[G10] 访问控制
来源：http://read.share.tarul.cn/Article/details/glzuiilxk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.bbcook.cn/Article/details/gilcltvfz.sHtML

PHP:  public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gdwkbokqc.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.yfazqb.com/Article/details/gkutlocjw.sHtML

TS:   public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/glrymiewj.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.epnwcf.com/Article/details/gnkclbvai.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.sjlbkw.cn/Article/details/gvjuedtcb.sHtML

Ruby: public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gewyuxoan.sHtML

C#:   public / protected / private / internal
来源：http://read.share.yfazqb.com/Article/details/glvvzqwsm.sHtML

[G11] getter / setter
来源：http://mobile.bbcook.cn/Article/details/gapuoylxi.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.yfazqb.com/Article/details/guwhhrnoi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gpavhxddj.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/gywfraqmd.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/gthmvxflo.sHtML

Java: public String getName() { return name; }
来源：http://3g.vehdjk.com/Article/details/gleppshkv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gpxexyhtx.sHtML

Ruby: attr_accessor :name
来源：http://3g.sjlbkw.cn/Article/details/gsyfuuwbj.sHtML

C#:   public string Name { get; set; }
来源：http://3g.vehdjk.com/Article/details/gihmjrbyk.sHtML

[G12] 对象转字符串
来源：http://baike.sjlbkw.cn/Article/details/gvpduqezm.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gpiofsuqq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gfynxnabu.sHtML

JS:   toString() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gbxljxeop.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gsllwtyyv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gndpozxzm.sHtML


<!-- 参考信息 -->