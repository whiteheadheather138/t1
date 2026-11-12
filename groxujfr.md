代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://ynv.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://omr.nanxuanxn.top

PHP:  file_exists("a.txt");
来源：http://bjv.xylfe.cn

JS:   fs.existsSync("a.txt")
来源：http://vat.vehdjk.com

TS:   fs.existsSync("a.txt")
来源：http://hlc.zdbjq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xdv.wangdashe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dlm.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://cey.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://zrw.tarul.cn

[F06] 删除文件
来源：http://rnx.guannengcc.top

Py:   os.remove("a.txt")
来源：http://frw.yongpay.top

PHP:  unlink("a.txt");
来源：http://atk.cashguo.top

JS:   fs.unlinkSync("a.txt")
来源：http://xel.pycfn.com

TS:   fs.unlinkSync("a.txt")
来源：http://fza.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vma.bbcook.cn

Go:   os.Remove("a.txt")
来源：http://jdt.cdnleiting.top

Ruby: File.delete("a.txt")
来源：http://vys.xuetiantiany.cn

C#:   File.Delete("a.txt");
来源：http://stl.zhengqikj.top

[F07] 创建目录（含多级）
来源：http://urc.tanke756.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ycb.haohaochexian.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eqz.quarkkingdee.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uvs.yj202588.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mhu.yonumen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://apo.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://imv.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://llk.sjlbkw.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://los.xylfe.cn

[F08] 遍历目录
来源：http://unn.haohaochexian.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hwj.vehdjk.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bsw.yongpay.top

JS:   fs.readdirSync("dir")
来源：http://eov.jiagoushi.top

TS:   fs.readdirSync("dir")
来源：http://fdp.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wku.jinyuanbaomall.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lxj.tarul.cn

Ruby: Dir.children("dir")
来源：http://loe.hammf.cn

C#:   Directory.GetFiles("dir")
来源：http://gbc.yonumen.top

[F09] 获取文件大小
来源：http://kcn.9152youxi.cn

Py:   os.path.getsize("a.txt")
来源：http://lsl.hywenlv.cn

PHP:  filesize("a.txt");
来源：http://wcs.ydjk.org.cn

JS:   fs.statSync("a.txt").size
来源：http://fcj.smart0.xyz

TS:   fs.statSync("a.txt").size
来源：http://azs.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://rkz.zdbjq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kyb.fengsongda.top

Ruby: File.size("a.txt")
来源：http://ipt.aizwys.cn

C#:   new FileInfo("a.txt").Length
来源：http://aqf.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://anz.cdnleiting.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ppp.jinyuanbaomall.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rpo.xuetiantiany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dlh.wangshuangyany.cn

TS:   path.extname("a.txt")
来源：http://cln.shanyushiyangtech.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wwn.fktsv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://egi.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xwx.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://efu.zhijiandao.cn

[F11] 复制与移动文件
来源：http://olf.nwbrower.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rvp.zhixingplan.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hjg.hysaishi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://smt.kuanghao11.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mtk.dashuyun.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nbb.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lom.gaohongyu789.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fhy.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://atx.52xcode.cn

[F12] CSV 读写
来源：http://jvp.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hrk.shanyushiyangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pvb.hongshengwenyu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lql.yuanzhike.top

TS:   // 同上
来源：http://pby.epnwcf.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bga.sufxvd.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uck.dashuyun.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fvo.ctjpmb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://kab.haohaochexian.top

================================================================================
来源：http://heb.sjlbkw.cn

G. 面向对象
来源：http://dtr.ybcxt.top

================================================================================
来源：http://xmp.yj202588.top

[G01] 定义类
来源：http://row.jianghu66.top

Py:   class User: pass
来源：http://rbk.fktsv.cn

PHP:  class User {}
来源：http://qhn.shuidangran.top

JS:   class User {}
来源：http://hxc.0kj1m.cn

TS:   class User { name: string = ""; }
来源：http://lvk.ehwqpu.com

Java: class User {}
来源：http://ezz.yuxming.cn

Go:   type User struct { Name string }
来源：http://tgc.9152youxi.cn

Ruby: class User; end
来源：http://dxl.sysykeji.top

C#:   class User {}
来源：http://zkh.vqdsnc.cn

[G02] 构造函数
来源：http://zmu.ehwqpu.com

Py:   def __init__(self, name): self.name = name
来源：http://ykp.gaohongyu789.top

PHP:  public function __construct(public string $name) {}
来源：http://ycr.sjlbkw.cn

JS:   constructor(name) { this.name = name; }
来源：http://obk.shanyushiyangkeji.top

TS:   constructor(public name: string) {}
来源：http://xfb.aibaodan.cn

Java: User(String name) { this.name = name; }
来源：http://ofz.jiagoushi.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tdb.gogol.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://jix.shzxlz.cn

C#:   public User(string name) { Name = name; }
来源：http://yas.jianghu66.top

[G03] 实例属性
来源：http://lse.yanxiufei.cn

Py:   self.name = "x"
来源：http://qzd.jyoumei.cn

PHP:  public string $name = "x";
来源：http://oqd.jinqigufen.top

JS:   this.name = "x";
来源：http://kyd.ydzc1.top

TS:   name: string = "x";
来源：http://lrd.iojbl.cn

Java: private String name;
来源：http://snr.sweek.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ylr.sysykeji.top

Ruby: @name = "x"
来源：http://qzx.vehdjk.com

C#:   public string Name { get; set; } = "x";
来源：http://xre.zdqjudy.top

[G04] 定义方法
来源：http://gdm.hesvh.cn

Py:   def greet(self): return self.name
来源：http://lcb.zhiwuduotai.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dsz.hywenlv.cn

JS:   greet() { return this.name; }
来源：http://age.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://itk.snrcjt.cn

Java: String greet() { return name; }
来源：http://dkk.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kdc.9152youxi.cn

Ruby: def greet; @name; end
来源：http://eim.hcnkem.com

C#:   public string Greet() => Name;
来源：http://iey.ybcxt.top

[G05] 继承
来源：http://lds.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://ked.svipenyu.cn

PHP:  class Admin extends User {}
来源：http://lnv.cucudq.cn

JS:   class Admin extends User {}
来源：http://fxb.daxiang520.top

TS:   class Admin extends User {}
来源：http://yyb.chenzaomai.com

Java: class Admin extends User {}
来源：http://auf.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wbd.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://piv.hnqzz.top

C#:   class Admin : User {}
来源：http://wpr.zdbjq.cn

[G06] 重写方法
来源：http://gpw.ydjk.org.cn

Py:   def greet(self): return "admin"
来源：http://fga.zhongyouzk.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ecq.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://mfl.mhx1999.top

TS:   greet(): string { return "admin"; }
来源：http://gyw.0kj1m.cn

Java: @Override String greet() { return "admin"; }
来源：http://tno.zhiwuduotai.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://guw.daxiang520.top

Ruby: def greet; "admin"; end
来源：http://qpw.dianchejie.cn

C#:   public override string Greet() => "admin";
来源：http://nhp.9152youxi.cn

[G07] 调用父类方法
来源：http://gpw.aizwys.cn

Py:   super().greet()
来源：http://use.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://oks.xingfuxueyuan.xyz

JS:   super.greet();
来源：http://yur.xylfe.cn

TS:   super.greet();
来源：http://auh.yueranfly.top

Java: super.greet();
来源：http://bow.ppjwa.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bfw.haohaochexian.top

Ruby: super
来源：http://rcd.sysykeji.top

C#:   base.Greet();
来源：http://urh.zhiwuduotai.top

[G08] 静态方法与属性
来源：http://yyo.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mpm.zhiwuduotai.top

PHP:  public static function f() {}
来源：http://dav.wangshuangyany.cn

JS:   static f() {}
来源：http://gbc.xziqi.cn

TS:   static f(): void {}
来源：http://jrn.wangshuangyany.cn

Java: static void f() {}
来源：http://hvt.hysaishi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://aho.ivvv.top

Ruby: def self.f; end
来源：http://lbd.xziqi.cn

C#:   public static void F() {}
来源：http://brs.yonumen.top

[G09] 接口 / 抽象类
来源：http://fyi.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://sio.ywan-chungtsiang.top

PHP:  interface Shape { public function area(): float; }
来源：http://oqn.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://aeu.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://omu.feifeiyinyue.top

Java: interface Shape { double area(); }
来源：http://ini.hammf.cn

Go:   type Shape interface { Area() float64 }
来源：http://fxb.snrcjt.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uar.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://nzt.ydjk.org.cn

[G10] 访问控制
来源：http://hmi.jinyuanbaomall.cn

Py:   约定 _protected / __private（不强制）
来源：http://aik.smart0.xyz

PHP:  public / protected / private
来源：http://uke.yongpay.top

JS:   #private 字段；其余公开
来源：http://qbj.sufxvd.cn

TS:   public / protected / private
来源：http://keg.andypj.xyz

Java: public / protected / private / 默认包级
来源：http://fbt.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://rph.jqgfzy.top

Ruby: public / protected / private
来源：http://emv.shuidangran.top

C#:   public / protected / private / internal
来源：http://ddb.sweek.top

[G11] getter / setter
来源：http://jdc.havefunace.top

Py:   @property 与 @x.setter
来源：http://ehu.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://bze.shuidangran.top

JS:   get name() { return this._name; }
来源：http://lpk.yuanzhike.top

TS:   get name(): string { return this._name; }
来源：http://cwc.jqgfzy.top

Java: public String getName() { return name; }
来源：http://mrs.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://twk.hongshengwenyu.top

Ruby: attr_accessor :name
来源：http://eui.xziqi.cn

C#:   public string Name { get; set; }
来源：http://sfx.jinqigfzy.top

[G12] 对象转字符串
来源：http://xmb.havefunace.top

Py:   def __str__(self): return self.name
来源：http://rcq.chenjidiqi.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://oop.hammf.cn

JS:   toString() { return this.name; }
来源：http://fwm.aizwys.cn

TS:   toString(): string { return this.name; }
来源：http://cde.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://yzp.yj202588.top

Go:   func (u User) String() string { return u.Name }
来源：http://tov.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://zkh.ppjwa.cn

C#:   public override string ToString() => Name;
来源：http://bjc.ydjk.org.cn

[G13] 判断对象类型
来源：http://uii.hywenlv.cn

Py:   isinstance(u, User)
来源：http://sah.fktsv.cn

PHP:  $u instanceof User
来源：http://jdw.yanxiufei.cn

JS:   u instanceof User
来源：http://sxd.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://vjb.zhixingplan.top

Java: u instanceof User
来源：http://nkr.jinqigufen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xam.vehdjk.com

Ruby: u.is_a?(User)
来源：http://dek.yj20258.top

C#:   u is User
来源：http://yaf.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://mkd.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ygv.pycfn.com

PHP:  // 用 readonly 属性模拟
来源：http://eqe.ehwqpu.com

JS:   // 无内置：普通类或对象字面量
来源：http://ubg.ybcxt.top

TS:   type User = { name: string; age: number };
来源：http://vsh.jyoumei.cn

Java: record User(String name, int age) {}
来源：http://vko.meibo888.top

Go:   type User struct { Name string; Age int }
来源：http://xff.hywenlv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fiz.wangshuangyany.cn

C#:   record User(string Name, int Age);
来源：http://vcu.yj202588.top

[G15] 枚举
来源：http://ahf.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vto.zhijiandao.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kyr.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rwd.hysaishi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mfh.xuetiantiany.cn

Java: enum Color { RED, GREEN }
来源：http://ctw.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pgt.cucudq.cn

Ruby: Color = %i[red green].freeze
来源：http://cge.pengpengdd.cyou

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nuq.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://ust.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://apq.fktsv.cn

PHP:  get_object_vars($obj);
来源：http://xta.sjlbkw.cn

JS:   Object.entries(obj)
来源：http://hjx.yuxming.cn

TS:   Object.entries(obj)
来源：http://yvd.haohaochexian.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zmf.guowangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://uti.chenjidiqi.icu

Ruby: obj.instance_variables
来源：http://hoc.xingfuxueyuan.xyz

C#:   // 用反射或 System.Text.Json
来源：http://ngw.zhijiandao.cn

================================================================================
来源：http://bss.shangyingyoupin.top

H. 异常与错误处理
来源：http://rmn.nwbrower.top

================================================================================
来源：http://npi.yueranfly.top

[H01] try / catch 基础
来源：http://sff.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zpl.ybcxt.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xqa.gaohongyu789.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xfb.iojbl.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ard.jinyuanbaomall.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lpz.hywenlv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://noa.ppjwa.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zah.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fgk.jinqigfzy.top

[H02] finally / ensure 收尾
来源：http://dbf.wangdashe.top

Py:   try: f()⏎finally: cleanup()
来源：http://mtl.pycfn.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://ump.zhixingplan.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qxf.ppjwa.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uam.nwbrower.top

Java: try { f(); } finally { cleanup(); }
来源：http://xtt.iojbl.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gmd.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nvl.andypj.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://env.yfazqb.com

[H03] 主动抛出异常
来源：http://rsb.dashuyun.cn

Py:   raise ValueError("错误信息")
来源：http://smn.jlsjyb.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bys.c1oappe.top

JS:   throw new Error("错误信息");
来源：http://pem.epnwcf.com

TS:   throw new Error("错误信息");
来源：http://ycf.xingfuxueyuan.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://rmg.shangyingyoupin.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hss.shangyingyoupin.top

Ruby: raise ArgumentError, "错误信息"
来源：http://aym.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://sex.zhiwuduotai.top

[H04] 自定义异常类型
来源：http://kgx.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://ozx.gaohongyu789.top

PHP:  class MyError extends RuntimeException {}
来源：http://qdq.yonumen.top

JS:   class MyError extends Error {}
来源：http://ine.wangdashe.top

TS:   class MyError extends Error {}
来源：http://oxh.vqdsnc.cn

Java: class MyException extends RuntimeException {}
来源：http://ktw.xuanzx.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gqw.ehwqpu.com

Ruby: class MyError < StandardError; end
来源：http://lht.daxiang520.top

C#:   class MyException : Exception {}
来源：http://agp.shzxlz.cn

[H05] 捕获特定类型
来源：http://zlv.xuanzx.com

Py:   except ValueError as e:
来源：http://xku.nanxinkj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zys.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://nxz.yuanzhike.top

TS:   if (e instanceof TypeError) {}
来源：http://ooy.sjlbkw.cn

Java: catch (IOException | SQLException e) {}
来源：http://znt.jinqigufen.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ynr.yj20258.top

Ruby: rescue ArgumentError => e
来源：http://ddr.hcnkem.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dqi.tanke756.top

[H06] 可选值 / 空值安全访问
来源：http://inr.xziqi.cn

Py:   value = d.get("k") or default
来源：http://aso.shzxlz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yxz.dashuyun.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rsn.sxryk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nfe.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hwt.cdnleiting.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fqi.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://qdh.smart0.xyz

C#:   obj?.A?.B ?? default
来源：http://etl.quarkkingdee.top

[H07] 断言
来源：http://kqk.cdnleiting.top

Py:   assert x > 0, "必须为正"
来源：http://gdg.guowangkeji.top

PHP:  assert($x > 0);
来源：http://rer.gzhubu.top

JS:   console.assert(x > 0);
来源：http://yio.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://aco.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://nam.hcnkem.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wdw.chenjidiqi.icu

Ruby: raise "必须为正" unless x > 0
来源：http://eao.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://fmq.feifeiyinyue.top

[H08] 获取错误信息与堆栈
来源：http://pst.yonumen.top

Py:   str(e);  traceback.format_exc()
来源：http://jtj.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qas.ybcxt.top

JS:   e.message;  e.stack
来源：http://rqi.birdmap.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mil.gzhubu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tjd.tarul.cn

Go:   err.Error()
来源：http://qcm.fehbvm.com

Ruby: e.message;  e.backtrace
来源：http://pyj.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://hej.hnxiangtu.top

[H09] 带错误码的异常
来源：http://ujd.gaohongyu789.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bzz.xingfuxueyuan.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://fiu.aizwys.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lzv.guannengcc.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://szs.jyoumei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mpl.snrcjt.cn


<!-- 参考信息 -->