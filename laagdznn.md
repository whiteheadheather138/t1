代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://tnf.ywan-chungtsiang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xti.zhengqikj.top

PHP:  file_exists("a.txt");
来源：http://kso.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://mzj.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://gsn.fehbvm.com

Java: Files.exists(Path.of("a.txt"))
来源：http://bnu.daria6918.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tmu.chenzaomai.com

Ruby: File.exist?("a.txt")
来源：http://jrg.dashuyun.cn

C#:   File.Exists("a.txt")
来源：http://dir.redwolf501.top

[F06] 删除文件
来源：http://mua.shanyushiyangkeji.top

Py:   os.remove("a.txt")
来源：http://fbl.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://meg.ivvv.top

JS:   fs.unlinkSync("a.txt")
来源：http://vqu.ywan-chungtsiang.top

TS:   fs.unlinkSync("a.txt")
来源：http://sgv.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mvd.52xcode.cn

Go:   os.Remove("a.txt")
来源：http://tty.ydjk.org.cn

Ruby: File.delete("a.txt")
来源：http://nxr.ppjwa.cn

C#:   File.Delete("a.txt");
来源：http://vtw.yuanzhike.top

[F07] 创建目录（含多级）
来源：http://obm.guowangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dtl.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lnk.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zkt.hongshengwenyu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lha.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wxz.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kfz.yvedp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hhs.yj20258.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jzw.zhongyouzk.top

[F08] 遍历目录
来源：http://ujp.tarul.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lsi.zhongyouzk.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bck.dashuyun.cn

JS:   fs.readdirSync("dir")
来源：http://cai.hnqzz.top

TS:   fs.readdirSync("dir")
来源：http://gea.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sti.smart0.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://xxg.feifeiyinyue.top

Ruby: Dir.children("dir")
来源：http://szo.zdbjq.cn

C#:   Directory.GetFiles("dir")
来源：http://dhl.fehbvm.com

[F09] 获取文件大小
来源：http://rev.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://rot.bbcook.cn

PHP:  filesize("a.txt");
来源：http://wti.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://obo.hammf.cn

TS:   fs.statSync("a.txt").size
来源：http://qak.nanxuanxn.top

Java: Files.size(Path.of("a.txt"))
来源：http://xnu.aizwys.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tfe.316326.xyz

Ruby: File.size("a.txt")
来源：http://xwm.haohaochexian.top

C#:   new FileInfo("a.txt").Length
来源：http://bvk.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://iym.smart0.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nrt.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ksj.birdmap.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://igd.snrcjt.cn

TS:   path.extname("a.txt")
来源：http://vog.316326.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zgh.shangyingyoupin.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lqr.snrcjt.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nqk.aibaodan.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lrs.yueranfly.top

[F11] 复制与移动文件
来源：http://vyp.hesvh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lpi.ehwqpu.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tju.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://luy.yuanzhike.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xvw.yfazqb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cwn.cheryme.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tom.316326.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://erc.xingfuxueyuan.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xtc.hammf.cn

[F12] CSV 读写
来源：http://dlb.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ktg.gogol.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yhh.daxiang520.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lts.ywan-chungtsiang.top

TS:   // 同上
来源：http://rah.meibo888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ywj.cdnleiting.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hrh.cashguo.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ues.snrcjt.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jyo.tian-w.cn

================================================================================
来源：http://qzf.chenlongwang.top

G. 面向对象
来源：http://kzl.ydjk.org.cn

================================================================================
来源：http://waw.hnxiangtu.top

[G01] 定义类
来源：http://skp.ctjpmb.com

Py:   class User: pass
来源：http://sar.daria6918.cn

PHP:  class User {}
来源：http://bvp.zhongyouzk.top

JS:   class User {}
来源：http://hjs.yj202588.top

TS:   class User { name: string = ""; }
来源：http://tvu.nanxuanxn.top

Java: class User {}
来源：http://sdc.ybcxt.top

Go:   type User struct { Name string }
来源：http://nnt.yonumen.top

Ruby: class User; end
来源：http://npt.aibaodan.cn

C#:   class User {}
来源：http://thm.hongshengwenyu.top

[G02] 构造函数
来源：http://uss.jyoumei.cn

Py:   def __init__(self, name): self.name = name
来源：http://eua.daria6918.cn

PHP:  public function __construct(public string $name) {}
来源：http://eer.ppjwa.cn

JS:   constructor(name) { this.name = name; }
来源：http://efu.bjfxy.top

TS:   constructor(public name: string) {}
来源：http://cko.andypj.xyz

Java: User(String name) { this.name = name; }
来源：http://lnl.sysykeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://szz.zdbjq.cn

Ruby: def initialize(name); @name = name; end
来源：http://ccc.c1oappe.top

C#:   public User(string name) { Name = name; }
来源：http://uvn.vqdsnc.cn

[G03] 实例属性
来源：http://wio.ppjwa.cn

Py:   self.name = "x"
来源：http://tvi.sysykeji.top

PHP:  public string $name = "x";
来源：http://vcq.316326.xyz

JS:   this.name = "x";
来源：http://qss.snrcjt.cn

TS:   name: string = "x";
来源：http://cdq.nwbrower.top

Java: private String name;
来源：http://auw.cucudq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dzk.jqgfzy.top

Ruby: @name = "x"
来源：http://won.chenjidiqi.icu

C#:   public string Name { get; set; } = "x";
来源：http://kaj.zdqjudy.top

[G04] 定义方法
来源：http://qmw.andypj.xyz

Py:   def greet(self): return self.name
来源：http://irw.yj20258888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rga.shanyushiyangtech.top

JS:   greet() { return this.name; }
来源：http://bho.ywan-chungtsiang.top

TS:   greet(): string { return this.name; }
来源：http://jcw.yongpay.top

Java: String greet() { return name; }
来源：http://krd.zdbjq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jsj.yuanzhike.top

Ruby: def greet; @name; end
来源：http://had.hcnkem.com

C#:   public string Greet() => Name;
来源：http://ilo.sweek.top

[G05] 继承
来源：http://tax.mhx1999.top

Py:   class Admin(User): pass
来源：http://kue.tianlin.xyz

PHP:  class Admin extends User {}
来源：http://dss.sxryk.cn

JS:   class Admin extends User {}
来源：http://nwk.ywan-chungtsiang.top

TS:   class Admin extends User {}
来源：http://ilj.tian-w.cn

Java: class Admin extends User {}
来源：http://btf.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://alf.snrcjt.cn

Ruby: class Admin < User; end
来源：http://ngm.pycfn.com

C#:   class Admin : User {}
来源：http://sga.hammf.cn

[G06] 重写方法
来源：http://lkg.yongpay.top

Py:   def greet(self): return "admin"
来源：http://zfg.jlsjyb.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sto.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://sxg.hfpthk.cn

TS:   greet(): string { return "admin"; }
来源：http://rhv.xingfuxueyuan.xyz

Java: @Override String greet() { return "admin"; }
来源：http://lco.hesvh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://chh.guannengcc.top

Ruby: def greet; "admin"; end
来源：http://gli.wangdashe.top

C#:   public override string Greet() => "admin";
来源：http://zsz.pycfn.com

[G07] 调用父类方法
来源：http://vfu.ivvv.top

Py:   super().greet()
来源：http://ehi.ivvv.top

PHP:  parent::greet();
来源：http://nsb.hongshengwenyu.top

JS:   super.greet();
来源：http://qnv.c1oappe.top

TS:   super.greet();
来源：http://bev.vehdjk.com

Java: super.greet();
来源：http://tpv.yuxming.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tic.yangfankeji.com

Ruby: super
来源：http://ndh.wangdashe.top

C#:   base.Greet();
来源：http://por.xingfuxueyuan.xyz

[G08] 静态方法与属性
来源：http://pbe.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://stm.ctjpmb.com

PHP:  public static function f() {}
来源：http://heo.pengpengdd.cyou

JS:   static f() {}
来源：http://gfi.hysaishi.cn

TS:   static f(): void {}
来源：http://qwz.hywenlv.cn

Java: static void f() {}
来源：http://cgi.hywenlv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hah.yuxming.cn

Ruby: def self.f; end
来源：http://eqm.ydjk.org.cn

C#:   public static void F() {}
来源：http://zbr.tanke756.top

[G09] 接口 / 抽象类
来源：http://gqy.xziqi.cn

Py:   from abc import ABC, abstractmethod
来源：http://cfo.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://osz.chenjidiqi.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://eyu.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://yxu.zhijiandao.cn

Java: interface Shape { double area(); }
来源：http://ftn.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://vxh.yueranfly.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vex.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://cvf.sjlbkw.cn

[G10] 访问控制
来源：http://rlh.yuanzhike.top

Py:   约定 _protected / __private（不强制）
来源：http://tqz.guowangkeji.top

PHP:  public / protected / private
来源：http://tzs.yongpay.top

JS:   #private 字段；其余公开
来源：http://etj.dianchejie.cn

TS:   public / protected / private
来源：http://cak.vehdjk.com

Java: public / protected / private / 默认包级
来源：http://lvp.hongshengwenyu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://txb.yj202588.top

Ruby: public / protected / private
来源：http://prh.zhongyouzk.top

C#:   public / protected / private / internal
来源：http://fjc.ywan-chungtsiang.top

[G11] getter / setter
来源：http://rki.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://eyy.daria6918.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zub.hnxiangtu.top

JS:   get name() { return this._name; }
来源：http://xyd.jqgfzy.top

TS:   get name(): string { return this._name; }
来源：http://inx.hesvh.cn

Java: public String getName() { return name; }
来源：http://zkp.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pyz.yvedp.cn

Ruby: attr_accessor :name
来源：http://ors.cqqwz.cn

C#:   public string Name { get; set; }
来源：http://avf.shuidangran.top

[G12] 对象转字符串
来源：http://ytf.daxiang520.top

Py:   def __str__(self): return self.name
来源：http://gin.0kj1m.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://eji.cashguo.top

JS:   toString() { return this.name; }
来源：http://ihn.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://yud.jlsjyb.cn

Java: @Override public String toString() { return name; }
来源：http://ywd.hcnkem.com

Go:   func (u User) String() string { return u.Name }
来源：http://zyb.ctjpmb.com

Ruby: def to_s; @name; end
来源：http://yjr.shuidangran.top

C#:   public override string ToString() => Name;
来源：http://qqe.hcnkem.com

[G13] 判断对象类型
来源：http://mbl.daria6918.cn

Py:   isinstance(u, User)
来源：http://tts.9152youxi.cn

PHP:  $u instanceof User
来源：http://axn.shanyushiyangkeji.top

JS:   u instanceof User
来源：http://sud.ybcxt.top

TS:   u instanceof User
来源：http://myg.bbcook.cn

Java: u instanceof User
来源：http://gly.zdqjudy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nmx.jinqigufen.top

Ruby: u.is_a?(User)
来源：http://ndn.ydzc1.top

C#:   u is User
来源：http://hms.ctjpmb.com

[G14] 数据类 / record
来源：http://lfz.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nxl.birdmap.top

PHP:  // 用 readonly 属性模拟
来源：http://bci.hfpthk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dem.tian-w.cn

TS:   type User = { name: string; age: number };
来源：http://gie.sweek.top

Java: record User(String name, int age) {}
来源：http://szi.tian-w.cn

Go:   type User struct { Name string; Age int }
来源：http://kml.jyoumei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lun.tarul.cn

C#:   record User(string Name, int Age);
来源：http://hry.jiagoushi.top

[G15] 枚举
来源：http://fzj.jyoumei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jli.haohaochexian.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://euh.chenlongwang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dyw.mhx1999.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tde.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://jgg.yj202588.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qgz.gzhubu.top

Ruby: Color = %i[red green].freeze
来源：http://hnv.hcnkem.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bva.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://wld.yj20258.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cjm.hfpthk.cn

PHP:  get_object_vars($obj);
来源：http://smq.havefunace.top

JS:   Object.entries(obj)
来源：http://bgs.xinyue.icu

TS:   Object.entries(obj)
来源：http://hbf.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vfo.pengpengdd.cyou

Go:   // 手写转换，或用 mapstructure 库
来源：http://esi.gzhubu.top

Ruby: obj.instance_variables
来源：http://pzs.sjlbkw.cn

C#:   // 用反射或 System.Text.Json
来源：http://rhl.chenjidiqi.icu

================================================================================
来源：http://nhg.jianghu66.top

H. 异常与错误处理
来源：http://pkj.shzxlz.cn

================================================================================
来源：http://svl.316326.xyz

[H01] try / catch 基础
来源：http://ojw.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ewl.vehdjk.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ojr.ydjk.org.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://srj.dianchejie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mqc.daxiang520.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ixg.xingfuxueyuan.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://emd.tarul.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xcm.52xcode.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lxf.fehbvm.com

[H02] finally / ensure 收尾
来源：http://ewk.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://zuv.xingfuxueyuan.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://hnp.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://qce.tianlin.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://jre.nwbrower.top

Java: try { f(); } finally { cleanup(); }
来源：http://voe.fanxiaobao.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://cht.316326.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://ziy.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://lka.birdmap.top

[H03] 主动抛出异常
来源：http://nmi.yj20258.top

Py:   raise ValueError("错误信息")
来源：http://dja.cheryme.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sjx.tian-w.cn

JS:   throw new Error("错误信息");
来源：http://eev.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://aea.vehdjk.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://ibm.ehwqpu.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bxp.zhiwuduotai.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ibe.zdqjudy.top

C#:   throw new ArgumentException("错误信息");
来源：http://oqg.jlsjyb.cn

[H04] 自定义异常类型
来源：http://won.sxryk.cn

Py:   class MyError(Exception): pass
来源：http://jov.sufxvd.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ihz.tian-w.cn

JS:   class MyError extends Error {}
来源：http://jtu.chenlongwang.top

TS:   class MyError extends Error {}
来源：http://iym.cucudq.cn

Java: class MyException extends RuntimeException {}
来源：http://nrq.jinqigufen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ken.vehdjk.com

Ruby: class MyError < StandardError; end
来源：http://qaz.fktsv.cn

C#:   class MyException : Exception {}
来源：http://tzl.ydzc1.top

[H05] 捕获特定类型
来源：http://ubj.nwbrower.top

Py:   except ValueError as e:
来源：http://key.cashguo.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ing.ydjk.org.cn

JS:   if (e instanceof TypeError) {}
来源：http://jwt.daxiang520.top

TS:   if (e instanceof TypeError) {}
来源：http://ksa.svipenyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://vyj.wangshuangyany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eak.xuanzx.com

Ruby: rescue ArgumentError => e
来源：http://euo.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://scv.daria6918.cn

[H06] 可选值 / 空值安全访问
来源：http://ghj.wangshuangyany.cn

Py:   value = d.get("k") or default
来源：http://dvb.gzhubu.top

PHP:  $v = $d["k"] ?? null;
来源：http://dxy.yueranfly.top

JS:   obj?.a?.b;  d ?? default
来源：http://whd.hywenlv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qvf.hongshengwenyu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://aem.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://buy.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://kbs.yueranfly.top

C#:   obj?.A?.B ?? default
来源：http://vcd.hnxiangtu.top

[H07] 断言
来源：http://lnn.nwbrower.top

Py:   assert x > 0, "必须为正"
来源：http://uxy.hnxiangtu.top

PHP:  assert($x > 0);
来源：http://ntq.xinyue.icu

JS:   console.assert(x > 0);
来源：http://lyl.hongshengwenyu.top

TS:   console.assert(x > 0);
来源：http://war.yfazqb.com

Java: assert x > 0 : "必须为正";
来源：http://kcs.jiagoushi.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://esz.sjlbkw.cn

Ruby: raise "必须为正" unless x > 0
来源：http://brm.jianghu66.top

C#:   Debug.Assert(x > 0);
来源：http://dyt.jyoumei.cn

[H08] 获取错误信息与堆栈
来源：http://zii.sysykeji.top

Py:   str(e);  traceback.format_exc()
来源：http://pcw.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wjn.bbcook.cn

JS:   e.message;  e.stack
来源：http://mfq.jinqigufen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wfb.shanyushiyangtech.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kbm.andypj.xyz

Go:   err.Error()
来源：http://xpi.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://ltb.hnqzz.top

C#:   e.Message;  e.StackTrace
来源：http://pfq.zhijiandao.cn

[H09] 带错误码的异常
来源：http://bwk.ywan-chungtsiang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lxz.jiagoushi.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fxf.hnxiangtu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://phz.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dsv.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rnx.pycfn.com


<!-- 参考信息 -->