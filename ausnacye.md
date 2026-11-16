代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://zrp.ydzc1.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yog.tanke756.top

Ruby: s.gsub(/\s+/, "")
来源：http://qqk.hammf.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aay.yuanzhike.top

[E10] 左侧补零 / 定长填充
来源：http://xhu.havefunace.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://evb.uphjek.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aqo.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://hhb.yuxming.cn

TS:   "7".padStart(3, "0")
来源：http://rrz.c1oappe.top

Java: String.format("%03d", 7)
来源：http://dbl.yanxiufei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ygu.gotoacloud.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gxm.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cxl.ydzc1.top

[E11] 反转字符串
来源：http://frk.redwolf501.top

Py:   s[::-1]
来源：http://dbg.ydzc1.top

PHP:  strrev($s);
来源：http://cbp.jinyuanbaomall.cn

JS:   [...s].reverse().join("")
来源：http://izi.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://hrg.yongpay.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wln.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://euv.sufxvd.cn

Ruby: s.reverse
来源：http://wag.ivvv.top

C#:   new string(s.Reverse().ToArray())
来源：http://llp.xziqi.cn

[E12] 统计某字符出现次数
来源：http://whe.cqqwz.cn

Py:   s.count("a")
来源：http://fdo.cheryme.top

PHP:  substr_count($s, "a");
来源：http://xzo.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://bxl.ydzc1.top

TS:   s.split("a").length - 1
来源：http://eay.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qex.xuanzx.com

Go:   strings.Count(s, "a")
来源：http://mvc.hesvh.cn

Ruby: s.count("a")
来源：http://qtn.svipenyu.cn

C#:   s.Count(c => c == 'a')
来源：http://gxs.zhengqikj.top

[E13] 逐字符遍历
来源：http://yeu.zycfv.cn

Py:   for ch in s: print(ch)
来源：http://elx.yfazqb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iob.fktsv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://szp.zhiwuduotai.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://grs.hysaishi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gge.wangdashe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vfi.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://znj.shuidangran.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pea.chenjidiqi.icu

[E14] URL 编码与 Base64
来源：http://bwp.zhiwuduotai.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pqx.0kj1m.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ofc.wangshuangyany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ply.yuanzhike.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tie.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lbn.chenjidiqi.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uso.pengpengdd.cyou

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qah.hongshengwenyu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vqk.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://fnc.sysykeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xzv.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://stt.fengsongda.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kww.shanyushiyangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dsd.cdnleiting.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sqs.svipenyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lbw.jyoumei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dvb.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iwj.redwolf501.top

[E16] 数字千分位
来源：http://hfv.shangyingyoupin.top

Py:   f"{1234567:,}"
来源：http://sis.cqqwz.cn

PHP:  number_format(1234567);
来源：http://jzs.nanxinkj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dzf.zhaomingkeji.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://asl.hfpthk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tle.zhoulong.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tjg.ppjwa.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://alk.vehdjk.com

C#:   1234567.ToString("N0")
来源：http://gcc.chenjidiqi.icu

[E17] 首字母大写
来源：http://mnw.hesvh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jvs.jinghuilouyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fyi.havefunace.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://olx.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://izj.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ufm.bbcook.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kvb.wangshuangyany.cn

Ruby: s.capitalize
来源：http://jzx.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://efw.yj20258888.top

[E18] 模板占位符替换
来源：http://kyh.fktsv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pau.0kj1m.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://evl.jqgfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gon.cashguo.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gbu.havefunace.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wzg.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zvo.svipenyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ycy.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://crg.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://fef.guannengcc.top

Py:   s.splitlines()
来源：http://ikn.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ddk.shuidangran.top

JS:   s.split(/\r?\n/)
来源：http://yet.zhoulong.xyz

TS:   s.split(/\r?\n/)
来源：http://bby.xuetiantiany.cn

Java: s.lines().toList()
来源：http://rps.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://nec.jqgufenzy.top

Ruby: s.lines
来源：http://ivn.jinyuanbaomall.cn

C#:   s.Split('\n')
来源：http://kcn.shuidangran.top

[E20] 判断字符串是否为空
来源：http://bbo.pycfn.com

Py:   if not s:
来源：http://yub.smart0.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uli.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hmy.pycfn.com

TS:   if (s === "") {}
来源：http://plb.tarul.cn

Java: if (s.isEmpty()) {}
来源：http://ztg.cashguo.top

Go:   if s == "" {}
来源：http://dqq.hysaishi.cn

Ruby: if s.empty?
来源：http://zqm.nanxinkj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mlf.shuidangran.top

[E21] 超长截断加省略号
来源：http://dfj.fzhhl.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ney.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ncd.ydzc1.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qmm.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pfz.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bcb.svipenyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://zbj.jiagoushi.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ohl.fengsongda.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tue.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://jvb.zhengqikj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sdl.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tzx.hammf.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uex.snrcjt.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mar.aizwys.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qyc.kuanghao11.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uqi.jinghuilouyu.cn

Ruby: s.bytesize;  s.length
来源：http://fbv.cashguo.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jtu.smart0.xyz

================================================================================
来源：http://mpg.daxiang520.top

F. 文件与目录
来源：http://cvm.shuidangran.top

================================================================================
来源：http://klo.cashguo.top

[F01] 读取整个文件
来源：http://kxq.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pms.hnxiangtu.top

PHP:  file_get_contents("a.txt");
来源：http://wel.nanxinkj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xab.sweek.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ooh.cqqwz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ird.yj20258888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uqb.zycfv.cn

Ruby: File.read("a.txt")
来源：http://mdo.guannengcc.top

C#:   File.ReadAllText("a.txt");
来源：http://vxy.iojbl.cn

[F02] 逐行读取文件
来源：http://ycj.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://idp.smart0.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jxx.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://miy.tian-w.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nck.chenlongwang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rxw.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fif.yangfankeji.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zve.xziqi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://npr.cdnleiting.top

[F03] 写入文件（覆盖）
来源：http://jvf.tarul.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zmx.jqgfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://doz.chenlongwang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rkq.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dea.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bfu.kuanghao11.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://imm.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://eko.hcnkem.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://juv.sweek.top

[F04] 追加写入文件
来源：http://uwr.tian-w.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pvu.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ohp.0kj1m.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wvv.birdmap.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://neh.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uyn.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bvo.ybcxt.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://awv.yuxming.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://klt.sxryk.cn

[F05] 判断文件或目录是否存在
来源：http://ect.hysaishi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wda.sufxvd.cn

PHP:  file_exists("a.txt");
来源：http://lsx.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://qqf.xziqi.cn

TS:   fs.existsSync("a.txt")
来源：http://szo.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://adv.ydzc1.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://itp.epnwcf.com

Ruby: File.exist?("a.txt")
来源：http://uii.smart0.xyz

C#:   File.Exists("a.txt")
来源：http://per.ydjk.org.cn

[F06] 删除文件
来源：http://zpv.birdmap.top

Py:   os.remove("a.txt")
来源：http://mqu.xziqi.cn

PHP:  unlink("a.txt");
来源：http://njl.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://epz.yj202588.top

TS:   fs.unlinkSync("a.txt")
来源：http://jui.feifeiyinyue.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xqq.nanxuanxn.top

Go:   os.Remove("a.txt")
来源：http://hae.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://iyz.yueranfly.top

C#:   File.Delete("a.txt");
来源：http://wil.cqqwz.cn

[F07] 创建目录（含多级）
来源：http://vfm.cheryme.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tkf.jinqigufen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fli.tarul.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://snk.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://frm.dashuyun.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zfw.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://acq.hesvh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wni.yfazqb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kxe.ppjwa.cn

[F08] 遍历目录
来源：http://avf.yvedp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cyk.gogol.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gvw.xylfe.cn

JS:   fs.readdirSync("dir")
来源：http://ezs.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://tcx.hysaishi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bbs.fehbvm.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://wsf.zhengqikj.top

Ruby: Dir.children("dir")
来源：http://uie.0kj1m.cn

C#:   Directory.GetFiles("dir")
来源：http://tkt.jqgufenzy.top

[F09] 获取文件大小
来源：http://yrk.nwbrower.top

Py:   os.path.getsize("a.txt")
来源：http://pmi.yfazqb.com

PHP:  filesize("a.txt");
来源：http://ovx.ydjk.org.cn

JS:   fs.statSync("a.txt").size
来源：http://xbu.vehdjk.com

TS:   fs.statSync("a.txt").size
来源：http://xdf.ehwqpu.com

Java: Files.size(Path.of("a.txt"))
来源：http://bhx.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fmu.bjfxy.top

Ruby: File.size("a.txt")
来源：http://dya.jinqigufen.top

C#:   new FileInfo("a.txt").Length
来源：http://bmf.aibaodan.cn

[F10] 取文件扩展名 / 文件名
来源：http://nor.ctjpmb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vtd.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sqy.gotoacloud.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ruk.vqdsnc.cn

TS:   path.extname("a.txt")
来源：http://cmo.ydzc1.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kbo.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iya.dianchejie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aye.pycfn.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lwy.shuidangran.top

[F11] 复制与移动文件
来源：http://otz.ctjpmb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ywh.gzhubu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jzo.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vrr.vqdsnc.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jiu.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ahv.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wxb.316326.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://snv.nanxuanxn.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sqy.havefunace.top

[F12] CSV 读写
来源：http://mmi.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://npw.cheryme.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://asj.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xrf.dashuyun.cn

TS:   // 同上
来源：http://qjd.shanyushiyangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vgx.yvedp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://crm.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uyg.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uht.hfpthk.cn

================================================================================
来源：http://qrm.tanke756.top

G. 面向对象
来源：http://qeo.pycfn.com

================================================================================
来源：http://iyf.yfazqb.com

[G01] 定义类
来源：http://jog.nwbrower.top

Py:   class User: pass
来源：http://yll.hfpthk.cn

PHP:  class User {}
来源：http://zzt.jyoumei.cn

JS:   class User {}
来源：http://rse.shzxlz.cn

TS:   class User { name: string = ""; }
来源：http://trd.chenjidiqi.icu

Java: class User {}
来源：http://iwy.yueranfly.top

Go:   type User struct { Name string }
来源：http://dpv.vqdsnc.cn

Ruby: class User; end
来源：http://grv.chenlongwang.top

C#:   class User {}
来源：http://dqj.0kj1m.cn

[G02] 构造函数
来源：http://xbk.cqqwz.cn

Py:   def __init__(self, name): self.name = name
来源：http://kej.yanxiufei.cn

PHP:  public function __construct(public string $name) {}
来源：http://key.ydzc1.top

JS:   constructor(name) { this.name = name; }
来源：http://bve.zhengqikj.top

TS:   constructor(public name: string) {}
来源：http://ndx.vehdjk.com

Java: User(String name) { this.name = name; }
来源：http://qpz.yonumen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uop.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://czk.fktsv.cn

C#:   public User(string name) { Name = name; }
来源：http://mfu.yvedp.cn

[G03] 实例属性
来源：http://ctd.yvedp.cn

Py:   self.name = "x"
来源：http://uwa.hywenlv.cn

PHP:  public string $name = "x";
来源：http://blu.jlsjyb.cn

JS:   this.name = "x";
来源：http://wff.zhoulong.xyz

TS:   name: string = "x";
来源：http://gqy.hywenlv.cn

Java: private String name;
来源：http://bwg.epnwcf.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rgv.jinyuanbaomall.cn

Ruby: @name = "x"
来源：http://hin.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://mzx.cucudq.cn

[G04] 定义方法
来源：http://xsz.yj20258.top

Py:   def greet(self): return self.name
来源：http://hwh.hfpthk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rwt.birdmap.top

JS:   greet() { return this.name; }
来源：http://mju.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://hlp.snrcjt.cn

Java: String greet() { return name; }
来源：http://xvn.jianghu66.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://beb.hfpthk.cn

Ruby: def greet; @name; end
来源：http://mdn.9152youxi.cn

C#:   public string Greet() => Name;
来源：http://yng.xziqi.cn

[G05] 继承
来源：http://wpo.gzhubu.top

Py:   class Admin(User): pass
来源：http://ynz.andypj.xyz

PHP:  class Admin extends User {}
来源：http://wml.hammf.cn

JS:   class Admin extends User {}
来源：http://xab.hammf.cn

TS:   class Admin extends User {}
来源：http://cah.shzxlz.cn

Java: class Admin extends User {}
来源：http://wiy.shzxlz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zoi.jqgufenzy.top

Ruby: class Admin < User; end
来源：http://rpl.yj202588.top

C#:   class Admin : User {}
来源：http://ezg.xinyue.icu

[G06] 重写方法
来源：http://vyi.sufxvd.cn

Py:   def greet(self): return "admin"
来源：http://ull.jinqigfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://aju.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://byf.0kj1m.cn

TS:   greet(): string { return "admin"; }
来源：http://kdc.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://nwm.chenzaomai.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zgl.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://zvb.fehbvm.com

C#:   public override string Greet() => "admin";
来源：http://shp.xziqi.cn

[G07] 调用父类方法
来源：http://gpe.ehwqpu.com

Py:   super().greet()
来源：http://eaw.jiagoushi.top

PHP:  parent::greet();
来源：http://tjx.ybcxt.top

JS:   super.greet();
来源：http://dva.yongpay.top

TS:   super.greet();
来源：http://hrs.snrcjt.cn

Java: super.greet();
来源：http://iel.fzhhl.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rgl.zhijiandao.cn

Ruby: super
来源：http://flk.wangshuangyany.cn

C#:   base.Greet();
来源：http://vus.xinyue.icu

[G08] 静态方法与属性
来源：http://hhq.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://csf.sjlbkw.cn


<!-- 参考信息 -->