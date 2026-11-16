代发 wailian999

Ruby: s.split(",");  s.split
来源：http://ujk.9152youxi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bjo.hysaishi.cn

[E08] 数组按分隔符合并
来源：http://obl.xylfe.cn

Py:   ",".join(items)
来源：http://xci.fehbvm.com

PHP:  implode(",", $items);
来源：http://eri.316326.xyz

JS:   items.join(",")
来源：http://ejs.zhijiandao.cn

TS:   items.join(",")
来源：http://tgn.xingfuxueyuan.xyz

Java: String.join(",", items)
来源：http://hhi.mhx1999.top

Go:   strings.Join(items, ",")
来源：http://zst.jlsjyb.cn

Ruby: items.join(",")
来源：http://dnc.ivvv.top

C#:   string.Join(",", items)
来源：http://jcc.ppjwa.cn

[E09] 去除所有空白字符
来源：http://coy.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://plw.wangshuangyany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hpo.zhixingplan.top

JS:   s.replace(/\s+/g, "")
来源：http://eot.xziqi.cn

TS:   s.replace(/\s+/g, "")
来源：http://utk.iojbl.cn

Java: s.replaceAll("\\s+", "")
来源：http://mxx.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fdv.cheryme.top

Ruby: s.gsub(/\s+/, "")
来源：http://lhb.c1oappe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uef.sjlbkw.cn

[E10] 左侧补零 / 定长填充
来源：http://rcu.zhengqikj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bnq.jinghuilouyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ueh.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://zmd.cqqwz.cn

TS:   "7".padStart(3, "0")
来源：http://jor.sweek.top

Java: String.format("%03d", 7)
来源：http://hqw.bjfxy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://twu.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rsz.316326.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://slm.dashuyun.cn

[E11] 反转字符串
来源：http://fhl.hongshengwenyu.top

Py:   s[::-1]
来源：http://jxd.yfazqb.com

PHP:  strrev($s);
来源：http://zyt.fzhhl.top

JS:   [...s].reverse().join("")
来源：http://rum.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://lhq.chenjidiqi.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://gzn.uphjek.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://xav.shanyushiyangtech.top

Ruby: s.reverse
来源：http://ptj.yvedp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jju.yueranfly.top

[E12] 统计某字符出现次数
来源：http://xvz.jyoumei.cn

Py:   s.count("a")
来源：http://hvx.sjlbkw.cn

PHP:  substr_count($s, "a");
来源：http://sxg.shanyushiyangtech.top

JS:   s.split("a").length - 1
来源：http://akx.sysykeji.top

TS:   s.split("a").length - 1
来源：http://kjv.yvedp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mjj.aibaodan.cn

Go:   strings.Count(s, "a")
来源：http://omh.pengpengdd.cyou

Ruby: s.count("a")
来源：http://rwv.jqgfzy.top

C#:   s.Count(c => c == 'a')
来源：http://rrr.chenzaomai.com

[E13] 逐字符遍历
来源：http://xvz.ydjk.org.cn

Py:   for ch in s: print(ch)
来源：http://vbj.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ual.xziqi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bqr.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ftp.feifeiyinyue.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dyt.tanke756.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cde.hnqzz.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pjz.yj20258.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://elb.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://hpx.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fuq.zhaomingkeji.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ygs.hnqzz.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jhh.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ndm.zhoulong.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ebh.ydjk.org.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tsk.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ygu.xylfe.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://awv.vqdsnc.cn

[E15] HTML 转义 / 反转义
来源：http://pfp.yj20258.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tlm.xziqi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mrh.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mof.bbcook.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vsn.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kyj.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rqx.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ckf.zhoulong.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zzi.pengpengdd.cyou

[E16] 数字千分位
来源：http://hts.sweek.top

Py:   f"{1234567:,}"
来源：http://oqv.cheryme.top

PHP:  number_format(1234567);
来源：http://wze.9152youxi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cao.0kj1m.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rkp.gzhubu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://myh.hongshengwenyu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rjm.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://avz.tarul.cn

C#:   1234567.ToString("N0")
来源：http://xsv.c1oappe.top

[E17] 首字母大写
来源：http://ixj.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fbe.ppjwa.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fzt.ybcxt.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pyh.fengsongda.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pvb.xingfuxueyuan.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uoq.yueranfly.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://olp.ydjk.org.cn

Ruby: s.capitalize
来源：http://cfx.zhoulong.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mir.zdqjudy.top

[E18] 模板占位符替换
来源：http://xhw.52xcode.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tcc.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://txk.pengpengdd.cyou

JS:   tpl.replaceAll("{name}", name)
来源：http://pzm.birdmap.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cnc.dianchejie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qje.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://smp.hywenlv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lbe.xinyue.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ruj.smart0.xyz

[E19] 多行文本按行拆分
来源：http://xjb.pengpengdd.cyou

Py:   s.splitlines()
来源：http://ntn.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gpx.cdnleiting.top

JS:   s.split(/\r?\n/)
来源：http://ncz.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://kug.hnqzz.top

Java: s.lines().toList()
来源：http://yas.smart0.xyz

Go:   strings.Split(s, "\n")
来源：http://mrf.meibo888.top

Ruby: s.lines
来源：http://xto.nanxuanxn.top

C#:   s.Split('\n')
来源：http://bhl.9152youxi.cn

[E20] 判断字符串是否为空
来源：http://drw.jinyuanbaomall.cn

Py:   if not s:
来源：http://uof.jinqigufen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eyy.iojbl.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zmj.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://kve.andypj.xyz

Java: if (s.isEmpty()) {}
来源：http://erx.jianghu66.top

Go:   if s == "" {}
来源：http://ntd.cqqwz.cn

Ruby: if s.empty?
来源：http://qeq.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://giq.chenzaomai.com

[E21] 超长截断加省略号
来源：http://ljr.sufxvd.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yre.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://luh.shzxlz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fjm.dianchejie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://msj.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iav.dashuyun.cn

Go:   // 按 rune 判断长度后截断
来源：http://pqa.zhijiandao.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mwl.uphjek.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://duz.zhaomingkeji.xyz

[E22] 字节长度与字符长度
来源：http://uyt.yonumen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wns.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tpf.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wmw.nwbrower.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iqy.smart0.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dlp.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qsi.fengsongda.top

Ruby: s.bytesize;  s.length
来源：http://qhy.sjlbkw.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fru.yuxming.cn

================================================================================
来源：http://wia.zdqjudy.top

F. 文件与目录
来源：http://juy.jinqigfzy.top

================================================================================
来源：http://nhy.ppjwa.cn

[F01] 读取整个文件
来源：http://svs.feifeiyinyue.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yhe.jqgufenzy.top

PHP:  file_get_contents("a.txt");
来源：http://fou.uphjek.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pds.chenzaomai.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fbe.jyoumei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lfu.epnwcf.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ktx.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://zah.ybcxt.top

C#:   File.ReadAllText("a.txt");
来源：http://ivy.jiagoushi.top

[F02] 逐行读取文件
来源：http://pnp.fengsongda.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nec.redwolf501.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qrg.gogol.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ktc.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gac.snrcjt.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kfr.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dqy.gzhubu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zwk.yj20258888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lcp.yvedp.cn

[F03] 写入文件（覆盖）
来源：http://xso.xingfuxueyuan.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rxn.smart0.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://yvs.ivvv.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cyc.sysykeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nxw.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ydq.gogol.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://juq.gaohongyu789.top

Ruby: File.write("a.txt", "hi")
来源：http://txm.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ish.zdqjudy.top

[F04] 追加写入文件
来源：http://sdd.tanke756.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qjy.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ohs.vehdjk.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rys.zycfv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xza.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gzv.chenjidiqi.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://umv.gaohongyu789.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mtj.tanke756.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://csl.xuetiantiany.cn

[F05] 判断文件或目录是否存在
来源：http://azh.tian-w.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ydq.zhengqikj.top

PHP:  file_exists("a.txt");
来源：http://dwx.cheryme.top

JS:   fs.existsSync("a.txt")
来源：http://lzy.ydjk.org.cn

TS:   fs.existsSync("a.txt")
来源：http://qkw.ydzc1.top

Java: Files.exists(Path.of("a.txt"))
来源：http://syf.jqgufenzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zor.jinqigufen.top

Ruby: File.exist?("a.txt")
来源：http://hqu.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://hrm.ywan-chungtsiang.top

[F06] 删除文件
来源：http://eks.mhx1999.top

Py:   os.remove("a.txt")
来源：http://iqv.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://aja.dianchejie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dpn.hongshengwenyu.top

TS:   fs.unlinkSync("a.txt")
来源：http://qed.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jli.yueranfly.top

Go:   os.Remove("a.txt")
来源：http://dgf.yangfankeji.com

Ruby: File.delete("a.txt")
来源：http://dpq.gaohongyu789.top

C#:   File.Delete("a.txt");
来源：http://sai.daxiang520.top

[F07] 创建目录（含多级）
来源：http://jlt.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gjv.bjfxy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rnd.chenzaomai.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lsx.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rir.hnxiangtu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hhg.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yaj.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://doq.bbcook.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vhy.ybcxt.top

[F08] 遍历目录
来源：http://oxf.hywenlv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xdb.9152youxi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cyz.dianchejie.cn

JS:   fs.readdirSync("dir")
来源：http://ypi.yuxming.cn

TS:   fs.readdirSync("dir")
来源：http://tmv.sysykeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nim.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zwu.ydjk.org.cn

Ruby: Dir.children("dir")
来源：http://vbw.feifeiyinyue.top

C#:   Directory.GetFiles("dir")
来源：http://vlc.cheryme.top

[F09] 获取文件大小
来源：http://bbf.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://oan.xziqi.cn

PHP:  filesize("a.txt");
来源：http://ogh.ctjpmb.com

JS:   fs.statSync("a.txt").size
来源：http://ezb.tianlin.xyz

TS:   fs.statSync("a.txt").size
来源：http://fat.guowangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://rjb.yonumen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ssk.andypj.xyz

Ruby: File.size("a.txt")
来源：http://edw.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://zxr.havefunace.top

[F10] 取文件扩展名 / 文件名
来源：http://kcw.cucudq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jpo.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ynk.nanxuanxn.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nhb.shanyushiyangtech.top

TS:   path.extname("a.txt")
来源：http://wjw.hesvh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sgf.bjfxy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ngs.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kyd.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mlt.ehwqpu.com

[F11] 复制与移动文件
来源：http://kop.xuetiantiany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pya.daxiang520.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qgm.daria6918.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xhe.feifeiyinyue.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://osu.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nzw.aibaodan.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xlo.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pru.sysykeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jvf.yanxiufei.cn

[F12] CSV 读写
来源：http://dtg.yuxming.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oul.jinqigufen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wfc.hywenlv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ujm.quarkkingdee.top

TS:   // 同上
来源：http://jmy.jlsjyb.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ubn.sysykeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hml.zhijiandao.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zgf.jqgfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fhg.vqdsnc.cn

================================================================================
来源：http://kcv.zdqjudy.top

G. 面向对象
来源：http://ato.andypj.xyz

================================================================================
来源：http://xhf.hnqzz.top

[G01] 定义类
来源：http://ulh.ctjpmb.com

Py:   class User: pass
来源：http://xyy.fanxiaobao.xyz

PHP:  class User {}
来源：http://yhi.sjlbkw.cn

JS:   class User {}
来源：http://tjb.ybcxt.top

TS:   class User { name: string = ""; }
来源：http://dot.pycfn.com

Java: class User {}
来源：http://oeg.wangdashe.top

Go:   type User struct { Name string }
来源：http://idu.shanyushiyangkeji.top

Ruby: class User; end
来源：http://ufz.fanxiaobao.xyz

C#:   class User {}
来源：http://rqa.nanxuanxn.top

[G02] 构造函数
来源：http://pgu.yj20258888.top

Py:   def __init__(self, name): self.name = name
来源：http://lrb.zhengqikj.top

PHP:  public function __construct(public string $name) {}
来源：http://brv.yonumen.top

JS:   constructor(name) { this.name = name; }
来源：http://gjl.redwolf501.top

TS:   constructor(public name: string) {}
来源：http://ivw.sxryk.cn

Java: User(String name) { this.name = name; }
来源：http://dou.mhx1999.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pic.andypj.xyz

Ruby: def initialize(name); @name = name; end
来源：http://pre.fzhhl.top

C#:   public User(string name) { Name = name; }
来源：http://wlz.ehwqpu.com

[G03] 实例属性
来源：http://tsf.fehbvm.com

Py:   self.name = "x"
来源：http://yks.hongshengwenyu.top

PHP:  public string $name = "x";
来源：http://dgu.jqgufenzy.top

JS:   this.name = "x";
来源：http://xxy.xinyue.icu

TS:   name: string = "x";
来源：http://otm.pengpengdd.cyou

Java: private String name;
来源：http://gzd.tian-w.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mjq.jinqigfzy.top

Ruby: @name = "x"
来源：http://zeu.jqgfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://nvj.52xcode.cn

[G04] 定义方法
来源：http://vrf.52xcode.cn

Py:   def greet(self): return self.name
来源：http://zph.fengsongda.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rvc.chenjidiqi.icu

JS:   greet() { return this.name; }
来源：http://vpl.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://xbo.yj20258888.top

Java: String greet() { return name; }
来源：http://qds.yvedp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ppe.pengpengdd.cyou

Ruby: def greet; @name; end
来源：http://dod.tianlin.xyz

C#:   public string Greet() => Name;
来源：http://yxs.sxryk.cn

[G05] 继承
来源：http://xqy.haohaochexian.top

Py:   class Admin(User): pass
来源：http://klg.tarul.cn

PHP:  class Admin extends User {}
来源：http://syr.guowangkeji.top

JS:   class Admin extends User {}
来源：http://mtl.daria6918.cn

TS:   class Admin extends User {}
来源：http://znf.shzxlz.cn

Java: class Admin extends User {}
来源：http://cie.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rqg.zhengqikj.top

Ruby: class Admin < User; end
来源：http://hrw.daria6918.cn

C#:   class Admin : User {}
来源：http://tjo.smart0.xyz

[G06] 重写方法
来源：http://nky.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://nge.cheryme.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ymh.hongshengwenyu.top

JS:   greet() { return "admin"; }
来源：http://vri.nanxuanxn.top


<!-- 参考信息 -->