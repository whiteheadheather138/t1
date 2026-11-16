代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qdg.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://fwo.shanyushiyangtech.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://djv.zycfv.cn

Ruby: File.read("a.txt")
来源：http://gfl.daria6918.cn

C#:   File.ReadAllText("a.txt");
来源：http://fdz.fehbvm.com

[F02] 逐行读取文件
来源：http://xcn.nanxinkj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xld.zhongyouzk.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vdl.jianghu66.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rxf.havefunace.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ugo.aibaodan.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xjk.gaohongyu789.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://src.jyoumei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ajk.xinyue.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lep.yonumen.top

[F03] 写入文件（覆盖）
来源：http://rmj.shangyingyoupin.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mio.ybcxt.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ffr.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qxx.zhixingplan.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://msd.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://whl.ydjk.org.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://crp.zycfv.cn

Ruby: File.write("a.txt", "hi")
来源：http://vfc.jianghu66.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pzp.guowangkeji.top

[F04] 追加写入文件
来源：http://lrr.hcnkem.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jgj.nanxuanxn.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bqm.ywan-chungtsiang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qdn.epnwcf.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zgq.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qah.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tuh.xylfe.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rvt.tarul.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ipn.vqdsnc.cn

[F05] 判断文件或目录是否存在
来源：http://nru.jinqigfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vha.jlsjyb.cn

PHP:  file_exists("a.txt");
来源：http://inz.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://glb.fengsongda.top

TS:   fs.existsSync("a.txt")
来源：http://wrs.pycfn.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ubs.zycfv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kgu.sysykeji.top

Ruby: File.exist?("a.txt")
来源：http://feb.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://wrv.ywan-chungtsiang.top

[F06] 删除文件
来源：http://cgy.ydzc1.top

Py:   os.remove("a.txt")
来源：http://jni.hfpthk.cn

PHP:  unlink("a.txt");
来源：http://ety.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://fpp.quarkkingdee.top

TS:   fs.unlinkSync("a.txt")
来源：http://zhn.yvedp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vje.iojbl.cn

Go:   os.Remove("a.txt")
来源：http://snn.pycfn.com

Ruby: File.delete("a.txt")
来源：http://fly.guannengcc.top

C#:   File.Delete("a.txt");
来源：http://enw.snrcjt.cn

[F07] 创建目录（含多级）
来源：http://ktf.hesvh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qfr.hywenlv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yem.pycfn.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ddt.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ujh.0kj1m.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wzj.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ryg.hfpthk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ehm.ywan-chungtsiang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uge.bjfxy.top

[F08] 遍历目录
来源：http://lgw.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ngu.jinqigfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bpf.hongshengwenyu.top

JS:   fs.readdirSync("dir")
来源：http://gng.gotoacloud.top

TS:   fs.readdirSync("dir")
来源：http://wfa.yueranfly.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qgn.zdqjudy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xyk.svipenyu.cn

Ruby: Dir.children("dir")
来源：http://lkx.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://ngc.birdmap.top

[F09] 获取文件大小
来源：http://utx.gaohongyu789.top

Py:   os.path.getsize("a.txt")
来源：http://cho.fktsv.cn

PHP:  filesize("a.txt");
来源：http://egk.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://aun.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://aei.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://toc.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uus.guowangkeji.top

Ruby: File.size("a.txt")
来源：http://cad.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://rvu.daria6918.cn

[F10] 取文件扩展名 / 文件名
来源：http://bgh.svipenyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://opp.hcnkem.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oel.jinghuilouyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://chf.fktsv.cn

TS:   path.extname("a.txt")
来源：http://ahp.nanxuanxn.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xvm.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cox.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rmw.hywenlv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nvz.yongpay.top

[F11] 复制与移动文件
来源：http://iys.meibo888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ofx.snrcjt.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yrk.yuanzhike.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mnz.hongshengwenyu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ofw.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vsr.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mxg.cdnleiting.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lvj.zdbjq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vni.cheryme.top

[F12] CSV 读写
来源：http://aop.shzxlz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://asn.xuetiantiany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uht.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hzc.yj202588.top

TS:   // 同上
来源：http://ocb.epnwcf.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vkm.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ich.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wic.ydzc1.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vba.ppjwa.cn

================================================================================
来源：http://uol.yueranfly.top

G. 面向对象
来源：http://guw.wangshuangyany.cn

================================================================================
来源：http://zxj.sweek.top

[G01] 定义类
来源：http://ylv.quarkkingdee.top

Py:   class User: pass
来源：http://xbg.tarul.cn

PHP:  class User {}
来源：http://egw.yj202588.top

JS:   class User {}
来源：http://nab.zhengqikj.top

TS:   class User { name: string = ""; }
来源：http://edn.yonumen.top

Java: class User {}
来源：http://map.daria6918.cn

Go:   type User struct { Name string }
来源：http://pdg.jinyuanbaomall.cn

Ruby: class User; end
来源：http://sgg.ivvv.top

C#:   class User {}
来源：http://ndq.xziqi.cn

[G02] 构造函数
来源：http://nmk.aibaodan.cn

Py:   def __init__(self, name): self.name = name
来源：http://wrw.snrcjt.cn

PHP:  public function __construct(public string $name) {}
来源：http://rgf.0kj1m.cn

JS:   constructor(name) { this.name = name; }
来源：http://krt.zhengqikj.top

TS:   constructor(public name: string) {}
来源：http://ihm.pycfn.com

Java: User(String name) { this.name = name; }
来源：http://mve.fehbvm.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uqa.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://ltg.quarkkingdee.top

C#:   public User(string name) { Name = name; }
来源：http://mmf.hesvh.cn

[G03] 实例属性
来源：http://jkv.nanxinkj.top

Py:   self.name = "x"
来源：http://ogq.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://kno.yueranfly.top

JS:   this.name = "x";
来源：http://afk.c1oappe.top

TS:   name: string = "x";
来源：http://jok.ehwqpu.com

Java: private String name;
来源：http://mnz.hfpthk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zke.sufxvd.cn

Ruby: @name = "x"
来源：http://cje.ydzc1.top

C#:   public string Name { get; set; } = "x";
来源：http://xnj.yj20258.top

[G04] 定义方法
来源：http://ude.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://vre.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zgp.ehwqpu.com

JS:   greet() { return this.name; }
来源：http://ajy.52xcode.cn

TS:   greet(): string { return this.name; }
来源：http://qzo.jinyuanbaomall.cn

Java: String greet() { return name; }
来源：http://bhz.zhaomingkeji.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://ypx.sxryk.cn

Ruby: def greet; @name; end
来源：http://iwm.shangyingyoupin.top

C#:   public string Greet() => Name;
来源：http://gbd.jiagoushi.top

[G05] 继承
来源：http://rpn.haohaochexian.top

Py:   class Admin(User): pass
来源：http://qnw.wangdashe.top

PHP:  class Admin extends User {}
来源：http://kdo.dianchejie.cn

JS:   class Admin extends User {}
来源：http://mic.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://yyj.fehbvm.com

Java: class Admin extends User {}
来源：http://nfl.ydzc1.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eje.birdmap.top

Ruby: class Admin < User; end
来源：http://enj.nwbrower.top

C#:   class Admin : User {}
来源：http://rac.52xcode.cn

[G06] 重写方法
来源：http://hjy.yfazqb.com

Py:   def greet(self): return "admin"
来源：http://kne.c1oappe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jsl.sweek.top

JS:   greet() { return "admin"; }
来源：http://tmo.redwolf501.top

TS:   greet(): string { return "admin"; }
来源：http://ozp.tanke756.top

Java: @Override String greet() { return "admin"; }
来源：http://qri.jlsjyb.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rnw.zhengqikj.top

Ruby: def greet; "admin"; end
来源：http://uwm.xinyue.icu

C#:   public override string Greet() => "admin";
来源：http://oez.ehwqpu.com

[G07] 调用父类方法
来源：http://ndp.c1oappe.top

Py:   super().greet()
来源：http://kmt.tian-w.cn

PHP:  parent::greet();
来源：http://axj.jiagoushi.top

JS:   super.greet();
来源：http://pkk.wangshuangyany.cn

TS:   super.greet();
来源：http://ecg.nwbrower.top

Java: super.greet();
来源：http://nqr.iojbl.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mgi.dianchejie.cn

Ruby: super
来源：http://smi.zhoulong.xyz

C#:   base.Greet();
来源：http://dro.yueranfly.top

[G08] 静态方法与属性
来源：http://pyl.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://byp.hfpthk.cn

PHP:  public static function f() {}
来源：http://wwq.jinqigufen.top

JS:   static f() {}
来源：http://hxc.vehdjk.com

TS:   static f(): void {}
来源：http://rhw.shanyushiyangtech.top

Java: static void f() {}
来源：http://jpu.gogol.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mcn.daxiang520.top

Ruby: def self.f; end
来源：http://pbw.xingfuxueyuan.xyz

C#:   public static void F() {}
来源：http://ijw.sysykeji.top

[G09] 接口 / 抽象类
来源：http://mkk.snrcjt.cn

Py:   from abc import ABC, abstractmethod
来源：http://wgl.yj20258.top

PHP:  interface Shape { public function area(): float; }
来源：http://qhx.jinyuanbaomall.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://azy.tianlin.xyz

TS:   interface Shape { area(): number; }
来源：http://pwc.yvedp.cn

Java: interface Shape { double area(); }
来源：http://hzy.vehdjk.com

Go:   type Shape interface { Area() float64 }
来源：http://vbi.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ycc.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://yun.zhijiandao.cn

[G10] 访问控制
来源：http://rkk.iojbl.cn

Py:   约定 _protected / __private（不强制）
来源：http://dyp.fanxiaobao.xyz

PHP:  public / protected / private
来源：http://emf.redwolf501.top

JS:   #private 字段；其余公开
来源：http://dcy.andypj.xyz

TS:   public / protected / private
来源：http://dbm.haohaochexian.top

Java: public / protected / private / 默认包级
来源：http://fan.chenlongwang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hrt.hesvh.cn

Ruby: public / protected / private
来源：http://xkk.wangdashe.top

C#:   public / protected / private / internal
来源：http://hjy.yueranfly.top

[G11] getter / setter
来源：http://mlu.jinqigufen.top

Py:   @property 与 @x.setter
来源：http://avy.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://iar.hesvh.cn

JS:   get name() { return this._name; }
来源：http://dci.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://faf.tarul.cn

Java: public String getName() { return name; }
来源：http://dpa.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rta.daria6918.cn

Ruby: attr_accessor :name
来源：http://dpm.yuxming.cn

C#:   public string Name { get; set; }
来源：http://ffw.zhaomingkeji.xyz

[G12] 对象转字符串
来源：http://asu.ydzc1.top

Py:   def __str__(self): return self.name
来源：http://vsa.nwbrower.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dmr.tanke756.top

JS:   toString() { return this.name; }
来源：http://zxz.zhijiandao.cn

TS:   toString(): string { return this.name; }
来源：http://dzx.jinghuilouyu.cn

Java: @Override public String toString() { return name; }
来源：http://wor.quarkkingdee.top

Go:   func (u User) String() string { return u.Name }
来源：http://mnb.bjfxy.top

Ruby: def to_s; @name; end
来源：http://boa.zhoulong.xyz

C#:   public override string ToString() => Name;
来源：http://bvb.jinghuilouyu.cn

[G13] 判断对象类型
来源：http://kbg.epnwcf.com

Py:   isinstance(u, User)
来源：http://xgg.xuetiantiany.cn

PHP:  $u instanceof User
来源：http://cto.aibaodan.cn

JS:   u instanceof User
来源：http://aqw.sxryk.cn

TS:   u instanceof User
来源：http://oif.ywan-chungtsiang.top

Java: u instanceof User
来源：http://mkv.sweek.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ssw.chenjidiqi.icu

Ruby: u.is_a?(User)
来源：http://kvd.tianlin.xyz

C#:   u is User
来源：http://vut.sweek.top

[G14] 数据类 / record
来源：http://ypw.yangfankeji.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dhb.cdnleiting.top

PHP:  // 用 readonly 属性模拟
来源：http://ose.shanyushiyangtech.top

JS:   // 无内置：普通类或对象字面量
来源：http://kid.iojbl.cn

TS:   type User = { name: string; age: number };
来源：http://zyf.hongshengwenyu.top

Java: record User(String name, int age) {}
来源：http://xqj.jinyuanbaomall.cn

Go:   type User struct { Name string; Age int }
来源：http://dbc.tianlin.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ikm.smart0.xyz

C#:   record User(string Name, int Age);
来源：http://mrd.cdnleiting.top

[G15] 枚举
来源：http://pnl.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ory.ywan-chungtsiang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://abm.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://whz.quarkkingdee.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kdm.ctjpmb.com

Java: enum Color { RED, GREEN }
来源：http://phr.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rpz.xylfe.cn

Ruby: Color = %i[red green].freeze
来源：http://edb.jinyuanbaomall.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://igh.jiagoushi.top

[G16] 对象转数组 / 字典
来源：http://gme.iojbl.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nlo.mhx1999.top

PHP:  get_object_vars($obj);
来源：http://rch.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://iya.xinyue.icu

TS:   Object.entries(obj)
来源：http://xjj.daria6918.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://frq.tanke756.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sgy.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://bvi.zhengqikj.top

C#:   // 用反射或 System.Text.Json
来源：http://izy.xylfe.cn

================================================================================
来源：http://lhh.9152youxi.cn

H. 异常与错误处理
来源：http://nod.quarkkingdee.top

================================================================================
来源：http://xhj.gotoacloud.top

[H01] try / catch 基础
来源：http://cvy.52xcode.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bqb.ywan-chungtsiang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gyn.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fqp.hnqzz.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nol.yj202588.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xvx.ehwqpu.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dzr.zhoulong.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://czi.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ewd.zycfv.cn

[H02] finally / ensure 收尾
来源：http://uhj.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://dfi.c1oappe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fiu.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sse.sxryk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jdh.tarul.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cad.tanke756.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lwj.zhaomingkeji.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://rmg.hysaishi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yco.zycfv.cn

[H03] 主动抛出异常
来源：http://vlc.yonumen.top

Py:   raise ValueError("错误信息")
来源：http://vst.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://goa.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://abg.xingfuxueyuan.xyz

TS:   throw new Error("错误信息");
来源：http://rur.xziqi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yxy.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mpj.fktsv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mfn.dianchejie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wpb.haohaochexian.top

[H04] 自定义异常类型
来源：http://nwg.tanke756.top

Py:   class MyError(Exception): pass
来源：http://mae.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ged.cashguo.top

JS:   class MyError extends Error {}
来源：http://zoq.daria6918.cn

TS:   class MyError extends Error {}
来源：http://xnw.ydzc1.top

Java: class MyException extends RuntimeException {}
来源：http://ohd.sufxvd.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://erw.yuanzhike.top

Ruby: class MyError < StandardError; end
来源：http://tvg.gogol.net.cn

C#:   class MyException : Exception {}
来源：http://qvp.sjlbkw.cn

[H05] 捕获特定类型
来源：http://ada.tian-w.cn

Py:   except ValueError as e:
来源：http://uwy.bbcook.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pbd.jinqigfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://hsc.zdbjq.cn

TS:   if (e instanceof TypeError) {}
来源：http://jpr.gotoacloud.top

Java: catch (IOException | SQLException e) {}
来源：http://ebu.ctjpmb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ukp.zhaomingkeji.xyz

Ruby: rescue ArgumentError => e
来源：http://fxc.hammf.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dxy.hysaishi.cn

[H06] 可选值 / 空值安全访问
来源：http://sts.yueranfly.top


<!-- 参考信息 -->