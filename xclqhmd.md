代发 wailian999

PHP:  number_format(1234567);
来源：http://baike.bbcook.cn/Article/details/gwwxcnhze.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/gfoqzxker.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gtlorgiaz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.sjlbkw.cn/Article/details/grkronrkh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fktsv.cn/Article/details/giqrfncdf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fktsv.cn/Article/details/ghbovpzmq.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.sjlbkw.cn/Article/details/gzfdhnxqa.sHtML

[E17] 首字母大写
来源：http://www.m.share.yfazqb.com/Article/details/garggklcz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.bbcook.cn/Article/details/gsskyrrgx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fktsv.cn/Article/details/gojjtjklz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/gkrpkpzgs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.sjlbkw.cn/Article/details/glunwfhvn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.epnwcf.com/Article/details/gmtypttto.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fktsv.cn/Article/details/guhguexnn.sHtML

Ruby: s.capitalize
来源：http://www.share.fktsv.cn/Article/details/gkeznoduf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.bbcook.cn/Article/details/gqirgyvfd.sHtML

[E18] 模板占位符替换
来源：http://mobile.fktsv.cn/Article/details/glasiwcvr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.tarul.cn/Article/details/goauxzcvv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.epnwcf.com/Article/details/gwsgfopdm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/giedwrhgy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gjgxvtyxw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gyqtpykde.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gqtbrbshy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.tarul.cn/Article/details/gmftmpecq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.vehdjk.com/Article/details/gpsemsixj.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.yfazqb.com/Article/details/gdcvpgane.sHtML

Py:   s.splitlines()
来源：http://www.m.share.vehdjk.com/Article/details/gtvyslwln.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.epnwcf.com/Article/details/gxzeqlqkq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gsgkhsicc.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/glnfouobx.sHtML

Java: s.lines().toList()
来源：http://m.share.epnwcf.com/Article/details/givtohrvc.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.yfazqb.com/Article/details/ghyldbxdx.sHtML

Ruby: s.lines
来源：http://m.share.tarul.cn/Article/details/grxlqptcv.sHtML

C#:   s.Split('\n')
来源：http://3g.tarul.cn/Article/details/gpmdaiila.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.vehdjk.com/Article/details/gauvmnqxr.sHtML

Py:   if not s:
来源：http://www.m.share.yfazqb.com/Article/details/gtpntkcgm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.tarul.cn/Article/details/glyqzlqcm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.yfazqb.com/Article/details/gvimafjia.sHtML

TS:   if (s === "") {}
来源：http://blog.tarul.cn/Article/details/gbliwxwqi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/ghdgsrtmf.sHtML

Go:   if s == "" {}
来源：http://blog.yfazqb.com/Article/details/giniiaiwo.sHtML

Ruby: if s.empty?
来源：http://wap.fktsv.cn/Article/details/gjvzovwgd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.bbcook.cn/Article/details/gncmmvjfo.sHtML

[E21] 超长截断加省略号
来源：http://wap.sjlbkw.cn/Article/details/gxquuyzzf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.epnwcf.com/Article/details/gbpnrzgip.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/ggniyphlk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gmkxaldno.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gpbtvolwd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/glrhxtuca.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.vehdjk.com/Article/details/grlooqwbw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/gjavtcvkh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gsnlnfcsd.sHtML

[E22] 字节长度与字符长度
来源：http://baike.sjlbkw.cn/Article/details/gtiiwoned.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.yfazqb.com/Article/details/gyezewfkl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gyxxfebfy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.epnwcf.com/Article/details/gdafziuti.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.yfazqb.com/Article/details/gezrmvpcs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.bbcook.cn/Article/details/gasqvidlb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.bbcook.cn/Article/details/gotzrbtln.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gnrgjvhdy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.epnwcf.com/Article/details/gvzbtkscr.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwiycohyi.sHtML

F. 文件与目录
来源：http://read.share.tarul.cn/Article/details/ggzspeeat.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gxakwravc.sHtML

[F01] 读取整个文件
来源：http://blog.bbcook.cn/Article/details/gxmuclgvl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fktsv.cn/Article/details/gxvgxyqsm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gkaipzpgv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.bbcook.cn/Article/details/gyafldefr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gfigseltd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gsjetyirt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.epnwcf.com/Article/details/grqmsxzpv.sHtML

Ruby: File.read("a.txt")
来源：http://wap.bbcook.cn/Article/details/gwhzocwkz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gfyzfljeg.sHtML

[F02] 逐行读取文件
来源：http://m.share.sjlbkw.cn/Article/details/gmxhakkbq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.vehdjk.com/Article/details/gfrrurgvf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fktsv.cn/Article/details/ggnljgsmu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/grdajowye.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/geokluvjr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/gmcwghsrn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.vehdjk.com/Article/details/gapspodiv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.vehdjk.com/Article/details/gqpaochnx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.vehdjk.com/Article/details/ghnsxkmso.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fktsv.cn/Article/details/gjwezxdzr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.bbcook.cn/Article/details/glhieeqgl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/gbejqjhdh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/ggwuaiegy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gviotishx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gkmvjsqoj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.tarul.cn/Article/details/gcqmgchdp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/gikktoovr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gzugdbcms.sHtML

[F04] 追加写入文件
来源：http://baike.bbcook.cn/Article/details/gftqfdbnh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.bbcook.cn/Article/details/gbmwqvyue.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.sjlbkw.cn/Article/details/gqwtytdzf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gywvwehwf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gjkahwfyy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.vehdjk.com/Article/details/gdczmbqdq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fktsv.cn/Article/details/gpdqwckdk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.tarul.cn/Article/details/gyrjwmyyw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.yfazqb.com/Article/details/gcddivnrf.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.vehdjk.com/Article/details/gazuzxghu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.vehdjk.com/Article/details/gcacqvfzn.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.yfazqb.com/Article/details/gavcdxznp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/goafterxu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gotkyquht.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gtpvldtcg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.sjlbkw.cn/Article/details/geciruhwq.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.tarul.cn/Article/details/grdsxfrzm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxspotlm.sHtML

[F06] 删除文件
来源：http://wap.bbcook.cn/Article/details/gyqiamavi.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/ghmnutcof.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gilklhofq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gsvmavxqd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gxchxhqwa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/goscbivjl.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gkkzkzacr.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gffdjvwzp.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gmxmwgkju.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fktsv.cn/Article/details/gyqqzecar.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gpajsybzh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.bbcook.cn/Article/details/gkegehkbt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.vehdjk.com/Article/details/gcxpskian.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/grtnkvpjv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.sjlbkw.cn/Article/details/gkklhrjhr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.yfazqb.com/Article/details/goxpnleqs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.bbcook.cn/Article/details/gwekyiuix.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fktsv.cn/Article/details/gkwerhacc.sHtML

[F08] 遍历目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwzhryiu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.sjlbkw.cn/Article/details/gfwjsyxlh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fktsv.cn/Article/details/gdlqmvqtn.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gxmvmrtxv.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/gfswzroxp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/gduuwzfin.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.sjlbkw.cn/Article/details/gkwxuyvwu.sHtML

Ruby: Dir.children("dir")
来源：http://baike.tarul.cn/Article/details/gyowcpklc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.yfazqb.com/Article/details/gbnyqoocy.sHtML

[F09] 获取文件大小
来源：http://m.share.vehdjk.com/Article/details/gxifynwca.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gscfywcav.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.tarul.cn/Article/details/getawvudw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gnudvzrfg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.tarul.cn/Article/details/gsjsgihim.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/ghojqmmbf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.vehdjk.com/Article/details/glejruilx.sHtML

Ruby: File.size("a.txt")
来源：http://3g.vehdjk.com/Article/details/gnedhzemr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fktsv.cn/Article/details/gkvnwegpc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.tarul.cn/Article/details/gxvbetfda.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gctmglhtr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fktsv.cn/Article/details/grdzskxgd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/grnbxvmpb.sHtML

TS:   path.extname("a.txt")
来源：http://3g.epnwcf.com/Article/details/gzzqnvrpj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fktsv.cn/Article/details/gnyfbdsoo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gvfficnbl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gawurwaqc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gpczxwsyn.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fktsv.cn/Article/details/gqyfoxuib.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gdfixyzmh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.vehdjk.com/Article/details/guinhvkpi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gpotkwzon.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gcxkfeefc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.yfazqb.com/Article/details/gqbgdsoav.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.vehdjk.com/Article/details/gzrhqybsd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/ghxfiecfp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.yfazqb.com/Article/details/ggayofzzl.sHtML

[F12] CSV 读写
来源：http://baike.tarul.cn/Article/details/gwkgnrmfs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.epnwcf.com/Article/details/gokubgsog.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.epnwcf.com/Article/details/gobyszxjv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.vehdjk.com/Article/details/grnnqpxmq.sHtML

TS:   // 同上
来源：http://mobile.bbcook.cn/Article/details/gfkynybjd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.tarul.cn/Article/details/gziyogdcm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/gdpnahwfs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.bbcook.cn/Article/details/gqqsopesz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.sjlbkw.cn/Article/details/gllgilzyx.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gocmqawsl.sHtML

G. 面向对象
来源：http://www.blog.vehdjk.com/Article/details/gvekjvyht.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gclsdkplb.sHtML

[G01] 定义类
来源：http://www.m.share.epnwcf.com/Article/details/gxjxcgdjm.sHtML

Py:   class User: pass
来源：http://www.share.vehdjk.com/Article/details/gabfgixru.sHtML

PHP:  class User {}
来源：http://www.m.share.tarul.cn/Article/details/gzlolznbo.sHtML

JS:   class User {}
来源：http://wap.epnwcf.com/Article/details/gnmlihjxh.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.bbcook.cn/Article/details/gnpucqcaf.sHtML

Java: class User {}
来源：http://www.share.epnwcf.com/Article/details/gxquyjjwo.sHtML

Go:   type User struct { Name string }
来源：http://mobile.yfazqb.com/Article/details/gbbwvqskp.sHtML

Ruby: class User; end
来源：http://www.share.epnwcf.com/Article/details/gszyqpzlw.sHtML

C#:   class User {}
来源：http://3g.vehdjk.com/Article/details/gfjstlkbz.sHtML

[G02] 构造函数
来源：http://www.share.yfazqb.com/Article/details/gcrlbjasn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/gqppnnttf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fktsv.cn/Article/details/gvldtacmk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fktsv.cn/Article/details/gqlngzdgm.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.sjlbkw.cn/Article/details/gsdufmzps.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/gyxgkmqqh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.bbcook.cn/Article/details/gjkyqjcps.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fktsv.cn/Article/details/ggucctwfu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.bbcook.cn/Article/details/gceoshexz.sHtML

[G03] 实例属性
来源：http://3g.epnwcf.com/Article/details/gszkvasub.sHtML

Py:   self.name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/ggrekteno.sHtML

PHP:  public string $name = "x";
来源：http://wap.vehdjk.com/Article/details/gganndweo.sHtML

JS:   this.name = "x";
来源：http://3g.sjlbkw.cn/Article/details/grmdgsoqj.sHtML

TS:   name: string = "x";
来源：http://www.share.yfazqb.com/Article/details/gcynxlkpr.sHtML

Java: private String name;
来源：http://blog.vehdjk.com/Article/details/garhevnns.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fktsv.cn/Article/details/gvfhmfzbg.sHtML

Ruby: @name = "x"
来源：http://wap.fktsv.cn/Article/details/gobsozrjn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.yfazqb.com/Article/details/goasbzifz.sHtML

[G04] 定义方法
来源：http://www.m.share.bbcook.cn/Article/details/ginsvycle.sHtML

Py:   def greet(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gzsyrgxuy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gcqgcnzar.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gaxohpzct.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gvwzslmiy.sHtML

Java: String greet() { return name; }
来源：http://www.share.bbcook.cn/Article/details/getzuohzw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gaqvvbmzm.sHtML

Ruby: def greet; @name; end
来源：http://blog.bbcook.cn/Article/details/gszzqfpws.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.vehdjk.com/Article/details/gwuvitvxc.sHtML

[G05] 继承
来源：http://m.share.vehdjk.com/Article/details/gjaulbxbr.sHtML

Py:   class Admin(User): pass
来源：http://3g.vehdjk.com/Article/details/gtowbtoew.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gqnijfvbw.sHtML

JS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/grzpjqbfc.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/glxnsqmnc.sHtML

Java: class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/govnazjqb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fktsv.cn/Article/details/gpvkqwzzp.sHtML

Ruby: class Admin < User; end
来源：http://baike.yfazqb.com/Article/details/gtacqsyav.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fktsv.cn/Article/details/guatzdfmr.sHtML

[G06] 重写方法
来源：http://www.m.share.fktsv.cn/Article/details/gvsprnsiv.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.epnwcf.com/Article/details/gqertfdoa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/glyztjagw.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/glscxfmkw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/geiltgcsk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gbxoyybrs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.epnwcf.com/Article/details/ghdlcxzyu.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.sjlbkw.cn/Article/details/gjzrzrhib.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.vehdjk.com/Article/details/gwetkgasv.sHtML

[G07] 调用父类方法
来源：http://www.m.share.epnwcf.com/Article/details/guizsqmcx.sHtML

Py:   super().greet()
来源：http://www.blog.vehdjk.com/Article/details/gezxbtpph.sHtML

PHP:  parent::greet();
来源：http://mobile.fktsv.cn/Article/details/gesfovezh.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gmywkemmm.sHtML

TS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/gzrcyecma.sHtML

Java: super.greet();
来源：http://3g.tarul.cn/Article/details/gvsiowsyq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.tarul.cn/Article/details/gclmzwvuo.sHtML

Ruby: super
来源：http://blog.sjlbkw.cn/Article/details/gmmtdzcvj.sHtML

C#:   base.Greet();
来源：http://m.share.fktsv.cn/Article/details/gpqfpebie.sHtML

[G08] 静态方法与属性
来源：http://mobile.fktsv.cn/Article/details/gbfqwcoqa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.bbcook.cn/Article/details/gdsdfxcep.sHtML

PHP:  public static function f() {}
来源：http://blog.yfazqb.com/Article/details/gdwjtuolc.sHtML

JS:   static f() {}
来源：http://read.share.bbcook.cn/Article/details/gbuuzdipg.sHtML

TS:   static f(): void {}
来源：http://blog.bbcook.cn/Article/details/gzxlrqbyl.sHtML

Java: static void f() {}
来源：http://www.share.yfazqb.com/Article/details/gcckhehll.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fktsv.cn/Article/details/gxelojjzx.sHtML

Ruby: def self.f; end
来源：http://read.share.yfazqb.com/Article/details/grxfrrlru.sHtML

C#:   public static void F() {}
来源：http://www.share.bbcook.cn/Article/details/gqweuzbhg.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fktsv.cn/Article/details/gdkkjsxix.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.epnwcf.com/Article/details/gokfqepcs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.epnwcf.com/Article/details/gohdvkyjr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.vehdjk.com/Article/details/gdrajhtke.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.sjlbkw.cn/Article/details/gkkbrzzep.sHtML

Java: interface Shape { double area(); }
来源：http://wap.yfazqb.com/Article/details/gwgoowcek.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.yfazqb.com/Article/details/gubxfpsdm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.yfazqb.com/Article/details/gbaahkjak.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fktsv.cn/Article/details/ghpqozcdd.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/glaornnis.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.bbcook.cn/Article/details/gmapemkhg.sHtML

PHP:  public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/ghaflpcto.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.yfazqb.com/Article/details/gvctllclz.sHtML

TS:   public / protected / private
来源：http://www.share.bbcook.cn/Article/details/graqgpplm.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fktsv.cn/Article/details/gjsxvrplx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.sjlbkw.cn/Article/details/gypwsqcbf.sHtML

Ruby: public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvuvasut.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.vehdjk.com/Article/details/gozdxpspd.sHtML

[G11] getter / setter
来源：http://www.blog.sjlbkw.cn/Article/details/gcpbamasp.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.yfazqb.com/Article/details/gfdjrxokq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/geaeibqnt.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gdwqccski.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.epnwcf.com/Article/details/gkwcvugpx.sHtML

Java: public String getName() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gnlxcbujr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gbzqkydxq.sHtML

Ruby: attr_accessor :name
来源：http://mobile.yfazqb.com/Article/details/gtdfbymqr.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.yfazqb.com/Article/details/ggcajzayq.sHtML

[G12] 对象转字符串
来源：http://read.share.vehdjk.com/Article/details/gsnkjmzbf.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.tarul.cn/Article/details/goeoayoyv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gseqeshrt.sHtML

JS:   toString() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/glulngxqa.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gdgoilrkr.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gxrldwewm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gnkrepyyr.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.vehdjk.com/Article/details/gkuxmfzij.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.vehdjk.com/Article/details/gurwvqhqk.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/giwqjtndw.sHtML

Py:   isinstance(u, User)
来源：http://mobile.sjlbkw.cn/Article/details/grjpnwtae.sHtML

PHP:  $u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gabzmphrv.sHtML

JS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gzfmoazog.sHtML

TS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gcfulmyco.sHtML

Java: u instanceof User
来源：http://baike.tarul.cn/Article/details/gojuesyng.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.vehdjk.com/Article/details/goajeqcby.sHtML

Ruby: u.is_a?(User)
来源：http://wap.vehdjk.com/Article/details/gbidtzntf.sHtML

C#:   u is User
来源：http://m.share.tarul.cn/Article/details/gjesomztg.sHtML

[G14] 数据类 / record
来源：http://3g.bbcook.cn/Article/details/gfmcuvavs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.sjlbkw.cn/Article/details/gjmcnjmpf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.yfazqb.com/Article/details/grqbuieho.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.epnwcf.com/Article/details/gnfradyph.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.vehdjk.com/Article/details/goisnqrgi.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.yfazqb.com/Article/details/gpvsjiiuc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.epnwcf.com/Article/details/gydaardau.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.bbcook.cn/Article/details/gkafjqmvt.sHtML


<!-- 参考信息 -->