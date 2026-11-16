代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tht.jinqigfzy.top

================================================================================
来源：http://bjn.jinghuilouyu.cn

F. 文件与目录
来源：http://cko.zhengqikj.top

================================================================================
来源：http://nmt.birdmap.top

[F01] 读取整个文件
来源：http://tjk.jqgufenzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oph.jiagoushi.top

PHP:  file_get_contents("a.txt");
来源：http://jty.hysaishi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bez.epnwcf.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gmk.fktsv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mja.sysykeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rhz.vehdjk.com

Ruby: File.read("a.txt")
来源：http://ddh.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://skg.xuanzx.com

[F02] 逐行读取文件
来源：http://nvd.zdbjq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rri.tarul.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hcz.daxiang520.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ldm.ehwqpu.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ptv.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sxy.tanke756.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pyd.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zxe.vehdjk.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vku.hcnkem.com

[F03] 写入文件（覆盖）
来源：http://amb.chenlongwang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ygu.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tim.cqqwz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mof.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xrg.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://woi.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zof.bbcook.cn

Ruby: File.write("a.txt", "hi")
来源：http://cnd.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ohu.hongshengwenyu.top

[F04] 追加写入文件
来源：http://jdh.hcnkem.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nkq.cdnleiting.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://psf.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qzn.andypj.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mhy.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rwy.ivvv.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dkk.kuanghao11.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pma.chenjidiqi.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hrh.mhx1999.top

[F05] 判断文件或目录是否存在
来源：http://rnp.zhixingplan.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mvj.xingfuxueyuan.xyz

PHP:  file_exists("a.txt");
来源：http://qex.daria6918.cn

JS:   fs.existsSync("a.txt")
来源：http://rbd.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://dje.xuanzx.com

Java: Files.exists(Path.of("a.txt"))
来源：http://pjm.gaohongyu789.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jch.vqdsnc.cn

Ruby: File.exist?("a.txt")
来源：http://nya.nanxinkj.top

C#:   File.Exists("a.txt")
来源：http://tpr.xziqi.cn

[F06] 删除文件
来源：http://rkn.daxiang520.top

Py:   os.remove("a.txt")
来源：http://dqc.aizwys.cn

PHP:  unlink("a.txt");
来源：http://lkm.yfazqb.com

JS:   fs.unlinkSync("a.txt")
来源：http://pec.dashuyun.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zyb.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pma.hywenlv.cn

Go:   os.Remove("a.txt")
来源：http://web.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://aue.52xcode.cn

C#:   File.Delete("a.txt");
来源：http://ymn.vqdsnc.cn

[F07] 创建目录（含多级）
来源：http://csr.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aim.bbcook.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mjj.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dme.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aio.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nde.yongpay.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hmg.pycfn.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uaq.ydjk.org.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://esa.nwbrower.top

[F08] 遍历目录
来源：http://bac.dashuyun.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kuh.sufxvd.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dxi.sufxvd.cn

JS:   fs.readdirSync("dir")
来源：http://kzx.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://dbk.pycfn.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://env.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vth.chenjidiqi.icu

Ruby: Dir.children("dir")
来源：http://uqg.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://dtz.fanxiaobao.xyz

[F09] 获取文件大小
来源：http://htr.zdqjudy.top

Py:   os.path.getsize("a.txt")
来源：http://ekh.sjlbkw.cn

PHP:  filesize("a.txt");
来源：http://npo.feifeiyinyue.top

JS:   fs.statSync("a.txt").size
来源：http://ajo.kuanghao11.cn

TS:   fs.statSync("a.txt").size
来源：http://saf.nanxuanxn.top

Java: Files.size(Path.of("a.txt"))
来源：http://vtg.kuanghao11.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ogm.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://qtc.jqgfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://jzk.0kj1m.cn

[F10] 取文件扩展名 / 文件名
来源：http://xfb.vqdsnc.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ofv.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ioj.zhixingplan.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jdc.fzhhl.top

TS:   path.extname("a.txt")
来源：http://jxr.jlsjyb.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mmf.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sai.sxryk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mtm.zhiwuduotai.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tkb.xziqi.cn

[F11] 复制与移动文件
来源：http://lmt.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xdz.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uss.fktsv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ynf.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gsn.redwolf501.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ock.chenzaomai.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qrs.yongpay.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pkc.jinqigfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uhp.zhongyouzk.top

[F12] CSV 读写
来源：http://qtt.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ehu.tianlin.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zql.andypj.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nld.hysaishi.cn

TS:   // 同上
来源：http://jsn.hesvh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fbl.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xsh.jianghu66.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ytj.chenjidiqi.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://hrl.xziqi.cn

================================================================================
来源：http://ufc.ywan-chungtsiang.top

G. 面向对象
来源：http://ujz.zhaomingkeji.xyz

================================================================================
来源：http://ylv.chenlongwang.top

[G01] 定义类
来源：http://cwa.iojbl.cn

Py:   class User: pass
来源：http://kwi.haohaochexian.top

PHP:  class User {}
来源：http://efj.smart0.xyz

JS:   class User {}
来源：http://hiz.chenlongwang.top

TS:   class User { name: string = ""; }
来源：http://yfm.uphjek.com

Java: class User {}
来源：http://ixm.xuanzx.com

Go:   type User struct { Name string }
来源：http://sub.sjlbkw.cn

Ruby: class User; end
来源：http://qdo.bjfxy.top

C#:   class User {}
来源：http://ljc.zhengqikj.top

[G02] 构造函数
来源：http://kez.jyoumei.cn

Py:   def __init__(self, name): self.name = name
来源：http://pnk.shuidangran.top

PHP:  public function __construct(public string $name) {}
来源：http://ixp.sjlbkw.cn

JS:   constructor(name) { this.name = name; }
来源：http://fmw.bjfxy.top

TS:   constructor(public name: string) {}
来源：http://bjn.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://abl.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bce.hysaishi.cn

Ruby: def initialize(name); @name = name; end
来源：http://syr.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://lhx.haohaochexian.top

[G03] 实例属性
来源：http://dlq.fengsongda.top

Py:   self.name = "x"
来源：http://fuy.shuidangran.top

PHP:  public string $name = "x";
来源：http://dej.kuanghao11.cn

JS:   this.name = "x";
来源：http://gjl.yangfankeji.com

TS:   name: string = "x";
来源：http://qef.vehdjk.com

Java: private String name;
来源：http://jyg.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ptx.svipenyu.cn

Ruby: @name = "x"
来源：http://qia.xingfuxueyuan.xyz

C#:   public string Name { get; set; } = "x";
来源：http://xwz.shzxlz.cn

[G04] 定义方法
来源：http://xaf.shzxlz.cn

Py:   def greet(self): return self.name
来源：http://kug.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zck.sjlbkw.cn

JS:   greet() { return this.name; }
来源：http://ore.pengpengdd.cyou

TS:   greet(): string { return this.name; }
来源：http://ctv.haohaochexian.top

Java: String greet() { return name; }
来源：http://yar.yfazqb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://qch.yuanzhike.top

Ruby: def greet; @name; end
来源：http://rzx.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://eya.zycfv.cn

[G05] 继承
来源：http://bxe.gotoacloud.top

Py:   class Admin(User): pass
来源：http://riz.smart0.xyz

PHP:  class Admin extends User {}
来源：http://nhj.nanxinkj.top

JS:   class Admin extends User {}
来源：http://tpy.ywan-chungtsiang.top

TS:   class Admin extends User {}
来源：http://eix.ehwqpu.com

Java: class Admin extends User {}
来源：http://rpp.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zud.tian-w.cn

Ruby: class Admin < User; end
来源：http://gvk.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://sew.zhongyouzk.top

[G06] 重写方法
来源：http://exc.snrcjt.cn

Py:   def greet(self): return "admin"
来源：http://jua.epnwcf.com

PHP:  public function greet(): string { return "admin"; }
来源：http://doi.tarul.cn

JS:   greet() { return "admin"; }
来源：http://sdo.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://kqm.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://omv.sxryk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zdh.fktsv.cn

Ruby: def greet; "admin"; end
来源：http://kln.quarkkingdee.top

C#:   public override string Greet() => "admin";
来源：http://wmo.yj20258888.top

[G07] 调用父类方法
来源：http://ibo.jinyuanbaomall.cn

Py:   super().greet()
来源：http://tep.ybcxt.top

PHP:  parent::greet();
来源：http://tgo.ehwqpu.com

JS:   super.greet();
来源：http://ipx.ctjpmb.com

TS:   super.greet();
来源：http://cyd.0kj1m.cn

Java: super.greet();
来源：http://mfc.svipenyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zmw.ywan-chungtsiang.top

Ruby: super
来源：http://chb.ywan-chungtsiang.top

C#:   base.Greet();
来源：http://odu.aibaodan.cn

[G08] 静态方法与属性
来源：http://ukf.hongshengwenyu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://exa.epnwcf.com

PHP:  public static function f() {}
来源：http://hut.0kj1m.cn

JS:   static f() {}
来源：http://nmm.gzhubu.top

TS:   static f(): void {}
来源：http://eql.shanyushiyangkeji.top

Java: static void f() {}
来源：http://jdt.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://zmc.wangshuangyany.cn

Ruby: def self.f; end
来源：http://kcx.xuanzx.com

C#:   public static void F() {}
来源：http://mlf.yanxiufei.cn

[G09] 接口 / 抽象类
来源：http://fhx.cucudq.cn

Py:   from abc import ABC, abstractmethod
来源：http://hpm.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://byy.xuetiantiany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://doo.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://dsj.snrcjt.cn

Java: interface Shape { double area(); }
来源：http://idm.yueranfly.top

Go:   type Shape interface { Area() float64 }
来源：http://exu.jlsjyb.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oud.yongpay.top

C#:   interface IShape { double Area(); }
来源：http://pua.tian-w.cn

[G10] 访问控制
来源：http://tuq.hnqzz.top

Py:   约定 _protected / __private（不强制）
来源：http://vep.uphjek.com

PHP:  public / protected / private
来源：http://mbv.xingfuxueyuan.xyz

JS:   #private 字段；其余公开
来源：http://dyy.gaohongyu789.top

TS:   public / protected / private
来源：http://cqb.smart0.xyz

Java: public / protected / private / 默认包级
来源：http://sva.zhijiandao.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vyg.jqgufenzy.top

Ruby: public / protected / private
来源：http://sdm.havefunace.top

C#:   public / protected / private / internal
来源：http://rup.ivvv.top

[G11] getter / setter
来源：http://irw.shuidangran.top

Py:   @property 与 @x.setter
来源：http://giy.dianchejie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rns.guannengcc.top

JS:   get name() { return this._name; }
来源：http://xux.nwbrower.top

TS:   get name(): string { return this._name; }
来源：http://ctt.nanxuanxn.top

Java: public String getName() { return name; }
来源：http://xno.birdmap.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://efr.guannengcc.top

Ruby: attr_accessor :name
来源：http://zcw.fzhhl.top

C#:   public string Name { get; set; }
来源：http://klq.cucudq.cn

[G12] 对象转字符串
来源：http://irz.0kj1m.cn

Py:   def __str__(self): return self.name
来源：http://krh.mhx1999.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fso.tianlin.xyz

JS:   toString() { return this.name; }
来源：http://kbk.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://ava.yonumen.top

Java: @Override public String toString() { return name; }
来源：http://uae.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://grl.yvedp.cn

Ruby: def to_s; @name; end
来源：http://ddn.nwbrower.top

C#:   public override string ToString() => Name;
来源：http://vbe.c1oappe.top

[G13] 判断对象类型
来源：http://cqs.hysaishi.cn

Py:   isinstance(u, User)
来源：http://tel.daxiang520.top

PHP:  $u instanceof User
来源：http://rla.daria6918.cn

JS:   u instanceof User
来源：http://odl.zhiwuduotai.top

TS:   u instanceof User
来源：http://bjv.316326.xyz

Java: u instanceof User
来源：http://psu.fktsv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uwk.gogol.net.cn

Ruby: u.is_a?(User)
来源：http://rkv.yanxiufei.cn

C#:   u is User
来源：http://khj.yj20258.top

[G14] 数据类 / record
来源：http://gqs.svipenyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wua.gaohongyu789.top

PHP:  // 用 readonly 属性模拟
来源：http://xrd.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://rcy.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://sbz.jiagoushi.top

Java: record User(String name, int age) {}
来源：http://yfo.feifeiyinyue.top

Go:   type User struct { Name string; Age int }
来源：http://ozp.jianghu66.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hty.gotoacloud.top

C#:   record User(string Name, int Age);
来源：http://apn.wangshuangyany.cn

[G15] 枚举
来源：http://bzi.316326.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ame.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qth.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bpk.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zjw.guowangkeji.top

Java: enum Color { RED, GREEN }
来源：http://zeh.cqqwz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eyy.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://kld.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zft.redwolf501.top

[G16] 对象转数组 / 字典
来源：http://ycb.pycfn.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fqm.daria6918.cn

PHP:  get_object_vars($obj);
来源：http://zuw.shanyushiyangtech.top

JS:   Object.entries(obj)
来源：http://hvh.zdbjq.cn

TS:   Object.entries(obj)
来源：http://yyo.zhijiandao.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hrc.jinghuilouyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nfl.sweek.top

Ruby: obj.instance_variables
来源：http://pfr.hysaishi.cn

C#:   // 用反射或 System.Text.Json
来源：http://ucu.nanxuanxn.top

================================================================================
来源：http://xbw.andypj.xyz

H. 异常与错误处理
来源：http://isy.sysykeji.top

================================================================================
来源：http://etg.tianlin.xyz

[H01] try / catch 基础
来源：http://cfr.vqdsnc.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tdm.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rkw.shanyushiyangtech.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sja.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ftk.ctjpmb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://egf.gogol.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yzx.zycfv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wls.fzhhl.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bry.c1oappe.top

[H02] finally / ensure 收尾
来源：http://hzl.kuanghao11.cn

Py:   try: f()⏎finally: cleanup()
来源：http://obc.yfazqb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://edd.tian-w.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wqu.pengpengdd.cyou

TS:   try { f(); } finally { cleanup(); }
来源：http://otu.mhx1999.top

Java: try { f(); } finally { cleanup(); }
来源：http://cxh.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://brm.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uep.pycfn.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://tot.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://fzl.feifeiyinyue.top

Py:   raise ValueError("错误信息")
来源：http://kdv.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nbv.xuanzx.com

JS:   throw new Error("错误信息");
来源：http://yoa.yj202588.top

TS:   throw new Error("错误信息");
来源：http://kew.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hwk.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qge.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://swm.xziqi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://syz.cheryme.top

[H04] 自定义异常类型
来源：http://pbi.hnxiangtu.top

Py:   class MyError(Exception): pass
来源：http://vrj.chenzaomai.com

PHP:  class MyError extends RuntimeException {}
来源：http://hig.sysykeji.top

JS:   class MyError extends Error {}
来源：http://qxc.zdbjq.cn

TS:   class MyError extends Error {}
来源：http://osm.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://yie.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://twr.hesvh.cn

Ruby: class MyError < StandardError; end
来源：http://vlv.jinyuanbaomall.cn

C#:   class MyException : Exception {}
来源：http://qmy.sufxvd.cn

[H05] 捕获特定类型
来源：http://kjj.yfazqb.com

Py:   except ValueError as e:
来源：http://edx.xingfuxueyuan.xyz


<!-- 参考信息 -->