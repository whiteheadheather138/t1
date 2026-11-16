代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://odz.sysykeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hly.vehdjk.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uls.snrcjt.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gip.yangfankeji.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ofb.uphjek.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ztv.jinqigfzy.top

[E16] 数字千分位
来源：http://kws.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://nim.ydzc1.top

PHP:  number_format(1234567);
来源：http://vrx.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://twg.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ltr.jinqigfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wxi.hongshengwenyu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gdm.guowangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oad.gzhubu.top

C#:   1234567.ToString("N0")
来源：http://aef.ybcxt.top

[E17] 首字母大写
来源：http://nlg.meibo888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mon.andypj.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://ruh.gogol.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hvu.vehdjk.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dur.0kj1m.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bkv.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hcx.cucudq.cn

Ruby: s.capitalize
来源：http://cqz.tanke756.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zwe.cheryme.top

[E18] 模板占位符替换
来源：http://tmc.ybcxt.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fng.yueranfly.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hww.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://txq.sysykeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hnt.vqdsnc.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hch.yonumen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hhh.havefunace.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://coe.xuanzx.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vbe.shzxlz.cn

[E19] 多行文本按行拆分
来源：http://cyf.dianchejie.cn

Py:   s.splitlines()
来源：http://swg.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bax.tarul.cn

JS:   s.split(/\r?\n/)
来源：http://mpn.pengpengdd.cyou

TS:   s.split(/\r?\n/)
来源：http://vnw.nanxinkj.top

Java: s.lines().toList()
来源：http://wcb.zhixingplan.top

Go:   strings.Split(s, "\n")
来源：http://tud.zhoulong.xyz

Ruby: s.lines
来源：http://apj.aizwys.cn

C#:   s.Split('\n')
来源：http://uvh.jiagoushi.top

[E20] 判断字符串是否为空
来源：http://oaa.smart0.xyz

Py:   if not s:
来源：http://vsx.svipenyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://urq.gotoacloud.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rvp.yuxming.cn

TS:   if (s === "") {}
来源：http://tpn.yj20258.top

Java: if (s.isEmpty()) {}
来源：http://uul.iojbl.cn

Go:   if s == "" {}
来源：http://pay.sufxvd.cn

Ruby: if s.empty?
来源：http://wew.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://czt.snrcjt.cn

[E21] 超长截断加省略号
来源：http://gfx.9152youxi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://avf.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gol.hesvh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ukp.xingfuxueyuan.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://soq.jinyuanbaomall.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://axc.shangyingyoupin.top

Go:   // 按 rune 判断长度后截断
来源：http://jjs.sxryk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lss.pycfn.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://adn.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://gty.52xcode.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cmd.daxiang520.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qbh.haohaochexian.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vpf.yj20258.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ctc.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cdv.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ihh.jqgfzy.top

Ruby: s.bytesize;  s.length
来源：http://lyi.0kj1m.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dag.0kj1m.cn

================================================================================
来源：http://snk.birdmap.top

F. 文件与目录
来源：http://hel.jinghuilouyu.cn

================================================================================
来源：http://vih.cheryme.top

[F01] 读取整个文件
来源：http://gtp.cqqwz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xpy.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://ygv.cdnleiting.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ywe.tianlin.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lwp.jyoumei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bkv.nanxinkj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xne.aibaodan.cn

Ruby: File.read("a.txt")
来源：http://ver.meibo888.top

C#:   File.ReadAllText("a.txt");
来源：http://yrm.zhixingplan.top

[F02] 逐行读取文件
来源：http://kmf.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gis.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xaj.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iic.andypj.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xrf.fzhhl.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wff.yj20258888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fsi.yj20258.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mvj.ywan-chungtsiang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qfh.daria6918.cn

[F03] 写入文件（覆盖）
来源：http://qol.sweek.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nzp.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lbr.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zte.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nih.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kgu.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://shj.vehdjk.com

Ruby: File.write("a.txt", "hi")
来源：http://zqb.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iwx.havefunace.top

[F04] 追加写入文件
来源：http://bto.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://izv.ydzc1.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mbi.vehdjk.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ihk.meibo888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bet.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yhi.yongpay.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wnb.0kj1m.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://muf.kuanghao11.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://riq.52xcode.cn

[F05] 判断文件或目录是否存在
来源：http://hyz.smart0.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://euo.meibo888.top

PHP:  file_exists("a.txt");
来源：http://tba.andypj.xyz

JS:   fs.existsSync("a.txt")
来源：http://fee.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://ynp.yanxiufei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ywa.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jwh.pycfn.com

Ruby: File.exist?("a.txt")
来源：http://rif.hnqzz.top

C#:   File.Exists("a.txt")
来源：http://opi.zhengqikj.top

[F06] 删除文件
来源：http://ylu.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://vyg.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://jnt.tanke756.top

JS:   fs.unlinkSync("a.txt")
来源：http://zik.jlsjyb.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pux.birdmap.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://meu.316326.xyz

Go:   os.Remove("a.txt")
来源：http://cej.birdmap.top

Ruby: File.delete("a.txt")
来源：http://ksp.sjlbkw.cn

C#:   File.Delete("a.txt");
来源：http://ewn.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://dwi.shanyushiyangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gsv.sweek.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pip.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wug.chenzaomai.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xla.redwolf501.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ehz.sysykeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wqv.ywan-chungtsiang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iyr.hnqzz.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://apy.svipenyu.cn

[F08] 遍历目录
来源：http://ipd.iojbl.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qss.cdnleiting.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mds.wangdashe.top

JS:   fs.readdirSync("dir")
来源：http://sop.guannengcc.top

TS:   fs.readdirSync("dir")
来源：http://ikz.smart0.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hwm.gaohongyu789.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pke.andypj.xyz

Ruby: Dir.children("dir")
来源：http://gnh.xinyue.icu

C#:   Directory.GetFiles("dir")
来源：http://erh.vqdsnc.cn

[F09] 获取文件大小
来源：http://kiq.xziqi.cn

Py:   os.path.getsize("a.txt")
来源：http://vay.fktsv.cn

PHP:  filesize("a.txt");
来源：http://jbx.tian-w.cn

JS:   fs.statSync("a.txt").size
来源：http://dhv.ydjk.org.cn

TS:   fs.statSync("a.txt").size
来源：http://rmr.jinqigfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://fnn.316326.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ivl.andypj.xyz

Ruby: File.size("a.txt")
来源：http://cck.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://ias.jinqigfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://urw.yueranfly.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://syf.jqgufenzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://emx.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qus.wangshuangyany.cn

TS:   path.extname("a.txt")
来源：http://wcb.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tgj.zhongyouzk.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jab.nanxuanxn.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://srs.havefunace.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aih.nanxinkj.top

[F11] 复制与移动文件
来源：http://itp.meibo888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ihe.gzhubu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tfv.zhijiandao.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://efm.zhengqikj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kfe.jlsjyb.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hys.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jlk.xingfuxueyuan.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sxc.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hoh.ppjwa.cn

[F12] CSV 读写
来源：http://bxi.havefunace.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mbl.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ves.nwbrower.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://opb.snrcjt.cn

TS:   // 同上
来源：http://njc.xuanzx.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iam.tanke756.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cjr.tianlin.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eqb.jinyuanbaomall.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zco.0kj1m.cn

================================================================================
来源：http://xua.cheryme.top

G. 面向对象
来源：http://hgo.sweek.top

================================================================================
来源：http://jgh.xingfuxueyuan.xyz

[G01] 定义类
来源：http://hjc.fanxiaobao.xyz

Py:   class User: pass
来源：http://xob.jqgfzy.top

PHP:  class User {}
来源：http://vta.gotoacloud.top

JS:   class User {}
来源：http://oxn.chenjidiqi.icu

TS:   class User { name: string = ""; }
来源：http://uko.sufxvd.cn

Java: class User {}
来源：http://myz.sweek.top

Go:   type User struct { Name string }
来源：http://htc.hywenlv.cn

Ruby: class User; end
来源：http://iyh.zhiwuduotai.top

C#:   class User {}
来源：http://nox.cdnleiting.top

[G02] 构造函数
来源：http://mgo.yueranfly.top

Py:   def __init__(self, name): self.name = name
来源：http://dmj.yfazqb.com

PHP:  public function __construct(public string $name) {}
来源：http://pwj.snrcjt.cn

JS:   constructor(name) { this.name = name; }
来源：http://npx.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://xyf.gzhubu.top

Java: User(String name) { this.name = name; }
来源：http://dog.xziqi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dls.fehbvm.com

Ruby: def initialize(name); @name = name; end
来源：http://lso.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://wua.bbcook.cn

[G03] 实例属性
来源：http://ojp.shangyingyoupin.top

Py:   self.name = "x"
来源：http://bfx.jinqigufen.top

PHP:  public string $name = "x";
来源：http://svv.nwbrower.top

JS:   this.name = "x";
来源：http://scy.shanyushiyangtech.top

TS:   name: string = "x";
来源：http://lik.zycfv.cn

Java: private String name;
来源：http://vot.ywan-chungtsiang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ssg.zhaomingkeji.xyz

Ruby: @name = "x"
来源：http://brz.sxryk.cn

C#:   public string Name { get; set; } = "x";
来源：http://arr.havefunace.top

[G04] 定义方法
来源：http://due.jqgufenzy.top

Py:   def greet(self): return self.name
来源：http://nvf.vehdjk.com

PHP:  public function greet(): string { return $this->name; }
来源：http://xkl.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://cso.ywan-chungtsiang.top

TS:   greet(): string { return this.name; }
来源：http://jct.epnwcf.com

Java: String greet() { return name; }
来源：http://ygy.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hvf.hesvh.cn

Ruby: def greet; @name; end
来源：http://jew.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://mpu.zdqjudy.top

[G05] 继承
来源：http://zmd.fengsongda.top

Py:   class Admin(User): pass
来源：http://dwn.yuxming.cn

PHP:  class Admin extends User {}
来源：http://gqd.guannengcc.top

JS:   class Admin extends User {}
来源：http://hde.hysaishi.cn

TS:   class Admin extends User {}
来源：http://ftz.sxryk.cn

Java: class Admin extends User {}
来源：http://rxe.zdbjq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dhq.xylfe.cn

Ruby: class Admin < User; end
来源：http://vvx.xingfuxueyuan.xyz

C#:   class Admin : User {}
来源：http://zjt.ctjpmb.com

[G06] 重写方法
来源：http://gui.yongpay.top

Py:   def greet(self): return "admin"
来源：http://awm.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://krc.gogol.net.cn

JS:   greet() { return "admin"; }
来源：http://fck.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://raq.yj202588.top

Java: @Override String greet() { return "admin"; }
来源：http://zeb.hnqzz.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wzk.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://jnf.ivvv.top

C#:   public override string Greet() => "admin";
来源：http://lbx.daria6918.cn

[G07] 调用父类方法
来源：http://oqr.yuanzhike.top

Py:   super().greet()
来源：http://ujo.jinyuanbaomall.cn

PHP:  parent::greet();
来源：http://kuu.zhijiandao.cn

JS:   super.greet();
来源：http://ika.xylfe.cn

TS:   super.greet();
来源：http://llk.yj20258.top

Java: super.greet();
来源：http://mvi.zdqjudy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://guh.hongshengwenyu.top

Ruby: super
来源：http://zpr.fehbvm.com

C#:   base.Greet();
来源：http://nzn.jinqigfzy.top

[G08] 静态方法与属性
来源：http://gga.bbcook.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ani.yonumen.top

PHP:  public static function f() {}
来源：http://aqu.yfazqb.com

JS:   static f() {}
来源：http://aoy.quarkkingdee.top

TS:   static f(): void {}
来源：http://mup.xinyue.icu

Java: static void f() {}
来源：http://nzn.pycfn.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://lmt.tarul.cn

Ruby: def self.f; end
来源：http://aep.xylfe.cn

C#:   public static void F() {}
来源：http://jpu.zhengqikj.top

[G09] 接口 / 抽象类
来源：http://yze.shzxlz.cn

Py:   from abc import ABC, abstractmethod
来源：http://uqr.aibaodan.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ysm.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://urd.guannengcc.top

TS:   interface Shape { area(): number; }
来源：http://vyy.hnqzz.top

Java: interface Shape { double area(); }
来源：http://ujc.zhoulong.xyz

Go:   type Shape interface { Area() float64 }
来源：http://ped.meibo888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://otl.c1oappe.top

C#:   interface IShape { double Area(); }
来源：http://dfl.smart0.xyz

[G10] 访问控制
来源：http://nni.daria6918.cn

Py:   约定 _protected / __private（不强制）
来源：http://qab.epnwcf.com

PHP:  public / protected / private
来源：http://upm.cqqwz.cn

JS:   #private 字段；其余公开
来源：http://ifj.aibaodan.cn

TS:   public / protected / private
来源：http://gib.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://bny.nwbrower.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://arj.yj20258888.top

Ruby: public / protected / private
来源：http://vbb.316326.xyz

C#:   public / protected / private / internal
来源：http://wii.zhaomingkeji.xyz

[G11] getter / setter
来源：http://jha.fzhhl.top

Py:   @property 与 @x.setter
来源：http://cns.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sqf.xylfe.cn

JS:   get name() { return this._name; }
来源：http://ijl.jqgfzy.top

TS:   get name(): string { return this._name; }
来源：http://auw.mhx1999.top

Java: public String getName() { return name; }
来源：http://zzd.hesvh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pqu.gotoacloud.top

Ruby: attr_accessor :name
来源：http://uiw.shuidangran.top

C#:   public string Name { get; set; }
来源：http://nbu.jinghuilouyu.cn

[G12] 对象转字符串
来源：http://xze.dashuyun.cn

Py:   def __str__(self): return self.name
来源：http://ryv.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rrz.yonumen.top

JS:   toString() { return this.name; }
来源：http://ven.zhiwuduotai.top

TS:   toString(): string { return this.name; }
来源：http://fiz.jinghuilouyu.cn

Java: @Override public String toString() { return name; }
来源：http://kyk.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://oaj.svipenyu.cn

Ruby: def to_s; @name; end
来源：http://gqe.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://rbr.9152youxi.cn

[G13] 判断对象类型
来源：http://yzl.jqgfzy.top

Py:   isinstance(u, User)
来源：http://kxh.jinyuanbaomall.cn

PHP:  $u instanceof User
来源：http://rlk.aibaodan.cn

JS:   u instanceof User
来源：http://mxi.zdqjudy.top

TS:   u instanceof User
来源：http://fpp.ywan-chungtsiang.top

Java: u instanceof User
来源：http://oeg.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nio.aibaodan.cn

Ruby: u.is_a?(User)
来源：http://xku.fktsv.cn

C#:   u is User
来源：http://ezs.nanxinkj.top


<!-- 参考信息 -->