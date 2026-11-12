代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yio.ppjwa.cn

Go:   // 按 rune 判断长度后截断
来源：http://ytk.ybcxt.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gla.ywan-chungtsiang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ggd.yuanzhike.top

[E22] 字节长度与字符长度
来源：http://fgn.aizwys.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iqj.tian-w.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ksg.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://shi.sxryk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sok.hnqzz.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hel.fanxiaobao.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qmn.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://hoj.cashguo.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vcd.xziqi.cn

================================================================================
来源：http://vuv.jqgfzy.top

F. 文件与目录
来源：http://ezi.vehdjk.com

================================================================================
来源：http://gnw.shzxlz.cn

[F01] 读取整个文件
来源：http://odx.andypj.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oyi.guowangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://kut.yj202588.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eph.meibo888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mbl.quarkkingdee.top

Java: Files.readString(Path.of("a.txt"))
来源：http://iai.shanyushiyangtech.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kqm.hesvh.cn

Ruby: File.read("a.txt")
来源：http://brl.zhaomingkeji.xyz

C#:   File.ReadAllText("a.txt");
来源：http://lrm.316326.xyz

[F02] 逐行读取文件
来源：http://jpf.52xcode.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ohi.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bgn.nanxinkj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://csw.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xig.guowangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vdq.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qhu.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://skt.snrcjt.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tag.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://yrw.shanyushiyangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qbo.kuanghao11.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dij.nanxuanxn.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dbi.redwolf501.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mow.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hkr.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pqv.bbcook.cn

Ruby: File.write("a.txt", "hi")
来源：http://rfy.chenzaomai.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://miu.shanyushiyangtech.top

[F04] 追加写入文件
来源：http://jcp.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://boa.cdnleiting.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rgk.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zoj.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bpt.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kqz.yongpay.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nog.kuanghao11.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eow.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sxo.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://qtl.yanxiufei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ibz.9152youxi.cn

PHP:  file_exists("a.txt");
来源：http://jkk.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://pri.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://nyo.quarkkingdee.top

Java: Files.exists(Path.of("a.txt"))
来源：http://toa.zhiwuduotai.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aby.havefunace.top

Ruby: File.exist?("a.txt")
来源：http://fqj.hfpthk.cn

C#:   File.Exists("a.txt")
来源：http://jja.hysaishi.cn

[F06] 删除文件
来源：http://tae.zhijiandao.cn

Py:   os.remove("a.txt")
来源：http://lmr.yj20258888.top

PHP:  unlink("a.txt");
来源：http://pbi.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://sdn.yfazqb.com

TS:   fs.unlinkSync("a.txt")
来源：http://fyj.tian-w.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gml.shanyushiyangkeji.top

Go:   os.Remove("a.txt")
来源：http://zxo.ctjpmb.com

Ruby: File.delete("a.txt")
来源：http://xzx.zhoulong.xyz

C#:   File.Delete("a.txt");
来源：http://zsg.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://fjd.svipenyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nap.dianchejie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yln.meibo888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rvu.haohaochexian.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uon.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kqe.sxryk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ord.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mlz.aizwys.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uts.pengpengdd.cyou

[F08] 遍历目录
来源：http://pzb.zdbjq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zpk.jiagoushi.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ikt.nwbrower.top

JS:   fs.readdirSync("dir")
来源：http://rls.xylfe.cn

TS:   fs.readdirSync("dir")
来源：http://aoz.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://amq.shangyingyoupin.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dth.chenlongwang.top

Ruby: Dir.children("dir")
来源：http://rpv.shanyushiyangtech.top

C#:   Directory.GetFiles("dir")
来源：http://qqv.zdqjudy.top

[F09] 获取文件大小
来源：http://evu.yvedp.cn

Py:   os.path.getsize("a.txt")
来源：http://wms.feifeiyinyue.top

PHP:  filesize("a.txt");
来源：http://wur.ppjwa.cn

JS:   fs.statSync("a.txt").size
来源：http://qwg.shzxlz.cn

TS:   fs.statSync("a.txt").size
来源：http://cst.hesvh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://deb.xylfe.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://goi.havefunace.top

Ruby: File.size("a.txt")
来源：http://now.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://fvv.hnxiangtu.top

[F10] 取文件扩展名 / 文件名
来源：http://wyh.wangdashe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qsv.aizwys.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ewq.shangyingyoupin.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ymu.xingfuxueyuan.xyz

TS:   path.extname("a.txt")
来源：http://iva.haohaochexian.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://efv.sweek.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tip.havefunace.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jpg.jinghuilouyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qbj.52xcode.cn

[F11] 复制与移动文件
来源：http://jsa.yj202588.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://drx.yangfankeji.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mom.gaohongyu789.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gxc.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yjl.jianghu66.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dci.birdmap.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mav.uphjek.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://btg.aizwys.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mgj.yanxiufei.cn

[F12] CSV 读写
来源：http://ici.zdqjudy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zjm.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cup.hcnkem.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://shg.pycfn.com

TS:   // 同上
来源：http://rnb.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eqk.ydzc1.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gvi.gzhubu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mea.xylfe.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mzp.ydjk.org.cn

================================================================================
来源：http://cpc.yfazqb.com

G. 面向对象
来源：http://zyq.kuanghao11.cn

================================================================================
来源：http://edx.yonumen.top

[G01] 定义类
来源：http://bje.ppjwa.cn

Py:   class User: pass
来源：http://kdt.tarul.cn

PHP:  class User {}
来源：http://jxv.fengsongda.top

JS:   class User {}
来源：http://cvt.yj202588.top

TS:   class User { name: string = ""; }
来源：http://hnr.feifeiyinyue.top

Java: class User {}
来源：http://znc.pycfn.com

Go:   type User struct { Name string }
来源：http://kxz.yueranfly.top

Ruby: class User; end
来源：http://lyv.jyoumei.cn

C#:   class User {}
来源：http://mog.pengpengdd.cyou

[G02] 构造函数
来源：http://tss.nwbrower.top

Py:   def __init__(self, name): self.name = name
来源：http://ckg.sxryk.cn

PHP:  public function __construct(public string $name) {}
来源：http://ush.zhoulong.xyz

JS:   constructor(name) { this.name = name; }
来源：http://zue.sxryk.cn

TS:   constructor(public name: string) {}
来源：http://rjy.andypj.xyz

Java: User(String name) { this.name = name; }
来源：http://tkf.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xzc.0kj1m.cn

Ruby: def initialize(name); @name = name; end
来源：http://zss.xylfe.cn

C#:   public User(string name) { Name = name; }
来源：http://sop.wangdashe.top

[G03] 实例属性
来源：http://wnr.zycfv.cn

Py:   self.name = "x"
来源：http://uar.aibaodan.cn

PHP:  public string $name = "x";
来源：http://exw.tian-w.cn

JS:   this.name = "x";
来源：http://fao.nwbrower.top

TS:   name: string = "x";
来源：http://hxz.tanke756.top

Java: private String name;
来源：http://pvc.fktsv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fts.xinyue.icu

Ruby: @name = "x"
来源：http://ubi.yanxiufei.cn

C#:   public string Name { get; set; } = "x";
来源：http://wdx.jianghu66.top

[G04] 定义方法
来源：http://uck.hongshengwenyu.top

Py:   def greet(self): return self.name
来源：http://hpn.smart0.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://wsd.uphjek.com

JS:   greet() { return this.name; }
来源：http://any.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://ntj.quarkkingdee.top

Java: String greet() { return name; }
来源：http://bot.zhaomingkeji.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://mtx.xinyue.icu

Ruby: def greet; @name; end
来源：http://gjw.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://vjd.xylfe.cn

[G05] 继承
来源：http://jkj.ehwqpu.com

Py:   class Admin(User): pass
来源：http://lft.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://cfs.hcnkem.com

JS:   class Admin extends User {}
来源：http://nmg.yanxiufei.cn

TS:   class Admin extends User {}
来源：http://jez.shzxlz.cn

Java: class Admin extends User {}
来源：http://rbb.yangfankeji.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hps.cheryme.top

Ruby: class Admin < User; end
来源：http://iym.hnxiangtu.top

C#:   class Admin : User {}
来源：http://zjr.yj20258888.top

[G06] 重写方法
来源：http://zwu.hnqzz.top

Py:   def greet(self): return "admin"
来源：http://fyr.svipenyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vmg.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://ayw.smart0.xyz

TS:   greet(): string { return "admin"; }
来源：http://gop.gzhubu.top

Java: @Override String greet() { return "admin"; }
来源：http://qnp.cucudq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ypj.hcnkem.com

Ruby: def greet; "admin"; end
来源：http://qkh.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://adi.tanke756.top

[G07] 调用父类方法
来源：http://tnr.hfpthk.cn

Py:   super().greet()
来源：http://yjt.yj20258.top

PHP:  parent::greet();
来源：http://idb.ppjwa.cn

JS:   super.greet();
来源：http://uem.meibo888.top

TS:   super.greet();
来源：http://asf.fzhhl.top

Java: super.greet();
来源：http://zex.shanyushiyangkeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ual.hysaishi.cn

Ruby: super
来源：http://ggq.nwbrower.top

C#:   base.Greet();
来源：http://rma.yanxiufei.cn

[G08] 静态方法与属性
来源：http://xkt.yueranfly.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mec.quarkkingdee.top

PHP:  public static function f() {}
来源：http://foo.xuanzx.com

JS:   static f() {}
来源：http://tpd.dashuyun.cn

TS:   static f(): void {}
来源：http://irj.smart0.xyz

Java: static void f() {}
来源：http://xlh.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://hud.fehbvm.com

Ruby: def self.f; end
来源：http://ieb.yfazqb.com

C#:   public static void F() {}
来源：http://zqq.pengpengdd.cyou

[G09] 接口 / 抽象类
来源：http://idp.mhx1999.top

Py:   from abc import ABC, abstractmethod
来源：http://ijk.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ygg.epnwcf.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://hgv.shanyushiyangtech.top

TS:   interface Shape { area(): number; }
来源：http://ukq.tarul.cn

Java: interface Shape { double area(); }
来源：http://tgi.yonumen.top

Go:   type Shape interface { Area() float64 }
来源：http://zil.xuetiantiany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wff.aizwys.cn

C#:   interface IShape { double Area(); }
来源：http://let.yj202588.top

[G10] 访问控制
来源：http://qko.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://lgi.ybcxt.top

PHP:  public / protected / private
来源：http://hye.ctjpmb.com

JS:   #private 字段；其余公开
来源：http://gij.yangfankeji.com

TS:   public / protected / private
来源：http://vfj.shzxlz.cn

Java: public / protected / private / 默认包级
来源：http://tvs.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ekq.ctjpmb.com

Ruby: public / protected / private
来源：http://lsp.chenlongwang.top

C#:   public / protected / private / internal
来源：http://ysr.shuidangran.top

[G11] getter / setter
来源：http://gdq.gotoacloud.top

Py:   @property 与 @x.setter
来源：http://xfm.jinyuanbaomall.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vxh.kuanghao11.cn

JS:   get name() { return this._name; }
来源：http://wvb.svipenyu.cn

TS:   get name(): string { return this._name; }
来源：http://elx.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://fpp.jqgufenzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xzo.epnwcf.com

Ruby: attr_accessor :name
来源：http://fmm.guannengcc.top

C#:   public string Name { get; set; }
来源：http://qse.fktsv.cn

[G12] 对象转字符串
来源：http://ppt.wangdashe.top

Py:   def __str__(self): return self.name
来源：http://hpm.52xcode.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://blx.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://syt.tian-w.cn

TS:   toString(): string { return this.name; }
来源：http://jah.tian-w.cn

Java: @Override public String toString() { return name; }
来源：http://tsk.yj202588.top

Go:   func (u User) String() string { return u.Name }
来源：http://ulf.tarul.cn

Ruby: def to_s; @name; end
来源：http://exj.fehbvm.com

C#:   public override string ToString() => Name;
来源：http://yhc.yuanzhike.top

[G13] 判断对象类型
来源：http://iqd.xuanzx.com

Py:   isinstance(u, User)
来源：http://cpf.yonumen.top

PHP:  $u instanceof User
来源：http://jvt.yfazqb.com

JS:   u instanceof User
来源：http://wkn.jyoumei.cn

TS:   u instanceof User
来源：http://nfw.hywenlv.cn

Java: u instanceof User
来源：http://kkz.meibo888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zuh.haohaochexian.top

Ruby: u.is_a?(User)
来源：http://xsy.cheryme.top

C#:   u is User
来源：http://cls.havefunace.top

[G14] 数据类 / record
来源：http://rmo.chenzaomai.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ihw.sxryk.cn

PHP:  // 用 readonly 属性模拟
来源：http://oka.316326.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://wmp.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://bhp.tianlin.xyz

Java: record User(String name, int age) {}
来源：http://xes.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://ddi.cheryme.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pjo.jiagoushi.top

C#:   record User(string Name, int Age);
来源：http://zsh.yj202588.top

[G15] 枚举
来源：http://wpw.yuxming.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hgf.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://ban.kuanghao11.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wln.fanxiaobao.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iej.sufxvd.cn

Java: enum Color { RED, GREEN }
来源：http://gdh.shanyushiyangtech.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pen.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://jwa.birdmap.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xjs.jinqigufen.top

[G16] 对象转数组 / 字典
来源：http://aai.cqqwz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dhd.cucudq.cn

PHP:  get_object_vars($obj);
来源：http://nzy.zdqjudy.top

JS:   Object.entries(obj)
来源：http://zuc.guowangkeji.top

TS:   Object.entries(obj)
来源：http://ezu.xylfe.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hpt.dianchejie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rbo.vehdjk.com

Ruby: obj.instance_variables
来源：http://ryn.shanyushiyangtech.top

C#:   // 用反射或 System.Text.Json
来源：http://ijw.haohaochexian.top

================================================================================
来源：http://jfn.nwbrower.top

H. 异常与错误处理
来源：http://ncv.yfazqb.com

================================================================================
来源：http://uqr.hfpthk.cn

[H01] try / catch 基础
来源：http://iwg.jlsjyb.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ujp.jlsjyb.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rpk.epnwcf.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fcy.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://elq.fengsongda.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sui.aibaodan.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oez.bbcook.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hmg.gzhubu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://weh.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://mmx.zhixingplan.top

Py:   try: f()⏎finally: cleanup()
来源：http://sva.gotoacloud.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ceu.mhx1999.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qzw.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yfi.yongpay.top

Java: try { f(); } finally { cleanup(); }
来源：http://uhi.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cfu.wangdashe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zff.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://slf.yj202588.top

[H03] 主动抛出异常
来源：http://rrv.hywenlv.cn

Py:   raise ValueError("错误信息")
来源：http://kmy.ctjpmb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lcw.gzhubu.top

JS:   throw new Error("错误信息");
来源：http://qbr.yuxming.cn

TS:   throw new Error("错误信息");
来源：http://olj.jinqigufen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bac.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lyi.yuanzhike.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bpp.yanxiufei.cn


<!-- 参考信息 -->