代发 wailian999

C#:   s.Replace("a", "b")
来源：https://be.zhonguo4118.cn

[E07] 按分隔符拆分
来源：https://kf.zhonguo5118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://tz.zhonguo3118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://rn.zhonguo6118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://dc.zhonguo7118.cn

TS:   s.split(",")
来源：https://uz.zhonguo2118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://wr.zhonguo6118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://yw.zhonguo2118.cn

Ruby: s.split(",");  s.split
来源：https://iz.zhonguo8118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://bb.zhonguo5118.cn

[E08] 数组按分隔符合并
来源：https://nn.zhonguo5118.cn

Py:   ",".join(items)
来源：https://ar.zhonguo4118.cn

PHP:  implode(",", $items);
来源：https://kb.zhonguo2118.cn

JS:   items.join(",")
来源：https://dh.zhonguo5118.cn

TS:   items.join(",")
来源：https://zs.zhonguo2118.cn

Java: String.join(",", items)
来源：https://sd.zhonguo5118.cn

Go:   strings.Join(items, ",")
来源：https://ea.zhonguo7118.cn

Ruby: items.join(",")
来源：https://fd.zhonguo8118.cn

C#:   string.Join(",", items)
来源：https://ib.zhonguo6118.cn

[E09] 去除所有空白字符
来源：https://db.zhonguo3118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://rs.zhonguo4118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://ro.zhonguo5118.cn

JS:   s.replace(/\s+/g, "")
来源：https://ag.zhonguo8118.cn

TS:   s.replace(/\s+/g, "")
来源：https://vk.zhonguo1118.cn

Java: s.replaceAll("\\s+", "")
来源：https://gb.zhonguo5118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://gz.zhonguo5118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://rh.zhonguo3118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://dt.zhonguo4118.cn

[E10] 左侧补零 / 定长填充
来源：https://lm.zhonguo3118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://qu.zhonguo8118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://rw.zhonguo5118.cn

JS:   "7".padStart(3, "0")
来源：https://fl.zhonguo4118.cn

TS:   "7".padStart(3, "0")
来源：https://ww.zhonguo6118.cn

Java: String.format("%03d", 7)
来源：https://if.zhonguo6118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://lc.zhonguo7118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://op.zhonguo8118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://hx.zhonguo1118.cn

[E11] 反转字符串
来源：https://du.zhonguo3118.cn

Py:   s[::-1]
来源：https://ku.zhonguo5118.cn

PHP:  strrev($s);
来源：https://qt.zhonguo1118.cn

JS:   [...s].reverse().join("")
来源：https://uu.zhonguo1118.cn

TS:   [...s].reverse().join("")
来源：https://bx.zhonguo3118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://sh.zhonguo3118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://yi.zhonguo7118.cn

Ruby: s.reverse
来源：https://ke.zhonguo8118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://wh.zhonguo2118.cn

[E12] 统计某字符出现次数
来源：https://fr.zhonguo8118.cn

Py:   s.count("a")
来源：https://fz.zhonguo5118.cn

PHP:  substr_count($s, "a");
来源：https://xi.zhonguo1118.cn

JS:   s.split("a").length - 1
来源：https://ss.zhonguo3118.cn

TS:   s.split("a").length - 1
来源：https://jw.zhonguo7118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://nc.zhonguo6118.cn

Go:   strings.Count(s, "a")
来源：https://ew.zhonguo8118.cn

Ruby: s.count("a")
来源：https://ox.zhonguo2118.cn

C#:   s.Count(c => c == 'a')
来源：https://ve.zhonguo5118.cn

[E13] 逐字符遍历
来源：https://xy.zhonguo3118.cn

Py:   for ch in s: print(ch)
来源：https://ov.zhonguo4118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://vf.zhonguo7118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://rr.zhonguo7118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://kb.zhonguo7118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://fh.zhonguo4118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://rt.zhonguo7118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://av.zhonguo8118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://jx.zhonguo1118.cn

[E14] URL 编码与 Base64
来源：https://ry.zhonguo5118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://ex.zhonguo5118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://tu.zhonguo6118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://pw.zhonguo5118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://zk.zhonguo8118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://ki.zhonguo2118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://lb.zhonguo7118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://hl.zhonguo2118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://wr.zhonguo6118.cn

[E15] HTML 转义 / 反转义
来源：https://rf.zhonguo7118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://ns.zhonguo7118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://cg.zhonguo1118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://yl.zhonguo1118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://jj.zhonguo8118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://fd.zhonguo2118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://cn.zhonguo5118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://vr.zhonguo6118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://ug.zhonguo7118.cn

[E16] 数字千分位
来源：https://hl.zhonguo2118.cn

Py:   f"{1234567:,}"
来源：https://qe.zhonguo7118.cn

PHP:  number_format(1234567);
来源：https://zo.zhonguo6118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://fg.zhonguo4118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://tp.zhonguo7118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://xc.zhonguo3118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://wb.zhonguo7118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://el.zhonguo1118.cn

C#:   1234567.ToString("N0")
来源：https://di.zhonguo7118.cn

[E17] 首字母大写
来源：https://rt.zhonguo6118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://bl.zhonguo5118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://ou.zhonguo8118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://qp.zhonguo8118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://mx.zhonguo2118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://vk.zhonguo3118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://ry.zhonguo7118.cn

Ruby: s.capitalize
来源：https://pa.zhonguo3118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://ak.zhonguo6118.cn

[E18] 模板占位符替换
来源：https://ha.zhonguo6118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://mn.zhonguo8118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://xk.zhonguo5118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://qx.zhonguo3118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://xq.zhonguo6118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://bi.zhonguo8118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://jb.zhonguo6118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://if.zhonguo2118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://rb.zhonguo6118.cn

[E19] 多行文本按行拆分
来源：https://jy.zhonguo5118.cn

Py:   s.splitlines()
来源：https://ih.zhonguo2118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://ja.zhonguo6118.cn

JS:   s.split(/\r?\n/)
来源：https://mq.zhonguo1118.cn

TS:   s.split(/\r?\n/)
来源：https://cz.zhonguo4118.cn

Java: s.lines().toList()
来源：https://gu.zhonguo1118.cn

Go:   strings.Split(s, "\n")
来源：https://xb.zhonguo5118.cn

Ruby: s.lines
来源：https://xc.zhonguo2118.cn

C#:   s.Split('\n')
来源：https://ma.zhonguo1118.cn

[E20] 判断字符串是否为空
来源：https://tw.zhonguo2118.cn

Py:   if not s:
来源：https://qc.zhonguo3118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://kn.zhonguo7118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://qv.zhonguo7118.cn

TS:   if (s === "") {}
来源：https://kc.zhonguo5118.cn

Java: if (s.isEmpty()) {}
来源：https://tx.zhonguo8118.cn

Go:   if s == "" {}
来源：https://xt.zhonguo5118.cn

Ruby: if s.empty?
来源：https://gz.zhonguo4118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://ef.zhonguo1118.cn

[E21] 超长截断加省略号
来源：https://gy.zhonguo4118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://ma.zhonguo5118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://mi.zhonguo4118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://sk.zhonguo4118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://dq.zhonguo8118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://pj.zhonguo2118.cn

Go:   // 按 rune 判断长度后截断
来源：https://qh.zhonguo3118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://vm.zhonguo1118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://ct.zhonguo5118.cn

[E22] 字节长度与字符长度
来源：https://pz.zhonguo6118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://eb.zhonguo2118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://sv.zhonguo7118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://jm.zhonguo7118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://zk.zhonguo8118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://if.zhonguo5118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://es.zhonguo2118.cn

Ruby: s.bytesize;  s.length
来源：https://yk.zhonguo2118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://jx.zhonguo5118.cn

================================================================================
来源：https://vp.zhonguo3118.cn

F. 文件与目录
来源：https://oh.zhonguo2118.cn

================================================================================
来源：https://wt.zhonguo5118.cn

[F01] 读取整个文件
来源：https://rk.zhonguo4118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://oz.zhonguo5118.cn

PHP:  file_get_contents("a.txt");
来源：https://fc.zhonguo3118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://pa.zhonguo3118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://fg.zhonguo2118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://hb.zhonguo7118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://xi.zhonguo1118.cn

Ruby: File.read("a.txt")
来源：https://oq.zhonguo1118.cn

C#:   File.ReadAllText("a.txt");
来源：https://fq.zhonguo8118.cn

[F02] 逐行读取文件
来源：https://gb.zhonguo2118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://ol.zhonguo5118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://ju.zhonguo4118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://mu.zhonguo5118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://br.zhonguo2118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://kq.zhonguo3118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://ox.zhonguo4118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://ul.zhonguo1118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://al.zhonguo7118.cn

[F03] 写入文件（覆盖）
来源：https://gj.zhonguo1118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://hv.zhonguo7118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://hr.zhonguo4118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://am.zhonguo3118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://ot.zhonguo5118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://fb.zhonguo5118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://px.zhonguo5118.cn

Ruby: File.write("a.txt", "hi")
来源：https://nw.zhonguo1118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://jb.zhonguo7118.cn

[F04] 追加写入文件
来源：https://px.zhonguo8118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://lt.zhonguo3118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://en.zhonguo5118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://dz.zhonguo2118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://vv.zhonguo2118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://ob.zhonguo5118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://bf.zhonguo4118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://fg.zhonguo6118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://sw.zhonguo1118.cn

[F05] 判断文件或目录是否存在
来源：https://hq.zhonguo5118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://rj.zhonguo3118.cn

PHP:  file_exists("a.txt");
来源：https://zf.zhonguo7118.cn

JS:   fs.existsSync("a.txt")
来源：https://bf.zhonguo3118.cn

TS:   fs.existsSync("a.txt")
来源：https://om.zhonguo4118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://vt.zhonguo2118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://mc.zhonguo6118.cn

Ruby: File.exist?("a.txt")
来源：https://im.zhonguo4118.cn

C#:   File.Exists("a.txt")
来源：https://pp.zhonguo1118.cn

[F06] 删除文件
来源：https://gr.zhonguo3118.cn

Py:   os.remove("a.txt")
来源：https://lu.zhonguo7118.cn

PHP:  unlink("a.txt");
来源：https://em.zhonguo1118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://be.zhonguo4118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://lt.zhonguo1118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://nz.zhonguo8118.cn

Go:   os.Remove("a.txt")
来源：https://qi.zhonguo3118.cn

Ruby: File.delete("a.txt")
来源：https://ta.zhonguo2118.cn

C#:   File.Delete("a.txt");
来源：https://xz.zhonguo4118.cn

[F07] 创建目录（含多级）
来源：https://pm.zhonguo2118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://ye.zhonguo4118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://mv.zhonguo5118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://xd.zhonguo1118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://ap.zhonguo8118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://bg.zhonguo2118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://ja.zhonguo3118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://ux.zhonguo8118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://tv.zhonguo8118.cn

[F08] 遍历目录
来源：https://hc.zhonguo8118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://gc.zhonguo2118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://cl.zhonguo6118.cn

JS:   fs.readdirSync("dir")
来源：https://ih.zhonguo6118.cn

TS:   fs.readdirSync("dir")
来源：https://uh.zhonguo8118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://ct.zhonguo7118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://sq.zhonguo2118.cn

Ruby: Dir.children("dir")
来源：https://rr.zhonguo3118.cn

C#:   Directory.GetFiles("dir")
来源：https://ny.zhonguo1118.cn

[F09] 获取文件大小
来源：https://re.zhonguo8118.cn

Py:   os.path.getsize("a.txt")
来源：https://aa.zhonguo7118.cn

PHP:  filesize("a.txt");
来源：https://lz.zhonguo2118.cn

JS:   fs.statSync("a.txt").size
来源：https://rf.zhonguo3118.cn

TS:   fs.statSync("a.txt").size
来源：https://gl.zhonguo2118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://sq.zhonguo1118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://xu.zhonguo6118.cn

Ruby: File.size("a.txt")
来源：https://hm.zhonguo2118.cn

C#:   new FileInfo("a.txt").Length
来源：https://nq.zhonguo3118.cn

[F10] 取文件扩展名 / 文件名
来源：https://da.zhonguo8118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://kv.zhonguo7118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://rx.zhonguo4118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://hx.zhonguo5118.cn

TS:   path.extname("a.txt")
来源：https://gn.zhonguo4118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://rm.zhonguo1118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://pv.zhonguo4118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://oz.zhonguo6118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://pv.zhonguo3118.cn

[F11] 复制与移动文件
来源：https://fx.zhonguo3118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://bx.zhonguo8118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://kf.zhonguo5118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://ae.zhonguo1118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://nn.zhonguo3118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://xi.zhonguo6118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://jh.zhonguo1118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://lk.zhonguo3118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://ym.zhonguo2118.cn

[F12] CSV 读写
来源：https://bg.zhonguo2118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://eb.zhonguo6118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://qu.zhonguo2118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://uy.zhonguo8118.cn

TS:   // 同上
来源：https://mh.zhonguo7118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://ln.zhonguo1118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://gs.zhonguo8118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://mm.zhonguo8118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://yu.zhonguo6118.cn

================================================================================
来源：https://hr.zhonguo1118.cn

G. 面向对象
来源：https://hw.zhonguo2118.cn

================================================================================
来源：https://sx.zhonguo5118.cn

[G01] 定义类
来源：https://gp.zhonguo7118.cn

Py:   class User: pass
来源：https://oc.zhonguo7118.cn

PHP:  class User {}
来源：https://gm.zhonguo5118.cn

JS:   class User {}
来源：https://mj.zhonguo5118.cn

TS:   class User { name: string = ""; }
来源：https://lf.zhonguo4118.cn

Java: class User {}
来源：https://uz.zhonguo5118.cn

Go:   type User struct { Name string }
来源：https://cw.zhonguo4118.cn

Ruby: class User; end
来源：https://ku.zhonguo5118.cn

C#:   class User {}
来源：https://ah.zhonguo8118.cn

[G02] 构造函数
来源：https://oi.zhonguo7118.cn

Py:   def __init__(self, name): self.name = name
来源：https://ch.zhonguo3118.cn

PHP:  public function __construct(public string $name) {}
来源：https://bf.zhonguo3118.cn

JS:   constructor(name) { this.name = name; }
来源：https://cg.zhonguo6118.cn

TS:   constructor(public name: string) {}
来源：https://al.zhonguo3118.cn

Java: User(String name) { this.name = name; }
来源：https://im.zhonguo6118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://ep.zhonguo6118.cn

Ruby: def initialize(name); @name = name; end
来源：https://wl.zhonguo7118.cn

C#:   public User(string name) { Name = name; }
来源：https://fx.zhonguo1118.cn

[G03] 实例属性
来源：https://cv.zhonguo6118.cn

Py:   self.name = "x"
来源：https://rp.zhonguo7118.cn

PHP:  public string $name = "x";
来源：https://gq.zhonguo3118.cn

JS:   this.name = "x";
来源：https://vs.zhonguo5118.cn

TS:   name: string = "x";
来源：https://yk.zhonguo3118.cn

Java: private String name;
来源：https://rh.zhonguo6118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://yl.zhonguo5118.cn

Ruby: @name = "x"
来源：https://vx.zhonguo5118.cn

C#:   public string Name { get; set; } = "x";
来源：https://lt.zhonguo3118.cn

[G04] 定义方法
来源：https://jd.zhonguo1118.cn

Py:   def greet(self): return self.name
来源：https://oh.zhonguo2118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://bc.zhonguo7118.cn

JS:   greet() { return this.name; }
来源：https://wa.zhonguo3118.cn

TS:   greet(): string { return this.name; }
来源：https://hh.zhonguo2118.cn

Java: String greet() { return name; }
来源：https://ip.zhonguo8118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://lz.zhonguo7118.cn

Ruby: def greet; @name; end
来源：https://ck.zhonguo7118.cn

C#:   public string Greet() => Name;
来源：https://sx.zhonguo1118.cn

[G05] 继承
来源：https://vi.zhonguo5118.cn

Py:   class Admin(User): pass
来源：https://wj.zhonguo7118.cn

PHP:  class Admin extends User {}
来源：https://jv.zhonguo7118.cn

JS:   class Admin extends User {}
来源：https://oz.zhonguo7118.cn

TS:   class Admin extends User {}
来源：https://gr.zhonguo1118.cn


<!-- 参考信息 -->