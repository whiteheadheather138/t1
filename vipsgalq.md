代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mcf.zhixingplan.top

================================================================================
来源：http://mfa.yj202588.top

F. 文件与目录
来源：http://kvp.ppjwa.cn

================================================================================
来源：http://uos.zdbjq.cn

[F01] 读取整个文件
来源：http://vzz.kuanghao11.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://psw.cdnleiting.top

PHP:  file_get_contents("a.txt");
来源：http://raw.nwbrower.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xcf.nwbrower.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ctv.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hpx.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://exv.haohaochexian.top

Ruby: File.read("a.txt")
来源：http://mcl.aizwys.cn

C#:   File.ReadAllText("a.txt");
来源：http://hyg.sysykeji.top

[F02] 逐行读取文件
来源：http://qxy.yfazqb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tsn.chenzaomai.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ngm.snrcjt.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://smi.sjlbkw.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ruk.shanyushiyangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://elw.jlsjyb.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qza.ctjpmb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://utc.svipenyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://phs.chenjidiqi.icu

[F03] 写入文件（覆盖）
来源：http://edd.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cel.yonumen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://eqr.9152youxi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ezy.vqdsnc.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://joe.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gti.xuetiantiany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rse.nanxinkj.top

Ruby: File.write("a.txt", "hi")
来源：http://mph.smart0.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aug.yonumen.top

[F04] 追加写入文件
来源：http://fum.chenlongwang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xjg.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hqn.dashuyun.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ifc.ivvv.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jdf.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kuk.vehdjk.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://riq.sufxvd.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://djx.tanke756.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cfs.zhijiandao.cn

[F05] 判断文件或目录是否存在
来源：http://pte.shangyingyoupin.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dic.hywenlv.cn

PHP:  file_exists("a.txt");
来源：http://hbb.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://pww.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://iyp.ybcxt.top

Java: Files.exists(Path.of("a.txt"))
来源：http://eom.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nrv.hysaishi.cn

Ruby: File.exist?("a.txt")
来源：http://bss.jinqigfzy.top

C#:   File.Exists("a.txt")
来源：http://lhq.chenjidiqi.icu

[F06] 删除文件
来源：http://ytv.yueranfly.top

Py:   os.remove("a.txt")
来源：http://iju.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://eiu.vqdsnc.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rwt.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qjz.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fea.xinyue.icu

Go:   os.Remove("a.txt")
来源：http://gff.xinyue.icu

Ruby: File.delete("a.txt")
来源：http://srr.wangdashe.top

C#:   File.Delete("a.txt");
来源：http://bqx.shuidangran.top

[F07] 创建目录（含多级）
来源：http://szq.vqdsnc.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://isx.vqdsnc.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gbu.cashguo.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sfu.ppjwa.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lgi.feifeiyinyue.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zic.shanyushiyangtech.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mgi.andypj.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wcn.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cao.jinqigufen.top

[F08] 遍历目录
来源：http://hkp.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vwe.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zzc.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://hgn.gotoacloud.top

TS:   fs.readdirSync("dir")
来源：http://uip.jianghu66.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qfd.shangyingyoupin.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uto.chenjidiqi.icu

Ruby: Dir.children("dir")
来源：http://yhv.fktsv.cn

C#:   Directory.GetFiles("dir")
来源：http://oeu.fengsongda.top

[F09] 获取文件大小
来源：http://bvd.cqqwz.cn

Py:   os.path.getsize("a.txt")
来源：http://ijt.xinyue.icu

PHP:  filesize("a.txt");
来源：http://son.yanxiufei.cn

JS:   fs.statSync("a.txt").size
来源：http://jsz.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://jmo.cashguo.top

Java: Files.size(Path.of("a.txt"))
来源：http://qez.daxiang520.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hwg.sxryk.cn

Ruby: File.size("a.txt")
来源：http://vki.zhixingplan.top

C#:   new FileInfo("a.txt").Length
来源：http://qvv.52xcode.cn

[F10] 取文件扩展名 / 文件名
来源：http://rjv.shzxlz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://igy.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iyk.fzhhl.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://auk.zdbjq.cn

TS:   path.extname("a.txt")
来源：http://grl.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lfq.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rpy.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aem.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uzu.pycfn.com

[F11] 复制与移动文件
来源：http://qpm.bjfxy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dph.smart0.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hrq.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xyf.kuanghao11.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rql.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jva.cucudq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xmb.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ngk.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://quz.sysykeji.top

[F12] CSV 读写
来源：http://ovx.nanxuanxn.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nsd.dianchejie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hzx.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ube.quarkkingdee.top

TS:   // 同上
来源：http://xla.aizwys.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wjh.hcnkem.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vup.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bmd.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rlr.pycfn.com

================================================================================
来源：http://nkl.yvedp.cn

G. 面向对象
来源：http://jli.hfpthk.cn

================================================================================
来源：http://ktm.shuidangran.top

[G01] 定义类
来源：http://jvs.daria6918.cn

Py:   class User: pass
来源：http://syr.zycfv.cn

PHP:  class User {}
来源：http://szd.kuanghao11.cn

JS:   class User {}
来源：http://cus.ivvv.top

TS:   class User { name: string = ""; }
来源：http://bdj.wangdashe.top

Java: class User {}
来源：http://mpo.yj20258888.top

Go:   type User struct { Name string }
来源：http://kiy.ydjk.org.cn

Ruby: class User; end
来源：http://kcl.nwbrower.top

C#:   class User {}
来源：http://trz.cucudq.cn

[G02] 构造函数
来源：http://coj.yj202588.top

Py:   def __init__(self, name): self.name = name
来源：http://ogl.pycfn.com

PHP:  public function __construct(public string $name) {}
来源：http://mqq.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://nog.yueranfly.top

TS:   constructor(public name: string) {}
来源：http://vco.zdqjudy.top

Java: User(String name) { this.name = name; }
来源：http://sel.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://afw.cucudq.cn

Ruby: def initialize(name); @name = name; end
来源：http://mhy.chenjidiqi.icu

C#:   public User(string name) { Name = name; }
来源：http://wvo.andypj.xyz

[G03] 实例属性
来源：http://evq.jinghuilouyu.cn

Py:   self.name = "x"
来源：http://csv.daxiang520.top

PHP:  public string $name = "x";
来源：http://xym.fktsv.cn

JS:   this.name = "x";
来源：http://qdo.zhengqikj.top

TS:   name: string = "x";
来源：http://jqr.zhongyouzk.top

Java: private String name;
来源：http://hxo.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yuo.nanxinkj.top

Ruby: @name = "x"
来源：http://gqe.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://jqu.xinyue.icu

[G04] 定义方法
来源：http://kus.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://ozf.cdnleiting.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hoy.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://xmv.yj20258888.top

TS:   greet(): string { return this.name; }
来源：http://mii.zhijiandao.cn

Java: String greet() { return name; }
来源：http://fqf.9152youxi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://etw.gzhubu.top

Ruby: def greet; @name; end
来源：http://ceh.gogol.net.cn

C#:   public string Greet() => Name;
来源：http://qgb.yj20258.top

[G05] 继承
来源：http://vkh.yj202588.top

Py:   class Admin(User): pass
来源：http://yhy.zhengqikj.top

PHP:  class Admin extends User {}
来源：http://ccb.jqgfzy.top

JS:   class Admin extends User {}
来源：http://bua.nwbrower.top

TS:   class Admin extends User {}
来源：http://jse.andypj.xyz

Java: class Admin extends User {}
来源：http://tik.chenjidiqi.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://aac.yj20258.top

Ruby: class Admin < User; end
来源：http://oat.jqgfzy.top

C#:   class Admin : User {}
来源：http://eqs.ybcxt.top

[G06] 重写方法
来源：http://imp.gzhubu.top

Py:   def greet(self): return "admin"
来源：http://lbq.zhengqikj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://onw.gaohongyu789.top

JS:   greet() { return "admin"; }
来源：http://ybb.tanke756.top

TS:   greet(): string { return "admin"; }
来源：http://ypp.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://gjc.pycfn.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://thm.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://idp.kuanghao11.cn

C#:   public override string Greet() => "admin";
来源：http://vlm.chenzaomai.com

[G07] 调用父类方法
来源：http://nqd.xuanzx.com

Py:   super().greet()
来源：http://ohr.zhengqikj.top

PHP:  parent::greet();
来源：http://she.fktsv.cn

JS:   super.greet();
来源：http://pyi.hongshengwenyu.top

TS:   super.greet();
来源：http://cbs.guannengcc.top

Java: super.greet();
来源：http://yim.nanxuanxn.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jyd.meibo888.top

Ruby: super
来源：http://mvs.wangdashe.top

C#:   base.Greet();
来源：http://bgd.hcnkem.com

[G08] 静态方法与属性
来源：http://svz.shzxlz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hij.daxiang520.top

PHP:  public static function f() {}
来源：http://llf.daxiang520.top

JS:   static f() {}
来源：http://wxt.fktsv.cn

TS:   static f(): void {}
来源：http://eqj.quarkkingdee.top

Java: static void f() {}
来源：http://rgk.redwolf501.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zsz.xuanzx.com

Ruby: def self.f; end
来源：http://opa.c1oappe.top

C#:   public static void F() {}
来源：http://wrr.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://hlc.yueranfly.top

Py:   from abc import ABC, abstractmethod
来源：http://gcg.dashuyun.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hug.yueranfly.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xyj.fktsv.cn

TS:   interface Shape { area(): number; }
来源：http://rtw.316326.xyz

Java: interface Shape { double area(); }
来源：http://mtf.ivvv.top

Go:   type Shape interface { Area() float64 }
来源：http://jaj.birdmap.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xsc.zdbjq.cn

C#:   interface IShape { double Area(); }
来源：http://hmi.kuanghao11.cn

[G10] 访问控制
来源：http://sbn.ppjwa.cn

Py:   约定 _protected / __private（不强制）
来源：http://fci.guannengcc.top

PHP:  public / protected / private
来源：http://byd.daria6918.cn

JS:   #private 字段；其余公开
来源：http://ndx.gogol.net.cn

TS:   public / protected / private
来源：http://rrc.andypj.xyz

Java: public / protected / private / 默认包级
来源：http://nru.sysykeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://lwi.yongpay.top

Ruby: public / protected / private
来源：http://tpe.zycfv.cn

C#:   public / protected / private / internal
来源：http://sgj.jqgufenzy.top

[G11] getter / setter
来源：http://ycp.sjlbkw.cn

Py:   @property 与 @x.setter
来源：http://ldp.shzxlz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dzn.ivvv.top

JS:   get name() { return this._name; }
来源：http://abf.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://zhv.yfazqb.com

Java: public String getName() { return name; }
来源：http://yhr.snrcjt.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://suh.shangyingyoupin.top

Ruby: attr_accessor :name
来源：http://vxu.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://rnk.ctjpmb.com

[G12] 对象转字符串
来源：http://nri.ctjpmb.com

Py:   def __str__(self): return self.name
来源：http://hvg.yfazqb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://kbu.jianghu66.top

JS:   toString() { return this.name; }
来源：http://tum.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://trg.quarkkingdee.top

Java: @Override public String toString() { return name; }
来源：http://mwf.hnqzz.top

Go:   func (u User) String() string { return u.Name }
来源：http://cob.uphjek.com

Ruby: def to_s; @name; end
来源：http://xqp.zdqjudy.top

C#:   public override string ToString() => Name;
来源：http://xrh.yanxiufei.cn

[G13] 判断对象类型
来源：http://nyv.zhixingplan.top

Py:   isinstance(u, User)
来源：http://acf.birdmap.top

PHP:  $u instanceof User
来源：http://huf.gaohongyu789.top

JS:   u instanceof User
来源：http://upk.nwbrower.top

TS:   u instanceof User
来源：http://huf.jinqigfzy.top

Java: u instanceof User
来源：http://zbn.sxryk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pme.quarkkingdee.top

Ruby: u.is_a?(User)
来源：http://mbe.jlsjyb.cn

C#:   u is User
来源：http://czs.sweek.top

[G14] 数据类 / record
来源：http://mkx.jlsjyb.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rme.nwbrower.top

PHP:  // 用 readonly 属性模拟
来源：http://gbf.tian-w.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qig.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://kqp.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://hnw.guannengcc.top

Go:   type User struct { Name string; Age int }
来源：http://ate.jinqigufen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ysb.hesvh.cn

C#:   record User(string Name, int Age);
来源：http://bcr.vqdsnc.cn

[G15] 枚举
来源：http://kwf.iojbl.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zds.zdbjq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fxr.bbcook.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pgs.hcnkem.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fti.hnxiangtu.top

Java: enum Color { RED, GREEN }
来源：http://uqz.pengpengdd.cyou

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ngw.jqgufenzy.top

Ruby: Color = %i[red green].freeze
来源：http://swu.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wva.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://asu.jlsjyb.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gqt.daria6918.cn

PHP:  get_object_vars($obj);
来源：http://cez.yj20258888.top

JS:   Object.entries(obj)
来源：http://sbd.epnwcf.com

TS:   Object.entries(obj)
来源：http://gaa.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mvv.nanxuanxn.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jtw.fanxiaobao.xyz

Ruby: obj.instance_variables
来源：http://vzp.andypj.xyz

C#:   // 用反射或 System.Text.Json
来源：http://mix.zhoulong.xyz

================================================================================
来源：http://iwx.jiagoushi.top

H. 异常与错误处理
来源：http://yya.jyoumei.cn

================================================================================
来源：http://dty.chenzaomai.com

[H01] try / catch 基础
来源：http://vqj.jinqigufen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jsz.yj202588.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fle.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fdw.redwolf501.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wjc.yuxming.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://koz.zhengqikj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pnl.sufxvd.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vfj.chenzaomai.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kyr.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://rle.gogol.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ets.cqqwz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tbv.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dlr.iojbl.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nlf.aizwys.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ajo.52xcode.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mzy.xylfe.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kqp.meibo888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://kui.dianchejie.cn

[H03] 主动抛出异常
来源：http://txv.sufxvd.cn

Py:   raise ValueError("错误信息")
来源：http://abb.chenzaomai.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hrc.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://fzc.fengsongda.top

TS:   throw new Error("错误信息");
来源：http://bdx.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mff.birdmap.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pjt.svipenyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zsd.quarkkingdee.top

C#:   throw new ArgumentException("错误信息");
来源：http://bnh.fzhhl.top

[H04] 自定义异常类型
来源：http://ovu.nanxinkj.top

Py:   class MyError(Exception): pass
来源：http://syu.jlsjyb.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ktk.ywan-chungtsiang.top

JS:   class MyError extends Error {}
来源：http://kkp.jinghuilouyu.cn

TS:   class MyError extends Error {}
来源：http://iit.sjlbkw.cn

Java: class MyException extends RuntimeException {}
来源：http://yha.xylfe.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://toq.yj20258888.top

Ruby: class MyError < StandardError; end
来源：http://oqm.aibaodan.cn

C#:   class MyException : Exception {}
来源：http://gwk.sjlbkw.cn

[H05] 捕获特定类型
来源：http://eie.gzhubu.top

Py:   except ValueError as e:
来源：http://gpg.ctjpmb.com


<!-- 参考信息 -->