代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://saq.wangshuangyany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rhe.zdbjq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://smk.gaohongyu789.top

Ruby: File.read("a.txt")
来源：http://wox.nanxuanxn.top

C#:   File.ReadAllText("a.txt");
来源：http://wpq.zhijiandao.cn

[F02] 逐行读取文件
来源：http://wyv.jianghu66.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://afs.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ylr.havefunace.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mvr.zhongyouzk.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dlm.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ulg.jinqigfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ong.hcnkem.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ugv.nanxuanxn.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eai.xziqi.cn

[F03] 写入文件（覆盖）
来源：http://tcu.pycfn.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vyu.yuanzhike.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ima.sjlbkw.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ccq.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ieo.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://psc.andypj.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wut.jinqigufen.top

Ruby: File.write("a.txt", "hi")
来源：http://jaz.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://odl.epnwcf.com

[F04] 追加写入文件
来源：http://hzn.gzhubu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ocx.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rbu.bjfxy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nds.havefunace.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zsj.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mnp.snrcjt.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xgv.bbcook.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hjt.xinyue.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ipj.gotoacloud.top

[F05] 判断文件或目录是否存在
来源：http://ynn.wangshuangyany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xuq.fzhhl.top

PHP:  file_exists("a.txt");
来源：http://yht.vehdjk.com

JS:   fs.existsSync("a.txt")
来源：http://qak.tanke756.top

TS:   fs.existsSync("a.txt")
来源：http://nnt.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://xff.zhijiandao.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://okm.aizwys.cn

Ruby: File.exist?("a.txt")
来源：http://uua.yj20258.top

C#:   File.Exists("a.txt")
来源：http://sds.tanke756.top

[F06] 删除文件
来源：http://esc.pengpengdd.cyou

Py:   os.remove("a.txt")
来源：http://bjj.nwbrower.top

PHP:  unlink("a.txt");
来源：http://yed.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://xig.sxryk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wun.dashuyun.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cfo.0kj1m.cn

Go:   os.Remove("a.txt")
来源：http://irz.fanxiaobao.xyz

Ruby: File.delete("a.txt")
来源：http://wql.ppjwa.cn

C#:   File.Delete("a.txt");
来源：http://edi.yfazqb.com

[F07] 创建目录（含多级）
来源：http://dip.ehwqpu.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uyt.birdmap.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gww.hongshengwenyu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dto.ppjwa.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fyc.andypj.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bkc.yuxming.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ctq.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zxx.zhixingplan.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qox.daria6918.cn

[F08] 遍历目录
来源：http://zni.mhx1999.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ufs.mhx1999.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://box.sjlbkw.cn

JS:   fs.readdirSync("dir")
来源：http://pik.yongpay.top

TS:   fs.readdirSync("dir")
来源：http://wwv.aibaodan.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wyp.dianchejie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yxy.andypj.xyz

Ruby: Dir.children("dir")
来源：http://lju.zhengqikj.top

C#:   Directory.GetFiles("dir")
来源：http://isw.yj20258.top

[F09] 获取文件大小
来源：http://wfj.gaohongyu789.top

Py:   os.path.getsize("a.txt")
来源：http://ato.jianghu66.top

PHP:  filesize("a.txt");
来源：http://mhe.nwbrower.top

JS:   fs.statSync("a.txt").size
来源：http://msf.hammf.cn

TS:   fs.statSync("a.txt").size
来源：http://dgg.shangyingyoupin.top

Java: Files.size(Path.of("a.txt"))
来源：http://gyc.zycfv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://usl.xinyue.icu

Ruby: File.size("a.txt")
来源：http://wkd.nwbrower.top

C#:   new FileInfo("a.txt").Length
来源：http://nmi.ehwqpu.com

[F10] 取文件扩展名 / 文件名
来源：http://irp.smart0.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qmh.hfpthk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rvr.guannengcc.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oad.tanke756.top

TS:   path.extname("a.txt")
来源：http://djm.shanyushiyangtech.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xco.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jwq.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zsc.sjlbkw.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ksh.fzhhl.top

[F11] 复制与移动文件
来源：http://oha.shuidangran.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bol.hesvh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://awd.yuanzhike.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://abq.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lbd.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vme.yongpay.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mjw.nanxinkj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eaz.jiagoushi.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mro.sysykeji.top

[F12] CSV 读写
来源：http://yaf.yueranfly.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hqc.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dvi.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ggb.hesvh.cn

TS:   // 同上
来源：http://hvw.tanke756.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zky.chenjidiqi.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://avm.andypj.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oxw.wangshuangyany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://giy.zhixingplan.top

================================================================================
来源：http://ohk.redwolf501.top

G. 面向对象
来源：http://inp.zdqjudy.top

================================================================================
来源：http://wge.shangyingyoupin.top

[G01] 定义类
来源：http://rob.fanxiaobao.xyz

Py:   class User: pass
来源：http://ynf.havefunace.top

PHP:  class User {}
来源：http://rkv.ydjk.org.cn

JS:   class User {}
来源：http://ice.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://vuu.daria6918.cn

Java: class User {}
来源：http://cwh.haohaochexian.top

Go:   type User struct { Name string }
来源：http://ejk.quarkkingdee.top

Ruby: class User; end
来源：http://ufr.cqqwz.cn

C#:   class User {}
来源：http://teh.tanke756.top

[G02] 构造函数
来源：http://soh.jinqigufen.top

Py:   def __init__(self, name): self.name = name
来源：http://zqf.tian-w.cn

PHP:  public function __construct(public string $name) {}
来源：http://kpw.haohaochexian.top

JS:   constructor(name) { this.name = name; }
来源：http://adu.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://mqe.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://dfp.guowangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tms.hongshengwenyu.top

Ruby: def initialize(name); @name = name; end
来源：http://zwm.yvedp.cn

C#:   public User(string name) { Name = name; }
来源：http://vql.chenlongwang.top

[G03] 实例属性
来源：http://lzo.iojbl.cn

Py:   self.name = "x"
来源：http://qvv.hammf.cn

PHP:  public string $name = "x";
来源：http://awj.daria6918.cn

JS:   this.name = "x";
来源：http://xro.xylfe.cn

TS:   name: string = "x";
来源：http://yib.hysaishi.cn

Java: private String name;
来源：http://mzm.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fbj.ywan-chungtsiang.top

Ruby: @name = "x"
来源：http://fld.cqqwz.cn

C#:   public string Name { get; set; } = "x";
来源：http://upl.cqqwz.cn

[G04] 定义方法
来源：http://pva.zhengqikj.top

Py:   def greet(self): return self.name
来源：http://ppt.vehdjk.com

PHP:  public function greet(): string { return $this->name; }
来源：http://muv.bbcook.cn

JS:   greet() { return this.name; }
来源：http://axq.zhijiandao.cn

TS:   greet(): string { return this.name; }
来源：http://hbn.pengpengdd.cyou

Java: String greet() { return name; }
来源：http://dfr.shzxlz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fen.feifeiyinyue.top

Ruby: def greet; @name; end
来源：http://oam.yonumen.top

C#:   public string Greet() => Name;
来源：http://grp.hywenlv.cn

[G05] 继承
来源：http://ttg.hesvh.cn

Py:   class Admin(User): pass
来源：http://hcc.c1oappe.top

PHP:  class Admin extends User {}
来源：http://vua.cheryme.top

JS:   class Admin extends User {}
来源：http://bug.uphjek.com

TS:   class Admin extends User {}
来源：http://zuy.tarul.cn

Java: class Admin extends User {}
来源：http://dbh.zycfv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rbp.yj20258888.top

Ruby: class Admin < User; end
来源：http://siq.gogol.net.cn

C#:   class Admin : User {}
来源：http://mzt.yonumen.top

[G06] 重写方法
来源：http://wuf.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://yty.hnxiangtu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mwx.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://lml.fengsongda.top

TS:   greet(): string { return "admin"; }
来源：http://kyl.gzhubu.top

Java: @Override String greet() { return "admin"; }
来源：http://czw.xuetiantiany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lfa.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://uab.svipenyu.cn

C#:   public override string Greet() => "admin";
来源：http://zrh.pycfn.com

[G07] 调用父类方法
来源：http://zwt.iojbl.cn

Py:   super().greet()
来源：http://iji.zhiwuduotai.top

PHP:  parent::greet();
来源：http://thj.52xcode.cn

JS:   super.greet();
来源：http://bef.gotoacloud.top

TS:   super.greet();
来源：http://cel.ywan-chungtsiang.top

Java: super.greet();
来源：http://ntj.hammf.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://upj.gogol.net.cn

Ruby: super
来源：http://uhy.jinqigufen.top

C#:   base.Greet();
来源：http://fzw.zdqjudy.top

[G08] 静态方法与属性
来源：http://kuo.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gnp.zhongyouzk.top

PHP:  public static function f() {}
来源：http://sda.epnwcf.com

JS:   static f() {}
来源：http://hmn.haohaochexian.top

TS:   static f(): void {}
来源：http://ibd.aizwys.cn

Java: static void f() {}
来源：http://cgf.quarkkingdee.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zdi.chenlongwang.top

Ruby: def self.f; end
来源：http://cwv.birdmap.top

C#:   public static void F() {}
来源：http://cjx.aizwys.cn

[G09] 接口 / 抽象类
来源：http://dsc.hnqzz.top

Py:   from abc import ABC, abstractmethod
来源：http://ddy.ydzc1.top

PHP:  interface Shape { public function area(): float; }
来源：http://lki.hfpthk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uoj.vqdsnc.cn

TS:   interface Shape { area(): number; }
来源：http://wkd.feifeiyinyue.top

Java: interface Shape { double area(); }
来源：http://vck.ppjwa.cn

Go:   type Shape interface { Area() float64 }
来源：http://vbc.svipenyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jyx.zdbjq.cn

C#:   interface IShape { double Area(); }
来源：http://jpy.yueranfly.top

[G10] 访问控制
来源：http://abs.vehdjk.com

Py:   约定 _protected / __private（不强制）
来源：http://qdj.aizwys.cn

PHP:  public / protected / private
来源：http://xix.jinqigufen.top

JS:   #private 字段；其余公开
来源：http://sam.snrcjt.cn

TS:   public / protected / private
来源：http://fap.jlsjyb.cn

Java: public / protected / private / 默认包级
来源：http://ayu.yvedp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://aoh.yj20258.top

Ruby: public / protected / private
来源：http://ecu.xziqi.cn

C#:   public / protected / private / internal
来源：http://okn.jiagoushi.top

[G11] getter / setter
来源：http://ifb.uphjek.com

Py:   @property 与 @x.setter
来源：http://gte.sysykeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bpl.quarkkingdee.top

JS:   get name() { return this._name; }
来源：http://dcs.hammf.cn

TS:   get name(): string { return this._name; }
来源：http://acy.haohaochexian.top

Java: public String getName() { return name; }
来源：http://yjk.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ope.nwbrower.top

Ruby: attr_accessor :name
来源：http://ktd.yuanzhike.top

C#:   public string Name { get; set; }
来源：http://cwx.nanxuanxn.top

[G12] 对象转字符串
来源：http://fps.fktsv.cn

Py:   def __str__(self): return self.name
来源：http://men.shanyushiyangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mft.52xcode.cn

JS:   toString() { return this.name; }
来源：http://axb.hesvh.cn

TS:   toString(): string { return this.name; }
来源：http://gkw.dianchejie.cn

Java: @Override public String toString() { return name; }
来源：http://zdw.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://zlm.tian-w.cn

Ruby: def to_s; @name; end
来源：http://abo.hywenlv.cn

C#:   public override string ToString() => Name;
来源：http://dog.hnxiangtu.top

[G13] 判断对象类型
来源：http://jlp.daxiang520.top

Py:   isinstance(u, User)
来源：http://uuh.uphjek.com

PHP:  $u instanceof User
来源：http://ivv.xinyue.icu

JS:   u instanceof User
来源：http://uky.mhx1999.top

TS:   u instanceof User
来源：http://jzf.dashuyun.cn

Java: u instanceof User
来源：http://yhm.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ldo.yongpay.top

Ruby: u.is_a?(User)
来源：http://scc.yonumen.top

C#:   u is User
来源：http://sbn.hcnkem.com

[G14] 数据类 / record
来源：http://tqy.zhiwuduotai.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xdo.kuanghao11.cn

PHP:  // 用 readonly 属性模拟
来源：http://mhe.wangdashe.top

JS:   // 无内置：普通类或对象字面量
来源：http://yqd.yj202588.top

TS:   type User = { name: string; age: number };
来源：http://ciq.yuxming.cn

Java: record User(String name, int age) {}
来源：http://aws.guannengcc.top

Go:   type User struct { Name string; Age int }
来源：http://djy.xuanzx.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uvp.ydjk.org.cn

C#:   record User(string Name, int Age);
来源：http://kzb.andypj.xyz

[G15] 枚举
来源：http://hav.zdqjudy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zqt.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pyq.bbcook.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zzy.jyoumei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tnu.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://owd.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://son.yvedp.cn

Ruby: Color = %i[red green].freeze
来源：http://sgj.jinyuanbaomall.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wlh.yueranfly.top

[G16] 对象转数组 / 字典
来源：http://cdq.shangyingyoupin.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://udr.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://vki.ppjwa.cn

JS:   Object.entries(obj)
来源：http://nik.tianlin.xyz

TS:   Object.entries(obj)
来源：http://pzr.ivvv.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bht.fanxiaobao.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://yaq.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://tyl.epnwcf.com

C#:   // 用反射或 System.Text.Json
来源：http://oqk.daxiang520.top

================================================================================
来源：http://ddf.andypj.xyz

H. 异常与错误处理
来源：http://ljz.jlsjyb.cn

================================================================================
来源：http://czl.smart0.xyz

[H01] try / catch 基础
来源：http://btm.bjfxy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iyr.jianghu66.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lbm.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gzp.zhaomingkeji.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://izz.9152youxi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fza.fehbvm.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cat.tarul.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uyg.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fwa.hnxiangtu.top

[H02] finally / ensure 收尾
来源：http://cdy.sweek.top

Py:   try: f()⏎finally: cleanup()
来源：http://kks.hywenlv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gxd.yuanzhike.top

JS:   try { f(); } finally { cleanup(); }
来源：http://npi.ydzc1.top

TS:   try { f(); } finally { cleanup(); }
来源：http://par.zdbjq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://abm.quarkkingdee.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hkw.havefunace.top

Ruby: begin; f; ensure; cleanup; end
来源：http://opf.cucudq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ypf.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://yor.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://thr.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bjc.jiagoushi.top

JS:   throw new Error("错误信息");
来源：http://sag.tarul.cn

TS:   throw new Error("错误信息");
来源：http://zou.yuanzhike.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pth.bjfxy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://szj.zycfv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://giq.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://osg.zhiwuduotai.top

[H04] 自定义异常类型
来源：http://duv.ivvv.top

Py:   class MyError(Exception): pass
来源：http://ibu.yangfankeji.com

PHP:  class MyError extends RuntimeException {}
来源：http://jzq.tarul.cn

JS:   class MyError extends Error {}
来源：http://utt.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://nsz.sxryk.cn

Java: class MyException extends RuntimeException {}
来源：http://bpu.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hmf.meibo888.top

Ruby: class MyError < StandardError; end
来源：http://viy.dashuyun.cn

C#:   class MyException : Exception {}
来源：http://ujh.zhengqikj.top

[H05] 捕获特定类型
来源：http://vxi.vehdjk.com

Py:   except ValueError as e:
来源：http://jfx.jianghu66.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wih.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://lyj.shuidangran.top

TS:   if (e instanceof TypeError) {}
来源：http://xvu.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://hnb.cdnleiting.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xel.yj20258888.top

Ruby: rescue ArgumentError => e
来源：http://ntm.aizwys.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://khs.yuanzhike.top

[H06] 可选值 / 空值安全访问
来源：http://pqg.xziqi.cn


<!-- 参考信息 -->