代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bqu.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://waw.ppjwa.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://shn.iojbl.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eun.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gfq.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hyi.shanyushiyangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://waj.jlsjyb.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kjr.dashuyun.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dqb.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wmt.meibo888.top

[E16] 数字千分位
来源：http://lwa.gotoacloud.top

Py:   f"{1234567:,}"
来源：http://ugd.jinqigufen.top

PHP:  number_format(1234567);
来源：http://ogs.xingfuxueyuan.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://aue.sysykeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qvv.zdqjudy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wtb.ctjpmb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pkx.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ctl.ydjk.org.cn

C#:   1234567.ToString("N0")
来源：http://qzx.chenjidiqi.icu

[E17] 首字母大写
来源：http://frl.zdqjudy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rhx.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://icw.ctjpmb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://twv.tarul.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ezb.guannengcc.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nlq.yj20258888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vho.hfpthk.cn

Ruby: s.capitalize
来源：http://bha.pycfn.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jen.fengsongda.top

[E18] 模板占位符替换
来源：http://unh.hnqzz.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wkk.jinyuanbaomall.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ukv.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tpt.hammf.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lxl.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tea.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://paj.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jue.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://otl.nanxuanxn.top

[E19] 多行文本按行拆分
来源：http://say.chenzaomai.com

Py:   s.splitlines()
来源：http://vis.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hpk.ydjk.org.cn

JS:   s.split(/\r?\n/)
来源：http://rib.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://dte.wangdashe.top

Java: s.lines().toList()
来源：http://kwf.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://mez.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://cqd.zdqjudy.top

C#:   s.Split('\n')
来源：http://mrn.ydjk.org.cn

[E20] 判断字符串是否为空
来源：http://tij.wangdashe.top

Py:   if not s:
来源：http://hwd.gaohongyu789.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ctt.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zfh.nwbrower.top

TS:   if (s === "") {}
来源：http://cnm.jqgfzy.top

Java: if (s.isEmpty()) {}
来源：http://avk.52xcode.cn

Go:   if s == "" {}
来源：http://zvq.jlsjyb.cn

Ruby: if s.empty?
来源：http://rfd.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kgt.guowangkeji.top

[E21] 超长截断加省略号
来源：http://cko.guannengcc.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hze.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://srf.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mkm.zhengqikj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://afc.zhijiandao.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aej.fktsv.cn

Go:   // 按 rune 判断长度后截断
来源：http://ghc.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ciz.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rdg.zhongyouzk.top

[E22] 字节长度与字符长度
来源：http://mnk.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qrr.sxryk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qpb.cheryme.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://orc.fzhhl.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bub.zhengqikj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gxv.pengpengdd.cyou

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tla.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://fqk.zhaomingkeji.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fog.sysykeji.top

================================================================================
来源：http://jvi.wangdashe.top

F. 文件与目录
来源：http://fym.xylfe.cn

================================================================================
来源：http://voh.jqgufenzy.top

[F01] 读取整个文件
来源：http://tyd.jqgfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fte.uphjek.com

PHP:  file_get_contents("a.txt");
来源：http://fij.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sin.fengsongda.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ppa.havefunace.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xbx.yanxiufei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kwa.xinyue.icu

Ruby: File.read("a.txt")
来源：http://krg.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://bvo.hammf.cn

[F02] 逐行读取文件
来源：http://fhl.ydjk.org.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://veb.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://reg.pengpengdd.cyou

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ouh.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jfo.jinqigufen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ago.ctjpmb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pzk.zycfv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eco.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sji.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://cae.vehdjk.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qtg.yj20258.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://oxb.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jtj.svipenyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ljt.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gjx.shanyushiyangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fla.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://fzm.hcnkem.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qrl.ywan-chungtsiang.top

[F04] 追加写入文件
来源：http://bcg.yj20258.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mtb.yuxming.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mpj.tarul.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zik.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wot.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xih.jqgfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hvt.shanyushiyangtech.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pea.sufxvd.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uvb.jinqigfzy.top

[F05] 判断文件或目录是否存在
来源：http://mnt.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iap.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://bej.dianchejie.cn

JS:   fs.existsSync("a.txt")
来源：http://zxb.daxiang520.top

TS:   fs.existsSync("a.txt")
来源：http://pmr.xylfe.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hdb.epnwcf.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cpr.cdnleiting.top

Ruby: File.exist?("a.txt")
来源：http://wgq.guowangkeji.top

C#:   File.Exists("a.txt")
来源：http://bby.zhengqikj.top

[F06] 删除文件
来源：http://kgf.yonumen.top

Py:   os.remove("a.txt")
来源：http://xis.ivvv.top

PHP:  unlink("a.txt");
来源：http://hsh.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://ejq.fengsongda.top

TS:   fs.unlinkSync("a.txt")
来源：http://tyh.fzhhl.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oxu.nanxuanxn.top

Go:   os.Remove("a.txt")
来源：http://xdq.jinqigfzy.top

Ruby: File.delete("a.txt")
来源：http://guv.zhoulong.xyz

C#:   File.Delete("a.txt");
来源：http://bmw.ywan-chungtsiang.top

[F07] 创建目录（含多级）
来源：http://szo.zhongyouzk.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ule.cashguo.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://msu.hcnkem.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tae.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://psf.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kxa.dianchejie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://otv.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tpw.hnqzz.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uvn.gzhubu.top

[F08] 遍历目录
来源：http://ngb.yuxming.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rbk.sjlbkw.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cfa.chenlongwang.top

JS:   fs.readdirSync("dir")
来源：http://uxv.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://fmi.xylfe.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aub.xuetiantiany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zdo.zhoulong.xyz

Ruby: Dir.children("dir")
来源：http://bcc.dashuyun.cn

C#:   Directory.GetFiles("dir")
来源：http://vet.shanyushiyangkeji.top

[F09] 获取文件大小
来源：http://rnr.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://hev.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://obo.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://zkr.xuanzx.com

TS:   fs.statSync("a.txt").size
来源：http://oml.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nmu.zhaomingkeji.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zhx.zdqjudy.top

Ruby: File.size("a.txt")
来源：http://ace.sufxvd.cn

C#:   new FileInfo("a.txt").Length
来源：http://yvg.vehdjk.com

[F10] 取文件扩展名 / 文件名
来源：http://cmc.ydzc1.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fin.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ipq.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bhg.meibo888.top

TS:   path.extname("a.txt")
来源：http://ujh.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rmo.hywenlv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://koi.dianchejie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://elp.gogol.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://okn.316326.xyz

[F11] 复制与移动文件
来源：http://rny.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ymj.52xcode.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bcd.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tgt.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fry.bjfxy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nkm.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dul.feifeiyinyue.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vnl.ehwqpu.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hei.jqgfzy.top

[F12] CSV 读写
来源：http://uzx.chenzaomai.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vls.zhixingplan.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://swg.yfazqb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ldu.fzhhl.top

TS:   // 同上
来源：http://bzf.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bxx.yj20258888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://woz.yj20258.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wxf.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://fkd.zhijiandao.cn

================================================================================
来源：http://hgc.ivvv.top

G. 面向对象
来源：http://ipd.xuetiantiany.cn

================================================================================
来源：http://kst.havefunace.top

[G01] 定义类
来源：http://ysr.aibaodan.cn

Py:   class User: pass
来源：http://oek.mhx1999.top

PHP:  class User {}
来源：http://rhc.yvedp.cn

JS:   class User {}
来源：http://lmj.cqqwz.cn

TS:   class User { name: string = ""; }
来源：http://wgt.guowangkeji.top

Java: class User {}
来源：http://wek.52xcode.cn

Go:   type User struct { Name string }
来源：http://zby.feifeiyinyue.top

Ruby: class User; end
来源：http://ori.52xcode.cn

C#:   class User {}
来源：http://uwk.tianlin.xyz

[G02] 构造函数
来源：http://edg.cucudq.cn

Py:   def __init__(self, name): self.name = name
来源：http://jvs.jinyuanbaomall.cn

PHP:  public function __construct(public string $name) {}
来源：http://gnz.andypj.xyz

JS:   constructor(name) { this.name = name; }
来源：http://ytq.cashguo.top

TS:   constructor(public name: string) {}
来源：http://wkr.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://chl.yj20258.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://duw.bbcook.cn

Ruby: def initialize(name); @name = name; end
来源：http://mlp.cdnleiting.top

C#:   public User(string name) { Name = name; }
来源：http://sxq.yanxiufei.cn

[G03] 实例属性
来源：http://sew.yj202588.top

Py:   self.name = "x"
来源：http://zwq.yj20258.top

PHP:  public string $name = "x";
来源：http://cnu.cucudq.cn

JS:   this.name = "x";
来源：http://yby.yangfankeji.com

TS:   name: string = "x";
来源：http://mtl.fktsv.cn

Java: private String name;
来源：http://yqn.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://stx.pycfn.com

Ruby: @name = "x"
来源：http://vdx.epnwcf.com

C#:   public string Name { get; set; } = "x";
来源：http://ggd.jianghu66.top

[G04] 定义方法
来源：http://dgn.nwbrower.top

Py:   def greet(self): return self.name
来源：http://fxk.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://edf.yongpay.top

JS:   greet() { return this.name; }
来源：http://wrc.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://xmp.redwolf501.top

Java: String greet() { return name; }
来源：http://jer.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xcx.jianghu66.top

Ruby: def greet; @name; end
来源：http://pjm.xziqi.cn

C#:   public string Greet() => Name;
来源：http://rod.guannengcc.top

[G05] 继承
来源：http://qst.cucudq.cn

Py:   class Admin(User): pass
来源：http://vov.fzhhl.top

PHP:  class Admin extends User {}
来源：http://wfd.xinyue.icu

JS:   class Admin extends User {}
来源：http://mpi.sufxvd.cn

TS:   class Admin extends User {}
来源：http://cos.feifeiyinyue.top

Java: class Admin extends User {}
来源：http://moj.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://txf.jinqigfzy.top

Ruby: class Admin < User; end
来源：http://aka.fengsongda.top

C#:   class Admin : User {}
来源：http://ntj.ivvv.top

[G06] 重写方法
来源：http://onj.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://fmm.uphjek.com

PHP:  public function greet(): string { return "admin"; }
来源：http://blg.yueranfly.top

JS:   greet() { return "admin"; }
来源：http://ifi.quarkkingdee.top

TS:   greet(): string { return "admin"; }
来源：http://osd.cqqwz.cn

Java: @Override String greet() { return "admin"; }
来源：http://nlh.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xqb.sjlbkw.cn

Ruby: def greet; "admin"; end
来源：http://run.meibo888.top

C#:   public override string Greet() => "admin";
来源：http://jen.yj20258.top

[G07] 调用父类方法
来源：http://wtl.hcnkem.com

Py:   super().greet()
来源：http://ajs.gaohongyu789.top

PHP:  parent::greet();
来源：http://icn.jinghuilouyu.cn

JS:   super.greet();
来源：http://eza.fanxiaobao.xyz

TS:   super.greet();
来源：http://rfz.kuanghao11.cn

Java: super.greet();
来源：http://kkm.mhx1999.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aub.52xcode.cn

Ruby: super
来源：http://gwy.pengpengdd.cyou

C#:   base.Greet();
来源：http://jib.epnwcf.com

[G08] 静态方法与属性
来源：http://lwt.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tqx.vehdjk.com

PHP:  public static function f() {}
来源：http://hnf.pengpengdd.cyou

JS:   static f() {}
来源：http://xqu.316326.xyz

TS:   static f(): void {}
来源：http://dib.yj20258.top

Java: static void f() {}
来源：http://hiz.tian-w.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://irp.hnqzz.top

Ruby: def self.f; end
来源：http://isi.jinqigfzy.top

C#:   public static void F() {}
来源：http://lqv.aibaodan.cn

[G09] 接口 / 抽象类
来源：http://biz.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://vwn.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://gqk.aizwys.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tma.ehwqpu.com

TS:   interface Shape { area(): number; }
来源：http://iog.xylfe.cn

Java: interface Shape { double area(); }
来源：http://izz.tianlin.xyz

Go:   type Shape interface { Area() float64 }
来源：http://xum.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zlk.jianghu66.top

C#:   interface IShape { double Area(); }
来源：http://efz.daria6918.cn

[G10] 访问控制
来源：http://mud.xuetiantiany.cn

Py:   约定 _protected / __private（不强制）
来源：http://pbb.yvedp.cn

PHP:  public / protected / private
来源：http://bmw.tian-w.cn

JS:   #private 字段；其余公开
来源：http://nkz.zhijiandao.cn

TS:   public / protected / private
来源：http://hmw.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://wxi.tianlin.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://ire.ehwqpu.com

Ruby: public / protected / private
来源：http://rzj.ydzc1.top

C#:   public / protected / private / internal
来源：http://jwp.iojbl.cn

[G11] getter / setter
来源：http://feg.cheryme.top

Py:   @property 与 @x.setter
来源：http://nur.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://qoy.jlsjyb.cn

JS:   get name() { return this._name; }
来源：http://riq.vehdjk.com

TS:   get name(): string { return this._name; }
来源：http://jpa.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://tmd.jinghuilouyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jbz.tanke756.top

Ruby: attr_accessor :name
来源：http://ryk.xuanzx.com

C#:   public string Name { get; set; }
来源：http://ali.yj20258.top

[G12] 对象转字符串
来源：http://tnj.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://pen.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ezu.tanke756.top

JS:   toString() { return this.name; }
来源：http://kwy.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://vss.yj202588.top

Java: @Override public String toString() { return name; }
来源：http://puo.sufxvd.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xuy.gotoacloud.top

Ruby: def to_s; @name; end
来源：http://fgf.uphjek.com

C#:   public override string ToString() => Name;
来源：http://nlt.yj20258.top

[G13] 判断对象类型
来源：http://yds.bjfxy.top

Py:   isinstance(u, User)
来源：http://nox.cqqwz.cn

PHP:  $u instanceof User
来源：http://lfv.ctjpmb.com

JS:   u instanceof User
来源：http://ank.ydjk.org.cn

TS:   u instanceof User
来源：http://nks.hongshengwenyu.top


<!-- 参考信息 -->