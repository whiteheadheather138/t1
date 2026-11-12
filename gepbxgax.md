代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pwa.mhx1999.top

================================================================================
来源：http://uwj.meibo888.top

F. 文件与目录
来源：http://kaq.hcnkem.com

================================================================================
来源：http://ehq.guannengcc.top

[F01] 读取整个文件
来源：http://jta.ywan-chungtsiang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ovm.yangfankeji.com

PHP:  file_get_contents("a.txt");
来源：http://dsg.mhx1999.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pwh.sweek.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tjc.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jdp.xylfe.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kpq.cdnleiting.top

Ruby: File.read("a.txt")
来源：http://pds.tian-w.cn

C#:   File.ReadAllText("a.txt");
来源：http://sud.ehwqpu.com

[F02] 逐行读取文件
来源：http://dxk.aibaodan.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kew.zhoulong.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://obz.ivvv.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rbf.zhiwuduotai.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://thb.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jgm.jinghuilouyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ksx.fzhhl.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gcq.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kbx.hcnkem.com

[F03] 写入文件（覆盖）
来源：http://kpr.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mvd.jyoumei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jdh.cqqwz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wjy.xingfuxueyuan.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jqa.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://phy.xziqi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://msl.shzxlz.cn

Ruby: File.write("a.txt", "hi")
来源：http://lgc.smart0.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://exd.zhixingplan.top

[F04] 追加写入文件
来源：http://nat.shzxlz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xgj.yuxming.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hyk.kuanghao11.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lpf.nanxinkj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oqh.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://goz.cdnleiting.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://esh.havefunace.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cos.hnqzz.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zue.xinyue.icu

[F05] 判断文件或目录是否存在
来源：http://yuo.jiagoushi.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nky.cashguo.top

PHP:  file_exists("a.txt");
来源：http://wvn.pycfn.com

JS:   fs.existsSync("a.txt")
来源：http://zab.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://svn.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://sow.316326.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pan.dianchejie.cn

Ruby: File.exist?("a.txt")
来源：http://ttv.zdbjq.cn

C#:   File.Exists("a.txt")
来源：http://tkc.chenlongwang.top

[F06] 删除文件
来源：http://uao.gotoacloud.top

Py:   os.remove("a.txt")
来源：http://vrd.meibo888.top

PHP:  unlink("a.txt");
来源：http://dzn.yueranfly.top

JS:   fs.unlinkSync("a.txt")
来源：http://zpb.andypj.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://drt.hfpthk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ikn.yongpay.top

Go:   os.Remove("a.txt")
来源：http://oqt.hammf.cn

Ruby: File.delete("a.txt")
来源：http://mbg.fanxiaobao.xyz

C#:   File.Delete("a.txt");
来源：http://puf.jinqigfzy.top

[F07] 创建目录（含多级）
来源：http://bnq.ydjk.org.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nil.shangyingyoupin.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hao.jinghuilouyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qwf.hesvh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xaw.fzhhl.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fvn.cdnleiting.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dbj.jqgfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mqb.chenzaomai.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://avp.jlsjyb.cn

[F08] 遍历目录
来源：http://bgm.yonumen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xjj.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tlm.sxryk.cn

JS:   fs.readdirSync("dir")
来源：http://weh.gzhubu.top

TS:   fs.readdirSync("dir")
来源：http://ybg.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://egy.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nry.xylfe.cn

Ruby: Dir.children("dir")
来源：http://zjz.tanke756.top

C#:   Directory.GetFiles("dir")
来源：http://yzm.shanyushiyangtech.top

[F09] 获取文件大小
来源：http://vek.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://gqk.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://okl.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://cly.zhoulong.xyz

TS:   fs.statSync("a.txt").size
来源：http://duj.ybcxt.top

Java: Files.size(Path.of("a.txt"))
来源：http://bnd.xylfe.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hbt.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://uka.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://ali.havefunace.top

[F10] 取文件扩展名 / 文件名
来源：http://qxp.cheryme.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hhe.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tet.pengpengdd.cyou

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rqj.ehwqpu.com

TS:   path.extname("a.txt")
来源：http://bcz.nwbrower.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gwo.yfazqb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ler.yvedp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://svt.yuanzhike.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ofv.svipenyu.cn

[F11] 复制与移动文件
来源：http://uwf.sysykeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xea.dianchejie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fer.chenlongwang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vzr.wangdashe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://svm.hesvh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lnu.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vhb.ybcxt.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rbo.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hmy.xingfuxueyuan.xyz

[F12] CSV 读写
来源：http://aka.fengsongda.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://otc.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uqr.aibaodan.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ujh.epnwcf.com

TS:   // 同上
来源：http://lzg.sufxvd.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iab.yj202588.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kux.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ybj.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://mbk.zhaomingkeji.xyz

================================================================================
来源：http://clz.dianchejie.cn

G. 面向对象
来源：http://tan.zhoulong.xyz

================================================================================
来源：http://xzb.shuidangran.top

[G01] 定义类
来源：http://plh.jyoumei.cn

Py:   class User: pass
来源：http://xqm.chenzaomai.com

PHP:  class User {}
来源：http://vzn.meibo888.top

JS:   class User {}
来源：http://ptg.yvedp.cn

TS:   class User { name: string = ""; }
来源：http://yxg.9152youxi.cn

Java: class User {}
来源：http://zrx.gogol.net.cn

Go:   type User struct { Name string }
来源：http://fug.andypj.xyz

Ruby: class User; end
来源：http://nez.xylfe.cn

C#:   class User {}
来源：http://mas.bbcook.cn

[G02] 构造函数
来源：http://dpx.yonumen.top

Py:   def __init__(self, name): self.name = name
来源：http://lda.cheryme.top

PHP:  public function __construct(public string $name) {}
来源：http://orb.ivvv.top

JS:   constructor(name) { this.name = name; }
来源：http://bsn.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://upw.sysykeji.top

Java: User(String name) { this.name = name; }
来源：http://dsb.zdbjq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vyt.wangdashe.top

Ruby: def initialize(name); @name = name; end
来源：http://rtm.wangshuangyany.cn

C#:   public User(string name) { Name = name; }
来源：http://rus.jqgufenzy.top

[G03] 实例属性
来源：http://alv.hammf.cn

Py:   self.name = "x"
来源：http://psq.jinqigfzy.top

PHP:  public string $name = "x";
来源：http://tuv.9152youxi.cn

JS:   this.name = "x";
来源：http://qhw.yangfankeji.com

TS:   name: string = "x";
来源：http://kjv.iojbl.cn

Java: private String name;
来源：http://hns.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sov.zdqjudy.top

Ruby: @name = "x"
来源：http://art.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://yqp.shzxlz.cn

[G04] 定义方法
来源：http://qpr.chenzaomai.com

Py:   def greet(self): return self.name
来源：http://xfe.snrcjt.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jax.quarkkingdee.top

JS:   greet() { return this.name; }
来源：http://zda.hnxiangtu.top

TS:   greet(): string { return this.name; }
来源：http://btt.9152youxi.cn

Java: String greet() { return name; }
来源：http://lym.nwbrower.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hbz.dianchejie.cn

Ruby: def greet; @name; end
来源：http://aca.vqdsnc.cn

C#:   public string Greet() => Name;
来源：http://lqi.feifeiyinyue.top

[G05] 继承
来源：http://hrn.fehbvm.com

Py:   class Admin(User): pass
来源：http://blp.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://cel.daxiang520.top

JS:   class Admin extends User {}
来源：http://dag.tanke756.top

TS:   class Admin extends User {}
来源：http://mmv.gzhubu.top

Java: class Admin extends User {}
来源：http://llr.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mna.uphjek.com

Ruby: class Admin < User; end
来源：http://hzq.hnqzz.top

C#:   class Admin : User {}
来源：http://ije.chenlongwang.top

[G06] 重写方法
来源：http://equ.smart0.xyz

Py:   def greet(self): return "admin"
来源：http://pkz.cucudq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://njs.yj20258888.top

JS:   greet() { return "admin"; }
来源：http://yky.quarkkingdee.top

TS:   greet(): string { return "admin"; }
来源：http://ftv.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://wgq.birdmap.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ixc.cheryme.top

Ruby: def greet; "admin"; end
来源：http://jff.hcnkem.com

C#:   public override string Greet() => "admin";
来源：http://ibl.jinghuilouyu.cn

[G07] 调用父类方法
来源：http://pof.zycfv.cn

Py:   super().greet()
来源：http://fxe.jiagoushi.top

PHP:  parent::greet();
来源：http://ibj.316326.xyz

JS:   super.greet();
来源：http://tha.jinyuanbaomall.cn

TS:   super.greet();
来源：http://hii.gotoacloud.top

Java: super.greet();
来源：http://kkz.yanxiufei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nyb.sxryk.cn

Ruby: super
来源：http://myc.cqqwz.cn

C#:   base.Greet();
来源：http://wnn.haohaochexian.top

[G08] 静态方法与属性
来源：http://etp.vehdjk.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://esh.ydzc1.top

PHP:  public static function f() {}
来源：http://kpw.hysaishi.cn

JS:   static f() {}
来源：http://dmn.jinghuilouyu.cn

TS:   static f(): void {}
来源：http://psw.yj20258888.top

Java: static void f() {}
来源：http://xka.yanxiufei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ayp.aibaodan.cn

Ruby: def self.f; end
来源：http://cag.9152youxi.cn

C#:   public static void F() {}
来源：http://kvg.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://gmf.jqgfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://atr.aibaodan.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nuh.jinqigfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tjp.shanyushiyangtech.top

TS:   interface Shape { area(): number; }
来源：http://dlq.ppjwa.cn

Java: interface Shape { double area(); }
来源：http://ixy.sjlbkw.cn

Go:   type Shape interface { Area() float64 }
来源：http://fyy.xinyue.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oom.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://ueu.ehwqpu.com

[G10] 访问控制
来源：http://ahy.jyoumei.cn

Py:   约定 _protected / __private（不强制）
来源：http://nph.yuanzhike.top

PHP:  public / protected / private
来源：http://eyn.ctjpmb.com

JS:   #private 字段；其余公开
来源：http://xcb.sxryk.cn

TS:   public / protected / private
来源：http://eed.nanxuanxn.top

Java: public / protected / private / 默认包级
来源：http://yhm.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://krz.guowangkeji.top

Ruby: public / protected / private
来源：http://ynu.yfazqb.com

C#:   public / protected / private / internal
来源：http://hlh.316326.xyz

[G11] getter / setter
来源：http://hmr.nanxinkj.top

Py:   @property 与 @x.setter
来源：http://cko.jinqigufen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ngz.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://ggf.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://hrq.gogol.net.cn

Java: public String getName() { return name; }
来源：http://eee.daria6918.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qug.wangdashe.top

Ruby: attr_accessor :name
来源：http://ymg.ydjk.org.cn

C#:   public string Name { get; set; }
来源：http://mmx.zdbjq.cn

[G12] 对象转字符串
来源：http://knt.epnwcf.com

Py:   def __str__(self): return self.name
来源：http://pyw.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jzr.zhijiandao.cn

JS:   toString() { return this.name; }
来源：http://jyc.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://fda.316326.xyz

Java: @Override public String toString() { return name; }
来源：http://nbc.gaohongyu789.top

Go:   func (u User) String() string { return u.Name }
来源：http://zcy.iojbl.cn

Ruby: def to_s; @name; end
来源：http://lfl.yj20258.top

C#:   public override string ToString() => Name;
来源：http://vto.ppjwa.cn

[G13] 判断对象类型
来源：http://nvl.tanke756.top

Py:   isinstance(u, User)
来源：http://mud.iojbl.cn

PHP:  $u instanceof User
来源：http://qdd.jinyuanbaomall.cn

JS:   u instanceof User
来源：http://okc.sjlbkw.cn

TS:   u instanceof User
来源：http://jlj.gzhubu.top

Java: u instanceof User
来源：http://cim.guowangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ffr.pengpengdd.cyou

Ruby: u.is_a?(User)
来源：http://xcz.jyoumei.cn

C#:   u is User
来源：http://wav.gogol.net.cn

[G14] 数据类 / record
来源：http://baq.hesvh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wjg.jiagoushi.top

PHP:  // 用 readonly 属性模拟
来源：http://dfp.quarkkingdee.top

JS:   // 无内置：普通类或对象字面量
来源：http://mmk.nanxuanxn.top

TS:   type User = { name: string; age: number };
来源：http://xxr.hesvh.cn

Java: record User(String name, int age) {}
来源：http://kcw.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://fpu.haohaochexian.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cjn.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://osy.hysaishi.cn

[G15] 枚举
来源：http://icd.cqqwz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qsa.xziqi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jdi.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gam.tanke756.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ikc.iojbl.cn

Java: enum Color { RED, GREEN }
来源：http://bpf.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jjq.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://ymf.zhongyouzk.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gbv.wangdashe.top

[G16] 对象转数组 / 字典
来源：http://jbp.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oup.ivvv.top

PHP:  get_object_vars($obj);
来源：http://cta.zhiwuduotai.top

JS:   Object.entries(obj)
来源：http://uot.zhongyouzk.top

TS:   Object.entries(obj)
来源：http://uti.xingfuxueyuan.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kui.aibaodan.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ygn.andypj.xyz

Ruby: obj.instance_variables
来源：http://fhb.dashuyun.cn

C#:   // 用反射或 System.Text.Json
来源：http://fnx.chenjidiqi.icu

================================================================================
来源：http://ybo.zhiwuduotai.top

H. 异常与错误处理
来源：http://nec.zhaomingkeji.xyz

================================================================================
来源：http://nrq.zhaomingkeji.xyz

[H01] try / catch 基础
来源：http://wvr.chenjidiqi.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ans.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mza.xziqi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lsu.hcnkem.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gqk.ctjpmb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fqq.ybcxt.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qhs.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eub.redwolf501.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bxs.shanyushiyangtech.top

[H02] finally / ensure 收尾
来源：http://ota.pengpengdd.cyou

Py:   try: f()⏎finally: cleanup()
来源：http://bhl.zdbjq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://odl.havefunace.top

JS:   try { f(); } finally { cleanup(); }
来源：http://eiv.xziqi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ppc.fengsongda.top

Java: try { f(); } finally { cleanup(); }
来源：http://jgn.yueranfly.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://afy.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ium.zhengqikj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zmp.zhijiandao.cn

[H03] 主动抛出异常
来源：http://gaw.aibaodan.cn

Py:   raise ValueError("错误信息")
来源：http://tix.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cvc.iojbl.cn

JS:   throw new Error("错误信息");
来源：http://ppt.zhengqikj.top

TS:   throw new Error("错误信息");
来源：http://wyt.hcnkem.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://tkz.0kj1m.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fda.tanke756.top

Ruby: raise ArgumentError, "错误信息"
来源：http://oim.ywan-chungtsiang.top

C#:   throw new ArgumentException("错误信息");
来源：http://hnx.andypj.xyz

[H04] 自定义异常类型
来源：http://pon.hcnkem.com

Py:   class MyError(Exception): pass
来源：http://zcl.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://dnv.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://hyx.gogol.net.cn

TS:   class MyError extends Error {}
来源：http://rci.chenjidiqi.icu

Java: class MyException extends RuntimeException {}
来源：http://wtw.0kj1m.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uqa.redwolf501.top

Ruby: class MyError < StandardError; end
来源：http://twk.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://mmy.cucudq.cn

[H05] 捕获特定类型
来源：http://qyf.hcnkem.com

Py:   except ValueError as e:
来源：http://ljk.fzhhl.top


<!-- 参考信息 -->