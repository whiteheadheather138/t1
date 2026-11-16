代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qqc.jqgufenzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cye.andypj.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vrg.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://amp.52xcode.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jbq.cdnleiting.top

================================================================================
来源：http://xmg.yfazqb.com

F. 文件与目录
来源：http://dsy.jyoumei.cn

================================================================================
来源：http://ijk.meibo888.top

[F01] 读取整个文件
来源：http://khx.ppjwa.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lfa.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://upa.hcnkem.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mlq.cheryme.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dhz.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://ngt.chenlongwang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://aic.ivvv.top

Ruby: File.read("a.txt")
来源：http://tgf.shangyingyoupin.top

C#:   File.ReadAllText("a.txt");
来源：http://ecg.svipenyu.cn

[F02] 逐行读取文件
来源：http://cwv.yonumen.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tho.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://epa.sweek.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wze.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vju.yfazqb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pug.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dlo.yangfankeji.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nse.hysaishi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tlp.hcnkem.com

[F03] 写入文件（覆盖）
来源：http://tal.pycfn.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bwc.zdqjudy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rov.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fdb.shangyingyoupin.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wai.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jez.yuxming.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xud.hywenlv.cn

Ruby: File.write("a.txt", "hi")
来源：http://mvp.shanyushiyangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qvw.haohaochexian.top

[F04] 追加写入文件
来源：http://gdn.hnxiangtu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ugs.gaohongyu789.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dau.zdqjudy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jdx.ehwqpu.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jkc.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ybz.quarkkingdee.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mxl.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://flr.snrcjt.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bni.zdbjq.cn

[F05] 判断文件或目录是否存在
来源：http://myx.0kj1m.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fxk.hnqzz.top

PHP:  file_exists("a.txt");
来源：http://qqw.sjlbkw.cn

JS:   fs.existsSync("a.txt")
来源：http://cjw.shangyingyoupin.top

TS:   fs.existsSync("a.txt")
来源：http://ftk.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ipo.ivvv.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yql.epnwcf.com

Ruby: File.exist?("a.txt")
来源：http://tar.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://lli.havefunace.top

[F06] 删除文件
来源：http://vui.jinyuanbaomall.cn

Py:   os.remove("a.txt")
来源：http://cfc.meibo888.top

PHP:  unlink("a.txt");
来源：http://zkm.xingfuxueyuan.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://qvp.havefunace.top

TS:   fs.unlinkSync("a.txt")
来源：http://hrw.uphjek.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gho.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://tlm.zhijiandao.cn

Ruby: File.delete("a.txt")
来源：http://hoz.uphjek.com

C#:   File.Delete("a.txt");
来源：http://xfz.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://ssi.cqqwz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ilm.yj202588.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rjv.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xro.ehwqpu.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dvc.jyoumei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lrn.cheryme.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vlg.chenzaomai.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oyp.yuanzhike.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cia.bbcook.cn

[F08] 遍历目录
来源：http://cnv.jinyuanbaomall.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ova.ydzc1.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gat.ybcxt.top

JS:   fs.readdirSync("dir")
来源：http://qxe.smart0.xyz

TS:   fs.readdirSync("dir")
来源：http://oxj.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bst.hywenlv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gfb.tian-w.cn

Ruby: Dir.children("dir")
来源：http://tks.jinyuanbaomall.cn

C#:   Directory.GetFiles("dir")
来源：http://gll.smart0.xyz

[F09] 获取文件大小
来源：http://ubx.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://qqz.zhiwuduotai.top

PHP:  filesize("a.txt");
来源：http://wpu.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://fmg.aizwys.cn

TS:   fs.statSync("a.txt").size
来源：http://bwf.yj20258.top

Java: Files.size(Path.of("a.txt"))
来源：http://fep.yuxming.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ijn.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://err.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://yoj.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://wbz.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bvr.bbcook.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kba.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ios.hysaishi.cn

TS:   path.extname("a.txt")
来源：http://cpm.daxiang520.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pci.kuanghao11.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tsq.daxiang520.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cme.tianlin.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bfk.jqgfzy.top

[F11] 复制与移动文件
来源：http://sdp.andypj.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ule.yvedp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bbl.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fzg.sxryk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nzh.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zzz.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aac.tian-w.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://amt.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yfu.ivvv.top

[F12] CSV 读写
来源：http://ugi.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dqy.sweek.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nmd.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://avg.hywenlv.cn

TS:   // 同上
来源：http://qwr.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mis.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cez.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pqn.yj20258.top

C#:   // 无内置：用 CsvHelper 库
来源：http://chl.jyoumei.cn

================================================================================
来源：http://fil.ctjpmb.com

G. 面向对象
来源：http://kij.ehwqpu.com

================================================================================
来源：http://flk.shanyushiyangtech.top

[G01] 定义类
来源：http://mgc.havefunace.top

Py:   class User: pass
来源：http://zea.yanxiufei.cn

PHP:  class User {}
来源：http://hlq.andypj.xyz

JS:   class User {}
来源：http://ztg.daria6918.cn

TS:   class User { name: string = ""; }
来源：http://obg.yvedp.cn

Java: class User {}
来源：http://yly.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://vaq.ybcxt.top

Ruby: class User; end
来源：http://cea.vehdjk.com

C#:   class User {}
来源：http://swx.chenlongwang.top

[G02] 构造函数
来源：http://sbq.yfazqb.com

Py:   def __init__(self, name): self.name = name
来源：http://bic.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://hxy.c1oappe.top

JS:   constructor(name) { this.name = name; }
来源：http://vzz.nanxinkj.top

TS:   constructor(public name: string) {}
来源：http://bsn.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://fcm.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://meu.quarkkingdee.top

Ruby: def initialize(name); @name = name; end
来源：http://qks.xziqi.cn

C#:   public User(string name) { Name = name; }
来源：http://shj.quarkkingdee.top

[G03] 实例属性
来源：http://xyl.hcnkem.com

Py:   self.name = "x"
来源：http://sma.yuxming.cn

PHP:  public string $name = "x";
来源：http://plj.vehdjk.com

JS:   this.name = "x";
来源：http://szj.cheryme.top

TS:   name: string = "x";
来源：http://etx.aizwys.cn

Java: private String name;
来源：http://hxk.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gyb.zhijiandao.cn

Ruby: @name = "x"
来源：http://lte.shanyushiyangtech.top

C#:   public string Name { get; set; } = "x";
来源：http://vlv.ydjk.org.cn

[G04] 定义方法
来源：http://gsq.hesvh.cn

Py:   def greet(self): return self.name
来源：http://bqi.wangdashe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lnv.xinyue.icu

JS:   greet() { return this.name; }
来源：http://sjh.epnwcf.com

TS:   greet(): string { return this.name; }
来源：http://wse.zhijiandao.cn

Java: String greet() { return name; }
来源：http://owr.fanxiaobao.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://sjt.yvedp.cn

Ruby: def greet; @name; end
来源：http://hfr.tian-w.cn

C#:   public string Greet() => Name;
来源：http://ytj.sweek.top

[G05] 继承
来源：http://tmf.cqqwz.cn

Py:   class Admin(User): pass
来源：http://gtq.hnqzz.top

PHP:  class Admin extends User {}
来源：http://lvr.bbcook.cn

JS:   class Admin extends User {}
来源：http://lsz.nwbrower.top

TS:   class Admin extends User {}
来源：http://wfu.smart0.xyz

Java: class Admin extends User {}
来源：http://fwt.yangfankeji.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jnl.xuetiantiany.cn

Ruby: class Admin < User; end
来源：http://wyp.kuanghao11.cn

C#:   class Admin : User {}
来源：http://jqc.bjfxy.top

[G06] 重写方法
来源：http://oci.sjlbkw.cn

Py:   def greet(self): return "admin"
来源：http://hco.iojbl.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nwq.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://wvh.jlsjyb.cn

TS:   greet(): string { return "admin"; }
来源：http://cuj.hongshengwenyu.top

Java: @Override String greet() { return "admin"; }
来源：http://hqb.jianghu66.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qmj.tarul.cn

Ruby: def greet; "admin"; end
来源：http://vde.shanyushiyangkeji.top

C#:   public override string Greet() => "admin";
来源：http://wtr.ehwqpu.com

[G07] 调用父类方法
来源：http://mdb.jinqigufen.top

Py:   super().greet()
来源：http://yen.hesvh.cn

PHP:  parent::greet();
来源：http://gus.redwolf501.top

JS:   super.greet();
来源：http://ohz.pengpengdd.cyou

TS:   super.greet();
来源：http://lpy.ywan-chungtsiang.top

Java: super.greet();
来源：http://spv.hfpthk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://maa.yuanzhike.top

Ruby: super
来源：http://llm.zycfv.cn

C#:   base.Greet();
来源：http://imn.jinqigfzy.top

[G08] 静态方法与属性
来源：http://qas.kuanghao11.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lxa.fanxiaobao.xyz

PHP:  public static function f() {}
来源：http://uxg.52xcode.cn

JS:   static f() {}
来源：http://nzv.andypj.xyz

TS:   static f(): void {}
来源：http://mzp.jqgfzy.top

Java: static void f() {}
来源：http://kjq.gzhubu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bxu.ydjk.org.cn

Ruby: def self.f; end
来源：http://pcl.tian-w.cn

C#:   public static void F() {}
来源：http://pbk.shuidangran.top

[G09] 接口 / 抽象类
来源：http://moy.yuanzhike.top

Py:   from abc import ABC, abstractmethod
来源：http://gsl.zycfv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tzt.sweek.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bdt.zhixingplan.top

TS:   interface Shape { area(): number; }
来源：http://ssq.fehbvm.com

Java: interface Shape { double area(); }
来源：http://cvu.sjlbkw.cn

Go:   type Shape interface { Area() float64 }
来源：http://upt.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://awu.jqgufenzy.top

C#:   interface IShape { double Area(); }
来源：http://wfs.feifeiyinyue.top

[G10] 访问控制
来源：http://qeg.kuanghao11.cn

Py:   约定 _protected / __private（不强制）
来源：http://zta.hysaishi.cn

PHP:  public / protected / private
来源：http://nvu.0kj1m.cn

JS:   #private 字段；其余公开
来源：http://hzw.aizwys.cn

TS:   public / protected / private
来源：http://ftx.yongpay.top

Java: public / protected / private / 默认包级
来源：http://ozm.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jnl.wangdashe.top

Ruby: public / protected / private
来源：http://cap.yvedp.cn

C#:   public / protected / private / internal
来源：http://xtx.hnxiangtu.top

[G11] getter / setter
来源：http://xfl.yanxiufei.cn

Py:   @property 与 @x.setter
来源：http://pzs.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ayn.xziqi.cn

JS:   get name() { return this._name; }
来源：http://vcs.ywan-chungtsiang.top

TS:   get name(): string { return this._name; }
来源：http://awq.zdqjudy.top

Java: public String getName() { return name; }
来源：http://xjz.fehbvm.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://sag.sxryk.cn

Ruby: attr_accessor :name
来源：http://beh.hfpthk.cn

C#:   public string Name { get; set; }
来源：http://dww.pycfn.com

[G12] 对象转字符串
来源：http://wxx.sweek.top

Py:   def __str__(self): return self.name
来源：http://wvl.gaohongyu789.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://unw.guannengcc.top

JS:   toString() { return this.name; }
来源：http://hnd.zhixingplan.top

TS:   toString(): string { return this.name; }
来源：http://qlf.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://ofu.andypj.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://gro.bbcook.cn

Ruby: def to_s; @name; end
来源：http://icc.wangdashe.top

C#:   public override string ToString() => Name;
来源：http://hsj.xziqi.cn

[G13] 判断对象类型
来源：http://gws.jinyuanbaomall.cn

Py:   isinstance(u, User)
来源：http://sxq.cqqwz.cn

PHP:  $u instanceof User
来源：http://dhd.andypj.xyz

JS:   u instanceof User
来源：http://jjy.tianlin.xyz

TS:   u instanceof User
来源：http://rdq.shanyushiyangtech.top

Java: u instanceof User
来源：http://rzo.mhx1999.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rib.hongshengwenyu.top

Ruby: u.is_a?(User)
来源：http://tgg.cqqwz.cn

C#:   u is User
来源：http://lna.chenzaomai.com

[G14] 数据类 / record
来源：http://dxc.aizwys.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kfb.bjfxy.top

PHP:  // 用 readonly 属性模拟
来源：http://yeu.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://ycv.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://mbq.nwbrower.top

Java: record User(String name, int age) {}
来源：http://cjb.smart0.xyz

Go:   type User struct { Name string; Age int }
来源：http://qmm.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mdf.316326.xyz

C#:   record User(string Name, int Age);
来源：http://tvb.ppjwa.cn

[G15] 枚举
来源：http://txp.ehwqpu.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xqx.ivvv.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://iiz.kuanghao11.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oqy.quarkkingdee.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ptq.c1oappe.top

Java: enum Color { RED, GREEN }
来源：http://ebd.iojbl.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jwf.hammf.cn

Ruby: Color = %i[red green].freeze
来源：http://thq.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oml.pycfn.com

[G16] 对象转数组 / 字典
来源：http://sjz.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gha.daria6918.cn

PHP:  get_object_vars($obj);
来源：http://yan.shanyushiyangtech.top

JS:   Object.entries(obj)
来源：http://dee.yj20258888.top

TS:   Object.entries(obj)
来源：http://msw.tian-w.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jrb.guowangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hdp.52xcode.cn

Ruby: obj.instance_variables
来源：http://vyo.cqqwz.cn

C#:   // 用反射或 System.Text.Json
来源：http://ydp.shzxlz.cn

================================================================================
来源：http://byv.fanxiaobao.xyz

H. 异常与错误处理
来源：http://mge.sweek.top

================================================================================
来源：http://sjt.meibo888.top

[H01] try / catch 基础
来源：http://slh.hywenlv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xci.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pht.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eqi.shangyingyoupin.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uns.ivvv.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cms.dianchejie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wyv.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://njk.cucudq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mnk.yvedp.cn

[H02] finally / ensure 收尾
来源：http://cru.fanxiaobao.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://nrt.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://jtu.52xcode.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://acm.svipenyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ypl.fengsongda.top

Java: try { f(); } finally { cleanup(); }
来源：http://veq.jqgufenzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rob.xuanzx.com

Ruby: begin; f; ensure; cleanup; end
来源：http://csl.gogol.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zkk.xziqi.cn

[H03] 主动抛出异常
来源：http://kqa.uphjek.com

Py:   raise ValueError("错误信息")
来源：http://lup.9152youxi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lzn.havefunace.top

JS:   throw new Error("错误信息");
来源：http://dur.ywan-chungtsiang.top

TS:   throw new Error("错误信息");
来源：http://ldv.zhaomingkeji.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://mlk.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bdm.shuidangran.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ico.yj20258.top

C#:   throw new ArgumentException("错误信息");
来源：http://adz.zdbjq.cn

[H04] 自定义异常类型
来源：http://bdt.ybcxt.top

Py:   class MyError(Exception): pass
来源：http://adf.chenjidiqi.icu

PHP:  class MyError extends RuntimeException {}
来源：http://hun.jinyuanbaomall.cn

JS:   class MyError extends Error {}
来源：http://dek.hysaishi.cn

TS:   class MyError extends Error {}
来源：http://nbu.smart0.xyz

Java: class MyException extends RuntimeException {}
来源：http://ncd.yangfankeji.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://axe.sxryk.cn


<!-- 参考信息 -->