代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dio.sxryk.cn

================================================================================
来源：http://eum.jiagoushi.top

F. 文件与目录
来源：http://xag.guannengcc.top

================================================================================
来源：http://xoo.hongshengwenyu.top

[F01] 读取整个文件
来源：http://omj.ywan-chungtsiang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lrk.fanxiaobao.xyz

PHP:  file_get_contents("a.txt");
来源：http://vgv.yuanzhike.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nav.ywan-chungtsiang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ajc.hfpthk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lql.zhaomingkeji.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tch.xingfuxueyuan.xyz

Ruby: File.read("a.txt")
来源：http://egw.yangfankeji.com

C#:   File.ReadAllText("a.txt");
来源：http://sam.dashuyun.cn

[F02] 逐行读取文件
来源：http://bfd.xuanzx.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gxt.xuanzx.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mpl.shanyushiyangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xgw.cdnleiting.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sso.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xhe.hongshengwenyu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rjf.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://prp.fehbvm.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sdp.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://qfs.nanxinkj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pcx.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jgs.dianchejie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qrh.bbcook.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zkn.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vqg.ybcxt.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://glf.nanxinkj.top

Ruby: File.write("a.txt", "hi")
来源：http://ddh.yongpay.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ibg.ydzc1.top

[F04] 追加写入文件
来源：http://tfg.sjlbkw.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jqq.zhongyouzk.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://svc.bjfxy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dgh.chenlongwang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wbd.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sqy.chenjidiqi.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ytk.pycfn.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iwq.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rxc.cheryme.top

[F05] 判断文件或目录是否存在
来源：http://swz.jinyuanbaomall.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fof.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://qdw.zycfv.cn

JS:   fs.existsSync("a.txt")
来源：http://vdl.wangdashe.top

TS:   fs.existsSync("a.txt")
来源：http://bfg.fktsv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ivw.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zsw.daxiang520.top

Ruby: File.exist?("a.txt")
来源：http://nwe.fehbvm.com

C#:   File.Exists("a.txt")
来源：http://kdk.wangshuangyany.cn

[F06] 删除文件
来源：http://pnf.jyoumei.cn

Py:   os.remove("a.txt")
来源：http://dgz.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://vca.cqqwz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nxw.0kj1m.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yff.c1oappe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jvx.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://ing.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://rbn.gotoacloud.top

C#:   File.Delete("a.txt");
来源：http://gob.hysaishi.cn

[F07] 创建目录（含多级）
来源：http://owi.yj202588.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://plb.shuidangran.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vpz.nanxinkj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tzu.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lhj.chenzaomai.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://afy.mhx1999.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zxf.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yvu.yuanzhike.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lad.xinyue.icu

[F08] 遍历目录
来源：http://leb.chenzaomai.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://bvv.nanxinkj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hje.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://kns.svipenyu.cn

TS:   fs.readdirSync("dir")
来源：http://igv.xylfe.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pcc.52xcode.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://end.yanxiufei.cn

Ruby: Dir.children("dir")
来源：http://cst.52xcode.cn

C#:   Directory.GetFiles("dir")
来源：http://tpg.jinyuanbaomall.cn

[F09] 获取文件大小
来源：http://zaq.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://wcq.ydzc1.top

PHP:  filesize("a.txt");
来源：http://eyz.jqgfzy.top

JS:   fs.statSync("a.txt").size
来源：http://huv.meibo888.top

TS:   fs.statSync("a.txt").size
来源：http://vnc.ydzc1.top

Java: Files.size(Path.of("a.txt"))
来源：http://jin.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fhg.svipenyu.cn

Ruby: File.size("a.txt")
来源：http://psz.shanyushiyangtech.top

C#:   new FileInfo("a.txt").Length
来源：http://boh.kuanghao11.cn

[F10] 取文件扩展名 / 文件名
来源：http://seb.fehbvm.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pdy.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sne.ybcxt.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pli.ybcxt.top

TS:   path.extname("a.txt")
来源：http://lvw.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dzz.yuxming.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vun.guowangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lcb.c1oappe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cvi.yueranfly.top

[F11] 复制与移动文件
来源：http://sdn.gaohongyu789.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ebv.gotoacloud.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://goa.hammf.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ooc.yuxming.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://haa.quarkkingdee.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://luu.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bfi.cashguo.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://skt.nwbrower.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qly.tianlin.xyz

[F12] CSV 读写
来源：http://eao.chenlongwang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zdj.sysykeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://txx.tian-w.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rei.wangshuangyany.cn

TS:   // 同上
来源：http://mpm.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hyj.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ukl.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dib.ydjk.org.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zbb.sxryk.cn

================================================================================
来源：http://cid.jinqigufen.top

G. 面向对象
来源：http://ven.fktsv.cn

================================================================================
来源：http://xyn.redwolf501.top

[G01] 定义类
来源：http://iah.guannengcc.top

Py:   class User: pass
来源：http://yri.hongshengwenyu.top

PHP:  class User {}
来源：http://dvk.hnxiangtu.top

JS:   class User {}
来源：http://jhp.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://vtr.pycfn.com

Java: class User {}
来源：http://abp.nwbrower.top

Go:   type User struct { Name string }
来源：http://kum.guowangkeji.top

Ruby: class User; end
来源：http://bhz.ctjpmb.com

C#:   class User {}
来源：http://ndi.zhixingplan.top

[G02] 构造函数
来源：http://pzx.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://bjc.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://vow.yuxming.cn

JS:   constructor(name) { this.name = name; }
来源：http://rhz.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://awy.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://buj.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://igz.epnwcf.com

Ruby: def initialize(name); @name = name; end
来源：http://ftr.daxiang520.top

C#:   public User(string name) { Name = name; }
来源：http://xgu.guowangkeji.top

[G03] 实例属性
来源：http://tdy.yuanzhike.top

Py:   self.name = "x"
来源：http://apq.pycfn.com

PHP:  public string $name = "x";
来源：http://pwd.redwolf501.top

JS:   this.name = "x";
来源：http://vtk.xylfe.cn

TS:   name: string = "x";
来源：http://iny.zhijiandao.cn

Java: private String name;
来源：http://dkj.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sdj.jqgufenzy.top

Ruby: @name = "x"
来源：http://gtj.ydjk.org.cn

C#:   public string Name { get; set; } = "x";
来源：http://fnx.dashuyun.cn

[G04] 定义方法
来源：http://yrc.ywan-chungtsiang.top

Py:   def greet(self): return self.name
来源：http://nfa.cdnleiting.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gzs.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://vjp.gaohongyu789.top

TS:   greet(): string { return this.name; }
来源：http://ivl.0kj1m.cn

Java: String greet() { return name; }
来源：http://efk.yvedp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ahl.uphjek.com

Ruby: def greet; @name; end
来源：http://smd.c1oappe.top

C#:   public string Greet() => Name;
来源：http://ncv.iojbl.cn

[G05] 继承
来源：http://jsg.smart0.xyz

Py:   class Admin(User): pass
来源：http://nqw.ehwqpu.com

PHP:  class Admin extends User {}
来源：http://nne.hongshengwenyu.top

JS:   class Admin extends User {}
来源：http://mzn.jinqigfzy.top

TS:   class Admin extends User {}
来源：http://nll.uphjek.com

Java: class Admin extends User {}
来源：http://xpu.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://byq.sxryk.cn

Ruby: class Admin < User; end
来源：http://fsi.cashguo.top

C#:   class Admin : User {}
来源：http://qgw.gzhubu.top

[G06] 重写方法
来源：http://yom.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://erp.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zkn.yangfankeji.com

JS:   greet() { return "admin"; }
来源：http://zdm.wangdashe.top

TS:   greet(): string { return "admin"; }
来源：http://rnz.uphjek.com

Java: @Override String greet() { return "admin"; }
来源：http://xtl.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kqb.fehbvm.com

Ruby: def greet; "admin"; end
来源：http://yut.gzhubu.top

C#:   public override string Greet() => "admin";
来源：http://nok.aizwys.cn

[G07] 调用父类方法
来源：http://ehy.jqgufenzy.top

Py:   super().greet()
来源：http://dbi.kuanghao11.cn

PHP:  parent::greet();
来源：http://jcf.yuxming.cn

JS:   super.greet();
来源：http://bqz.smart0.xyz

TS:   super.greet();
来源：http://idp.zhoulong.xyz

Java: super.greet();
来源：http://aqu.shuidangran.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zwh.pycfn.com

Ruby: super
来源：http://qjx.tanke756.top

C#:   base.Greet();
来源：http://hag.shangyingyoupin.top

[G08] 静态方法与属性
来源：http://zpf.yueranfly.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wmd.fanxiaobao.xyz

PHP:  public static function f() {}
来源：http://gbf.jiagoushi.top

JS:   static f() {}
来源：http://ytb.zhoulong.xyz

TS:   static f(): void {}
来源：http://gjz.316326.xyz

Java: static void f() {}
来源：http://ukr.tianlin.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://dbq.gzhubu.top

Ruby: def self.f; end
来源：http://tkr.shanyushiyangtech.top

C#:   public static void F() {}
来源：http://jxv.fanxiaobao.xyz

[G09] 接口 / 抽象类
来源：http://wqz.zdbjq.cn

Py:   from abc import ABC, abstractmethod
来源：http://jes.jinqigfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://cpa.xziqi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yny.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://usb.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://gdi.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://kod.ctjpmb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vdi.shanyushiyangkeji.top

C#:   interface IShape { double Area(); }
来源：http://lqn.sufxvd.cn

[G10] 访问控制
来源：http://gnm.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://zve.mhx1999.top

PHP:  public / protected / private
来源：http://rhb.cdnleiting.top

JS:   #private 字段；其余公开
来源：http://jof.yangfankeji.com

TS:   public / protected / private
来源：http://pkp.wangdashe.top

Java: public / protected / private / 默认包级
来源：http://bwr.fanxiaobao.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://kob.0kj1m.cn

Ruby: public / protected / private
来源：http://cgu.nanxuanxn.top

C#:   public / protected / private / internal
来源：http://uba.chenjidiqi.icu

[G11] getter / setter
来源：http://yve.fanxiaobao.xyz

Py:   @property 与 @x.setter
来源：http://odi.zhaomingkeji.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://hmc.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://zop.cqqwz.cn

TS:   get name(): string { return this._name; }
来源：http://ezw.yj20258.top

Java: public String getName() { return name; }
来源：http://hya.hongshengwenyu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nkh.quarkkingdee.top

Ruby: attr_accessor :name
来源：http://ees.gotoacloud.top

C#:   public string Name { get; set; }
来源：http://gja.zdbjq.cn

[G12] 对象转字符串
来源：http://nar.ehwqpu.com

Py:   def __str__(self): return self.name
来源：http://itd.ppjwa.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dnd.hesvh.cn

JS:   toString() { return this.name; }
来源：http://wqw.svipenyu.cn

TS:   toString(): string { return this.name; }
来源：http://odq.jinghuilouyu.cn

Java: @Override public String toString() { return name; }
来源：http://ihv.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ibm.c1oappe.top

Ruby: def to_s; @name; end
来源：http://fgq.ydzc1.top

C#:   public override string ToString() => Name;
来源：http://cvm.jinyuanbaomall.cn

[G13] 判断对象类型
来源：http://prf.shangyingyoupin.top

Py:   isinstance(u, User)
来源：http://uxe.zhoulong.xyz

PHP:  $u instanceof User
来源：http://ufp.sweek.top

JS:   u instanceof User
来源：http://ush.sysykeji.top

TS:   u instanceof User
来源：http://qii.jinghuilouyu.cn

Java: u instanceof User
来源：http://ipw.zdqjudy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xuo.fengsongda.top

Ruby: u.is_a?(User)
来源：http://jff.wangdashe.top

C#:   u is User
来源：http://lti.bbcook.cn

[G14] 数据类 / record
来源：http://kwh.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xhf.redwolf501.top

PHP:  // 用 readonly 属性模拟
来源：http://jig.snrcjt.cn

JS:   // 无内置：普通类或对象字面量
来源：http://igt.hywenlv.cn

TS:   type User = { name: string; age: number };
来源：http://kfo.ydzc1.top

Java: record User(String name, int age) {}
来源：http://lrz.zhaomingkeji.xyz

Go:   type User struct { Name string; Age int }
来源：http://bbu.yongpay.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://der.guannengcc.top

C#:   record User(string Name, int Age);
来源：http://hjo.feifeiyinyue.top

[G15] 枚举
来源：http://cmj.yanxiufei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lzv.iojbl.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zwo.cucudq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nwp.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tie.yj202588.top

Java: enum Color { RED, GREEN }
来源：http://ucp.ywan-chungtsiang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hqu.gaohongyu789.top

Ruby: Color = %i[red green].freeze
来源：http://hgm.shanyushiyangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ehd.redwolf501.top

[G16] 对象转数组 / 字典
来源：http://qim.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tst.pengpengdd.cyou

PHP:  get_object_vars($obj);
来源：http://dxw.fengsongda.top

JS:   Object.entries(obj)
来源：http://ots.aibaodan.cn

TS:   Object.entries(obj)
来源：http://rgj.yuxming.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fgn.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://aue.jianghu66.top

Ruby: obj.instance_variables
来源：http://gwi.316326.xyz

C#:   // 用反射或 System.Text.Json
来源：http://kgs.yonumen.top

================================================================================
来源：http://xee.jinyuanbaomall.cn

H. 异常与错误处理
来源：http://gse.jyoumei.cn

================================================================================
来源：http://xkx.zycfv.cn

[H01] try / catch 基础
来源：http://ezb.jinyuanbaomall.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://szd.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aty.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zbx.daxiang520.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fnr.zycfv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nge.wangshuangyany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qww.cdnleiting.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pjq.cucudq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lpz.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://osq.hfpthk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://emv.pengpengdd.cyou

PHP:  try { f(); } finally { cleanup(); }
来源：http://ick.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://dlr.xinyue.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://hcm.xuanzx.com

Java: try { f(); } finally { cleanup(); }
来源：http://zzs.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://dzk.aibaodan.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://eaf.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tok.jyoumei.cn

[H03] 主动抛出异常
来源：http://qfn.ppjwa.cn

Py:   raise ValueError("错误信息")
来源：http://igh.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ttm.uphjek.com

JS:   throw new Error("错误信息");
来源：http://wgg.shanyushiyangkeji.top

TS:   throw new Error("错误信息");
来源：http://ufw.xuanzx.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://tqk.yongpay.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qrp.316326.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://bhr.fzhhl.top

C#:   throw new ArgumentException("错误信息");
来源：http://hkh.9152youxi.cn

[H04] 自定义异常类型
来源：http://lio.gzhubu.top

Py:   class MyError(Exception): pass
来源：http://hkf.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://cfs.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://sys.shanyushiyangtech.top

TS:   class MyError extends Error {}
来源：http://ciq.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://czw.yj20258.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dow.dashuyun.cn

Ruby: class MyError < StandardError; end
来源：http://yel.epnwcf.com

C#:   class MyException : Exception {}
来源：http://txl.fktsv.cn

[H05] 捕获特定类型
来源：http://hau.yuxming.cn

Py:   except ValueError as e:
来源：http://pbm.hnqzz.top


<!-- 参考信息 -->