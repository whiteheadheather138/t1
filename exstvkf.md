代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gvsedvidr.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fktsv.cn/Article/details/gfaazrrcs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.epnwcf.com/Article/details/gfadzqisv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.bbcook.cn/Article/details/guexddlno.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.vehdjk.com/Article/details/gtkdbqvet.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.bbcook.cn/Article/details/gouyqstnh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.sjlbkw.cn/Article/details/geivzxzeq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.yfazqb.com/Article/details/gtjbuhkou.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.epnwcf.com/Article/details/gspvxikoh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.tarul.cn/Article/details/ghpmiuowj.sHtML

[E16] 数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gfktzfqlb.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.vehdjk.com/Article/details/gfruiytpn.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fktsv.cn/Article/details/gtglbnsfw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/gmqbfjsky.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/giqapejxe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.vehdjk.com/Article/details/gwrjvgizt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.tarul.cn/Article/details/ggtbdvuoi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.bbcook.cn/Article/details/gwnfajhgv.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.yfazqb.com/Article/details/gxiegxrnt.sHtML

[E17] 首字母大写
来源：http://m.share.tarul.cn/Article/details/gfzahaoew.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.bbcook.cn/Article/details/glyjoswrw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.yfazqb.com/Article/details/guuygxufo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gxvparqbm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/gbhxakooi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.tarul.cn/Article/details/gpklsupop.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gfzvtawpi.sHtML

Ruby: s.capitalize
来源：http://mobile.tarul.cn/Article/details/gyjulypyw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.bbcook.cn/Article/details/gwghntvnq.sHtML

[E18] 模板占位符替换
来源：http://mobile.vehdjk.com/Article/details/ggegbtocn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.epnwcf.com/Article/details/gwubwverr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.vehdjk.com/Article/details/gobrhrzsc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gukrfwwqo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/grizlljun.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gwdmubyjr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gdmdiuhle.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.tarul.cn/Article/details/gtuqgtqds.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.sjlbkw.cn/Article/details/gnpsyvzvi.sHtML

[E19] 多行文本按行拆分
来源：http://blog.sjlbkw.cn/Article/details/giqhdafxg.sHtML

Py:   s.splitlines()
来源：http://3g.vehdjk.com/Article/details/gqzocbimd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.epnwcf.com/Article/details/ggapzpftf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.tarul.cn/Article/details/gdtxgibtv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gxmtcbbcw.sHtML

Java: s.lines().toList()
来源：http://read.share.yfazqb.com/Article/details/gmlihkzye.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.tarul.cn/Article/details/gluqmduap.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/gslvpgpzc.sHtML

C#:   s.Split('\n')
来源：http://baike.tarul.cn/Article/details/glkecoxin.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.bbcook.cn/Article/details/ghqtcdalk.sHtML

Py:   if not s:
来源：http://baike.tarul.cn/Article/details/gxbuitewk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.epnwcf.com/Article/details/guzpurijj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.bbcook.cn/Article/details/ghwicbzhx.sHtML

TS:   if (s === "") {}
来源：http://wap.vehdjk.com/Article/details/gwmcicwsj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gcmpeqohu.sHtML

Go:   if s == "" {}
来源：http://mobile.epnwcf.com/Article/details/gpvcmmmch.sHtML

Ruby: if s.empty?
来源：http://www.blog.epnwcf.com/Article/details/gcxylknxg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/gmfpscnii.sHtML

[E21] 超长截断加省略号
来源：http://mobile.yfazqb.com/Article/details/gwuucdctq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.tarul.cn/Article/details/ghgatslqy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gnuxghlcr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gwbsxldpj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/geqgjicpb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gbtcvlwsp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.tarul.cn/Article/details/gzgxnlsbb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gubipnmzb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gzngcqunv.sHtML

[E22] 字节长度与字符长度
来源：http://blog.tarul.cn/Article/details/giiezegbi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.tarul.cn/Article/details/guxxhksfk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/guagkzghi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/gzifabotd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gphatbmba.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.vehdjk.com/Article/details/gvtnmdaqy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fktsv.cn/Article/details/gspvkkljf.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.bbcook.cn/Article/details/gacdzfluo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.tarul.cn/Article/details/gkfcaolzj.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gqucgylwh.sHtML

F. 文件与目录
来源：http://3g.epnwcf.com/Article/details/gtxizvofc.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gioxpkwcj.sHtML

[F01] 读取整个文件
来源：http://mobile.tarul.cn/Article/details/gwotxstpw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.bbcook.cn/Article/details/gytojswds.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gdnbvntte.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.yfazqb.com/Article/details/giikcqocz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.epnwcf.com/Article/details/gzszyomlp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/giyqmkxhg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwxfpnhu.sHtML

Ruby: File.read("a.txt")
来源：http://wap.epnwcf.com/Article/details/grimygtru.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gmnrszecg.sHtML

[F02] 逐行读取文件
来源：http://m.share.epnwcf.com/Article/details/gwndeirdv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.yfazqb.com/Article/details/gbsjscfvh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.yfazqb.com/Article/details/glajuuabb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.yfazqb.com/Article/details/goyjdjyfz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.yfazqb.com/Article/details/giwcpenkr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/gpmylldlg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fktsv.cn/Article/details/gkmzicvck.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/gyohncgbe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.vehdjk.com/Article/details/gayjefiot.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.vehdjk.com/Article/details/gzkgmujtn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gqjujvent.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.sjlbkw.cn/Article/details/glyvgmcub.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/gmcxmlvdy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/gghzcjjjb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.bbcook.cn/Article/details/gotjyypdg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.sjlbkw.cn/Article/details/gpsotaxou.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.epnwcf.com/Article/details/gbyjfekxf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gbetixvlj.sHtML

[F04] 追加写入文件
来源：http://mobile.tarul.cn/Article/details/gkzfwobjz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fktsv.cn/Article/details/goaqcoysy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fktsv.cn/Article/details/goqzgslan.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gszpncyjd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/glfapoznn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fktsv.cn/Article/details/gjkezuayl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.tarul.cn/Article/details/gekcuapsu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.vehdjk.com/Article/details/gzcmxrnmi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.tarul.cn/Article/details/guuibpdkw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gcihfnjbg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.bbcook.cn/Article/details/gzgvmieyc.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.epnwcf.com/Article/details/grzsoyxmj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/ghudjfpsz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gapqmkuhf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gbrlkmkqr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.tarul.cn/Article/details/gxvdllxux.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gvkjcwuhp.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gxcfuruop.sHtML

[F06] 删除文件
来源：http://www.share.yfazqb.com/Article/details/gsrppcxrn.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gszfpbklp.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gaufnukjh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gjchhtjgj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gdxylhnda.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gsjdokakd.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gofzuoant.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.vehdjk.com/Article/details/ggxrsmpoc.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gkbsumagr.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.tarul.cn/Article/details/gisymodjx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.tarul.cn/Article/details/glfzpwdpy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.bbcook.cn/Article/details/gctcpfuln.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gskafwpio.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gkfgsnagf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fktsv.cn/Article/details/gvahtismh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.vehdjk.com/Article/details/gnqesbjzr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.tarul.cn/Article/details/gegrpjvqo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.epnwcf.com/Article/details/gomnkzvuz.sHtML

[F08] 遍历目录
来源：http://mobile.epnwcf.com/Article/details/gzjitrdor.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.bbcook.cn/Article/details/gyecshnjw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.epnwcf.com/Article/details/geolrsytt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/grozzkece.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.sjlbkw.cn/Article/details/gvcolldfs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/grkvpxxlx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.epnwcf.com/Article/details/gytbrfuyw.sHtML

Ruby: Dir.children("dir")
来源：http://baike.yfazqb.com/Article/details/gbsglpdvq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.bbcook.cn/Article/details/goivktboh.sHtML

[F09] 获取文件大小
来源：http://wap.sjlbkw.cn/Article/details/gbnmqhchq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/ggfiyffhd.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gjetoiyzx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gkxubnqgn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gcyhjtqeh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gfhmldxwq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.tarul.cn/Article/details/gdltxfenm.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gmwpkimth.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.epnwcf.com/Article/details/gvpalomkd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.vehdjk.com/Article/details/gsorznyoo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gwnykmupn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.vehdjk.com/Article/details/gdijftlve.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gkdsojrij.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gtiamslok.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.vehdjk.com/Article/details/gvawzdgxa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gvbqvaqvo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gxzhooanw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gdvhiirds.sHtML

[F11] 复制与移动文件
来源：http://m.share.vehdjk.com/Article/details/gpgtqlnjx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/ghctlceee.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.tarul.cn/Article/details/gpgkubost.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/ghsmtesdt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gmhmyhjgb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fktsv.cn/Article/details/glagtmzjw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.vehdjk.com/Article/details/gltyzetsc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gqktljmfj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.epnwcf.com/Article/details/gjwghdjwn.sHtML

[F12] CSV 读写
来源：http://baike.tarul.cn/Article/details/gmrfrdyht.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.epnwcf.com/Article/details/ggngjjupb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fktsv.cn/Article/details/grohmarir.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.vehdjk.com/Article/details/ghsvxqrtz.sHtML

TS:   // 同上
来源：http://www.blog.tarul.cn/Article/details/gyfpvwado.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.vehdjk.com/Article/details/gpqpesyjf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.vehdjk.com/Article/details/gjaobvvkm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.epnwcf.com/Article/details/gbzzvniqu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.tarul.cn/Article/details/geegibyvb.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gclqizyid.sHtML

G. 面向对象
来源：http://www.blog.vehdjk.com/Article/details/gquuyljui.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gryjxqvgc.sHtML

[G01] 定义类
来源：http://www.blog.vehdjk.com/Article/details/gqilqgdmo.sHtML

Py:   class User: pass
来源：http://m.share.epnwcf.com/Article/details/gazuvoloi.sHtML

PHP:  class User {}
来源：http://mobile.fktsv.cn/Article/details/gamarcjyp.sHtML

JS:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gtnxufsgt.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.tarul.cn/Article/details/gjgnvxdlf.sHtML

Java: class User {}
来源：http://blog.sjlbkw.cn/Article/details/gpplowkng.sHtML

Go:   type User struct { Name string }
来源：http://blog.vehdjk.com/Article/details/ggjxedynz.sHtML

Ruby: class User; end
来源：http://blog.fktsv.cn/Article/details/glvchlouv.sHtML

C#:   class User {}
来源：http://blog.bbcook.cn/Article/details/grxqpqkok.sHtML

[G02] 构造函数
来源：http://read.share.epnwcf.com/Article/details/gibvtxsbl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.tarul.cn/Article/details/grqggxtnx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.yfazqb.com/Article/details/gjhkryfcu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/gxanzsqka.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.epnwcf.com/Article/details/guazwtedg.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/ggeuwljaw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.tarul.cn/Article/details/geowribyt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.bbcook.cn/Article/details/gyxndmgmg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.tarul.cn/Article/details/gjvqrjtyx.sHtML

[G03] 实例属性
来源：http://www.blog.bbcook.cn/Article/details/geuvmthtq.sHtML

Py:   self.name = "x"
来源：http://baike.tarul.cn/Article/details/gzygpsukf.sHtML

PHP:  public string $name = "x";
来源：http://mobile.vehdjk.com/Article/details/gszdncrql.sHtML

JS:   this.name = "x";
来源：http://m.share.tarul.cn/Article/details/gikijyokq.sHtML

TS:   name: string = "x";
来源：http://baike.fktsv.cn/Article/details/gelhmmssh.sHtML

Java: private String name;
来源：http://www.share.fktsv.cn/Article/details/gkxgwkpnk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.bbcook.cn/Article/details/gleknowoz.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gomflpjet.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.tarul.cn/Article/details/goafylmop.sHtML

[G04] 定义方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjffrohm.sHtML

Py:   def greet(self): return self.name
来源：http://wap.bbcook.cn/Article/details/govzyymkl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/grmhgvlby.sHtML

JS:   greet() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gltzhdgln.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gkznmhonz.sHtML

Java: String greet() { return name; }
来源：http://3g.tarul.cn/Article/details/gwmhbqfgt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gjuleovhn.sHtML

Ruby: def greet; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gwlmlrzmr.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.tarul.cn/Article/details/gqycswwof.sHtML

[G05] 继承
来源：http://blog.bbcook.cn/Article/details/gqcemfvit.sHtML

Py:   class Admin(User): pass
来源：http://blog.fktsv.cn/Article/details/gvjuadwxi.sHtML

PHP:  class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/ghfqoleit.sHtML

JS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gsolroorv.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gitmvaqoe.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gqlojjvkh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fktsv.cn/Article/details/gaoivgqmn.sHtML

Ruby: class Admin < User; end
来源：http://www.share.tarul.cn/Article/details/glytxrejw.sHtML

C#:   class Admin : User {}
来源：http://3g.tarul.cn/Article/details/gciljzjqs.sHtML

[G06] 重写方法
来源：http://read.share.yfazqb.com/Article/details/gpqhrtlfx.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.epnwcf.com/Article/details/gbplpwkbj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gfuoswqxs.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/grchghshi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gphulbfsp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gtmkzxdbu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.bbcook.cn/Article/details/gjzbuxryo.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.tarul.cn/Article/details/gnznlzvhv.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.sjlbkw.cn/Article/details/gwcsihytz.sHtML

[G07] 调用父类方法
来源：http://read.share.vehdjk.com/Article/details/gwunopgcr.sHtML

Py:   super().greet()
来源：http://baike.bbcook.cn/Article/details/gftlddjwk.sHtML

PHP:  parent::greet();
来源：http://www.blog.vehdjk.com/Article/details/grqlhgbsb.sHtML

JS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/guburvgdd.sHtML

TS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gyzvccpoc.sHtML

Java: super.greet();
来源：http://m.share.fktsv.cn/Article/details/gqthtjicj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fktsv.cn/Article/details/grfpqizdb.sHtML

Ruby: super
来源：http://m.share.epnwcf.com/Article/details/grfzybefa.sHtML

C#:   base.Greet();
来源：http://www.m.share.fktsv.cn/Article/details/gjbbvtndm.sHtML

[G08] 静态方法与属性
来源：http://www.share.epnwcf.com/Article/details/gylnsruqx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.epnwcf.com/Article/details/grlitmaqo.sHtML

PHP:  public static function f() {}
来源：http://3g.sjlbkw.cn/Article/details/ghotwofkk.sHtML

JS:   static f() {}
来源：http://www.blog.vehdjk.com/Article/details/gchywqqpe.sHtML

TS:   static f(): void {}
来源：http://read.share.bbcook.cn/Article/details/girxjhfkj.sHtML

Java: static void f() {}
来源：http://www.blog.tarul.cn/Article/details/gjomaxpbc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.bbcook.cn/Article/details/gnsuraybn.sHtML

Ruby: def self.f; end
来源：http://www.m.share.epnwcf.com/Article/details/gzpbuvslw.sHtML

C#:   public static void F() {}
来源：http://mobile.yfazqb.com/Article/details/gxiunjqbl.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/gqmedfoga.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.tarul.cn/Article/details/gwqjrlsyz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.sjlbkw.cn/Article/details/gjuqsbedb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.yfazqb.com/Article/details/gwnvgudod.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fktsv.cn/Article/details/grnfgzedx.sHtML

Java: interface Shape { double area(); }
来源：http://wap.tarul.cn/Article/details/gpsxfibgu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fktsv.cn/Article/details/gbupjppwy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.epnwcf.com/Article/details/grmqvuthx.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.vehdjk.com/Article/details/ggmqroumw.sHtML

[G10] 访问控制
来源：http://mobile.yfazqb.com/Article/details/gtkzuskoe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.tarul.cn/Article/details/gaazycupz.sHtML

PHP:  public / protected / private
来源：http://m.share.bbcook.cn/Article/details/ggxzwluih.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.bbcook.cn/Article/details/gglbnkjuu.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/gqleoyteh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.yfazqb.com/Article/details/gjysfdbzr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.epnwcf.com/Article/details/gcllpayjw.sHtML

Ruby: public / protected / private
来源：http://www.share.tarul.cn/Article/details/giklyfzda.sHtML

C#:   public / protected / private / internal
来源：http://blog.bbcook.cn/Article/details/gpsbtzdol.sHtML

[G11] getter / setter
来源：http://3g.yfazqb.com/Article/details/gqxjaepus.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.sjlbkw.cn/Article/details/gpgyvjggw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gxxvhhapz.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gzydndkcg.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.tarul.cn/Article/details/gzmrddajs.sHtML

Java: public String getName() { return name; }
来源：http://m.share.vehdjk.com/Article/details/gzaisuzec.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gpopkgmgd.sHtML

Ruby: attr_accessor :name
来源：http://3g.sjlbkw.cn/Article/details/glfhugboy.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.tarul.cn/Article/details/gcqomtuvj.sHtML

[G12] 对象转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gwyobbkgx.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/gayuutkpr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/goexkdamz.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gqqjfgoer.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gyhzbildp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gwdzvdkiv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/guiooosvw.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gzjeizdrf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gufnmuimu.sHtML

[G13] 判断对象类型
来源：http://3g.tarul.cn/Article/details/glibhebvj.sHtML

Py:   isinstance(u, User)
来源：http://m.share.yfazqb.com/Article/details/gxmwgnrgp.sHtML

PHP:  $u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gwnjbpcnf.sHtML

JS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gimffgwkh.sHtML

TS:   u instanceof User
来源：http://3g.vehdjk.com/Article/details/gnxmbahmj.sHtML


<!-- 参考信息 -->