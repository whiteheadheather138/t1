代发 wailian999

[E22] 字节长度与字符长度
来源：http://usr.yongpay.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bvi.hesvh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gus.ydjk.org.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mkq.ydjk.org.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://imj.sweek.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oim.sjlbkw.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hfz.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://xhm.ydzc1.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://opt.zhijiandao.cn

================================================================================
来源：http://gui.zycfv.cn

F. 文件与目录
来源：http://uja.cqqwz.cn

================================================================================
来源：http://ypy.hongshengwenyu.top

[F01] 读取整个文件
来源：http://vmk.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xww.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://umd.chenlongwang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zud.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ujj.yj20258888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yls.xylfe.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ner.redwolf501.top

Ruby: File.read("a.txt")
来源：http://vgl.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://zlt.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://gqu.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://auk.redwolf501.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://llk.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://obl.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nfg.tanke756.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sec.hcnkem.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fit.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aly.hongshengwenyu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vuq.xinyue.icu

[F03] 写入文件（覆盖）
来源：http://lzo.shangyingyoupin.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wxn.yvedp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sge.fktsv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hvy.jiagoushi.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gnn.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ppl.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rnf.nanxuanxn.top

Ruby: File.write("a.txt", "hi")
来源：http://inh.hammf.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gdb.xinyue.icu

[F04] 追加写入文件
来源：http://wzd.wangdashe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://orm.nanxinkj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://osk.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zeh.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mbg.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ugi.aizwys.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zho.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bda.pycfn.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ymu.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://tsk.mhx1999.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ink.shuidangran.top

PHP:  file_exists("a.txt");
来源：http://fby.shanyushiyangtech.top

JS:   fs.existsSync("a.txt")
来源：http://zlf.cqqwz.cn

TS:   fs.existsSync("a.txt")
来源：http://ofc.quarkkingdee.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mdv.xziqi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wkt.yj202588.top

Ruby: File.exist?("a.txt")
来源：http://hbd.meibo888.top

C#:   File.Exists("a.txt")
来源：http://ocg.yj20258.top

[F06] 删除文件
来源：http://bgw.quarkkingdee.top

Py:   os.remove("a.txt")
来源：http://ciu.guowangkeji.top

PHP:  unlink("a.txt");
来源：http://pnr.vehdjk.com

JS:   fs.unlinkSync("a.txt")
来源：http://vnq.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://ekj.pycfn.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rpo.hywenlv.cn

Go:   os.Remove("a.txt")
来源：http://ump.yfazqb.com

Ruby: File.delete("a.txt")
来源：http://yzi.guowangkeji.top

C#:   File.Delete("a.txt");
来源：http://gwp.zhiwuduotai.top

[F07] 创建目录（含多级）
来源：http://uva.xinyue.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://orv.yuxming.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lvm.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://irk.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ckc.snrcjt.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oer.fehbvm.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ddi.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wik.daxiang520.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://loo.mhx1999.top

[F08] 遍历目录
来源：http://jii.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dwe.fzhhl.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uzb.sufxvd.cn

JS:   fs.readdirSync("dir")
来源：http://ail.yueranfly.top

TS:   fs.readdirSync("dir")
来源：http://uzi.xziqi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zxl.tian-w.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fjn.wangdashe.top

Ruby: Dir.children("dir")
来源：http://yxa.hnxiangtu.top

C#:   Directory.GetFiles("dir")
来源：http://ksl.jinqigfzy.top

[F09] 获取文件大小
来源：http://gvy.ydjk.org.cn

Py:   os.path.getsize("a.txt")
来源：http://zjh.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://bak.sufxvd.cn

JS:   fs.statSync("a.txt").size
来源：http://wrk.ivvv.top

TS:   fs.statSync("a.txt").size
来源：http://ysj.chenzaomai.com

Java: Files.size(Path.of("a.txt"))
来源：http://prt.daxiang520.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://row.ivvv.top

Ruby: File.size("a.txt")
来源：http://gbo.zhoulong.xyz

C#:   new FileInfo("a.txt").Length
来源：http://dxm.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://gco.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vdl.ehwqpu.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kto.ybcxt.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xgl.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://uht.0kj1m.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://deh.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hft.yj20258.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gvq.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aoc.hywenlv.cn

[F11] 复制与移动文件
来源：http://ave.dianchejie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zpl.cashguo.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://snt.bbcook.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gqb.xylfe.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dio.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rqz.sxryk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bvl.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vmp.shzxlz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ajz.xingfuxueyuan.xyz

[F12] CSV 读写
来源：http://wls.jlsjyb.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dsj.redwolf501.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://obz.nwbrower.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dib.havefunace.top

TS:   // 同上
来源：http://ebd.pycfn.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gfb.yuxming.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rgh.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vhk.sxryk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://idk.tian-w.cn

================================================================================
来源：http://rci.nwbrower.top

G. 面向对象
来源：http://iqp.tanke756.top

================================================================================
来源：http://jas.tianlin.xyz

[G01] 定义类
来源：http://tgc.bjfxy.top

Py:   class User: pass
来源：http://ctr.jinyuanbaomall.cn

PHP:  class User {}
来源：http://zxf.jianghu66.top

JS:   class User {}
来源：http://ovf.tianlin.xyz

TS:   class User { name: string = ""; }
来源：http://xnv.hcnkem.com

Java: class User {}
来源：http://que.sweek.top

Go:   type User struct { Name string }
来源：http://nyg.meibo888.top

Ruby: class User; end
来源：http://omw.mhx1999.top

C#:   class User {}
来源：http://tli.ivvv.top

[G02] 构造函数
来源：http://mds.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://uyo.yongpay.top

PHP:  public function __construct(public string $name) {}
来源：http://qdg.chenlongwang.top

JS:   constructor(name) { this.name = name; }
来源：http://qem.zhengqikj.top

TS:   constructor(public name: string) {}
来源：http://onv.c1oappe.top

Java: User(String name) { this.name = name; }
来源：http://uvf.bbcook.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yli.kuanghao11.cn

Ruby: def initialize(name); @name = name; end
来源：http://edr.jyoumei.cn

C#:   public User(string name) { Name = name; }
来源：http://hcv.tanke756.top

[G03] 实例属性
来源：http://pph.vqdsnc.cn

Py:   self.name = "x"
来源：http://esw.ivvv.top

PHP:  public string $name = "x";
来源：http://aub.yuanzhike.top

JS:   this.name = "x";
来源：http://xii.ywan-chungtsiang.top

TS:   name: string = "x";
来源：http://jpx.xingfuxueyuan.xyz

Java: private String name;
来源：http://tpf.fehbvm.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xgr.andypj.xyz

Ruby: @name = "x"
来源：http://iex.havefunace.top

C#:   public string Name { get; set; } = "x";
来源：http://rpf.xziqi.cn

[G04] 定义方法
来源：http://cew.chenzaomai.com

Py:   def greet(self): return self.name
来源：http://tpy.wangshuangyany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://akh.epnwcf.com

JS:   greet() { return this.name; }
来源：http://oui.guannengcc.top

TS:   greet(): string { return this.name; }
来源：http://axa.hnxiangtu.top

Java: String greet() { return name; }
来源：http://ldt.gogol.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gac.shanyushiyangkeji.top

Ruby: def greet; @name; end
来源：http://nxo.daxiang520.top

C#:   public string Greet() => Name;
来源：http://ybg.nanxinkj.top

[G05] 继承
来源：http://tfe.jinghuilouyu.cn

Py:   class Admin(User): pass
来源：http://pby.zdqjudy.top

PHP:  class Admin extends User {}
来源：http://hds.ppjwa.cn

JS:   class Admin extends User {}
来源：http://nlj.gotoacloud.top

TS:   class Admin extends User {}
来源：http://jyw.zhongyouzk.top

Java: class Admin extends User {}
来源：http://lwl.zhaomingkeji.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nrz.tanke756.top

Ruby: class Admin < User; end
来源：http://gun.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://ckg.jiagoushi.top

[G06] 重写方法
来源：http://fkl.epnwcf.com

Py:   def greet(self): return "admin"
来源：http://ddp.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nkk.vehdjk.com

JS:   greet() { return "admin"; }
来源：http://rhb.zdqjudy.top

TS:   greet(): string { return "admin"; }
来源：http://itc.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://zrp.guowangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kss.hnqzz.top

Ruby: def greet; "admin"; end
来源：http://uxb.yfazqb.com

C#:   public override string Greet() => "admin";
来源：http://ywu.bbcook.cn

[G07] 调用父类方法
来源：http://zgr.52xcode.cn

Py:   super().greet()
来源：http://wnv.kuanghao11.cn

PHP:  parent::greet();
来源：http://lym.fengsongda.top

JS:   super.greet();
来源：http://aac.ybcxt.top

TS:   super.greet();
来源：http://pyh.jyoumei.cn

Java: super.greet();
来源：http://lma.yj202588.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://efw.hongshengwenyu.top

Ruby: super
来源：http://jyk.gotoacloud.top

C#:   base.Greet();
来源：http://nkb.yj202588.top

[G08] 静态方法与属性
来源：http://rmf.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wed.fengsongda.top

PHP:  public static function f() {}
来源：http://qkc.shzxlz.cn

JS:   static f() {}
来源：http://dpw.hnxiangtu.top

TS:   static f(): void {}
来源：http://lvy.shzxlz.cn

Java: static void f() {}
来源：http://oej.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qov.havefunace.top

Ruby: def self.f; end
来源：http://uyc.cdnleiting.top

C#:   public static void F() {}
来源：http://utt.yvedp.cn

[G09] 接口 / 抽象类
来源：http://fjt.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://lyd.hfpthk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wqp.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nnk.ppjwa.cn

TS:   interface Shape { area(): number; }
来源：http://onr.jinyuanbaomall.cn

Java: interface Shape { double area(); }
来源：http://gzg.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://liw.chenzaomai.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lrp.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://plb.gotoacloud.top

[G10] 访问控制
来源：http://kak.hesvh.cn

Py:   约定 _protected / __private（不强制）
来源：http://dhe.nwbrower.top

PHP:  public / protected / private
来源：http://ttq.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://hto.xylfe.cn

TS:   public / protected / private
来源：http://hoz.nanxuanxn.top

Java: public / protected / private / 默认包级
来源：http://zow.tian-w.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://axl.zhaomingkeji.xyz

Ruby: public / protected / private
来源：http://vfh.sysykeji.top

C#:   public / protected / private / internal
来源：http://mqe.yfazqb.com

[G11] getter / setter
来源：http://ciq.hnxiangtu.top

Py:   @property 与 @x.setter
来源：http://tfl.hnqzz.top

PHP:  public function getName(): string { return $this->name; }
来源：http://edx.yfazqb.com

JS:   get name() { return this._name; }
来源：http://hzq.xingfuxueyuan.xyz

TS:   get name(): string { return this._name; }
来源：http://zog.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://zhj.hammf.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://isj.gotoacloud.top

Ruby: attr_accessor :name
来源：http://ruq.gogol.net.cn

C#:   public string Name { get; set; }
来源：http://qrq.ivvv.top

[G12] 对象转字符串
来源：http://ccm.tianlin.xyz

Py:   def __str__(self): return self.name
来源：http://cji.zhixingplan.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fnp.jlsjyb.cn

JS:   toString() { return this.name; }
来源：http://ire.fengsongda.top

TS:   toString(): string { return this.name; }
来源：http://xsl.shanyushiyangtech.top

Java: @Override public String toString() { return name; }
来源：http://iye.cdnleiting.top

Go:   func (u User) String() string { return u.Name }
来源：http://pgj.aizwys.cn

Ruby: def to_s; @name; end
来源：http://rfe.cqqwz.cn

C#:   public override string ToString() => Name;
来源：http://jcl.yj20258888.top

[G13] 判断对象类型
来源：http://mlm.pycfn.com

Py:   isinstance(u, User)
来源：http://cfh.daria6918.cn

PHP:  $u instanceof User
来源：http://anp.chenlongwang.top

JS:   u instanceof User
来源：http://wut.shzxlz.cn

TS:   u instanceof User
来源：http://xxf.yuxming.cn

Java: u instanceof User
来源：http://fyr.ctjpmb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://tfq.birdmap.top

Ruby: u.is_a?(User)
来源：http://dph.tarul.cn

C#:   u is User
来源：http://ioq.sysykeji.top

[G14] 数据类 / record
来源：http://gmn.bbcook.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pxn.fktsv.cn

PHP:  // 用 readonly 属性模拟
来源：http://vyr.meibo888.top

JS:   // 无内置：普通类或对象字面量
来源：http://jtj.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://gdt.gaohongyu789.top

Java: record User(String name, int age) {}
来源：http://dwp.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://ksr.ydjk.org.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iti.nanxinkj.top

C#:   record User(string Name, int Age);
来源：http://kkl.zycfv.cn

[G15] 枚举
来源：http://uvp.jiagoushi.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fda.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xis.tianlin.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xzi.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pbd.redwolf501.top

Java: enum Color { RED, GREEN }
来源：http://wca.shangyingyoupin.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xdt.ehwqpu.com

Ruby: Color = %i[red green].freeze
来源：http://cwb.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dvl.zhaomingkeji.xyz

[G16] 对象转数组 / 字典
来源：http://csb.aibaodan.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gvv.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://gic.smart0.xyz

JS:   Object.entries(obj)
来源：http://sxu.xingfuxueyuan.xyz

TS:   Object.entries(obj)
来源：http://jjm.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://scr.chenlongwang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hzm.xinyue.icu

Ruby: obj.instance_variables
来源：http://qtl.zhixingplan.top

C#:   // 用反射或 System.Text.Json
来源：http://cef.nanxuanxn.top

================================================================================
来源：http://kws.snrcjt.cn

H. 异常与错误处理
来源：http://fft.c1oappe.top

================================================================================
来源：http://kzw.hesvh.cn

[H01] try / catch 基础
来源：http://kkl.tianlin.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://daa.hfpthk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eil.iojbl.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://arv.aizwys.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ogk.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://poq.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kip.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ztk.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mkq.hesvh.cn

[H02] finally / ensure 收尾
来源：http://uup.cashguo.top

Py:   try: f()⏎finally: cleanup()
来源：http://ssl.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://evf.wangdashe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://piw.xziqi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yob.nwbrower.top

Java: try { f(); } finally { cleanup(); }
来源：http://wkp.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://egf.cqqwz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ndr.pycfn.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://yzj.wangdashe.top

[H03] 主动抛出异常
来源：http://cdv.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://rrc.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mkm.jiagoushi.top

JS:   throw new Error("错误信息");
来源：http://qui.zhaomingkeji.xyz

TS:   throw new Error("错误信息");
来源：http://sqk.tarul.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uea.ctjpmb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hqv.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mvu.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://czo.nanxinkj.top

[H04] 自定义异常类型
来源：http://lcg.kuanghao11.cn

Py:   class MyError(Exception): pass
来源：http://dgz.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mwa.epnwcf.com


<!-- 参考信息 -->