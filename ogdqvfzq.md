代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lws.tarul.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qqc.9152youxi.cn

[E16] 数字千分位
来源：http://vcg.ywan-chungtsiang.top

Py:   f"{1234567:,}"
来源：http://lby.cheryme.top

PHP:  number_format(1234567);
来源：http://nys.sweek.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ygm.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://skq.yj20258.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://csz.yj20258.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://emq.quarkkingdee.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://flw.fengsongda.top

C#:   1234567.ToString("N0")
来源：http://qsb.aibaodan.cn

[E17] 首字母大写
来源：http://iwy.dianchejie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hfh.yj202588.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://icp.pengpengdd.cyou

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mat.yvedp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://azy.ivvv.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rwn.gotoacloud.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wvc.hfpthk.cn

Ruby: s.capitalize
来源：http://phc.gogol.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://alg.cheryme.top

[E18] 模板占位符替换
来源：http://gbj.52xcode.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ikw.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://erc.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://thz.ydzc1.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wwk.jlsjyb.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://boj.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://irz.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lbc.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lzg.cdnleiting.top

[E19] 多行文本按行拆分
来源：http://gbz.feifeiyinyue.top

Py:   s.splitlines()
来源：http://ifs.zhoulong.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dzn.ywan-chungtsiang.top

JS:   s.split(/\r?\n/)
来源：http://xwg.zhengqikj.top

TS:   s.split(/\r?\n/)
来源：http://dom.wangshuangyany.cn

Java: s.lines().toList()
来源：http://pyo.0kj1m.cn

Go:   strings.Split(s, "\n")
来源：http://zzr.redwolf501.top

Ruby: s.lines
来源：http://ftl.xingfuxueyuan.xyz

C#:   s.Split('\n')
来源：http://sxp.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://psc.bjfxy.top

Py:   if not s:
来源：http://den.hysaishi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aqq.sufxvd.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ioc.havefunace.top

TS:   if (s === "") {}
来源：http://egj.52xcode.cn

Java: if (s.isEmpty()) {}
来源：http://jqn.shuidangran.top

Go:   if s == "" {}
来源：http://sll.epnwcf.com

Ruby: if s.empty?
来源：http://oxv.gogol.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nuo.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://hix.jinyuanbaomall.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nml.haohaochexian.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uis.tianlin.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://glp.feifeiyinyue.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ngo.yuanzhike.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xir.pengpengdd.cyou

Go:   // 按 rune 判断长度后截断
来源：http://sfi.yongpay.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bkj.316326.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cyy.cdnleiting.top

[E22] 字节长度与字符长度
来源：http://wxz.aizwys.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://thy.cucudq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://axj.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://edm.snrcjt.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yoi.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xxd.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bma.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://vqm.jinghuilouyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qon.bbcook.cn

================================================================================
来源：http://tmy.yonumen.top

F. 文件与目录
来源：http://gsc.pycfn.com

================================================================================
来源：http://ckd.xingfuxueyuan.xyz

[F01] 读取整个文件
来源：http://roa.xziqi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pew.ywan-chungtsiang.top

PHP:  file_get_contents("a.txt");
来源：http://hjp.52xcode.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fou.yj20258.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qzs.bbcook.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xpe.kuanghao11.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mbj.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://ezs.hnxiangtu.top

C#:   File.ReadAllText("a.txt");
来源：http://kjx.dashuyun.cn

[F02] 逐行读取文件
来源：http://fhk.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uez.ydjk.org.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mxt.ivvv.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wil.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kkw.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mng.bjfxy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eqd.xingfuxueyuan.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zol.uphjek.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kou.zhixingplan.top

[F03] 写入文件（覆盖）
来源：http://ukr.cqqwz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tju.shzxlz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://npv.yj202588.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gko.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hqb.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qan.yongpay.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ltj.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://oxv.chenzaomai.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jkk.chenlongwang.top

[F04] 追加写入文件
来源：http://yik.jinghuilouyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://phi.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hkg.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wob.zhijiandao.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ncy.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mly.aizwys.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yyj.vqdsnc.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://znd.aibaodan.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eyg.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://qsd.nanxuanxn.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ein.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://nvg.jinyuanbaomall.cn

JS:   fs.existsSync("a.txt")
来源：http://rub.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://nov.daxiang520.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sax.birdmap.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://coy.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://tex.fehbvm.com

C#:   File.Exists("a.txt")
来源：http://pfx.epnwcf.com

[F06] 删除文件
来源：http://zib.fehbvm.com

Py:   os.remove("a.txt")
来源：http://sic.jiagoushi.top

PHP:  unlink("a.txt");
来源：http://bkz.jinqigfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://pwy.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nux.ivvv.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pwt.guowangkeji.top

Go:   os.Remove("a.txt")
来源：http://qyr.snrcjt.cn

Ruby: File.delete("a.txt")
来源：http://tph.jiagoushi.top

C#:   File.Delete("a.txt");
来源：http://zwd.mhx1999.top

[F07] 创建目录（含多级）
来源：http://aet.tian-w.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cyg.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hos.cqqwz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aam.jinghuilouyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mly.gzhubu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://soy.yuxming.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hqu.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tma.xingfuxueyuan.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://frz.shzxlz.cn

[F08] 遍历目录
来源：http://jfk.ywan-chungtsiang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://aqx.bbcook.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kfx.dashuyun.cn

JS:   fs.readdirSync("dir")
来源：http://mjj.mhx1999.top

TS:   fs.readdirSync("dir")
来源：http://giz.xziqi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tsz.vehdjk.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://veg.chenzaomai.com

Ruby: Dir.children("dir")
来源：http://tau.zhongyouzk.top

C#:   Directory.GetFiles("dir")
来源：http://ekh.zhoulong.xyz

[F09] 获取文件大小
来源：http://uwt.pycfn.com

Py:   os.path.getsize("a.txt")
来源：http://qwz.zhijiandao.cn

PHP:  filesize("a.txt");
来源：http://zpe.tarul.cn

JS:   fs.statSync("a.txt").size
来源：http://gcm.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://hdf.hywenlv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://amf.yfazqb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lgt.yangfankeji.com

Ruby: File.size("a.txt")
来源：http://niw.fktsv.cn

C#:   new FileInfo("a.txt").Length
来源：http://plu.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://plr.ydjk.org.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tvl.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lwy.smart0.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vqp.fehbvm.com

TS:   path.extname("a.txt")
来源：http://auw.chenzaomai.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://afq.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://owq.zhoulong.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xpk.fktsv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ess.gaohongyu789.top

[F11] 复制与移动文件
来源：http://bmy.zhongyouzk.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ixg.yj20258888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nfd.ybcxt.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dgy.tianlin.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://szw.xingfuxueyuan.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mpm.nanxinkj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uwm.pengpengdd.cyou

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bae.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jfn.zhixingplan.top

[F12] CSV 读写
来源：http://med.shangyingyoupin.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mpm.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://onc.sufxvd.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cgx.hysaishi.cn

TS:   // 同上
来源：http://dpl.ivvv.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pcj.shzxlz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lio.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yfi.shzxlz.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rty.zhoulong.xyz

================================================================================
来源：http://dfr.uphjek.com

G. 面向对象
来源：http://khj.shzxlz.cn

================================================================================
来源：http://mtn.jlsjyb.cn

[G01] 定义类
来源：http://edm.shuidangran.top

Py:   class User: pass
来源：http://wml.wangshuangyany.cn

PHP:  class User {}
来源：http://hux.vehdjk.com

JS:   class User {}
来源：http://hbg.yanxiufei.cn

TS:   class User { name: string = ""; }
来源：http://dfv.iojbl.cn

Java: class User {}
来源：http://raf.pycfn.com

Go:   type User struct { Name string }
来源：http://lbv.dashuyun.cn

Ruby: class User; end
来源：http://cej.hongshengwenyu.top

C#:   class User {}
来源：http://qak.daxiang520.top

[G02] 构造函数
来源：http://beo.ybcxt.top

Py:   def __init__(self, name): self.name = name
来源：http://tew.yj20258.top

PHP:  public function __construct(public string $name) {}
来源：http://ufr.cqqwz.cn

JS:   constructor(name) { this.name = name; }
来源：http://lfn.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://pgy.sxryk.cn

Java: User(String name) { this.name = name; }
来源：http://wyl.ydzc1.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xez.quarkkingdee.top

Ruby: def initialize(name); @name = name; end
来源：http://ieq.vqdsnc.cn

C#:   public User(string name) { Name = name; }
来源：http://ljk.xuanzx.com

[G03] 实例属性
来源：http://ptf.tarul.cn

Py:   self.name = "x"
来源：http://tmh.hammf.cn

PHP:  public string $name = "x";
来源：http://txn.hcnkem.com

JS:   this.name = "x";
来源：http://mqg.hesvh.cn

TS:   name: string = "x";
来源：http://vrx.epnwcf.com

Java: private String name;
来源：http://xqb.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wga.hammf.cn

Ruby: @name = "x"
来源：http://bwh.hnxiangtu.top

C#:   public string Name { get; set; } = "x";
来源：http://tvh.hesvh.cn

[G04] 定义方法
来源：http://teg.andypj.xyz

Py:   def greet(self): return self.name
来源：http://vqh.gzhubu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ldz.gaohongyu789.top

JS:   greet() { return this.name; }
来源：http://rmu.jinghuilouyu.cn

TS:   greet(): string { return this.name; }
来源：http://hol.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://yxc.nanxuanxn.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fxx.yj20258.top

Ruby: def greet; @name; end
来源：http://ipv.aibaodan.cn

C#:   public string Greet() => Name;
来源：http://frz.fktsv.cn

[G05] 继承
来源：http://lbc.yanxiufei.cn

Py:   class Admin(User): pass
来源：http://xmh.yfazqb.com

PHP:  class Admin extends User {}
来源：http://rwc.mhx1999.top

JS:   class Admin extends User {}
来源：http://jii.sysykeji.top

TS:   class Admin extends User {}
来源：http://beq.snrcjt.cn

Java: class Admin extends User {}
来源：http://zvy.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bgp.jinghuilouyu.cn

Ruby: class Admin < User; end
来源：http://wmz.daria6918.cn

C#:   class Admin : User {}
来源：http://tfq.snrcjt.cn

[G06] 重写方法
来源：http://mfr.hfpthk.cn

Py:   def greet(self): return "admin"
来源：http://nes.zhijiandao.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://riq.zhixingplan.top

JS:   greet() { return "admin"; }
来源：http://zgs.hesvh.cn

TS:   greet(): string { return "admin"; }
来源：http://rmx.0kj1m.cn

Java: @Override String greet() { return "admin"; }
来源：http://fmp.sysykeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vbc.xinyue.icu

Ruby: def greet; "admin"; end
来源：http://fbh.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://ceu.hesvh.cn

[G07] 调用父类方法
来源：http://yuq.fanxiaobao.xyz

Py:   super().greet()
来源：http://uhz.ivvv.top

PHP:  parent::greet();
来源：http://lrd.yvedp.cn

JS:   super.greet();
来源：http://nsk.jinqigfzy.top

TS:   super.greet();
来源：http://vnz.hongshengwenyu.top

Java: super.greet();
来源：http://jkb.yj20258888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ivl.tian-w.cn

Ruby: super
来源：http://lfs.zhoulong.xyz

C#:   base.Greet();
来源：http://olw.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://gqs.sysykeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dob.havefunace.top

PHP:  public static function f() {}
来源：http://xvj.52xcode.cn

JS:   static f() {}
来源：http://goq.shanyushiyangtech.top

TS:   static f(): void {}
来源：http://ole.vehdjk.com

Java: static void f() {}
来源：http://cos.aibaodan.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hjm.jiagoushi.top

Ruby: def self.f; end
来源：http://vtx.snrcjt.cn

C#:   public static void F() {}
来源：http://aji.fengsongda.top

[G09] 接口 / 抽象类
来源：http://ayu.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://hvg.hesvh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xlj.52xcode.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://spa.iojbl.cn

TS:   interface Shape { area(): number; }
来源：http://trb.pengpengdd.cyou

Java: interface Shape { double area(); }
来源：http://pze.shanyushiyangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://ifn.hfpthk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yzu.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://pwh.fktsv.cn

[G10] 访问控制
来源：http://feu.iojbl.cn

Py:   约定 _protected / __private（不强制）
来源：http://pub.jinghuilouyu.cn

PHP:  public / protected / private
来源：http://yca.bjfxy.top

JS:   #private 字段；其余公开
来源：http://shi.wangdashe.top

TS:   public / protected / private
来源：http://jmv.cdnleiting.top

Java: public / protected / private / 默认包级
来源：http://sxj.feifeiyinyue.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kmz.sysykeji.top

Ruby: public / protected / private
来源：http://ivd.havefunace.top

C#:   public / protected / private / internal
来源：http://sbe.ydzc1.top

[G11] getter / setter
来源：http://ssz.hammf.cn

Py:   @property 与 @x.setter
来源：http://ibw.andypj.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://trs.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://ibo.iojbl.cn

TS:   get name(): string { return this._name; }
来源：http://buv.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://vrq.yvedp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bin.hesvh.cn

Ruby: attr_accessor :name
来源：http://vik.chenlongwang.top

C#:   public string Name { get; set; }
来源：http://whf.xuanzx.com

[G12] 对象转字符串
来源：http://ptd.kuanghao11.cn

Py:   def __str__(self): return self.name
来源：http://ekv.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bat.chenzaomai.com

JS:   toString() { return this.name; }
来源：http://dng.jiagoushi.top

TS:   toString(): string { return this.name; }
来源：http://tzw.xingfuxueyuan.xyz

Java: @Override public String toString() { return name; }
来源：http://svn.ywan-chungtsiang.top

Go:   func (u User) String() string { return u.Name }
来源：http://xom.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://bly.52xcode.cn

C#:   public override string ToString() => Name;
来源：http://rtm.zdbjq.cn

[G13] 判断对象类型
来源：http://dyg.wangshuangyany.cn

Py:   isinstance(u, User)
来源：http://rhy.epnwcf.com

PHP:  $u instanceof User
来源：http://wvh.ctjpmb.com

JS:   u instanceof User
来源：http://oph.uphjek.com

TS:   u instanceof User
来源：http://yje.zhiwuduotai.top

Java: u instanceof User
来源：http://lui.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jbe.ydzc1.top

Ruby: u.is_a?(User)
来源：http://hbt.bjfxy.top

C#:   u is User
来源：http://xdv.shzxlz.cn

[G14] 数据类 / record
来源：http://wbw.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hul.316326.xyz

PHP:  // 用 readonly 属性模拟
来源：http://jnw.hammf.cn

JS:   // 无内置：普通类或对象字面量
来源：http://avc.jinqigufen.top


<!-- 参考信息 -->