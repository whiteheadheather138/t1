代发 wailian999

Go:   strings.Count(s, "a")
来源：http://zhn.fktsv.cn

Ruby: s.count("a")
来源：http://lzr.aibaodan.cn

C#:   s.Count(c => c == 'a')
来源：http://xmt.bjfxy.top

[E13] 逐字符遍历
来源：http://cjo.vehdjk.com

Py:   for ch in s: print(ch)
来源：http://khw.birdmap.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rfs.fanxiaobao.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://xth.gogol.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hgq.cheryme.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hwe.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ilq.zhixingplan.top

Ruby: s.each_char { |ch| puts ch }
来源：http://uex.mhx1999.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qme.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://qzr.tarul.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zcl.zhongyouzk.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yac.cucudq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jlu.yangfankeji.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tdm.pengpengdd.cyou

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pkm.daria6918.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sen.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qsf.bbcook.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lol.gogol.net.cn

[E15] HTML 转义 / 反转义
来源：http://zyx.jqgfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ctj.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lkl.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uwr.yvedp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fos.hcnkem.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qag.jqgfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://drl.mhx1999.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bqt.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ekn.jinghuilouyu.cn

[E16] 数字千分位
来源：http://fqk.52xcode.cn

Py:   f"{1234567:,}"
来源：http://ywx.ppjwa.cn

PHP:  number_format(1234567);
来源：http://xco.0kj1m.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://muu.wangshuangyany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pmd.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sqm.shangyingyoupin.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ggp.iojbl.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wul.cdnleiting.top

C#:   1234567.ToString("N0")
来源：http://clg.yuxming.cn

[E17] 首字母大写
来源：http://vvo.gaohongyu789.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qxx.jinqigufen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cqe.quarkkingdee.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ubq.zdbjq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xpg.vqdsnc.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ioq.yonumen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wyb.yvedp.cn

Ruby: s.capitalize
来源：http://zoj.tanke756.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dnk.nwbrower.top

[E18] 模板占位符替换
来源：http://zdy.zhoulong.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hng.yuxming.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yan.hysaishi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tjv.vehdjk.com

TS:   tpl.replaceAll("{name}", name)
来源：http://mzd.yj20258.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zjx.fehbvm.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oai.xziqi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://htt.xingfuxueyuan.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xnm.aibaodan.cn

[E19] 多行文本按行拆分
来源：http://kqo.316326.xyz

Py:   s.splitlines()
来源：http://red.havefunace.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ctu.0kj1m.cn

JS:   s.split(/\r?\n/)
来源：http://qqa.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://gnx.quarkkingdee.top

Java: s.lines().toList()
来源：http://yst.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://thm.hcnkem.com

Ruby: s.lines
来源：http://ves.chenzaomai.com

C#:   s.Split('\n')
来源：http://ays.9152youxi.cn

[E20] 判断字符串是否为空
来源：http://olb.ppjwa.cn

Py:   if not s:
来源：http://lga.dashuyun.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://koe.gogol.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://odf.haohaochexian.top

TS:   if (s === "") {}
来源：http://bwo.iojbl.cn

Java: if (s.isEmpty()) {}
来源：http://kml.ppjwa.cn

Go:   if s == "" {}
来源：http://cmz.cashguo.top

Ruby: if s.empty?
来源：http://ccs.hywenlv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zes.zhoulong.xyz

[E21] 超长截断加省略号
来源：http://ayz.wangshuangyany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://msd.zhoulong.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pjt.sweek.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aha.yanxiufei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://caw.yfazqb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://amx.hammf.cn

Go:   // 按 rune 判断长度后截断
来源：http://opg.tanke756.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uhw.jinyuanbaomall.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dev.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://lhn.yangfankeji.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mcl.shanyushiyangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rke.jinyuanbaomall.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ppf.uphjek.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://clz.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://anj.cqqwz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fhq.jinghuilouyu.cn

Ruby: s.bytesize;  s.length
来源：http://qma.ehwqpu.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vio.hongshengwenyu.top

================================================================================
来源：http://ryr.vehdjk.com

F. 文件与目录
来源：http://gpg.pycfn.com

================================================================================
来源：http://xka.bbcook.cn

[F01] 读取整个文件
来源：http://gvt.hysaishi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://epu.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://ibz.havefunace.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ihx.nwbrower.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://efy.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://met.svipenyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kjf.jinqigufen.top

Ruby: File.read("a.txt")
来源：http://mgl.hammf.cn

C#:   File.ReadAllText("a.txt");
来源：http://vey.sxryk.cn

[F02] 逐行读取文件
来源：http://xcw.wangdashe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qng.nanxuanxn.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tsf.ydjk.org.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rdp.ivvv.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hyr.jlsjyb.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ptd.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sqr.fzhhl.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://evr.hcnkem.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://udf.nanxinkj.top

[F03] 写入文件（覆盖）
来源：http://tpq.xuetiantiany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dfj.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yac.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hcy.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ehi.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xvn.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gkh.jinqigufen.top

Ruby: File.write("a.txt", "hi")
来源：http://gsq.aibaodan.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://feg.tian-w.cn

[F04] 追加写入文件
来源：http://tos.sufxvd.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://njl.zhoulong.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nnr.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dul.zhaomingkeji.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cwy.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uut.sxryk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kra.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cxs.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kvd.zycfv.cn

[F05] 判断文件或目录是否存在
来源：http://wze.jqgufenzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mqk.chenjidiqi.icu

PHP:  file_exists("a.txt");
来源：http://clt.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://fzo.yfazqb.com

TS:   fs.existsSync("a.txt")
来源：http://xua.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kaq.yj20258888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ril.andypj.xyz

Ruby: File.exist?("a.txt")
来源：http://bao.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://tvk.mhx1999.top

[F06] 删除文件
来源：http://zwh.hesvh.cn

Py:   os.remove("a.txt")
来源：http://wux.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://clx.chenzaomai.com

JS:   fs.unlinkSync("a.txt")
来源：http://qyl.cucudq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tma.zhengqikj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tjn.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://fmh.hfpthk.cn

Ruby: File.delete("a.txt")
来源：http://jai.gaohongyu789.top

C#:   File.Delete("a.txt");
来源：http://zlk.dianchejie.cn

[F07] 创建目录（含多级）
来源：http://kun.zycfv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ttc.mhx1999.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kbl.bbcook.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://api.nanxinkj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ylr.yfazqb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://doc.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://noh.jlsjyb.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tdy.shanyushiyangtech.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hnx.ydjk.org.cn

[F08] 遍历目录
来源：http://bdl.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mpt.dashuyun.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bhu.hfpthk.cn

JS:   fs.readdirSync("dir")
来源：http://xel.birdmap.top

TS:   fs.readdirSync("dir")
来源：http://bic.daxiang520.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://eaj.jyoumei.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xnj.jinqigfzy.top

Ruby: Dir.children("dir")
来源：http://kez.zycfv.cn

C#:   Directory.GetFiles("dir")
来源：http://zlw.chenzaomai.com

[F09] 获取文件大小
来源：http://dpx.snrcjt.cn

Py:   os.path.getsize("a.txt")
来源：http://jjv.52xcode.cn

PHP:  filesize("a.txt");
来源：http://ucb.jinyuanbaomall.cn

JS:   fs.statSync("a.txt").size
来源：http://kui.yangfankeji.com

TS:   fs.statSync("a.txt").size
来源：http://ppf.wangdashe.top

Java: Files.size(Path.of("a.txt"))
来源：http://znn.zhixingplan.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rvz.yj20258.top

Ruby: File.size("a.txt")
来源：http://hdc.tianlin.xyz

C#:   new FileInfo("a.txt").Length
来源：http://egz.jlsjyb.cn

[F10] 取文件扩展名 / 文件名
来源：http://vml.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ujv.316326.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iyt.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ztm.chenzaomai.com

TS:   path.extname("a.txt")
来源：http://agt.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kvo.pengpengdd.cyou

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tqe.jianghu66.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://omd.smart0.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nyp.cdnleiting.top

[F11] 复制与移动文件
来源：http://fgd.wangshuangyany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dxk.sweek.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://atz.shanyushiyangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wsh.yangfankeji.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ufo.jianghu66.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dfh.cashguo.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oyg.yj202588.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bvu.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lhu.jyoumei.cn

[F12] CSV 读写
来源：http://xof.zhixingplan.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wrf.vehdjk.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ges.hammf.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jlp.hongshengwenyu.top

TS:   // 同上
来源：http://jex.zhongyouzk.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xsd.xziqi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vom.xinyue.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://grb.tian-w.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ypa.hcnkem.com

================================================================================
来源：http://ntd.guowangkeji.top

G. 面向对象
来源：http://rcm.zhaomingkeji.xyz

================================================================================
来源：http://fxf.tian-w.cn

[G01] 定义类
来源：http://tfp.jinyuanbaomall.cn

Py:   class User: pass
来源：http://fav.aizwys.cn

PHP:  class User {}
来源：http://ncj.chenzaomai.com

JS:   class User {}
来源：http://bnh.epnwcf.com

TS:   class User { name: string = ""; }
来源：http://qas.ybcxt.top

Java: class User {}
来源：http://avo.yanxiufei.cn

Go:   type User struct { Name string }
来源：http://bxb.birdmap.top

Ruby: class User; end
来源：http://rek.fehbvm.com

C#:   class User {}
来源：http://guh.tianlin.xyz

[G02] 构造函数
来源：http://lbv.xziqi.cn

Py:   def __init__(self, name): self.name = name
来源：http://smc.jyoumei.cn

PHP:  public function __construct(public string $name) {}
来源：http://wpl.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://cox.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://koq.yuanzhike.top

Java: User(String name) { this.name = name; }
来源：http://rje.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qav.yuanzhike.top

Ruby: def initialize(name); @name = name; end
来源：http://czy.havefunace.top

C#:   public User(string name) { Name = name; }
来源：http://rcl.ehwqpu.com

[G03] 实例属性
来源：http://gtc.jianghu66.top

Py:   self.name = "x"
来源：http://tkd.ivvv.top

PHP:  public string $name = "x";
来源：http://nia.mhx1999.top

JS:   this.name = "x";
来源：http://fxn.xingfuxueyuan.xyz

TS:   name: string = "x";
来源：http://sim.sysykeji.top

Java: private String name;
来源：http://frn.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://joa.xuanzx.com

Ruby: @name = "x"
来源：http://qsi.feifeiyinyue.top

C#:   public string Name { get; set; } = "x";
来源：http://bfh.9152youxi.cn

[G04] 定义方法
来源：http://oie.c1oappe.top

Py:   def greet(self): return self.name
来源：http://vds.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://svh.shzxlz.cn

JS:   greet() { return this.name; }
来源：http://vok.jiagoushi.top

TS:   greet(): string { return this.name; }
来源：http://xph.hnqzz.top

Java: String greet() { return name; }
来源：http://xls.c1oappe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vqk.hnqzz.top

Ruby: def greet; @name; end
来源：http://sjq.shangyingyoupin.top

C#:   public string Greet() => Name;
来源：http://xhu.hcnkem.com

[G05] 继承
来源：http://rlm.pengpengdd.cyou

Py:   class Admin(User): pass
来源：http://uit.aibaodan.cn

PHP:  class Admin extends User {}
来源：http://ruj.shzxlz.cn

JS:   class Admin extends User {}
来源：http://txs.guannengcc.top

TS:   class Admin extends User {}
来源：http://jml.316326.xyz

Java: class Admin extends User {}
来源：http://doc.zhiwuduotai.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tzh.havefunace.top

Ruby: class Admin < User; end
来源：http://pxt.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://tne.quarkkingdee.top

[G06] 重写方法
来源：http://akn.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://vzj.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nqo.jinghuilouyu.cn

JS:   greet() { return "admin"; }
来源：http://kmj.yongpay.top

TS:   greet(): string { return "admin"; }
来源：http://mat.shanyushiyangtech.top

Java: @Override String greet() { return "admin"; }
来源：http://tok.nwbrower.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xmv.yj202588.top

Ruby: def greet; "admin"; end
来源：http://wef.hcnkem.com

C#:   public override string Greet() => "admin";
来源：http://yxp.xuanzx.com

[G07] 调用父类方法
来源：http://pnr.jqgfzy.top

Py:   super().greet()
来源：http://thz.jinyuanbaomall.cn

PHP:  parent::greet();
来源：http://oej.0kj1m.cn

JS:   super.greet();
来源：http://ihw.ivvv.top

TS:   super.greet();
来源：http://iha.jlsjyb.cn

Java: super.greet();
来源：http://qoi.sweek.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vde.ydjk.org.cn

Ruby: super
来源：http://oob.xinyue.icu

C#:   base.Greet();
来源：http://pgc.tian-w.cn

[G08] 静态方法与属性
来源：http://rvq.tarul.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zch.hfpthk.cn

PHP:  public static function f() {}
来源：http://xdx.ywan-chungtsiang.top

JS:   static f() {}
来源：http://gcf.shanyushiyangtech.top

TS:   static f(): void {}
来源：http://pgo.jianghu66.top

Java: static void f() {}
来源：http://jfo.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://cmb.cheryme.top

Ruby: def self.f; end
来源：http://ofw.zycfv.cn

C#:   public static void F() {}
来源：http://sba.hesvh.cn

[G09] 接口 / 抽象类
来源：http://esm.yuxming.cn

Py:   from abc import ABC, abstractmethod
来源：http://mfk.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xpk.xingfuxueyuan.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://lcu.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://opm.fanxiaobao.xyz

Java: interface Shape { double area(); }
来源：http://zio.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://xun.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yib.hfpthk.cn

C#:   interface IShape { double Area(); }
来源：http://dtn.jqgfzy.top

[G10] 访问控制
来源：http://aql.xingfuxueyuan.xyz

Py:   约定 _protected / __private（不强制）
来源：http://foj.yuxming.cn

PHP:  public / protected / private
来源：http://jjj.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://cwd.yj20258.top

TS:   public / protected / private
来源：http://out.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://ouz.yonumen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fxj.0kj1m.cn

Ruby: public / protected / private
来源：http://egj.ydzc1.top

C#:   public / protected / private / internal
来源：http://jzz.fktsv.cn

[G11] getter / setter
来源：http://dwz.316326.xyz

Py:   @property 与 @x.setter
来源：http://qcu.kuanghao11.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dlo.nwbrower.top


<!-- 参考信息 -->