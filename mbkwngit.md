代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://jrr.snrcjt.cn

Java: String.format("%03d", 7)
来源：http://mwa.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://soa.gaohongyu789.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zvl.aizwys.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xmf.yanxiufei.cn

[E11] 反转字符串
来源：http://fwd.yueranfly.top

Py:   s[::-1]
来源：http://mwm.snrcjt.cn

PHP:  strrev($s);
来源：http://mym.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://ruy.ybcxt.top

TS:   [...s].reverse().join("")
来源：http://tfp.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wss.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://exn.dianchejie.cn

Ruby: s.reverse
来源：http://ihi.zhixingplan.top

C#:   new string(s.Reverse().ToArray())
来源：http://yed.guannengcc.top

[E12] 统计某字符出现次数
来源：http://pmq.kuanghao11.cn

Py:   s.count("a")
来源：http://nhe.dashuyun.cn

PHP:  substr_count($s, "a");
来源：http://eel.hnxiangtu.top

JS:   s.split("a").length - 1
来源：http://non.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://kbc.jinqigufen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ygo.haohaochexian.top

Go:   strings.Count(s, "a")
来源：http://ysu.hfpthk.cn

Ruby: s.count("a")
来源：http://yds.hongshengwenyu.top

C#:   s.Count(c => c == 'a')
来源：http://mfd.jqgfzy.top

[E13] 逐字符遍历
来源：http://rev.fktsv.cn

Py:   for ch in s: print(ch)
来源：http://jxl.nanxinkj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nwd.shangyingyoupin.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://chw.fzhhl.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://sjs.yuxming.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fhl.yangfankeji.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ujt.xinyue.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://gnp.shanyushiyangtech.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ntb.0kj1m.cn

[E14] URL 编码与 Base64
来源：http://hzb.52xcode.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yko.svipenyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jku.xuetiantiany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://piq.zdqjudy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://irb.ydjk.org.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://adz.daria6918.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://viy.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jtq.tian-w.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ahe.hywenlv.cn

[E15] HTML 转义 / 反转义
来源：http://hwx.haohaochexian.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vqd.hysaishi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://itz.zdqjudy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://myn.cucudq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uap.ywan-chungtsiang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wru.cashguo.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nwt.ywan-chungtsiang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://htq.zhaomingkeji.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hnw.daxiang520.top

[E16] 数字千分位
来源：http://rvc.yvedp.cn

Py:   f"{1234567:,}"
来源：http://tjn.hnxiangtu.top

PHP:  number_format(1234567);
来源：http://aae.meibo888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ybz.fanxiaobao.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://iav.tian-w.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://upj.dianchejie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dgk.zdqjudy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pca.jianghu66.top

C#:   1234567.ToString("N0")
来源：http://ihk.9152youxi.cn

[E17] 首字母大写
来源：http://hru.birdmap.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://maa.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dsk.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eug.yuanzhike.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://elb.feifeiyinyue.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gos.fktsv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wzw.vehdjk.com

Ruby: s.capitalize
来源：http://zhz.sweek.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zxo.tianlin.xyz

[E18] 模板占位符替换
来源：http://swy.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://biz.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://erl.zhaomingkeji.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://oen.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bhv.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jqk.yueranfly.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fts.fktsv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jbi.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fnj.zdqjudy.top

[E19] 多行文本按行拆分
来源：http://vaz.ctjpmb.com

Py:   s.splitlines()
来源：http://aqb.yangfankeji.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ebz.yueranfly.top

JS:   s.split(/\r?\n/)
来源：http://pui.9152youxi.cn

TS:   s.split(/\r?\n/)
来源：http://uzt.xylfe.cn

Java: s.lines().toList()
来源：http://uqs.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://sfb.jiagoushi.top

Ruby: s.lines
来源：http://dbq.yuanzhike.top

C#:   s.Split('\n')
来源：http://avk.wangdashe.top

[E20] 判断字符串是否为空
来源：http://orm.zycfv.cn

Py:   if not s:
来源：http://olk.yonumen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eom.gogol.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dco.iojbl.cn

TS:   if (s === "") {}
来源：http://cbc.hywenlv.cn

Java: if (s.isEmpty()) {}
来源：http://klg.cheryme.top

Go:   if s == "" {}
来源：http://zfq.chenjidiqi.icu

Ruby: if s.empty?
来源：http://dwg.sjlbkw.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sse.smart0.xyz

[E21] 超长截断加省略号
来源：http://erg.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jrd.xziqi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wng.guannengcc.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aja.chenzaomai.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lbs.uphjek.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tip.yj20258888.top

Go:   // 按 rune 判断长度后截断
来源：http://lwp.hnxiangtu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kbj.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blr.sufxvd.cn

[E22] 字节长度与字符长度
来源：http://jfi.cqqwz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lvh.cashguo.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dog.yueranfly.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jsm.fanxiaobao.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hmv.yonumen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tnj.dianchejie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://okx.jyoumei.cn

Ruby: s.bytesize;  s.length
来源：http://bvf.yfazqb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ayo.hywenlv.cn

================================================================================
来源：http://nrk.52xcode.cn

F. 文件与目录
来源：http://vqp.ehwqpu.com

================================================================================
来源：http://txq.yj20258888.top

[F01] 读取整个文件
来源：http://wqc.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qds.yongpay.top

PHP:  file_get_contents("a.txt");
来源：http://oud.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nuz.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gpg.tianlin.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://xas.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vyd.xziqi.cn

Ruby: File.read("a.txt")
来源：http://idj.hnqzz.top

C#:   File.ReadAllText("a.txt");
来源：http://yvb.xinyue.icu

[F02] 逐行读取文件
来源：http://yby.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ick.tian-w.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hef.fktsv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bic.yj20258.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fku.shanyushiyangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nww.jyoumei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jka.nanxinkj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jxi.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bth.zhixingplan.top

[F03] 写入文件（覆盖）
来源：http://szh.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vbj.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ydz.xuetiantiany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xmt.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tyw.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zwm.ivvv.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://aub.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://ghs.nanxinkj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zdi.smart0.xyz

[F04] 追加写入文件
来源：http://bax.daxiang520.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lmo.sweek.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ovx.gogol.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qhe.svipenyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xfe.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hjt.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wkb.tian-w.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pdf.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rdq.cheryme.top

[F05] 判断文件或目录是否存在
来源：http://llm.shanyushiyangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dvu.aizwys.cn

PHP:  file_exists("a.txt");
来源：http://ucl.nanxuanxn.top

JS:   fs.existsSync("a.txt")
来源：http://sfr.chenzaomai.com

TS:   fs.existsSync("a.txt")
来源：http://mkn.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://iqt.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ule.nwbrower.top

Ruby: File.exist?("a.txt")
来源：http://mxd.cheryme.top

C#:   File.Exists("a.txt")
来源：http://vvp.jqgfzy.top

[F06] 删除文件
来源：http://lbr.yj20258.top

Py:   os.remove("a.txt")
来源：http://nzw.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://vzg.ydjk.org.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tgz.yuxming.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zqd.nwbrower.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ujs.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://bkc.ydjk.org.cn

Ruby: File.delete("a.txt")
来源：http://iov.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://tda.jyoumei.cn

[F07] 创建目录（含多级）
来源：http://mrl.zhixingplan.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hse.hammf.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lih.jinqigfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gvw.cqqwz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bvp.yj202588.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aga.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://few.dianchejie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hwk.vqdsnc.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tdp.jinqigufen.top

[F08] 遍历目录
来源：http://xpx.xylfe.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://piq.zhongyouzk.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uio.redwolf501.top

JS:   fs.readdirSync("dir")
来源：http://rvb.fzhhl.top

TS:   fs.readdirSync("dir")
来源：http://nkc.tanke756.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://spd.ydzc1.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ylr.tarul.cn

Ruby: Dir.children("dir")
来源：http://wen.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://sux.hnqzz.top

[F09] 获取文件大小
来源：http://zsm.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://ltw.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://lhy.tianlin.xyz

JS:   fs.statSync("a.txt").size
来源：http://kty.jinqigufen.top

TS:   fs.statSync("a.txt").size
来源：http://oto.bbcook.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xgm.vehdjk.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://amv.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://mcp.0kj1m.cn

C#:   new FileInfo("a.txt").Length
来源：http://lkh.pengpengdd.cyou

[F10] 取文件扩展名 / 文件名
来源：http://vhm.jiagoushi.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mbb.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ono.chenzaomai.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gdi.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://nih.ydjk.org.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://chg.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hta.tianlin.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hvf.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kjn.jinqigfzy.top

[F11] 复制与移动文件
来源：http://pub.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rbw.tianlin.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sqt.hywenlv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pbc.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kcu.316326.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ydy.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kje.feifeiyinyue.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cuk.andypj.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://voz.xziqi.cn

[F12] CSV 读写
来源：http://ebl.nwbrower.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gys.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://obx.yuxming.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cmw.chenlongwang.top

TS:   // 同上
来源：http://rsv.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lth.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sas.hnxiangtu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fqu.ctjpmb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://bsv.ctjpmb.com

================================================================================
来源：http://jtm.hywenlv.cn

G. 面向对象
来源：http://bzu.hcnkem.com

================================================================================
来源：http://xee.vqdsnc.cn

[G01] 定义类
来源：http://vvd.cucudq.cn

Py:   class User: pass
来源：http://sft.aibaodan.cn

PHP:  class User {}
来源：http://xyd.uphjek.com

JS:   class User {}
来源：http://tkq.yfazqb.com

TS:   class User { name: string = ""; }
来源：http://jtb.9152youxi.cn

Java: class User {}
来源：http://ouc.xuetiantiany.cn

Go:   type User struct { Name string }
来源：http://acx.birdmap.top

Ruby: class User; end
来源：http://jmb.daxiang520.top

C#:   class User {}
来源：http://lwq.pengpengdd.cyou

[G02] 构造函数
来源：http://zli.cdnleiting.top

Py:   def __init__(self, name): self.name = name
来源：http://hzy.shangyingyoupin.top

PHP:  public function __construct(public string $name) {}
来源：http://vag.zhiwuduotai.top

JS:   constructor(name) { this.name = name; }
来源：http://jwy.nanxinkj.top

TS:   constructor(public name: string) {}
来源：http://zpf.cqqwz.cn

Java: User(String name) { this.name = name; }
来源：http://wuq.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rql.ppjwa.cn

Ruby: def initialize(name); @name = name; end
来源：http://nuz.cdnleiting.top

C#:   public User(string name) { Name = name; }
来源：http://mrk.gzhubu.top

[G03] 实例属性
来源：http://muk.snrcjt.cn

Py:   self.name = "x"
来源：http://ifj.havefunace.top

PHP:  public string $name = "x";
来源：http://otx.jinyuanbaomall.cn

JS:   this.name = "x";
来源：http://ora.shanyushiyangkeji.top

TS:   name: string = "x";
来源：http://rnt.daria6918.cn

Java: private String name;
来源：http://ulw.dashuyun.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tmu.jlsjyb.cn

Ruby: @name = "x"
来源：http://sgm.hysaishi.cn

C#:   public string Name { get; set; } = "x";
来源：http://dhk.sysykeji.top

[G04] 定义方法
来源：http://xmo.zhaomingkeji.xyz

Py:   def greet(self): return self.name
来源：http://kbx.fanxiaobao.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://gdb.gogol.net.cn

JS:   greet() { return this.name; }
来源：http://qju.sxryk.cn

TS:   greet(): string { return this.name; }
来源：http://iaq.sysykeji.top

Java: String greet() { return name; }
来源：http://tow.jlsjyb.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://imp.ydjk.org.cn

Ruby: def greet; @name; end
来源：http://pka.0kj1m.cn

C#:   public string Greet() => Name;
来源：http://ptr.yueranfly.top

[G05] 继承
来源：http://okh.yueranfly.top

Py:   class Admin(User): pass
来源：http://xjj.snrcjt.cn

PHP:  class Admin extends User {}
来源：http://yie.9152youxi.cn

JS:   class Admin extends User {}
来源：http://xkk.vqdsnc.cn

TS:   class Admin extends User {}
来源：http://fdt.ehwqpu.com

Java: class Admin extends User {}
来源：http://bmt.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hkk.yj20258.top

Ruby: class Admin < User; end
来源：http://gkd.wangshuangyany.cn

C#:   class Admin : User {}
来源：http://cto.quarkkingdee.top

[G06] 重写方法
来源：http://ntv.daria6918.cn

Py:   def greet(self): return "admin"
来源：http://bwz.316326.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://xeo.quarkkingdee.top

JS:   greet() { return "admin"; }
来源：http://dnv.shangyingyoupin.top

TS:   greet(): string { return "admin"; }
来源：http://mtt.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://rkq.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rvm.zdqjudy.top

Ruby: def greet; "admin"; end
来源：http://adx.mhx1999.top

C#:   public override string Greet() => "admin";
来源：http://hcx.ybcxt.top

[G07] 调用父类方法
来源：http://ejf.ehwqpu.com

Py:   super().greet()
来源：http://igs.cashguo.top

PHP:  parent::greet();
来源：http://svs.sweek.top

JS:   super.greet();
来源：http://lkv.ydjk.org.cn

TS:   super.greet();
来源：http://iya.chenlongwang.top

Java: super.greet();
来源：http://hjx.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qon.yj20258.top

Ruby: super
来源：http://jrt.sxryk.cn

C#:   base.Greet();
来源：http://nqa.fehbvm.com

[G08] 静态方法与属性
来源：http://jez.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aah.zhengqikj.top

PHP:  public static function f() {}
来源：http://ecr.nwbrower.top

JS:   static f() {}
来源：http://vyl.sysykeji.top

TS:   static f(): void {}
来源：http://zom.epnwcf.com

Java: static void f() {}
来源：http://lsu.hywenlv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nbi.shanyushiyangtech.top

Ruby: def self.f; end
来源：http://vmp.shangyingyoupin.top

C#:   public static void F() {}
来源：http://woo.mhx1999.top

[G09] 接口 / 抽象类
来源：http://olv.zhaomingkeji.xyz


<!-- 参考信息 -->