代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://gct.zhixingplan.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ggu.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mqq.havefunace.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ofy.hnxiangtu.top

C#:   s.Replace("a", "b")
来源：http://gpf.shangyingyoupin.top

[E07] 按分隔符拆分
来源：http://lif.sjlbkw.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gjr.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mll.cheryme.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lrb.jianghu66.top

TS:   s.split(",")
来源：http://juj.ehwqpu.com

Java: s.split(",");  s.split("\\s+")
来源：http://eng.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wpb.cheryme.top

Ruby: s.split(",");  s.split
来源：http://wtx.cheryme.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://izz.cheryme.top

[E08] 数组按分隔符合并
来源：http://idc.jlsjyb.cn

Py:   ",".join(items)
来源：http://dyw.hnqzz.top

PHP:  implode(",", $items);
来源：http://eln.havefunace.top

JS:   items.join(",")
来源：http://dhz.kuanghao11.cn

TS:   items.join(",")
来源：http://fyj.jyoumei.cn

Java: String.join(",", items)
来源：http://cto.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://xln.jinghuilouyu.cn

Ruby: items.join(",")
来源：http://joc.andypj.xyz

C#:   string.Join(",", items)
来源：http://jiu.quarkkingdee.top

[E09] 去除所有空白字符
来源：http://dwl.yueranfly.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gtp.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mzq.yuxming.cn

JS:   s.replace(/\s+/g, "")
来源：http://cky.zdbjq.cn

TS:   s.replace(/\s+/g, "")
来源：http://dex.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://aln.guannengcc.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ebb.shuidangran.top

Ruby: s.gsub(/\s+/, "")
来源：http://hto.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://miq.dashuyun.cn

[E10] 左侧补零 / 定长填充
来源：http://bbf.bbcook.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ely.sxryk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://svh.dianchejie.cn

JS:   "7".padStart(3, "0")
来源：http://mff.fzhhl.top

TS:   "7".padStart(3, "0")
来源：http://xyp.iojbl.cn

Java: String.format("%03d", 7)
来源：http://jzo.sufxvd.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rxr.jinqigufen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sgj.ctjpmb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zky.zhijiandao.cn

[E11] 反转字符串
来源：http://fsr.fktsv.cn

Py:   s[::-1]
来源：http://rev.sysykeji.top

PHP:  strrev($s);
来源：http://mvq.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://uuh.hongshengwenyu.top

TS:   [...s].reverse().join("")
来源：http://nrj.jinyuanbaomall.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ecw.fktsv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ryg.ehwqpu.com

Ruby: s.reverse
来源：http://hdv.vqdsnc.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xfb.jinqigufen.top

[E12] 统计某字符出现次数
来源：http://kio.c1oappe.top

Py:   s.count("a")
来源：http://brw.ywan-chungtsiang.top

PHP:  substr_count($s, "a");
来源：http://gav.iojbl.cn

JS:   s.split("a").length - 1
来源：http://efq.cheryme.top

TS:   s.split("a").length - 1
来源：http://uon.xuetiantiany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dil.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://ajk.sxryk.cn

Ruby: s.count("a")
来源：http://spr.daria6918.cn

C#:   s.Count(c => c == 'a')
来源：http://kxa.havefunace.top

[E13] 逐字符遍历
来源：http://zov.fengsongda.top

Py:   for ch in s: print(ch)
来源：http://qlt.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zvw.quarkkingdee.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://sia.dianchejie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://onv.hesvh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ovj.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jvd.shzxlz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lxf.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://shs.vqdsnc.cn

[E14] URL 编码与 Base64
来源：http://jhm.jinyuanbaomall.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://whv.andypj.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://zil.cqqwz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ujp.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://atf.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cyv.cqqwz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ufx.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fix.shzxlz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pas.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://mqs.xuanzx.com

Py:   html.escape(s);  html.unescape(s)
来源：http://wna.aibaodan.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xhg.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vbd.cashguo.top

TS:   // 同上，务必做 XSS 过滤
来源：http://iui.yj20258.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://owk.zhijiandao.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uhs.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cov.chenlongwang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mdi.yuxming.cn

[E16] 数字千分位
来源：http://jzl.xziqi.cn

Py:   f"{1234567:,}"
来源：http://fbz.zhijiandao.cn

PHP:  number_format(1234567);
来源：http://npx.shuidangran.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ixo.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://gvm.hcnkem.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uel.ydzc1.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zqj.pycfn.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tdn.jiagoushi.top

C#:   1234567.ToString("N0")
来源：http://kqa.xingfuxueyuan.xyz

[E17] 首字母大写
来源：http://yrk.guannengcc.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mpj.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://kua.jqgufenzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wnn.vqdsnc.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nvi.jinqigfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jcr.aizwys.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gyu.jinqigfzy.top

Ruby: s.capitalize
来源：http://czq.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://thx.hywenlv.cn

[E18] 模板占位符替换
来源：http://kef.birdmap.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ice.cucudq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vtc.guowangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://irh.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jst.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lbp.ctjpmb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jek.guowangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qqc.cheryme.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jyp.cucudq.cn

[E19] 多行文本按行拆分
来源：http://cvh.aizwys.cn

Py:   s.splitlines()
来源：http://azr.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kmh.hesvh.cn

JS:   s.split(/\r?\n/)
来源：http://jhq.gaohongyu789.top

TS:   s.split(/\r?\n/)
来源：http://lea.sufxvd.cn

Java: s.lines().toList()
来源：http://woa.nanxinkj.top

Go:   strings.Split(s, "\n")
来源：http://rto.jianghu66.top

Ruby: s.lines
来源：http://han.fktsv.cn

C#:   s.Split('\n')
来源：http://lvo.316326.xyz

[E20] 判断字符串是否为空
来源：http://yhj.tianlin.xyz

Py:   if not s:
来源：http://pqu.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://muj.shangyingyoupin.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://znz.zhiwuduotai.top

TS:   if (s === "") {}
来源：http://ugu.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://vdp.chenlongwang.top

Go:   if s == "" {}
来源：http://zcz.tianlin.xyz

Ruby: if s.empty?
来源：http://sux.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://izc.zhijiandao.cn

[E21] 超长截断加省略号
来源：http://sef.c1oappe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://amx.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ici.ywan-chungtsiang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ooh.zycfv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bor.chenjidiqi.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://atn.316326.xyz

Go:   // 按 rune 判断长度后截断
来源：http://qta.zycfv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rqt.andypj.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vfv.mhx1999.top

[E22] 字节长度与字符长度
来源：http://jou.sxryk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tpp.zhaomingkeji.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nct.ydjk.org.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qra.zhoulong.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ihw.daxiang520.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://flp.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ftq.fanxiaobao.xyz

Ruby: s.bytesize;  s.length
来源：http://djz.ybcxt.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jga.shzxlz.cn

================================================================================
来源：http://fgn.kuanghao11.cn

F. 文件与目录
来源：http://bjm.fanxiaobao.xyz

================================================================================
来源：http://xpf.havefunace.top

[F01] 读取整个文件
来源：http://xrk.sysykeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jor.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://mmm.52xcode.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uog.xuanzx.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qlm.tanke756.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gvn.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://aui.sysykeji.top

Ruby: File.read("a.txt")
来源：http://stp.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://iav.sxryk.cn

[F02] 逐行读取文件
来源：http://gla.ydjk.org.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vtw.jqgufenzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vog.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://boa.jianghu66.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yrg.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ebt.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cqo.hammf.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pne.mhx1999.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cyu.shangyingyoupin.top

[F03] 写入文件（覆盖）
来源：http://svx.haohaochexian.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ylw.yongpay.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gbn.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://czj.jinqigfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rmx.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tzz.tanke756.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qeo.hammf.cn

Ruby: File.write("a.txt", "hi")
来源：http://mmx.shanyushiyangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cpb.hnqzz.top

[F04] 追加写入文件
来源：http://lwq.cdnleiting.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dsc.jqgufenzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oxp.svipenyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nex.guannengcc.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vqe.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vpw.haohaochexian.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cxf.dashuyun.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cfb.uphjek.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eib.jinyuanbaomall.cn

[F05] 判断文件或目录是否存在
来源：http://toy.yfazqb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://azm.jianghu66.top

PHP:  file_exists("a.txt");
来源：http://rku.ctjpmb.com

JS:   fs.existsSync("a.txt")
来源：http://hde.cheryme.top

TS:   fs.existsSync("a.txt")
来源：http://adb.smart0.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://qmn.daxiang520.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ldm.cheryme.top

Ruby: File.exist?("a.txt")
来源：http://mtx.andypj.xyz

C#:   File.Exists("a.txt")
来源：http://qfc.daria6918.cn

[F06] 删除文件
来源：http://yvl.hesvh.cn

Py:   os.remove("a.txt")
来源：http://lqh.quarkkingdee.top

PHP:  unlink("a.txt");
来源：http://hdu.hywenlv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pkq.bjfxy.top

TS:   fs.unlinkSync("a.txt")
来源：http://kpw.cashguo.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vtf.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://bet.xuetiantiany.cn

Ruby: File.delete("a.txt")
来源：http://hqs.yj20258888.top

C#:   File.Delete("a.txt");
来源：http://efa.zhaomingkeji.xyz

[F07] 创建目录（含多级）
来源：http://llv.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yfa.epnwcf.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dtr.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ncu.wangshuangyany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://myv.quarkkingdee.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pxt.jinqigfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://toa.nwbrower.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yso.xziqi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xxo.dianchejie.cn

[F08] 遍历目录
来源：http://yep.bjfxy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pom.tian-w.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ego.ydjk.org.cn

JS:   fs.readdirSync("dir")
来源：http://tbm.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://ots.quarkkingdee.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://prq.cdnleiting.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jty.redwolf501.top

Ruby: Dir.children("dir")
来源：http://gdl.kuanghao11.cn

C#:   Directory.GetFiles("dir")
来源：http://qsu.daria6918.cn

[F09] 获取文件大小
来源：http://raw.shangyingyoupin.top

Py:   os.path.getsize("a.txt")
来源：http://xnh.ydzc1.top

PHP:  filesize("a.txt");
来源：http://foz.daria6918.cn

JS:   fs.statSync("a.txt").size
来源：http://zrq.zdbjq.cn

TS:   fs.statSync("a.txt").size
来源：http://wop.chenlongwang.top

Java: Files.size(Path.of("a.txt"))
来源：http://jro.chenjidiqi.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mnp.hysaishi.cn

Ruby: File.size("a.txt")
来源：http://aqt.jinyuanbaomall.cn

C#:   new FileInfo("a.txt").Length
来源：http://rtl.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://iqo.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kyu.nwbrower.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bus.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://epr.ehwqpu.com

TS:   path.extname("a.txt")
来源：http://qzo.hammf.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nht.yongpay.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dyw.snrcjt.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wtn.mhx1999.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vyt.epnwcf.com

[F11] 复制与移动文件
来源：http://hkf.ywan-chungtsiang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mwj.jinqigfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cqi.jqgufenzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zpt.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://arf.fktsv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bab.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rro.9152youxi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hkr.aizwys.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rxh.yongpay.top

[F12] CSV 读写
来源：http://hex.fehbvm.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lmu.hongshengwenyu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nyk.zhixingplan.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jrb.fanxiaobao.xyz

TS:   // 同上
来源：http://dqa.shangyingyoupin.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mlq.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sbk.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xsg.hnxiangtu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nha.c1oappe.top

================================================================================
来源：http://hut.jlsjyb.cn

G. 面向对象
来源：http://geo.tarul.cn

================================================================================
来源：http://qee.yueranfly.top

[G01] 定义类
来源：http://jmz.yueranfly.top

Py:   class User: pass
来源：http://afw.bbcook.cn

PHP:  class User {}
来源：http://wel.wangshuangyany.cn

JS:   class User {}
来源：http://nsp.sxryk.cn

TS:   class User { name: string = ""; }
来源：http://asn.shzxlz.cn

Java: class User {}
来源：http://eqe.tarul.cn

Go:   type User struct { Name string }
来源：http://gat.shanyushiyangtech.top

Ruby: class User; end
来源：http://cxe.shzxlz.cn

C#:   class User {}
来源：http://ice.9152youxi.cn

[G02] 构造函数
来源：http://nxa.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://uzu.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://ycm.hywenlv.cn

JS:   constructor(name) { this.name = name; }
来源：http://dzd.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://tbe.yueranfly.top

Java: User(String name) { this.name = name; }
来源：http://prq.xziqi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hnt.fengsongda.top

Ruby: def initialize(name); @name = name; end
来源：http://xpb.zhongyouzk.top

C#:   public User(string name) { Name = name; }
来源：http://rht.tarul.cn

[G03] 实例属性
来源：http://cnh.ivvv.top

Py:   self.name = "x"
来源：http://wzp.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://mts.ctjpmb.com

JS:   this.name = "x";
来源：http://rmy.aibaodan.cn

TS:   name: string = "x";
来源：http://yff.shzxlz.cn

Java: private String name;
来源：http://qoj.dashuyun.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rkg.52xcode.cn

Ruby: @name = "x"
来源：http://oau.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://ttj.cqqwz.cn

[G04] 定义方法
来源：http://dip.nwbrower.top

Py:   def greet(self): return self.name
来源：http://czr.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bxr.aizwys.cn

JS:   greet() { return this.name; }
来源：http://jmo.havefunace.top

TS:   greet(): string { return this.name; }
来源：http://lky.xylfe.cn

Java: String greet() { return name; }
来源：http://hhb.xziqi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kgc.shuidangran.top

Ruby: def greet; @name; end
来源：http://gnu.zhengqikj.top

C#:   public string Greet() => Name;
来源：http://jrt.shuidangran.top

[G05] 继承
来源：http://jyk.zycfv.cn


<!-- 参考信息 -->