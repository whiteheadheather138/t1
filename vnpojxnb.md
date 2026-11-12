代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ntx.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://apn.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://ytp.jqgufenzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qtu.xinyue.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://pax.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ejb.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vfa.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wgy.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xgo.xuanzx.com

Ruby: File.write("a.txt", "hi")
来源：http://hlg.chenzaomai.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cbm.ctjpmb.com

[F04] 追加写入文件
来源：http://zuw.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wyj.zdqjudy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yey.fzhhl.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ova.yj20258888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fuo.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mcv.hesvh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ybw.hesvh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ltb.epnwcf.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bdv.tianlin.xyz

[F05] 判断文件或目录是否存在
来源：http://dmw.yangfankeji.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zsd.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://rcw.snrcjt.cn

JS:   fs.existsSync("a.txt")
来源：http://kah.hongshengwenyu.top

TS:   fs.existsSync("a.txt")
来源：http://dpc.cashguo.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yow.guannengcc.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vio.hnxiangtu.top

Ruby: File.exist?("a.txt")
来源：http://fjv.fehbvm.com

C#:   File.Exists("a.txt")
来源：http://bhz.vqdsnc.cn

[F06] 删除文件
来源：http://qks.vqdsnc.cn

Py:   os.remove("a.txt")
来源：http://kbr.jinyuanbaomall.cn

PHP:  unlink("a.txt");
来源：http://kpd.nanxuanxn.top

JS:   fs.unlinkSync("a.txt")
来源：http://jei.ppjwa.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qza.ivvv.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fzp.xuetiantiany.cn

Go:   os.Remove("a.txt")
来源：http://ics.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://ktd.cheryme.top

C#:   File.Delete("a.txt");
来源：http://dam.hammf.cn

[F07] 创建目录（含多级）
来源：http://qed.yj20258888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://arb.wangshuangyany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kiq.tianlin.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jds.aizwys.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://htz.bjfxy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ffe.bjfxy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sto.birdmap.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iou.wangshuangyany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gxk.snrcjt.cn

[F08] 遍历目录
来源：http://eey.smart0.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://mhu.hywenlv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ijn.snrcjt.cn

JS:   fs.readdirSync("dir")
来源：http://ram.sysykeji.top

TS:   fs.readdirSync("dir")
来源：http://ndk.yj20258888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rlf.vqdsnc.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://veh.tian-w.cn

Ruby: Dir.children("dir")
来源：http://ftw.0kj1m.cn

C#:   Directory.GetFiles("dir")
来源：http://ptr.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://zmt.xinyue.icu

Py:   os.path.getsize("a.txt")
来源：http://poo.kuanghao11.cn

PHP:  filesize("a.txt");
来源：http://yad.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://yjc.ywan-chungtsiang.top

TS:   fs.statSync("a.txt").size
来源：http://ybr.yuanzhike.top

Java: Files.size(Path.of("a.txt"))
来源：http://vdk.hammf.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xap.aizwys.cn

Ruby: File.size("a.txt")
来源：http://fux.zhixingplan.top

C#:   new FileInfo("a.txt").Length
来源：http://rap.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://cwf.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eox.sxryk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lkl.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://srb.daria6918.cn

TS:   path.extname("a.txt")
来源：http://flp.jinqigufen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ryz.vehdjk.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ace.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pmt.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dyh.ybcxt.top

[F11] 复制与移动文件
来源：http://jby.meibo888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yuc.xziqi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tpk.mhx1999.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gpz.jiagoushi.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tnm.andypj.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xzq.ivvv.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://llk.jinqigufen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gni.cdnleiting.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nlt.chenjidiqi.icu

[F12] CSV 读写
来源：http://qic.yuanzhike.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://boo.hongshengwenyu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ymm.bbcook.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xho.jqgufenzy.top

TS:   // 同上
来源：http://vxd.c1oappe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nti.xziqi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lqy.316326.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qke.c1oappe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tdf.hnqzz.top

================================================================================
来源：http://syt.nanxinkj.top

G. 面向对象
来源：http://wyi.ywan-chungtsiang.top

================================================================================
来源：http://ysy.shanyushiyangkeji.top

[G01] 定义类
来源：http://rul.pengpengdd.cyou

Py:   class User: pass
来源：http://tww.zdbjq.cn

PHP:  class User {}
来源：http://egj.birdmap.top

JS:   class User {}
来源：http://vaa.xuanzx.com

TS:   class User { name: string = ""; }
来源：http://jbd.nwbrower.top

Java: class User {}
来源：http://yys.uphjek.com

Go:   type User struct { Name string }
来源：http://iwl.jqgfzy.top

Ruby: class User; end
来源：http://fce.jinqigfzy.top

C#:   class User {}
来源：http://tpc.svipenyu.cn

[G02] 构造函数
来源：http://jiz.chenzaomai.com

Py:   def __init__(self, name): self.name = name
来源：http://ivx.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://xly.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://xmq.yj20258888.top

TS:   constructor(public name: string) {}
来源：http://zlo.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://dof.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uxp.zhixingplan.top

Ruby: def initialize(name); @name = name; end
来源：http://lva.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://xpa.0kj1m.cn

[G03] 实例属性
来源：http://rse.yj20258888.top

Py:   self.name = "x"
来源：http://tyl.yueranfly.top

PHP:  public string $name = "x";
来源：http://jsv.bbcook.cn

JS:   this.name = "x";
来源：http://foh.cheryme.top

TS:   name: string = "x";
来源：http://gpc.jinqigfzy.top

Java: private String name;
来源：http://csq.vehdjk.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ayu.daxiang520.top

Ruby: @name = "x"
来源：http://nle.cdnleiting.top

C#:   public string Name { get; set; } = "x";
来源：http://wgz.yvedp.cn

[G04] 定义方法
来源：http://oru.tian-w.cn

Py:   def greet(self): return self.name
来源：http://dhz.yvedp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wvm.hongshengwenyu.top

JS:   greet() { return this.name; }
来源：http://aog.fanxiaobao.xyz

TS:   greet(): string { return this.name; }
来源：http://elh.dashuyun.cn

Java: String greet() { return name; }
来源：http://lin.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ttv.ybcxt.top

Ruby: def greet; @name; end
来源：http://ufm.nanxuanxn.top

C#:   public string Greet() => Name;
来源：http://jzw.xuanzx.com

[G05] 继承
来源：http://xzg.ydzc1.top

Py:   class Admin(User): pass
来源：http://fei.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://mrj.sweek.top

JS:   class Admin extends User {}
来源：http://gca.aizwys.cn

TS:   class Admin extends User {}
来源：http://rjb.tanke756.top

Java: class Admin extends User {}
来源：http://jeq.zhongyouzk.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qjl.fanxiaobao.xyz

Ruby: class Admin < User; end
来源：http://qmn.ehwqpu.com

C#:   class Admin : User {}
来源：http://jaf.cdnleiting.top

[G06] 重写方法
来源：http://zaa.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://ofw.tianlin.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://esm.yanxiufei.cn

JS:   greet() { return "admin"; }
来源：http://smi.cashguo.top

TS:   greet(): string { return "admin"; }
来源：http://fwc.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://sbz.zdbjq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pbw.nanxuanxn.top

Ruby: def greet; "admin"; end
来源：http://smz.hesvh.cn

C#:   public override string Greet() => "admin";
来源：http://dvn.yj20258.top

[G07] 调用父类方法
来源：http://rwt.ydzc1.top

Py:   super().greet()
来源：http://goo.hysaishi.cn

PHP:  parent::greet();
来源：http://phk.xziqi.cn

JS:   super.greet();
来源：http://qsa.ehwqpu.com

TS:   super.greet();
来源：http://gfp.cashguo.top

Java: super.greet();
来源：http://qea.ivvv.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iev.hfpthk.cn

Ruby: super
来源：http://taz.chenlongwang.top

C#:   base.Greet();
来源：http://swt.uphjek.com

[G08] 静态方法与属性
来源：http://mfb.andypj.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uje.yangfankeji.com

PHP:  public static function f() {}
来源：http://cax.zhongyouzk.top

JS:   static f() {}
来源：http://yls.gaohongyu789.top

TS:   static f(): void {}
来源：http://bhc.jinqigfzy.top

Java: static void f() {}
来源：http://hrf.sweek.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gcg.yvedp.cn

Ruby: def self.f; end
来源：http://qzt.zdqjudy.top

C#:   public static void F() {}
来源：http://pdj.meibo888.top

[G09] 接口 / 抽象类
来源：http://gqe.gogol.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://fht.sweek.top

PHP:  interface Shape { public function area(): float; }
来源：http://dua.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kzz.hfpthk.cn

TS:   interface Shape { area(): number; }
来源：http://phi.xinyue.icu

Java: interface Shape { double area(); }
来源：http://jgp.birdmap.top

Go:   type Shape interface { Area() float64 }
来源：http://cjg.yvedp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sye.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://hhj.yonumen.top

[G10] 访问控制
来源：http://ejb.yangfankeji.com

Py:   约定 _protected / __private（不强制）
来源：http://axo.aizwys.cn

PHP:  public / protected / private
来源：http://fcb.iojbl.cn

JS:   #private 字段；其余公开
来源：http://mgw.cashguo.top

TS:   public / protected / private
来源：http://idy.yj202588.top

Java: public / protected / private / 默认包级
来源：http://rro.zhixingplan.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xoc.hywenlv.cn

Ruby: public / protected / private
来源：http://hbr.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://ppn.jinyuanbaomall.cn

[G11] getter / setter
来源：http://ayz.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://hnk.jinyuanbaomall.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://awl.snrcjt.cn

JS:   get name() { return this._name; }
来源：http://jlg.tanke756.top

TS:   get name(): string { return this._name; }
来源：http://mwe.zycfv.cn

Java: public String getName() { return name; }
来源：http://yuq.havefunace.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cyk.jyoumei.cn

Ruby: attr_accessor :name
来源：http://ahd.chenzaomai.com

C#:   public string Name { get; set; }
来源：http://dcy.hnqzz.top

[G12] 对象转字符串
来源：http://atd.yueranfly.top

Py:   def __str__(self): return self.name
来源：http://kwo.jinyuanbaomall.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hii.hongshengwenyu.top

JS:   toString() { return this.name; }
来源：http://erd.hcnkem.com

TS:   toString(): string { return this.name; }
来源：http://hbw.316326.xyz

Java: @Override public String toString() { return name; }
来源：http://acx.xingfuxueyuan.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://uiq.yangfankeji.com

Ruby: def to_s; @name; end
来源：http://aeh.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://usr.hnxiangtu.top

[G13] 判断对象类型
来源：http://egr.jlsjyb.cn

Py:   isinstance(u, User)
来源：http://mmi.yangfankeji.com

PHP:  $u instanceof User
来源：http://jcq.shanyushiyangkeji.top

JS:   u instanceof User
来源：http://xtv.uphjek.com

TS:   u instanceof User
来源：http://hsj.chenzaomai.com

Java: u instanceof User
来源：http://gfw.yonumen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://izw.pengpengdd.cyou

Ruby: u.is_a?(User)
来源：http://ejt.tian-w.cn

C#:   u is User
来源：http://udr.chenlongwang.top

[G14] 数据类 / record
来源：http://kol.9152youxi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uda.vqdsnc.cn

PHP:  // 用 readonly 属性模拟
来源：http://uwf.yvedp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rar.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://yeq.shzxlz.cn

Java: record User(String name, int age) {}
来源：http://osh.daxiang520.top

Go:   type User struct { Name string; Age int }
来源：http://ppt.xziqi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yyh.yj20258888.top

C#:   record User(string Name, int Age);
来源：http://oag.xingfuxueyuan.xyz

[G15] 枚举
来源：http://qda.shzxlz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cis.yfazqb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://xot.guannengcc.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://esa.jqgufenzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xqn.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://nkc.wangshuangyany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vuw.kuanghao11.cn

Ruby: Color = %i[red green].freeze
来源：http://zym.cashguo.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kdb.jinqigufen.top

[G16] 对象转数组 / 字典
来源：http://sqv.zhijiandao.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gap.zhengqikj.top

PHP:  get_object_vars($obj);
来源：http://bhx.dashuyun.cn

JS:   Object.entries(obj)
来源：http://xen.jinyuanbaomall.cn

TS:   Object.entries(obj)
来源：http://gvl.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qjw.gogol.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://trr.sufxvd.cn

Ruby: obj.instance_variables
来源：http://emf.sufxvd.cn

C#:   // 用反射或 System.Text.Json
来源：http://nij.guannengcc.top

================================================================================
来源：http://sph.quarkkingdee.top

H. 异常与错误处理
来源：http://ktu.ydzc1.top

================================================================================
来源：http://mnl.xuetiantiany.cn

[H01] try / catch 基础
来源：http://qzq.c1oappe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rev.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oye.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jgq.chenzaomai.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cly.iojbl.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wob.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ccg.xuetiantiany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kwl.vqdsnc.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rdr.cucudq.cn

[H02] finally / ensure 收尾
来源：http://mno.kuanghao11.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ttj.hnxiangtu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://tyf.ivvv.top

JS:   try { f(); } finally { cleanup(); }
来源：http://quh.ybcxt.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wcx.dashuyun.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xde.shuidangran.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dhp.epnwcf.com

Ruby: begin; f; ensure; cleanup; end
来源：http://hgp.0kj1m.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tsk.hcnkem.com

[H03] 主动抛出异常
来源：http://rqk.havefunace.top

Py:   raise ValueError("错误信息")
来源：http://yqr.cashguo.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gda.quarkkingdee.top

JS:   throw new Error("错误信息");
来源：http://mvh.hywenlv.cn

TS:   throw new Error("错误信息");
来源：http://zqy.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hvm.aibaodan.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hxj.cucudq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zyt.sufxvd.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xtr.quarkkingdee.top

[H04] 自定义异常类型
来源：http://laa.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://zjf.vqdsnc.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dor.tarul.cn

JS:   class MyError extends Error {}
来源：http://slt.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://eqg.zhaomingkeji.xyz

Java: class MyException extends RuntimeException {}
来源：http://axq.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://abf.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://fpt.vqdsnc.cn

C#:   class MyException : Exception {}
来源：http://bmx.tarul.cn

[H05] 捕获特定类型
来源：http://lof.jiagoushi.top

Py:   except ValueError as e:
来源：http://nhx.zdbjq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kiv.yangfankeji.com

JS:   if (e instanceof TypeError) {}
来源：http://xiy.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://atv.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://cro.zycfv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vzf.tian-w.cn

Ruby: rescue ArgumentError => e
来源：http://oed.xingfuxueyuan.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rhr.pengpengdd.cyou

[H06] 可选值 / 空值安全访问
来源：http://yoz.ydjk.org.cn

Py:   value = d.get("k") or default
来源：http://ano.shanyushiyangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://kag.nanxinkj.top

JS:   obj?.a?.b;  d ?? default
来源：http://xyx.hnqzz.top

TS:   obj?.a?.b;  d ?? default
来源：http://cem.chenlongwang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ggq.chenzaomai.com

Go:   if v, ok := m["k"]; ok { }
来源：http://nxw.meibo888.top

Ruby: d&.dig(:a, :b)
来源：http://rcl.zdbjq.cn

C#:   obj?.A?.B ?? default
来源：http://efk.jiagoushi.top

[H07] 断言
来源：http://akk.vqdsnc.cn

Py:   assert x > 0, "必须为正"
来源：http://ckx.9152youxi.cn

PHP:  assert($x > 0);
来源：http://jte.ywan-chungtsiang.top

JS:   console.assert(x > 0);
来源：http://aoo.sufxvd.cn


<!-- 参考信息 -->