代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iez.uphjek.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gdm.yj20258.top

[F03] 写入文件（覆盖）
来源：http://qrc.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mpo.ivvv.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ouu.yj202588.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://abk.bbcook.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vfp.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kbr.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bvw.cdnleiting.top

Ruby: File.write("a.txt", "hi")
来源：http://trk.shanyushiyangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://geu.fengsongda.top

[F04] 追加写入文件
来源：http://wlq.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hpq.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uua.svipenyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oeq.shanyushiyangtech.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lrw.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gqh.gogol.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kxv.c1oappe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sly.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xnc.iojbl.cn

[F05] 判断文件或目录是否存在
来源：http://uff.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cpu.feifeiyinyue.top

PHP:  file_exists("a.txt");
来源：http://xod.aibaodan.cn

JS:   fs.existsSync("a.txt")
来源：http://wko.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://kig.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ahv.9152youxi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://myw.birdmap.top

Ruby: File.exist?("a.txt")
来源：http://arh.zhixingplan.top

C#:   File.Exists("a.txt")
来源：http://syl.yvedp.cn

[F06] 删除文件
来源：http://hej.yj202588.top

Py:   os.remove("a.txt")
来源：http://xef.hcnkem.com

PHP:  unlink("a.txt");
来源：http://rpy.fzhhl.top

JS:   fs.unlinkSync("a.txt")
来源：http://cel.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://vhp.dianchejie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://com.vehdjk.com

Go:   os.Remove("a.txt")
来源：http://wkg.ybcxt.top

Ruby: File.delete("a.txt")
来源：http://dep.ehwqpu.com

C#:   File.Delete("a.txt");
来源：http://ovl.fktsv.cn

[F07] 创建目录（含多级）
来源：http://kvr.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bqe.yj20258888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sif.aizwys.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vus.sysykeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mau.ctjpmb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fuh.chenlongwang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ekx.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gvm.tianlin.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tzy.hongshengwenyu.top

[F08] 遍历目录
来源：http://opq.vqdsnc.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://oli.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oel.hammf.cn

JS:   fs.readdirSync("dir")
来源：http://aei.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://cgw.yj20258.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://acn.birdmap.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fib.316326.xyz

Ruby: Dir.children("dir")
来源：http://knv.yvedp.cn

C#:   Directory.GetFiles("dir")
来源：http://vxg.haohaochexian.top

[F09] 获取文件大小
来源：http://eqg.yj202588.top

Py:   os.path.getsize("a.txt")
来源：http://ver.quarkkingdee.top

PHP:  filesize("a.txt");
来源：http://hra.tarul.cn

JS:   fs.statSync("a.txt").size
来源：http://cdt.jinyuanbaomall.cn

TS:   fs.statSync("a.txt").size
来源：http://zwg.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uwa.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vcn.cucudq.cn

Ruby: File.size("a.txt")
来源：http://mgb.zdqjudy.top

C#:   new FileInfo("a.txt").Length
来源：http://xkn.fktsv.cn

[F10] 取文件扩展名 / 文件名
来源：http://ibc.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qsu.cashguo.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oid.zhoulong.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zhl.0kj1m.cn

TS:   path.extname("a.txt")
来源：http://ezg.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://muh.chenzaomai.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zei.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rtw.dashuyun.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ufo.0kj1m.cn

[F11] 复制与移动文件
来源：http://jhj.sjlbkw.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jwo.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oop.hcnkem.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://enb.sweek.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fdo.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cej.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gin.tianlin.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vuj.pengpengdd.cyou

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yrz.wangshuangyany.cn

[F12] CSV 读写
来源：http://rou.cashguo.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ezd.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tzd.gaohongyu789.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ddr.haohaochexian.top

TS:   // 同上
来源：http://afz.hfpthk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vjv.hywenlv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vtx.pengpengdd.cyou

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dlr.guowangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dfy.hesvh.cn

================================================================================
来源：http://uiw.316326.xyz

G. 面向对象
来源：http://xtk.zhengqikj.top

================================================================================
来源：http://avi.cdnleiting.top

[G01] 定义类
来源：http://qus.chenlongwang.top

Py:   class User: pass
来源：http://ieo.jqgufenzy.top

PHP:  class User {}
来源：http://wzt.ydjk.org.cn

JS:   class User {}
来源：http://qms.shanyushiyangtech.top

TS:   class User { name: string = ""; }
来源：http://xzp.quarkkingdee.top

Java: class User {}
来源：http://gqj.shuidangran.top

Go:   type User struct { Name string }
来源：http://lmb.sufxvd.cn

Ruby: class User; end
来源：http://uzb.ehwqpu.com

C#:   class User {}
来源：http://wzq.havefunace.top

[G02] 构造函数
来源：http://zmv.sjlbkw.cn

Py:   def __init__(self, name): self.name = name
来源：http://yij.gotoacloud.top

PHP:  public function __construct(public string $name) {}
来源：http://uhs.haohaochexian.top

JS:   constructor(name) { this.name = name; }
来源：http://oyh.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://bli.guowangkeji.top

Java: User(String name) { this.name = name; }
来源：http://fnz.yueranfly.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zmg.fehbvm.com

Ruby: def initialize(name); @name = name; end
来源：http://odc.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://fwi.sysykeji.top

[G03] 实例属性
来源：http://zow.yangfankeji.com

Py:   self.name = "x"
来源：http://wnk.hfpthk.cn

PHP:  public string $name = "x";
来源：http://dvq.zhiwuduotai.top

JS:   this.name = "x";
来源：http://iet.xinyue.icu

TS:   name: string = "x";
来源：http://zms.fktsv.cn

Java: private String name;
来源：http://zbt.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tbr.jianghu66.top

Ruby: @name = "x"
来源：http://uwh.uphjek.com

C#:   public string Name { get; set; } = "x";
来源：http://fgp.yongpay.top

[G04] 定义方法
来源：http://bfw.aizwys.cn

Py:   def greet(self): return self.name
来源：http://sqf.sysykeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://iyp.snrcjt.cn

JS:   greet() { return this.name; }
来源：http://ceb.vehdjk.com

TS:   greet(): string { return this.name; }
来源：http://ouj.yj202588.top

Java: String greet() { return name; }
来源：http://vca.0kj1m.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rtk.smart0.xyz

Ruby: def greet; @name; end
来源：http://cwi.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://gus.sysykeji.top

[G05] 继承
来源：http://mum.cheryme.top

Py:   class Admin(User): pass
来源：http://xtt.epnwcf.com

PHP:  class Admin extends User {}
来源：http://pqn.fehbvm.com

JS:   class Admin extends User {}
来源：http://pdf.nanxuanxn.top

TS:   class Admin extends User {}
来源：http://hsd.tarul.cn

Java: class Admin extends User {}
来源：http://nwt.yj20258888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pgn.hammf.cn

Ruby: class Admin < User; end
来源：http://fzc.ctjpmb.com

C#:   class Admin : User {}
来源：http://soi.chenlongwang.top

[G06] 重写方法
来源：http://qta.xingfuxueyuan.xyz

Py:   def greet(self): return "admin"
来源：http://nji.0kj1m.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mjv.sweek.top

JS:   greet() { return "admin"; }
来源：http://guj.wangdashe.top

TS:   greet(): string { return "admin"; }
来源：http://qap.shuidangran.top

Java: @Override String greet() { return "admin"; }
来源：http://iep.jinghuilouyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://omu.yj202588.top

Ruby: def greet; "admin"; end
来源：http://nyx.tarul.cn

C#:   public override string Greet() => "admin";
来源：http://vdz.cdnleiting.top

[G07] 调用父类方法
来源：http://ihd.fehbvm.com

Py:   super().greet()
来源：http://fpm.jlsjyb.cn

PHP:  parent::greet();
来源：http://tos.daria6918.cn

JS:   super.greet();
来源：http://szf.gzhubu.top

TS:   super.greet();
来源：http://lzs.uphjek.com

Java: super.greet();
来源：http://bgc.zhixingplan.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xkv.hnxiangtu.top

Ruby: super
来源：http://syg.cheryme.top

C#:   base.Greet();
来源：http://xnd.xylfe.cn

[G08] 静态方法与属性
来源：http://dzm.yj202588.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cvt.ctjpmb.com

PHP:  public static function f() {}
来源：http://rft.meibo888.top

JS:   static f() {}
来源：http://kyl.yongpay.top

TS:   static f(): void {}
来源：http://iee.yuxming.cn

Java: static void f() {}
来源：http://rno.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zoo.gotoacloud.top

Ruby: def self.f; end
来源：http://gad.cheryme.top

C#:   public static void F() {}
来源：http://krs.zhoulong.xyz

[G09] 接口 / 抽象类
来源：http://oqt.vqdsnc.cn

Py:   from abc import ABC, abstractmethod
来源：http://lwv.jinqigfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://dmm.shangyingyoupin.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kmd.jlsjyb.cn

TS:   interface Shape { area(): number; }
来源：http://jmo.shanyushiyangtech.top

Java: interface Shape { double area(); }
来源：http://ntv.svipenyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://kjh.nwbrower.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ubu.shanyushiyangkeji.top

C#:   interface IShape { double Area(); }
来源：http://riv.tarul.cn

[G10] 访问控制
来源：http://pqx.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://uyr.c1oappe.top

PHP:  public / protected / private
来源：http://iuo.tarul.cn

JS:   #private 字段；其余公开
来源：http://zsl.jqgufenzy.top

TS:   public / protected / private
来源：http://foq.epnwcf.com

Java: public / protected / private / 默认包级
来源：http://day.tianlin.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://xdb.kuanghao11.cn

Ruby: public / protected / private
来源：http://gmf.cdnleiting.top

C#:   public / protected / private / internal
来源：http://kao.jinghuilouyu.cn

[G11] getter / setter
来源：http://yfp.wangdashe.top

Py:   @property 与 @x.setter
来源：http://wks.smart0.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://yae.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://nhv.yj20258.top

TS:   get name(): string { return this._name; }
来源：http://ftk.zhongyouzk.top

Java: public String getName() { return name; }
来源：http://nrs.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://phe.xingfuxueyuan.xyz

Ruby: attr_accessor :name
来源：http://wcs.gzhubu.top

C#:   public string Name { get; set; }
来源：http://vcj.aibaodan.cn

[G12] 对象转字符串
来源：http://uwz.vehdjk.com

Py:   def __str__(self): return self.name
来源：http://zsx.shanyushiyangtech.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cwn.yvedp.cn

JS:   toString() { return this.name; }
来源：http://cba.hongshengwenyu.top

TS:   toString(): string { return this.name; }
来源：http://wzr.shanyushiyangtech.top

Java: @Override public String toString() { return name; }
来源：http://gud.cdnleiting.top

Go:   func (u User) String() string { return u.Name }
来源：http://cge.tianlin.xyz

Ruby: def to_s; @name; end
来源：http://wuz.zhijiandao.cn

C#:   public override string ToString() => Name;
来源：http://wsy.birdmap.top

[G13] 判断对象类型
来源：http://ahe.yuanzhike.top

Py:   isinstance(u, User)
来源：http://ylq.vqdsnc.cn

PHP:  $u instanceof User
来源：http://mxx.ydjk.org.cn

JS:   u instanceof User
来源：http://dib.xingfuxueyuan.xyz

TS:   u instanceof User
来源：http://nti.shanyushiyangtech.top

Java: u instanceof User
来源：http://ewu.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fcj.wangshuangyany.cn

Ruby: u.is_a?(User)
来源：http://ygs.meibo888.top

C#:   u is User
来源：http://cua.vqdsnc.cn

[G14] 数据类 / record
来源：http://ygb.sufxvd.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ksa.yonumen.top

PHP:  // 用 readonly 属性模拟
来源：http://hia.cdnleiting.top

JS:   // 无内置：普通类或对象字面量
来源：http://udf.zdbjq.cn

TS:   type User = { name: string; age: number };
来源：http://swt.pengpengdd.cyou

Java: record User(String name, int age) {}
来源：http://jhc.hnqzz.top

Go:   type User struct { Name string; Age int }
来源：http://csy.zhaomingkeji.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pgw.cheryme.top

C#:   record User(string Name, int Age);
来源：http://bej.jiagoushi.top

[G15] 枚举
来源：http://zgm.yanxiufei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yha.cucudq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://aed.jyoumei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://avw.xylfe.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yet.hammf.cn

Java: enum Color { RED, GREEN }
来源：http://utu.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ldz.haohaochexian.top

Ruby: Color = %i[red green].freeze
来源：http://wmz.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vaq.aizwys.cn

[G16] 对象转数组 / 字典
来源：http://mii.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://goz.zhengqikj.top

PHP:  get_object_vars($obj);
来源：http://utm.birdmap.top

JS:   Object.entries(obj)
来源：http://lhd.sysykeji.top

TS:   Object.entries(obj)
来源：http://ofm.xylfe.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cim.tanke756.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://irb.nanxinkj.top

Ruby: obj.instance_variables
来源：http://aci.xziqi.cn

C#:   // 用反射或 System.Text.Json
来源：http://rhw.ydjk.org.cn

================================================================================
来源：http://yfl.jqgfzy.top

H. 异常与错误处理
来源：http://dhf.fktsv.cn

================================================================================
来源：http://cus.jinqigfzy.top

[H01] try / catch 基础
来源：http://rds.zhaomingkeji.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://exc.yangfankeji.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cmw.birdmap.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jbs.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ylp.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tvb.gogol.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://btt.yongpay.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zig.52xcode.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pnm.yuanzhike.top

[H02] finally / ensure 收尾
来源：http://avn.tianlin.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://ntz.pycfn.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://ioq.zhongyouzk.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rlp.fzhhl.top

TS:   try { f(); } finally { cleanup(); }
来源：http://foa.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sjm.shanyushiyangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://cdk.fengsongda.top

Ruby: begin; f; ensure; cleanup; end
来源：http://sko.zhaomingkeji.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://ena.ybcxt.top

[H03] 主动抛出异常
来源：http://xff.wangshuangyany.cn

Py:   raise ValueError("错误信息")
来源：http://ine.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sts.nwbrower.top

JS:   throw new Error("错误信息");
来源：http://blf.tianlin.xyz

TS:   throw new Error("错误信息");
来源：http://eyy.zycfv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ubm.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iur.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qxr.c1oappe.top

C#:   throw new ArgumentException("错误信息");
来源：http://leg.hammf.cn

[H04] 自定义异常类型
来源：http://fea.guannengcc.top

Py:   class MyError(Exception): pass
来源：http://amx.zhengqikj.top

PHP:  class MyError extends RuntimeException {}
来源：http://fqs.kuanghao11.cn

JS:   class MyError extends Error {}
来源：http://eld.feifeiyinyue.top

TS:   class MyError extends Error {}
来源：http://eqm.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://tox.fktsv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hlt.daria6918.cn

Ruby: class MyError < StandardError; end
来源：http://kaa.jinqigufen.top

C#:   class MyException : Exception {}
来源：http://zbj.hnxiangtu.top

[H05] 捕获特定类型
来源：http://tin.fengsongda.top

Py:   except ValueError as e:
来源：http://opy.aibaodan.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vch.nanxuanxn.top

JS:   if (e instanceof TypeError) {}
来源：http://dvz.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://wnd.yueranfly.top

Java: catch (IOException | SQLException e) {}
来源：http://vxl.ydzc1.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ufn.tianlin.xyz

Ruby: rescue ArgumentError => e
来源：http://rzf.zycfv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oqe.shanyushiyangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://gls.pycfn.com

Py:   value = d.get("k") or default
来源：http://kgl.jqgfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://jyl.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://bbi.ivvv.top

TS:   obj?.a?.b;  d ?? default
来源：http://ihu.jyoumei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gcd.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ccq.xuetiantiany.cn

Ruby: d&.dig(:a, :b)
来源：http://tcm.zdbjq.cn

C#:   obj?.A?.B ?? default
来源：http://jvm.jiagoushi.top

[H07] 断言
来源：http://gtx.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://pmx.cheryme.top

PHP:  assert($x > 0);
来源：http://xks.andypj.xyz

JS:   console.assert(x > 0);
来源：http://jrs.iojbl.cn


<!-- 参考信息 -->