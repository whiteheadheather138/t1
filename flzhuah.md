代发 wailian999

Ruby: s.split(",");  s.split
来源：https://io.zhonguo4118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://gd.zhonguo7118.cn

[E08] 数组按分隔符合并
来源：https://fn.zhonguo7118.cn

Py:   ",".join(items)
来源：https://ep.zhonguo4118.cn

PHP:  implode(",", $items);
来源：https://ea.zhonguo5118.cn

JS:   items.join(",")
来源：https://na.zhonguo6118.cn

TS:   items.join(",")
来源：https://sw.zhonguo3118.cn

Java: String.join(",", items)
来源：https://qb.zhonguo2118.cn

Go:   strings.Join(items, ",")
来源：https://qb.zhonguo5118.cn

Ruby: items.join(",")
来源：https://ht.zhonguo6118.cn

C#:   string.Join(",", items)
来源：https://tt.zhonguo5118.cn

[E09] 去除所有空白字符
来源：https://zn.zhonguo1118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://ze.zhonguo2118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://pq.zhonguo3118.cn

JS:   s.replace(/\s+/g, "")
来源：https://ao.zhonguo8118.cn

TS:   s.replace(/\s+/g, "")
来源：https://kk.zhonguo1118.cn

Java: s.replaceAll("\\s+", "")
来源：https://ng.zhonguo3118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://kc.zhonguo5118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://xy.zhonguo8118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://hq.zhonguo1118.cn

[E10] 左侧补零 / 定长填充
来源：https://lw.zhonguo2118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://jc.zhonguo1118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://ip.zhonguo2118.cn

JS:   "7".padStart(3, "0")
来源：https://fe.zhonguo7118.cn

TS:   "7".padStart(3, "0")
来源：https://gx.zhonguo8118.cn

Java: String.format("%03d", 7)
来源：https://pr.zhonguo5118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://ix.zhonguo2118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://be.zhonguo8118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://um.zhonguo8118.cn

[E11] 反转字符串
来源：https://cm.zhonguo3118.cn

Py:   s[::-1]
来源：https://st.zhonguo4118.cn

PHP:  strrev($s);
来源：https://ah.zhonguo8118.cn

JS:   [...s].reverse().join("")
来源：https://hq.zhonguo5118.cn

TS:   [...s].reverse().join("")
来源：https://lk.zhonguo4118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://jt.zhonguo8118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://qx.zhonguo4118.cn

Ruby: s.reverse
来源：https://pu.zhonguo4118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://yc.zhonguo8118.cn

[E12] 统计某字符出现次数
来源：https://vi.zhonguo3118.cn

Py:   s.count("a")
来源：https://hm.zhonguo3118.cn

PHP:  substr_count($s, "a");
来源：https://mo.zhonguo7118.cn

JS:   s.split("a").length - 1
来源：https://up.zhonguo2118.cn

TS:   s.split("a").length - 1
来源：https://ky.zhonguo6118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://hh.zhonguo6118.cn

Go:   strings.Count(s, "a")
来源：https://kc.zhonguo7118.cn

Ruby: s.count("a")
来源：https://jg.zhonguo1118.cn

C#:   s.Count(c => c == 'a')
来源：https://kx.zhonguo4118.cn

[E13] 逐字符遍历
来源：https://va.zhonguo7118.cn

Py:   for ch in s: print(ch)
来源：https://kw.zhonguo8118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://rz.zhonguo6118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://xe.zhonguo2118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://ti.zhonguo7118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://fa.zhonguo1118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://ji.zhonguo5118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://ud.zhonguo7118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://gp.zhonguo5118.cn

[E14] URL 编码与 Base64
来源：https://ps.zhonguo2118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://yq.zhonguo7118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://qn.zhonguo1118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://gk.zhonguo2118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://ni.zhonguo3118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://er.zhonguo1118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://ul.zhonguo5118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://nk.zhonguo1118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://wt.zhonguo1118.cn

[E15] HTML 转义 / 反转义
来源：https://sy.zhonguo8118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://so.zhonguo4118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://yz.zhonguo4118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://as.zhonguo8118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://nn.zhonguo4118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://uj.zhonguo6118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://gs.zhonguo6118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://wi.zhonguo5118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://tq.zhonguo7118.cn

[E16] 数字千分位
来源：https://uh.zhonguo8118.cn

Py:   f"{1234567:,}"
来源：https://gw.zhonguo6118.cn

PHP:  number_format(1234567);
来源：https://xm.zhonguo7118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://tm.zhonguo5118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://fz.zhonguo5118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://lg.zhonguo3118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://us.zhonguo6118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://ib.zhonguo1118.cn

C#:   1234567.ToString("N0")
来源：https://ut.zhonguo8118.cn

[E17] 首字母大写
来源：https://pm.zhonguo5118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://il.zhonguo3118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://jy.zhonguo5118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://cs.zhonguo5118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://oy.zhonguo1118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://qu.zhonguo7118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://xy.zhonguo2118.cn

Ruby: s.capitalize
来源：https://jy.zhonguo8118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://wr.zhonguo3118.cn

[E18] 模板占位符替换
来源：https://bg.zhonguo4118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://ot.zhonguo3118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://qb.zhonguo2118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://fh.zhonguo7118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://gs.zhonguo7118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://fd.zhonguo7118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://jy.zhonguo4118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://tu.zhonguo7118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://hy.zhonguo5118.cn

[E19] 多行文本按行拆分
来源：https://js.zhonguo6118.cn

Py:   s.splitlines()
来源：https://un.zhonguo2118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://qb.zhonguo4118.cn

JS:   s.split(/\r?\n/)
来源：https://pw.zhonguo5118.cn

TS:   s.split(/\r?\n/)
来源：https://hy.zhonguo2118.cn

Java: s.lines().toList()
来源：https://ln.zhonguo5118.cn

Go:   strings.Split(s, "\n")
来源：https://zi.zhonguo2118.cn

Ruby: s.lines
来源：https://ix.zhonguo2118.cn

C#:   s.Split('\n')
来源：https://op.zhonguo3118.cn

[E20] 判断字符串是否为空
来源：https://ta.zhonguo4118.cn

Py:   if not s:
来源：https://en.zhonguo3118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://nv.zhonguo6118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://pl.zhonguo6118.cn

TS:   if (s === "") {}
来源：https://dq.zhonguo7118.cn

Java: if (s.isEmpty()) {}
来源：https://br.zhonguo8118.cn

Go:   if s == "" {}
来源：https://pb.zhonguo5118.cn

Ruby: if s.empty?
来源：https://io.zhonguo4118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://zk.zhonguo8118.cn

[E21] 超长截断加省略号
来源：https://rb.zhonguo1118.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：https://yq.zhonguo5118.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：https://jb.zhonguo2118.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://ec.zhonguo7118.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：https://id.zhonguo2118.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：https://ht.zhonguo6118.cn

Go:   // 按 rune 判断长度后截断
来源：https://wz.zhonguo8118.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：https://us.zhonguo3118.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：https://cl.zhonguo2118.cn

[E22] 字节长度与字符长度
来源：https://eu.zhonguo6118.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：https://um.zhonguo7118.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://eg.zhonguo2118.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：https://tk.zhonguo8118.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：https://xu.zhonguo6118.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：https://fn.zhonguo1118.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：https://dn.zhonguo6118.cn

Ruby: s.bytesize;  s.length
来源：https://ql.zhonguo6118.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：https://hs.zhonguo5118.cn

================================================================================
来源：https://oz.zhonguo7118.cn

F. 文件与目录
来源：https://gp.zhonguo2118.cn

================================================================================
来源：https://eq.zhonguo8118.cn

[F01] 读取整个文件
来源：https://sw.zhonguo8118.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：https://qk.zhonguo2118.cn

PHP:  file_get_contents("a.txt");
来源：https://pa.zhonguo8118.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：https://xp.zhonguo5118.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://js.zhonguo6118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://fz.zhonguo7118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://tw.zhonguo8118.cn

Ruby: File.read("a.txt")
来源：https://kr.zhonguo3118.cn

C#:   File.ReadAllText("a.txt");
来源：https://py.zhonguo6118.cn

[F02] 逐行读取文件
来源：https://pd.zhonguo7118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://by.zhonguo8118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://bu.zhonguo8118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://gr.zhonguo4118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://rj.zhonguo3118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://gh.zhonguo2118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://jc.zhonguo3118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://sf.zhonguo8118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://gx.zhonguo6118.cn

[F03] 写入文件（覆盖）
来源：https://gk.zhonguo6118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://ud.zhonguo7118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://ft.zhonguo5118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://vt.zhonguo1118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://oo.zhonguo5118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://dp.zhonguo2118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://rk.zhonguo3118.cn

Ruby: File.write("a.txt", "hi")
来源：https://az.zhonguo4118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://lc.zhonguo7118.cn

[F04] 追加写入文件
来源：https://dg.zhonguo8118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://mb.zhonguo6118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://qu.zhonguo2118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://by.zhonguo3118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://ym.zhonguo5118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://xx.zhonguo5118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://aq.zhonguo1118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://cl.zhonguo7118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://oo.zhonguo6118.cn

[F05] 判断文件或目录是否存在
来源：https://cj.zhonguo5118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://vo.zhonguo5118.cn

PHP:  file_exists("a.txt");
来源：https://is.zhonguo6118.cn

JS:   fs.existsSync("a.txt")
来源：https://fn.zhonguo1118.cn

TS:   fs.existsSync("a.txt")
来源：https://ob.zhonguo8118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://xv.zhonguo6118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://ok.zhonguo8118.cn

Ruby: File.exist?("a.txt")
来源：https://lf.zhonguo5118.cn

C#:   File.Exists("a.txt")
来源：https://bc.zhonguo3118.cn

[F06] 删除文件
来源：https://um.zhonguo7118.cn

Py:   os.remove("a.txt")
来源：https://zy.zhonguo7118.cn

PHP:  unlink("a.txt");
来源：https://hb.zhonguo3118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://me.zhonguo2118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://gn.zhonguo1118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://td.zhonguo4118.cn

Go:   os.Remove("a.txt")
来源：https://iv.zhonguo4118.cn

Ruby: File.delete("a.txt")
来源：https://is.zhonguo7118.cn

C#:   File.Delete("a.txt");
来源：https://gw.zhonguo5118.cn

[F07] 创建目录（含多级）
来源：https://ge.zhonguo3118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://vz.zhonguo1118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://os.zhonguo4118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://jk.zhonguo8118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://ch.zhonguo7118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://wg.zhonguo2118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://td.zhonguo2118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://vv.zhonguo3118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://by.zhonguo4118.cn

[F08] 遍历目录
来源：https://ae.zhonguo4118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://uc.zhonguo1118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://jh.zhonguo1118.cn

JS:   fs.readdirSync("dir")
来源：https://nd.zhonguo5118.cn

TS:   fs.readdirSync("dir")
来源：https://gm.zhonguo1118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://le.zhonguo3118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://iv.zhonguo6118.cn

Ruby: Dir.children("dir")
来源：https://zh.zhonguo8118.cn

C#:   Directory.GetFiles("dir")
来源：https://ec.zhonguo4118.cn

[F09] 获取文件大小
来源：https://ap.zhonguo3118.cn

Py:   os.path.getsize("a.txt")
来源：https://td.zhonguo5118.cn

PHP:  filesize("a.txt");
来源：https://bl.zhonguo1118.cn

JS:   fs.statSync("a.txt").size
来源：https://mt.zhonguo3118.cn

TS:   fs.statSync("a.txt").size
来源：https://jy.zhonguo5118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://hz.zhonguo2118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://di.zhonguo6118.cn

Ruby: File.size("a.txt")
来源：https://ft.zhonguo8118.cn

C#:   new FileInfo("a.txt").Length
来源：https://pm.zhonguo2118.cn

[F10] 取文件扩展名 / 文件名
来源：https://fc.zhonguo3118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://ce.zhonguo2118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://xb.zhonguo6118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://cg.zhonguo1118.cn

TS:   path.extname("a.txt")
来源：https://me.zhonguo1118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://hr.zhonguo4118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://vt.zhonguo6118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://iy.zhonguo1118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://mc.zhonguo2118.cn

[F11] 复制与移动文件
来源：https://ma.zhonguo1118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://dg.zhonguo7118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://ec.zhonguo8118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://ht.zhonguo3118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://bj.zhonguo3118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://hc.zhonguo4118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://qk.zhonguo7118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://wq.zhonguo4118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://ld.zhonguo1118.cn

[F12] CSV 读写
来源：https://qg.zhonguo3118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://bg.zhonguo5118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://eu.zhonguo1118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://or.zhonguo3118.cn

TS:   // 同上
来源：https://wg.zhonguo5118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://hi.zhonguo2118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://hx.zhonguo1118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://de.zhonguo2118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://wm.zhonguo3118.cn

================================================================================
来源：https://xn.zhonguo4118.cn

G. 面向对象
来源：https://dk.zhonguo3118.cn

================================================================================
来源：https://xs.zhonguo1118.cn

[G01] 定义类
来源：https://mm.zhonguo6118.cn

Py:   class User: pass
来源：https://jx.zhonguo4118.cn

PHP:  class User {}
来源：https://fd.zhonguo6118.cn

JS:   class User {}
来源：https://dm.zhonguo6118.cn

TS:   class User { name: string = ""; }
来源：https://ti.zhonguo4118.cn

Java: class User {}
来源：https://fx.zhonguo3118.cn

Go:   type User struct { Name string }
来源：https://ci.zhonguo6118.cn

Ruby: class User; end
来源：https://fy.zhonguo7118.cn

C#:   class User {}
来源：https://kq.zhonguo2118.cn

[G02] 构造函数
来源：https://bv.zhonguo4118.cn

Py:   def __init__(self, name): self.name = name
来源：https://yd.zhonguo2118.cn

PHP:  public function __construct(public string $name) {}
来源：https://xm.zhonguo4118.cn

JS:   constructor(name) { this.name = name; }
来源：https://yn.zhonguo6118.cn

TS:   constructor(public name: string) {}
来源：https://yu.zhonguo5118.cn

Java: User(String name) { this.name = name; }
来源：https://zx.zhonguo2118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://ou.zhonguo6118.cn

Ruby: def initialize(name); @name = name; end
来源：https://vi.zhonguo8118.cn

C#:   public User(string name) { Name = name; }
来源：https://nu.zhonguo1118.cn

[G03] 实例属性
来源：https://pr.zhonguo5118.cn

Py:   self.name = "x"
来源：https://uw.zhonguo8118.cn

PHP:  public string $name = "x";
来源：https://xe.zhonguo6118.cn

JS:   this.name = "x";
来源：https://xr.zhonguo5118.cn

TS:   name: string = "x";
来源：https://hm.zhonguo5118.cn

Java: private String name;
来源：https://ky.zhonguo6118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://dh.zhonguo3118.cn

Ruby: @name = "x"
来源：https://ie.zhonguo4118.cn

C#:   public string Name { get; set; } = "x";
来源：https://yl.zhonguo4118.cn

[G04] 定义方法
来源：https://xi.zhonguo1118.cn

Py:   def greet(self): return self.name
来源：https://jw.zhonguo6118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://zm.zhonguo3118.cn

JS:   greet() { return this.name; }
来源：https://yl.zhonguo7118.cn

TS:   greet(): string { return this.name; }
来源：https://uu.zhonguo4118.cn

Java: String greet() { return name; }
来源：https://vz.zhonguo4118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://uc.zhonguo2118.cn

Ruby: def greet; @name; end
来源：https://by.zhonguo1118.cn

C#:   public string Greet() => Name;
来源：https://tl.zhonguo7118.cn

[G05] 继承
来源：https://jb.zhonguo5118.cn

Py:   class Admin(User): pass
来源：https://au.zhonguo4118.cn

PHP:  class Admin extends User {}
来源：https://xv.zhonguo1118.cn

JS:   class Admin extends User {}
来源：https://cc.zhonguo6118.cn

TS:   class Admin extends User {}
来源：https://dz.zhonguo3118.cn

Java: class Admin extends User {}
来源：https://la.zhonguo3118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://vb.zhonguo6118.cn

Ruby: class Admin < User; end
来源：https://ol.zhonguo8118.cn

C#:   class Admin : User {}
来源：https://nu.zhonguo1118.cn

[G06] 重写方法
来源：https://nr.zhonguo2118.cn

Py:   def greet(self): return "admin"
来源：https://ge.zhonguo4118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://ch.zhonguo2118.cn

JS:   greet() { return "admin"; }
来源：https://mt.zhonguo1118.cn


<!-- 参考信息 -->