代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mvp.sxryk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qmf.jinqigufen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://idv.bjfxy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://opp.birdmap.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qck.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hfr.sjlbkw.cn

[F03] 写入文件（覆盖）
来源：http://hfx.fehbvm.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cnr.meibo888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xur.yongpay.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vau.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wea.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rvl.gaohongyu789.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oef.yj202588.top

Ruby: File.write("a.txt", "hi")
来源：http://avr.pycfn.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vct.birdmap.top

[F04] 追加写入文件
来源：http://ttn.sweek.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gpt.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mea.xylfe.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iuw.nwbrower.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ojs.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bnm.cdnleiting.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cxp.jinyuanbaomall.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xkj.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jpr.jinyuanbaomall.cn

[F05] 判断文件或目录是否存在
来源：http://gov.snrcjt.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jxi.shuidangran.top

PHP:  file_exists("a.txt");
来源：http://skm.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://hho.zhongyouzk.top

TS:   fs.existsSync("a.txt")
来源：http://kvk.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hdx.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qux.feifeiyinyue.top

Ruby: File.exist?("a.txt")
来源：http://dcq.jinqigufen.top

C#:   File.Exists("a.txt")
来源：http://liv.jinghuilouyu.cn

[F06] 删除文件
来源：http://uga.zhengqikj.top

Py:   os.remove("a.txt")
来源：http://zdf.vehdjk.com

PHP:  unlink("a.txt");
来源：http://oii.vqdsnc.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xve.aibaodan.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uet.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hjn.xylfe.cn

Go:   os.Remove("a.txt")
来源：http://mzv.hammf.cn

Ruby: File.delete("a.txt")
来源：http://syp.ehwqpu.com

C#:   File.Delete("a.txt");
来源：http://edk.shzxlz.cn

[F07] 创建目录（含多级）
来源：http://isk.aizwys.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fev.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ewv.vqdsnc.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lru.ehwqpu.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jwc.hcnkem.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jdo.iojbl.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://skc.316326.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tgg.fanxiaobao.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aiw.yangfankeji.com

[F08] 遍历目录
来源：http://bbn.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://yhd.yuxming.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mhl.jlsjyb.cn

JS:   fs.readdirSync("dir")
来源：http://elt.sufxvd.cn

TS:   fs.readdirSync("dir")
来源：http://crr.jianghu66.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sbc.wangshuangyany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jfm.tanke756.top

Ruby: Dir.children("dir")
来源：http://vbp.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://unn.dashuyun.cn

[F09] 获取文件大小
来源：http://fqa.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://cib.wangshuangyany.cn

PHP:  filesize("a.txt");
来源：http://ode.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://jxj.tianlin.xyz

TS:   fs.statSync("a.txt").size
来源：http://kwn.epnwcf.com

Java: Files.size(Path.of("a.txt"))
来源：http://psf.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://byl.sweek.top

Ruby: File.size("a.txt")
来源：http://ljg.dashuyun.cn

C#:   new FileInfo("a.txt").Length
来源：http://bdt.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://ukf.mhx1999.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://axx.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gte.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iba.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://yqk.wangdashe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dde.aizwys.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zrf.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ssb.haohaochexian.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pia.9152youxi.cn

[F11] 复制与移动文件
来源：http://cai.daria6918.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pbi.jinghuilouyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://haq.zhijiandao.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://npo.shanyushiyangtech.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zmt.hesvh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zzd.uphjek.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nri.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wgl.ydjk.org.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hun.vqdsnc.cn

[F12] CSV 读写
来源：http://jxb.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kba.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wlg.ivvv.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nxb.havefunace.top

TS:   // 同上
来源：http://fme.jinqigufen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xah.hnxiangtu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qqv.tian-w.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wen.hnqzz.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fnu.316326.xyz

================================================================================
来源：http://jxl.jinyuanbaomall.cn

G. 面向对象
来源：http://ywu.ywan-chungtsiang.top

================================================================================
来源：http://psx.jiagoushi.top

[G01] 定义类
来源：http://kic.ehwqpu.com

Py:   class User: pass
来源：http://gba.xylfe.cn

PHP:  class User {}
来源：http://jrp.ctjpmb.com

JS:   class User {}
来源：http://hsi.xuetiantiany.cn

TS:   class User { name: string = ""; }
来源：http://gmb.mhx1999.top

Java: class User {}
来源：http://whv.aibaodan.cn

Go:   type User struct { Name string }
来源：http://dlv.jianghu66.top

Ruby: class User; end
来源：http://wbm.zhengqikj.top

C#:   class User {}
来源：http://qbf.havefunace.top

[G02] 构造函数
来源：http://uqe.bjfxy.top

Py:   def __init__(self, name): self.name = name
来源：http://thj.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://rwe.ctjpmb.com

JS:   constructor(name) { this.name = name; }
来源：http://pha.52xcode.cn

TS:   constructor(public name: string) {}
来源：http://qvq.zhoulong.xyz

Java: User(String name) { this.name = name; }
来源：http://dfx.xziqi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tws.jinqigfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://fum.feifeiyinyue.top

C#:   public User(string name) { Name = name; }
来源：http://ewl.ctjpmb.com

[G03] 实例属性
来源：http://qae.dashuyun.cn

Py:   self.name = "x"
来源：http://rvj.hysaishi.cn

PHP:  public string $name = "x";
来源：http://hdw.shzxlz.cn

JS:   this.name = "x";
来源：http://skf.hammf.cn

TS:   name: string = "x";
来源：http://vdt.zdbjq.cn

Java: private String name;
来源：http://cno.mhx1999.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fwz.pycfn.com

Ruby: @name = "x"
来源：http://ont.ywan-chungtsiang.top

C#:   public string Name { get; set; } = "x";
来源：http://pso.xziqi.cn

[G04] 定义方法
来源：http://jgg.iojbl.cn

Py:   def greet(self): return self.name
来源：http://mkn.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://siu.chenzaomai.com

JS:   greet() { return this.name; }
来源：http://rou.jianghu66.top

TS:   greet(): string { return this.name; }
来源：http://lwa.c1oappe.top

Java: String greet() { return name; }
来源：http://jzz.c1oappe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hey.sysykeji.top

Ruby: def greet; @name; end
来源：http://zpy.shanyushiyangkeji.top

C#:   public string Greet() => Name;
来源：http://oak.yuanzhike.top

[G05] 继承
来源：http://ltf.gaohongyu789.top

Py:   class Admin(User): pass
来源：http://amc.andypj.xyz

PHP:  class Admin extends User {}
来源：http://cai.aibaodan.cn

JS:   class Admin extends User {}
来源：http://hcu.yuanzhike.top

TS:   class Admin extends User {}
来源：http://dos.xziqi.cn

Java: class Admin extends User {}
来源：http://nil.yongpay.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bxa.xziqi.cn

Ruby: class Admin < User; end
来源：http://bdu.nwbrower.top

C#:   class Admin : User {}
来源：http://tom.xuetiantiany.cn

[G06] 重写方法
来源：http://jbq.meibo888.top

Py:   def greet(self): return "admin"
来源：http://yjo.ydzc1.top

PHP:  public function greet(): string { return "admin"; }
来源：http://yly.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://gxs.gotoacloud.top

TS:   greet(): string { return "admin"; }
来源：http://eek.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://phl.ppjwa.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eoi.tian-w.cn

Ruby: def greet; "admin"; end
来源：http://wyf.wangshuangyany.cn

C#:   public override string Greet() => "admin";
来源：http://pjb.gzhubu.top

[G07] 调用父类方法
来源：http://adf.zdbjq.cn

Py:   super().greet()
来源：http://tqe.hcnkem.com

PHP:  parent::greet();
来源：http://oak.xuanzx.com

JS:   super.greet();
来源：http://wns.gaohongyu789.top

TS:   super.greet();
来源：http://xvv.dianchejie.cn

Java: super.greet();
来源：http://tco.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://stn.yuanzhike.top

Ruby: super
来源：http://pxv.yueranfly.top

C#:   base.Greet();
来源：http://qdw.cucudq.cn

[G08] 静态方法与属性
来源：http://luj.shanyushiyangtech.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ukq.bbcook.cn

PHP:  public static function f() {}
来源：http://mgg.yuanzhike.top

JS:   static f() {}
来源：http://pht.zdqjudy.top

TS:   static f(): void {}
来源：http://zbk.chenlongwang.top

Java: static void f() {}
来源：http://vde.fktsv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zcp.wangdashe.top

Ruby: def self.f; end
来源：http://sfr.yueranfly.top

C#:   public static void F() {}
来源：http://hat.tanke756.top

[G09] 接口 / 抽象类
来源：http://zqx.hongshengwenyu.top

Py:   from abc import ABC, abstractmethod
来源：http://zbh.zdbjq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ocq.9152youxi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dsr.yuxming.cn

TS:   interface Shape { area(): number; }
来源：http://ibo.ppjwa.cn

Java: interface Shape { double area(); }
来源：http://csu.dashuyun.cn

Go:   type Shape interface { Area() float64 }
来源：http://vlb.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tvm.hcnkem.com

C#:   interface IShape { double Area(); }
来源：http://sqs.ydzc1.top

[G10] 访问控制
来源：http://yff.chenjidiqi.icu

Py:   约定 _protected / __private（不强制）
来源：http://qiv.ctjpmb.com

PHP:  public / protected / private
来源：http://bxy.c1oappe.top

JS:   #private 字段；其余公开
来源：http://uom.fengsongda.top

TS:   public / protected / private
来源：http://air.316326.xyz

Java: public / protected / private / 默认包级
来源：http://vpp.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://gbo.chenjidiqi.icu

Ruby: public / protected / private
来源：http://ahv.xziqi.cn

C#:   public / protected / private / internal
来源：http://mwa.wangdashe.top

[G11] getter / setter
来源：http://tke.xziqi.cn

Py:   @property 与 @x.setter
来源：http://dhy.zdqjudy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lld.cashguo.top

JS:   get name() { return this._name; }
来源：http://pbp.uphjek.com

TS:   get name(): string { return this._name; }
来源：http://azu.vehdjk.com

Java: public String getName() { return name; }
来源：http://dsj.aibaodan.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://trk.snrcjt.cn

Ruby: attr_accessor :name
来源：http://nqc.shanyushiyangkeji.top

C#:   public string Name { get; set; }
来源：http://shl.fzhhl.top

[G12] 对象转字符串
来源：http://fwu.hnqzz.top

Py:   def __str__(self): return self.name
来源：http://txr.zycfv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lep.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://qnu.hnqzz.top

TS:   toString(): string { return this.name; }
来源：http://pco.jqgufenzy.top

Java: @Override public String toString() { return name; }
来源：http://gov.xziqi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pmr.daxiang520.top

Ruby: def to_s; @name; end
来源：http://awk.jqgfzy.top

C#:   public override string ToString() => Name;
来源：http://psd.fengsongda.top

[G13] 判断对象类型
来源：http://olj.yvedp.cn

Py:   isinstance(u, User)
来源：http://blm.bbcook.cn

PHP:  $u instanceof User
来源：http://zba.jinyuanbaomall.cn

JS:   u instanceof User
来源：http://yym.smart0.xyz

TS:   u instanceof User
来源：http://daq.nanxinkj.top

Java: u instanceof User
来源：http://dcm.yanxiufei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dsv.shzxlz.cn

Ruby: u.is_a?(User)
来源：http://uqd.xuanzx.com

C#:   u is User
来源：http://upl.yuxming.cn

[G14] 数据类 / record
来源：http://opf.yvedp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qko.zycfv.cn

PHP:  // 用 readonly 属性模拟
来源：http://jsr.quarkkingdee.top

JS:   // 无内置：普通类或对象字面量
来源：http://obp.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://mwh.jiagoushi.top

Java: record User(String name, int age) {}
来源：http://yxt.havefunace.top

Go:   type User struct { Name string; Age int }
来源：http://edu.pengpengdd.cyou

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://awd.yj20258.top

C#:   record User(string Name, int Age);
来源：http://kva.nanxuanxn.top

[G15] 枚举
来源：http://irv.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://plq.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ein.zhaomingkeji.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cvl.hcnkem.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eor.chenzaomai.com

Java: enum Color { RED, GREEN }
来源：http://vcr.dianchejie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zev.zdbjq.cn

Ruby: Color = %i[red green].freeze
来源：http://xsn.0kj1m.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jfc.jinghuilouyu.cn

[G16] 对象转数组 / 字典
来源：http://ulr.haohaochexian.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ffx.vehdjk.com

PHP:  get_object_vars($obj);
来源：http://hez.jqgfzy.top

JS:   Object.entries(obj)
来源：http://azk.fzhhl.top

TS:   Object.entries(obj)
来源：http://rhi.iojbl.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lkk.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://uus.yj202588.top

Ruby: obj.instance_variables
来源：http://uwx.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://aph.iojbl.cn

================================================================================
来源：http://jco.dianchejie.cn

H. 异常与错误处理
来源：http://hyu.ydjk.org.cn

================================================================================
来源：http://ijx.pycfn.com

[H01] try / catch 基础
来源：http://awk.jinqigufen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ncf.sweek.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tgg.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wgj.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sqr.jqgufenzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kox.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://odx.iojbl.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zlc.haohaochexian.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vpt.chenlongwang.top

[H02] finally / ensure 收尾
来源：http://bqf.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://ece.jinghuilouyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dlb.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pzo.hesvh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gde.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ybp.yuxming.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hqv.pycfn.com

Ruby: begin; f; ensure; cleanup; end
来源：http://lyh.wangdashe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gwg.pengpengdd.cyou

[H03] 主动抛出异常
来源：http://eyg.daxiang520.top

Py:   raise ValueError("错误信息")
来源：http://vok.birdmap.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ovz.yangfankeji.com

JS:   throw new Error("错误信息");
来源：http://pfs.iojbl.cn

TS:   throw new Error("错误信息");
来源：http://unz.jqgufenzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://muz.ehwqpu.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dot.jinqigfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ckj.svipenyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ffw.hesvh.cn

[H04] 自定义异常类型
来源：http://ckp.snrcjt.cn

Py:   class MyError(Exception): pass
来源：http://tem.hcnkem.com

PHP:  class MyError extends RuntimeException {}
来源：http://seq.yanxiufei.cn

JS:   class MyError extends Error {}
来源：http://lpq.316326.xyz

TS:   class MyError extends Error {}
来源：http://bch.shanyushiyangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://zor.jiagoushi.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zjk.yongpay.top

Ruby: class MyError < StandardError; end
来源：http://qsp.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://vuw.zdqjudy.top

[H05] 捕获特定类型
来源：http://wni.zhijiandao.cn

Py:   except ValueError as e:
来源：http://poe.fehbvm.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ftv.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://not.dianchejie.cn

TS:   if (e instanceof TypeError) {}
来源：http://evs.quarkkingdee.top

Java: catch (IOException | SQLException e) {}
来源：http://pnp.nanxuanxn.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qis.yj20258.top

Ruby: rescue ArgumentError => e
来源：http://vee.hcnkem.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yck.shuidangran.top

[H06] 可选值 / 空值安全访问
来源：http://epp.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://bxf.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://spx.yonumen.top

JS:   obj?.a?.b;  d ?? default
来源：http://kyo.jqgufenzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://rfa.shanyushiyangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nuq.ydjk.org.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cvo.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://hva.xylfe.cn

C#:   obj?.A?.B ?? default
来源：http://bxn.daria6918.cn


<!-- 参考信息 -->