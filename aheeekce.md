代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lkf.c1oappe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wvm.gzhubu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dtx.jiagoushi.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://acl.c1oappe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kcx.yanxiufei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sht.52xcode.cn

Ruby: s.capitalize
来源：http://vqo.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hdm.wangdashe.top

[E18] 模板占位符替换
来源：http://iwp.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://saz.aizwys.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dkc.zhongyouzk.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rri.ydzc1.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yhn.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://igc.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://equ.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qqe.tanke756.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dtr.dashuyun.cn

[E19] 多行文本按行拆分
来源：http://iip.sufxvd.cn

Py:   s.splitlines()
来源：http://sxy.cqqwz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iwr.zhongyouzk.top

JS:   s.split(/\r?\n/)
来源：http://juy.hammf.cn

TS:   s.split(/\r?\n/)
来源：http://pms.ctjpmb.com

Java: s.lines().toList()
来源：http://sit.dianchejie.cn

Go:   strings.Split(s, "\n")
来源：http://uum.zhaomingkeji.xyz

Ruby: s.lines
来源：http://dlx.shanyushiyangtech.top

C#:   s.Split('\n')
来源：http://fbq.bjfxy.top

[E20] 判断字符串是否为空
来源：http://uci.havefunace.top

Py:   if not s:
来源：http://upa.yj20258.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xmw.fengsongda.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ibu.ivvv.top

TS:   if (s === "") {}
来源：http://rqm.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://uyk.feifeiyinyue.top

Go:   if s == "" {}
来源：http://yor.yueranfly.top

Ruby: if s.empty?
来源：http://stw.yanxiufei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qol.guowangkeji.top

[E21] 超长截断加省略号
来源：http://zrh.jinqigufen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xrv.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lqr.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pnk.jinqigfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fjh.wangshuangyany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kce.gzhubu.top

Go:   // 按 rune 判断长度后截断
来源：http://rnt.zycfv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bah.xuanzx.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zrg.tian-w.cn

[E22] 字节长度与字符长度
来源：http://trr.sxryk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ehe.epnwcf.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tnb.hammf.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tph.hammf.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ksh.nwbrower.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lzl.shanyushiyangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://djz.fktsv.cn

Ruby: s.bytesize;  s.length
来源：http://alo.sxryk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://azr.aibaodan.cn

================================================================================
来源：http://geo.ivvv.top

F. 文件与目录
来源：http://mxd.shzxlz.cn

================================================================================
来源：http://rea.jqgufenzy.top

[F01] 读取整个文件
来源：http://zcd.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nuf.wangshuangyany.cn

PHP:  file_get_contents("a.txt");
来源：http://hik.316326.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blu.xziqi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ffd.hesvh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://new.xziqi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dlm.shangyingyoupin.top

Ruby: File.read("a.txt")
来源：http://qpy.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://fpm.xuanzx.com

[F02] 逐行读取文件
来源：http://poi.fengsongda.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ier.guowangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eti.ppjwa.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nwl.cashguo.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zff.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ukk.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rdg.gaohongyu789.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kne.gotoacloud.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fbf.yonumen.top

[F03] 写入文件（覆盖）
来源：http://guf.fktsv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hug.ivvv.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nur.yongpay.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cks.yangfankeji.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rdg.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tyk.hywenlv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ywt.aizwys.cn

Ruby: File.write("a.txt", "hi")
来源：http://ped.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zjc.yanxiufei.cn

[F04] 追加写入文件
来源：http://kwm.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eme.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lox.kuanghao11.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fwb.zycfv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gsg.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ope.chenlongwang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dal.fengsongda.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xcz.aizwys.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://reh.sysykeji.top

[F05] 判断文件或目录是否存在
来源：http://eab.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wiv.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://wic.havefunace.top

JS:   fs.existsSync("a.txt")
来源：http://dmc.iojbl.cn

TS:   fs.existsSync("a.txt")
来源：http://vgq.yonumen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cmg.9152youxi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zcu.jinqigufen.top

Ruby: File.exist?("a.txt")
来源：http://wmj.gotoacloud.top

C#:   File.Exists("a.txt")
来源：http://awk.cdnleiting.top

[F06] 删除文件
来源：http://shn.zhixingplan.top

Py:   os.remove("a.txt")
来源：http://xya.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://thc.pengpengdd.cyou

JS:   fs.unlinkSync("a.txt")
来源：http://rzc.meibo888.top

TS:   fs.unlinkSync("a.txt")
来源：http://hdd.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yzu.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://ntr.redwolf501.top

Ruby: File.delete("a.txt")
来源：http://hkl.hysaishi.cn

C#:   File.Delete("a.txt");
来源：http://oem.yvedp.cn

[F07] 创建目录（含多级）
来源：http://xth.316326.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kpx.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tyv.bbcook.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tui.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yzr.guannengcc.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://llx.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vji.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kwy.yangfankeji.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nvr.daxiang520.top

[F08] 遍历目录
来源：http://qxs.xuetiantiany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zod.ybcxt.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://brp.fengsongda.top

JS:   fs.readdirSync("dir")
来源：http://nhv.aibaodan.cn

TS:   fs.readdirSync("dir")
来源：http://cxo.yj20258888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wjz.haohaochexian.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mdu.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://jug.xziqi.cn

C#:   Directory.GetFiles("dir")
来源：http://hvq.chenzaomai.com

[F09] 获取文件大小
来源：http://dvd.sxryk.cn

Py:   os.path.getsize("a.txt")
来源：http://bwv.sweek.top

PHP:  filesize("a.txt");
来源：http://dab.yanxiufei.cn

JS:   fs.statSync("a.txt").size
来源：http://cdf.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://tqm.ydjk.org.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xng.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zgj.0kj1m.cn

Ruby: File.size("a.txt")
来源：http://wzq.smart0.xyz

C#:   new FileInfo("a.txt").Length
来源：http://jdb.xziqi.cn

[F10] 取文件扩展名 / 文件名
来源：http://xiv.chenzaomai.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dzb.dianchejie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jbd.ivvv.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lxm.nanxinkj.top

TS:   path.extname("a.txt")
来源：http://ppd.pycfn.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ems.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zsz.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bpw.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lzm.ydzc1.top

[F11] 复制与移动文件
来源：http://xpm.epnwcf.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ngf.sweek.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uqr.yongpay.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://syj.zhongyouzk.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pmv.kuanghao11.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dqr.fengsongda.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://twi.yvedp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tup.meibo888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xkh.pengpengdd.cyou

[F12] CSV 读写
来源：http://jwl.feifeiyinyue.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xxb.jianghu66.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ycf.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mea.zhaomingkeji.xyz

TS:   // 同上
来源：http://hjc.hfpthk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kuf.yj202588.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://egj.aibaodan.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jvu.shanyushiyangtech.top

C#:   // 无内置：用 CsvHelper 库
来源：http://awl.xziqi.cn

================================================================================
来源：http://zef.gotoacloud.top

G. 面向对象
来源：http://dgk.yanxiufei.cn

================================================================================
来源：http://moy.gogol.net.cn

[G01] 定义类
来源：http://ypb.fzhhl.top

Py:   class User: pass
来源：http://mvg.jqgufenzy.top

PHP:  class User {}
来源：http://opq.bjfxy.top

JS:   class User {}
来源：http://pri.ydzc1.top

TS:   class User { name: string = ""; }
来源：http://fac.pycfn.com

Java: class User {}
来源：http://sfq.fzhhl.top

Go:   type User struct { Name string }
来源：http://jml.fengsongda.top

Ruby: class User; end
来源：http://wcz.wangshuangyany.cn

C#:   class User {}
来源：http://gmp.yonumen.top

[G02] 构造函数
来源：http://pmf.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://csq.xuanzx.com

PHP:  public function __construct(public string $name) {}
来源：http://lnz.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://kjf.sweek.top

TS:   constructor(public name: string) {}
来源：http://iph.jinyuanbaomall.cn

Java: User(String name) { this.name = name; }
来源：http://fnn.wangshuangyany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://smm.hcnkem.com

Ruby: def initialize(name); @name = name; end
来源：http://wjt.316326.xyz

C#:   public User(string name) { Name = name; }
来源：http://org.zycfv.cn

[G03] 实例属性
来源：http://agt.vehdjk.com

Py:   self.name = "x"
来源：http://von.kuanghao11.cn

PHP:  public string $name = "x";
来源：http://ezs.ywan-chungtsiang.top

JS:   this.name = "x";
来源：http://plj.pycfn.com

TS:   name: string = "x";
来源：http://pkd.pengpengdd.cyou

Java: private String name;
来源：http://iru.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nzo.aibaodan.cn

Ruby: @name = "x"
来源：http://yzo.tian-w.cn

C#:   public string Name { get; set; } = "x";
来源：http://brh.zhijiandao.cn

[G04] 定义方法
来源：http://pbn.jqgfzy.top

Py:   def greet(self): return self.name
来源：http://ltc.dianchejie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oxl.yj202588.top

JS:   greet() { return this.name; }
来源：http://iwk.chenzaomai.com

TS:   greet(): string { return this.name; }
来源：http://dkx.jinghuilouyu.cn

Java: String greet() { return name; }
来源：http://ckg.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://iri.chenlongwang.top

Ruby: def greet; @name; end
来源：http://azo.0kj1m.cn

C#:   public string Greet() => Name;
来源：http://pzx.feifeiyinyue.top

[G05] 继承
来源：http://knk.vqdsnc.cn

Py:   class Admin(User): pass
来源：http://mto.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://cyr.havefunace.top

JS:   class Admin extends User {}
来源：http://ahs.uphjek.com

TS:   class Admin extends User {}
来源：http://ebc.jiagoushi.top

Java: class Admin extends User {}
来源：http://uyk.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fvb.c1oappe.top

Ruby: class Admin < User; end
来源：http://jcb.316326.xyz

C#:   class Admin : User {}
来源：http://dja.dianchejie.cn

[G06] 重写方法
来源：http://wdy.sufxvd.cn

Py:   def greet(self): return "admin"
来源：http://qog.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qqd.aibaodan.cn

JS:   greet() { return "admin"; }
来源：http://sbw.yj202588.top

TS:   greet(): string { return "admin"; }
来源：http://xoo.chenlongwang.top

Java: @Override String greet() { return "admin"; }
来源：http://ekx.bjfxy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jbs.ydjk.org.cn

Ruby: def greet; "admin"; end
来源：http://vwj.52xcode.cn

C#:   public override string Greet() => "admin";
来源：http://iya.zhaomingkeji.xyz

[G07] 调用父类方法
来源：http://zzu.andypj.xyz

Py:   super().greet()
来源：http://tkb.9152youxi.cn

PHP:  parent::greet();
来源：http://tsw.jqgufenzy.top

JS:   super.greet();
来源：http://uqj.smart0.xyz

TS:   super.greet();
来源：http://iuf.havefunace.top

Java: super.greet();
来源：http://gas.epnwcf.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wes.0kj1m.cn

Ruby: super
来源：http://kut.bbcook.cn

C#:   base.Greet();
来源：http://art.jqgfzy.top

[G08] 静态方法与属性
来源：http://yqe.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fii.yuanzhike.top

PHP:  public static function f() {}
来源：http://ihp.chenjidiqi.icu

JS:   static f() {}
来源：http://cyh.jinghuilouyu.cn

TS:   static f(): void {}
来源：http://jft.cdnleiting.top

Java: static void f() {}
来源：http://lbm.ivvv.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ftd.gotoacloud.top

Ruby: def self.f; end
来源：http://ork.svipenyu.cn

C#:   public static void F() {}
来源：http://iyk.shanyushiyangtech.top

[G09] 接口 / 抽象类
来源：http://alm.fengsongda.top

Py:   from abc import ABC, abstractmethod
来源：http://gbw.xuetiantiany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ali.chenlongwang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cbb.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://vnz.zdbjq.cn

Java: interface Shape { double area(); }
来源：http://iio.aibaodan.cn

Go:   type Shape interface { Area() float64 }
来源：http://fue.cheryme.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pqt.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://mzh.haohaochexian.top

[G10] 访问控制
来源：http://tor.jinqigufen.top

Py:   约定 _protected / __private（不强制）
来源：http://yup.ydjk.org.cn

PHP:  public / protected / private
来源：http://dlt.jqgufenzy.top

JS:   #private 字段；其余公开
来源：http://ykm.cashguo.top

TS:   public / protected / private
来源：http://pjq.jqgfzy.top

Java: public / protected / private / 默认包级
来源：http://vsy.shanyushiyangtech.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kcy.epnwcf.com

Ruby: public / protected / private
来源：http://puf.dashuyun.cn

C#:   public / protected / private / internal
来源：http://inv.tian-w.cn

[G11] getter / setter
来源：http://xof.dianchejie.cn

Py:   @property 与 @x.setter
来源：http://jpd.xylfe.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vin.zhongyouzk.top

JS:   get name() { return this._name; }
来源：http://szf.tian-w.cn

TS:   get name(): string { return this._name; }
来源：http://okm.jinghuilouyu.cn

Java: public String getName() { return name; }
来源：http://idd.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://qbc.hongshengwenyu.top

Ruby: attr_accessor :name
来源：http://mnu.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://sdp.zhiwuduotai.top

[G12] 对象转字符串
来源：http://ale.shanyushiyangkeji.top

Py:   def __str__(self): return self.name
来源：http://prz.52xcode.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mjz.yfazqb.com

JS:   toString() { return this.name; }
来源：http://zch.tanke756.top

TS:   toString(): string { return this.name; }
来源：http://vcm.guannengcc.top

Java: @Override public String toString() { return name; }
来源：http://fvh.316326.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://xij.ivvv.top

Ruby: def to_s; @name; end
来源：http://qha.hongshengwenyu.top

C#:   public override string ToString() => Name;
来源：http://nzx.feifeiyinyue.top

[G13] 判断对象类型
来源：http://rxi.yuanzhike.top

Py:   isinstance(u, User)
来源：http://cdj.dianchejie.cn

PHP:  $u instanceof User
来源：http://gbf.shanyushiyangtech.top

JS:   u instanceof User
来源：http://ubn.sxryk.cn

TS:   u instanceof User
来源：http://fas.zdbjq.cn

Java: u instanceof User
来源：http://jai.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mtm.daria6918.cn

Ruby: u.is_a?(User)
来源：http://ase.yj20258888.top

C#:   u is User
来源：http://ghs.jinghuilouyu.cn

[G14] 数据类 / record
来源：http://tmh.yueranfly.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cxn.yj20258.top

PHP:  // 用 readonly 属性模拟
来源：http://dri.cucudq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://len.jinqigufen.top

TS:   type User = { name: string; age: number };
来源：http://sib.xylfe.cn

Java: record User(String name, int age) {}
来源：http://wif.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://lkv.yuxming.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ihc.hysaishi.cn

C#:   record User(string Name, int Age);
来源：http://kvx.nanxinkj.top

[G15] 枚举
来源：http://ktl.iojbl.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://njo.chenlongwang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qha.meibo888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://djg.chenjidiqi.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xfs.kuanghao11.cn

Java: enum Color { RED, GREEN }
来源：http://sfy.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fho.snrcjt.cn


<!-- 参考信息 -->