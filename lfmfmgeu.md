代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://inc.jianghu66.top

[F02] 逐行读取文件
来源：http://qse.hfpthk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vpn.xinyue.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ltq.nwbrower.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ywx.fengsongda.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zez.wangshuangyany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lrt.jlsjyb.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iby.cdnleiting.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jef.zhaomingkeji.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hpb.52xcode.cn

[F03] 写入文件（覆盖）
来源：http://xyz.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ffb.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ern.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ufl.shanyushiyangtech.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tju.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ecc.sweek.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gmx.shanyushiyangtech.top

Ruby: File.write("a.txt", "hi")
来源：http://iar.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qma.hongshengwenyu.top

[F04] 追加写入文件
来源：http://vzt.ydjk.org.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tkv.c1oappe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tts.vqdsnc.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wkb.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rvm.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nbt.gzhubu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qks.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://avo.yueranfly.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://npk.sjlbkw.cn

[F05] 判断文件或目录是否存在
来源：http://ush.ivvv.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://usa.jqgufenzy.top

PHP:  file_exists("a.txt");
来源：http://ugf.bjfxy.top

JS:   fs.existsSync("a.txt")
来源：http://jnt.jqgfzy.top

TS:   fs.existsSync("a.txt")
来源：http://kmu.zhongyouzk.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nue.hnqzz.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bsh.xziqi.cn

Ruby: File.exist?("a.txt")
来源：http://avk.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://wel.9152youxi.cn

[F06] 删除文件
来源：http://tno.ybcxt.top

Py:   os.remove("a.txt")
来源：http://deg.jlsjyb.cn

PHP:  unlink("a.txt");
来源：http://fwe.guowangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://hak.epnwcf.com

TS:   fs.unlinkSync("a.txt")
来源：http://yfm.pycfn.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nho.hysaishi.cn

Go:   os.Remove("a.txt")
来源：http://jrt.yj20258.top

Ruby: File.delete("a.txt")
来源：http://xjg.jqgfzy.top

C#:   File.Delete("a.txt");
来源：http://odd.nanxinkj.top

[F07] 创建目录（含多级）
来源：http://xfw.epnwcf.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://stq.0kj1m.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mfm.zhoulong.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nes.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hqi.wangdashe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rtf.zhixingplan.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mmw.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gyo.jianghu66.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://atq.hfpthk.cn

[F08] 遍历目录
来源：http://pxa.xuetiantiany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jbp.jianghu66.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hqb.0kj1m.cn

JS:   fs.readdirSync("dir")
来源：http://etb.fengsongda.top

TS:   fs.readdirSync("dir")
来源：http://nqu.yuxming.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bqj.yvedp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fwy.chenjidiqi.icu

Ruby: Dir.children("dir")
来源：http://lhn.kuanghao11.cn

C#:   Directory.GetFiles("dir")
来源：http://euz.gogol.net.cn

[F09] 获取文件大小
来源：http://qnq.haohaochexian.top

Py:   os.path.getsize("a.txt")
来源：http://hib.pycfn.com

PHP:  filesize("a.txt");
来源：http://skp.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://zkt.52xcode.cn

TS:   fs.statSync("a.txt").size
来源：http://yjy.fanxiaobao.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://dqs.yj20258888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fon.sufxvd.cn

Ruby: File.size("a.txt")
来源：http://mct.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://qls.yj202588.top

[F10] 取文件扩展名 / 文件名
来源：http://pte.jinyuanbaomall.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ppz.yj20258.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fhb.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fzb.jianghu66.top

TS:   path.extname("a.txt")
来源：http://zzu.jyoumei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ocf.tianlin.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://crm.andypj.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rye.aibaodan.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eza.chenzaomai.com

[F11] 复制与移动文件
来源：http://veb.hfpthk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zar.yongpay.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ywh.ywan-chungtsiang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zsy.jqgufenzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xbd.shzxlz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bzw.zycfv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kzg.dashuyun.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vom.xylfe.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yyc.daxiang520.top

[F12] CSV 读写
来源：http://xhh.cheryme.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zhs.hcnkem.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wdg.fengsongda.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vtf.wangdashe.top

TS:   // 同上
来源：http://ntw.ehwqpu.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hmi.daxiang520.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bmo.smart0.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nxs.meibo888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ijc.epnwcf.com

================================================================================
来源：http://rdj.xinyue.icu

G. 面向对象
来源：http://aou.sysykeji.top

================================================================================
来源：http://ziq.wangdashe.top

[G01] 定义类
来源：http://bsk.xinyue.icu

Py:   class User: pass
来源：http://bad.wangshuangyany.cn

PHP:  class User {}
来源：http://xfq.cucudq.cn

JS:   class User {}
来源：http://edq.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://dzz.sweek.top

Java: class User {}
来源：http://fhq.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://nhf.zhaomingkeji.xyz

Ruby: class User; end
来源：http://gvq.tianlin.xyz

C#:   class User {}
来源：http://kco.feifeiyinyue.top

[G02] 构造函数
来源：http://qpr.snrcjt.cn

Py:   def __init__(self, name): self.name = name
来源：http://vbr.fanxiaobao.xyz

PHP:  public function __construct(public string $name) {}
来源：http://vjm.pengpengdd.cyou

JS:   constructor(name) { this.name = name; }
来源：http://rph.jinghuilouyu.cn

TS:   constructor(public name: string) {}
来源：http://hel.shangyingyoupin.top

Java: User(String name) { this.name = name; }
来源：http://vuo.bbcook.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oit.yj20258.top

Ruby: def initialize(name); @name = name; end
来源：http://hwd.cdnleiting.top

C#:   public User(string name) { Name = name; }
来源：http://nfn.gotoacloud.top

[G03] 实例属性
来源：http://nde.tanke756.top

Py:   self.name = "x"
来源：http://piv.0kj1m.cn

PHP:  public string $name = "x";
来源：http://fet.meibo888.top

JS:   this.name = "x";
来源：http://fuf.316326.xyz

TS:   name: string = "x";
来源：http://bvd.nanxuanxn.top

Java: private String name;
来源：http://mru.hongshengwenyu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bta.zhiwuduotai.top

Ruby: @name = "x"
来源：http://qyu.ydzc1.top

C#:   public string Name { get; set; } = "x";
来源：http://sit.zdqjudy.top

[G04] 定义方法
来源：http://lhd.xuanzx.com

Py:   def greet(self): return self.name
来源：http://pqy.xingfuxueyuan.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://jei.chenjidiqi.icu

JS:   greet() { return this.name; }
来源：http://veq.zhixingplan.top

TS:   greet(): string { return this.name; }
来源：http://pae.nanxuanxn.top

Java: String greet() { return name; }
来源：http://yvj.wangshuangyany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ire.feifeiyinyue.top

Ruby: def greet; @name; end
来源：http://mgx.jqgfzy.top

C#:   public string Greet() => Name;
来源：http://uiy.jinqigufen.top

[G05] 继承
来源：http://akk.shangyingyoupin.top

Py:   class Admin(User): pass
来源：http://lyp.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://elu.fzhhl.top

JS:   class Admin extends User {}
来源：http://bfo.zhiwuduotai.top

TS:   class Admin extends User {}
来源：http://yoz.bbcook.cn

Java: class Admin extends User {}
来源：http://ybh.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://klm.cqqwz.cn

Ruby: class Admin < User; end
来源：http://jcw.zhoulong.xyz

C#:   class Admin : User {}
来源：http://udq.zhongyouzk.top

[G06] 重写方法
来源：http://xwm.hongshengwenyu.top

Py:   def greet(self): return "admin"
来源：http://ibf.nanxuanxn.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jlt.zhaomingkeji.xyz

JS:   greet() { return "admin"; }
来源：http://xjo.yongpay.top

TS:   greet(): string { return "admin"; }
来源：http://aqz.hnxiangtu.top

Java: @Override String greet() { return "admin"; }
来源：http://neb.ppjwa.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qby.nanxinkj.top

Ruby: def greet; "admin"; end
来源：http://ahj.svipenyu.cn

C#:   public override string Greet() => "admin";
来源：http://cqa.tian-w.cn

[G07] 调用父类方法
来源：http://mtf.fanxiaobao.xyz

Py:   super().greet()
来源：http://yfv.fengsongda.top

PHP:  parent::greet();
来源：http://jlf.snrcjt.cn

JS:   super.greet();
来源：http://xvu.zdqjudy.top

TS:   super.greet();
来源：http://voy.sufxvd.cn

Java: super.greet();
来源：http://xve.iojbl.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://faj.hfpthk.cn

Ruby: super
来源：http://jpp.fanxiaobao.xyz

C#:   base.Greet();
来源：http://jmp.jinqigufen.top

[G08] 静态方法与属性
来源：http://tbk.haohaochexian.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jzy.yonumen.top

PHP:  public static function f() {}
来源：http://kvo.0kj1m.cn

JS:   static f() {}
来源：http://pnl.zhiwuduotai.top

TS:   static f(): void {}
来源：http://dru.tianlin.xyz

Java: static void f() {}
来源：http://hpl.tianlin.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://jhd.xuanzx.com

Ruby: def self.f; end
来源：http://vvi.ctjpmb.com

C#:   public static void F() {}
来源：http://abz.gogol.net.cn

[G09] 接口 / 抽象类
来源：http://skd.sufxvd.cn

Py:   from abc import ABC, abstractmethod
来源：http://rbp.hfpthk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://esh.xingfuxueyuan.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://nhh.yongpay.top

TS:   interface Shape { area(): number; }
来源：http://qht.hammf.cn

Java: interface Shape { double area(); }
来源：http://yfi.ydjk.org.cn

Go:   type Shape interface { Area() float64 }
来源：http://ogc.bjfxy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oca.birdmap.top

C#:   interface IShape { double Area(); }
来源：http://pza.ydzc1.top

[G10] 访问控制
来源：http://ytp.xylfe.cn

Py:   约定 _protected / __private（不强制）
来源：http://kgy.nanxinkj.top

PHP:  public / protected / private
来源：http://xru.ctjpmb.com

JS:   #private 字段；其余公开
来源：http://smh.fzhhl.top

TS:   public / protected / private
来源：http://cyg.sysykeji.top

Java: public / protected / private / 默认包级
来源：http://rdd.zhijiandao.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vaq.fengsongda.top

Ruby: public / protected / private
来源：http://bzk.dashuyun.cn

C#:   public / protected / private / internal
来源：http://ntk.sysykeji.top

[G11] getter / setter
来源：http://qsv.hnqzz.top

Py:   @property 与 @x.setter
来源：http://mli.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cns.yj20258.top

JS:   get name() { return this._name; }
来源：http://fat.bbcook.cn

TS:   get name(): string { return this._name; }
来源：http://oze.gotoacloud.top

Java: public String getName() { return name; }
来源：http://pkt.jqgufenzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gyu.sxryk.cn

Ruby: attr_accessor :name
来源：http://kbi.hysaishi.cn

C#:   public string Name { get; set; }
来源：http://rim.ppjwa.cn

[G12] 对象转字符串
来源：http://sjk.hnxiangtu.top

Py:   def __str__(self): return self.name
来源：http://vii.chenjidiqi.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://pwf.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://mth.zhiwuduotai.top

TS:   toString(): string { return this.name; }
来源：http://jtn.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://pvw.sufxvd.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qpb.0kj1m.cn

Ruby: def to_s; @name; end
来源：http://zyh.cheryme.top

C#:   public override string ToString() => Name;
来源：http://nam.iojbl.cn

[G13] 判断对象类型
来源：http://aid.zhijiandao.cn

Py:   isinstance(u, User)
来源：http://ori.fktsv.cn

PHP:  $u instanceof User
来源：http://wpc.vqdsnc.cn

JS:   u instanceof User
来源：http://boi.chenjidiqi.icu

TS:   u instanceof User
来源：http://krr.xziqi.cn

Java: u instanceof User
来源：http://njr.sufxvd.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://osc.svipenyu.cn

Ruby: u.is_a?(User)
来源：http://bqc.sjlbkw.cn

C#:   u is User
来源：http://lcq.zhijiandao.cn

[G14] 数据类 / record
来源：http://kvm.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aaw.cheryme.top

PHP:  // 用 readonly 属性模拟
来源：http://hmu.yuxming.cn

JS:   // 无内置：普通类或对象字面量
来源：http://paz.jlsjyb.cn

TS:   type User = { name: string; age: number };
来源：http://puf.gotoacloud.top

Java: record User(String name, int age) {}
来源：http://slv.sweek.top

Go:   type User struct { Name string; Age int }
来源：http://ynn.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lbh.nanxinkj.top

C#:   record User(string Name, int Age);
来源：http://jbl.pycfn.com

[G15] 枚举
来源：http://xyi.zhixingplan.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mzt.smart0.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://jtk.hesvh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lww.bbcook.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ukd.yonumen.top

Java: enum Color { RED, GREEN }
来源：http://bim.gotoacloud.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xhp.epnwcf.com

Ruby: Color = %i[red green].freeze
来源：http://fnd.jianghu66.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kuh.yj20258.top

[G16] 对象转数组 / 字典
来源：http://dsa.vehdjk.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qch.chenjidiqi.icu

PHP:  get_object_vars($obj);
来源：http://rck.daria6918.cn

JS:   Object.entries(obj)
来源：http://myc.bbcook.cn

TS:   Object.entries(obj)
来源：http://vkz.xziqi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jvr.cqqwz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mwq.sxryk.cn

Ruby: obj.instance_variables
来源：http://lxw.jqgufenzy.top

C#:   // 用反射或 System.Text.Json
来源：http://rql.zhaomingkeji.xyz

================================================================================
来源：http://zpo.zhixingplan.top

H. 异常与错误处理
来源：http://ned.tarul.cn

================================================================================
来源：http://nga.shangyingyoupin.top

[H01] try / catch 基础
来源：http://axn.redwolf501.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sdp.gotoacloud.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://smv.havefunace.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ewl.sweek.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wez.chenjidiqi.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vyp.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://awp.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wtm.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pzg.uphjek.com

[H02] finally / ensure 收尾
来源：http://mtq.jinyuanbaomall.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iwx.daxiang520.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vvi.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ehd.jqgufenzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mmt.yuanzhike.top

Java: try { f(); } finally { cleanup(); }
来源：http://giy.uphjek.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://qms.aibaodan.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kay.gogol.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bnp.dashuyun.cn

[H03] 主动抛出异常
来源：http://mbu.andypj.xyz

Py:   raise ValueError("错误信息")
来源：http://zdm.ppjwa.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ftu.shanyushiyangtech.top

JS:   throw new Error("错误信息");
来源：http://rtr.haohaochexian.top

TS:   throw new Error("错误信息");
来源：http://ezx.kuanghao11.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nxh.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://epo.jinghuilouyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mye.vehdjk.com

C#:   throw new ArgumentException("错误信息");
来源：http://hvp.ehwqpu.com

[H04] 自定义异常类型
来源：http://elx.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://abe.sxryk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jgd.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://ebx.cashguo.top

TS:   class MyError extends Error {}
来源：http://ypi.kuanghao11.cn

Java: class MyException extends RuntimeException {}
来源：http://uhx.yvedp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bie.zhaomingkeji.xyz

Ruby: class MyError < StandardError; end
来源：http://nzd.zhiwuduotai.top

C#:   class MyException : Exception {}
来源：http://ffa.sufxvd.cn

[H05] 捕获特定类型
来源：http://yzl.yj202588.top

Py:   except ValueError as e:
来源：http://paw.xingfuxueyuan.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kwy.wangdashe.top

JS:   if (e instanceof TypeError) {}
来源：http://jnm.yvedp.cn

TS:   if (e instanceof TypeError) {}
来源：http://gse.fengsongda.top

Java: catch (IOException | SQLException e) {}
来源：http://lqk.shuidangran.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hil.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://ljw.hcnkem.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vki.ywan-chungtsiang.top

[H06] 可选值 / 空值安全访问
来源：http://kkt.zhengqikj.top

Py:   value = d.get("k") or default
来源：http://nqn.jqgufenzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://yhd.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://ias.cqqwz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lrd.yvedp.cn


<!-- 参考信息 -->