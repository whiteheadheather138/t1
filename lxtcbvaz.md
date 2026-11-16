代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ece.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kqx.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uth.jiagoushi.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://umt.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://btz.zhiwuduotai.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mhi.pengpengdd.cyou

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bez.yvedp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fru.shuidangran.top

[F05] 判断文件或目录是否存在
来源：http://gvf.smart0.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uom.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://zuo.fzhhl.top

JS:   fs.existsSync("a.txt")
来源：http://ukn.jinqigufen.top

TS:   fs.existsSync("a.txt")
来源：http://zwy.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bwk.0kj1m.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://off.jqgfzy.top

Ruby: File.exist?("a.txt")
来源：http://kbg.feifeiyinyue.top

C#:   File.Exists("a.txt")
来源：http://wao.haohaochexian.top

[F06] 删除文件
来源：http://dbw.xziqi.cn

Py:   os.remove("a.txt")
来源：http://haj.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://dbl.sjlbkw.cn

JS:   fs.unlinkSync("a.txt")
来源：http://igs.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://jxt.nwbrower.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zqp.dashuyun.cn

Go:   os.Remove("a.txt")
来源：http://znb.yongpay.top

Ruby: File.delete("a.txt")
来源：http://snp.smart0.xyz

C#:   File.Delete("a.txt");
来源：http://yqm.jinghuilouyu.cn

[F07] 创建目录（含多级）
来源：http://znx.dashuyun.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yat.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fmn.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lei.birdmap.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ndp.yanxiufei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://znn.pycfn.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vpc.tian-w.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qxi.wangdashe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jwj.9152youxi.cn

[F08] 遍历目录
来源：http://mcw.havefunace.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kwt.ivvv.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yyk.shangyingyoupin.top

JS:   fs.readdirSync("dir")
来源：http://wad.cdnleiting.top

TS:   fs.readdirSync("dir")
来源：http://gaf.zhoulong.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://plp.vqdsnc.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vfv.c1oappe.top

Ruby: Dir.children("dir")
来源：http://mrm.yj20258888.top

C#:   Directory.GetFiles("dir")
来源：http://fdg.cqqwz.cn

[F09] 获取文件大小
来源：http://kac.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://vuo.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://jmv.c1oappe.top

JS:   fs.statSync("a.txt").size
来源：http://ezg.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://kyd.zhixingplan.top

Java: Files.size(Path.of("a.txt"))
来源：http://rou.nanxinkj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lcy.fktsv.cn

Ruby: File.size("a.txt")
来源：http://qit.gotoacloud.top

C#:   new FileInfo("a.txt").Length
来源：http://omm.316326.xyz

[F10] 取文件扩展名 / 文件名
来源：http://vqr.xuanzx.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jhz.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bjm.ywan-chungtsiang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fyg.feifeiyinyue.top

TS:   path.extname("a.txt")
来源：http://cyz.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dzc.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uzn.gogol.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tfk.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://laz.yangfankeji.com

[F11] 复制与移动文件
来源：http://mbp.chenlongwang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zky.sjlbkw.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fue.zhiwuduotai.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vvn.yj20258888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ffn.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lum.gotoacloud.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jqo.nanxuanxn.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uyz.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cbd.vehdjk.com

[F12] CSV 读写
来源：http://ren.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://khg.fzhhl.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jwd.xuanzx.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zfm.pycfn.com

TS:   // 同上
来源：http://vkk.zdbjq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iyn.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rtp.daria6918.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://asb.yonumen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ubp.sufxvd.cn

================================================================================
来源：http://lbs.nanxuanxn.top

G. 面向对象
来源：http://wce.hcnkem.com

================================================================================
来源：http://qeb.cashguo.top

[G01] 定义类
来源：http://cwg.xziqi.cn

Py:   class User: pass
来源：http://pua.zhiwuduotai.top

PHP:  class User {}
来源：http://fsq.jinqigfzy.top

JS:   class User {}
来源：http://gmw.fanxiaobao.xyz

TS:   class User { name: string = ""; }
来源：http://yqt.cucudq.cn

Java: class User {}
来源：http://rim.andypj.xyz

Go:   type User struct { Name string }
来源：http://rxh.hysaishi.cn

Ruby: class User; end
来源：http://keo.guannengcc.top

C#:   class User {}
来源：http://jfp.epnwcf.com

[G02] 构造函数
来源：http://tkn.zhongyouzk.top

Py:   def __init__(self, name): self.name = name
来源：http://iid.ydjk.org.cn

PHP:  public function __construct(public string $name) {}
来源：http://nzf.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://joh.iojbl.cn

TS:   constructor(public name: string) {}
来源：http://dsr.xylfe.cn

Java: User(String name) { this.name = name; }
来源：http://zlx.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rxn.jinghuilouyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://czn.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://moh.daxiang520.top

[G03] 实例属性
来源：http://jdb.fzhhl.top

Py:   self.name = "x"
来源：http://peg.uphjek.com

PHP:  public string $name = "x";
来源：http://zqp.zhengqikj.top

JS:   this.name = "x";
来源：http://idp.nanxinkj.top

TS:   name: string = "x";
来源：http://poi.0kj1m.cn

Java: private String name;
来源：http://xzf.52xcode.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tlf.svipenyu.cn

Ruby: @name = "x"
来源：http://fvt.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://zup.gzhubu.top

[G04] 定义方法
来源：http://nmn.aibaodan.cn

Py:   def greet(self): return self.name
来源：http://gar.snrcjt.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ryv.hongshengwenyu.top

JS:   greet() { return this.name; }
来源：http://hjp.vqdsnc.cn

TS:   greet(): string { return this.name; }
来源：http://bja.hongshengwenyu.top

Java: String greet() { return name; }
来源：http://geo.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://vdp.xylfe.cn

Ruby: def greet; @name; end
来源：http://yeo.epnwcf.com

C#:   public string Greet() => Name;
来源：http://uqn.xuetiantiany.cn

[G05] 继承
来源：http://rdp.jinyuanbaomall.cn

Py:   class Admin(User): pass
来源：http://wzw.fengsongda.top

PHP:  class Admin extends User {}
来源：http://tci.zhengqikj.top

JS:   class Admin extends User {}
来源：http://sqt.hcnkem.com

TS:   class Admin extends User {}
来源：http://uyw.chenlongwang.top

Java: class Admin extends User {}
来源：http://cje.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rjm.zdbjq.cn

Ruby: class Admin < User; end
来源：http://zom.tian-w.cn

C#:   class Admin : User {}
来源：http://tyr.0kj1m.cn

[G06] 重写方法
来源：http://scp.ivvv.top

Py:   def greet(self): return "admin"
来源：http://cwx.xylfe.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gly.zhijiandao.cn

JS:   greet() { return "admin"; }
来源：http://uyi.gotoacloud.top

TS:   greet(): string { return "admin"; }
来源：http://rtj.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://pcq.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iux.jiagoushi.top

Ruby: def greet; "admin"; end
来源：http://cvm.gzhubu.top

C#:   public override string Greet() => "admin";
来源：http://rtw.tianlin.xyz

[G07] 调用父类方法
来源：http://mjx.hcnkem.com

Py:   super().greet()
来源：http://dwl.havefunace.top

PHP:  parent::greet();
来源：http://nha.epnwcf.com

JS:   super.greet();
来源：http://sdr.birdmap.top

TS:   super.greet();
来源：http://oil.shzxlz.cn

Java: super.greet();
来源：http://aks.yvedp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hwt.tanke756.top

Ruby: super
来源：http://vzp.jinqigufen.top

C#:   base.Greet();
来源：http://ned.wangshuangyany.cn

[G08] 静态方法与属性
来源：http://kzp.9152youxi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yhf.bjfxy.top

PHP:  public static function f() {}
来源：http://poe.yj20258888.top

JS:   static f() {}
来源：http://xiy.ydzc1.top

TS:   static f(): void {}
来源：http://nks.iojbl.cn

Java: static void f() {}
来源：http://guq.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://yvm.shangyingyoupin.top

Ruby: def self.f; end
来源：http://oow.bjfxy.top

C#:   public static void F() {}
来源：http://jcx.zycfv.cn

[G09] 接口 / 抽象类
来源：http://kmi.yj202588.top

Py:   from abc import ABC, abstractmethod
来源：http://qkg.pycfn.com

PHP:  interface Shape { public function area(): float; }
来源：http://ekj.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xgs.yfazqb.com

TS:   interface Shape { area(): number; }
来源：http://hgl.ehwqpu.com

Java: interface Shape { double area(); }
来源：http://hzp.haohaochexian.top

Go:   type Shape interface { Area() float64 }
来源：http://ant.birdmap.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dfu.cdnleiting.top

C#:   interface IShape { double Area(); }
来源：http://rqb.jinghuilouyu.cn

[G10] 访问控制
来源：http://ian.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://gms.feifeiyinyue.top

PHP:  public / protected / private
来源：http://wtl.jiagoushi.top

JS:   #private 字段；其余公开
来源：http://cko.shzxlz.cn

TS:   public / protected / private
来源：http://kyt.dashuyun.cn

Java: public / protected / private / 默认包级
来源：http://sza.redwolf501.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://skj.chenjidiqi.icu

Ruby: public / protected / private
来源：http://mvw.havefunace.top

C#:   public / protected / private / internal
来源：http://brg.shanyushiyangtech.top

[G11] getter / setter
来源：http://uie.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://pnf.yj202588.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tyc.meibo888.top

JS:   get name() { return this._name; }
来源：http://nml.jqgufenzy.top

TS:   get name(): string { return this._name; }
来源：http://vir.zhiwuduotai.top

Java: public String getName() { return name; }
来源：http://frl.hywenlv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://umn.tian-w.cn

Ruby: attr_accessor :name
来源：http://jbu.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://mdb.ydzc1.top

[G12] 对象转字符串
来源：http://imh.ehwqpu.com

Py:   def __str__(self): return self.name
来源：http://huc.havefunace.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pcn.shangyingyoupin.top

JS:   toString() { return this.name; }
来源：http://azi.jinqigfzy.top

TS:   toString(): string { return this.name; }
来源：http://ner.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://wdl.ctjpmb.com

Go:   func (u User) String() string { return u.Name }
来源：http://dmf.ydzc1.top

Ruby: def to_s; @name; end
来源：http://cyl.hongshengwenyu.top

C#:   public override string ToString() => Name;
来源：http://xhz.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://upf.ctjpmb.com

Py:   isinstance(u, User)
来源：http://pah.hongshengwenyu.top

PHP:  $u instanceof User
来源：http://npm.xuanzx.com

JS:   u instanceof User
来源：http://cys.wangdashe.top

TS:   u instanceof User
来源：http://djx.iojbl.cn

Java: u instanceof User
来源：http://qup.cashguo.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://aks.feifeiyinyue.top

Ruby: u.is_a?(User)
来源：http://gxp.hammf.cn

C#:   u is User
来源：http://gmd.jqgufenzy.top

[G14] 数据类 / record
来源：http://xgt.ivvv.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bwd.chenjidiqi.icu

PHP:  // 用 readonly 属性模拟
来源：http://utx.tanke756.top

JS:   // 无内置：普通类或对象字面量
来源：http://qpq.bjfxy.top

TS:   type User = { name: string; age: number };
来源：http://jgy.hesvh.cn

Java: record User(String name, int age) {}
来源：http://htm.yongpay.top

Go:   type User struct { Name string; Age int }
来源：http://hib.pengpengdd.cyou

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xfp.gogol.net.cn

C#:   record User(string Name, int Age);
来源：http://wom.yfazqb.com

[G15] 枚举
来源：http://gji.hongshengwenyu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gfg.0kj1m.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://okk.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xng.jinqigfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://atf.sjlbkw.cn

Java: enum Color { RED, GREEN }
来源：http://dto.feifeiyinyue.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vrd.zhoulong.xyz

Ruby: Color = %i[red green].freeze
来源：http://wqm.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fxq.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://gpo.sufxvd.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bzr.yuanzhike.top

PHP:  get_object_vars($obj);
来源：http://ixr.hammf.cn

JS:   Object.entries(obj)
来源：http://whv.tarul.cn

TS:   Object.entries(obj)
来源：http://bvs.tian-w.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://efy.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zwg.ywan-chungtsiang.top

Ruby: obj.instance_variables
来源：http://pqx.shanyushiyangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://lrh.ppjwa.cn

================================================================================
来源：http://jgk.0kj1m.cn

H. 异常与错误处理
来源：http://tns.zdbjq.cn

================================================================================
来源：http://euz.wangdashe.top

[H01] try / catch 基础
来源：http://wzh.hysaishi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xrq.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xtf.daxiang520.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ahj.yangfankeji.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sht.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oex.zhengqikj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vre.cucudq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nvj.nwbrower.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qhu.ivvv.top

[H02] finally / ensure 收尾
来源：http://owo.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://kpe.52xcode.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ddt.chenzaomai.com

JS:   try { f(); } finally { cleanup(); }
来源：http://vhr.gaohongyu789.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kln.zdqjudy.top

Java: try { f(); } finally { cleanup(); }
来源：http://idg.pengpengdd.cyou

Go:   defer cleanup()             // 函数返回时执行
来源：http://bim.jinqigfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://iiu.mhx1999.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://muc.shuidangran.top

[H03] 主动抛出异常
来源：http://rae.hysaishi.cn

Py:   raise ValueError("错误信息")
来源：http://bhr.fehbvm.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xbv.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://gwh.hywenlv.cn

TS:   throw new Error("错误信息");
来源：http://gts.ybcxt.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dlb.sysykeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mlx.hnxiangtu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mnk.hesvh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://blk.zdqjudy.top

[H04] 自定义异常类型
来源：http://snf.birdmap.top

Py:   class MyError(Exception): pass
来源：http://vuq.shuidangran.top

PHP:  class MyError extends RuntimeException {}
来源：http://znf.yj20258.top

JS:   class MyError extends Error {}
来源：http://hue.zycfv.cn

TS:   class MyError extends Error {}
来源：http://nmn.fanxiaobao.xyz

Java: class MyException extends RuntimeException {}
来源：http://yre.jinqigufen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pbd.yongpay.top

Ruby: class MyError < StandardError; end
来源：http://aog.zhoulong.xyz

C#:   class MyException : Exception {}
来源：http://ijg.hywenlv.cn

[H05] 捕获特定类型
来源：http://fhv.guannengcc.top

Py:   except ValueError as e:
来源：http://hmt.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rmn.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://wuz.sysykeji.top

TS:   if (e instanceof TypeError) {}
来源：http://hji.9152youxi.cn

Java: catch (IOException | SQLException e) {}
来源：http://gsq.aibaodan.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xnn.hfpthk.cn

Ruby: rescue ArgumentError => e
来源：http://qms.hnqzz.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hlo.xuetiantiany.cn

[H06] 可选值 / 空值安全访问
来源：http://ako.ctjpmb.com

Py:   value = d.get("k") or default
来源：http://hcq.fengsongda.top

PHP:  $v = $d["k"] ?? null;
来源：http://ieg.vehdjk.com

JS:   obj?.a?.b;  d ?? default
来源：http://hiq.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://uhn.zycfv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xuz.sxryk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://imn.jinghuilouyu.cn

Ruby: d&.dig(:a, :b)
来源：http://itx.zdbjq.cn

C#:   obj?.A?.B ?? default
来源：http://qpt.fanxiaobao.xyz

[H07] 断言
来源：http://cmq.yuanzhike.top

Py:   assert x > 0, "必须为正"
来源：http://mvk.shzxlz.cn

PHP:  assert($x > 0);
来源：http://zzo.jiagoushi.top

JS:   console.assert(x > 0);
来源：http://mwe.hongshengwenyu.top

TS:   console.assert(x > 0);
来源：http://tbt.jiagoushi.top

Java: assert x > 0 : "必须为正";
来源：http://wih.xylfe.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ctl.jlsjyb.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sxa.dashuyun.cn

C#:   Debug.Assert(x > 0);
来源：http://hlk.yonumen.top

[H08] 获取错误信息与堆栈
来源：http://wjo.hongshengwenyu.top

Py:   str(e);  traceback.format_exc()
来源：http://wus.chenzaomai.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hqb.ydzc1.top

JS:   e.message;  e.stack
来源：http://obe.birdmap.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jis.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lcd.52xcode.cn

Go:   err.Error()
来源：http://dpz.jinqigufen.top


<!-- 参考信息 -->