代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rhr.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uxb.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hzo.birdmap.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://itt.sxryk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://azp.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://roo.xuetiantiany.cn

[E16] 数字千分位
来源：http://cyh.shangyingyoupin.top

Py:   f"{1234567:,}"
来源：http://tgb.feifeiyinyue.top

PHP:  number_format(1234567);
来源：http://hhe.zhijiandao.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qnw.guowangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://dhg.sufxvd.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://miz.cashguo.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xdy.c1oappe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ucp.xuetiantiany.cn

C#:   1234567.ToString("N0")
来源：http://xha.jlsjyb.cn

[E17] 首字母大写
来源：http://gie.tanke756.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dgq.bbcook.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jzu.fehbvm.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kau.ybcxt.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xym.smart0.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wfq.yueranfly.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ola.sysykeji.top

Ruby: s.capitalize
来源：http://vjj.shanyushiyangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vdh.0kj1m.cn

[E18] 模板占位符替换
来源：http://fyz.xuanzx.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://prn.jinghuilouyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jtz.chenjidiqi.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://jdt.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dim.yangfankeji.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zmq.zycfv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jtc.zhongyouzk.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vka.zdbjq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eta.sufxvd.cn

[E19] 多行文本按行拆分
来源：http://gdy.yuanzhike.top

Py:   s.splitlines()
来源：http://pfj.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rfm.shuidangran.top

JS:   s.split(/\r?\n/)
来源：http://xem.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://taz.0kj1m.cn

Java: s.lines().toList()
来源：http://lvk.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://lgk.hcnkem.com

Ruby: s.lines
来源：http://zfd.guowangkeji.top

C#:   s.Split('\n')
来源：http://rro.meibo888.top

[E20] 判断字符串是否为空
来源：http://teh.jyoumei.cn

Py:   if not s:
来源：http://qwr.zhixingplan.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://red.hongshengwenyu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://slq.hcnkem.com

TS:   if (s === "") {}
来源：http://qsf.guowangkeji.top

Java: if (s.isEmpty()) {}
来源：http://dur.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://irf.zycfv.cn

Ruby: if s.empty?
来源：http://zwv.chenzaomai.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cif.hcnkem.com

[E21] 超长截断加省略号
来源：http://yav.zhixingplan.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://piq.aizwys.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jdo.chenlongwang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iti.daxiang520.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lhq.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nkd.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://wjt.jinqigufen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mdm.jlsjyb.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hra.epnwcf.com

[E22] 字节长度与字符长度
来源：http://rkg.ybcxt.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jkh.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tnm.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://olj.fanxiaobao.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://thf.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ilq.xylfe.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vke.xingfuxueyuan.xyz

Ruby: s.bytesize;  s.length
来源：http://xxa.hysaishi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wsd.epnwcf.com

================================================================================
来源：http://ngh.ivvv.top

F. 文件与目录
来源：http://mco.c1oappe.top

================================================================================
来源：http://tvo.uphjek.com

[F01] 读取整个文件
来源：http://jwy.sweek.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://atl.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://uyk.ywan-chungtsiang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xoq.redwolf501.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kcl.yvedp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hkr.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gtr.tanke756.top

Ruby: File.read("a.txt")
来源：http://kji.redwolf501.top

C#:   File.ReadAllText("a.txt");
来源：http://uga.quarkkingdee.top

[F02] 逐行读取文件
来源：http://nku.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://evj.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jft.yj20258888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cnj.yj20258.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xuj.jqgufenzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ghk.dianchejie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yzf.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jpg.fanxiaobao.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zjq.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://uxz.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jnx.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://ezb.316326.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qii.zhaomingkeji.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zsj.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iox.ywan-chungtsiang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rqk.pengpengdd.cyou

Ruby: File.write("a.txt", "hi")
来源：http://lig.sysykeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tkf.yueranfly.top

[F04] 追加写入文件
来源：http://lgz.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jrb.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://peq.cdnleiting.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jld.hcnkem.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wzf.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ghf.shuidangran.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jdx.yvedp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wdj.epnwcf.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://etd.kuanghao11.cn

[F05] 判断文件或目录是否存在
来源：http://mot.hesvh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hef.yj20258888.top

PHP:  file_exists("a.txt");
来源：http://fhs.hysaishi.cn

JS:   fs.existsSync("a.txt")
来源：http://bfx.hfpthk.cn

TS:   fs.existsSync("a.txt")
来源：http://oid.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://xdp.zdqjudy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://caz.fehbvm.com

Ruby: File.exist?("a.txt")
来源：http://ubu.shanyushiyangtech.top

C#:   File.Exists("a.txt")
来源：http://vfl.cucudq.cn

[F06] 删除文件
来源：http://pdt.havefunace.top

Py:   os.remove("a.txt")
来源：http://yte.0kj1m.cn

PHP:  unlink("a.txt");
来源：http://xcl.wangdashe.top

JS:   fs.unlinkSync("a.txt")
来源：http://wbr.9152youxi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://him.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hfg.yangfankeji.com

Go:   os.Remove("a.txt")
来源：http://iyg.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://dnz.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://gzc.hongshengwenyu.top

[F07] 创建目录（含多级）
来源：http://pic.cashguo.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jwh.yanxiufei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ruq.hongshengwenyu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hzy.iojbl.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kub.yj20258888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sjk.zhongyouzk.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mzn.yvedp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uif.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zal.fzhhl.top

[F08] 遍历目录
来源：http://kjy.yuanzhike.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pmb.yonumen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wgd.hongshengwenyu.top

JS:   fs.readdirSync("dir")
来源：http://hhz.hysaishi.cn

TS:   fs.readdirSync("dir")
来源：http://evq.tian-w.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jee.xziqi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mtb.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://cpm.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://xzy.hywenlv.cn

[F09] 获取文件大小
来源：http://xrh.aizwys.cn

Py:   os.path.getsize("a.txt")
来源：http://tev.zhixingplan.top

PHP:  filesize("a.txt");
来源：http://anr.gaohongyu789.top

JS:   fs.statSync("a.txt").size
来源：http://hpj.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://xmh.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://cwc.zdqjudy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lyg.xinyue.icu

Ruby: File.size("a.txt")
来源：http://spc.yj20258888.top

C#:   new FileInfo("a.txt").Length
来源：http://yxi.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://yvy.redwolf501.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://elp.ydzc1.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nlr.birdmap.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lhx.cucudq.cn

TS:   path.extname("a.txt")
来源：http://dnq.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hhk.vehdjk.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vtw.yj202588.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vnc.yuxming.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gvs.redwolf501.top

[F11] 复制与移动文件
来源：http://dvp.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vji.tianlin.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://msc.hfpthk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://abk.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dih.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sup.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oht.ctjpmb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://htp.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zsy.cqqwz.cn

[F12] CSV 读写
来源：http://tcy.hysaishi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://can.tianlin.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ixq.pycfn.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rhw.hesvh.cn

TS:   // 同上
来源：http://xrg.sweek.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iwh.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yvx.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ega.vqdsnc.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pyw.feifeiyinyue.top

================================================================================
来源：http://qiy.yuxming.cn

G. 面向对象
来源：http://igm.52xcode.cn

================================================================================
来源：http://toq.mhx1999.top

[G01] 定义类
来源：http://ocr.xinyue.icu

Py:   class User: pass
来源：http://dop.hongshengwenyu.top

PHP:  class User {}
来源：http://xte.zhengqikj.top

JS:   class User {}
来源：http://nrl.hongshengwenyu.top

TS:   class User { name: string = ""; }
来源：http://asb.c1oappe.top

Java: class User {}
来源：http://lps.yuxming.cn

Go:   type User struct { Name string }
来源：http://abb.pengpengdd.cyou

Ruby: class User; end
来源：http://yye.svipenyu.cn

C#:   class User {}
来源：http://kiz.hammf.cn

[G02] 构造函数
来源：http://guj.xinyue.icu

Py:   def __init__(self, name): self.name = name
来源：http://yqn.xuanzx.com

PHP:  public function __construct(public string $name) {}
来源：http://pgi.pengpengdd.cyou

JS:   constructor(name) { this.name = name; }
来源：http://ptf.birdmap.top

TS:   constructor(public name: string) {}
来源：http://ztu.andypj.xyz

Java: User(String name) { this.name = name; }
来源：http://nwe.haohaochexian.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ppd.yonumen.top

Ruby: def initialize(name); @name = name; end
来源：http://xkz.nanxuanxn.top

C#:   public User(string name) { Name = name; }
来源：http://afk.bbcook.cn

[G03] 实例属性
来源：http://bcu.quarkkingdee.top

Py:   self.name = "x"
来源：http://elb.svipenyu.cn

PHP:  public string $name = "x";
来源：http://vqa.birdmap.top

JS:   this.name = "x";
来源：http://kxz.zdqjudy.top

TS:   name: string = "x";
来源：http://lme.bjfxy.top

Java: private String name;
来源：http://wdn.tian-w.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vds.fktsv.cn

Ruby: @name = "x"
来源：http://npm.jlsjyb.cn

C#:   public string Name { get; set; } = "x";
来源：http://aqg.gogol.net.cn

[G04] 定义方法
来源：http://vgx.yuxming.cn

Py:   def greet(self): return self.name
来源：http://xyy.shanyushiyangtech.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qkk.hysaishi.cn

JS:   greet() { return this.name; }
来源：http://soz.9152youxi.cn

TS:   greet(): string { return this.name; }
来源：http://doy.hfpthk.cn

Java: String greet() { return name; }
来源：http://dur.9152youxi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tpz.hywenlv.cn

Ruby: def greet; @name; end
来源：http://nut.havefunace.top

C#:   public string Greet() => Name;
来源：http://ybf.pycfn.com

[G05] 继承
来源：http://mvg.daxiang520.top

Py:   class Admin(User): pass
来源：http://uwn.hesvh.cn

PHP:  class Admin extends User {}
来源：http://cgf.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://xft.hammf.cn

TS:   class Admin extends User {}
来源：http://aru.wangdashe.top

Java: class Admin extends User {}
来源：http://ick.andypj.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://srk.dashuyun.cn

Ruby: class Admin < User; end
来源：http://rwx.sweek.top

C#:   class Admin : User {}
来源：http://onr.zhaomingkeji.xyz

[G06] 重写方法
来源：http://njg.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://ivz.fengsongda.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pig.dianchejie.cn

JS:   greet() { return "admin"; }
来源：http://rpw.zdbjq.cn

TS:   greet(): string { return "admin"; }
来源：http://qzq.9152youxi.cn

Java: @Override String greet() { return "admin"; }
来源：http://vkd.vehdjk.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://crj.ywan-chungtsiang.top

Ruby: def greet; "admin"; end
来源：http://gfv.yuxming.cn

C#:   public override string Greet() => "admin";
来源：http://qws.zhijiandao.cn

[G07] 调用父类方法
来源：http://fvw.xuanzx.com

Py:   super().greet()
来源：http://oed.yonumen.top

PHP:  parent::greet();
来源：http://mkb.xingfuxueyuan.xyz

JS:   super.greet();
来源：http://ayt.epnwcf.com

TS:   super.greet();
来源：http://owh.snrcjt.cn

Java: super.greet();
来源：http://jsx.xuanzx.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eom.316326.xyz

Ruby: super
来源：http://qpd.ydjk.org.cn

C#:   base.Greet();
来源：http://xwl.iojbl.cn

[G08] 静态方法与属性
来源：http://wac.ydzc1.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lut.xylfe.cn

PHP:  public static function f() {}
来源：http://cae.mhx1999.top

JS:   static f() {}
来源：http://ujb.yanxiufei.cn

TS:   static f(): void {}
来源：http://tpl.yj20258888.top

Java: static void f() {}
来源：http://woj.ppjwa.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bzq.yuanzhike.top

Ruby: def self.f; end
来源：http://wng.xingfuxueyuan.xyz

C#:   public static void F() {}
来源：http://pne.yj20258888.top

[G09] 接口 / 抽象类
来源：http://jhx.aibaodan.cn

Py:   from abc import ABC, abstractmethod
来源：http://zew.hfpthk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ymk.jqgfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ads.shanyushiyangkeji.top

TS:   interface Shape { area(): number; }
来源：http://hhu.fzhhl.top

Java: interface Shape { double area(); }
来源：http://juf.yuanzhike.top

Go:   type Shape interface { Area() float64 }
来源：http://nju.zdbjq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xnw.andypj.xyz

C#:   interface IShape { double Area(); }
来源：http://ufb.c1oappe.top

[G10] 访问控制
来源：http://kkb.c1oappe.top

Py:   约定 _protected / __private（不强制）
来源：http://uaf.ydzc1.top

PHP:  public / protected / private
来源：http://veg.yuxming.cn

JS:   #private 字段；其余公开
来源：http://wia.gotoacloud.top

TS:   public / protected / private
来源：http://vav.tianlin.xyz

Java: public / protected / private / 默认包级
来源：http://ozd.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rfi.cqqwz.cn

Ruby: public / protected / private
来源：http://fob.shzxlz.cn

C#:   public / protected / private / internal
来源：http://kdv.svipenyu.cn

[G11] getter / setter
来源：http://qrn.svipenyu.cn

Py:   @property 与 @x.setter
来源：http://lkw.yvedp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vkv.tarul.cn

JS:   get name() { return this._name; }
来源：http://mat.zdbjq.cn

TS:   get name(): string { return this._name; }
来源：http://zxw.jiagoushi.top

Java: public String getName() { return name; }
来源：http://lsa.sjlbkw.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jil.bbcook.cn

Ruby: attr_accessor :name
来源：http://pzd.yj202588.top

C#:   public string Name { get; set; }
来源：http://mme.jinyuanbaomall.cn

[G12] 对象转字符串
来源：http://fvf.tanke756.top

Py:   def __str__(self): return self.name
来源：http://fwj.dianchejie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pum.fanxiaobao.xyz

JS:   toString() { return this.name; }
来源：http://qne.hesvh.cn

TS:   toString(): string { return this.name; }
来源：http://grk.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://zkj.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://xmb.sufxvd.cn

Ruby: def to_s; @name; end
来源：http://utm.cucudq.cn

C#:   public override string ToString() => Name;
来源：http://ntl.gogol.net.cn

[G13] 判断对象类型
来源：http://nxe.sufxvd.cn

Py:   isinstance(u, User)
来源：http://ydd.fengsongda.top

PHP:  $u instanceof User
来源：http://tvh.vqdsnc.cn

JS:   u instanceof User
来源：http://web.ivvv.top

TS:   u instanceof User
来源：http://hzk.hammf.cn

Java: u instanceof User
来源：http://bkb.fengsongda.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gsc.shanyushiyangkeji.top

Ruby: u.is_a?(User)
来源：http://hne.fanxiaobao.xyz

C#:   u is User
来源：http://sej.daria6918.cn


<!-- 参考信息 -->