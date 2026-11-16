代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lly.kuanghao11.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ori.xuanzx.com

[F03] 写入文件（覆盖）
来源：http://ywb.shanyushiyangtech.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ekd.fzhhl.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://imr.xuanzx.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kbj.yanxiufei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://frc.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lah.316326.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://edw.yuxming.cn

Ruby: File.write("a.txt", "hi")
来源：http://pif.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sdi.52xcode.cn

[F04] 追加写入文件
来源：http://hgr.xinyue.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vxn.zhoulong.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xie.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dak.guannengcc.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uew.yangfankeji.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qmj.smart0.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pyx.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://prm.jinqigufen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qim.yj202588.top

[F05] 判断文件或目录是否存在
来源：http://sfk.tarul.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dgn.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://rfm.ppjwa.cn

JS:   fs.existsSync("a.txt")
来源：http://dgk.nanxuanxn.top

TS:   fs.existsSync("a.txt")
来源：http://ezc.quarkkingdee.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nxl.zhaomingkeji.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vji.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://zai.bjfxy.top

C#:   File.Exists("a.txt")
来源：http://bsr.ctjpmb.com

[F06] 删除文件
来源：http://wwk.zhixingplan.top

Py:   os.remove("a.txt")
来源：http://dby.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://bwi.jyoumei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eaa.sysykeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://lgt.nwbrower.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nxm.hysaishi.cn

Go:   os.Remove("a.txt")
来源：http://fsa.chenjidiqi.icu

Ruby: File.delete("a.txt")
来源：http://nvw.nanxinkj.top

C#:   File.Delete("a.txt");
来源：http://gbf.hesvh.cn

[F07] 创建目录（含多级）
来源：http://nhx.ehwqpu.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zxh.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dag.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jbg.pycfn.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tyu.aizwys.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://byb.snrcjt.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tqw.ehwqpu.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ioy.cdnleiting.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cgo.sysykeji.top

[F08] 遍历目录
来源：http://ufu.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qgn.guannengcc.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://awt.316326.xyz

JS:   fs.readdirSync("dir")
来源：http://caf.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://rii.svipenyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lhh.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wgu.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://jho.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://jlz.zhaomingkeji.xyz

[F09] 获取文件大小
来源：http://oqn.tianlin.xyz

Py:   os.path.getsize("a.txt")
来源：http://xfs.sysykeji.top

PHP:  filesize("a.txt");
来源：http://nzn.hammf.cn

JS:   fs.statSync("a.txt").size
来源：http://pzo.sweek.top

TS:   fs.statSync("a.txt").size
来源：http://xuu.yj202588.top

Java: Files.size(Path.of("a.txt"))
来源：http://zfm.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oxg.sufxvd.cn

Ruby: File.size("a.txt")
来源：http://cly.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://frt.sxryk.cn

[F10] 取文件扩展名 / 文件名
来源：http://eas.yvedp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wpk.sjlbkw.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ege.fengsongda.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wbp.ybcxt.top

TS:   path.extname("a.txt")
来源：http://hkp.316326.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zbi.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://etu.ybcxt.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pym.nanxinkj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jvv.jinghuilouyu.cn

[F11] 复制与移动文件
来源：http://acl.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ggb.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dqu.gaohongyu789.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cuk.mhx1999.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nza.iojbl.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://juo.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bfd.fanxiaobao.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rtb.chenlongwang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://znk.chenlongwang.top

[F12] CSV 读写
来源：http://lfo.zhongyouzk.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wlq.ivvv.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cbs.sjlbkw.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tce.sufxvd.cn

TS:   // 同上
来源：http://dtp.yanxiufei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bbe.svipenyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hoj.zdqjudy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hlq.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://iqg.yangfankeji.com

================================================================================
来源：http://vtw.chenlongwang.top

G. 面向对象
来源：http://yos.jinghuilouyu.cn

================================================================================
来源：http://oqa.tarul.cn

[G01] 定义类
来源：http://csh.tian-w.cn

Py:   class User: pass
来源：http://gmt.hfpthk.cn

PHP:  class User {}
来源：http://hzf.zdqjudy.top

JS:   class User {}
来源：http://pdi.shzxlz.cn

TS:   class User { name: string = ""; }
来源：http://sxd.wangdashe.top

Java: class User {}
来源：http://dkq.zhengqikj.top

Go:   type User struct { Name string }
来源：http://ohn.zdbjq.cn

Ruby: class User; end
来源：http://lxi.shuidangran.top

C#:   class User {}
来源：http://yzx.aizwys.cn

[G02] 构造函数
来源：http://mpn.jqgufenzy.top

Py:   def __init__(self, name): self.name = name
来源：http://uzz.yongpay.top

PHP:  public function __construct(public string $name) {}
来源：http://dhs.haohaochexian.top

JS:   constructor(name) { this.name = name; }
来源：http://izt.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://lrr.sysykeji.top

Java: User(String name) { this.name = name; }
来源：http://kdv.cqqwz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rit.haohaochexian.top

Ruby: def initialize(name); @name = name; end
来源：http://zgl.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://kfd.ydzc1.top

[G03] 实例属性
来源：http://ius.aizwys.cn

Py:   self.name = "x"
来源：http://rwa.zhixingplan.top

PHP:  public string $name = "x";
来源：http://ico.hongshengwenyu.top

JS:   this.name = "x";
来源：http://mgx.cheryme.top

TS:   name: string = "x";
来源：http://iqf.vehdjk.com

Java: private String name;
来源：http://ifj.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uzz.xuanzx.com

Ruby: @name = "x"
来源：http://efs.svipenyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://tbd.zdqjudy.top

[G04] 定义方法
来源：http://xqn.yueranfly.top

Py:   def greet(self): return self.name
来源：http://tze.svipenyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rod.cheryme.top

JS:   greet() { return this.name; }
来源：http://wgw.shzxlz.cn

TS:   greet(): string { return this.name; }
来源：http://zlg.fengsongda.top

Java: String greet() { return name; }
来源：http://gdi.cashguo.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hly.chenlongwang.top

Ruby: def greet; @name; end
来源：http://ref.zhaomingkeji.xyz

C#:   public string Greet() => Name;
来源：http://dqj.shzxlz.cn

[G05] 继承
来源：http://bqn.hesvh.cn

Py:   class Admin(User): pass
来源：http://fkf.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://iti.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://dbl.xingfuxueyuan.xyz

TS:   class Admin extends User {}
来源：http://sfb.zdqjudy.top

Java: class Admin extends User {}
来源：http://jmc.zdqjudy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ncy.aizwys.cn

Ruby: class Admin < User; end
来源：http://bfs.shanyushiyangkeji.top

C#:   class Admin : User {}
来源：http://arq.ppjwa.cn

[G06] 重写方法
来源：http://dqp.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://rxy.tarul.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mlb.wangshuangyany.cn

JS:   greet() { return "admin"; }
来源：http://fci.shanyushiyangtech.top

TS:   greet(): string { return "admin"; }
来源：http://iaz.cqqwz.cn

Java: @Override String greet() { return "admin"; }
来源：http://vkk.bbcook.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fae.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://wtl.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://nqj.pengpengdd.cyou

[G07] 调用父类方法
来源：http://ogt.zhoulong.xyz

Py:   super().greet()
来源：http://nxi.epnwcf.com

PHP:  parent::greet();
来源：http://atk.shangyingyoupin.top

JS:   super.greet();
来源：http://dmw.dianchejie.cn

TS:   super.greet();
来源：http://vtq.yuanzhike.top

Java: super.greet();
来源：http://hpf.jianghu66.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bge.birdmap.top

Ruby: super
来源：http://fif.fanxiaobao.xyz

C#:   base.Greet();
来源：http://oii.xziqi.cn

[G08] 静态方法与属性
来源：http://qdd.hfpthk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vfi.gzhubu.top

PHP:  public static function f() {}
来源：http://moq.feifeiyinyue.top

JS:   static f() {}
来源：http://oim.daria6918.cn

TS:   static f(): void {}
来源：http://thz.hcnkem.com

Java: static void f() {}
来源：http://rzy.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mve.zdqjudy.top

Ruby: def self.f; end
来源：http://acd.9152youxi.cn

C#:   public static void F() {}
来源：http://zkz.jinyuanbaomall.cn

[G09] 接口 / 抽象类
来源：http://tuh.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://bly.yangfankeji.com

PHP:  interface Shape { public function area(): float; }
来源：http://ixw.pengpengdd.cyou

JS:   // 无接口：靠约定或 JSDoc
来源：http://fex.tarul.cn

TS:   interface Shape { area(): number; }
来源：http://ddx.zdqjudy.top

Java: interface Shape { double area(); }
来源：http://hsd.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://ftc.52xcode.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lwd.gogol.net.cn

C#:   interface IShape { double Area(); }
来源：http://xqk.hywenlv.cn

[G10] 访问控制
来源：http://oep.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://azb.wangdashe.top

PHP:  public / protected / private
来源：http://gft.52xcode.cn

JS:   #private 字段；其余公开
来源：http://cdk.hfpthk.cn

TS:   public / protected / private
来源：http://rty.zhaomingkeji.xyz

Java: public / protected / private / 默认包级
来源：http://vcz.cheryme.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ehr.gaohongyu789.top

Ruby: public / protected / private
来源：http://gpr.wangshuangyany.cn

C#:   public / protected / private / internal
来源：http://yhf.tian-w.cn

[G11] getter / setter
来源：http://kwt.quarkkingdee.top

Py:   @property 与 @x.setter
来源：http://mdw.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jom.bbcook.cn

JS:   get name() { return this._name; }
来源：http://hql.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://kdc.birdmap.top

Java: public String getName() { return name; }
来源：http://ldm.dashuyun.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jpr.sxryk.cn

Ruby: attr_accessor :name
来源：http://iuh.cashguo.top

C#:   public string Name { get; set; }
来源：http://olp.shzxlz.cn

[G12] 对象转字符串
来源：http://anm.wangdashe.top

Py:   def __str__(self): return self.name
来源：http://cqt.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://gtf.316326.xyz

JS:   toString() { return this.name; }
来源：http://sol.zhiwuduotai.top

TS:   toString(): string { return this.name; }
来源：http://ywo.jinghuilouyu.cn

Java: @Override public String toString() { return name; }
来源：http://xzo.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ycq.gzhubu.top

Ruby: def to_s; @name; end
来源：http://gri.fengsongda.top

C#:   public override string ToString() => Name;
来源：http://ydh.hywenlv.cn

[G13] 判断对象类型
来源：http://euk.yanxiufei.cn

Py:   isinstance(u, User)
来源：http://sfl.yanxiufei.cn

PHP:  $u instanceof User
来源：http://yqh.smart0.xyz

JS:   u instanceof User
来源：http://tls.ehwqpu.com

TS:   u instanceof User
来源：http://jma.dianchejie.cn

Java: u instanceof User
来源：http://zog.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://btu.xingfuxueyuan.xyz

Ruby: u.is_a?(User)
来源：http://xfn.kuanghao11.cn

C#:   u is User
来源：http://dmp.meibo888.top

[G14] 数据类 / record
来源：http://vbe.chenlongwang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vgc.hammf.cn

PHP:  // 用 readonly 属性模拟
来源：http://wvy.zdqjudy.top

JS:   // 无内置：普通类或对象字面量
来源：http://yom.shangyingyoupin.top

TS:   type User = { name: string; age: number };
来源：http://uyi.yfazqb.com

Java: record User(String name, int age) {}
来源：http://tsv.xuanzx.com

Go:   type User struct { Name string; Age int }
来源：http://peb.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://igo.zycfv.cn

C#:   record User(string Name, int Age);
来源：http://dud.pycfn.com

[G15] 枚举
来源：http://aeb.xylfe.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://axe.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vlr.vehdjk.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://upv.jlsjyb.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fxm.tianlin.xyz

Java: enum Color { RED, GREEN }
来源：http://abc.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hpa.tianlin.xyz

Ruby: Color = %i[red green].freeze
来源：http://jik.ctjpmb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kej.andypj.xyz

[G16] 对象转数组 / 字典
来源：http://tjf.ybcxt.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pbv.jqgfzy.top

PHP:  get_object_vars($obj);
来源：http://ozl.sxryk.cn

JS:   Object.entries(obj)
来源：http://def.snrcjt.cn

TS:   Object.entries(obj)
来源：http://mgn.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pek.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ead.yj20258.top

Ruby: obj.instance_variables
来源：http://tol.sjlbkw.cn

C#:   // 用反射或 System.Text.Json
来源：http://zhl.yangfankeji.com

================================================================================
来源：http://agh.vqdsnc.cn

H. 异常与错误处理
来源：http://gob.zhongyouzk.top

================================================================================
来源：http://eah.jinqigufen.top

[H01] try / catch 基础
来源：http://rhz.hysaishi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ohz.hnqzz.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://smj.ctjpmb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hdm.cashguo.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://udo.ehwqpu.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ltd.jinqigfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ski.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wtr.feifeiyinyue.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pqy.zdqjudy.top

[H02] finally / ensure 收尾
来源：http://mfa.andypj.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://aeh.wangshuangyany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vnn.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://nlu.bbcook.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mio.pycfn.com

Java: try { f(); } finally { cleanup(); }
来源：http://yla.jinqigfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ssk.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://scw.nanxuanxn.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gyx.svipenyu.cn

[H03] 主动抛出异常
来源：http://owa.xuanzx.com

Py:   raise ValueError("错误信息")
来源：http://sfq.daria6918.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://icv.yanxiufei.cn

JS:   throw new Error("错误信息");
来源：http://uhe.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://zho.gaohongyu789.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lik.ehwqpu.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ppk.9152youxi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jjl.ywan-chungtsiang.top

C#:   throw new ArgumentException("错误信息");
来源：http://veo.vehdjk.com

[H04] 自定义异常类型
来源：http://unl.smart0.xyz

Py:   class MyError(Exception): pass
来源：http://yfn.zhiwuduotai.top

PHP:  class MyError extends RuntimeException {}
来源：http://qus.jinqigfzy.top

JS:   class MyError extends Error {}
来源：http://wrz.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://ttz.shuidangran.top

Java: class MyException extends RuntimeException {}
来源：http://bms.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nzl.jqgfzy.top

Ruby: class MyError < StandardError; end
来源：http://wuw.yuanzhike.top

C#:   class MyException : Exception {}
来源：http://rne.hywenlv.cn

[H05] 捕获特定类型
来源：http://gqc.ctjpmb.com

Py:   except ValueError as e:
来源：http://msn.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://opj.hesvh.cn

JS:   if (e instanceof TypeError) {}
来源：http://mvv.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://nyc.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://eah.shuidangran.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cvi.c1oappe.top

Ruby: rescue ArgumentError => e
来源：http://onv.shanyushiyangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ses.sjlbkw.cn

[H06] 可选值 / 空值安全访问
来源：http://vyo.sysykeji.top

Py:   value = d.get("k") or default
来源：http://chr.nwbrower.top

PHP:  $v = $d["k"] ?? null;
来源：http://gua.yanxiufei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vgg.shanyushiyangtech.top

TS:   obj?.a?.b;  d ?? default
来源：http://utr.kuanghao11.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hof.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://izs.shuidangran.top

Ruby: d&.dig(:a, :b)
来源：http://cko.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://rvj.nwbrower.top

[H07] 断言
来源：http://vwk.jinghuilouyu.cn

Py:   assert x > 0, "必须为正"
来源：http://tms.ydzc1.top

PHP:  assert($x > 0);
来源：http://caa.redwolf501.top

JS:   console.assert(x > 0);
来源：http://oyb.cheryme.top


<!-- 参考信息 -->