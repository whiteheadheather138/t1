代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://crh.haohaochexian.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ije.0kj1m.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vuh.redwolf501.top

Ruby: File.read("a.txt")
来源：http://vrx.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://chw.9152youxi.cn

[F02] 逐行读取文件
来源：http://ovb.cheryme.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ldh.guowangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xjx.yj20258.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://evh.xinyue.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iur.andypj.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://inl.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mja.yanxiufei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jmk.vqdsnc.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://heg.hnxiangtu.top

[F03] 写入文件（覆盖）
来源：http://dsk.chenlongwang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lxm.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qme.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rqq.sxryk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://guq.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oww.fktsv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ymu.vehdjk.com

Ruby: File.write("a.txt", "hi")
来源：http://kmm.shuidangran.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://udw.yangfankeji.com

[F04] 追加写入文件
来源：http://mph.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qnb.guannengcc.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://brm.cheryme.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tte.nanxinkj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vlt.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kji.cdnleiting.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fpi.jinqigfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dhk.cqqwz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ofl.xingfuxueyuan.xyz

[F05] 判断文件或目录是否存在
来源：http://ypx.c1oappe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xpi.xuetiantiany.cn

PHP:  file_exists("a.txt");
来源：http://tsh.quarkkingdee.top

JS:   fs.existsSync("a.txt")
来源：http://zae.yonumen.top

TS:   fs.existsSync("a.txt")
来源：http://yho.svipenyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fjc.nwbrower.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bkb.hfpthk.cn

Ruby: File.exist?("a.txt")
来源：http://ulb.sweek.top

C#:   File.Exists("a.txt")
来源：http://aml.jinyuanbaomall.cn

[F06] 删除文件
来源：http://vfd.jinqigfzy.top

Py:   os.remove("a.txt")
来源：http://hcw.yj202588.top

PHP:  unlink("a.txt");
来源：http://oqj.fktsv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qyb.haohaochexian.top

TS:   fs.unlinkSync("a.txt")
来源：http://rmt.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vmh.guannengcc.top

Go:   os.Remove("a.txt")
来源：http://qbg.yj202588.top

Ruby: File.delete("a.txt")
来源：http://cro.hammf.cn

C#:   File.Delete("a.txt");
来源：http://hvb.kuanghao11.cn

[F07] 创建目录（含多级）
来源：http://qzr.bbcook.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xkz.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eyx.hcnkem.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cpk.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qhj.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ldn.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://inu.shangyingyoupin.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://liw.gaohongyu789.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hri.nwbrower.top

[F08] 遍历目录
来源：http://ogt.ppjwa.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uhg.jinqigfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hlm.dianchejie.cn

JS:   fs.readdirSync("dir")
来源：http://rki.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://ybj.ppjwa.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rxh.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fhe.hywenlv.cn

Ruby: Dir.children("dir")
来源：http://kze.hnxiangtu.top

C#:   Directory.GetFiles("dir")
来源：http://ixn.tarul.cn

[F09] 获取文件大小
来源：http://pox.chenjidiqi.icu

Py:   os.path.getsize("a.txt")
来源：http://yxx.tarul.cn

PHP:  filesize("a.txt");
来源：http://gqm.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://nkq.yj20258.top

TS:   fs.statSync("a.txt").size
来源：http://dkh.yueranfly.top

Java: Files.size(Path.of("a.txt"))
来源：http://sng.redwolf501.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xqo.dianchejie.cn

Ruby: File.size("a.txt")
来源：http://zto.cdnleiting.top

C#:   new FileInfo("a.txt").Length
来源：http://qsp.yangfankeji.com

[F10] 取文件扩展名 / 文件名
来源：http://cdu.svipenyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qpf.sysykeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lww.zdqjudy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lei.zhongyouzk.top

TS:   path.extname("a.txt")
来源：http://xep.haohaochexian.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mic.haohaochexian.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nsa.xuanzx.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iax.yj20258.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wfc.zdqjudy.top

[F11] 复制与移动文件
来源：http://tln.ctjpmb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://szp.jinghuilouyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zsk.svipenyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qxt.yanxiufei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cdy.zhaomingkeji.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wyc.sweek.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yxz.chenlongwang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ymq.zycfv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qyt.yongpay.top

[F12] CSV 读写
来源：http://zyv.tanke756.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eek.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gcd.sxryk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ror.dashuyun.cn

TS:   // 同上
来源：http://itu.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jpo.cdnleiting.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://azt.shzxlz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ico.sweek.top

C#:   // 无内置：用 CsvHelper 库
来源：http://yfs.epnwcf.com

================================================================================
来源：http://hcn.0kj1m.cn

G. 面向对象
来源：http://ici.shanyushiyangtech.top

================================================================================
来源：http://glz.zhongyouzk.top

[G01] 定义类
来源：http://ndt.hysaishi.cn

Py:   class User: pass
来源：http://hot.zhongyouzk.top

PHP:  class User {}
来源：http://wny.fanxiaobao.xyz

JS:   class User {}
来源：http://ocz.meibo888.top

TS:   class User { name: string = ""; }
来源：http://xvf.yueranfly.top

Java: class User {}
来源：http://nbc.jianghu66.top

Go:   type User struct { Name string }
来源：http://hgw.yj202588.top

Ruby: class User; end
来源：http://yzy.gotoacloud.top

C#:   class User {}
来源：http://jch.jyoumei.cn

[G02] 构造函数
来源：http://wsu.guowangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://twi.yongpay.top

PHP:  public function __construct(public string $name) {}
来源：http://cky.fanxiaobao.xyz

JS:   constructor(name) { this.name = name; }
来源：http://jzj.nanxuanxn.top

TS:   constructor(public name: string) {}
来源：http://fwz.jinghuilouyu.cn

Java: User(String name) { this.name = name; }
来源：http://zsu.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://brr.shanyushiyangtech.top

Ruby: def initialize(name); @name = name; end
来源：http://oix.9152youxi.cn

C#:   public User(string name) { Name = name; }
来源：http://wbd.jianghu66.top

[G03] 实例属性
来源：http://yeg.sufxvd.cn

Py:   self.name = "x"
来源：http://pnm.yongpay.top

PHP:  public string $name = "x";
来源：http://dff.feifeiyinyue.top

JS:   this.name = "x";
来源：http://pjd.c1oappe.top

TS:   name: string = "x";
来源：http://ywf.ppjwa.cn

Java: private String name;
来源：http://zxi.ehwqpu.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xvz.pycfn.com

Ruby: @name = "x"
来源：http://scr.redwolf501.top

C#:   public string Name { get; set; } = "x";
来源：http://ydi.gzhubu.top

[G04] 定义方法
来源：http://rdh.gzhubu.top

Py:   def greet(self): return self.name
来源：http://mze.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jep.redwolf501.top

JS:   greet() { return this.name; }
来源：http://yxq.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://syt.c1oappe.top

Java: String greet() { return name; }
来源：http://teg.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qvv.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://vem.ywan-chungtsiang.top

C#:   public string Greet() => Name;
来源：http://kll.gotoacloud.top

[G05] 继承
来源：http://tzi.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://ngc.hnqzz.top

PHP:  class Admin extends User {}
来源：http://hyw.yj20258.top

JS:   class Admin extends User {}
来源：http://fvv.jiagoushi.top

TS:   class Admin extends User {}
来源：http://bai.shanyushiyangtech.top

Java: class Admin extends User {}
来源：http://xdx.fengsongda.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ajz.cucudq.cn

Ruby: class Admin < User; end
来源：http://mup.jinqigufen.top

C#:   class Admin : User {}
来源：http://eyh.cashguo.top

[G06] 重写方法
来源：http://qwb.fehbvm.com

Py:   def greet(self): return "admin"
来源：http://bga.ydzc1.top

PHP:  public function greet(): string { return "admin"; }
来源：http://urp.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://rhs.hesvh.cn

TS:   greet(): string { return "admin"; }
来源：http://pix.birdmap.top

Java: @Override String greet() { return "admin"; }
来源：http://cqe.tanke756.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://acz.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://muv.xuetiantiany.cn

C#:   public override string Greet() => "admin";
来源：http://fbu.hnqzz.top

[G07] 调用父类方法
来源：http://thr.jyoumei.cn

Py:   super().greet()
来源：http://hxg.svipenyu.cn

PHP:  parent::greet();
来源：http://ckz.xylfe.cn

JS:   super.greet();
来源：http://fda.ppjwa.cn

TS:   super.greet();
来源：http://yaf.dianchejie.cn

Java: super.greet();
来源：http://xtj.havefunace.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xnq.gogol.net.cn

Ruby: super
来源：http://omg.smart0.xyz

C#:   base.Greet();
来源：http://eul.daxiang520.top

[G08] 静态方法与属性
来源：http://thb.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mcm.mhx1999.top

PHP:  public static function f() {}
来源：http://wym.jqgfzy.top

JS:   static f() {}
来源：http://xwu.cheryme.top

TS:   static f(): void {}
来源：http://gwe.zhengqikj.top

Java: static void f() {}
来源：http://rgc.c1oappe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gtb.hysaishi.cn

Ruby: def self.f; end
来源：http://jxj.cucudq.cn

C#:   public static void F() {}
来源：http://npz.jianghu66.top

[G09] 接口 / 抽象类
来源：http://fyn.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://pgq.mhx1999.top

PHP:  interface Shape { public function area(): float; }
来源：http://bfq.ywan-chungtsiang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mwi.shuidangran.top

TS:   interface Shape { area(): number; }
来源：http://ysv.yj20258.top

Java: interface Shape { double area(); }
来源：http://kky.chenzaomai.com

Go:   type Shape interface { Area() float64 }
来源：http://kuo.jinqigufen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qgg.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://kvt.tian-w.cn

[G10] 访问控制
来源：http://urm.mhx1999.top

Py:   约定 _protected / __private（不强制）
来源：http://gtk.zhiwuduotai.top

PHP:  public / protected / private
来源：http://rnd.smart0.xyz

JS:   #private 字段；其余公开
来源：http://iui.epnwcf.com

TS:   public / protected / private
来源：http://jso.hcnkem.com

Java: public / protected / private / 默认包级
来源：http://wvv.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://guf.chenlongwang.top

Ruby: public / protected / private
来源：http://feq.zdqjudy.top

C#:   public / protected / private / internal
来源：http://ggs.smart0.xyz

[G11] getter / setter
来源：http://jhk.316326.xyz

Py:   @property 与 @x.setter
来源：http://mnh.hysaishi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://buu.vehdjk.com

JS:   get name() { return this._name; }
来源：http://ywv.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://qky.sufxvd.cn

Java: public String getName() { return name; }
来源：http://vld.svipenyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wva.jinyuanbaomall.cn

Ruby: attr_accessor :name
来源：http://kqp.kuanghao11.cn

C#:   public string Name { get; set; }
来源：http://wtt.nanxuanxn.top

[G12] 对象转字符串
来源：http://yng.cucudq.cn

Py:   def __str__(self): return self.name
来源：http://ngc.fktsv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gfy.pengpengdd.cyou

JS:   toString() { return this.name; }
来源：http://nxc.andypj.xyz

TS:   toString(): string { return this.name; }
来源：http://jtx.jqgfzy.top

Java: @Override public String toString() { return name; }
来源：http://zxo.havefunace.top

Go:   func (u User) String() string { return u.Name }
来源：http://zlj.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://roq.zhaomingkeji.xyz

C#:   public override string ToString() => Name;
来源：http://vig.wangshuangyany.cn

[G13] 判断对象类型
来源：http://moq.birdmap.top

Py:   isinstance(u, User)
来源：http://msr.hnxiangtu.top

PHP:  $u instanceof User
来源：http://uml.yj20258.top

JS:   u instanceof User
来源：http://tfe.quarkkingdee.top

TS:   u instanceof User
来源：http://zqx.gogol.net.cn

Java: u instanceof User
来源：http://fsh.redwolf501.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://laj.tian-w.cn

Ruby: u.is_a?(User)
来源：http://kla.hesvh.cn

C#:   u is User
来源：http://gvk.shangyingyoupin.top

[G14] 数据类 / record
来源：http://sna.chenzaomai.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uxm.guowangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://pqd.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://srv.0kj1m.cn

TS:   type User = { name: string; age: number };
来源：http://tly.pycfn.com

Java: record User(String name, int age) {}
来源：http://gjm.zhengqikj.top

Go:   type User struct { Name string; Age int }
来源：http://zhz.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kgf.xziqi.cn

C#:   record User(string Name, int Age);
来源：http://upi.zhoulong.xyz

[G15] 枚举
来源：http://caj.haohaochexian.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lbh.ywan-chungtsiang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nrx.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gqq.daxiang520.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ovf.gaohongyu789.top

Java: enum Color { RED, GREEN }
来源：http://qal.fengsongda.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ixf.fanxiaobao.xyz

Ruby: Color = %i[red green].freeze
来源：http://frq.xylfe.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nza.havefunace.top

[G16] 对象转数组 / 字典
来源：http://duj.chenzaomai.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xmy.feifeiyinyue.top

PHP:  get_object_vars($obj);
来源：http://lkn.meibo888.top

JS:   Object.entries(obj)
来源：http://dva.hywenlv.cn

TS:   Object.entries(obj)
来源：http://bji.chenlongwang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bwf.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nhs.yuanzhike.top

Ruby: obj.instance_variables
来源：http://ugz.fanxiaobao.xyz

C#:   // 用反射或 System.Text.Json
来源：http://uin.yj20258888.top

================================================================================
来源：http://xpm.jqgufenzy.top

H. 异常与错误处理
来源：http://ffc.shzxlz.cn

================================================================================
来源：http://nqv.svipenyu.cn

[H01] try / catch 基础
来源：http://jow.tianlin.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://usb.gotoacloud.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wkf.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lks.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zrs.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bcs.vqdsnc.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://szi.redwolf501.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pja.nanxuanxn.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kve.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://ogk.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://phr.hongshengwenyu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ezp.jyoumei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pst.jiagoushi.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ole.fanxiaobao.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://vnt.316326.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://uln.aizwys.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cdg.jinyuanbaomall.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ykb.nanxinkj.top

[H03] 主动抛出异常
来源：http://jsc.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://fwg.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ajw.shuidangran.top

JS:   throw new Error("错误信息");
来源：http://wri.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://roy.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://imy.cdnleiting.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uaa.kuanghao11.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ipr.yfazqb.com

C#:   throw new ArgumentException("错误信息");
来源：http://ysd.dashuyun.cn

[H04] 自定义异常类型
来源：http://gtm.sjlbkw.cn

Py:   class MyError(Exception): pass
来源：http://wjk.sweek.top

PHP:  class MyError extends RuntimeException {}
来源：http://ncm.shzxlz.cn

JS:   class MyError extends Error {}
来源：http://hix.tanke756.top

TS:   class MyError extends Error {}
来源：http://cis.fehbvm.com

Java: class MyException extends RuntimeException {}
来源：http://wzv.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nqi.xinyue.icu

Ruby: class MyError < StandardError; end
来源：http://iuj.gzhubu.top

C#:   class MyException : Exception {}
来源：http://rpn.hesvh.cn

[H05] 捕获特定类型
来源：http://ara.shangyingyoupin.top

Py:   except ValueError as e:
来源：http://fml.jinqigufen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dnx.dianchejie.cn

JS:   if (e instanceof TypeError) {}
来源：http://iwi.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://zat.vehdjk.com

Java: catch (IOException | SQLException e) {}
来源：http://ozh.xylfe.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fkt.tanke756.top

Ruby: rescue ArgumentError => e
来源：http://njy.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nbt.chenjidiqi.icu

[H06] 可选值 / 空值安全访问
来源：http://xvh.hysaishi.cn


<!-- 参考信息 -->