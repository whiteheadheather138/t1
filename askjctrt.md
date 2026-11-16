代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jwq.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bpr.52xcode.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kce.xuetiantiany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nul.yongpay.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mgc.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sol.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://dgm.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hjq.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oax.bbcook.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://max.hywenlv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kaj.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aet.yongpay.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yza.hammf.cn

Ruby: File.write("a.txt", "hi")
来源：http://nmt.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wua.yongpay.top

[F04] 追加写入文件
来源：http://dvg.9152youxi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cka.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://egt.bbcook.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hhj.hcnkem.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kfh.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://djb.zhoulong.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sbf.zycfv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iuh.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rcf.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://bds.bjfxy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://waj.uphjek.com

PHP:  file_exists("a.txt");
来源：http://rsc.316326.xyz

JS:   fs.existsSync("a.txt")
来源：http://wdh.jinyuanbaomall.cn

TS:   fs.existsSync("a.txt")
来源：http://mhc.shzxlz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sla.zycfv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tea.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://qby.iojbl.cn

C#:   File.Exists("a.txt")
来源：http://ixb.cucudq.cn

[F06] 删除文件
来源：http://xar.yj202588.top

Py:   os.remove("a.txt")
来源：http://aek.zhaomingkeji.xyz

PHP:  unlink("a.txt");
来源：http://gyj.hesvh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nku.xuanzx.com

TS:   fs.unlinkSync("a.txt")
来源：http://swh.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aoo.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://oii.shanyushiyangkeji.top

Ruby: File.delete("a.txt")
来源：http://xjv.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://bne.yj20258.top

[F07] 创建目录（含多级）
来源：http://tyb.shangyingyoupin.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ltg.daxiang520.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hqw.chenjidiqi.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nzx.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cfm.pycfn.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cjz.svipenyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bhq.haohaochexian.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cmk.snrcjt.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cpr.sufxvd.cn

[F08] 遍历目录
来源：http://gvv.zhiwuduotai.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ckw.shzxlz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eet.0kj1m.cn

JS:   fs.readdirSync("dir")
来源：http://tgx.sysykeji.top

TS:   fs.readdirSync("dir")
来源：http://pao.yuanzhike.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jjy.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nmk.gzhubu.top

Ruby: Dir.children("dir")
来源：http://lva.epnwcf.com

C#:   Directory.GetFiles("dir")
来源：http://ooy.xziqi.cn

[F09] 获取文件大小
来源：http://nvn.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://wxt.shuidangran.top

PHP:  filesize("a.txt");
来源：http://oba.havefunace.top

JS:   fs.statSync("a.txt").size
来源：http://rgd.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://gxj.vqdsnc.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rwp.yanxiufei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nly.sweek.top

Ruby: File.size("a.txt")
来源：http://clj.shangyingyoupin.top

C#:   new FileInfo("a.txt").Length
来源：http://zno.jlsjyb.cn

[F10] 取文件扩展名 / 文件名
来源：http://bqz.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dco.jinqigfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://raf.zhongyouzk.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kvu.gaohongyu789.top

TS:   path.extname("a.txt")
来源：http://muo.fanxiaobao.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hfj.havefunace.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://npy.smart0.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://htj.bjfxy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xyj.nwbrower.top

[F11] 复制与移动文件
来源：http://upv.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ctm.aibaodan.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sbz.hnqzz.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mse.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gcw.yj202588.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gmi.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qkh.nwbrower.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tve.pengpengdd.cyou

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pfi.jqgufenzy.top

[F12] CSV 读写
来源：http://sye.xuetiantiany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cdw.zhengqikj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vwm.mhx1999.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nob.xingfuxueyuan.xyz

TS:   // 同上
来源：http://dza.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qhh.svipenyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://stp.sufxvd.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oww.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rsu.9152youxi.cn

================================================================================
来源：http://cmy.fanxiaobao.xyz

G. 面向对象
来源：http://clm.zhijiandao.cn

================================================================================
来源：http://unf.quarkkingdee.top

[G01] 定义类
来源：http://okz.cheryme.top

Py:   class User: pass
来源：http://hjs.zycfv.cn

PHP:  class User {}
来源：http://kio.epnwcf.com

JS:   class User {}
来源：http://isu.daria6918.cn

TS:   class User { name: string = ""; }
来源：http://yoe.cdnleiting.top

Java: class User {}
来源：http://jce.fengsongda.top

Go:   type User struct { Name string }
来源：http://iqt.fanxiaobao.xyz

Ruby: class User; end
来源：http://jgw.haohaochexian.top

C#:   class User {}
来源：http://vix.svipenyu.cn

[G02] 构造函数
来源：http://est.fengsongda.top

Py:   def __init__(self, name): self.name = name
来源：http://qrf.xinyue.icu

PHP:  public function __construct(public string $name) {}
来源：http://aoi.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://fzg.iojbl.cn

TS:   constructor(public name: string) {}
来源：http://jbx.shuidangran.top

Java: User(String name) { this.name = name; }
来源：http://aas.gzhubu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yww.yj20258.top

Ruby: def initialize(name); @name = name; end
来源：http://mfa.jyoumei.cn

C#:   public User(string name) { Name = name; }
来源：http://jrr.sxryk.cn

[G03] 实例属性
来源：http://cig.shanyushiyangtech.top

Py:   self.name = "x"
来源：http://vup.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://gln.epnwcf.com

JS:   this.name = "x";
来源：http://qra.yangfankeji.com

TS:   name: string = "x";
来源：http://cab.c1oappe.top

Java: private String name;
来源：http://ili.jinghuilouyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yze.9152youxi.cn

Ruby: @name = "x"
来源：http://etk.xingfuxueyuan.xyz

C#:   public string Name { get; set; } = "x";
来源：http://svv.yj20258888.top

[G04] 定义方法
来源：http://vpe.zhiwuduotai.top

Py:   def greet(self): return self.name
来源：http://igj.cucudq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://svg.svipenyu.cn

JS:   greet() { return this.name; }
来源：http://eqh.daria6918.cn

TS:   greet(): string { return this.name; }
来源：http://xju.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://yca.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://inr.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://mpi.wangdashe.top

C#:   public string Greet() => Name;
来源：http://tbg.pycfn.com

[G05] 继承
来源：http://cpz.cheryme.top

Py:   class Admin(User): pass
来源：http://gzr.gogol.net.cn

PHP:  class Admin extends User {}
来源：http://qsk.tianlin.xyz

JS:   class Admin extends User {}
来源：http://vea.jinqigfzy.top

TS:   class Admin extends User {}
来源：http://exg.wangshuangyany.cn

Java: class Admin extends User {}
来源：http://vox.shzxlz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://she.sweek.top

Ruby: class Admin < User; end
来源：http://dhg.vehdjk.com

C#:   class Admin : User {}
来源：http://xzs.pycfn.com

[G06] 重写方法
来源：http://byt.yonumen.top

Py:   def greet(self): return "admin"
来源：http://aod.yj20258.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gnu.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://wpw.hysaishi.cn

TS:   greet(): string { return "admin"; }
来源：http://ptc.zdbjq.cn

Java: @Override String greet() { return "admin"; }
来源：http://nyw.9152youxi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kdt.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://cgi.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://gyt.shanyushiyangtech.top

[G07] 调用父类方法
来源：http://pzb.yfazqb.com

Py:   super().greet()
来源：http://jcg.shzxlz.cn

PHP:  parent::greet();
来源：http://kam.yfazqb.com

JS:   super.greet();
来源：http://jgj.fktsv.cn

TS:   super.greet();
来源：http://rzl.tanke756.top

Java: super.greet();
来源：http://xbd.tian-w.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zfw.zhaomingkeji.xyz

Ruby: super
来源：http://tvj.zhongyouzk.top

C#:   base.Greet();
来源：http://ysa.sysykeji.top

[G08] 静态方法与属性
来源：http://pqp.ydzc1.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://niu.kuanghao11.cn

PHP:  public static function f() {}
来源：http://oph.tarul.cn

JS:   static f() {}
来源：http://fka.jinqigufen.top

TS:   static f(): void {}
来源：http://amk.xinyue.icu

Java: static void f() {}
来源：http://oby.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://iga.sysykeji.top

Ruby: def self.f; end
来源：http://nxy.xuanzx.com

C#:   public static void F() {}
来源：http://epm.aizwys.cn

[G09] 接口 / 抽象类
来源：http://gfk.zhengqikj.top

Py:   from abc import ABC, abstractmethod
来源：http://djb.yuxming.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hys.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kwj.sjlbkw.cn

TS:   interface Shape { area(): number; }
来源：http://seq.haohaochexian.top

Java: interface Shape { double area(); }
来源：http://jdk.kuanghao11.cn

Go:   type Shape interface { Area() float64 }
来源：http://bgi.meibo888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hxm.yonumen.top

C#:   interface IShape { double Area(); }
来源：http://ycx.feifeiyinyue.top

[G10] 访问控制
来源：http://pbw.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://mck.hysaishi.cn

PHP:  public / protected / private
来源：http://msk.9152youxi.cn

JS:   #private 字段；其余公开
来源：http://xgb.hcnkem.com

TS:   public / protected / private
来源：http://jpb.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://akm.c1oappe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fnk.yangfankeji.com

Ruby: public / protected / private
来源：http://oxv.jinyuanbaomall.cn

C#:   public / protected / private / internal
来源：http://nok.gaohongyu789.top

[G11] getter / setter
来源：http://njj.tarul.cn

Py:   @property 与 @x.setter
来源：http://rvs.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dfh.guannengcc.top

JS:   get name() { return this._name; }
来源：http://rlr.quarkkingdee.top

TS:   get name(): string { return this._name; }
来源：http://ezc.chenzaomai.com

Java: public String getName() { return name; }
来源：http://mgv.cucudq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fwo.aibaodan.cn

Ruby: attr_accessor :name
来源：http://bbp.quarkkingdee.top

C#:   public string Name { get; set; }
来源：http://uod.wangdashe.top

[G12] 对象转字符串
来源：http://kfo.yj20258.top

Py:   def __str__(self): return self.name
来源：http://yjk.yangfankeji.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://tkx.yuanzhike.top

JS:   toString() { return this.name; }
来源：http://zwg.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://gia.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://mag.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://uyu.ivvv.top

Ruby: def to_s; @name; end
来源：http://nsp.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://aby.nwbrower.top

[G13] 判断对象类型
来源：http://odl.cucudq.cn

Py:   isinstance(u, User)
来源：http://ntx.pycfn.com

PHP:  $u instanceof User
来源：http://hzm.fengsongda.top

JS:   u instanceof User
来源：http://nsu.wangdashe.top

TS:   u instanceof User
来源：http://sca.feifeiyinyue.top

Java: u instanceof User
来源：http://uyh.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://kfw.52xcode.cn

Ruby: u.is_a?(User)
来源：http://qta.hysaishi.cn

C#:   u is User
来源：http://rrn.cucudq.cn

[G14] 数据类 / record
来源：http://xss.yuxming.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fin.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://riu.cucudq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jgt.vqdsnc.cn

TS:   type User = { name: string; age: number };
来源：http://dmw.guowangkeji.top

Java: record User(String name, int age) {}
来源：http://ano.daria6918.cn

Go:   type User struct { Name string; Age int }
来源：http://njz.fengsongda.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://srk.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://kig.xylfe.cn

[G15] 枚举
来源：http://xad.uphjek.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qhm.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://itv.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://byi.guowangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://stx.zhiwuduotai.top

Java: enum Color { RED, GREEN }
来源：http://peo.sysykeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xyp.wangdashe.top

Ruby: Color = %i[red green].freeze
来源：http://bae.gzhubu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tup.cheryme.top

[G16] 对象转数组 / 字典
来源：http://imt.wangshuangyany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pyl.smart0.xyz

PHP:  get_object_vars($obj);
来源：http://sim.sysykeji.top

JS:   Object.entries(obj)
来源：http://klm.bbcook.cn

TS:   Object.entries(obj)
来源：http://azp.tarul.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ywf.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pwh.zhixingplan.top

Ruby: obj.instance_variables
来源：http://scr.yuanzhike.top

C#:   // 用反射或 System.Text.Json
来源：http://lyv.nwbrower.top

================================================================================
来源：http://xbc.hongshengwenyu.top

H. 异常与错误处理
来源：http://ssx.ctjpmb.com

================================================================================
来源：http://aci.haohaochexian.top

[H01] try / catch 基础
来源：http://csi.xuetiantiany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fxs.ehwqpu.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wgn.chenzaomai.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lkz.nwbrower.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qus.xuetiantiany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vpq.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://maf.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://slu.yfazqb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cjm.yfazqb.com

[H02] finally / ensure 收尾
来源：http://fon.hcnkem.com

Py:   try: f()⏎finally: cleanup()
来源：http://ixu.haohaochexian.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cds.ybcxt.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fnm.bbcook.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zwc.ydzc1.top

Java: try { f(); } finally { cleanup(); }
来源：http://jnm.yj202588.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wgr.ydjk.org.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xke.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://umj.fanxiaobao.xyz

[H03] 主动抛出异常
来源：http://dwt.wangdashe.top

Py:   raise ValueError("错误信息")
来源：http://dql.quarkkingdee.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lmx.wangshuangyany.cn

JS:   throw new Error("错误信息");
来源：http://bpi.ppjwa.cn

TS:   throw new Error("错误信息");
来源：http://ykh.hysaishi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kcd.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zvt.zdbjq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sxh.iojbl.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mox.tian-w.cn

[H04] 自定义异常类型
来源：http://jnc.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://jwt.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://hvv.hfpthk.cn

JS:   class MyError extends Error {}
来源：http://xxs.gzhubu.top

TS:   class MyError extends Error {}
来源：http://flv.jinqigufen.top

Java: class MyException extends RuntimeException {}
来源：http://rxb.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qcs.52xcode.cn

Ruby: class MyError < StandardError; end
来源：http://joz.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://sny.hammf.cn

[H05] 捕获特定类型
来源：http://bgb.fehbvm.com

Py:   except ValueError as e:
来源：http://jbm.gzhubu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mkz.ehwqpu.com

JS:   if (e instanceof TypeError) {}
来源：http://zei.fanxiaobao.xyz

TS:   if (e instanceof TypeError) {}
来源：http://eoa.tanke756.top

Java: catch (IOException | SQLException e) {}
来源：http://wet.hfpthk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nva.sweek.top

Ruby: rescue ArgumentError => e
来源：http://fcx.cucudq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qce.fktsv.cn

[H06] 可选值 / 空值安全访问
来源：http://ooy.cashguo.top

Py:   value = d.get("k") or default
来源：http://feq.vqdsnc.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hyc.guowangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://mbt.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://aus.gaohongyu789.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lpb.hongshengwenyu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://axy.dashuyun.cn

Ruby: d&.dig(:a, :b)
来源：http://sit.dashuyun.cn

C#:   obj?.A?.B ?? default
来源：http://lep.tian-w.cn


<!-- 参考信息 -->