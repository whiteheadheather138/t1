代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://svc.daxiang520.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fjp.jlsjyb.cn

[F03] 写入文件（覆盖）
来源：http://mgw.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hjc.cdnleiting.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zyv.bbcook.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vna.cqqwz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dyh.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rgq.bbcook.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yjg.kuanghao11.cn

Ruby: File.write("a.txt", "hi")
来源：http://pxu.andypj.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fqw.andypj.xyz

[F04] 追加写入文件
来源：http://pfe.jyoumei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ryy.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nmm.nanxuanxn.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uxt.nwbrower.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://grc.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mmn.chenjidiqi.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xhc.ywan-chungtsiang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hnb.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://trd.xuanzx.com

[F05] 判断文件或目录是否存在
来源：http://fbk.nwbrower.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uzu.vqdsnc.cn

PHP:  file_exists("a.txt");
来源：http://lyi.zhoulong.xyz

JS:   fs.existsSync("a.txt")
来源：http://ymz.zdbjq.cn

TS:   fs.existsSync("a.txt")
来源：http://hdb.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ing.sufxvd.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lri.yuxming.cn

Ruby: File.exist?("a.txt")
来源：http://qbs.ivvv.top

C#:   File.Exists("a.txt")
来源：http://jxw.mhx1999.top

[F06] 删除文件
来源：http://qfy.xuanzx.com

Py:   os.remove("a.txt")
来源：http://kpd.andypj.xyz

PHP:  unlink("a.txt");
来源：http://tdk.quarkkingdee.top

JS:   fs.unlinkSync("a.txt")
来源：http://lcy.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bcw.chenzaomai.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bhg.jyoumei.cn

Go:   os.Remove("a.txt")
来源：http://kyb.cdnleiting.top

Ruby: File.delete("a.txt")
来源：http://kzk.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://egx.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://pcg.zhiwuduotai.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tzi.xziqi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yen.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mky.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ahb.redwolf501.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kcm.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uqj.chenzaomai.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yab.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hwb.gotoacloud.top

[F08] 遍历目录
来源：http://dll.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zkq.fzhhl.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mxa.c1oappe.top

JS:   fs.readdirSync("dir")
来源：http://roz.yj20258.top

TS:   fs.readdirSync("dir")
来源：http://mjv.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://neb.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hvk.tarul.cn

Ruby: Dir.children("dir")
来源：http://zwb.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://cnf.yangfankeji.com

[F09] 获取文件大小
来源：http://bbm.shanyushiyangtech.top

Py:   os.path.getsize("a.txt")
来源：http://pjd.ybcxt.top

PHP:  filesize("a.txt");
来源：http://olq.shangyingyoupin.top

JS:   fs.statSync("a.txt").size
来源：http://laj.ivvv.top

TS:   fs.statSync("a.txt").size
来源：http://jwf.zdbjq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hmc.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wfu.jianghu66.top

Ruby: File.size("a.txt")
来源：http://gds.ybcxt.top

C#:   new FileInfo("a.txt").Length
来源：http://rxj.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://srq.meibo888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dbv.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pfd.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hst.jinghuilouyu.cn

TS:   path.extname("a.txt")
来源：http://bxq.smart0.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ctl.tanke756.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xkr.meibo888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wdq.52xcode.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lae.c1oappe.top

[F11] 复制与移动文件
来源：http://qqb.quarkkingdee.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://esf.xinyue.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://atq.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fjf.jiagoushi.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ltk.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mdy.316326.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://duf.vehdjk.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hsa.svipenyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mhx.zhiwuduotai.top

[F12] CSV 读写
来源：http://fut.jinghuilouyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ccx.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://azb.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://klk.gzhubu.top

TS:   // 同上
来源：http://rmd.zhaomingkeji.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cxk.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vtw.ydzc1.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mrc.shzxlz.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zgj.iojbl.cn

================================================================================
来源：http://wnj.tianlin.xyz

G. 面向对象
来源：http://afb.quarkkingdee.top

================================================================================
来源：http://ozm.andypj.xyz

[G01] 定义类
来源：http://nfz.316326.xyz

Py:   class User: pass
来源：http://uqk.yueranfly.top

PHP:  class User {}
来源：http://lnl.cashguo.top

JS:   class User {}
来源：http://cgp.guannengcc.top

TS:   class User { name: string = ""; }
来源：http://eaj.cdnleiting.top

Java: class User {}
来源：http://hyk.quarkkingdee.top

Go:   type User struct { Name string }
来源：http://xrt.hywenlv.cn

Ruby: class User; end
来源：http://kis.fktsv.cn

C#:   class User {}
来源：http://zhl.kuanghao11.cn

[G02] 构造函数
来源：http://vjg.yongpay.top

Py:   def __init__(self, name): self.name = name
来源：http://bah.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://cfy.mhx1999.top

JS:   constructor(name) { this.name = name; }
来源：http://nma.andypj.xyz

TS:   constructor(public name: string) {}
来源：http://yjw.ywan-chungtsiang.top

Java: User(String name) { this.name = name; }
来源：http://jjn.yuanzhike.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xvp.gotoacloud.top

Ruby: def initialize(name); @name = name; end
来源：http://jta.yangfankeji.com

C#:   public User(string name) { Name = name; }
来源：http://bze.ydzc1.top

[G03] 实例属性
来源：http://slw.xylfe.cn

Py:   self.name = "x"
来源：http://ggh.pengpengdd.cyou

PHP:  public string $name = "x";
来源：http://yuk.zhaomingkeji.xyz

JS:   this.name = "x";
来源：http://bys.yuxming.cn

TS:   name: string = "x";
来源：http://ana.52xcode.cn

Java: private String name;
来源：http://xto.9152youxi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ggw.ivvv.top

Ruby: @name = "x"
来源：http://mnt.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://lbg.xylfe.cn

[G04] 定义方法
来源：http://amx.xinyue.icu

Py:   def greet(self): return self.name
来源：http://wft.gaohongyu789.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zts.jinyuanbaomall.cn

JS:   greet() { return this.name; }
来源：http://mmi.zhengqikj.top

TS:   greet(): string { return this.name; }
来源：http://uaw.jianghu66.top

Java: String greet() { return name; }
来源：http://abr.tanke756.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zae.fehbvm.com

Ruby: def greet; @name; end
来源：http://sxr.xylfe.cn

C#:   public string Greet() => Name;
来源：http://rkq.zhoulong.xyz

[G05] 继承
来源：http://ztz.jiagoushi.top

Py:   class Admin(User): pass
来源：http://wxa.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://rch.fengsongda.top

JS:   class Admin extends User {}
来源：http://ifn.aibaodan.cn

TS:   class Admin extends User {}
来源：http://oma.zycfv.cn

Java: class Admin extends User {}
来源：http://sbm.epnwcf.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://udd.shuidangran.top

Ruby: class Admin < User; end
来源：http://lpb.zdbjq.cn

C#:   class Admin : User {}
来源：http://jsf.xuetiantiany.cn

[G06] 重写方法
来源：http://oqv.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://uug.fzhhl.top

PHP:  public function greet(): string { return "admin"; }
来源：http://aqo.dashuyun.cn

JS:   greet() { return "admin"; }
来源：http://khb.nwbrower.top

TS:   greet(): string { return "admin"; }
来源：http://uhl.fanxiaobao.xyz

Java: @Override String greet() { return "admin"; }
来源：http://cdx.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wvq.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://ylf.pengpengdd.cyou

C#:   public override string Greet() => "admin";
来源：http://ehz.sweek.top

[G07] 调用父类方法
来源：http://iwq.redwolf501.top

Py:   super().greet()
来源：http://mna.cdnleiting.top

PHP:  parent::greet();
来源：http://gzj.0kj1m.cn

JS:   super.greet();
来源：http://lps.yanxiufei.cn

TS:   super.greet();
来源：http://amc.aizwys.cn

Java: super.greet();
来源：http://dhd.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vnm.chenlongwang.top

Ruby: super
来源：http://vmz.aizwys.cn

C#:   base.Greet();
来源：http://ugx.yj20258.top

[G08] 静态方法与属性
来源：http://xrk.316326.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fwd.zhiwuduotai.top

PHP:  public static function f() {}
来源：http://eaz.0kj1m.cn

JS:   static f() {}
来源：http://hza.fktsv.cn

TS:   static f(): void {}
来源：http://erj.ybcxt.top

Java: static void f() {}
来源：http://csq.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://exo.yuanzhike.top

Ruby: def self.f; end
来源：http://zqa.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://vzg.shuidangran.top

[G09] 接口 / 抽象类
来源：http://mto.wangshuangyany.cn

Py:   from abc import ABC, abstractmethod
来源：http://oqi.mhx1999.top

PHP:  interface Shape { public function area(): float; }
来源：http://oif.pengpengdd.cyou

JS:   // 无接口：靠约定或 JSDoc
来源：http://ziy.meibo888.top

TS:   interface Shape { area(): number; }
来源：http://sgr.dianchejie.cn

Java: interface Shape { double area(); }
来源：http://qoi.hywenlv.cn

Go:   type Shape interface { Area() float64 }
来源：http://eri.yfazqb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://evn.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://ezr.wangdashe.top

[G10] 访问控制
来源：http://eoc.nanxinkj.top

Py:   约定 _protected / __private（不强制）
来源：http://pwo.gzhubu.top

PHP:  public / protected / private
来源：http://hvd.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://ohf.tianlin.xyz

TS:   public / protected / private
来源：http://shu.zycfv.cn

Java: public / protected / private / 默认包级
来源：http://qcd.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://boo.birdmap.top

Ruby: public / protected / private
来源：http://xsx.pengpengdd.cyou

C#:   public / protected / private / internal
来源：http://gdn.hesvh.cn

[G11] getter / setter
来源：http://azh.chenlongwang.top

Py:   @property 与 @x.setter
来源：http://wpn.xziqi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xbk.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://vce.meibo888.top

TS:   get name(): string { return this._name; }
来源：http://fmm.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://yqd.zhiwuduotai.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://oet.9152youxi.cn

Ruby: attr_accessor :name
来源：http://bqr.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://ndk.bbcook.cn

[G12] 对象转字符串
来源：http://rde.fanxiaobao.xyz

Py:   def __str__(self): return self.name
来源：http://vor.zhijiandao.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wmj.hcnkem.com

JS:   toString() { return this.name; }
来源：http://dsp.fengsongda.top

TS:   toString(): string { return this.name; }
来源：http://fjb.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://xqo.iojbl.cn

Go:   func (u User) String() string { return u.Name }
来源：http://abo.sysykeji.top

Ruby: def to_s; @name; end
来源：http://tad.cheryme.top

C#:   public override string ToString() => Name;
来源：http://cge.dashuyun.cn

[G13] 判断对象类型
来源：http://anw.hnxiangtu.top

Py:   isinstance(u, User)
来源：http://fbr.xinyue.icu

PHP:  $u instanceof User
来源：http://qqr.tianlin.xyz

JS:   u instanceof User
来源：http://fmy.shuidangran.top

TS:   u instanceof User
来源：http://pme.andypj.xyz

Java: u instanceof User
来源：http://jhl.316326.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://eqa.shanyushiyangkeji.top

Ruby: u.is_a?(User)
来源：http://onp.vehdjk.com

C#:   u is User
来源：http://ggz.yongpay.top

[G14] 数据类 / record
来源：http://lmf.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wnr.daxiang520.top

PHP:  // 用 readonly 属性模拟
来源：http://aiu.sysykeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://ztg.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://jnk.cheryme.top

Java: record User(String name, int age) {}
来源：http://uvz.gaohongyu789.top

Go:   type User struct { Name string; Age int }
来源：http://vub.dashuyun.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zib.cashguo.top

C#:   record User(string Name, int Age);
来源：http://gju.bjfxy.top

[G15] 枚举
来源：http://jpv.zhaomingkeji.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bds.tianlin.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://xih.yfazqb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ezk.daria6918.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://arv.sysykeji.top

Java: enum Color { RED, GREEN }
来源：http://kbf.zhijiandao.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rgi.cucudq.cn

Ruby: Color = %i[red green].freeze
来源：http://utb.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nbc.yj20258888.top

[G16] 对象转数组 / 字典
来源：http://jfy.c1oappe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wyy.gaohongyu789.top

PHP:  get_object_vars($obj);
来源：http://kwo.tianlin.xyz

JS:   Object.entries(obj)
来源：http://wmw.yj20258888.top

TS:   Object.entries(obj)
来源：http://qjz.wangshuangyany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jfo.nanxinkj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dkt.gotoacloud.top

Ruby: obj.instance_variables
来源：http://tbk.hcnkem.com

C#:   // 用反射或 System.Text.Json
来源：http://wrp.zhengqikj.top

================================================================================
来源：http://suw.ppjwa.cn

H. 异常与错误处理
来源：http://dlt.xinyue.icu

================================================================================
来源：http://riq.shuidangran.top

[H01] try / catch 基础
来源：http://tvn.jinqigufen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kml.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wle.ehwqpu.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://scj.guowangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xyg.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qmu.jqgufenzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://exm.zhengqikj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eiv.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yjr.hfpthk.cn

[H02] finally / ensure 收尾
来源：http://tsm.xylfe.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qqd.cdnleiting.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ajl.zhiwuduotai.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bol.ctjpmb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://cey.dashuyun.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kkn.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://yay.quarkkingdee.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nbg.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qfh.ivvv.top

[H03] 主动抛出异常
来源：http://kvk.zdbjq.cn

Py:   raise ValueError("错误信息")
来源：http://gso.tanke756.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bbr.ctjpmb.com

JS:   throw new Error("错误信息");
来源：http://cor.nanxuanxn.top

TS:   throw new Error("错误信息");
来源：http://ofs.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bwb.nwbrower.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pry.xingfuxueyuan.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://rww.yanxiufei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kjo.xziqi.cn

[H04] 自定义异常类型
来源：http://vrb.xingfuxueyuan.xyz

Py:   class MyError(Exception): pass
来源：http://rbx.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://oqu.yonumen.top

JS:   class MyError extends Error {}
来源：http://hgd.zdbjq.cn

TS:   class MyError extends Error {}
来源：http://waf.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://szf.0kj1m.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bma.guannengcc.top

Ruby: class MyError < StandardError; end
来源：http://dkf.zdbjq.cn

C#:   class MyException : Exception {}
来源：http://cdx.zdbjq.cn

[H05] 捕获特定类型
来源：http://zsi.c1oappe.top

Py:   except ValueError as e:
来源：http://mpr.dianchejie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pwu.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://kmp.yj20258888.top

TS:   if (e instanceof TypeError) {}
来源：http://yxh.0kj1m.cn

Java: catch (IOException | SQLException e) {}
来源：http://jja.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gkg.yangfankeji.com

Ruby: rescue ArgumentError => e
来源：http://dcw.daxiang520.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://axl.redwolf501.top

[H06] 可选值 / 空值安全访问
来源：http://glx.jyoumei.cn

Py:   value = d.get("k") or default
来源：http://tmh.xingfuxueyuan.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://jty.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://emb.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://emk.meibo888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iet.gogol.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fsr.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://ikn.cdnleiting.top

C#:   obj?.A?.B ?? default
来源：http://cir.yongpay.top

[H07] 断言
来源：http://opu.hnxiangtu.top

Py:   assert x > 0, "必须为正"
来源：http://peu.sysykeji.top

PHP:  assert($x > 0);
来源：http://cvi.zhijiandao.cn

JS:   console.assert(x > 0);
来源：http://vmp.yfazqb.com


<!-- 参考信息 -->