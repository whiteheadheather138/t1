代发 wailian999

[F01] 读取整个文件
来源：http://kzh.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://soo.jinghuilouyu.cn

PHP:  file_get_contents("a.txt");
来源：http://ftv.dianchejie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://inx.fehbvm.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pva.guannengcc.top

Java: Files.readString(Path.of("a.txt"))
来源：http://boz.xuanzx.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tvo.andypj.xyz

Ruby: File.read("a.txt")
来源：http://hzn.cheryme.top

C#:   File.ReadAllText("a.txt");
来源：http://abu.hywenlv.cn

[F02] 逐行读取文件
来源：http://ofm.daxiang520.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cic.birdmap.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tit.ctjpmb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pny.hammf.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ymy.haohaochexian.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nlh.sufxvd.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cff.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fgd.316326.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://arz.andypj.xyz

[F03] 写入文件（覆盖）
来源：http://llt.yangfankeji.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rbd.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ubi.sjlbkw.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lit.gogol.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qlw.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rnr.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rjh.havefunace.top

Ruby: File.write("a.txt", "hi")
来源：http://efg.c1oappe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ezl.jinyuanbaomall.cn

[F04] 追加写入文件
来源：http://uol.hywenlv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xfh.sysykeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dds.guannengcc.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ybq.jinqigfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rlt.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ykb.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xah.gotoacloud.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://run.dashuyun.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aoz.jinqigfzy.top

[F05] 判断文件或目录是否存在
来源：http://rab.zhiwuduotai.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rhe.wangdashe.top

PHP:  file_exists("a.txt");
来源：http://ofw.jinyuanbaomall.cn

JS:   fs.existsSync("a.txt")
来源：http://baj.jqgfzy.top

TS:   fs.existsSync("a.txt")
来源：http://uys.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lli.nanxinkj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dnm.zdbjq.cn

Ruby: File.exist?("a.txt")
来源：http://kwc.andypj.xyz

C#:   File.Exists("a.txt")
来源：http://fmy.sufxvd.cn

[F06] 删除文件
来源：http://tjc.bbcook.cn

Py:   os.remove("a.txt")
来源：http://ito.redwolf501.top

PHP:  unlink("a.txt");
来源：http://qru.guowangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://btv.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://qdo.guannengcc.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://unt.pengpengdd.cyou

Go:   os.Remove("a.txt")
来源：http://tzy.guannengcc.top

Ruby: File.delete("a.txt")
来源：http://iwu.zhongyouzk.top

C#:   File.Delete("a.txt");
来源：http://ghj.wangdashe.top

[F07] 创建目录（含多级）
来源：http://pov.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jgj.fengsongda.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iqq.fktsv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aqe.xinyue.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fil.zdqjudy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pat.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yyu.xylfe.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wbo.haohaochexian.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://haj.shzxlz.cn

[F08] 遍历目录
来源：http://fti.ydzc1.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nvd.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bvp.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://fvb.aibaodan.cn

TS:   fs.readdirSync("dir")
来源：http://yoa.0kj1m.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cha.yonumen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gcb.vqdsnc.cn

Ruby: Dir.children("dir")
来源：http://cxh.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://uqz.snrcjt.cn

[F09] 获取文件大小
来源：http://qbs.pycfn.com

Py:   os.path.getsize("a.txt")
来源：http://ggj.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://xcc.haohaochexian.top

JS:   fs.statSync("a.txt").size
来源：http://jrz.mhx1999.top

TS:   fs.statSync("a.txt").size
来源：http://kkl.shangyingyoupin.top

Java: Files.size(Path.of("a.txt"))
来源：http://rdd.bjfxy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ynl.xinyue.icu

Ruby: File.size("a.txt")
来源：http://jgs.52xcode.cn

C#:   new FileInfo("a.txt").Length
来源：http://deq.shzxlz.cn

[F10] 取文件扩展名 / 文件名
来源：http://rll.bjfxy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://urr.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zeb.fengsongda.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dlr.iojbl.cn

TS:   path.extname("a.txt")
来源：http://qhw.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pun.gogol.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ihm.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rqc.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rel.andypj.xyz

[F11] 复制与移动文件
来源：http://xho.316326.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sro.wangdashe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vkh.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wix.zhaomingkeji.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qyp.cashguo.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yqz.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ory.hcnkem.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://map.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ueu.snrcjt.cn

[F12] CSV 读写
来源：http://dsr.cheryme.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hux.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xoq.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xmu.zdbjq.cn

TS:   // 同上
来源：http://cqn.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://utc.feifeiyinyue.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pvz.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://knj.fzhhl.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rij.wangshuangyany.cn

================================================================================
来源：http://kkl.jqgfzy.top

G. 面向对象
来源：http://ynq.tanke756.top

================================================================================
来源：http://uzx.tianlin.xyz

[G01] 定义类
来源：http://erl.chenjidiqi.icu

Py:   class User: pass
来源：http://iud.daxiang520.top

PHP:  class User {}
来源：http://jtl.aibaodan.cn

JS:   class User {}
来源：http://lla.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://ewv.zhijiandao.cn

Java: class User {}
来源：http://ogv.birdmap.top

Go:   type User struct { Name string }
来源：http://kgx.ydzc1.top

Ruby: class User; end
来源：http://mlx.cashguo.top

C#:   class User {}
来源：http://pfg.sjlbkw.cn

[G02] 构造函数
来源：http://xzu.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://pns.tarul.cn

PHP:  public function __construct(public string $name) {}
来源：http://lwm.yj20258.top

JS:   constructor(name) { this.name = name; }
来源：http://boh.gaohongyu789.top

TS:   constructor(public name: string) {}
来源：http://ehd.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://iir.ehwqpu.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ghj.guowangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://erz.havefunace.top

C#:   public User(string name) { Name = name; }
来源：http://mce.chenjidiqi.icu

[G03] 实例属性
来源：http://jif.zdbjq.cn

Py:   self.name = "x"
来源：http://wht.nwbrower.top

PHP:  public string $name = "x";
来源：http://zfd.ivvv.top

JS:   this.name = "x";
来源：http://zlb.nanxuanxn.top

TS:   name: string = "x";
来源：http://sdu.c1oappe.top

Java: private String name;
来源：http://gdp.mhx1999.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oht.bjfxy.top

Ruby: @name = "x"
来源：http://uyh.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://jdu.zhoulong.xyz

[G04] 定义方法
来源：http://mvr.gzhubu.top

Py:   def greet(self): return self.name
来源：http://qiq.daria6918.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tzi.xuetiantiany.cn

JS:   greet() { return this.name; }
来源：http://bkw.yj20258.top

TS:   greet(): string { return this.name; }
来源：http://nvx.jinghuilouyu.cn

Java: String greet() { return name; }
来源：http://eix.ywan-chungtsiang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://orj.vqdsnc.cn

Ruby: def greet; @name; end
来源：http://uzo.bjfxy.top

C#:   public string Greet() => Name;
来源：http://njc.meibo888.top

[G05] 继承
来源：http://nlh.gaohongyu789.top

Py:   class Admin(User): pass
来源：http://dwf.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://rso.hywenlv.cn

JS:   class Admin extends User {}
来源：http://kcb.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://nnc.havefunace.top

Java: class Admin extends User {}
来源：http://qwk.cqqwz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hhk.nanxinkj.top

Ruby: class Admin < User; end
来源：http://thz.hnxiangtu.top

C#:   class Admin : User {}
来源：http://xlv.fzhhl.top

[G06] 重写方法
来源：http://yjj.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://rnr.yanxiufei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hny.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://gff.quarkkingdee.top

TS:   greet(): string { return "admin"; }
来源：http://bck.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://gqn.aibaodan.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ill.yuxming.cn

Ruby: def greet; "admin"; end
来源：http://hpy.yuxming.cn

C#:   public override string Greet() => "admin";
来源：http://pvv.jinqigufen.top

[G07] 调用父类方法
来源：http://mtu.chenzaomai.com

Py:   super().greet()
来源：http://eje.ydjk.org.cn

PHP:  parent::greet();
来源：http://tom.wangshuangyany.cn

JS:   super.greet();
来源：http://vbz.quarkkingdee.top

TS:   super.greet();
来源：http://iet.sxryk.cn

Java: super.greet();
来源：http://nio.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lzr.aizwys.cn

Ruby: super
来源：http://lvw.zhixingplan.top

C#:   base.Greet();
来源：http://jjj.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://yvo.gzhubu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iel.fehbvm.com

PHP:  public static function f() {}
来源：http://iks.fzhhl.top

JS:   static f() {}
来源：http://oym.cdnleiting.top

TS:   static f(): void {}
来源：http://xak.yfazqb.com

Java: static void f() {}
来源：http://faj.ppjwa.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://guz.c1oappe.top

Ruby: def self.f; end
来源：http://woa.gotoacloud.top

C#:   public static void F() {}
来源：http://ztf.sjlbkw.cn

[G09] 接口 / 抽象类
来源：http://zrg.ydzc1.top

Py:   from abc import ABC, abstractmethod
来源：http://ojb.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://kxg.yangfankeji.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://pbw.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://lcq.smart0.xyz

Java: interface Shape { double area(); }
来源：http://kyp.yuxming.cn

Go:   type Shape interface { Area() float64 }
来源：http://tfc.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xcc.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://kzr.cqqwz.cn

[G10] 访问控制
来源：http://hje.daxiang520.top

Py:   约定 _protected / __private（不强制）
来源：http://aqj.yj20258.top

PHP:  public / protected / private
来源：http://ayn.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://slg.meibo888.top

TS:   public / protected / private
来源：http://hap.vqdsnc.cn

Java: public / protected / private / 默认包级
来源：http://cnf.zhaomingkeji.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://och.jqgufenzy.top

Ruby: public / protected / private
来源：http://tby.hywenlv.cn

C#:   public / protected / private / internal
来源：http://dho.52xcode.cn

[G11] getter / setter
来源：http://yqp.gotoacloud.top

Py:   @property 与 @x.setter
来源：http://fhh.guowangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rnt.xuetiantiany.cn

JS:   get name() { return this._name; }
来源：http://fhg.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://mhu.ywan-chungtsiang.top

Java: public String getName() { return name; }
来源：http://qez.quarkkingdee.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://oje.tanke756.top

Ruby: attr_accessor :name
来源：http://nzt.shangyingyoupin.top

C#:   public string Name { get; set; }
来源：http://axy.snrcjt.cn

[G12] 对象转字符串
来源：http://wva.nwbrower.top

Py:   def __str__(self): return self.name
来源：http://gqy.hcnkem.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://jfj.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://ind.hnqzz.top

TS:   toString(): string { return this.name; }
来源：http://mzl.yueranfly.top

Java: @Override public String toString() { return name; }
来源：http://kgc.ywan-chungtsiang.top

Go:   func (u User) String() string { return u.Name }
来源：http://key.daria6918.cn

Ruby: def to_s; @name; end
来源：http://yie.haohaochexian.top

C#:   public override string ToString() => Name;
来源：http://xlv.bjfxy.top

[G13] 判断对象类型
来源：http://eoi.sweek.top

Py:   isinstance(u, User)
来源：http://vrg.jianghu66.top

PHP:  $u instanceof User
来源：http://ajc.shuidangran.top

JS:   u instanceof User
来源：http://ohw.vqdsnc.cn

TS:   u instanceof User
来源：http://fgt.yfazqb.com

Java: u instanceof User
来源：http://pmt.iojbl.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://blx.zhaomingkeji.xyz

Ruby: u.is_a?(User)
来源：http://qic.epnwcf.com

C#:   u is User
来源：http://kgv.yj202588.top

[G14] 数据类 / record
来源：http://rzd.yj202588.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zmu.sweek.top

PHP:  // 用 readonly 属性模拟
来源：http://xty.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://ctn.cqqwz.cn

TS:   type User = { name: string; age: number };
来源：http://pjq.tarul.cn

Java: record User(String name, int age) {}
来源：http://spv.cashguo.top

Go:   type User struct { Name string; Age int }
来源：http://unx.hywenlv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hkj.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://sag.tian-w.cn

[G15] 枚举
来源：http://ahc.sweek.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ouj.9152youxi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nvy.dashuyun.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fwr.yueranfly.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jeu.daria6918.cn

Java: enum Color { RED, GREEN }
来源：http://sdb.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://smo.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://idp.nwbrower.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kpc.sjlbkw.cn

[G16] 对象转数组 / 字典
来源：http://okw.tianlin.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ewt.wangdashe.top

PHP:  get_object_vars($obj);
来源：http://xni.hammf.cn

JS:   Object.entries(obj)
来源：http://urv.haohaochexian.top

TS:   Object.entries(obj)
来源：http://hgm.fehbvm.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hut.sysykeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dvv.fzhhl.top

Ruby: obj.instance_variables
来源：http://iwk.guannengcc.top

C#:   // 用反射或 System.Text.Json
来源：http://clj.havefunace.top

================================================================================
来源：http://dlm.chenlongwang.top

H. 异常与错误处理
来源：http://ajy.redwolf501.top

================================================================================
来源：http://bsm.yueranfly.top

[H01] try / catch 基础
来源：http://uav.yj202588.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lyh.52xcode.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tlx.gzhubu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wzg.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://spc.andypj.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ypz.quarkkingdee.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sil.tian-w.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mre.9152youxi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vpi.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://adl.wangdashe.top

Py:   try: f()⏎finally: cleanup()
来源：http://cve.haohaochexian.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zqv.hywenlv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gsj.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kre.0kj1m.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yfw.hesvh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nop.gzhubu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zsr.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oza.guannengcc.top

[H03] 主动抛出异常
来源：http://naw.quarkkingdee.top

Py:   raise ValueError("错误信息")
来源：http://exb.epnwcf.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://col.shanyushiyangkeji.top

JS:   throw new Error("错误信息");
来源：http://tya.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://bad.nanxinkj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xbu.uphjek.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://czu.andypj.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://pwg.chenjidiqi.icu

C#:   throw new ArgumentException("错误信息");
来源：http://sov.jqgufenzy.top

[H04] 自定义异常类型
来源：http://wus.sxryk.cn

Py:   class MyError(Exception): pass
来源：http://txs.bjfxy.top

PHP:  class MyError extends RuntimeException {}
来源：http://veh.chenlongwang.top

JS:   class MyError extends Error {}
来源：http://yyi.aizwys.cn

TS:   class MyError extends Error {}
来源：http://guo.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://vxr.fehbvm.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xcc.nanxinkj.top

Ruby: class MyError < StandardError; end
来源：http://bxu.ydjk.org.cn

C#:   class MyException : Exception {}
来源：http://oye.epnwcf.com

[H05] 捕获特定类型
来源：http://rim.9152youxi.cn

Py:   except ValueError as e:
来源：http://rhg.yangfankeji.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oen.birdmap.top

JS:   if (e instanceof TypeError) {}
来源：http://vyl.hysaishi.cn

TS:   if (e instanceof TypeError) {}
来源：http://lrc.gaohongyu789.top

Java: catch (IOException | SQLException e) {}
来源：http://pdd.wangshuangyany.cn


<!-- 参考信息 -->