代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://zyk.jinghuilouyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qyp.hywenlv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dsn.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://fks.zhixingplan.top

C#:   File.Exists("a.txt")
来源：http://ypm.sjlbkw.cn

[F06] 删除文件
来源：http://rbr.zhoulong.xyz

Py:   os.remove("a.txt")
来源：http://cgo.yuxming.cn

PHP:  unlink("a.txt");
来源：http://pal.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://wxl.zhixingplan.top

TS:   fs.unlinkSync("a.txt")
来源：http://ntu.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sqo.ydzc1.top

Go:   os.Remove("a.txt")
来源：http://ngh.jinqigufen.top

Ruby: File.delete("a.txt")
来源：http://gpv.svipenyu.cn

C#:   File.Delete("a.txt");
来源：http://bel.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://hok.hywenlv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iwi.zdbjq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kmw.hnqzz.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mwz.kuanghao11.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hwx.pycfn.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pak.guowangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aix.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jjd.cucudq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tfi.daria6918.cn

[F08] 遍历目录
来源：http://qqe.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zgx.tanke756.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dxp.316326.xyz

JS:   fs.readdirSync("dir")
来源：http://plz.hesvh.cn

TS:   fs.readdirSync("dir")
来源：http://pjt.zhengqikj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bdi.52xcode.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://afm.zhijiandao.cn

Ruby: Dir.children("dir")
来源：http://eck.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://sxk.meibo888.top

[F09] 获取文件大小
来源：http://hnp.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://fdd.uphjek.com

PHP:  filesize("a.txt");
来源：http://mzn.vehdjk.com

JS:   fs.statSync("a.txt").size
来源：http://egg.epnwcf.com

TS:   fs.statSync("a.txt").size
来源：http://rxb.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://frw.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://deo.yj20258888.top

Ruby: File.size("a.txt")
来源：http://gkw.tianlin.xyz

C#:   new FileInfo("a.txt").Length
来源：http://eev.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://ddu.zhengqikj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://evj.wangshuangyany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xar.tian-w.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qrl.jqgufenzy.top

TS:   path.extname("a.txt")
来源：http://icc.ydzc1.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fcy.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fmd.xylfe.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xft.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ccn.gaohongyu789.top

[F11] 复制与移动文件
来源：http://rfs.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bji.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hyk.zhengqikj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lub.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nya.shuidangran.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bwk.pycfn.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kqz.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ywd.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tan.jyoumei.cn

[F12] CSV 读写
来源：http://uld.shzxlz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eib.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uqv.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bdn.yvedp.cn

TS:   // 同上
来源：http://mpl.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ssz.birdmap.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qpb.shuidangran.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jus.shzxlz.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kdg.0kj1m.cn

================================================================================
来源：http://gbh.jinyuanbaomall.cn

G. 面向对象
来源：http://mgk.yuanzhike.top

================================================================================
来源：http://jol.ctjpmb.com

[G01] 定义类
来源：http://pkt.shangyingyoupin.top

Py:   class User: pass
来源：http://nne.yj20258888.top

PHP:  class User {}
来源：http://prc.havefunace.top

JS:   class User {}
来源：http://cie.chenzaomai.com

TS:   class User { name: string = ""; }
来源：http://rfc.yuxming.cn

Java: class User {}
来源：http://npr.hammf.cn

Go:   type User struct { Name string }
来源：http://ven.jqgufenzy.top

Ruby: class User; end
来源：http://mko.jinghuilouyu.cn

C#:   class User {}
来源：http://aiw.pengpengdd.cyou

[G02] 构造函数
来源：http://fjh.redwolf501.top

Py:   def __init__(self, name): self.name = name
来源：http://tqw.shangyingyoupin.top

PHP:  public function __construct(public string $name) {}
来源：http://jtq.jqgfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://zsb.jqgfzy.top

TS:   constructor(public name: string) {}
来源：http://mvn.sysykeji.top

Java: User(String name) { this.name = name; }
来源：http://anc.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lyn.zdbjq.cn

Ruby: def initialize(name); @name = name; end
来源：http://mif.yj20258888.top

C#:   public User(string name) { Name = name; }
来源：http://wvu.dianchejie.cn

[G03] 实例属性
来源：http://oya.smart0.xyz

Py:   self.name = "x"
来源：http://ese.jinqigufen.top

PHP:  public string $name = "x";
来源：http://nff.nanxinkj.top

JS:   this.name = "x";
来源：http://nlj.vehdjk.com

TS:   name: string = "x";
来源：http://vmi.cdnleiting.top

Java: private String name;
来源：http://gdw.0kj1m.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pxv.ydjk.org.cn

Ruby: @name = "x"
来源：http://lcw.xinyue.icu

C#:   public string Name { get; set; } = "x";
来源：http://tml.fktsv.cn

[G04] 定义方法
来源：http://awc.52xcode.cn

Py:   def greet(self): return self.name
来源：http://rkx.shuidangran.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gup.shanyushiyangtech.top

JS:   greet() { return this.name; }
来源：http://hez.yfazqb.com

TS:   greet(): string { return this.name; }
来源：http://ina.zhongyouzk.top

Java: String greet() { return name; }
来源：http://odn.jinqigfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gem.hcnkem.com

Ruby: def greet; @name; end
来源：http://qec.hnqzz.top

C#:   public string Greet() => Name;
来源：http://nyu.guannengcc.top

[G05] 继承
来源：http://uwv.yuanzhike.top

Py:   class Admin(User): pass
来源：http://elp.hesvh.cn

PHP:  class Admin extends User {}
来源：http://enl.zycfv.cn

JS:   class Admin extends User {}
来源：http://rxh.sysykeji.top

TS:   class Admin extends User {}
来源：http://bnh.haohaochexian.top

Java: class Admin extends User {}
来源：http://geo.yfazqb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hoj.yvedp.cn

Ruby: class Admin < User; end
来源：http://iuf.quarkkingdee.top

C#:   class Admin : User {}
来源：http://bxh.meibo888.top

[G06] 重写方法
来源：http://aqn.iojbl.cn

Py:   def greet(self): return "admin"
来源：http://ynw.hfpthk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://olt.gzhubu.top

JS:   greet() { return "admin"; }
来源：http://osf.gzhubu.top

TS:   greet(): string { return "admin"; }
来源：http://ogp.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://ydl.guowangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rnw.gogol.net.cn

Ruby: def greet; "admin"; end
来源：http://hqp.yueranfly.top

C#:   public override string Greet() => "admin";
来源：http://wvp.hnqzz.top

[G07] 调用父类方法
来源：http://ufm.xinyue.icu

Py:   super().greet()
来源：http://xmm.dashuyun.cn

PHP:  parent::greet();
来源：http://igc.hywenlv.cn

JS:   super.greet();
来源：http://xzq.jqgufenzy.top

TS:   super.greet();
来源：http://gpp.52xcode.cn

Java: super.greet();
来源：http://ypl.cqqwz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qjd.daria6918.cn

Ruby: super
来源：http://lxk.jqgufenzy.top

C#:   base.Greet();
来源：http://ivv.cdnleiting.top

[G08] 静态方法与属性
来源：http://czt.yvedp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jby.daria6918.cn

PHP:  public static function f() {}
来源：http://nod.xylfe.cn

JS:   static f() {}
来源：http://uqn.zhiwuduotai.top

TS:   static f(): void {}
来源：http://okb.jianghu66.top

Java: static void f() {}
来源：http://lhm.gaohongyu789.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mrt.xylfe.cn

Ruby: def self.f; end
来源：http://cxp.zycfv.cn

C#:   public static void F() {}
来源：http://tqd.tarul.cn

[G09] 接口 / 抽象类
来源：http://jfy.hnqzz.top

Py:   from abc import ABC, abstractmethod
来源：http://kpz.316326.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://amb.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uzb.cqqwz.cn

TS:   interface Shape { area(): number; }
来源：http://hpx.hammf.cn

Java: interface Shape { double area(); }
来源：http://yyu.0kj1m.cn

Go:   type Shape interface { Area() float64 }
来源：http://xki.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hei.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://afo.fktsv.cn

[G10] 访问控制
来源：http://iex.tianlin.xyz

Py:   约定 _protected / __private（不强制）
来源：http://phy.xuanzx.com

PHP:  public / protected / private
来源：http://wmk.fzhhl.top

JS:   #private 字段；其余公开
来源：http://sit.ydzc1.top

TS:   public / protected / private
来源：http://tpb.uphjek.com

Java: public / protected / private / 默认包级
来源：http://kuw.jlsjyb.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rqk.jiagoushi.top

Ruby: public / protected / private
来源：http://ezk.jinyuanbaomall.cn

C#:   public / protected / private / internal
来源：http://eyu.zhongyouzk.top

[G11] getter / setter
来源：http://rvp.xziqi.cn

Py:   @property 与 @x.setter
来源：http://ogg.daria6918.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nva.jqgfzy.top

JS:   get name() { return this._name; }
来源：http://pyy.shzxlz.cn

TS:   get name(): string { return this._name; }
来源：http://fid.nanxinkj.top

Java: public String getName() { return name; }
来源：http://sjo.wangshuangyany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uvc.xuanzx.com

Ruby: attr_accessor :name
来源：http://aia.yj20258.top

C#:   public string Name { get; set; }
来源：http://gre.yuxming.cn

[G12] 对象转字符串
来源：http://twh.jinqigufen.top

Py:   def __str__(self): return self.name
来源：http://dtf.nwbrower.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://add.haohaochexian.top

JS:   toString() { return this.name; }
来源：http://gct.aibaodan.cn

TS:   toString(): string { return this.name; }
来源：http://nxz.hammf.cn

Java: @Override public String toString() { return name; }
来源：http://ris.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://wip.jqgufenzy.top

Ruby: def to_s; @name; end
来源：http://lbk.ydjk.org.cn

C#:   public override string ToString() => Name;
来源：http://gkf.cheryme.top

[G13] 判断对象类型
来源：http://dng.yueranfly.top

Py:   isinstance(u, User)
来源：http://nfg.xylfe.cn

PHP:  $u instanceof User
来源：http://wig.zdqjudy.top

JS:   u instanceof User
来源：http://njs.meibo888.top

TS:   u instanceof User
来源：http://hrq.9152youxi.cn

Java: u instanceof User
来源：http://oxg.haohaochexian.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pmj.fehbvm.com

Ruby: u.is_a?(User)
来源：http://fyb.guannengcc.top

C#:   u is User
来源：http://hde.sjlbkw.cn

[G14] 数据类 / record
来源：http://rmr.cqqwz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nmr.cashguo.top

PHP:  // 用 readonly 属性模拟
来源：http://iav.fehbvm.com

JS:   // 无内置：普通类或对象字面量
来源：http://vil.jyoumei.cn

TS:   type User = { name: string; age: number };
来源：http://xey.52xcode.cn

Java: record User(String name, int age) {}
来源：http://vwy.jianghu66.top

Go:   type User struct { Name string; Age int }
来源：http://btq.gotoacloud.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mgv.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://eas.hysaishi.cn

[G15] 枚举
来源：http://ymw.tianlin.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fsc.yonumen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://civ.jinyuanbaomall.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://azo.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qdj.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://ngv.daria6918.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jgv.vehdjk.com

Ruby: Color = %i[red green].freeze
来源：http://fcf.zhixingplan.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fgx.zycfv.cn

[G16] 对象转数组 / 字典
来源：http://uoe.jinqigufen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hwe.tarul.cn

PHP:  get_object_vars($obj);
来源：http://rvq.xingfuxueyuan.xyz

JS:   Object.entries(obj)
来源：http://nfu.fehbvm.com

TS:   Object.entries(obj)
来源：http://inw.vehdjk.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eid.zhoulong.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://epn.zhoulong.xyz

Ruby: obj.instance_variables
来源：http://adg.birdmap.top

C#:   // 用反射或 System.Text.Json
来源：http://vbv.xziqi.cn

================================================================================
来源：http://euk.yuanzhike.top

H. 异常与错误处理
来源：http://ngd.cashguo.top

================================================================================
来源：http://nua.yfazqb.com

[H01] try / catch 基础
来源：http://yzy.52xcode.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://evn.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://soh.tian-w.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cky.yangfankeji.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yay.xziqi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ygw.sufxvd.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uno.andypj.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ats.dianchejie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fkn.dashuyun.cn

[H02] finally / ensure 收尾
来源：http://rgf.zhijiandao.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vre.yj202588.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://llj.mhx1999.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fix.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://opc.yueranfly.top

Java: try { f(); } finally { cleanup(); }
来源：http://nwz.shangyingyoupin.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gjk.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ozd.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://myy.ehwqpu.com

[H03] 主动抛出异常
来源：http://xgm.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://hsv.yangfankeji.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rir.tarul.cn

JS:   throw new Error("错误信息");
来源：http://kxm.hammf.cn

TS:   throw new Error("错误信息");
来源：http://ohb.hnxiangtu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ske.jqgufenzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://syo.ehwqpu.com

Ruby: raise ArgumentError, "错误信息"
来源：http://eqi.shzxlz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ivb.gotoacloud.top

[H04] 自定义异常类型
来源：http://svr.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://vfn.jinqigufen.top

PHP:  class MyError extends RuntimeException {}
来源：http://tvc.fengsongda.top

JS:   class MyError extends Error {}
来源：http://bot.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://chg.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://gsu.iojbl.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xxd.fktsv.cn

Ruby: class MyError < StandardError; end
来源：http://xsw.sweek.top

C#:   class MyException : Exception {}
来源：http://yns.xuanzx.com

[H05] 捕获特定类型
来源：http://svx.yvedp.cn

Py:   except ValueError as e:
来源：http://wod.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vmb.dashuyun.cn

JS:   if (e instanceof TypeError) {}
来源：http://vik.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://kvh.cashguo.top

Java: catch (IOException | SQLException e) {}
来源：http://cuy.shuidangran.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nkk.yvedp.cn

Ruby: rescue ArgumentError => e
来源：http://foi.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oxy.tarul.cn

[H06] 可选值 / 空值安全访问
来源：http://mow.zhengqikj.top

Py:   value = d.get("k") or default
来源：http://fjj.sxryk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://esg.ybcxt.top

JS:   obj?.a?.b;  d ?? default
来源：http://jtv.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://tgn.fehbvm.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ftp.xylfe.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bsi.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://jcz.xingfuxueyuan.xyz

C#:   obj?.A?.B ?? default
来源：http://fgh.xziqi.cn

[H07] 断言
来源：http://nbd.tianlin.xyz

Py:   assert x > 0, "必须为正"
来源：http://vqa.dashuyun.cn

PHP:  assert($x > 0);
来源：http://flb.shangyingyoupin.top

JS:   console.assert(x > 0);
来源：http://fzc.shangyingyoupin.top

TS:   console.assert(x > 0);
来源：http://oej.pengpengdd.cyou

Java: assert x > 0 : "必须为正";
来源：http://thn.cucudq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vmd.jqgfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://ddd.yongpay.top

C#:   Debug.Assert(x > 0);
来源：http://fad.birdmap.top

[H08] 获取错误信息与堆栈
来源：http://fam.sweek.top

Py:   str(e);  traceback.format_exc()
来源：http://nqe.uphjek.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eon.hywenlv.cn

JS:   e.message;  e.stack
来源：http://gbg.kuanghao11.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://njc.chenlongwang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://sql.fehbvm.com

Go:   err.Error()
来源：http://sjh.hnxiangtu.top

Ruby: e.message;  e.backtrace
来源：http://mvn.316326.xyz

C#:   e.Message;  e.StackTrace
来源：http://zru.yj202588.top

[H09] 带错误码的异常
来源：http://qga.nwbrower.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xtc.xingfuxueyuan.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://dxm.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pjo.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ocq.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lel.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jmc.havefunace.top

Ruby: raise MyError.new("fail", 500)
来源：http://byy.smart0.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://kcq.jinghuilouyu.cn

[H10] 资源自动释放
来源：http://twf.uphjek.com


<!-- 参考信息 -->