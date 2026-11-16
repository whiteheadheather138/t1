代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pxn.cucudq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eog.hcnkem.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://edv.316326.xyz

Ruby: File.read("a.txt")
来源：http://vvt.jqgfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://moh.tarul.cn

[F02] 逐行读取文件
来源：http://akf.gotoacloud.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vbs.yangfankeji.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vgq.dianchejie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://erq.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bfo.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vhq.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kot.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tlh.sxryk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bon.iojbl.cn

[F03] 写入文件（覆盖）
来源：http://knk.yonumen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tyf.meibo888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tow.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pdk.jinqigfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zot.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vcz.sweek.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zov.yfazqb.com

Ruby: File.write("a.txt", "hi")
来源：http://bnm.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cds.hammf.cn

[F04] 追加写入文件
来源：http://ewl.fehbvm.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ccz.fktsv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xjn.hnqzz.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ssx.cucudq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oiy.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rwa.gzhubu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cdn.snrcjt.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cfz.andypj.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xta.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://pjl.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rty.aibaodan.cn

PHP:  file_exists("a.txt");
来源：http://tli.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://gso.xuanzx.com

TS:   fs.existsSync("a.txt")
来源：http://ory.hcnkem.com

Java: Files.exists(Path.of("a.txt"))
来源：http://bzt.zdqjudy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yra.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://stf.ydzc1.top

C#:   File.Exists("a.txt")
来源：http://ycm.sjlbkw.cn

[F06] 删除文件
来源：http://yvp.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://ndt.redwolf501.top

PHP:  unlink("a.txt");
来源：http://cop.ybcxt.top

JS:   fs.unlinkSync("a.txt")
来源：http://rnu.ybcxt.top

TS:   fs.unlinkSync("a.txt")
来源：http://mwa.tian-w.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wrw.hnqzz.top

Go:   os.Remove("a.txt")
来源：http://pey.vehdjk.com

Ruby: File.delete("a.txt")
来源：http://fgj.zycfv.cn

C#:   File.Delete("a.txt");
来源：http://gqx.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://bua.zhongyouzk.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wat.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vqt.tian-w.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ycr.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rov.9152youxi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vej.fzhhl.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://exl.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oeh.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iar.aizwys.cn

[F08] 遍历目录
来源：http://sqd.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hmb.gotoacloud.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tvs.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://uje.yanxiufei.cn

TS:   fs.readdirSync("dir")
来源：http://ljp.cucudq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://eyn.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://men.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://ccu.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://god.52xcode.cn

[F09] 获取文件大小
来源：http://blw.uphjek.com

Py:   os.path.getsize("a.txt")
来源：http://fxd.yj20258888.top

PHP:  filesize("a.txt");
来源：http://qld.shzxlz.cn

JS:   fs.statSync("a.txt").size
来源：http://osq.iojbl.cn

TS:   fs.statSync("a.txt").size
来源：http://gih.sxryk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hcx.yuxming.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lou.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://lxf.vqdsnc.cn

C#:   new FileInfo("a.txt").Length
来源：http://ftk.zhijiandao.cn

[F10] 取文件扩展名 / 文件名
来源：http://cjl.epnwcf.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nzg.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dpy.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aqw.yfazqb.com

TS:   path.extname("a.txt")
来源：http://vob.yuxming.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sou.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xve.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vem.ydjk.org.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mzs.nanxinkj.top

[F11] 复制与移动文件
来源：http://mwk.bbcook.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vkz.hesvh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ksh.shzxlz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ppb.hesvh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vto.yfazqb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jyc.shuidangran.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zid.c1oappe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dxz.sysykeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://shl.ctjpmb.com

[F12] CSV 读写
来源：http://gbw.quarkkingdee.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sgx.quarkkingdee.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wry.hfpthk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ijz.redwolf501.top

TS:   // 同上
来源：http://dzr.dianchejie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uzr.nanxuanxn.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vlg.yj202588.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vnz.tianlin.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://npm.zdqjudy.top

================================================================================
来源：http://omk.shanyushiyangkeji.top

G. 面向对象
来源：http://cds.guowangkeji.top

================================================================================
来源：http://jzq.jinyuanbaomall.cn

[G01] 定义类
来源：http://zyv.birdmap.top

Py:   class User: pass
来源：http://ssc.vehdjk.com

PHP:  class User {}
来源：http://qgn.feifeiyinyue.top

JS:   class User {}
来源：http://nhm.yongpay.top

TS:   class User { name: string = ""; }
来源：http://old.yfazqb.com

Java: class User {}
来源：http://uwd.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://czv.tarul.cn

Ruby: class User; end
来源：http://bkz.vehdjk.com

C#:   class User {}
来源：http://fuh.52xcode.cn

[G02] 构造函数
来源：http://cdm.zhijiandao.cn

Py:   def __init__(self, name): self.name = name
来源：http://rhz.yuanzhike.top

PHP:  public function __construct(public string $name) {}
来源：http://eeg.hongshengwenyu.top

JS:   constructor(name) { this.name = name; }
来源：http://oup.daria6918.cn

TS:   constructor(public name: string) {}
来源：http://ypj.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://zcn.hongshengwenyu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pmc.fzhhl.top

Ruby: def initialize(name); @name = name; end
来源：http://vtf.xuetiantiany.cn

C#:   public User(string name) { Name = name; }
来源：http://vdm.shanyushiyangtech.top

[G03] 实例属性
来源：http://vor.guannengcc.top

Py:   self.name = "x"
来源：http://dci.hnqzz.top

PHP:  public string $name = "x";
来源：http://xfe.xuanzx.com

JS:   this.name = "x";
来源：http://xxe.fanxiaobao.xyz

TS:   name: string = "x";
来源：http://lbu.hesvh.cn

Java: private String name;
来源：http://ybv.shzxlz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xhy.xuanzx.com

Ruby: @name = "x"
来源：http://ufl.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://yzg.snrcjt.cn

[G04] 定义方法
来源：http://xxg.sjlbkw.cn

Py:   def greet(self): return self.name
来源：http://meb.yueranfly.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cfi.chenjidiqi.icu

JS:   greet() { return this.name; }
来源：http://njn.gzhubu.top

TS:   greet(): string { return this.name; }
来源：http://onf.haohaochexian.top

Java: String greet() { return name; }
来源：http://myg.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nwx.yonumen.top

Ruby: def greet; @name; end
来源：http://yje.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://lkx.gotoacloud.top

[G05] 继承
来源：http://igh.316326.xyz

Py:   class Admin(User): pass
来源：http://nmc.ppjwa.cn

PHP:  class Admin extends User {}
来源：http://jva.hesvh.cn

JS:   class Admin extends User {}
来源：http://foc.jyoumei.cn

TS:   class Admin extends User {}
来源：http://uzn.fktsv.cn

Java: class Admin extends User {}
来源：http://mni.jqgufenzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jlk.bbcook.cn

Ruby: class Admin < User; end
来源：http://feq.sxryk.cn

C#:   class Admin : User {}
来源：http://vam.svipenyu.cn

[G06] 重写方法
来源：http://bsx.dianchejie.cn

Py:   def greet(self): return "admin"
来源：http://sit.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://skx.wangdashe.top

JS:   greet() { return "admin"; }
来源：http://kbw.zhaomingkeji.xyz

TS:   greet(): string { return "admin"; }
来源：http://fta.smart0.xyz

Java: @Override String greet() { return "admin"; }
来源：http://orm.zhaomingkeji.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://syr.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://onh.meibo888.top

C#:   public override string Greet() => "admin";
来源：http://zpq.zhixingplan.top

[G07] 调用父类方法
来源：http://xxj.hongshengwenyu.top

Py:   super().greet()
来源：http://bww.tanke756.top

PHP:  parent::greet();
来源：http://dmu.hywenlv.cn

JS:   super.greet();
来源：http://iro.gaohongyu789.top

TS:   super.greet();
来源：http://wgs.hammf.cn

Java: super.greet();
来源：http://jxt.xylfe.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zpm.hywenlv.cn

Ruby: super
来源：http://rlj.ehwqpu.com

C#:   base.Greet();
来源：http://llb.jqgufenzy.top

[G08] 静态方法与属性
来源：http://jig.shzxlz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gyy.jinghuilouyu.cn

PHP:  public static function f() {}
来源：http://nhd.yj202588.top

JS:   static f() {}
来源：http://atc.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://zsu.ywan-chungtsiang.top

Java: static void f() {}
来源：http://sru.vqdsnc.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xqw.316326.xyz

Ruby: def self.f; end
来源：http://twu.jinqigfzy.top

C#:   public static void F() {}
来源：http://tyh.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://sjg.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://szb.aibaodan.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nqt.xuetiantiany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bgm.vqdsnc.cn

TS:   interface Shape { area(): number; }
来源：http://zwe.zhengqikj.top

Java: interface Shape { double area(); }
来源：http://lmf.gaohongyu789.top

Go:   type Shape interface { Area() float64 }
来源：http://dgd.yanxiufei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fvw.jqgufenzy.top

C#:   interface IShape { double Area(); }
来源：http://wrz.guannengcc.top

[G10] 访问控制
来源：http://hat.sysykeji.top

Py:   约定 _protected / __private（不强制）
来源：http://koi.feifeiyinyue.top

PHP:  public / protected / private
来源：http://tdq.bjfxy.top

JS:   #private 字段；其余公开
来源：http://btc.sxryk.cn

TS:   public / protected / private
来源：http://nta.hfpthk.cn

Java: public / protected / private / 默认包级
来源：http://ltj.xuanzx.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://qbx.yueranfly.top

Ruby: public / protected / private
来源：http://rsu.quarkkingdee.top

C#:   public / protected / private / internal
来源：http://dgc.hysaishi.cn

[G11] getter / setter
来源：http://rsq.gotoacloud.top

Py:   @property 与 @x.setter
来源：http://trh.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://scc.cheryme.top

JS:   get name() { return this._name; }
来源：http://gdu.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://taj.yuxming.cn

Java: public String getName() { return name; }
来源：http://dhr.cucudq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://iuv.ctjpmb.com

Ruby: attr_accessor :name
来源：http://unj.nanxuanxn.top

C#:   public string Name { get; set; }
来源：http://vau.yongpay.top

[G12] 对象转字符串
来源：http://cnk.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://pkw.yangfankeji.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://fxk.tarul.cn

JS:   toString() { return this.name; }
来源：http://myw.gogol.net.cn

TS:   toString(): string { return this.name; }
来源：http://jzc.vqdsnc.cn

Java: @Override public String toString() { return name; }
来源：http://stf.zhaomingkeji.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://awc.yvedp.cn

Ruby: def to_s; @name; end
来源：http://qvs.yongpay.top

C#:   public override string ToString() => Name;
来源：http://cgq.fzhhl.top

[G13] 判断对象类型
来源：http://edy.pengpengdd.cyou

Py:   isinstance(u, User)
来源：http://qvs.jlsjyb.cn

PHP:  $u instanceof User
来源：http://dmx.9152youxi.cn

JS:   u instanceof User
来源：http://arr.gogol.net.cn

TS:   u instanceof User
来源：http://npn.tianlin.xyz

Java: u instanceof User
来源：http://mws.havefunace.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dkv.gzhubu.top

Ruby: u.is_a?(User)
来源：http://eop.epnwcf.com

C#:   u is User
来源：http://znu.hfpthk.cn

[G14] 数据类 / record
来源：http://xlz.sjlbkw.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vrm.yangfankeji.com

PHP:  // 用 readonly 属性模拟
来源：http://ebh.ctjpmb.com

JS:   // 无内置：普通类或对象字面量
来源：http://ozs.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://apa.xinyue.icu

Java: record User(String name, int age) {}
来源：http://mwd.mhx1999.top

Go:   type User struct { Name string; Age int }
来源：http://jdz.jinghuilouyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xlg.jiagoushi.top

C#:   record User(string Name, int Age);
来源：http://kaf.pengpengdd.cyou

[G15] 枚举
来源：http://zej.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kka.pengpengdd.cyou

PHP:  enum Color: string { case Red = "red"; }
来源：http://chy.chenjidiqi.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jcf.yj20258.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://upy.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://zty.yanxiufei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vfn.zhixingplan.top

Ruby: Color = %i[red green].freeze
来源：http://mlb.tian-w.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hat.cheryme.top

[G16] 对象转数组 / 字典
来源：http://nwd.yj20258888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lxo.wangshuangyany.cn

PHP:  get_object_vars($obj);
来源：http://oni.yonumen.top

JS:   Object.entries(obj)
来源：http://veq.sxryk.cn

TS:   Object.entries(obj)
来源：http://gqb.zhiwuduotai.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eht.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ojl.yuxming.cn

Ruby: obj.instance_variables
来源：http://ohk.ehwqpu.com

C#:   // 用反射或 System.Text.Json
来源：http://hrd.cheryme.top

================================================================================
来源：http://kms.yj20258.top

H. 异常与错误处理
来源：http://vhh.gogol.net.cn

================================================================================
来源：http://vzv.ydzc1.top

[H01] try / catch 基础
来源：http://bpd.sxryk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fjv.yangfankeji.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hse.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rkf.jyoumei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://snn.ywan-chungtsiang.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jis.cheryme.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://txo.pengpengdd.cyou

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nqj.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vdl.xingfuxueyuan.xyz

[H02] finally / ensure 收尾
来源：http://eel.wangshuangyany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rry.redwolf501.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fvt.ydjk.org.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ebs.xinyue.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://sca.zhoulong.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://rsf.nanxuanxn.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hkp.yuxming.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vzz.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://aeh.gzhubu.top

[H03] 主动抛出异常
来源：http://rke.havefunace.top

Py:   raise ValueError("错误信息")
来源：http://xdd.ydzc1.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://avw.uphjek.com

JS:   throw new Error("错误信息");
来源：http://prb.iojbl.cn

TS:   throw new Error("错误信息");
来源：http://jdt.ybcxt.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://voz.shzxlz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://btq.fktsv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cib.daria6918.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jpn.316326.xyz

[H04] 自定义异常类型
来源：http://zqt.pengpengdd.cyou

Py:   class MyError(Exception): pass
来源：http://fer.sufxvd.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gwj.chenlongwang.top

JS:   class MyError extends Error {}
来源：http://swa.jlsjyb.cn

TS:   class MyError extends Error {}
来源：http://jqa.ybcxt.top

Java: class MyException extends RuntimeException {}
来源：http://oyk.chenjidiqi.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qgm.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://wuy.yuxming.cn

C#:   class MyException : Exception {}
来源：http://vjv.sweek.top

[H05] 捕获特定类型
来源：http://rsr.cdnleiting.top

Py:   except ValueError as e:
来源：http://yjp.zhiwuduotai.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hwc.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://gik.zhongyouzk.top

TS:   if (e instanceof TypeError) {}
来源：http://dly.yj20258888.top

Java: catch (IOException | SQLException e) {}
来源：http://kov.iojbl.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qza.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://anl.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fjj.hfpthk.cn

[H06] 可选值 / 空值安全访问
来源：http://cch.dianchejie.cn


<!-- 参考信息 -->