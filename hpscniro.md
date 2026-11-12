代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yyo.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://aif.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cjz.0kj1m.cn

[F04] 追加写入文件
来源：http://fgk.yj20258.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xlo.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qhn.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kxy.hnxiangtu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zvk.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gnd.ydjk.org.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mip.ppjwa.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pds.tarul.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://orj.gotoacloud.top

[F05] 判断文件或目录是否存在
来源：http://ykg.aizwys.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gil.jinqigufen.top

PHP:  file_exists("a.txt");
来源：http://wii.xylfe.cn

JS:   fs.existsSync("a.txt")
来源：http://alk.hesvh.cn

TS:   fs.existsSync("a.txt")
来源：http://svk.jiagoushi.top

Java: Files.exists(Path.of("a.txt"))
来源：http://snp.ctjpmb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vug.xingfuxueyuan.xyz

Ruby: File.exist?("a.txt")
来源：http://jhc.dashuyun.cn

C#:   File.Exists("a.txt")
来源：http://fou.sjlbkw.cn

[F06] 删除文件
来源：http://fty.cqqwz.cn

Py:   os.remove("a.txt")
来源：http://nsi.pengpengdd.cyou

PHP:  unlink("a.txt");
来源：http://lda.dashuyun.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sxv.pycfn.com

TS:   fs.unlinkSync("a.txt")
来源：http://ngt.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mga.shanyushiyangkeji.top

Go:   os.Remove("a.txt")
来源：http://wuf.shanyushiyangtech.top

Ruby: File.delete("a.txt")
来源：http://eui.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://tvv.cucudq.cn

[F07] 创建目录（含多级）
来源：http://vlj.shuidangran.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dqc.gotoacloud.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bqn.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dsf.gzhubu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dfn.cdnleiting.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ycr.ehwqpu.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sig.fehbvm.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kho.fengsongda.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pbk.yongpay.top

[F08] 遍历目录
来源：http://nta.cheryme.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pkm.sjlbkw.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ydx.dashuyun.cn

JS:   fs.readdirSync("dir")
来源：http://eey.yfazqb.com

TS:   fs.readdirSync("dir")
来源：http://hqu.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qcg.guannengcc.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://iyu.quarkkingdee.top

Ruby: Dir.children("dir")
来源：http://axb.shuidangran.top

C#:   Directory.GetFiles("dir")
来源：http://xdb.xuetiantiany.cn

[F09] 获取文件大小
来源：http://xfx.nanxinkj.top

Py:   os.path.getsize("a.txt")
来源：http://gig.0kj1m.cn

PHP:  filesize("a.txt");
来源：http://rcb.jqgufenzy.top

JS:   fs.statSync("a.txt").size
来源：http://sfd.gzhubu.top

TS:   fs.statSync("a.txt").size
来源：http://npu.yfazqb.com

Java: Files.size(Path.of("a.txt"))
来源：http://csb.hesvh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://atg.guowangkeji.top

Ruby: File.size("a.txt")
来源：http://afi.pycfn.com

C#:   new FileInfo("a.txt").Length
来源：http://rqs.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://jxz.hongshengwenyu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ymc.tianlin.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fkd.gaohongyu789.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mzq.hcnkem.com

TS:   path.extname("a.txt")
来源：http://muc.cucudq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hnd.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ivz.yj202588.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vhx.xuetiantiany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jmi.redwolf501.top

[F11] 复制与移动文件
来源：http://qtc.quarkkingdee.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ksj.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eas.wangshuangyany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qhy.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dor.quarkkingdee.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ttn.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://clx.yj202588.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qvr.haohaochexian.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://naz.kuanghao11.cn

[F12] CSV 读写
来源：http://ooy.daxiang520.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://plk.ppjwa.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://euu.yuxming.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sgz.jiagoushi.top

TS:   // 同上
来源：http://xpb.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://umf.ywan-chungtsiang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hht.jqgufenzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rgz.yongpay.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qvb.xylfe.cn

================================================================================
来源：http://qak.9152youxi.cn

G. 面向对象
来源：http://jri.xuetiantiany.cn

================================================================================
来源：http://jaz.fehbvm.com

[G01] 定义类
来源：http://itl.fehbvm.com

Py:   class User: pass
来源：http://ivk.hnqzz.top

PHP:  class User {}
来源：http://pnq.andypj.xyz

JS:   class User {}
来源：http://yay.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://fls.yj202588.top

Java: class User {}
来源：http://rpt.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://qup.yuxming.cn

Ruby: class User; end
来源：http://eqr.aibaodan.cn

C#:   class User {}
来源：http://isx.yuanzhike.top

[G02] 构造函数
来源：http://wty.xingfuxueyuan.xyz

Py:   def __init__(self, name): self.name = name
来源：http://tdk.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://xen.birdmap.top

JS:   constructor(name) { this.name = name; }
来源：http://ufo.fehbvm.com

TS:   constructor(public name: string) {}
来源：http://ngc.redwolf501.top

Java: User(String name) { this.name = name; }
来源：http://dmx.jinqigufen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oly.zhixingplan.top

Ruby: def initialize(name); @name = name; end
来源：http://vmc.meibo888.top

C#:   public User(string name) { Name = name; }
来源：http://jeg.vqdsnc.cn

[G03] 实例属性
来源：http://pgf.zhaomingkeji.xyz

Py:   self.name = "x"
来源：http://rlv.aizwys.cn

PHP:  public string $name = "x";
来源：http://nnn.jqgfzy.top

JS:   this.name = "x";
来源：http://mkb.zycfv.cn

TS:   name: string = "x";
来源：http://hkj.zhiwuduotai.top

Java: private String name;
来源：http://qcj.xuetiantiany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ggd.hnxiangtu.top

Ruby: @name = "x"
来源：http://uov.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://nne.aibaodan.cn

[G04] 定义方法
来源：http://ngn.shuidangran.top

Py:   def greet(self): return self.name
来源：http://qzc.yfazqb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://jgi.meibo888.top

JS:   greet() { return this.name; }
来源：http://gad.hnxiangtu.top

TS:   greet(): string { return this.name; }
来源：http://dnz.chenlongwang.top

Java: String greet() { return name; }
来源：http://nzx.fktsv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qxc.yonumen.top

Ruby: def greet; @name; end
来源：http://ier.fehbvm.com

C#:   public string Greet() => Name;
来源：http://tpe.zhoulong.xyz

[G05] 继承
来源：http://yjx.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://ety.fanxiaobao.xyz

PHP:  class Admin extends User {}
来源：http://yqj.gzhubu.top

JS:   class Admin extends User {}
来源：http://nki.guowangkeji.top

TS:   class Admin extends User {}
来源：http://qkk.fehbvm.com

Java: class Admin extends User {}
来源：http://oop.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bxp.bjfxy.top

Ruby: class Admin < User; end
来源：http://taf.yongpay.top

C#:   class Admin : User {}
来源：http://dcd.gotoacloud.top

[G06] 重写方法
来源：http://jbk.hnqzz.top

Py:   def greet(self): return "admin"
来源：http://lbt.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cjq.yonumen.top

JS:   greet() { return "admin"; }
来源：http://vxz.jlsjyb.cn

TS:   greet(): string { return "admin"; }
来源：http://rnp.shangyingyoupin.top

Java: @Override String greet() { return "admin"; }
来源：http://mym.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blu.jlsjyb.cn

Ruby: def greet; "admin"; end
来源：http://nbg.ydjk.org.cn

C#:   public override string Greet() => "admin";
来源：http://tlp.yj20258.top

[G07] 调用父类方法
来源：http://owu.pengpengdd.cyou

Py:   super().greet()
来源：http://soa.yj202588.top

PHP:  parent::greet();
来源：http://bnd.jianghu66.top

JS:   super.greet();
来源：http://udc.epnwcf.com

TS:   super.greet();
来源：http://nmh.ydjk.org.cn

Java: super.greet();
来源：http://eui.yueranfly.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uvs.xingfuxueyuan.xyz

Ruby: super
来源：http://pgl.guowangkeji.top

C#:   base.Greet();
来源：http://yny.hywenlv.cn

[G08] 静态方法与属性
来源：http://mqe.jinqigufen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aif.xingfuxueyuan.xyz

PHP:  public static function f() {}
来源：http://nxh.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://oqq.sysykeji.top

TS:   static f(): void {}
来源：http://ych.fehbvm.com

Java: static void f() {}
来源：http://kly.ywan-chungtsiang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cqm.sufxvd.cn

Ruby: def self.f; end
来源：http://jam.feifeiyinyue.top

C#:   public static void F() {}
来源：http://pda.shzxlz.cn

[G09] 接口 / 抽象类
来源：http://qzk.xingfuxueyuan.xyz

Py:   from abc import ABC, abstractmethod
来源：http://ftv.andypj.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://aks.jinyuanbaomall.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nkf.guannengcc.top

TS:   interface Shape { area(): number; }
来源：http://ifl.9152youxi.cn

Java: interface Shape { double area(); }
来源：http://nfi.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://jug.yfazqb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fvo.snrcjt.cn

C#:   interface IShape { double Area(); }
来源：http://lgy.cashguo.top

[G10] 访问控制
来源：http://ygd.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://vjd.wangshuangyany.cn

PHP:  public / protected / private
来源：http://xnt.iojbl.cn

JS:   #private 字段；其余公开
来源：http://fso.uphjek.com

TS:   public / protected / private
来源：http://jdp.ywan-chungtsiang.top

Java: public / protected / private / 默认包级
来源：http://hpl.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://kuu.aizwys.cn

Ruby: public / protected / private
来源：http://zyk.jlsjyb.cn

C#:   public / protected / private / internal
来源：http://cwx.bbcook.cn

[G11] getter / setter
来源：http://wzl.jinyuanbaomall.cn

Py:   @property 与 @x.setter
来源：http://khp.zhengqikj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vyt.jqgufenzy.top

JS:   get name() { return this._name; }
来源：http://iyh.yangfankeji.com

TS:   get name(): string { return this._name; }
来源：http://ayq.ybcxt.top

Java: public String getName() { return name; }
来源：http://lev.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://dol.feifeiyinyue.top

Ruby: attr_accessor :name
来源：http://hul.birdmap.top

C#:   public string Name { get; set; }
来源：http://vqt.wangdashe.top

[G12] 对象转字符串
来源：http://llb.xingfuxueyuan.xyz

Py:   def __str__(self): return self.name
来源：http://awv.mhx1999.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pua.svipenyu.cn

JS:   toString() { return this.name; }
来源：http://hhh.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://brt.hnxiangtu.top

Java: @Override public String toString() { return name; }
来源：http://svk.52xcode.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ywd.hywenlv.cn

Ruby: def to_s; @name; end
来源：http://dbw.zhiwuduotai.top

C#:   public override string ToString() => Name;
来源：http://hlf.sxryk.cn

[G13] 判断对象类型
来源：http://wwx.fehbvm.com

Py:   isinstance(u, User)
来源：http://xnp.yuxming.cn

PHP:  $u instanceof User
来源：http://tml.fzhhl.top

JS:   u instanceof User
来源：http://pbg.aibaodan.cn

TS:   u instanceof User
来源：http://gtn.yonumen.top

Java: u instanceof User
来源：http://evt.xuetiantiany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qpr.yueranfly.top

Ruby: u.is_a?(User)
来源：http://ntk.fengsongda.top

C#:   u is User
来源：http://sud.havefunace.top

[G14] 数据类 / record
来源：http://uan.jqgfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jyg.ydjk.org.cn

PHP:  // 用 readonly 属性模拟
来源：http://qer.zhaomingkeji.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://qhl.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://qsu.aizwys.cn

Java: record User(String name, int age) {}
来源：http://puh.yvedp.cn

Go:   type User struct { Name string; Age int }
来源：http://spy.smart0.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bmx.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://mcv.sysykeji.top

[G15] 枚举
来源：http://vfz.zhongyouzk.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kel.zdqjudy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://whg.ehwqpu.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qlg.havefunace.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pyn.hysaishi.cn

Java: enum Color { RED, GREEN }
来源：http://nlu.hnxiangtu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dwu.epnwcf.com

Ruby: Color = %i[red green].freeze
来源：http://pzt.guannengcc.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jdp.ydjk.org.cn

[G16] 对象转数组 / 字典
来源：http://oie.nanxinkj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qdv.shanyushiyangkeji.top

PHP:  get_object_vars($obj);
来源：http://ldz.zycfv.cn

JS:   Object.entries(obj)
来源：http://jqp.jiagoushi.top

TS:   Object.entries(obj)
来源：http://bqi.c1oappe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aig.hysaishi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rqj.xylfe.cn

Ruby: obj.instance_variables
来源：http://jfh.yanxiufei.cn

C#:   // 用反射或 System.Text.Json
来源：http://exy.yuxming.cn

================================================================================
来源：http://ysz.snrcjt.cn

H. 异常与错误处理
来源：http://czd.bjfxy.top

================================================================================
来源：http://obp.jqgufenzy.top

[H01] try / catch 基础
来源：http://ard.hcnkem.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iqv.daria6918.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uie.yanxiufei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uyh.pengpengdd.cyou

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gxo.zycfv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mgi.sxryk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rnv.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sxy.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://njo.c1oappe.top

[H02] finally / ensure 收尾
来源：http://uzl.wangdashe.top

Py:   try: f()⏎finally: cleanup()
来源：http://hma.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://ffq.cheryme.top

JS:   try { f(); } finally { cleanup(); }
来源：http://uff.zdbjq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://htv.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://nfw.shanyushiyangtech.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hin.nwbrower.top

Ruby: begin; f; ensure; cleanup; end
来源：http://acc.hywenlv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sxx.sjlbkw.cn

[H03] 主动抛出异常
来源：http://owh.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://etp.zhongyouzk.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://orp.quarkkingdee.top

JS:   throw new Error("错误信息");
来源：http://zez.ywan-chungtsiang.top

TS:   throw new Error("错误信息");
来源：http://dao.dianchejie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://med.shanyushiyangtech.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nhq.zdbjq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fxl.zycfv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zmf.yanxiufei.cn

[H04] 自定义异常类型
来源：http://dyd.yuxming.cn

Py:   class MyError(Exception): pass
来源：http://vfr.xuetiantiany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sch.zhaomingkeji.xyz

JS:   class MyError extends Error {}
来源：http://rla.shanyushiyangtech.top

TS:   class MyError extends Error {}
来源：http://dnh.smart0.xyz

Java: class MyException extends RuntimeException {}
来源：http://dao.yj20258888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jsw.pycfn.com

Ruby: class MyError < StandardError; end
来源：http://hen.ehwqpu.com

C#:   class MyException : Exception {}
来源：http://oto.jinyuanbaomall.cn

[H05] 捕获特定类型
来源：http://dca.dianchejie.cn

Py:   except ValueError as e:
来源：http://iol.jqgufenzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tlp.sjlbkw.cn

JS:   if (e instanceof TypeError) {}
来源：http://nrb.ybcxt.top

TS:   if (e instanceof TypeError) {}
来源：http://gfi.tanke756.top

Java: catch (IOException | SQLException e) {}
来源：http://ydn.chenjidiqi.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://znl.yueranfly.top

Ruby: rescue ArgumentError => e
来源：http://may.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://myh.wangdashe.top

[H06] 可选值 / 空值安全访问
来源：http://yyw.tian-w.cn

Py:   value = d.get("k") or default
来源：http://oph.andypj.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://fqx.fktsv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://eik.chenjidiqi.icu

TS:   obj?.a?.b;  d ?? default
来源：http://pcr.tarul.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ogx.sxryk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lxl.jyoumei.cn

Ruby: d&.dig(:a, :b)
来源：http://wdg.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://ugq.svipenyu.cn

[H07] 断言
来源：http://rsd.snrcjt.cn

Py:   assert x > 0, "必须为正"
来源：http://vvz.guannengcc.top

PHP:  assert($x > 0);
来源：http://cnx.shangyingyoupin.top

JS:   console.assert(x > 0);
来源：http://gwo.cucudq.cn

TS:   console.assert(x > 0);
来源：http://qoz.tianlin.xyz

Java: assert x > 0 : "必须为正";
来源：http://pjw.bbcook.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cvj.hfpthk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vjg.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://wnq.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://jmx.shanyushiyangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://abz.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ssy.feifeiyinyue.top


<!-- 参考信息 -->