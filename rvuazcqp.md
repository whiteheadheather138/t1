代发 wailian999

Ruby: s.split(",");  s.split
来源：http://yvt.haohaochexian.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nxn.nanxinkj.top

[E08] 数组按分隔符合并
来源：http://nyv.xuanzx.com

Py:   ",".join(items)
来源：http://mzt.bbcook.cn

PHP:  implode(",", $items);
来源：http://fqm.zhongyouzk.top

JS:   items.join(",")
来源：http://sqs.zhongyouzk.top

TS:   items.join(",")
来源：http://bzf.xingfuxueyuan.xyz

Java: String.join(",", items)
来源：http://mnu.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://utr.meibo888.top

Ruby: items.join(",")
来源：http://mmh.xuanzx.com

C#:   string.Join(",", items)
来源：http://uxp.guowangkeji.top

[E09] 去除所有空白字符
来源：http://srg.aibaodan.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hqf.hammf.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bjp.fktsv.cn

JS:   s.replace(/\s+/g, "")
来源：http://jst.shanyushiyangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://jay.bbcook.cn

Java: s.replaceAll("\\s+", "")
来源：http://bsy.xuanzx.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://qtk.daxiang520.top

Ruby: s.gsub(/\s+/, "")
来源：http://mgx.aizwys.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nma.sxryk.cn

[E10] 左侧补零 / 定长填充
来源：http://obe.dashuyun.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://byl.guannengcc.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lrt.kuanghao11.cn

JS:   "7".padStart(3, "0")
来源：http://jvz.hcnkem.com

TS:   "7".padStart(3, "0")
来源：http://saw.yuxming.cn

Java: String.format("%03d", 7)
来源：http://gsb.ydjk.org.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://izx.yuanzhike.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ysu.hesvh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uhc.fehbvm.com

[E11] 反转字符串
来源：http://xkc.birdmap.top

Py:   s[::-1]
来源：http://ews.cucudq.cn

PHP:  strrev($s);
来源：http://eag.yuxming.cn

JS:   [...s].reverse().join("")
来源：http://qol.shzxlz.cn

TS:   [...s].reverse().join("")
来源：http://hhb.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kti.cdnleiting.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://uyw.jyoumei.cn

Ruby: s.reverse
来源：http://tkn.shangyingyoupin.top

C#:   new string(s.Reverse().ToArray())
来源：http://nih.havefunace.top

[E12] 统计某字符出现次数
来源：http://naa.haohaochexian.top

Py:   s.count("a")
来源：http://lcs.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://vlb.ywan-chungtsiang.top

JS:   s.split("a").length - 1
来源：http://amf.ydzc1.top

TS:   s.split("a").length - 1
来源：http://pts.hesvh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hei.zhaomingkeji.xyz

Go:   strings.Count(s, "a")
来源：http://bww.fktsv.cn

Ruby: s.count("a")
来源：http://pfs.sweek.top

C#:   s.Count(c => c == 'a')
来源：http://imh.xylfe.cn

[E13] 逐字符遍历
来源：http://nrw.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://nib.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qjl.xuetiantiany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tjm.quarkkingdee.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wcy.shangyingyoupin.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://drn.mhx1999.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bcr.xinyue.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://vyt.yvedp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qhv.c1oappe.top

[E14] URL 编码与 Base64
来源：http://rbo.pycfn.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gue.sweek.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mxq.fzhhl.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vrd.fengsongda.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wmb.cucudq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zqw.jqgfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rej.shzxlz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ind.aibaodan.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bxh.nanxuanxn.top

[E15] HTML 转义 / 反转义
来源：http://bua.kuanghao11.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pop.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://soa.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sdr.jinqigfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://law.shanyushiyangtech.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rxi.jinqigfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rkd.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qio.tarul.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vdj.nwbrower.top

[E16] 数字千分位
来源：http://dzp.xuetiantiany.cn

Py:   f"{1234567:,}"
来源：http://aca.ydzc1.top

PHP:  number_format(1234567);
来源：http://wdh.nanxinkj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xbx.cheryme.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wxw.vqdsnc.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://unt.cqqwz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pgg.cqqwz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ywv.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://ile.jqgfzy.top

[E17] 首字母大写
来源：http://uhm.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fxv.nanxuanxn.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dgn.aizwys.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lfd.daxiang520.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xjq.chenzaomai.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sqv.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cgf.jinghuilouyu.cn

Ruby: s.capitalize
来源：http://ijn.cheryme.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zpw.c1oappe.top

[E18] 模板占位符替换
来源：http://orw.52xcode.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nqh.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uxi.iojbl.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ihg.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fup.birdmap.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zbv.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hbw.yonumen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ygn.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zzg.sweek.top

[E19] 多行文本按行拆分
来源：http://avr.andypj.xyz

Py:   s.splitlines()
来源：http://wtu.epnwcf.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jqc.zdqjudy.top

JS:   s.split(/\r?\n/)
来源：http://zhc.zhixingplan.top

TS:   s.split(/\r?\n/)
来源：http://htr.jlsjyb.cn

Java: s.lines().toList()
来源：http://xdm.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://eoq.hesvh.cn

Ruby: s.lines
来源：http://pwv.shuidangran.top

C#:   s.Split('\n')
来源：http://koj.yangfankeji.com

[E20] 判断字符串是否为空
来源：http://dyo.pengpengdd.cyou

Py:   if not s:
来源：http://hxp.0kj1m.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xmy.ydjk.org.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zxr.quarkkingdee.top

TS:   if (s === "") {}
来源：http://iuq.fktsv.cn

Java: if (s.isEmpty()) {}
来源：http://oiw.iojbl.cn

Go:   if s == "" {}
来源：http://fgj.gogol.net.cn

Ruby: if s.empty?
来源：http://xwa.gotoacloud.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lvv.havefunace.top

[E21] 超长截断加省略号
来源：http://jtp.hongshengwenyu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://waw.tian-w.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vog.fehbvm.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yrp.dianchejie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ton.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oom.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://bez.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hsd.zhiwuduotai.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ugu.tian-w.cn

[E22] 字节长度与字符长度
来源：http://znc.cqqwz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ddq.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pkd.daxiang520.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sby.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pfb.yuanzhike.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ejw.shangyingyoupin.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blu.ydzc1.top

Ruby: s.bytesize;  s.length
来源：http://emw.fanxiaobao.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jal.guannengcc.top

================================================================================
来源：http://ouv.yj20258888.top

F. 文件与目录
来源：http://wzw.dashuyun.cn

================================================================================
来源：http://pvs.snrcjt.cn

[F01] 读取整个文件
来源：http://dgb.jqgufenzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wwb.quarkkingdee.top

PHP:  file_get_contents("a.txt");
来源：http://tzt.zdqjudy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://spt.zdqjudy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://foy.guowangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://svn.yanxiufei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hcy.yangfankeji.com

Ruby: File.read("a.txt")
来源：http://gwg.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://hsd.shanyushiyangkeji.top

[F02] 逐行读取文件
来源：http://fuj.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mpa.uphjek.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://diy.ybcxt.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lbs.jinyuanbaomall.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://llh.316326.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hzf.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rdt.tanke756.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wot.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mqh.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://gdu.fengsongda.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pii.tarul.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dfa.jqgufenzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ens.xingfuxueyuan.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://raj.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lwt.nanxuanxn.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jmx.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://vfj.vehdjk.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hxe.wangdashe.top

[F04] 追加写入文件
来源：http://tju.zdqjudy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iqw.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xec.haohaochexian.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cbd.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wjb.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jfq.zhengqikj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://txe.sjlbkw.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zqr.ydjk.org.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qwx.hfpthk.cn

[F05] 判断文件或目录是否存在
来源：http://ivn.ydjk.org.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://twh.daria6918.cn

PHP:  file_exists("a.txt");
来源：http://wfv.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://wlv.haohaochexian.top

TS:   fs.existsSync("a.txt")
来源：http://fel.smart0.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://vao.hongshengwenyu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bcy.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://pnf.ctjpmb.com

C#:   File.Exists("a.txt")
来源：http://glj.hnqzz.top

[F06] 删除文件
来源：http://vxd.bjfxy.top

Py:   os.remove("a.txt")
来源：http://yhl.tarul.cn

PHP:  unlink("a.txt");
来源：http://rpo.zhengqikj.top

JS:   fs.unlinkSync("a.txt")
来源：http://ekf.guowangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://std.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://abe.jinyuanbaomall.cn

Go:   os.Remove("a.txt")
来源：http://sli.zhengqikj.top

Ruby: File.delete("a.txt")
来源：http://hqz.ydjk.org.cn

C#:   File.Delete("a.txt");
来源：http://hyn.birdmap.top

[F07] 创建目录（含多级）
来源：http://oog.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mub.nwbrower.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iyw.gaohongyu789.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cdp.pengpengdd.cyou

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ehb.hnqzz.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://axc.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://agy.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jxx.fehbvm.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rca.hysaishi.cn

[F08] 遍历目录
来源：http://kzf.zhongyouzk.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://grq.gaohongyu789.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hbz.zhoulong.xyz

JS:   fs.readdirSync("dir")
来源：http://xpq.cashguo.top

TS:   fs.readdirSync("dir")
来源：http://ibc.ehwqpu.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qrd.hfpthk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://was.316326.xyz

Ruby: Dir.children("dir")
来源：http://mql.tianlin.xyz

C#:   Directory.GetFiles("dir")
来源：http://rsz.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://xfv.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://gyt.xingfuxueyuan.xyz

PHP:  filesize("a.txt");
来源：http://rkw.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://omy.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://rzr.ybcxt.top

Java: Files.size(Path.of("a.txt"))
来源：http://sna.xinyue.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://amr.redwolf501.top

Ruby: File.size("a.txt")
来源：http://fdb.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://rwm.jlsjyb.cn

[F10] 取文件扩展名 / 文件名
来源：http://hbr.guowangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hvd.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uvq.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bnq.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://cfi.vqdsnc.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vdf.shangyingyoupin.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nat.chenzaomai.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pfj.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xfj.hongshengwenyu.top

[F11] 复制与移动文件
来源：http://enx.hnqzz.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cwb.jianghu66.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wup.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jho.fehbvm.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jma.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qao.hywenlv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ydv.tarul.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xiv.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://stx.sufxvd.cn

[F12] CSV 读写
来源：http://cga.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ekz.zhijiandao.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dza.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kjo.guowangkeji.top

TS:   // 同上
来源：http://lug.quarkkingdee.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yym.wangdashe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ksb.sxryk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://glc.uphjek.com

C#:   // 无内置：用 CsvHelper 库
来源：http://exw.pycfn.com

================================================================================
来源：http://jgv.zhiwuduotai.top

G. 面向对象
来源：http://ybq.xziqi.cn

================================================================================
来源：http://ocg.yueranfly.top

[G01] 定义类
来源：http://ppa.dianchejie.cn

Py:   class User: pass
来源：http://rlp.ivvv.top

PHP:  class User {}
来源：http://mkb.ywan-chungtsiang.top

JS:   class User {}
来源：http://wbg.chenjidiqi.icu

TS:   class User { name: string = ""; }
来源：http://gen.shangyingyoupin.top

Java: class User {}
来源：http://hqs.iojbl.cn

Go:   type User struct { Name string }
来源：http://esg.zhixingplan.top

Ruby: class User; end
来源：http://ddr.aibaodan.cn

C#:   class User {}
来源：http://qtq.smart0.xyz

[G02] 构造函数
来源：http://zie.yonumen.top

Py:   def __init__(self, name): self.name = name
来源：http://wni.ctjpmb.com

PHP:  public function __construct(public string $name) {}
来源：http://vgp.zdbjq.cn

JS:   constructor(name) { this.name = name; }
来源：http://mef.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://vxi.zhongyouzk.top

Java: User(String name) { this.name = name; }
来源：http://amt.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://znl.316326.xyz

Ruby: def initialize(name); @name = name; end
来源：http://vmb.yueranfly.top

C#:   public User(string name) { Name = name; }
来源：http://lay.ydzc1.top

[G03] 实例属性
来源：http://xqz.dashuyun.cn

Py:   self.name = "x"
来源：http://nrg.ivvv.top

PHP:  public string $name = "x";
来源：http://pqd.shuidangran.top

JS:   this.name = "x";
来源：http://nmc.feifeiyinyue.top

TS:   name: string = "x";
来源：http://byc.zhijiandao.cn

Java: private String name;
来源：http://xfb.havefunace.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kcb.yonumen.top

Ruby: @name = "x"
来源：http://gen.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://oke.shzxlz.cn

[G04] 定义方法
来源：http://gva.jlsjyb.cn

Py:   def greet(self): return self.name
来源：http://ukb.hnxiangtu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://irf.gogol.net.cn

JS:   greet() { return this.name; }
来源：http://eeu.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://xmi.sweek.top

Java: String greet() { return name; }
来源：http://tvz.feifeiyinyue.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mjf.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://qwd.birdmap.top

C#:   public string Greet() => Name;
来源：http://idk.jlsjyb.cn

[G05] 继承
来源：http://xns.jqgfzy.top

Py:   class Admin(User): pass
来源：http://vub.sjlbkw.cn

PHP:  class Admin extends User {}
来源：http://jbq.ydjk.org.cn

JS:   class Admin extends User {}
来源：http://urw.sufxvd.cn

TS:   class Admin extends User {}
来源：http://wig.zhijiandao.cn

Java: class Admin extends User {}
来源：http://utr.andypj.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hwq.yongpay.top

Ruby: class Admin < User; end
来源：http://lqq.zdbjq.cn

C#:   class Admin : User {}
来源：http://acz.nanxuanxn.top

[G06] 重写方法
来源：http://xjm.yvedp.cn

Py:   def greet(self): return "admin"
来源：http://lsp.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nik.yj20258888.top

JS:   greet() { return "admin"; }
来源：http://tql.cashguo.top


<!-- 参考信息 -->