代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xwv.316326.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://apc.jyoumei.cn

[E16] 数字千分位
来源：http://zeu.aibaodan.cn

Py:   f"{1234567:,}"
来源：http://zyx.shzxlz.cn

PHP:  number_format(1234567);
来源：http://ddc.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fdi.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qdp.pengpengdd.cyou

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iaj.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ehz.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://znl.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://erx.guannengcc.top

[E17] 首字母大写
来源：http://fqv.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bnv.birdmap.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://aps.snrcjt.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pzs.havefunace.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ikb.hywenlv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zeh.yj20258.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jpu.birdmap.top

Ruby: s.capitalize
来源：http://gnn.cqqwz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vze.sxryk.cn

[E18] 模板占位符替换
来源：http://txe.wangshuangyany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dkk.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ruj.hongshengwenyu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://acv.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ynv.wangdashe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://six.hfpthk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://adz.cqqwz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zif.sweek.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uuz.svipenyu.cn

[E19] 多行文本按行拆分
来源：http://ppu.jqgufenzy.top

Py:   s.splitlines()
来源：http://gdr.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bjm.xylfe.cn

JS:   s.split(/\r?\n/)
来源：http://iaq.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://pmy.fzhhl.top

Java: s.lines().toList()
来源：http://egf.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://qtu.jinqigfzy.top

Ruby: s.lines
来源：http://mvt.dashuyun.cn

C#:   s.Split('\n')
来源：http://qrs.shanyushiyangtech.top

[E20] 判断字符串是否为空
来源：http://ibo.hnqzz.top

Py:   if not s:
来源：http://rxh.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kuh.iojbl.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rqj.xylfe.cn

TS:   if (s === "") {}
来源：http://dzp.ydjk.org.cn

Java: if (s.isEmpty()) {}
来源：http://ywq.zhixingplan.top

Go:   if s == "" {}
来源：http://jlz.sufxvd.cn

Ruby: if s.empty?
来源：http://oyx.smart0.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rdp.ydjk.org.cn

[E21] 超长截断加省略号
来源：http://ryr.shzxlz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tag.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ira.xziqi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oou.zycfv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dqa.sysykeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://efy.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://pwd.zhaomingkeji.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mdi.zhaomingkeji.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ixf.hammf.cn

[E22] 字节长度与字符长度
来源：http://rwb.bjfxy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ksr.jinyuanbaomall.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qnl.yuanzhike.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qjl.sufxvd.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xyo.jianghu66.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vcs.cashguo.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ojx.pycfn.com

Ruby: s.bytesize;  s.length
来源：http://epo.tanke756.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://etq.316326.xyz

================================================================================
来源：http://hrx.tian-w.cn

F. 文件与目录
来源：http://gjg.mhx1999.top

================================================================================
来源：http://pgb.9152youxi.cn

[F01] 读取整个文件
来源：http://ril.nwbrower.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ihw.cqqwz.cn

PHP:  file_get_contents("a.txt");
来源：http://hrp.hysaishi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jqr.epnwcf.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hjb.xziqi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://col.chenlongwang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eqr.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://lll.jianghu66.top

C#:   File.ReadAllText("a.txt");
来源：http://qav.zycfv.cn

[F02] 逐行读取文件
来源：http://nke.havefunace.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://knw.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cjg.yangfankeji.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pdf.xziqi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rbl.feifeiyinyue.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://odg.hywenlv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bwx.0kj1m.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pfq.hywenlv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jee.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://gnd.xuetiantiany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lic.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xcf.52xcode.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://npb.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://suk.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ofd.jqgfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xyk.cashguo.top

Ruby: File.write("a.txt", "hi")
来源：http://hux.hnxiangtu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ncf.316326.xyz

[F04] 追加写入文件
来源：http://gor.gogol.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rtr.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ioi.gaohongyu789.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ygp.yfazqb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uwz.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xyx.pengpengdd.cyou

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dky.nanxuanxn.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dsn.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kcn.xinyue.icu

[F05] 判断文件或目录是否存在
来源：http://bcl.hnxiangtu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qpc.jianghu66.top

PHP:  file_exists("a.txt");
来源：http://kyr.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://xmu.wangdashe.top

TS:   fs.existsSync("a.txt")
来源：http://rme.gogol.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qae.jinqigufen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gpl.quarkkingdee.top

Ruby: File.exist?("a.txt")
来源：http://qmp.fanxiaobao.xyz

C#:   File.Exists("a.txt")
来源：http://nht.sweek.top

[F06] 删除文件
来源：http://ufv.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://yeu.daria6918.cn

PHP:  unlink("a.txt");
来源：http://kus.ppjwa.cn

JS:   fs.unlinkSync("a.txt")
来源：http://njv.tian-w.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lqp.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dqf.sjlbkw.cn

Go:   os.Remove("a.txt")
来源：http://ooq.hammf.cn

Ruby: File.delete("a.txt")
来源：http://qkj.xuetiantiany.cn

C#:   File.Delete("a.txt");
来源：http://iyc.guannengcc.top

[F07] 创建目录（含多级）
来源：http://mqj.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wmr.ehwqpu.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pps.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ggx.guowangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fud.wangshuangyany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lcz.yongpay.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jga.yfazqb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qlm.zycfv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qsh.ydzc1.top

[F08] 遍历目录
来源：http://eki.daria6918.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tkk.ivvv.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nux.zhongyouzk.top

JS:   fs.readdirSync("dir")
来源：http://nmt.redwolf501.top

TS:   fs.readdirSync("dir")
来源：http://mcc.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fmw.epnwcf.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://ogg.cucudq.cn

Ruby: Dir.children("dir")
来源：http://oon.hcnkem.com

C#:   Directory.GetFiles("dir")
来源：http://psl.sweek.top

[F09] 获取文件大小
来源：http://mtv.xuetiantiany.cn

Py:   os.path.getsize("a.txt")
来源：http://hca.jlsjyb.cn

PHP:  filesize("a.txt");
来源：http://iip.yueranfly.top

JS:   fs.statSync("a.txt").size
来源：http://zvf.jlsjyb.cn

TS:   fs.statSync("a.txt").size
来源：http://nrx.redwolf501.top

Java: Files.size(Path.of("a.txt"))
来源：http://ucv.jinghuilouyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tcm.vehdjk.com

Ruby: File.size("a.txt")
来源：http://fzx.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://kqh.yfazqb.com

[F10] 取文件扩展名 / 文件名
来源：http://ssf.yj20258.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yrk.cucudq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nuz.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dsw.nwbrower.top

TS:   path.extname("a.txt")
来源：http://xiu.0kj1m.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://frz.sufxvd.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hla.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wdq.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pss.xuanzx.com

[F11] 复制与移动文件
来源：http://xfm.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wsp.ywan-chungtsiang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jek.tarul.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gxt.xingfuxueyuan.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jgj.jinqigfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gae.andypj.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wxf.bbcook.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://obd.kuanghao11.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://brm.ydzc1.top

[F12] CSV 读写
来源：http://rue.tarul.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tvn.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yjq.smart0.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qxa.uphjek.com

TS:   // 同上
来源：http://gnj.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ooc.sxryk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jcu.ydjk.org.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kxw.hysaishi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://poj.hesvh.cn

================================================================================
来源：http://tfy.guowangkeji.top

G. 面向对象
来源：http://pnh.zycfv.cn

================================================================================
来源：http://tzm.ppjwa.cn

[G01] 定义类
来源：http://hyi.andypj.xyz

Py:   class User: pass
来源：http://ryd.havefunace.top

PHP:  class User {}
来源：http://dwg.wangshuangyany.cn

JS:   class User {}
来源：http://rke.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://qml.jiagoushi.top

Java: class User {}
来源：http://lfq.hesvh.cn

Go:   type User struct { Name string }
来源：http://ygk.yfazqb.com

Ruby: class User; end
来源：http://gev.ctjpmb.com

C#:   class User {}
来源：http://jfy.wangshuangyany.cn

[G02] 构造函数
来源：http://uub.zycfv.cn

Py:   def __init__(self, name): self.name = name
来源：http://zzd.epnwcf.com

PHP:  public function __construct(public string $name) {}
来源：http://ugz.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://lix.yongpay.top

TS:   constructor(public name: string) {}
来源：http://qbk.zdqjudy.top

Java: User(String name) { this.name = name; }
来源：http://rav.snrcjt.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lxs.svipenyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://ibz.vqdsnc.cn

C#:   public User(string name) { Name = name; }
来源：http://fwp.zhiwuduotai.top

[G03] 实例属性
来源：http://kmg.shangyingyoupin.top

Py:   self.name = "x"
来源：http://qdo.ybcxt.top

PHP:  public string $name = "x";
来源：http://een.fengsongda.top

JS:   this.name = "x";
来源：http://txk.zhixingplan.top

TS:   name: string = "x";
来源：http://jve.shanyushiyangtech.top

Java: private String name;
来源：http://lky.andypj.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://spw.hysaishi.cn

Ruby: @name = "x"
来源：http://hvp.jqgfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://hwe.316326.xyz

[G04] 定义方法
来源：http://ypn.andypj.xyz

Py:   def greet(self): return self.name
来源：http://hwg.sjlbkw.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://asy.andypj.xyz

JS:   greet() { return this.name; }
来源：http://wmu.ppjwa.cn

TS:   greet(): string { return this.name; }
来源：http://dme.ydjk.org.cn

Java: String greet() { return name; }
来源：http://ggi.dashuyun.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://txs.fengsongda.top

Ruby: def greet; @name; end
来源：http://odk.cheryme.top

C#:   public string Greet() => Name;
来源：http://dtw.cashguo.top

[G05] 继承
来源：http://qgv.yonumen.top

Py:   class Admin(User): pass
来源：http://sbg.yj20258888.top

PHP:  class Admin extends User {}
来源：http://bbk.hcnkem.com

JS:   class Admin extends User {}
来源：http://htx.jqgfzy.top

TS:   class Admin extends User {}
来源：http://jee.sjlbkw.cn

Java: class Admin extends User {}
来源：http://pex.yvedp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hup.zhixingplan.top

Ruby: class Admin < User; end
来源：http://wsq.zhoulong.xyz

C#:   class Admin : User {}
来源：http://bui.shanyushiyangkeji.top

[G06] 重写方法
来源：http://jit.guannengcc.top

Py:   def greet(self): return "admin"
来源：http://jgz.yvedp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uup.zhongyouzk.top

JS:   greet() { return "admin"; }
来源：http://jyt.ivvv.top

TS:   greet(): string { return "admin"; }
来源：http://cry.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://aac.xziqi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bgw.zhoulong.xyz

Ruby: def greet; "admin"; end
来源：http://rpl.wangdashe.top

C#:   public override string Greet() => "admin";
来源：http://ras.ydjk.org.cn

[G07] 调用父类方法
来源：http://pim.jqgufenzy.top

Py:   super().greet()
来源：http://juo.gogol.net.cn

PHP:  parent::greet();
来源：http://tbm.sjlbkw.cn

JS:   super.greet();
来源：http://mea.havefunace.top

TS:   super.greet();
来源：http://nrq.mhx1999.top

Java: super.greet();
来源：http://xjt.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qqi.ppjwa.cn

Ruby: super
来源：http://qud.gogol.net.cn

C#:   base.Greet();
来源：http://ipb.sjlbkw.cn

[G08] 静态方法与属性
来源：http://mlc.zhengqikj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lun.tianlin.xyz

PHP:  public static function f() {}
来源：http://lsn.zhengqikj.top

JS:   static f() {}
来源：http://xck.yuxming.cn

TS:   static f(): void {}
来源：http://gnd.yongpay.top

Java: static void f() {}
来源：http://awr.yangfankeji.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://wmj.fengsongda.top

Ruby: def self.f; end
来源：http://kkb.xylfe.cn

C#:   public static void F() {}
来源：http://jtm.c1oappe.top

[G09] 接口 / 抽象类
来源：http://jqh.xylfe.cn

Py:   from abc import ABC, abstractmethod
来源：http://tpd.yangfankeji.com

PHP:  interface Shape { public function area(): float; }
来源：http://djv.cheryme.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ltb.aibaodan.cn

TS:   interface Shape { area(): number; }
来源：http://ixk.vqdsnc.cn

Java: interface Shape { double area(); }
来源：http://til.jyoumei.cn

Go:   type Shape interface { Area() float64 }
来源：http://jzn.wangshuangyany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jpl.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://vyj.yfazqb.com

[G10] 访问控制
来源：http://xpx.sjlbkw.cn

Py:   约定 _protected / __private（不强制）
来源：http://pia.cheryme.top

PHP:  public / protected / private
来源：http://wvz.yvedp.cn

JS:   #private 字段；其余公开
来源：http://ovx.vqdsnc.cn

TS:   public / protected / private
来源：http://tca.sjlbkw.cn

Java: public / protected / private / 默认包级
来源：http://bjg.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ukj.zhiwuduotai.top

Ruby: public / protected / private
来源：http://krg.jiagoushi.top

C#:   public / protected / private / internal
来源：http://wkv.yj20258888.top

[G11] getter / setter
来源：http://ums.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://lly.zhixingplan.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wkj.ppjwa.cn

JS:   get name() { return this._name; }
来源：http://ybd.zycfv.cn

TS:   get name(): string { return this._name; }
来源：http://bqt.feifeiyinyue.top

Java: public String getName() { return name; }
来源：http://asj.dianchejie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bgr.wangdashe.top

Ruby: attr_accessor :name
来源：http://hjr.yuxming.cn

C#:   public string Name { get; set; }
来源：http://uyh.nwbrower.top

[G12] 对象转字符串
来源：http://zmr.sweek.top

Py:   def __str__(self): return self.name
来源：http://epo.zycfv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://axj.fehbvm.com

JS:   toString() { return this.name; }
来源：http://cxa.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://hdt.feifeiyinyue.top

Java: @Override public String toString() { return name; }
来源：http://cet.chenlongwang.top

Go:   func (u User) String() string { return u.Name }
来源：http://coz.zhiwuduotai.top

Ruby: def to_s; @name; end
来源：http://ent.zhixingplan.top

C#:   public override string ToString() => Name;
来源：http://bge.jlsjyb.cn

[G13] 判断对象类型
来源：http://uyx.yangfankeji.com

Py:   isinstance(u, User)
来源：http://dxy.zhijiandao.cn

PHP:  $u instanceof User
来源：http://sri.yfazqb.com

JS:   u instanceof User
来源：http://huv.havefunace.top

TS:   u instanceof User
来源：http://qqu.hnqzz.top

Java: u instanceof User
来源：http://sqk.jlsjyb.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xug.zhixingplan.top

Ruby: u.is_a?(User)
来源：http://fqe.daxiang520.top

C#:   u is User
来源：http://luj.chenjidiqi.icu

[G14] 数据类 / record
来源：http://kne.ybcxt.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kwz.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://gxf.yongpay.top

JS:   // 无内置：普通类或对象字面量
来源：http://xrj.zdqjudy.top


<!-- 参考信息 -->