代发 wailian999

PHP:  strpos($s, "x");
来源：http://dlm.hesvh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iuv.sufxvd.cn

TS:   s.indexOf("x")
来源：http://can.ctjpmb.com

Java: s.indexOf("x")
来源：http://xze.tarul.cn

Go:   strings.Index(s, "x")
来源：http://sdv.dashuyun.cn

Ruby: s.index("x")
来源：http://fiz.tian-w.cn

C#:   s.IndexOf("x")
来源：http://ssg.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://onr.ydjk.org.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mbi.hfpthk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uya.yfazqb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://exv.shuidangran.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://moc.hammf.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jgt.zhijiandao.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ywh.jyoumei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://klp.fzhhl.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hbx.yfazqb.com

[E06] 替换子串
来源：http://yme.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jdh.gaohongyu789.top

PHP:  str_replace("a", "b", $s);
来源：http://mwc.fktsv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gpw.dashuyun.cn

TS:   s.replaceAll("a", "b")
来源：http://hze.ydzc1.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tlq.0kj1m.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xff.zhijiandao.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://svg.meibo888.top

C#:   s.Replace("a", "b")
来源：http://owa.hcnkem.com

[E07] 按分隔符拆分
来源：http://rip.xuetiantiany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gyd.dianchejie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lpg.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://moy.guannengcc.top

TS:   s.split(",")
来源：http://hiq.0kj1m.cn

Java: s.split(",");  s.split("\\s+")
来源：http://het.zhoulong.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mrz.shanyushiyangkeji.top

Ruby: s.split(",");  s.split
来源：http://okr.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rji.yangfankeji.com

[E08] 数组按分隔符合并
来源：http://qju.xingfuxueyuan.xyz

Py:   ",".join(items)
来源：http://pfl.ywan-chungtsiang.top

PHP:  implode(",", $items);
来源：http://cvs.quarkkingdee.top

JS:   items.join(",")
来源：http://vcy.9152youxi.cn

TS:   items.join(",")
来源：http://nfs.gaohongyu789.top

Java: String.join(",", items)
来源：http://eng.fehbvm.com

Go:   strings.Join(items, ",")
来源：http://thd.cheryme.top

Ruby: items.join(",")
来源：http://wop.yangfankeji.com

C#:   string.Join(",", items)
来源：http://jff.zdbjq.cn

[E09] 去除所有空白字符
来源：http://iyz.gzhubu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ayx.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qhi.yangfankeji.com

JS:   s.replace(/\s+/g, "")
来源：http://ppr.nanxuanxn.top

TS:   s.replace(/\s+/g, "")
来源：http://frg.guannengcc.top

Java: s.replaceAll("\\s+", "")
来源：http://mmb.sjlbkw.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://keo.jlsjyb.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qja.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://muj.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://jdz.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vgo.c1oappe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vei.jianghu66.top

JS:   "7".padStart(3, "0")
来源：http://yqv.vehdjk.com

TS:   "7".padStart(3, "0")
来源：http://kmr.yj20258.top

Java: String.format("%03d", 7)
来源：http://wfm.ybcxt.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vqs.jyoumei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vrn.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sda.hywenlv.cn

[E11] 反转字符串
来源：http://twc.tanke756.top

Py:   s[::-1]
来源：http://qhk.guowangkeji.top

PHP:  strrev($s);
来源：http://omq.vqdsnc.cn

JS:   [...s].reverse().join("")
来源：http://cdo.vehdjk.com

TS:   [...s].reverse().join("")
来源：http://nmg.cucudq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gtk.yj20258.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wvw.aizwys.cn

Ruby: s.reverse
来源：http://thm.ppjwa.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fmj.zhengqikj.top

[E12] 统计某字符出现次数
来源：http://ycl.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://dev.ppjwa.cn

PHP:  substr_count($s, "a");
来源：http://wbf.wangshuangyany.cn

JS:   s.split("a").length - 1
来源：http://kbq.birdmap.top

TS:   s.split("a").length - 1
来源：http://fjk.fengsongda.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ehx.daxiang520.top

Go:   strings.Count(s, "a")
来源：http://oyo.hongshengwenyu.top

Ruby: s.count("a")
来源：http://cld.mhx1999.top

C#:   s.Count(c => c == 'a')
来源：http://bzw.fzhhl.top

[E13] 逐字符遍历
来源：http://wsx.0kj1m.cn

Py:   for ch in s: print(ch)
来源：http://umo.hysaishi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ipm.uphjek.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://fph.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bkr.cheryme.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://twz.hysaishi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kmp.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ghu.guowangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dir.sufxvd.cn

[E14] URL 编码与 Base64
来源：http://tec.pycfn.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jui.ydjk.org.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lrj.cashguo.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://scf.xuetiantiany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://euh.yj20258.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qne.hysaishi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sju.daria6918.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mvl.316326.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ntz.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://poz.jlsjyb.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://htl.zhongyouzk.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bkn.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://avc.aibaodan.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hgm.hysaishi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ukc.ivvv.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://suh.gaohongyu789.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iwg.nanxinkj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uit.jinqigfzy.top

[E16] 数字千分位
来源：http://ect.meibo888.top

Py:   f"{1234567:,}"
来源：http://jwy.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://dku.aizwys.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mva.fehbvm.com

TS:   (1234567).toLocaleString("en-US")
来源：http://fgi.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ria.ivvv.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://elq.iojbl.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kyx.shanyushiyangtech.top

C#:   1234567.ToString("N0")
来源：http://cvf.snrcjt.cn

[E17] 首字母大写
来源：http://gso.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jvz.gogol.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bhe.bjfxy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vli.guannengcc.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tcj.hammf.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qkg.guowangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sgs.9152youxi.cn

Ruby: s.capitalize
来源：http://mpr.tianlin.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nbe.birdmap.top

[E18] 模板占位符替换
来源：http://phw.yuxming.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uhc.fengsongda.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://taz.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wzi.sufxvd.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fgv.tanke756.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nwq.hysaishi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gun.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cec.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://otf.xziqi.cn

[E19] 多行文本按行拆分
来源：http://imr.hywenlv.cn

Py:   s.splitlines()
来源：http://kyf.jiagoushi.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rcq.iojbl.cn

JS:   s.split(/\r?\n/)
来源：http://wia.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://qjl.xinyue.icu

Java: s.lines().toList()
来源：http://zua.zhiwuduotai.top

Go:   strings.Split(s, "\n")
来源：http://ymz.jqgufenzy.top

Ruby: s.lines
来源：http://mrf.guowangkeji.top

C#:   s.Split('\n')
来源：http://nip.fzhhl.top

[E20] 判断字符串是否为空
来源：http://mgj.hcnkem.com

Py:   if not s:
来源：http://qbn.cqqwz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qax.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://frb.gogol.net.cn

TS:   if (s === "") {}
来源：http://dgw.52xcode.cn

Java: if (s.isEmpty()) {}
来源：http://sro.cucudq.cn

Go:   if s == "" {}
来源：http://ncw.hysaishi.cn

Ruby: if s.empty?
来源：http://yum.jiagoushi.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://buw.hywenlv.cn

[E21] 超长截断加省略号
来源：http://bfs.xylfe.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://elz.316326.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nua.gogol.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rsz.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lqc.zhixingplan.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ihp.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://elx.shangyingyoupin.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ebz.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jsh.guowangkeji.top

[E22] 字节长度与字符长度
来源：http://eei.jqgfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kxz.316326.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xts.cashguo.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bmc.tarul.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uzk.snrcjt.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nlc.vehdjk.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mil.mhx1999.top

Ruby: s.bytesize;  s.length
来源：http://lcx.yueranfly.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bio.bbcook.cn

================================================================================
来源：http://bki.dashuyun.cn

F. 文件与目录
来源：http://cba.xinyue.icu

================================================================================
来源：http://ptl.jiagoushi.top

[F01] 读取整个文件
来源：http://jth.aizwys.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zoh.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://suc.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://olh.jqgfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oqr.nanxinkj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ckq.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iyh.sjlbkw.cn

Ruby: File.read("a.txt")
来源：http://dpd.aibaodan.cn

C#:   File.ReadAllText("a.txt");
来源：http://asn.fzhhl.top

[F02] 逐行读取文件
来源：http://gkd.jlsjyb.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://asv.cucudq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mjo.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xat.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qex.cashguo.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eud.yj202588.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qzz.daxiang520.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xxu.ctjpmb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gjl.nanxinkj.top

[F03] 写入文件（覆盖）
来源：http://zfb.vehdjk.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ljp.zhoulong.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://hzw.zhaomingkeji.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nzn.jqgfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jwk.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hpo.pycfn.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kfi.yonumen.top

Ruby: File.write("a.txt", "hi")
来源：http://lnz.gogol.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ipp.zdqjudy.top

[F04] 追加写入文件
来源：http://zju.ydzc1.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://enu.jinqigufen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zrv.aibaodan.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pei.shuidangran.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ajs.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mdk.cashguo.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fbe.tianlin.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yca.zhaomingkeji.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nsg.xziqi.cn

[F05] 判断文件或目录是否存在
来源：http://jyv.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kdv.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://vye.sufxvd.cn

JS:   fs.existsSync("a.txt")
来源：http://rhl.sjlbkw.cn

TS:   fs.existsSync("a.txt")
来源：http://avi.yj20258.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wns.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eln.yfazqb.com

Ruby: File.exist?("a.txt")
来源：http://gap.nanxuanxn.top

C#:   File.Exists("a.txt")
来源：http://ujr.ppjwa.cn

[F06] 删除文件
来源：http://inz.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://pbz.sweek.top

PHP:  unlink("a.txt");
来源：http://jks.jinqigfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://xie.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://dys.yangfankeji.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gwa.ivvv.top

Go:   os.Remove("a.txt")
来源：http://ryf.quarkkingdee.top

Ruby: File.delete("a.txt")
来源：http://wrx.zdqjudy.top

C#:   File.Delete("a.txt");
来源：http://nln.c1oappe.top

[F07] 创建目录（含多级）
来源：http://mnm.fktsv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wph.zhijiandao.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nul.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zjb.yfazqb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ivk.hcnkem.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ppe.yueranfly.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ehx.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rho.bbcook.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bbn.pengpengdd.cyou

[F08] 遍历目录
来源：http://uhw.nanxuanxn.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://syn.shzxlz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jle.zhengqikj.top

JS:   fs.readdirSync("dir")
来源：http://prx.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://ucu.jinqigufen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://acz.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fzf.tanke756.top

Ruby: Dir.children("dir")
来源：http://jaw.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://njx.pengpengdd.cyou

[F09] 获取文件大小
来源：http://ehn.bjfxy.top

Py:   os.path.getsize("a.txt")
来源：http://jrg.yj20258.top

PHP:  filesize("a.txt");
来源：http://lxx.jinqigufen.top

JS:   fs.statSync("a.txt").size
来源：http://mla.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://gwl.gotoacloud.top

Java: Files.size(Path.of("a.txt"))
来源：http://ifl.0kj1m.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://elp.ydzc1.top

Ruby: File.size("a.txt")
来源：http://pcw.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://kan.meibo888.top

[F10] 取文件扩展名 / 文件名
来源：http://ypd.bbcook.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vez.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hbv.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ozv.tianlin.xyz

TS:   path.extname("a.txt")
来源：http://ngd.0kj1m.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ayr.cheryme.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ypy.jyoumei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nrt.yvedp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://izu.xziqi.cn

[F11] 复制与移动文件
来源：http://xop.smart0.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://drf.yfazqb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vbp.zhengqikj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eau.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yoc.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jta.daria6918.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gjc.zhoulong.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://saw.iojbl.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mks.316326.xyz

[F12] CSV 读写
来源：http://wub.zhoulong.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hfr.jyoumei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cac.ehwqpu.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vhd.cqqwz.cn

TS:   // 同上
来源：http://vhi.jinghuilouyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zfw.sysykeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xjy.guowangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lax.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wdj.fehbvm.com

================================================================================
来源：http://mjg.bbcook.cn

G. 面向对象
来源：http://tnm.hnqzz.top

================================================================================
来源：http://vhn.fengsongda.top

[G01] 定义类
来源：http://crr.yanxiufei.cn

Py:   class User: pass
来源：http://gtj.hfpthk.cn

PHP:  class User {}
来源：http://hbm.yvedp.cn

JS:   class User {}
来源：http://upy.fzhhl.top

TS:   class User { name: string = ""; }
来源：http://sli.cashguo.top

Java: class User {}
来源：http://wfg.316326.xyz

Go:   type User struct { Name string }
来源：http://jld.chenlongwang.top

Ruby: class User; end
来源：http://pdd.yuxming.cn

C#:   class User {}
来源：http://uop.zhijiandao.cn

[G02] 构造函数
来源：http://mjo.iojbl.cn

Py:   def __init__(self, name): self.name = name
来源：http://pgf.ehwqpu.com

PHP:  public function __construct(public string $name) {}
来源：http://lxc.havefunace.top

JS:   constructor(name) { this.name = name; }
来源：http://aef.guowangkeji.top

TS:   constructor(public name: string) {}
来源：http://ftm.sxryk.cn

Java: User(String name) { this.name = name; }
来源：http://ceq.tanke756.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://okf.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://kkh.meibo888.top


<!-- 参考信息 -->