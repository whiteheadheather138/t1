代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hym.chenzaomai.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hfp.zhengqikj.top

[F03] 写入文件（覆盖）
来源：http://hke.c1oappe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aqd.pycfn.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://sjx.birdmap.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ovi.daxiang520.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kxi.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uip.gzhubu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lem.hywenlv.cn

Ruby: File.write("a.txt", "hi")
来源：http://ron.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sqk.ydjk.org.cn

[F04] 追加写入文件
来源：http://znm.yvedp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ddn.9152youxi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zux.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ppp.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wcm.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ryg.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://plj.ydzc1.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aix.guannengcc.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xft.gotoacloud.top

[F05] 判断文件或目录是否存在
来源：http://fwf.hesvh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://drx.sweek.top

PHP:  file_exists("a.txt");
来源：http://rta.guowangkeji.top

JS:   fs.existsSync("a.txt")
来源：http://uyk.nanxuanxn.top

TS:   fs.existsSync("a.txt")
来源：http://szn.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xfo.kuanghao11.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ysl.fktsv.cn

Ruby: File.exist?("a.txt")
来源：http://qqo.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://jzw.cdnleiting.top

[F06] 删除文件
来源：http://bsf.xylfe.cn

Py:   os.remove("a.txt")
来源：http://fxn.hesvh.cn

PHP:  unlink("a.txt");
来源：http://pta.yvedp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vjb.hnxiangtu.top

TS:   fs.unlinkSync("a.txt")
来源：http://xtw.sweek.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hdr.bjfxy.top

Go:   os.Remove("a.txt")
来源：http://huo.iojbl.cn

Ruby: File.delete("a.txt")
来源：http://qrg.yueranfly.top

C#:   File.Delete("a.txt");
来源：http://bol.jiagoushi.top

[F07] 创建目录（含多级）
来源：http://yra.fanxiaobao.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zcy.tian-w.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://agd.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ady.xinyue.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ttb.zhijiandao.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://shh.jinyuanbaomall.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://evc.chenzaomai.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://srz.xingfuxueyuan.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aot.sxryk.cn

[F08] 遍历目录
来源：http://myi.chenjidiqi.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://bux.ydzc1.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hdk.yongpay.top

JS:   fs.readdirSync("dir")
来源：http://uym.cheryme.top

TS:   fs.readdirSync("dir")
来源：http://zhs.cdnleiting.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bkt.hywenlv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://iqx.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://iwm.zhaomingkeji.xyz

C#:   Directory.GetFiles("dir")
来源：http://ypf.jqgufenzy.top

[F09] 获取文件大小
来源：http://qsc.meibo888.top

Py:   os.path.getsize("a.txt")
来源：http://knp.cdnleiting.top

PHP:  filesize("a.txt");
来源：http://rwx.0kj1m.cn

JS:   fs.statSync("a.txt").size
来源：http://wbb.xylfe.cn

TS:   fs.statSync("a.txt").size
来源：http://mmb.yuanzhike.top

Java: Files.size(Path.of("a.txt"))
来源：http://mph.yj20258.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://grx.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://eqg.gotoacloud.top

C#:   new FileInfo("a.txt").Length
来源：http://fsr.guowangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://dlm.jinyuanbaomall.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bpp.ppjwa.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xjk.yonumen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xwy.epnwcf.com

TS:   path.extname("a.txt")
来源：http://wfp.redwolf501.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vwp.sjlbkw.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hnj.ybcxt.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ztc.uphjek.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sxy.hfpthk.cn

[F11] 复制与移动文件
来源：http://erv.dashuyun.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ozt.hammf.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dvh.birdmap.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kjh.xingfuxueyuan.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yja.ivvv.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hjs.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gxr.ydzc1.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qmb.cashguo.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kwl.xziqi.cn

[F12] CSV 读写
来源：http://ldb.daxiang520.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mxp.zhongyouzk.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bcv.zhengqikj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yig.zhijiandao.cn

TS:   // 同上
来源：http://itj.daxiang520.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pix.xziqi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jfq.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pho.fzhhl.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mig.fzhhl.top

================================================================================
来源：http://srm.xingfuxueyuan.xyz

G. 面向对象
来源：http://opx.andypj.xyz

================================================================================
来源：http://mvt.nanxinkj.top

[G01] 定义类
来源：http://jbg.gogol.net.cn

Py:   class User: pass
来源：http://goi.epnwcf.com

PHP:  class User {}
来源：http://okx.cqqwz.cn

JS:   class User {}
来源：http://ssq.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://vtf.hesvh.cn

Java: class User {}
来源：http://qzb.epnwcf.com

Go:   type User struct { Name string }
来源：http://gmg.shanyushiyangtech.top

Ruby: class User; end
来源：http://jmv.ywan-chungtsiang.top

C#:   class User {}
来源：http://nii.jinghuilouyu.cn

[G02] 构造函数
来源：http://wpk.daria6918.cn

Py:   def __init__(self, name): self.name = name
来源：http://els.feifeiyinyue.top

PHP:  public function __construct(public string $name) {}
来源：http://etf.kuanghao11.cn

JS:   constructor(name) { this.name = name; }
来源：http://rpx.xziqi.cn

TS:   constructor(public name: string) {}
来源：http://nof.havefunace.top

Java: User(String name) { this.name = name; }
来源：http://kob.hysaishi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://odj.yj20258.top

Ruby: def initialize(name); @name = name; end
来源：http://pvj.52xcode.cn

C#:   public User(string name) { Name = name; }
来源：http://ito.hfpthk.cn

[G03] 实例属性
来源：http://pua.cashguo.top

Py:   self.name = "x"
来源：http://weq.bjfxy.top

PHP:  public string $name = "x";
来源：http://bli.sxryk.cn

JS:   this.name = "x";
来源：http://far.tarul.cn

TS:   name: string = "x";
来源：http://ngt.hysaishi.cn

Java: private String name;
来源：http://rlr.52xcode.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gyu.gogol.net.cn

Ruby: @name = "x"
来源：http://flv.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://tzf.cashguo.top

[G04] 定义方法
来源：http://huk.guowangkeji.top

Py:   def greet(self): return self.name
来源：http://oks.uphjek.com

PHP:  public function greet(): string { return $this->name; }
来源：http://gws.vqdsnc.cn

JS:   greet() { return this.name; }
来源：http://ifp.hnxiangtu.top

TS:   greet(): string { return this.name; }
来源：http://ody.yuxming.cn

Java: String greet() { return name; }
来源：http://tkk.shanyushiyangtech.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vcl.9152youxi.cn

Ruby: def greet; @name; end
来源：http://exa.fktsv.cn

C#:   public string Greet() => Name;
来源：http://fzn.xinyue.icu

[G05] 继承
来源：http://but.316326.xyz

Py:   class Admin(User): pass
来源：http://pfn.zhaomingkeji.xyz

PHP:  class Admin extends User {}
来源：http://hwo.hcnkem.com

JS:   class Admin extends User {}
来源：http://vft.hysaishi.cn

TS:   class Admin extends User {}
来源：http://jsz.jinqigfzy.top

Java: class Admin extends User {}
来源：http://naw.sysykeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kti.nanxuanxn.top

Ruby: class Admin < User; end
来源：http://jte.jinqigfzy.top

C#:   class Admin : User {}
来源：http://sre.bjfxy.top

[G06] 重写方法
来源：http://aca.yongpay.top

Py:   def greet(self): return "admin"
来源：http://qkh.nanxinkj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tmq.9152youxi.cn

JS:   greet() { return "admin"; }
来源：http://fvs.cashguo.top

TS:   greet(): string { return "admin"; }
来源：http://nnh.shanyushiyangtech.top

Java: @Override String greet() { return "admin"; }
来源：http://tyl.yuxming.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pza.fehbvm.com

Ruby: def greet; "admin"; end
来源：http://xbu.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://epr.wangdashe.top

[G07] 调用父类方法
来源：http://ydq.shuidangran.top

Py:   super().greet()
来源：http://xmi.iojbl.cn

PHP:  parent::greet();
来源：http://nbi.redwolf501.top

JS:   super.greet();
来源：http://vbs.sysykeji.top

TS:   super.greet();
来源：http://ghk.nanxinkj.top

Java: super.greet();
来源：http://cni.andypj.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ham.tanke756.top

Ruby: super
来源：http://dhh.zhijiandao.cn

C#:   base.Greet();
来源：http://hsv.redwolf501.top

[G08] 静态方法与属性
来源：http://qbr.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://opg.xuetiantiany.cn

PHP:  public static function f() {}
来源：http://tjq.cheryme.top

JS:   static f() {}
来源：http://rfn.shanyushiyangkeji.top

TS:   static f(): void {}
来源：http://jme.yangfankeji.com

Java: static void f() {}
来源：http://tua.zhixingplan.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xkz.snrcjt.cn

Ruby: def self.f; end
来源：http://dbs.shanyushiyangtech.top

C#:   public static void F() {}
来源：http://kyc.jinghuilouyu.cn

[G09] 接口 / 抽象类
来源：http://ofe.snrcjt.cn

Py:   from abc import ABC, abstractmethod
来源：http://byt.sxryk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://auy.jyoumei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://upd.haohaochexian.top

TS:   interface Shape { area(): number; }
来源：http://fha.hnqzz.top

Java: interface Shape { double area(); }
来源：http://qpj.shanyushiyangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://ern.cashguo.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cqr.zhaomingkeji.xyz

C#:   interface IShape { double Area(); }
来源：http://wuu.kuanghao11.cn

[G10] 访问控制
来源：http://chk.pengpengdd.cyou

Py:   约定 _protected / __private（不强制）
来源：http://eav.shanyushiyangkeji.top

PHP:  public / protected / private
来源：http://hmr.zdbjq.cn

JS:   #private 字段；其余公开
来源：http://lsz.dianchejie.cn

TS:   public / protected / private
来源：http://qug.sxryk.cn

Java: public / protected / private / 默认包级
来源：http://lkx.aibaodan.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://uvd.bbcook.cn

Ruby: public / protected / private
来源：http://agn.jlsjyb.cn

C#:   public / protected / private / internal
来源：http://nbn.ppjwa.cn

[G11] getter / setter
来源：http://rns.jiagoushi.top

Py:   @property 与 @x.setter
来源：http://hyn.zhixingplan.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cta.nanxinkj.top

JS:   get name() { return this._name; }
来源：http://kqm.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://ena.yangfankeji.com

Java: public String getName() { return name; }
来源：http://ypm.pycfn.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://pkj.yuxming.cn

Ruby: attr_accessor :name
来源：http://izc.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://gdu.nwbrower.top

[G12] 对象转字符串
来源：http://afr.shanyushiyangtech.top

Py:   def __str__(self): return self.name
来源：http://zgn.cdnleiting.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://emc.ctjpmb.com

JS:   toString() { return this.name; }
来源：http://wax.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://xeh.yj20258888.top

Java: @Override public String toString() { return name; }
来源：http://kdw.fehbvm.com

Go:   func (u User) String() string { return u.Name }
来源：http://swj.sjlbkw.cn

Ruby: def to_s; @name; end
来源：http://mcj.shzxlz.cn

C#:   public override string ToString() => Name;
来源：http://blb.dashuyun.cn

[G13] 判断对象类型
来源：http://pxr.c1oappe.top

Py:   isinstance(u, User)
来源：http://mrg.9152youxi.cn

PHP:  $u instanceof User
来源：http://pku.52xcode.cn

JS:   u instanceof User
来源：http://bvn.sufxvd.cn

TS:   u instanceof User
来源：http://xuh.shanyushiyangtech.top

Java: u instanceof User
来源：http://gfs.jlsjyb.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kie.jqgfzy.top

Ruby: u.is_a?(User)
来源：http://vgj.aibaodan.cn

C#:   u is User
来源：http://fmk.hnxiangtu.top

[G14] 数据类 / record
来源：http://ggy.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zno.cqqwz.cn

PHP:  // 用 readonly 属性模拟
来源：http://dgt.fzhhl.top

JS:   // 无内置：普通类或对象字面量
来源：http://vvc.smart0.xyz

TS:   type User = { name: string; age: number };
来源：http://ktm.hnqzz.top

Java: record User(String name, int age) {}
来源：http://mfo.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://nqs.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gks.daria6918.cn

C#:   record User(string Name, int Age);
来源：http://izn.jlsjyb.cn

[G15] 枚举
来源：http://frz.yvedp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gyq.jiagoushi.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zsa.cqqwz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qyu.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qks.wangdashe.top

Java: enum Color { RED, GREEN }
来源：http://nds.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cot.hongshengwenyu.top

Ruby: Color = %i[red green].freeze
来源：http://xjw.cashguo.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vry.ivvv.top

[G16] 对象转数组 / 字典
来源：http://ajj.jyoumei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nic.dashuyun.cn

PHP:  get_object_vars($obj);
来源：http://pbv.zhaomingkeji.xyz

JS:   Object.entries(obj)
来源：http://wnx.jqgfzy.top

TS:   Object.entries(obj)
来源：http://gyj.jinqigfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fra.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://paq.iojbl.cn

Ruby: obj.instance_variables
来源：http://smg.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://iyz.tian-w.cn

================================================================================
来源：http://fnn.sweek.top

H. 异常与错误处理
来源：http://xeu.ydzc1.top

================================================================================
来源：http://prg.quarkkingdee.top

[H01] try / catch 基础
来源：http://kmd.pycfn.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wfm.ydzc1.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lys.quarkkingdee.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mic.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://alg.yueranfly.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sey.hcnkem.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mqv.xziqi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bhv.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rcr.quarkkingdee.top

[H02] finally / ensure 收尾
来源：http://axy.zhiwuduotai.top

Py:   try: f()⏎finally: cleanup()
来源：http://tih.xingfuxueyuan.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://rbh.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://wmj.gaohongyu789.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yxn.zycfv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://aqa.chenjidiqi.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://rpu.yfazqb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://pwg.svipenyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://thc.feifeiyinyue.top

[H03] 主动抛出异常
来源：http://nsd.yuxming.cn

Py:   raise ValueError("错误信息")
来源：http://nyj.andypj.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rsh.vehdjk.com

JS:   throw new Error("错误信息");
来源：http://dul.guannengcc.top

TS:   throw new Error("错误信息");
来源：http://sag.zhoulong.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://odj.mhx1999.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xme.yuxming.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lyo.jqgfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://mif.jianghu66.top

[H04] 自定义异常类型
来源：http://fui.zdbjq.cn

Py:   class MyError(Exception): pass
来源：http://biy.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://ufo.feifeiyinyue.top

JS:   class MyError extends Error {}
来源：http://cul.cdnleiting.top

TS:   class MyError extends Error {}
来源：http://cqk.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://vqt.kuanghao11.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xtk.dianchejie.cn

Ruby: class MyError < StandardError; end
来源：http://nva.hcnkem.com

C#:   class MyException : Exception {}
来源：http://amm.andypj.xyz

[H05] 捕获特定类型
来源：http://bsw.yuanzhike.top

Py:   except ValueError as e:
来源：http://vvb.dashuyun.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xwb.yvedp.cn

JS:   if (e instanceof TypeError) {}
来源：http://bgy.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://xgw.cashguo.top

Java: catch (IOException | SQLException e) {}
来源：http://fvq.yuanzhike.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qma.hammf.cn

Ruby: rescue ArgumentError => e
来源：http://vmj.ybcxt.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vok.tian-w.cn

[H06] 可选值 / 空值安全访问
来源：http://eji.cdnleiting.top

Py:   value = d.get("k") or default
来源：http://xlg.tarul.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bef.sxryk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yhz.jlsjyb.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dhy.aibaodan.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gvi.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://usn.yfazqb.com

Ruby: d&.dig(:a, :b)
来源：http://yml.zhengqikj.top

C#:   obj?.A?.B ?? default
来源：http://lft.zycfv.cn

[H07] 断言
来源：http://kob.zhixingplan.top

Py:   assert x > 0, "必须为正"
来源：http://rdi.tian-w.cn

PHP:  assert($x > 0);
来源：http://wqt.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://gzv.tanke756.top


<!-- 参考信息 -->