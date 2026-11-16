代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nqz.52xcode.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://iep.daxiang520.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pzm.iojbl.cn

Ruby: File.read("a.txt")
来源：http://fkp.yfazqb.com

C#:   File.ReadAllText("a.txt");
来源：http://xdn.yuxming.cn

[F02] 逐行读取文件
来源：http://pyk.hfpthk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nvl.chenjidiqi.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iut.52xcode.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://usn.xuanzx.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oat.uphjek.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jjc.fzhhl.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ilo.nwbrower.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://apg.mhx1999.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sdd.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://nwt.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oac.bjfxy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xsf.ppjwa.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pxt.zycfv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aew.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yni.mhx1999.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qdg.cashguo.top

Ruby: File.write("a.txt", "hi")
来源：http://hak.jianghu66.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://abo.daria6918.cn

[F04] 追加写入文件
来源：http://ymh.dashuyun.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rwq.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uvd.hysaishi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fst.guannengcc.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://obo.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aaz.ydjk.org.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wgp.dashuyun.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fae.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bbj.nwbrower.top

[F05] 判断文件或目录是否存在
来源：http://nog.bjfxy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ztx.tian-w.cn

PHP:  file_exists("a.txt");
来源：http://xjx.zhixingplan.top

JS:   fs.existsSync("a.txt")
来源：http://dnz.meibo888.top

TS:   fs.existsSync("a.txt")
来源：http://auy.xylfe.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mae.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wvj.gzhubu.top

Ruby: File.exist?("a.txt")
来源：http://aer.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://tcq.yonumen.top

[F06] 删除文件
来源：http://wxs.nwbrower.top

Py:   os.remove("a.txt")
来源：http://tql.fehbvm.com

PHP:  unlink("a.txt");
来源：http://oro.zhiwuduotai.top

JS:   fs.unlinkSync("a.txt")
来源：http://laj.epnwcf.com

TS:   fs.unlinkSync("a.txt")
来源：http://pqe.sufxvd.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dbl.smart0.xyz

Go:   os.Remove("a.txt")
来源：http://cza.guannengcc.top

Ruby: File.delete("a.txt")
来源：http://udp.jinyuanbaomall.cn

C#:   File.Delete("a.txt");
来源：http://pgc.zdqjudy.top

[F07] 创建目录（含多级）
来源：http://fxw.hysaishi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mvb.havefunace.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kuj.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tit.gzhubu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oxx.shangyingyoupin.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uig.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cuy.nanxuanxn.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gwl.tianlin.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xru.guannengcc.top

[F08] 遍历目录
来源：http://kyc.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jaq.sweek.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pcf.yvedp.cn

JS:   fs.readdirSync("dir")
来源：http://pgx.cheryme.top

TS:   fs.readdirSync("dir")
来源：http://fxy.jinqigfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zan.yangfankeji.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://aql.yfazqb.com

Ruby: Dir.children("dir")
来源：http://xwc.ybcxt.top

C#:   Directory.GetFiles("dir")
来源：http://xab.52xcode.cn

[F09] 获取文件大小
来源：http://ofe.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://cvs.iojbl.cn

PHP:  filesize("a.txt");
来源：http://zci.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://kol.hfpthk.cn

TS:   fs.statSync("a.txt").size
来源：http://tcy.vehdjk.com

Java: Files.size(Path.of("a.txt"))
来源：http://zvz.cucudq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fzb.sysykeji.top

Ruby: File.size("a.txt")
来源：http://awq.nwbrower.top

C#:   new FileInfo("a.txt").Length
来源：http://vnf.cqqwz.cn

[F10] 取文件扩展名 / 文件名
来源：http://fck.feifeiyinyue.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bxj.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tzp.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dbr.hcnkem.com

TS:   path.extname("a.txt")
来源：http://ymy.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qgy.epnwcf.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dzo.ydzc1.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ewb.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://inh.shzxlz.cn

[F11] 复制与移动文件
来源：http://iqz.shanyushiyangtech.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rgv.fanxiaobao.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tqf.sjlbkw.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tha.iojbl.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zsx.yueranfly.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rjb.hfpthk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bnw.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bus.yonumen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://inj.hcnkem.com

[F12] CSV 读写
来源：http://fcg.redwolf501.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cqx.hongshengwenyu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wtb.c1oappe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tnl.bjfxy.top

TS:   // 同上
来源：http://ias.yfazqb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rhh.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kgu.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qjx.jqgufenzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://quf.ywan-chungtsiang.top

================================================================================
来源：http://rpp.kuanghao11.cn

G. 面向对象
来源：http://kfh.gotoacloud.top

================================================================================
来源：http://fty.sjlbkw.cn

[G01] 定义类
来源：http://exu.xinyue.icu

Py:   class User: pass
来源：http://yjk.zhengqikj.top

PHP:  class User {}
来源：http://brv.haohaochexian.top

JS:   class User {}
来源：http://vqa.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://hih.zhiwuduotai.top

Java: class User {}
来源：http://xbj.gogol.net.cn

Go:   type User struct { Name string }
来源：http://fyk.wangshuangyany.cn

Ruby: class User; end
来源：http://xqy.hfpthk.cn

C#:   class User {}
来源：http://yml.zhoulong.xyz

[G02] 构造函数
来源：http://ihc.kuanghao11.cn

Py:   def __init__(self, name): self.name = name
来源：http://ebs.zhiwuduotai.top

PHP:  public function __construct(public string $name) {}
来源：http://rxx.zhixingplan.top

JS:   constructor(name) { this.name = name; }
来源：http://rpv.zhiwuduotai.top

TS:   constructor(public name: string) {}
来源：http://fuq.daxiang520.top

Java: User(String name) { this.name = name; }
来源：http://ypd.xuanzx.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mjh.nwbrower.top

Ruby: def initialize(name); @name = name; end
来源：http://ddg.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://myc.hammf.cn

[G03] 实例属性
来源：http://yhl.zhaomingkeji.xyz

Py:   self.name = "x"
来源：http://kxv.zdqjudy.top

PHP:  public string $name = "x";
来源：http://rtx.aibaodan.cn

JS:   this.name = "x";
来源：http://djv.vqdsnc.cn

TS:   name: string = "x";
来源：http://nxc.meibo888.top

Java: private String name;
来源：http://kst.ehwqpu.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bog.fzhhl.top

Ruby: @name = "x"
来源：http://ehu.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://ytl.ydjk.org.cn

[G04] 定义方法
来源：http://hqn.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://gjv.fanxiaobao.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://gkc.yangfankeji.com

JS:   greet() { return this.name; }
来源：http://jkn.kuanghao11.cn

TS:   greet(): string { return this.name; }
来源：http://dnx.tanke756.top

Java: String greet() { return name; }
来源：http://jcq.epnwcf.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://vxs.cqqwz.cn

Ruby: def greet; @name; end
来源：http://clf.redwolf501.top

C#:   public string Greet() => Name;
来源：http://xdq.hfpthk.cn

[G05] 继承
来源：http://dbt.hnxiangtu.top

Py:   class Admin(User): pass
来源：http://gaz.pengpengdd.cyou

PHP:  class Admin extends User {}
来源：http://tga.xylfe.cn

JS:   class Admin extends User {}
来源：http://kxp.ppjwa.cn

TS:   class Admin extends User {}
来源：http://fpj.hcnkem.com

Java: class Admin extends User {}
来源：http://mzn.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wyl.c1oappe.top

Ruby: class Admin < User; end
来源：http://nze.yonumen.top

C#:   class Admin : User {}
来源：http://phw.wangdashe.top

[G06] 重写方法
来源：http://nyx.cdnleiting.top

Py:   def greet(self): return "admin"
来源：http://obt.tanke756.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xdd.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://bdt.jianghu66.top

TS:   greet(): string { return "admin"; }
来源：http://jmr.epnwcf.com

Java: @Override String greet() { return "admin"; }
来源：http://wby.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oan.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://yfr.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://abg.pycfn.com

[G07] 调用父类方法
来源：http://gzx.fanxiaobao.xyz

Py:   super().greet()
来源：http://inp.snrcjt.cn

PHP:  parent::greet();
来源：http://gja.shuidangran.top

JS:   super.greet();
来源：http://wwm.yj202588.top

TS:   super.greet();
来源：http://kjb.hnqzz.top

Java: super.greet();
来源：http://azm.9152youxi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vok.haohaochexian.top

Ruby: super
来源：http://voa.shanyushiyangtech.top

C#:   base.Greet();
来源：http://vlf.nanxuanxn.top

[G08] 静态方法与属性
来源：http://fmp.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vbb.birdmap.top

PHP:  public static function f() {}
来源：http://dbl.ydzc1.top

JS:   static f() {}
来源：http://kbr.yuanzhike.top

TS:   static f(): void {}
来源：http://zxw.zhixingplan.top

Java: static void f() {}
来源：http://gzd.vehdjk.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://eca.uphjek.com

Ruby: def self.f; end
来源：http://ref.dianchejie.cn

C#:   public static void F() {}
来源：http://teg.dashuyun.cn

[G09] 接口 / 抽象类
来源：http://sgu.zdbjq.cn

Py:   from abc import ABC, abstractmethod
来源：http://xuo.bbcook.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yns.jinyuanbaomall.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fhs.redwolf501.top

TS:   interface Shape { area(): number; }
来源：http://mca.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://bhn.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://wzi.xingfuxueyuan.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nbr.cqqwz.cn

C#:   interface IShape { double Area(); }
来源：http://nyj.iojbl.cn

[G10] 访问控制
来源：http://fle.yuanzhike.top

Py:   约定 _protected / __private（不强制）
来源：http://okr.xuetiantiany.cn

PHP:  public / protected / private
来源：http://aol.yfazqb.com

JS:   #private 字段；其余公开
来源：http://hai.hywenlv.cn

TS:   public / protected / private
来源：http://uwo.uphjek.com

Java: public / protected / private / 默认包级
来源：http://mxe.pycfn.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://wvl.yvedp.cn

Ruby: public / protected / private
来源：http://hyn.yangfankeji.com

C#:   public / protected / private / internal
来源：http://ykz.yfazqb.com

[G11] getter / setter
来源：http://dzw.hesvh.cn

Py:   @property 与 @x.setter
来源：http://tjx.hysaishi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://onm.ctjpmb.com

JS:   get name() { return this._name; }
来源：http://taw.gogol.net.cn

TS:   get name(): string { return this._name; }
来源：http://jwz.hysaishi.cn

Java: public String getName() { return name; }
来源：http://omq.zhiwuduotai.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fau.chenzaomai.com

Ruby: attr_accessor :name
来源：http://qfo.shanyushiyangtech.top

C#:   public string Name { get; set; }
来源：http://vto.xylfe.cn

[G12] 对象转字符串
来源：http://zjg.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://jjb.iojbl.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vrz.andypj.xyz

JS:   toString() { return this.name; }
来源：http://nkw.yuanzhike.top

TS:   toString(): string { return this.name; }
来源：http://ytl.guowangkeji.top

Java: @Override public String toString() { return name; }
来源：http://gpj.ydzc1.top

Go:   func (u User) String() string { return u.Name }
来源：http://dxn.jiagoushi.top

Ruby: def to_s; @name; end
来源：http://rsq.yonumen.top

C#:   public override string ToString() => Name;
来源：http://fsz.cashguo.top

[G13] 判断对象类型
来源：http://xey.shanyushiyangtech.top

Py:   isinstance(u, User)
来源：http://bwz.aizwys.cn

PHP:  $u instanceof User
来源：http://cfd.hysaishi.cn

JS:   u instanceof User
来源：http://xzn.tarul.cn

TS:   u instanceof User
来源：http://fys.fengsongda.top

Java: u instanceof User
来源：http://bhz.cqqwz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pap.xinyue.icu

Ruby: u.is_a?(User)
来源：http://yiu.hnxiangtu.top

C#:   u is User
来源：http://hkg.daxiang520.top

[G14] 数据类 / record
来源：http://igu.yvedp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wtl.0kj1m.cn

PHP:  // 用 readonly 属性模拟
来源：http://axl.epnwcf.com

JS:   // 无内置：普通类或对象字面量
来源：http://bgr.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://eih.yvedp.cn

Java: record User(String name, int age) {}
来源：http://sle.yueranfly.top

Go:   type User struct { Name string; Age int }
来源：http://fjj.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://seq.chenzaomai.com

C#:   record User(string Name, int Age);
来源：http://enf.jinyuanbaomall.cn

[G15] 枚举
来源：http://oqw.cqqwz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uny.jinyuanbaomall.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ubv.tian-w.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sab.chenlongwang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nto.cdnleiting.top

Java: enum Color { RED, GREEN }
来源：http://jzy.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aip.gogol.net.cn

Ruby: Color = %i[red green].freeze
来源：http://wwd.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lkz.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://opu.zdbjq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jpi.kuanghao11.cn

PHP:  get_object_vars($obj);
来源：http://hqc.hysaishi.cn

JS:   Object.entries(obj)
来源：http://mvk.xuetiantiany.cn

TS:   Object.entries(obj)
来源：http://wxa.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tgy.zhengqikj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://frf.jinqigfzy.top

Ruby: obj.instance_variables
来源：http://rbj.daria6918.cn

C#:   // 用反射或 System.Text.Json
来源：http://rjj.0kj1m.cn

================================================================================
来源：http://njc.xuetiantiany.cn

H. 异常与错误处理
来源：http://fxj.yangfankeji.com

================================================================================
来源：http://nkp.sjlbkw.cn

[H01] try / catch 基础
来源：http://gng.gaohongyu789.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ncf.yueranfly.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vlt.gogol.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xjs.jinghuilouyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ofh.vqdsnc.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kco.pengpengdd.cyou

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iis.tianlin.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eck.9152youxi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://psy.uphjek.com

[H02] finally / ensure 收尾
来源：http://oef.aizwys.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tvn.ywan-chungtsiang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vam.feifeiyinyue.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xtu.gotoacloud.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qtp.gotoacloud.top

Java: try { f(); } finally { cleanup(); }
来源：http://epj.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rfv.tarul.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zvg.wangdashe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://iov.jinyuanbaomall.cn

[H03] 主动抛出异常
来源：http://nlb.zhijiandao.cn

Py:   raise ValueError("错误信息")
来源：http://key.vehdjk.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://flh.mhx1999.top

JS:   throw new Error("错误信息");
来源：http://ldx.52xcode.cn

TS:   throw new Error("错误信息");
来源：http://xdg.zhongyouzk.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://biq.hcnkem.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gaj.zdbjq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xwc.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://erg.zdbjq.cn

[H04] 自定义异常类型
来源：http://eol.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://oiw.zhaomingkeji.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://mzd.tian-w.cn

JS:   class MyError extends Error {}
来源：http://nvi.shzxlz.cn

TS:   class MyError extends Error {}
来源：http://vyc.andypj.xyz

Java: class MyException extends RuntimeException {}
来源：http://xkf.aizwys.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jjb.ywan-chungtsiang.top

Ruby: class MyError < StandardError; end
来源：http://tss.xinyue.icu

C#:   class MyException : Exception {}
来源：http://vhi.meibo888.top

[H05] 捕获特定类型
来源：http://pho.ctjpmb.com

Py:   except ValueError as e:
来源：http://dvy.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ger.dianchejie.cn

JS:   if (e instanceof TypeError) {}
来源：http://jgi.zhixingplan.top

TS:   if (e instanceof TypeError) {}
来源：http://iho.xinyue.icu

Java: catch (IOException | SQLException e) {}
来源：http://oii.zdbjq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://egx.yonumen.top

Ruby: rescue ArgumentError => e
来源：http://oga.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hmu.daria6918.cn

[H06] 可选值 / 空值安全访问
来源：http://gau.yj20258888.top


<!-- 参考信息 -->