代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vyg.yueranfly.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kei.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://eap.jlsjyb.cn

TS:   s.replace(/\s+/g, "")
来源：http://jgg.zhongyouzk.top

Java: s.replaceAll("\\s+", "")
来源：http://uje.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rbp.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rsc.chenlongwang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oyp.bjfxy.top

[E10] 左侧补零 / 定长填充
来源：http://iva.vqdsnc.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lvk.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://byj.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://kah.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://shz.0kj1m.cn

Java: String.format("%03d", 7)
来源：http://jhj.zhiwuduotai.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mnk.fehbvm.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uqm.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://voq.hammf.cn

[E11] 反转字符串
来源：http://qrr.shanyushiyangtech.top

Py:   s[::-1]
来源：http://exc.xylfe.cn

PHP:  strrev($s);
来源：http://zqq.guowangkeji.top

JS:   [...s].reverse().join("")
来源：http://cfo.ydzc1.top

TS:   [...s].reverse().join("")
来源：http://sth.xingfuxueyuan.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://lvp.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ukl.shzxlz.cn

Ruby: s.reverse
来源：http://yfc.haohaochexian.top

C#:   new string(s.Reverse().ToArray())
来源：http://uxa.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://mag.sweek.top

Py:   s.count("a")
来源：http://qme.jiagoushi.top

PHP:  substr_count($s, "a");
来源：http://udb.wangshuangyany.cn

JS:   s.split("a").length - 1
来源：http://und.yuanzhike.top

TS:   s.split("a").length - 1
来源：http://igc.shuidangran.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qhj.316326.xyz

Go:   strings.Count(s, "a")
来源：http://oew.0kj1m.cn

Ruby: s.count("a")
来源：http://weo.yongpay.top

C#:   s.Count(c => c == 'a')
来源：http://kam.chenlongwang.top

[E13] 逐字符遍历
来源：http://iug.xingfuxueyuan.xyz

Py:   for ch in s: print(ch)
来源：http://bld.tarul.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fqa.9152youxi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lzs.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://ike.xingfuxueyuan.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qzk.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vsl.jqgufenzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gnn.316326.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wnm.andypj.xyz

[E14] URL 编码与 Base64
来源：http://lpw.yj20258.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dgr.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vxi.yanxiufei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://svz.sxryk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vez.jinqigufen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uru.jqgfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://esc.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tot.cucudq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ygh.ppjwa.cn

[E15] HTML 转义 / 反转义
来源：http://mjz.cheryme.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qil.xylfe.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eul.guannengcc.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dtz.ppjwa.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yni.zhijiandao.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://agq.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ctq.jqgufenzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://owf.zhengqikj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vwp.ehwqpu.com

[E16] 数字千分位
来源：http://nlg.yj20258888.top

Py:   f"{1234567:,}"
来源：http://rbn.zhongyouzk.top

PHP:  number_format(1234567);
来源：http://cco.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wlt.shanyushiyangtech.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nuy.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rbc.ehwqpu.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rqc.yvedp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fcn.daxiang520.top

C#:   1234567.ToString("N0")
来源：http://oqt.ivvv.top

[E17] 首字母大写
来源：http://lak.ydzc1.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qec.cucudq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dan.zhijiandao.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://akq.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oxt.daria6918.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rnz.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mmu.nwbrower.top

Ruby: s.capitalize
来源：http://uol.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xel.wangdashe.top

[E18] 模板占位符替换
来源：http://jtw.bbcook.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://upa.nanxinkj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://khk.hcnkem.com

JS:   tpl.replaceAll("{name}", name)
来源：http://xpp.fengsongda.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mkb.9152youxi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tvo.9152youxi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ppp.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kiq.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lts.jianghu66.top

[E19] 多行文本按行拆分
来源：http://jdo.tian-w.cn

Py:   s.splitlines()
来源：http://grm.sysykeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://edg.zdqjudy.top

JS:   s.split(/\r?\n/)
来源：http://qwr.nwbrower.top

TS:   s.split(/\r?\n/)
来源：http://erm.zhengqikj.top

Java: s.lines().toList()
来源：http://kvv.vqdsnc.cn

Go:   strings.Split(s, "\n")
来源：http://irk.haohaochexian.top

Ruby: s.lines
来源：http://kav.pengpengdd.cyou

C#:   s.Split('\n')
来源：http://jgw.yongpay.top

[E20] 判断字符串是否为空
来源：http://dlu.pengpengdd.cyou

Py:   if not s:
来源：http://eer.bbcook.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rjx.zhaomingkeji.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pqi.yangfankeji.com

TS:   if (s === "") {}
来源：http://ozr.fanxiaobao.xyz

Java: if (s.isEmpty()) {}
来源：http://avc.ppjwa.cn

Go:   if s == "" {}
来源：http://tyz.yj202588.top

Ruby: if s.empty?
来源：http://maw.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gns.ivvv.top

[E21] 超长截断加省略号
来源：http://esu.tanke756.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sus.jlsjyb.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dhc.jyoumei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://izh.chenlongwang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tit.yonumen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vmn.hcnkem.com

Go:   // 按 rune 判断长度后截断
来源：http://fwd.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wbw.redwolf501.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ivc.sysykeji.top

[E22] 字节长度与字符长度
来源：http://dld.hnxiangtu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kfo.redwolf501.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zfs.chenzaomai.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rua.gogol.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iwf.guannengcc.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gfq.nanxinkj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ait.hcnkem.com

Ruby: s.bytesize;  s.length
来源：http://avt.cdnleiting.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xou.dianchejie.cn

================================================================================
来源：http://acx.jqgufenzy.top

F. 文件与目录
来源：http://ubp.yj20258888.top

================================================================================
来源：http://ffp.cqqwz.cn

[F01] 读取整个文件
来源：http://ayp.hongshengwenyu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bxs.jinyuanbaomall.cn

PHP:  file_get_contents("a.txt");
来源：http://fev.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dfe.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wqz.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jzs.zdqjudy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sij.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://pjs.kuanghao11.cn

C#:   File.ReadAllText("a.txt");
来源：http://mfk.jianghu66.top

[F02] 逐行读取文件
来源：http://goq.yj20258888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://khy.cucudq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uqg.yuxming.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://snz.xinyue.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sex.yueranfly.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://abd.xuetiantiany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://egw.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jqm.sxryk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bdo.tarul.cn

[F03] 写入文件（覆盖）
来源：http://tix.sxryk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dbh.hnqzz.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tut.sweek.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nhv.yanxiufei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rqo.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ljw.nanxuanxn.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://knc.quarkkingdee.top

Ruby: File.write("a.txt", "hi")
来源：http://oqf.xingfuxueyuan.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lpi.hnxiangtu.top

[F04] 追加写入文件
来源：http://rwv.ydjk.org.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rsj.snrcjt.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lho.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hxd.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://owa.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zas.cucudq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vrn.fengsongda.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pon.shzxlz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://riv.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://ocy.wangshuangyany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://puu.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://qhc.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://ekp.tarul.cn

TS:   fs.existsSync("a.txt")
来源：http://iqz.feifeiyinyue.top

Java: Files.exists(Path.of("a.txt"))
来源：http://erw.yfazqb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bjy.cqqwz.cn

Ruby: File.exist?("a.txt")
来源：http://iea.ydzc1.top

C#:   File.Exists("a.txt")
来源：http://uns.guannengcc.top

[F06] 删除文件
来源：http://wxp.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://ouw.guowangkeji.top

PHP:  unlink("a.txt");
来源：http://hba.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://utk.cashguo.top

TS:   fs.unlinkSync("a.txt")
来源：http://qyb.cheryme.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zoe.daria6918.cn

Go:   os.Remove("a.txt")
来源：http://rrz.hammf.cn

Ruby: File.delete("a.txt")
来源：http://hqr.jinqigfzy.top

C#:   File.Delete("a.txt");
来源：http://woy.tian-w.cn

[F07] 创建目录（含多级）
来源：http://bbz.ctjpmb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gps.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fds.xinyue.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://phe.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aob.guowangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xoo.yuanzhike.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://auu.cqqwz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gty.tanke756.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sqz.meibo888.top

[F08] 遍历目录
来源：http://aur.daxiang520.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tdl.gaohongyu789.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ozc.ivvv.top

JS:   fs.readdirSync("dir")
来源：http://tui.bbcook.cn

TS:   fs.readdirSync("dir")
来源：http://wfs.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nue.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rmq.mhx1999.top

Ruby: Dir.children("dir")
来源：http://cif.xziqi.cn

C#:   Directory.GetFiles("dir")
来源：http://fps.gogol.net.cn

[F09] 获取文件大小
来源：http://rxj.zhaomingkeji.xyz

Py:   os.path.getsize("a.txt")
来源：http://qkr.ydzc1.top

PHP:  filesize("a.txt");
来源：http://meb.cdnleiting.top

JS:   fs.statSync("a.txt").size
来源：http://rwx.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://soe.sxryk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://erz.hysaishi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ypg.jiagoushi.top

Ruby: File.size("a.txt")
来源：http://qum.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://rbe.birdmap.top

[F10] 取文件扩展名 / 文件名
来源：http://bdx.jianghu66.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hos.cucudq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dix.hnxiangtu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bzf.svipenyu.cn

TS:   path.extname("a.txt")
来源：http://rmn.daria6918.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://irg.jinyuanbaomall.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dat.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://osd.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fxt.iojbl.cn

[F11] 复制与移动文件
来源：http://osd.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dqi.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bav.pengpengdd.cyou

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xgf.hnqzz.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ybh.cqqwz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dbt.52xcode.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://psm.zhoulong.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://onm.316326.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gaz.iojbl.cn

[F12] CSV 读写
来源：http://ocn.9152youxi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://thh.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dyr.uphjek.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://myb.jlsjyb.cn

TS:   // 同上
来源：http://ngs.yanxiufei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qpp.yanxiufei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zzg.sufxvd.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vxa.yj20258.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ydl.aizwys.cn

================================================================================
来源：http://dqd.feifeiyinyue.top

G. 面向对象
来源：http://tpt.0kj1m.cn

================================================================================
来源：http://xyc.jinqigfzy.top

[G01] 定义类
来源：http://ios.vehdjk.com

Py:   class User: pass
来源：http://pzo.chenjidiqi.icu

PHP:  class User {}
来源：http://wpr.hesvh.cn

JS:   class User {}
来源：http://ymw.redwolf501.top

TS:   class User { name: string = ""; }
来源：http://kiy.quarkkingdee.top

Java: class User {}
来源：http://tte.quarkkingdee.top

Go:   type User struct { Name string }
来源：http://vxd.ydjk.org.cn

Ruby: class User; end
来源：http://dwi.gzhubu.top

C#:   class User {}
来源：http://toq.xuanzx.com

[G02] 构造函数
来源：http://koz.jyoumei.cn

Py:   def __init__(self, name): self.name = name
来源：http://jwv.c1oappe.top

PHP:  public function __construct(public string $name) {}
来源：http://mnv.xuetiantiany.cn

JS:   constructor(name) { this.name = name; }
来源：http://juv.aibaodan.cn

TS:   constructor(public name: string) {}
来源：http://ihg.nwbrower.top

Java: User(String name) { this.name = name; }
来源：http://puf.hywenlv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wgg.uphjek.com

Ruby: def initialize(name); @name = name; end
来源：http://vgn.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://fhc.vehdjk.com

[G03] 实例属性
来源：http://vhz.sjlbkw.cn

Py:   self.name = "x"
来源：http://zfx.tian-w.cn

PHP:  public string $name = "x";
来源：http://lwd.aibaodan.cn

JS:   this.name = "x";
来源：http://nnf.sweek.top

TS:   name: string = "x";
来源：http://cry.tianlin.xyz

Java: private String name;
来源：http://pnd.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lfu.zhixingplan.top

Ruby: @name = "x"
来源：http://qlj.feifeiyinyue.top

C#:   public string Name { get; set; } = "x";
来源：http://zxn.wangshuangyany.cn

[G04] 定义方法
来源：http://uxx.bbcook.cn

Py:   def greet(self): return self.name
来源：http://wma.quarkkingdee.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nwg.chenlongwang.top

JS:   greet() { return this.name; }
来源：http://fip.aizwys.cn

TS:   greet(): string { return this.name; }
来源：http://zpz.aizwys.cn

Java: String greet() { return name; }
来源：http://nas.jlsjyb.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kqc.jinqigufen.top

Ruby: def greet; @name; end
来源：http://psm.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://hwx.hnxiangtu.top

[G05] 继承
来源：http://nvj.dashuyun.cn

Py:   class Admin(User): pass
来源：http://ztm.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://ssq.yvedp.cn

JS:   class Admin extends User {}
来源：http://vmb.zdbjq.cn

TS:   class Admin extends User {}
来源：http://cym.chenjidiqi.icu

Java: class Admin extends User {}
来源：http://atj.yonumen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jsq.zhengqikj.top

Ruby: class Admin < User; end
来源：http://ndo.ydzc1.top

C#:   class Admin : User {}
来源：http://krx.zhijiandao.cn

[G06] 重写方法
来源：http://tur.redwolf501.top

Py:   def greet(self): return "admin"
来源：http://rlj.jinyuanbaomall.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kbs.guowangkeji.top

JS:   greet() { return "admin"; }
来源：http://uco.aizwys.cn

TS:   greet(): string { return "admin"; }
来源：http://mth.havefunace.top

Java: @Override String greet() { return "admin"; }
来源：http://vtu.sysykeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://aoj.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://lsb.uphjek.com

C#:   public override string Greet() => "admin";
来源：http://zyw.xuetiantiany.cn

[G07] 调用父类方法
来源：http://zwt.cdnleiting.top

Py:   super().greet()
来源：http://qal.jiagoushi.top

PHP:  parent::greet();
来源：http://wtm.yangfankeji.com

JS:   super.greet();
来源：http://ejr.9152youxi.cn

TS:   super.greet();
来源：http://ccr.sjlbkw.cn

Java: super.greet();
来源：http://tzs.mhx1999.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ppa.xingfuxueyuan.xyz


<!-- 参考信息 -->