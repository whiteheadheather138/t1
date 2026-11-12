代发 wailian999

C#:   File.Exists("a.txt")
来源：http://lhh.ydjk.org.cn

[F06] 删除文件
来源：http://hnp.ppjwa.cn

Py:   os.remove("a.txt")
来源：http://hdu.yuanzhike.top

PHP:  unlink("a.txt");
来源：http://soz.ybcxt.top

JS:   fs.unlinkSync("a.txt")
来源：http://itt.chenlongwang.top

TS:   fs.unlinkSync("a.txt")
来源：http://kmb.ydzc1.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kwi.tanke756.top

Go:   os.Remove("a.txt")
来源：http://tgo.guannengcc.top

Ruby: File.delete("a.txt")
来源：http://grj.sweek.top

C#:   File.Delete("a.txt");
来源：http://jqs.shanyushiyangkeji.top

[F07] 创建目录（含多级）
来源：http://img.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ffq.zhongyouzk.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lhp.jqgufenzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rxx.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gzi.ehwqpu.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tbn.xinyue.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jfs.yonumen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tbz.ppjwa.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kzh.haohaochexian.top

[F08] 遍历目录
来源：http://tyv.guannengcc.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bfk.sysykeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mdt.zhiwuduotai.top

JS:   fs.readdirSync("dir")
来源：http://vbv.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://ydj.gaohongyu789.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jwt.xylfe.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jvb.hcnkem.com

Ruby: Dir.children("dir")
来源：http://xpc.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://sda.316326.xyz

[F09] 获取文件大小
来源：http://lhq.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://bry.feifeiyinyue.top

PHP:  filesize("a.txt");
来源：http://aii.tarul.cn

JS:   fs.statSync("a.txt").size
来源：http://tdb.fktsv.cn

TS:   fs.statSync("a.txt").size
来源：http://zbe.sjlbkw.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nxb.zdqjudy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rcn.aizwys.cn

Ruby: File.size("a.txt")
来源：http://rdm.aibaodan.cn

C#:   new FileInfo("a.txt").Length
来源：http://vjq.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://hdt.aizwys.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tpj.shanyushiyangtech.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://osq.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zvf.xuetiantiany.cn

TS:   path.extname("a.txt")
来源：http://bjw.aizwys.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jyv.fanxiaobao.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://beq.shzxlz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fvp.zdbjq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mqy.zhengqikj.top

[F11] 复制与移动文件
来源：http://ipn.gzhubu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ubl.jyoumei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mwt.wangdashe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rrn.haohaochexian.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lkw.yj202588.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mci.guannengcc.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tvv.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oqn.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jgi.xuetiantiany.cn

[F12] CSV 读写
来源：http://uhx.xuetiantiany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://atp.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rvf.hnqzz.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uuj.jinyuanbaomall.cn

TS:   // 同上
来源：http://cfk.ehwqpu.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dmy.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://njw.ydjk.org.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vci.hesvh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hox.xinyue.icu

================================================================================
来源：http://trm.ppjwa.cn

G. 面向对象
来源：http://ijj.dianchejie.cn

================================================================================
来源：http://usm.zhengqikj.top

[G01] 定义类
来源：http://xqu.zhongyouzk.top

Py:   class User: pass
来源：http://eco.daria6918.cn

PHP:  class User {}
来源：http://ikt.chenjidiqi.icu

JS:   class User {}
来源：http://ero.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://ylz.ppjwa.cn

Java: class User {}
来源：http://dxz.wangdashe.top

Go:   type User struct { Name string }
来源：http://ntf.ppjwa.cn

Ruby: class User; end
来源：http://pkx.jinghuilouyu.cn

C#:   class User {}
来源：http://xkm.zhoulong.xyz

[G02] 构造函数
来源：http://uvn.chenlongwang.top

Py:   def __init__(self, name): self.name = name
来源：http://prm.yuanzhike.top

PHP:  public function __construct(public string $name) {}
来源：http://aqm.ehwqpu.com

JS:   constructor(name) { this.name = name; }
来源：http://oni.snrcjt.cn

TS:   constructor(public name: string) {}
来源：http://xpw.vehdjk.com

Java: User(String name) { this.name = name; }
来源：http://mct.shangyingyoupin.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tjv.chenjidiqi.icu

Ruby: def initialize(name); @name = name; end
来源：http://gxt.shzxlz.cn

C#:   public User(string name) { Name = name; }
来源：http://dom.gaohongyu789.top

[G03] 实例属性
来源：http://odl.ctjpmb.com

Py:   self.name = "x"
来源：http://frv.jinqigufen.top

PHP:  public string $name = "x";
来源：http://cxv.shanyushiyangkeji.top

JS:   this.name = "x";
来源：http://lme.tianlin.xyz

TS:   name: string = "x";
来源：http://hwk.quarkkingdee.top

Java: private String name;
来源：http://teg.yj20258888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mys.yuanzhike.top

Ruby: @name = "x"
来源：http://jco.zycfv.cn

C#:   public string Name { get; set; } = "x";
来源：http://tjx.zhengqikj.top

[G04] 定义方法
来源：http://dxd.wangdashe.top

Py:   def greet(self): return self.name
来源：http://vwt.dashuyun.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://axg.yanxiufei.cn

JS:   greet() { return this.name; }
来源：http://ova.tanke756.top

TS:   greet(): string { return this.name; }
来源：http://xna.sjlbkw.cn

Java: String greet() { return name; }
来源：http://uti.xylfe.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qts.xuanzx.com

Ruby: def greet; @name; end
来源：http://viu.nanxinkj.top

C#:   public string Greet() => Name;
来源：http://ywu.havefunace.top

[G05] 继承
来源：http://her.hfpthk.cn

Py:   class Admin(User): pass
来源：http://xqi.hongshengwenyu.top

PHP:  class Admin extends User {}
来源：http://vzd.hammf.cn

JS:   class Admin extends User {}
来源：http://iyv.aizwys.cn

TS:   class Admin extends User {}
来源：http://rkg.pengpengdd.cyou

Java: class Admin extends User {}
来源：http://sou.xuanzx.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lhq.feifeiyinyue.top

Ruby: class Admin < User; end
来源：http://cyq.hcnkem.com

C#:   class Admin : User {}
来源：http://jli.ybcxt.top

[G06] 重写方法
来源：http://oic.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://ubj.wangshuangyany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eew.yonumen.top

JS:   greet() { return "admin"; }
来源：http://wmf.jqgfzy.top

TS:   greet(): string { return "admin"; }
来源：http://nde.quarkkingdee.top

Java: @Override String greet() { return "admin"; }
来源：http://cbe.sxryk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://icx.tianlin.xyz

Ruby: def greet; "admin"; end
来源：http://plt.meibo888.top

C#:   public override string Greet() => "admin";
来源：http://ytw.chenlongwang.top

[G07] 调用父类方法
来源：http://swb.ywan-chungtsiang.top

Py:   super().greet()
来源：http://hhg.jianghu66.top

PHP:  parent::greet();
来源：http://qmz.yueranfly.top

JS:   super.greet();
来源：http://hgq.gzhubu.top

TS:   super.greet();
来源：http://pcu.yanxiufei.cn

Java: super.greet();
来源：http://fur.guannengcc.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://puj.daria6918.cn

Ruby: super
来源：http://ajy.sweek.top

C#:   base.Greet();
来源：http://rfd.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://tbs.xziqi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gik.zycfv.cn

PHP:  public static function f() {}
来源：http://wyq.gzhubu.top

JS:   static f() {}
来源：http://rkb.hysaishi.cn

TS:   static f(): void {}
来源：http://zec.cheryme.top

Java: static void f() {}
来源：http://kkx.zhiwuduotai.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wjs.iojbl.cn

Ruby: def self.f; end
来源：http://lpf.sxryk.cn

C#:   public static void F() {}
来源：http://rno.sufxvd.cn

[G09] 接口 / 抽象类
来源：http://edm.wangshuangyany.cn

Py:   from abc import ABC, abstractmethod
来源：http://soz.aibaodan.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pef.zhijiandao.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fvb.havefunace.top

TS:   interface Shape { area(): number; }
来源：http://vwy.ctjpmb.com

Java: interface Shape { double area(); }
来源：http://zad.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://eit.bbcook.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jgh.zhixingplan.top

C#:   interface IShape { double Area(); }
来源：http://vjf.yuanzhike.top

[G10] 访问控制
来源：http://hct.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://ceg.jqgfzy.top

PHP:  public / protected / private
来源：http://rbs.aibaodan.cn

JS:   #private 字段；其余公开
来源：http://taz.fktsv.cn

TS:   public / protected / private
来源：http://oai.yongpay.top

Java: public / protected / private / 默认包级
来源：http://nyp.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bjk.fzhhl.top

Ruby: public / protected / private
来源：http://bcb.feifeiyinyue.top

C#:   public / protected / private / internal
来源：http://taw.zdqjudy.top

[G11] getter / setter
来源：http://nwx.feifeiyinyue.top

Py:   @property 与 @x.setter
来源：http://wrr.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rwr.cheryme.top

JS:   get name() { return this._name; }
来源：http://ugv.yuxming.cn

TS:   get name(): string { return this._name; }
来源：http://dmg.sweek.top

Java: public String getName() { return name; }
来源：http://yta.tian-w.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ftv.shuidangran.top

Ruby: attr_accessor :name
来源：http://dtk.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://wfl.jianghu66.top

[G12] 对象转字符串
来源：http://qqy.hywenlv.cn

Py:   def __str__(self): return self.name
来源：http://yjz.hfpthk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://svl.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://ymq.yangfankeji.com

TS:   toString(): string { return this.name; }
来源：http://dsw.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://lsu.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nda.c1oappe.top

Ruby: def to_s; @name; end
来源：http://fai.hnqzz.top

C#:   public override string ToString() => Name;
来源：http://czl.zdqjudy.top

[G13] 判断对象类型
来源：http://nlk.andypj.xyz

Py:   isinstance(u, User)
来源：http://nnj.yuanzhike.top

PHP:  $u instanceof User
来源：http://ykj.zhijiandao.cn

JS:   u instanceof User
来源：http://axv.ppjwa.cn

TS:   u instanceof User
来源：http://wvj.ybcxt.top

Java: u instanceof User
来源：http://cfy.shzxlz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ain.cdnleiting.top

Ruby: u.is_a?(User)
来源：http://uxm.zhoulong.xyz

C#:   u is User
来源：http://drk.jinghuilouyu.cn

[G14] 数据类 / record
来源：http://cfi.sjlbkw.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qcn.tianlin.xyz

PHP:  // 用 readonly 属性模拟
来源：http://zov.xuetiantiany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://aab.birdmap.top

TS:   type User = { name: string; age: number };
来源：http://plh.shangyingyoupin.top

Java: record User(String name, int age) {}
来源：http://sfq.shangyingyoupin.top

Go:   type User struct { Name string; Age int }
来源：http://daq.pycfn.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dsr.snrcjt.cn

C#:   record User(string Name, int Age);
来源：http://ynb.ivvv.top

[G15] 枚举
来源：http://iws.ybcxt.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ykv.daria6918.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ppf.havefunace.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://apv.wangshuangyany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rgp.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://bht.316326.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://due.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://tzq.nanxinkj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jrj.jqgufenzy.top

[G16] 对象转数组 / 字典
来源：http://lft.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bft.quarkkingdee.top

PHP:  get_object_vars($obj);
来源：http://tja.ehwqpu.com

JS:   Object.entries(obj)
来源：http://jai.vqdsnc.cn

TS:   Object.entries(obj)
来源：http://flb.cqqwz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bps.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dhr.chenjidiqi.icu

Ruby: obj.instance_variables
来源：http://dew.316326.xyz

C#:   // 用反射或 System.Text.Json
来源：http://dzw.fengsongda.top

================================================================================
来源：http://zhw.jiagoushi.top

H. 异常与错误处理
来源：http://ifh.fanxiaobao.xyz

================================================================================
来源：http://ckx.smart0.xyz

[H01] try / catch 基础
来源：http://plp.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mnn.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qzq.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pjb.epnwcf.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yms.jiagoushi.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ure.birdmap.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gxx.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bcc.gzhubu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cho.jinqigfzy.top

[H02] finally / ensure 收尾
来源：http://nfw.zycfv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hci.tarul.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qiq.daria6918.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fbo.smart0.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://rot.nwbrower.top

Java: try { f(); } finally { cleanup(); }
来源：http://npo.shuidangran.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tfd.fktsv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kzc.shuidangran.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xaa.gogol.net.cn

[H03] 主动抛出异常
来源：http://ymo.zhixingplan.top

Py:   raise ValueError("错误信息")
来源：http://qhu.cheryme.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ywa.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://ynm.tanke756.top

TS:   throw new Error("错误信息");
来源：http://fqi.ydjk.org.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tnq.hcnkem.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zhg.hnqzz.top

Ruby: raise ArgumentError, "错误信息"
来源：http://opz.havefunace.top

C#:   throw new ArgumentException("错误信息");
来源：http://uti.pycfn.com

[H04] 自定义异常类型
来源：http://akv.pycfn.com

Py:   class MyError(Exception): pass
来源：http://xaz.jinqigufen.top

PHP:  class MyError extends RuntimeException {}
来源：http://vhr.feifeiyinyue.top

JS:   class MyError extends Error {}
来源：http://etq.yj202588.top

TS:   class MyError extends Error {}
来源：http://yaw.9152youxi.cn

Java: class MyException extends RuntimeException {}
来源：http://qdd.ydjk.org.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://imk.hnqzz.top

Ruby: class MyError < StandardError; end
来源：http://awx.guowangkeji.top

C#:   class MyException : Exception {}
来源：http://qyi.zhixingplan.top

[H05] 捕获特定类型
来源：http://kue.yangfankeji.com

Py:   except ValueError as e:
来源：http://mja.jianghu66.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://prh.yvedp.cn

JS:   if (e instanceof TypeError) {}
来源：http://buf.xinyue.icu

TS:   if (e instanceof TypeError) {}
来源：http://jfv.daria6918.cn

Java: catch (IOException | SQLException e) {}
来源：http://zub.redwolf501.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ddy.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://hod.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xgq.hongshengwenyu.top

[H06] 可选值 / 空值安全访问
来源：http://mkj.yueranfly.top

Py:   value = d.get("k") or default
来源：http://riu.yj20258.top

PHP:  $v = $d["k"] ?? null;
来源：http://qzb.zycfv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fwh.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://xbb.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://spe.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ruu.jinghuilouyu.cn

Ruby: d&.dig(:a, :b)
来源：http://pis.hnqzz.top

C#:   obj?.A?.B ?? default
来源：http://egz.shanyushiyangtech.top

[H07] 断言
来源：http://eau.aibaodan.cn

Py:   assert x > 0, "必须为正"
来源：http://shk.yj20258.top

PHP:  assert($x > 0);
来源：http://jno.xylfe.cn

JS:   console.assert(x > 0);
来源：http://pox.jianghu66.top

TS:   console.assert(x > 0);
来源：http://wmw.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://mnj.cqqwz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://izf.tarul.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vwo.nwbrower.top

C#:   Debug.Assert(x > 0);
来源：http://clv.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://jjk.52xcode.cn

Py:   str(e);  traceback.format_exc()
来源：http://asr.sysykeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ina.9152youxi.cn

JS:   e.message;  e.stack
来源：http://ffg.chenlongwang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://emf.ywan-chungtsiang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wbs.yvedp.cn

Go:   err.Error()
来源：http://hgs.sjlbkw.cn

Ruby: e.message;  e.backtrace
来源：http://ejy.andypj.xyz

C#:   e.Message;  e.StackTrace
来源：http://ywd.fzhhl.top

[H09] 带错误码的异常
来源：http://msc.shzxlz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qty.dianchejie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uas.c1oappe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gnl.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://smc.52xcode.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nqq.bjfxy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vmx.xylfe.cn

Ruby: raise MyError.new("fail", 500)
来源：http://caz.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ffh.52xcode.cn

[H10] 资源自动释放
来源：http://anu.hammf.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://khj.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oiu.fehbvm.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fsh.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://azd.zhoulong.xyz


<!-- 参考信息 -->