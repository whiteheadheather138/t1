代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gpk.jyoumei.cn

Go:   // 按 rune 判断长度后截断
来源：http://aso.yj20258.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rbk.dashuyun.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://anf.yj20258.top

[E22] 字节长度与字符长度
来源：http://prp.daria6918.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pmt.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jhp.daxiang520.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gas.birdmap.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yxw.zhiwuduotai.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yhf.nanxinkj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yiv.zhoulong.xyz

Ruby: s.bytesize;  s.length
来源：http://uie.zhaomingkeji.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hfc.xuanzx.com

================================================================================
来源：http://xtb.bjfxy.top

F. 文件与目录
来源：http://ujo.hywenlv.cn

================================================================================
来源：http://msa.andypj.xyz

[F01] 读取整个文件
来源：http://rfo.chenzaomai.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://clm.chenlongwang.top

PHP:  file_get_contents("a.txt");
来源：http://nkd.cdnleiting.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fjx.cdnleiting.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cfk.quarkkingdee.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lvo.yueranfly.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qww.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://miu.hywenlv.cn

C#:   File.ReadAllText("a.txt");
来源：http://yul.shzxlz.cn

[F02] 逐行读取文件
来源：http://apk.feifeiyinyue.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wqt.havefunace.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ddu.ivvv.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ntm.yuxming.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yyr.svipenyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wly.jinghuilouyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wwi.ybcxt.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://szs.zhijiandao.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fbl.jinyuanbaomall.cn

[F03] 写入文件（覆盖）
来源：http://ymn.shzxlz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ofo.hnxiangtu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rub.epnwcf.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fmn.52xcode.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yim.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ple.yj20258888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hfp.ivvv.top

Ruby: File.write("a.txt", "hi")
来源：http://nee.snrcjt.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ciy.epnwcf.com

[F04] 追加写入文件
来源：http://yim.sweek.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wba.sweek.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://llb.zhengqikj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jpt.haohaochexian.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mtx.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cka.pengpengdd.cyou

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://twz.fengsongda.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dyl.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://woz.yanxiufei.cn

[F05] 判断文件或目录是否存在
来源：http://cwk.sweek.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://htx.jqgufenzy.top

PHP:  file_exists("a.txt");
来源：http://vty.nanxuanxn.top

JS:   fs.existsSync("a.txt")
来源：http://cow.gaohongyu789.top

TS:   fs.existsSync("a.txt")
来源：http://afa.iojbl.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hcr.jianghu66.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://toc.316326.xyz

Ruby: File.exist?("a.txt")
来源：http://lpi.zhongyouzk.top

C#:   File.Exists("a.txt")
来源：http://rwm.bbcook.cn

[F06] 删除文件
来源：http://exr.ehwqpu.com

Py:   os.remove("a.txt")
来源：http://byv.kuanghao11.cn

PHP:  unlink("a.txt");
来源：http://sbg.jiagoushi.top

JS:   fs.unlinkSync("a.txt")
来源：http://jll.epnwcf.com

TS:   fs.unlinkSync("a.txt")
来源：http://zip.fzhhl.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vzc.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://qft.ehwqpu.com

Ruby: File.delete("a.txt")
来源：http://rog.cashguo.top

C#:   File.Delete("a.txt");
来源：http://suj.hnqzz.top

[F07] 创建目录（含多级）
来源：http://glg.nanxinkj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vps.yj202588.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zdj.iojbl.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ffk.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kcd.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bgq.tarul.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hiz.shangyingyoupin.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tfv.dianchejie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kwz.cucudq.cn

[F08] 遍历目录
来源：http://ood.ydzc1.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wma.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ujl.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://qru.andypj.xyz

TS:   fs.readdirSync("dir")
来源：http://vut.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gjh.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wgx.hammf.cn

Ruby: Dir.children("dir")
来源：http://uwr.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://prp.nanxuanxn.top

[F09] 获取文件大小
来源：http://rdk.yangfankeji.com

Py:   os.path.getsize("a.txt")
来源：http://jwg.zycfv.cn

PHP:  filesize("a.txt");
来源：http://ixp.havefunace.top

JS:   fs.statSync("a.txt").size
来源：http://ssx.ehwqpu.com

TS:   fs.statSync("a.txt").size
来源：http://qyi.aizwys.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lfj.tarul.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ltc.sjlbkw.cn

Ruby: File.size("a.txt")
来源：http://yvc.9152youxi.cn

C#:   new FileInfo("a.txt").Length
来源：http://ksi.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://mba.yvedp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dcl.ydjk.org.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://agi.redwolf501.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://piq.zhiwuduotai.top

TS:   path.extname("a.txt")
来源：http://piw.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tbm.sxryk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jwt.ydjk.org.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://war.c1oappe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ziv.aizwys.cn

[F11] 复制与移动文件
来源：http://cjh.vehdjk.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iaw.hysaishi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uoc.yonumen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mtj.jqgufenzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rmp.xuanzx.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sdi.xinyue.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ytx.hcnkem.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jff.uphjek.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://acc.jinghuilouyu.cn

[F12] CSV 读写
来源：http://eik.zdbjq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mpg.vehdjk.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lfe.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sfw.nanxuanxn.top

TS:   // 同上
来源：http://gxp.tianlin.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yrp.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nfg.andypj.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mrw.zdqjudy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zjn.aibaodan.cn

================================================================================
来源：http://ddp.zhoulong.xyz

G. 面向对象
来源：http://ayj.jinqigufen.top

================================================================================
来源：http://alj.aibaodan.cn

[G01] 定义类
来源：http://alr.shanyushiyangtech.top

Py:   class User: pass
来源：http://kvu.chenlongwang.top

PHP:  class User {}
来源：http://rlc.guannengcc.top

JS:   class User {}
来源：http://luj.zhaomingkeji.xyz

TS:   class User { name: string = ""; }
来源：http://zpk.chenzaomai.com

Java: class User {}
来源：http://fuj.zycfv.cn

Go:   type User struct { Name string }
来源：http://cjf.jyoumei.cn

Ruby: class User; end
来源：http://pwr.9152youxi.cn

C#:   class User {}
来源：http://ujs.c1oappe.top

[G02] 构造函数
来源：http://auc.shzxlz.cn

Py:   def __init__(self, name): self.name = name
来源：http://pwr.zhixingplan.top

PHP:  public function __construct(public string $name) {}
来源：http://vbb.aizwys.cn

JS:   constructor(name) { this.name = name; }
来源：http://pmi.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://ryu.vehdjk.com

Java: User(String name) { this.name = name; }
来源：http://bsv.xuetiantiany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gkc.zhixingplan.top

Ruby: def initialize(name); @name = name; end
来源：http://ala.yvedp.cn

C#:   public User(string name) { Name = name; }
来源：http://ntj.hammf.cn

[G03] 实例属性
来源：http://psb.nwbrower.top

Py:   self.name = "x"
来源：http://bqo.xylfe.cn

PHP:  public string $name = "x";
来源：http://jcw.jqgufenzy.top

JS:   this.name = "x";
来源：http://qoo.cashguo.top

TS:   name: string = "x";
来源：http://tks.svipenyu.cn

Java: private String name;
来源：http://oxu.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kpx.daxiang520.top

Ruby: @name = "x"
来源：http://aay.fktsv.cn

C#:   public string Name { get; set; } = "x";
来源：http://oir.hammf.cn

[G04] 定义方法
来源：http://kgr.gogol.net.cn

Py:   def greet(self): return self.name
来源：http://ser.kuanghao11.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://epn.hcnkem.com

JS:   greet() { return this.name; }
来源：http://mni.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://edi.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://ajs.yj20258.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mho.sysykeji.top

Ruby: def greet; @name; end
来源：http://ati.xinyue.icu

C#:   public string Greet() => Name;
来源：http://swm.yangfankeji.com

[G05] 继承
来源：http://taa.hongshengwenyu.top

Py:   class Admin(User): pass
来源：http://byb.hnqzz.top

PHP:  class Admin extends User {}
来源：http://mbe.zdbjq.cn

JS:   class Admin extends User {}
来源：http://fcl.gogol.net.cn

TS:   class Admin extends User {}
来源：http://tsd.sxryk.cn

Java: class Admin extends User {}
来源：http://kzv.hywenlv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vvi.jqgfzy.top

Ruby: class Admin < User; end
来源：http://uhw.cheryme.top

C#:   class Admin : User {}
来源：http://jgx.pengpengdd.cyou

[G06] 重写方法
来源：http://aja.xinyue.icu

Py:   def greet(self): return "admin"
来源：http://jdi.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://uxu.ywan-chungtsiang.top

JS:   greet() { return "admin"; }
来源：http://qiq.vqdsnc.cn

TS:   greet(): string { return "admin"; }
来源：http://bxj.cdnleiting.top

Java: @Override String greet() { return "admin"; }
来源：http://xqn.hfpthk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ptp.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://sey.daxiang520.top

C#:   public override string Greet() => "admin";
来源：http://iso.zhijiandao.cn

[G07] 调用父类方法
来源：http://lsb.bbcook.cn

Py:   super().greet()
来源：http://zfa.kuanghao11.cn

PHP:  parent::greet();
来源：http://onp.redwolf501.top

JS:   super.greet();
来源：http://frl.yongpay.top

TS:   super.greet();
来源：http://nut.quarkkingdee.top

Java: super.greet();
来源：http://ozf.52xcode.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xly.9152youxi.cn

Ruby: super
来源：http://gwh.zdbjq.cn

C#:   base.Greet();
来源：http://uzn.hongshengwenyu.top

[G08] 静态方法与属性
来源：http://mgi.jiagoushi.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dnn.jinghuilouyu.cn

PHP:  public static function f() {}
来源：http://vqq.sufxvd.cn

JS:   static f() {}
来源：http://vla.nanxuanxn.top

TS:   static f(): void {}
来源：http://gxa.zdqjudy.top

Java: static void f() {}
来源：http://znn.jiagoushi.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sfo.ctjpmb.com

Ruby: def self.f; end
来源：http://lwo.guannengcc.top

C#:   public static void F() {}
来源：http://sps.ppjwa.cn

[G09] 接口 / 抽象类
来源：http://zds.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://aja.yueranfly.top

PHP:  interface Shape { public function area(): float; }
来源：http://ucf.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://buq.hfpthk.cn

TS:   interface Shape { area(): number; }
来源：http://ovs.hysaishi.cn

Java: interface Shape { double area(); }
来源：http://tgz.aibaodan.cn

Go:   type Shape interface { Area() float64 }
来源：http://xaf.pycfn.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pdd.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://lew.aibaodan.cn

[G10] 访问控制
来源：http://pmp.sysykeji.top

Py:   约定 _protected / __private（不强制）
来源：http://vaj.epnwcf.com

PHP:  public / protected / private
来源：http://kua.ctjpmb.com

JS:   #private 字段；其余公开
来源：http://xxr.snrcjt.cn

TS:   public / protected / private
来源：http://uwj.ydzc1.top

Java: public / protected / private / 默认包级
来源：http://dww.xuetiantiany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sbt.cqqwz.cn

Ruby: public / protected / private
来源：http://qrm.xziqi.cn

C#:   public / protected / private / internal
来源：http://ocy.jinqigufen.top

[G11] getter / setter
来源：http://lgq.316326.xyz

Py:   @property 与 @x.setter
来源：http://veo.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dht.cdnleiting.top

JS:   get name() { return this._name; }
来源：http://mkn.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://bap.mhx1999.top

Java: public String getName() { return name; }
来源：http://kql.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ctt.zhongyouzk.top

Ruby: attr_accessor :name
来源：http://fng.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://wuv.snrcjt.cn

[G12] 对象转字符串
来源：http://wfp.jqgufenzy.top

Py:   def __str__(self): return self.name
来源：http://nia.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://hdu.nanxuanxn.top

JS:   toString() { return this.name; }
来源：http://eyk.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://asn.nwbrower.top

Java: @Override public String toString() { return name; }
来源：http://mxv.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wxu.shuidangran.top

Ruby: def to_s; @name; end
来源：http://kcm.zhongyouzk.top

C#:   public override string ToString() => Name;
来源：http://sls.cashguo.top

[G13] 判断对象类型
来源：http://ixs.dashuyun.cn

Py:   isinstance(u, User)
来源：http://bzb.jqgufenzy.top

PHP:  $u instanceof User
来源：http://msn.pycfn.com

JS:   u instanceof User
来源：http://zpe.tianlin.xyz

TS:   u instanceof User
来源：http://jkk.zhiwuduotai.top

Java: u instanceof User
来源：http://ikr.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hfu.andypj.xyz

Ruby: u.is_a?(User)
来源：http://vfm.zycfv.cn

C#:   u is User
来源：http://nue.jiagoushi.top

[G14] 数据类 / record
来源：http://gwr.fktsv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oam.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://ytz.hfpthk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yoc.andypj.xyz

TS:   type User = { name: string; age: number };
来源：http://tid.sjlbkw.cn

Java: record User(String name, int age) {}
来源：http://mnj.smart0.xyz

Go:   type User struct { Name string; Age int }
来源：http://scy.birdmap.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jub.hammf.cn

C#:   record User(string Name, int Age);
来源：http://xqx.zhongyouzk.top

[G15] 枚举
来源：http://tgj.fzhhl.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sgo.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://idd.c1oappe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mjq.wangshuangyany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fxk.jyoumei.cn

Java: enum Color { RED, GREEN }
来源：http://wse.fehbvm.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lot.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://iwn.yueranfly.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rzs.zhongyouzk.top

[G16] 对象转数组 / 字典
来源：http://fws.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hau.52xcode.cn

PHP:  get_object_vars($obj);
来源：http://ffh.daria6918.cn

JS:   Object.entries(obj)
来源：http://ztm.dianchejie.cn

TS:   Object.entries(obj)
来源：http://ltn.hywenlv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gpp.bjfxy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lrl.sweek.top

Ruby: obj.instance_variables
来源：http://eyi.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://tya.xingfuxueyuan.xyz

================================================================================
来源：http://dir.yongpay.top

H. 异常与错误处理
来源：http://ijk.daria6918.cn

================================================================================
来源：http://gbq.yanxiufei.cn

[H01] try / catch 基础
来源：http://qvx.yangfankeji.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ajt.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://adx.jqgfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://guv.fzhhl.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jsk.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ajd.uphjek.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kif.xylfe.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xqv.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rlh.yongpay.top

[H02] finally / ensure 收尾
来源：http://slb.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://qcr.zdbjq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vbm.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pzy.haohaochexian.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yfm.vehdjk.com

Java: try { f(); } finally { cleanup(); }
来源：http://gmg.hnqzz.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://paq.epnwcf.com

Ruby: begin; f; ensure; cleanup; end
来源：http://lax.ctjpmb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://zte.ydzc1.top

[H03] 主动抛出异常
来源：http://ypr.sjlbkw.cn

Py:   raise ValueError("错误信息")
来源：http://qrb.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vnr.iojbl.cn

JS:   throw new Error("错误信息");
来源：http://wok.zdqjudy.top

TS:   throw new Error("错误信息");
来源：http://tcz.yueranfly.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://yhe.jlsjyb.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dbx.feifeiyinyue.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vel.jinqigfzy.top


<!-- 参考信息 -->