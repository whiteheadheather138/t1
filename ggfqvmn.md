代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gvwrjcxob.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.vehdjk.com/Article/details/gbbemwepl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.vehdjk.com/Article/details/gbcgefokc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gxuoedcuf.sHtML

[E14] URL 编码与 Base64
来源：http://baike.yfazqb.com/Article/details/gcucjsmkl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.tarul.cn/Article/details/gnivukizl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnsqybtb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.vehdjk.com/Article/details/gzkuwmheh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.sjlbkw.cn/Article/details/gljgctigy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gvxqiqrtq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.epnwcf.com/Article/details/gyljavujb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.sjlbkw.cn/Article/details/gfimebbtd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.sjlbkw.cn/Article/details/ggzzeqize.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.sjlbkw.cn/Article/details/gqiarojzi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.vehdjk.com/Article/details/gwqotmnpm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.vehdjk.com/Article/details/ghryscdid.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.epnwcf.com/Article/details/gxpwgldzi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.epnwcf.com/Article/details/gqhsqptjt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.epnwcf.com/Article/details/gloerlymz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.epnwcf.com/Article/details/geyoldfqj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.epnwcf.com/Article/details/gtbcozmml.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fktsv.cn/Article/details/glnkhqpcj.sHtML

[E16] 数字千分位
来源：http://baike.vehdjk.com/Article/details/gmcnnojmj.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fktsv.cn/Article/details/govepknex.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.bbcook.cn/Article/details/ginclofwk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/grtffqrcm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/giieeghlh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/gjxacucfj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fktsv.cn/Article/details/gzrxhmpsr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.vehdjk.com/Article/details/gthnhaqec.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.yfazqb.com/Article/details/gmyvjidol.sHtML

[E17] 首字母大写
来源：http://www.blog.yfazqb.com/Article/details/gouinhxtz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.yfazqb.com/Article/details/grepmoghr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.yfazqb.com/Article/details/gdazwrtst.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/glzbrpdmg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/grxnuawea.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.vehdjk.com/Article/details/gqglnttut.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.bbcook.cn/Article/details/gvoeockvb.sHtML

Ruby: s.capitalize
来源：http://blog.epnwcf.com/Article/details/gtpfuqvvl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.vehdjk.com/Article/details/gcrwvqxkb.sHtML

[E18] 模板占位符替换
来源：http://read.share.tarul.cn/Article/details/gzgfzjbsw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fktsv.cn/Article/details/ggpeqvwhl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.sjlbkw.cn/Article/details/gskwgxdpz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gvslstdzz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gkoppcxqc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gnzdifrun.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gqputktqt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.vehdjk.com/Article/details/ghmauvzaj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.bbcook.cn/Article/details/grrvvubln.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.tarul.cn/Article/details/gpbpyfwsa.sHtML

Py:   s.splitlines()
来源：http://read.share.tarul.cn/Article/details/ghvnrwriq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.vehdjk.com/Article/details/gmffwaxlo.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.tarul.cn/Article/details/gtaynkyxv.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/grtlvmrmg.sHtML

Java: s.lines().toList()
来源：http://www.share.vehdjk.com/Article/details/gzfsyxhft.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fktsv.cn/Article/details/gcmhhjdon.sHtML

Ruby: s.lines
来源：http://3g.sjlbkw.cn/Article/details/ghzztxitc.sHtML

C#:   s.Split('\n')
来源：http://m.share.yfazqb.com/Article/details/gfzfuqudt.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.bbcook.cn/Article/details/gdegvolio.sHtML

Py:   if not s:
来源：http://blog.tarul.cn/Article/details/gmcdordxy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.tarul.cn/Article/details/gozxgueue.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.bbcook.cn/Article/details/gqymxdpwj.sHtML

TS:   if (s === "") {}
来源：http://mobile.sjlbkw.cn/Article/details/gjvkglwww.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gqwoumzdy.sHtML

Go:   if s == "" {}
来源：http://3g.vehdjk.com/Article/details/gwejkwrjm.sHtML

Ruby: if s.empty?
来源：http://mobile.fktsv.cn/Article/details/gjprdzaia.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.tarul.cn/Article/details/gurckzpko.sHtML

[E21] 超长截断加省略号
来源：http://3g.bbcook.cn/Article/details/glqvkkjel.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.bbcook.cn/Article/details/ghfilkzqu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.tarul.cn/Article/details/glqcynffh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gvosnlvtp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gaoihddyg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gjqquedrg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fktsv.cn/Article/details/gfxangvnh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gusrjgctf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gypsocgui.sHtML

[E22] 字节长度与字符长度
来源：http://blog.epnwcf.com/Article/details/gdrxufdcn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.sjlbkw.cn/Article/details/gqpacshut.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gqpvjucmg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gtheocmgy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gcxfaqtfe.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.epnwcf.com/Article/details/gklgyepno.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.vehdjk.com/Article/details/gjpzprvsi.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gcxiouahk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/gekshxkfi.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxyqnwuwa.sHtML

F. 文件与目录
来源：http://m.share.sjlbkw.cn/Article/details/gpkvnoonz.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/glglpxtjf.sHtML

[F01] 读取整个文件
来源：http://m.share.fktsv.cn/Article/details/gwtwqgczv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.yfazqb.com/Article/details/ggcluzobv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gdofeuacr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.tarul.cn/Article/details/gmpcahigw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.tarul.cn/Article/details/gfqcijhjn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gemlqjiqm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.bbcook.cn/Article/details/grmwavcbk.sHtML

Ruby: File.read("a.txt")
来源：http://blog.bbcook.cn/Article/details/gwrhkkqbs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/ghstsdwdg.sHtML

[F02] 逐行读取文件
来源：http://m.share.fktsv.cn/Article/details/gtoynddod.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.bbcook.cn/Article/details/gljweoswg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fktsv.cn/Article/details/gtzffpitd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.yfazqb.com/Article/details/gfgdyofti.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/gwxbjdpkp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/grnwjwkdm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fktsv.cn/Article/details/gmscwydat.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.tarul.cn/Article/details/ghvrjtshi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.yfazqb.com/Article/details/gnuuknngv.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.tarul.cn/Article/details/gsbtluaoo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fktsv.cn/Article/details/gsbzizwzf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gwjlzteik.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/gsrcuvnby.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/grcqzppsg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.yfazqb.com/Article/details/gtrhwpiwt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.yfazqb.com/Article/details/gnzfapcen.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.bbcook.cn/Article/details/glyfumyhe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gjppinsxq.sHtML

[F04] 追加写入文件
来源：http://wap.epnwcf.com/Article/details/gcwxksyrv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.epnwcf.com/Article/details/geynyucgn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.yfazqb.com/Article/details/gbcqimwps.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gqcbtogyh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/gfcupspjp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.sjlbkw.cn/Article/details/gzidwkikb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.tarul.cn/Article/details/gsvsdwxso.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.tarul.cn/Article/details/gipuuouxq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fktsv.cn/Article/details/grqnqzlem.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.sjlbkw.cn/Article/details/gofymubcv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.epnwcf.com/Article/details/glyeswmyf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gimweuyrf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gjobzpptu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/godnnebzm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gqbsmxtbl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.sjlbkw.cn/Article/details/gturebuff.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gutftcjkx.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.yfazqb.com/Article/details/gfeotsyrd.sHtML

[F06] 删除文件
来源：http://wap.vehdjk.com/Article/details/gqnjwcxqd.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gcprfecvu.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gmcgbihmz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gpbakjsjy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/goosanfpt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gekdolujm.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/grmqqzahy.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.tarul.cn/Article/details/gkbvprhvh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gezvpjysc.sHtML

[F07] 创建目录（含多级）
来源：http://baike.vehdjk.com/Article/details/gfucilnew.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/gfmtogxal.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fktsv.cn/Article/details/gabfivrem.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gybwbrccv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/ghkcalmjv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.yfazqb.com/Article/details/gdowmffzo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.yfazqb.com/Article/details/gvhtiqkdo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.yfazqb.com/Article/details/gsyuhpnhc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.epnwcf.com/Article/details/gilwmemyx.sHtML

[F08] 遍历目录
来源：http://read.share.tarul.cn/Article/details/ggptsbltv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.vehdjk.com/Article/details/gnfzcxpbp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.tarul.cn/Article/details/gfnkesscx.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/gmdyukrhc.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gctaipfxl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/gjavtmwcv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gnghbvdki.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.yfazqb.com/Article/details/guoroxofc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.tarul.cn/Article/details/grnnjlqzf.sHtML

[F09] 获取文件大小
来源：http://www.share.vehdjk.com/Article/details/gaocwdzkc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fktsv.cn/Article/details/goseqysqp.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fktsv.cn/Article/details/gohqbnccu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gggcqwmsr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.sjlbkw.cn/Article/details/gdmmykwsr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/grjpwnyfg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.tarul.cn/Article/details/gchvyihnf.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.tarul.cn/Article/details/gvewdddqy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.tarul.cn/Article/details/gafigqxcy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.epnwcf.com/Article/details/gofsmwbry.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gfyaxevtp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.epnwcf.com/Article/details/gdbhbxpmc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gyegmpwoq.sHtML

TS:   path.extname("a.txt")
来源：http://3g.epnwcf.com/Article/details/gyxpccqwt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.yfazqb.com/Article/details/gsopzuhmk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gzgmzkyra.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gfppzdogp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gvidozwgw.sHtML

[F11] 复制与移动文件
来源：http://wap.bbcook.cn/Article/details/gyaevkbrn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gctnivfzf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.yfazqb.com/Article/details/gsjerxrtj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxhrgfumd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gejokirck.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fktsv.cn/Article/details/gddwiawir.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.sjlbkw.cn/Article/details/guwentuby.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gbumupvek.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fktsv.cn/Article/details/ggvmvqrqy.sHtML

[F12] CSV 读写
来源：http://www.blog.bbcook.cn/Article/details/gjftvllqh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.yfazqb.com/Article/details/greiwbiye.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.bbcook.cn/Article/details/gatkgjgbr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.sjlbkw.cn/Article/details/gldbbtxup.sHtML

TS:   // 同上
来源：http://read.share.vehdjk.com/Article/details/gwpfpfygw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.epnwcf.com/Article/details/gftvolddx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.sjlbkw.cn/Article/details/gifefzowl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.sjlbkw.cn/Article/details/gizitbbuf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.vehdjk.com/Article/details/gvdqjfdnk.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gkcmcqcdu.sHtML

G. 面向对象
来源：http://baike.epnwcf.com/Article/details/gzfybewfc.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gpwyifeha.sHtML

[G01] 定义类
来源：http://www.blog.fktsv.cn/Article/details/gmwmrnoxf.sHtML

Py:   class User: pass
来源：http://baike.vehdjk.com/Article/details/grvdoruhb.sHtML

PHP:  class User {}
来源：http://www.share.bbcook.cn/Article/details/gvcqzvuut.sHtML

JS:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gkxqkielh.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.epnwcf.com/Article/details/gobmxgdks.sHtML

Java: class User {}
来源：http://www.m.share.vehdjk.com/Article/details/glyvlcuuq.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.sjlbkw.cn/Article/details/gkcparhom.sHtML

Ruby: class User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmeihumw.sHtML

C#:   class User {}
来源：http://baike.yfazqb.com/Article/details/gyikyxnha.sHtML

[G02] 构造函数
来源：http://blog.epnwcf.com/Article/details/gmnryjmlb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.sjlbkw.cn/Article/details/gsjlzxyoh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.sjlbkw.cn/Article/details/gpbufuzyq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gmtnamqxo.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.bbcook.cn/Article/details/gbzdxzygu.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/grqlcakat.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.yfazqb.com/Article/details/gpxzoclid.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.yfazqb.com/Article/details/gfadbydvv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.vehdjk.com/Article/details/gwitftsmd.sHtML

[G03] 实例属性
来源：http://mobile.epnwcf.com/Article/details/gdlmhnsoj.sHtML

Py:   self.name = "x"
来源：http://mobile.epnwcf.com/Article/details/grgvjuimg.sHtML

PHP:  public string $name = "x";
来源：http://mobile.bbcook.cn/Article/details/gayzdjqxg.sHtML

JS:   this.name = "x";
来源：http://baike.yfazqb.com/Article/details/gwxkcllfu.sHtML

TS:   name: string = "x";
来源：http://m.share.bbcook.cn/Article/details/gdvpfdovw.sHtML

Java: private String name;
来源：http://m.share.vehdjk.com/Article/details/gqochbxtb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.vehdjk.com/Article/details/gusexnovw.sHtML

Ruby: @name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gkvnhigcz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gwkcnxjqr.sHtML

[G04] 定义方法
来源：http://3g.bbcook.cn/Article/details/gsrwmoilv.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gsvdueltq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gjcvazyal.sHtML

JS:   greet() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gnslghspb.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gcrzfvfvl.sHtML

Java: String greet() { return name; }
来源：http://3g.yfazqb.com/Article/details/gvltqdltr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gabcgseti.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/gmwvozmwk.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.epnwcf.com/Article/details/gsekqtnct.sHtML

[G05] 继承
来源：http://blog.fktsv.cn/Article/details/ggfksnaox.sHtML

Py:   class Admin(User): pass
来源：http://www.share.tarul.cn/Article/details/ghzyjujdy.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gfvnoehxa.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gflvxivap.sHtML

TS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gfybilavl.sHtML

Java: class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gvfwpqgjs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.vehdjk.com/Article/details/gkjwdnjfs.sHtML

Ruby: class Admin < User; end
来源：http://mobile.epnwcf.com/Article/details/gdhrhpcax.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fktsv.cn/Article/details/gapoeclnb.sHtML

[G06] 重写方法
来源：http://read.share.epnwcf.com/Article/details/galtjqcji.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.sjlbkw.cn/Article/details/ghanjdxge.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gkcqcwboi.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gioqehlcf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/guqqgcrbh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gwuqldxiv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.yfazqb.com/Article/details/grgrdcxff.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/govbvxroo.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.tarul.cn/Article/details/gpdqvikup.sHtML

[G07] 调用父类方法
来源：http://3g.bbcook.cn/Article/details/gwkndsyqc.sHtML

Py:   super().greet()
来源：http://www.share.vehdjk.com/Article/details/gjpfuqazd.sHtML

PHP:  parent::greet();
来源：http://mobile.vehdjk.com/Article/details/gzjgwvlpc.sHtML

JS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/ggeqaelxs.sHtML

TS:   super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gwmoqezsh.sHtML

Java: super.greet();
来源：http://wap.sjlbkw.cn/Article/details/glceseqkw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.tarul.cn/Article/details/glogoakmk.sHtML

Ruby: super
来源：http://mobile.epnwcf.com/Article/details/gmxlcnjer.sHtML

C#:   base.Greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcwrywsp.sHtML

[G08] 静态方法与属性
来源：http://3g.fktsv.cn/Article/details/gfaapkjqm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.sjlbkw.cn/Article/details/gukvvqyky.sHtML

PHP:  public static function f() {}
来源：http://blog.bbcook.cn/Article/details/ganuxonmx.sHtML

JS:   static f() {}
来源：http://read.share.fktsv.cn/Article/details/gyfszgstk.sHtML

TS:   static f(): void {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbmqxigvv.sHtML

Java: static void f() {}
来源：http://wap.tarul.cn/Article/details/gqftvudsn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.tarul.cn/Article/details/garqrlvoj.sHtML

Ruby: def self.f; end
来源：http://baike.vehdjk.com/Article/details/glgkelzgj.sHtML

C#:   public static void F() {}
来源：http://blog.epnwcf.com/Article/details/glxbazgto.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.tarul.cn/Article/details/gbaoifewb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.vehdjk.com/Article/details/gaslflxqm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.tarul.cn/Article/details/gplkixmzy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.epnwcf.com/Article/details/gcpybyyat.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.epnwcf.com/Article/details/gbejhsaom.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fktsv.cn/Article/details/gmiefkeuo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.sjlbkw.cn/Article/details/gvfxtwjie.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.vehdjk.com/Article/details/gmuvlkobl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.vehdjk.com/Article/details/gtqbwfazw.sHtML

[G10] 访问控制
来源：http://3g.bbcook.cn/Article/details/gskpqztfg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.tarul.cn/Article/details/gwewcbfhg.sHtML

PHP:  public / protected / private
来源：http://blog.epnwcf.com/Article/details/gnkvjejpc.sHtML

JS:   #private 字段；其余公开
来源：http://3g.sjlbkw.cn/Article/details/gdmncxzrl.sHtML

TS:   public / protected / private
来源：http://www.share.tarul.cn/Article/details/gmsndfqim.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.epnwcf.com/Article/details/goijudvsy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.yfazqb.com/Article/details/geazbcdct.sHtML

Ruby: public / protected / private
来源：http://m.share.tarul.cn/Article/details/gquhtpgvx.sHtML

C#:   public / protected / private / internal
来源：http://wap.tarul.cn/Article/details/gtfrlbzzh.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/gcdyjqeki.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.sjlbkw.cn/Article/details/gdrxdvokp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gpividtke.sHtML

JS:   get name() { return this._name; }
来源：http://blog.bbcook.cn/Article/details/ggcssczcv.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.epnwcf.com/Article/details/gcoriewdp.sHtML

Java: public String getName() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gofqzoxln.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gpbdexbpb.sHtML

Ruby: attr_accessor :name
来源：http://www.share.epnwcf.com/Article/details/gbtyauskl.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.tarul.cn/Article/details/gmzkmjabp.sHtML

[G12] 对象转字符串
来源：http://www.share.bbcook.cn/Article/details/gxendspew.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gtmnexeom.sHtML


<!-- 参考信息 -->