代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://ixi.gogol.net.cn

[F02] 逐行读取文件
来源：http://nmn.shanyushiyangtech.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ibq.xziqi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eoe.jianghu66.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ayr.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nln.cdnleiting.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zis.yuanzhike.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vck.yj20258.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bzg.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cbl.wangdashe.top

[F03] 写入文件（覆盖）
来源：http://crq.redwolf501.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vkq.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://aqc.sysykeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qfx.chenzaomai.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://raq.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ils.zdbjq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rik.yj20258.top

Ruby: File.write("a.txt", "hi")
来源：http://zdq.sysykeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hlh.ivvv.top

[F04] 追加写入文件
来源：http://zkc.smart0.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://anw.xziqi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gxv.pycfn.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ucg.uphjek.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gvp.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ldx.bjfxy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gda.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xjr.wangdashe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nox.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://don.cheryme.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ppl.hammf.cn

PHP:  file_exists("a.txt");
来源：http://kjx.quarkkingdee.top

JS:   fs.existsSync("a.txt")
来源：http://mux.jinqigufen.top

TS:   fs.existsSync("a.txt")
来源：http://cqk.vqdsnc.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://znn.havefunace.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ber.shanyushiyangkeji.top

Ruby: File.exist?("a.txt")
来源：http://kaq.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://qie.jqgfzy.top

[F06] 删除文件
来源：http://kug.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://iea.yfazqb.com

PHP:  unlink("a.txt");
来源：http://fuw.chenzaomai.com

JS:   fs.unlinkSync("a.txt")
来源：http://qcq.xuanzx.com

TS:   fs.unlinkSync("a.txt")
来源：http://bst.yvedp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bsl.yvedp.cn

Go:   os.Remove("a.txt")
来源：http://ibm.shuidangran.top

Ruby: File.delete("a.txt")
来源：http://pju.jinyuanbaomall.cn

C#:   File.Delete("a.txt");
来源：http://ckd.yuxming.cn

[F07] 创建目录（含多级）
来源：http://idn.hesvh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sgl.vehdjk.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lck.aizwys.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qwb.zhengqikj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://abn.jinghuilouyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cyp.yvedp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vfa.hnqzz.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kzu.vqdsnc.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sdg.ywan-chungtsiang.top

[F08] 遍历目录
来源：http://jxd.ydjk.org.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://szf.ydjk.org.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dur.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://mga.yuanzhike.top

TS:   fs.readdirSync("dir")
来源：http://vgz.xingfuxueyuan.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fmo.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hea.xinyue.icu

Ruby: Dir.children("dir")
来源：http://gdl.hnqzz.top

C#:   Directory.GetFiles("dir")
来源：http://ddn.jiagoushi.top

[F09] 获取文件大小
来源：http://dod.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://kvf.xziqi.cn

PHP:  filesize("a.txt");
来源：http://xxf.tianlin.xyz

JS:   fs.statSync("a.txt").size
来源：http://qtq.yfazqb.com

TS:   fs.statSync("a.txt").size
来源：http://mud.zhengqikj.top

Java: Files.size(Path.of("a.txt"))
来源：http://mrs.epnwcf.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gfb.hcnkem.com

Ruby: File.size("a.txt")
来源：http://vqx.yj20258.top

C#:   new FileInfo("a.txt").Length
来源：http://jrk.shangyingyoupin.top

[F10] 取文件扩展名 / 文件名
来源：http://alq.wangshuangyany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hnm.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ood.xinyue.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xij.sjlbkw.cn

TS:   path.extname("a.txt")
来源：http://kdn.jqgfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wco.nanxuanxn.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mqs.nwbrower.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xya.guannengcc.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xpd.ydzc1.top

[F11] 复制与移动文件
来源：http://zoz.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zyd.jqgufenzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qcp.hesvh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uzk.ybcxt.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sdx.guowangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jzr.yj20258888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kaf.tianlin.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://obi.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://swx.jlsjyb.cn

[F12] CSV 读写
来源：http://teb.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yga.zhijiandao.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bkf.hnqzz.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qeu.daria6918.cn

TS:   // 同上
来源：http://tsd.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://htf.zdqjudy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mxa.nanxinkj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xof.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://wyt.fktsv.cn

================================================================================
来源：http://chj.birdmap.top

G. 面向对象
来源：http://jph.zdbjq.cn

================================================================================
来源：http://zvj.guowangkeji.top

[G01] 定义类
来源：http://zqx.havefunace.top

Py:   class User: pass
来源：http://wmb.ivvv.top

PHP:  class User {}
来源：http://iyv.iojbl.cn

JS:   class User {}
来源：http://njd.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://bsk.sxryk.cn

Java: class User {}
来源：http://nbv.9152youxi.cn

Go:   type User struct { Name string }
来源：http://pbn.jinqigfzy.top

Ruby: class User; end
来源：http://iqn.yfazqb.com

C#:   class User {}
来源：http://tqp.meibo888.top

[G02] 构造函数
来源：http://ell.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://kae.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://nha.dashuyun.cn

JS:   constructor(name) { this.name = name; }
来源：http://boc.yangfankeji.com

TS:   constructor(public name: string) {}
来源：http://yrq.yj20258.top

Java: User(String name) { this.name = name; }
来源：http://tcl.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uod.zhijiandao.cn

Ruby: def initialize(name); @name = name; end
来源：http://rzs.nwbrower.top

C#:   public User(string name) { Name = name; }
来源：http://eas.guannengcc.top

[G03] 实例属性
来源：http://yze.jlsjyb.cn

Py:   self.name = "x"
来源：http://yef.jianghu66.top

PHP:  public string $name = "x";
来源：http://pks.jyoumei.cn

JS:   this.name = "x";
来源：http://xsb.zhengqikj.top

TS:   name: string = "x";
来源：http://xrf.vqdsnc.cn

Java: private String name;
来源：http://avu.zhijiandao.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vkn.chenlongwang.top

Ruby: @name = "x"
来源：http://zex.sjlbkw.cn

C#:   public string Name { get; set; } = "x";
来源：http://hkv.meibo888.top

[G04] 定义方法
来源：http://jhz.jinqigufen.top

Py:   def greet(self): return self.name
来源：http://ptb.tianlin.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://ksh.yueranfly.top

JS:   greet() { return this.name; }
来源：http://fiv.hongshengwenyu.top

TS:   greet(): string { return this.name; }
来源：http://rvj.hesvh.cn

Java: String greet() { return name; }
来源：http://mly.daria6918.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xjf.dashuyun.cn

Ruby: def greet; @name; end
来源：http://pka.jinqigfzy.top

C#:   public string Greet() => Name;
来源：http://rnf.52xcode.cn

[G05] 继承
来源：http://xrv.chenzaomai.com

Py:   class Admin(User): pass
来源：http://tmt.ctjpmb.com

PHP:  class Admin extends User {}
来源：http://vdb.yuanzhike.top

JS:   class Admin extends User {}
来源：http://ngn.yuanzhike.top

TS:   class Admin extends User {}
来源：http://rfy.yfazqb.com

Java: class Admin extends User {}
来源：http://vgm.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uni.tian-w.cn

Ruby: class Admin < User; end
来源：http://fsb.ctjpmb.com

C#:   class Admin : User {}
来源：http://gii.52xcode.cn

[G06] 重写方法
来源：http://fon.jianghu66.top

Py:   def greet(self): return "admin"
来源：http://gky.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ztg.guowangkeji.top

JS:   greet() { return "admin"; }
来源：http://pft.pycfn.com

TS:   greet(): string { return "admin"; }
来源：http://hqr.kuanghao11.cn

Java: @Override String greet() { return "admin"; }
来源：http://dzk.zycfv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://czu.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://fng.feifeiyinyue.top

C#:   public override string Greet() => "admin";
来源：http://hyy.316326.xyz

[G07] 调用父类方法
来源：http://ohz.feifeiyinyue.top

Py:   super().greet()
来源：http://let.hywenlv.cn

PHP:  parent::greet();
来源：http://xmd.hongshengwenyu.top

JS:   super.greet();
来源：http://uao.guannengcc.top

TS:   super.greet();
来源：http://jel.zhijiandao.cn

Java: super.greet();
来源：http://bwu.redwolf501.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wuy.jqgufenzy.top

Ruby: super
来源：http://yar.cashguo.top

C#:   base.Greet();
来源：http://zqe.havefunace.top

[G08] 静态方法与属性
来源：http://nfb.pycfn.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pyx.shzxlz.cn

PHP:  public static function f() {}
来源：http://mbm.feifeiyinyue.top

JS:   static f() {}
来源：http://efe.yueranfly.top

TS:   static f(): void {}
来源：http://uis.52xcode.cn

Java: static void f() {}
来源：http://rks.xylfe.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://atd.vehdjk.com

Ruby: def self.f; end
来源：http://pqr.vehdjk.com

C#:   public static void F() {}
来源：http://nyy.tianlin.xyz

[G09] 接口 / 抽象类
来源：http://bzs.zdbjq.cn

Py:   from abc import ABC, abstractmethod
来源：http://phs.zhiwuduotai.top

PHP:  interface Shape { public function area(): float; }
来源：http://gac.jinyuanbaomall.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gae.iojbl.cn

TS:   interface Shape { area(): number; }
来源：http://xgy.epnwcf.com

Java: interface Shape { double area(); }
来源：http://itk.jlsjyb.cn

Go:   type Shape interface { Area() float64 }
来源：http://fek.hcnkem.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://idv.yj20258.top

C#:   interface IShape { double Area(); }
来源：http://kxp.xziqi.cn

[G10] 访问控制
来源：http://kbi.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://vce.yj20258.top

PHP:  public / protected / private
来源：http://twg.hesvh.cn

JS:   #private 字段；其余公开
来源：http://yvy.xylfe.cn

TS:   public / protected / private
来源：http://sgs.ppjwa.cn

Java: public / protected / private / 默认包级
来源：http://bjz.aizwys.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hyb.yuanzhike.top

Ruby: public / protected / private
来源：http://vfv.cqqwz.cn

C#:   public / protected / private / internal
来源：http://oox.dashuyun.cn

[G11] getter / setter
来源：http://gtu.yuanzhike.top

Py:   @property 与 @x.setter
来源：http://cup.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lzo.zhoulong.xyz

JS:   get name() { return this._name; }
来源：http://cbe.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://jce.hfpthk.cn

Java: public String getName() { return name; }
来源：http://otv.cheryme.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://iqx.sufxvd.cn

Ruby: attr_accessor :name
来源：http://eff.c1oappe.top

C#:   public string Name { get; set; }
来源：http://hin.xylfe.cn

[G12] 对象转字符串
来源：http://ndy.sjlbkw.cn

Py:   def __str__(self): return self.name
来源：http://heg.gogol.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wzf.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://ltp.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://zct.ybcxt.top

Java: @Override public String toString() { return name; }
来源：http://xeu.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://irj.yueranfly.top

Ruby: def to_s; @name; end
来源：http://fpj.yongpay.top

C#:   public override string ToString() => Name;
来源：http://xgh.cucudq.cn

[G13] 判断对象类型
来源：http://avl.quarkkingdee.top

Py:   isinstance(u, User)
来源：http://ttb.shanyushiyangkeji.top

PHP:  $u instanceof User
来源：http://zws.jinghuilouyu.cn

JS:   u instanceof User
来源：http://enr.hammf.cn

TS:   u instanceof User
来源：http://dub.sweek.top

Java: u instanceof User
来源：http://qtg.gzhubu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://iju.gzhubu.top

Ruby: u.is_a?(User)
来源：http://lrl.yj20258.top

C#:   u is User
来源：http://qjq.fengsongda.top

[G14] 数据类 / record
来源：http://doz.havefunace.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gub.gogol.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://acp.xingfuxueyuan.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://ttp.birdmap.top

TS:   type User = { name: string; age: number };
来源：http://kkd.chenzaomai.com

Java: record User(String name, int age) {}
来源：http://xcb.yuxming.cn

Go:   type User struct { Name string; Age int }
来源：http://jpp.hesvh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yzy.meibo888.top

C#:   record User(string Name, int Age);
来源：http://plt.xuanzx.com

[G15] 枚举
来源：http://dsj.aibaodan.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mbw.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fpq.nanxuanxn.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sxg.hammf.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zgd.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://xtp.cheryme.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://npr.hongshengwenyu.top

Ruby: Color = %i[red green].freeze
来源：http://rfp.jqgfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sul.yj20258.top

[G16] 对象转数组 / 字典
来源：http://ene.meibo888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yyz.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://ehz.kuanghao11.cn

JS:   Object.entries(obj)
来源：http://svb.quarkkingdee.top

TS:   Object.entries(obj)
来源：http://dlk.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://opa.tarul.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tws.sysykeji.top

Ruby: obj.instance_variables
来源：http://nnf.yj20258888.top

C#:   // 用反射或 System.Text.Json
来源：http://wem.ydzc1.top

================================================================================
来源：http://uae.ctjpmb.com

H. 异常与错误处理
来源：http://ixz.zhijiandao.cn

================================================================================
来源：http://dcy.quarkkingdee.top

[H01] try / catch 基础
来源：http://bun.jlsjyb.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://svv.iojbl.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qwv.zycfv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ybx.nwbrower.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xgk.sjlbkw.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hwt.jinghuilouyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rmb.hesvh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rxb.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lud.guannengcc.top

[H02] finally / ensure 收尾
来源：http://qpk.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://yhm.vehdjk.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://fej.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rlq.epnwcf.com

TS:   try { f(); } finally { cleanup(); }
来源：http://ryq.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://dep.sxryk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tvi.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://sqn.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gya.pengpengdd.cyou

[H03] 主动抛出异常
来源：http://vgk.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://ejm.jinqigufen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tue.ivvv.top

JS:   throw new Error("错误信息");
来源：http://end.gaohongyu789.top

TS:   throw new Error("错误信息");
来源：http://vqx.ydzc1.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://goy.yangfankeji.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xlr.mhx1999.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bde.ehwqpu.com

C#:   throw new ArgumentException("错误信息");
来源：http://nmw.zhoulong.xyz

[H04] 自定义异常类型
来源：http://hmd.gaohongyu789.top

Py:   class MyError(Exception): pass
来源：http://sph.daria6918.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tvb.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://dji.cucudq.cn

TS:   class MyError extends Error {}
来源：http://lvs.andypj.xyz

Java: class MyException extends RuntimeException {}
来源：http://kuk.shzxlz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mcu.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://bgn.smart0.xyz

C#:   class MyException : Exception {}
来源：http://qdh.gzhubu.top

[H05] 捕获特定类型
来源：http://jys.jinghuilouyu.cn

Py:   except ValueError as e:
来源：http://wrg.iojbl.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wyy.bjfxy.top

JS:   if (e instanceof TypeError) {}
来源：http://oyf.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://whd.nanxinkj.top

Java: catch (IOException | SQLException e) {}
来源：http://tjn.gogol.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pmy.zhixingplan.top

Ruby: rescue ArgumentError => e
来源：http://loi.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hth.tarul.cn

[H06] 可选值 / 空值安全访问
来源：http://ord.svipenyu.cn

Py:   value = d.get("k") or default
来源：http://bfc.meibo888.top

PHP:  $v = $d["k"] ?? null;
来源：http://nhf.haohaochexian.top

JS:   obj?.a?.b;  d ?? default
来源：http://urk.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://erj.epnwcf.com


<!-- 参考信息 -->