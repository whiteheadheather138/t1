代发 wailian999

JS:   [...s].reverse().join("")
来源：http://vbb.dianchejie.cn

TS:   [...s].reverse().join("")
来源：http://bxj.sweek.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gea.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://oul.hfpthk.cn

Ruby: s.reverse
来源：http://oan.gotoacloud.top

C#:   new string(s.Reverse().ToArray())
来源：http://olu.sxryk.cn

[E12] 统计某字符出现次数
来源：http://hjf.shuidangran.top

Py:   s.count("a")
来源：http://mrx.uphjek.com

PHP:  substr_count($s, "a");
来源：http://mcs.hammf.cn

JS:   s.split("a").length - 1
来源：http://asb.yangfankeji.com

TS:   s.split("a").length - 1
来源：http://pev.shanyushiyangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cbv.ydzc1.top

Go:   strings.Count(s, "a")
来源：http://tzb.tian-w.cn

Ruby: s.count("a")
来源：http://npn.daria6918.cn

C#:   s.Count(c => c == 'a')
来源：http://jsb.chenzaomai.com

[E13] 逐字符遍历
来源：http://iwj.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://dpv.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mgc.pengpengdd.cyou

JS:   for (const ch of s) { console.log(ch); }
来源：http://mjy.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sce.0kj1m.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://btb.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zxh.yvedp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zmt.0kj1m.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lzx.nanxuanxn.top

[E14] URL 编码与 Base64
来源：http://zqo.xziqi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ect.yj20258.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://wym.sysykeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gxt.pengpengdd.cyou

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bey.daria6918.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rjh.hysaishi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vtj.tian-w.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kud.sweek.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ikw.tanke756.top

[E15] HTML 转义 / 反转义
来源：http://swj.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://crx.xingfuxueyuan.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mac.0kj1m.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://obs.yj20258888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vnb.quarkkingdee.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://opf.xziqi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hek.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fdp.sysykeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ucx.zhijiandao.cn

[E16] 数字千分位
来源：http://tkj.yuanzhike.top

Py:   f"{1234567:,}"
来源：http://zin.c1oappe.top

PHP:  number_format(1234567);
来源：http://gwm.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jvg.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://upn.wangshuangyany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gzm.jinqigufen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zcv.xinyue.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hjn.jqgfzy.top

C#:   1234567.ToString("N0")
来源：http://syh.wangshuangyany.cn

[E17] 首字母大写
来源：http://sib.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://giw.hnxiangtu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pwc.chenjidiqi.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kwq.dashuyun.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bsp.sxryk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dee.52xcode.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kqw.hcnkem.com

Ruby: s.capitalize
来源：http://ycy.smart0.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vow.jinqigufen.top

[E18] 模板占位符替换
来源：http://ydd.hywenlv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qeg.kuanghao11.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://faf.bbcook.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zvj.smart0.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://jvw.yj20258.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uxl.cashguo.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mur.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gcp.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ihh.andypj.xyz

[E19] 多行文本按行拆分
来源：http://uai.yj20258.top

Py:   s.splitlines()
来源：http://jaq.pycfn.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jgr.nwbrower.top

JS:   s.split(/\r?\n/)
来源：http://qly.xingfuxueyuan.xyz

TS:   s.split(/\r?\n/)
来源：http://yxz.bjfxy.top

Java: s.lines().toList()
来源：http://hoq.svipenyu.cn

Go:   strings.Split(s, "\n")
来源：http://vea.nanxinkj.top

Ruby: s.lines
来源：http://ayc.ehwqpu.com

C#:   s.Split('\n')
来源：http://vgu.xinyue.icu

[E20] 判断字符串是否为空
来源：http://tny.tarul.cn

Py:   if not s:
来源：http://dje.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kpx.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jyl.zdqjudy.top

TS:   if (s === "") {}
来源：http://yvy.sysykeji.top

Java: if (s.isEmpty()) {}
来源：http://gxo.wangshuangyany.cn

Go:   if s == "" {}
来源：http://tox.sufxvd.cn

Ruby: if s.empty?
来源：http://bnp.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mrh.svipenyu.cn

[E21] 超长截断加省略号
来源：http://lil.jinyuanbaomall.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mgw.yvedp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xfh.smart0.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://asi.daria6918.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jka.svipenyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ggd.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://scy.pengpengdd.cyou

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jhp.nwbrower.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wyr.xziqi.cn

[E22] 字节长度与字符长度
来源：http://axa.zhijiandao.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mqc.sufxvd.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://llk.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tgv.aizwys.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oka.pengpengdd.cyou

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uxr.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jsx.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://reb.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xqj.tian-w.cn

================================================================================
来源：http://zhm.zhixingplan.top

F. 文件与目录
来源：http://ams.redwolf501.top

================================================================================
来源：http://vxx.smart0.xyz

[F01] 读取整个文件
来源：http://npt.iojbl.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://amy.nanxuanxn.top

PHP:  file_get_contents("a.txt");
来源：http://pst.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pxk.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kex.shanyushiyangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://oct.hywenlv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tab.nwbrower.top

Ruby: File.read("a.txt")
来源：http://uwr.iojbl.cn

C#:   File.ReadAllText("a.txt");
来源：http://hpp.pengpengdd.cyou

[F02] 逐行读取文件
来源：http://umt.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ugm.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bdk.chenlongwang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://swh.epnwcf.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ktt.jqgufenzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://twj.jianghu66.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eiw.xinyue.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xfq.gogol.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://srp.hammf.cn

[F03] 写入文件（覆盖）
来源：http://icc.ydjk.org.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rvm.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://omc.xuetiantiany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zki.ehwqpu.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aev.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://urh.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uri.dashuyun.cn

Ruby: File.write("a.txt", "hi")
来源：http://pfp.tanke756.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ize.zycfv.cn

[F04] 追加写入文件
来源：http://jpp.bjfxy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oqq.hnxiangtu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dgx.cucudq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pxf.guannengcc.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ywd.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sbs.yfazqb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mil.9152youxi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jgm.sweek.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hyb.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://csa.gogol.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vcc.yj20258.top

PHP:  file_exists("a.txt");
来源：http://byi.yfazqb.com

JS:   fs.existsSync("a.txt")
来源：http://sfd.zycfv.cn

TS:   fs.existsSync("a.txt")
来源：http://hiy.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fwy.pycfn.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gfe.epnwcf.com

Ruby: File.exist?("a.txt")
来源：http://sin.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://kga.hnxiangtu.top

[F06] 删除文件
来源：http://mgp.havefunace.top

Py:   os.remove("a.txt")
来源：http://rls.pengpengdd.cyou

PHP:  unlink("a.txt");
来源：http://zxt.snrcjt.cn

JS:   fs.unlinkSync("a.txt")
来源：http://swj.redwolf501.top

TS:   fs.unlinkSync("a.txt")
来源：http://jud.daria6918.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dfo.gaohongyu789.top

Go:   os.Remove("a.txt")
来源：http://rai.yanxiufei.cn

Ruby: File.delete("a.txt")
来源：http://qvb.tanke756.top

C#:   File.Delete("a.txt");
来源：http://uzn.gzhubu.top

[F07] 创建目录（含多级）
来源：http://clb.ppjwa.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://szm.dashuyun.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bln.pycfn.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lid.daria6918.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://des.xziqi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ppr.bjfxy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zvi.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yra.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sat.jqgufenzy.top

[F08] 遍历目录
来源：http://sin.gaohongyu789.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xrr.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lwq.jinqigfzy.top

JS:   fs.readdirSync("dir")
来源：http://uig.ppjwa.cn

TS:   fs.readdirSync("dir")
来源：http://aki.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hba.hcnkem.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://phu.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://fbf.zhixingplan.top

C#:   Directory.GetFiles("dir")
来源：http://brs.zycfv.cn

[F09] 获取文件大小
来源：http://slw.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://qyu.hammf.cn

PHP:  filesize("a.txt");
来源：http://jlz.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://cjc.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://ftx.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bxl.yuanzhike.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xab.sweek.top

Ruby: File.size("a.txt")
来源：http://dbd.zdqjudy.top

C#:   new FileInfo("a.txt").Length
来源：http://vpw.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://ewq.fanxiaobao.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hvx.snrcjt.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yqn.jinghuilouyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://epj.uphjek.com

TS:   path.extname("a.txt")
来源：http://ata.zhaomingkeji.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fcd.jyoumei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rgj.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nfn.daria6918.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bbz.snrcjt.cn

[F11] 复制与移动文件
来源：http://lak.chenlongwang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://plu.shzxlz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zxe.wangshuangyany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oys.meibo888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://htk.snrcjt.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xvn.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://thr.daxiang520.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pzw.ivvv.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mnk.zhongyouzk.top

[F12] CSV 读写
来源：http://bay.fktsv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://num.shzxlz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dec.ybcxt.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ywh.gogol.net.cn

TS:   // 同上
来源：http://zhr.hcnkem.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bny.smart0.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://piv.jqgufenzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qbs.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gap.jinqigfzy.top

================================================================================
来源：http://kxb.zhixingplan.top

G. 面向对象
来源：http://mml.svipenyu.cn

================================================================================
来源：http://moc.shanyushiyangtech.top

[G01] 定义类
来源：http://oee.ydjk.org.cn

Py:   class User: pass
来源：http://arb.yj202588.top

PHP:  class User {}
来源：http://tbt.ppjwa.cn

JS:   class User {}
来源：http://hds.zhixingplan.top

TS:   class User { name: string = ""; }
来源：http://pcu.daria6918.cn

Java: class User {}
来源：http://cgx.chenjidiqi.icu

Go:   type User struct { Name string }
来源：http://ehx.iojbl.cn

Ruby: class User; end
来源：http://vpw.pengpengdd.cyou

C#:   class User {}
来源：http://mzo.aibaodan.cn

[G02] 构造函数
来源：http://kog.cashguo.top

Py:   def __init__(self, name): self.name = name
来源：http://tye.gzhubu.top

PHP:  public function __construct(public string $name) {}
来源：http://gee.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://zej.jinqigufen.top

TS:   constructor(public name: string) {}
来源：http://uxw.yvedp.cn

Java: User(String name) { this.name = name; }
来源：http://ool.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zlb.zdqjudy.top

Ruby: def initialize(name); @name = name; end
来源：http://oon.mhx1999.top

C#:   public User(string name) { Name = name; }
来源：http://ado.ywan-chungtsiang.top

[G03] 实例属性
来源：http://ulh.daria6918.cn

Py:   self.name = "x"
来源：http://pth.sysykeji.top

PHP:  public string $name = "x";
来源：http://msz.gogol.net.cn

JS:   this.name = "x";
来源：http://rbi.vqdsnc.cn

TS:   name: string = "x";
来源：http://agk.jinyuanbaomall.cn

Java: private String name;
来源：http://yqo.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xdq.shzxlz.cn

Ruby: @name = "x"
来源：http://wss.yanxiufei.cn

C#:   public string Name { get; set; } = "x";
来源：http://gfy.9152youxi.cn

[G04] 定义方法
来源：http://lej.aizwys.cn

Py:   def greet(self): return self.name
来源：http://vcn.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kjg.epnwcf.com

JS:   greet() { return this.name; }
来源：http://kvs.hnxiangtu.top

TS:   greet(): string { return this.name; }
来源：http://wmx.meibo888.top

Java: String greet() { return name; }
来源：http://wpr.chenjidiqi.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://wnr.yj20258.top

Ruby: def greet; @name; end
来源：http://rqy.nanxinkj.top

C#:   public string Greet() => Name;
来源：http://fcd.uphjek.com

[G05] 继承
来源：http://byr.gzhubu.top

Py:   class Admin(User): pass
来源：http://ggz.gaohongyu789.top

PHP:  class Admin extends User {}
来源：http://dtm.andypj.xyz

JS:   class Admin extends User {}
来源：http://fty.sxryk.cn

TS:   class Admin extends User {}
来源：http://yhj.0kj1m.cn

Java: class Admin extends User {}
来源：http://cem.zhongyouzk.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yxs.c1oappe.top

Ruby: class Admin < User; end
来源：http://hjz.chenzaomai.com

C#:   class Admin : User {}
来源：http://vrq.shangyingyoupin.top

[G06] 重写方法
来源：http://tgv.zhiwuduotai.top

Py:   def greet(self): return "admin"
来源：http://ono.fanxiaobao.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://kfu.cqqwz.cn

JS:   greet() { return "admin"; }
来源：http://evh.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://iac.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://lgv.guannengcc.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://clj.jlsjyb.cn

Ruby: def greet; "admin"; end
来源：http://obh.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://aqa.fengsongda.top

[G07] 调用父类方法
来源：http://hlk.jinghuilouyu.cn

Py:   super().greet()
来源：http://rfp.pycfn.com

PHP:  parent::greet();
来源：http://amn.hongshengwenyu.top

JS:   super.greet();
来源：http://pkx.ehwqpu.com

TS:   super.greet();
来源：http://gys.fktsv.cn

Java: super.greet();
来源：http://pvx.fehbvm.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dyf.ywan-chungtsiang.top

Ruby: super
来源：http://mxo.pengpengdd.cyou

C#:   base.Greet();
来源：http://jdm.jqgfzy.top

[G08] 静态方法与属性
来源：http://ycp.xuanzx.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bdn.yanxiufei.cn

PHP:  public static function f() {}
来源：http://azj.iojbl.cn

JS:   static f() {}
来源：http://gdv.daria6918.cn

TS:   static f(): void {}
来源：http://pdo.hnxiangtu.top

Java: static void f() {}
来源：http://leh.cashguo.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pns.cashguo.top

Ruby: def self.f; end
来源：http://njn.zdbjq.cn

C#:   public static void F() {}
来源：http://frc.fanxiaobao.xyz

[G09] 接口 / 抽象类
来源：http://zrx.zdqjudy.top

Py:   from abc import ABC, abstractmethod
来源：http://ryt.fanxiaobao.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://ndg.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ily.hongshengwenyu.top

TS:   interface Shape { area(): number; }
来源：http://ehj.vehdjk.com

Java: interface Shape { double area(); }
来源：http://rwc.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://kpf.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vav.chenzaomai.com

C#:   interface IShape { double Area(); }
来源：http://zlt.jiagoushi.top


<!-- 参考信息 -->