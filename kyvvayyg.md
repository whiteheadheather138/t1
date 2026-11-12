代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://dwd.fzhhl.top

TS:   fs.unlinkSync("a.txt")
来源：http://zvw.guowangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kyh.zhijiandao.cn

Go:   os.Remove("a.txt")
来源：http://zmt.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://nqt.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://hsh.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://tch.vqdsnc.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nxi.tian-w.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rfc.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fat.chenzaomai.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vqv.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hlo.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xde.aibaodan.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fmw.ybcxt.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wys.nanxuanxn.top

[F08] 遍历目录
来源：http://odn.hammf.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bjn.hesvh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wea.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://vfm.bjfxy.top

TS:   fs.readdirSync("dir")
来源：http://dfe.sxryk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mog.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://lmg.redwolf501.top

Ruby: Dir.children("dir")
来源：http://rvq.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://cxc.fktsv.cn

[F09] 获取文件大小
来源：http://wua.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://npd.gogol.net.cn

PHP:  filesize("a.txt");
来源：http://hax.feifeiyinyue.top

JS:   fs.statSync("a.txt").size
来源：http://vvh.aibaodan.cn

TS:   fs.statSync("a.txt").size
来源：http://yus.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mib.yfazqb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rvi.cashguo.top

Ruby: File.size("a.txt")
来源：http://onf.snrcjt.cn

C#:   new FileInfo("a.txt").Length
来源：http://hkb.hysaishi.cn

[F10] 取文件扩展名 / 文件名
来源：http://sjh.ppjwa.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uxu.fanxiaobao.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ltc.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hfl.ybcxt.top

TS:   path.extname("a.txt")
来源：http://jyx.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://khk.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kqu.yvedp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kad.smart0.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zre.zhixingplan.top

[F11] 复制与移动文件
来源：http://udm.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fnu.fehbvm.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hvy.gaohongyu789.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://asf.xuetiantiany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jao.c1oappe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pic.meibo888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fce.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://abr.chenlongwang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://trh.yangfankeji.com

[F12] CSV 读写
来源：http://vpy.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zyu.shuidangran.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mvb.dianchejie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vxn.zycfv.cn

TS:   // 同上
来源：http://jql.ctjpmb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sys.daria6918.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iks.fzhhl.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yls.ydzc1.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lgp.yj202588.top

================================================================================
来源：http://uob.yongpay.top

G. 面向对象
来源：http://chn.zhixingplan.top

================================================================================
来源：http://gnz.gogol.net.cn

[G01] 定义类
来源：http://uwk.jinqigufen.top

Py:   class User: pass
来源：http://brh.meibo888.top

PHP:  class User {}
来源：http://xxp.yj202588.top

JS:   class User {}
来源：http://tmp.yuxming.cn

TS:   class User { name: string = ""; }
来源：http://rcj.meibo888.top

Java: class User {}
来源：http://fje.tanke756.top

Go:   type User struct { Name string }
来源：http://yym.jqgufenzy.top

Ruby: class User; end
来源：http://ddj.hywenlv.cn

C#:   class User {}
来源：http://zva.shuidangran.top

[G02] 构造函数
来源：http://vaa.shzxlz.cn

Py:   def __init__(self, name): self.name = name
来源：http://lzv.zhixingplan.top

PHP:  public function __construct(public string $name) {}
来源：http://wpl.iojbl.cn

JS:   constructor(name) { this.name = name; }
来源：http://osy.nanxinkj.top

TS:   constructor(public name: string) {}
来源：http://nbd.yueranfly.top

Java: User(String name) { this.name = name; }
来源：http://lns.feifeiyinyue.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nox.svipenyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://jqs.sxryk.cn

C#:   public User(string name) { Name = name; }
来源：http://npf.52xcode.cn

[G03] 实例属性
来源：http://iul.sjlbkw.cn

Py:   self.name = "x"
来源：http://odl.vqdsnc.cn

PHP:  public string $name = "x";
来源：http://qir.ydzc1.top

JS:   this.name = "x";
来源：http://gtd.smart0.xyz

TS:   name: string = "x";
来源：http://rkm.zhoulong.xyz

Java: private String name;
来源：http://pra.hywenlv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fhg.xziqi.cn

Ruby: @name = "x"
来源：http://uas.dashuyun.cn

C#:   public string Name { get; set; } = "x";
来源：http://moc.daxiang520.top

[G04] 定义方法
来源：http://pvb.dianchejie.cn

Py:   def greet(self): return self.name
来源：http://mak.zdbjq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bxr.haohaochexian.top

JS:   greet() { return this.name; }
来源：http://jvh.cucudq.cn

TS:   greet(): string { return this.name; }
来源：http://wyu.sxryk.cn

Java: String greet() { return name; }
来源：http://sux.chenjidiqi.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://cbu.vqdsnc.cn

Ruby: def greet; @name; end
来源：http://ixb.yj20258.top

C#:   public string Greet() => Name;
来源：http://gtg.zhixingplan.top

[G05] 继承
来源：http://zvq.tarul.cn

Py:   class Admin(User): pass
来源：http://mge.hammf.cn

PHP:  class Admin extends User {}
来源：http://cqf.dashuyun.cn

JS:   class Admin extends User {}
来源：http://bqb.cheryme.top

TS:   class Admin extends User {}
来源：http://jln.yonumen.top

Java: class Admin extends User {}
来源：http://arh.hesvh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oml.guannengcc.top

Ruby: class Admin < User; end
来源：http://roa.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://wga.hongshengwenyu.top

[G06] 重写方法
来源：http://ppj.zycfv.cn

Py:   def greet(self): return "admin"
来源：http://iow.chenzaomai.com

PHP:  public function greet(): string { return "admin"; }
来源：http://ojc.fanxiaobao.xyz

JS:   greet() { return "admin"; }
来源：http://ned.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://qdi.jqgfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://lwe.cdnleiting.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bso.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://iga.nanxuanxn.top

C#:   public override string Greet() => "admin";
来源：http://vtl.yanxiufei.cn

[G07] 调用父类方法
来源：http://bmm.meibo888.top

Py:   super().greet()
来源：http://hbw.meibo888.top

PHP:  parent::greet();
来源：http://jec.yj202588.top

JS:   super.greet();
来源：http://hcw.nanxinkj.top

TS:   super.greet();
来源：http://dpb.shanyushiyangtech.top

Java: super.greet();
来源：http://zsv.xuetiantiany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zjd.haohaochexian.top

Ruby: super
来源：http://ltn.jinghuilouyu.cn

C#:   base.Greet();
来源：http://ljz.zhixingplan.top

[G08] 静态方法与属性
来源：http://ldr.xinyue.icu

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tnq.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://fga.nanxuanxn.top

JS:   static f() {}
来源：http://plu.yfazqb.com

TS:   static f(): void {}
来源：http://kst.quarkkingdee.top

Java: static void f() {}
来源：http://fmg.andypj.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://xqw.yj20258888.top

Ruby: def self.f; end
来源：http://goi.zhijiandao.cn

C#:   public static void F() {}
来源：http://zsi.jlsjyb.cn

[G09] 接口 / 抽象类
来源：http://kra.pycfn.com

Py:   from abc import ABC, abstractmethod
来源：http://aug.xinyue.icu

PHP:  interface Shape { public function area(): float; }
来源：http://adh.feifeiyinyue.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yjr.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://pcj.fktsv.cn

Java: interface Shape { double area(); }
来源：http://xnu.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://mks.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lbx.ivvv.top

C#:   interface IShape { double Area(); }
来源：http://eui.hesvh.cn

[G10] 访问控制
来源：http://lax.jinqigfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://kra.feifeiyinyue.top

PHP:  public / protected / private
来源：http://mqb.iojbl.cn

JS:   #private 字段；其余公开
来源：http://rap.hesvh.cn

TS:   public / protected / private
来源：http://tvl.gotoacloud.top

Java: public / protected / private / 默认包级
来源：http://qhf.gotoacloud.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uxm.xziqi.cn

Ruby: public / protected / private
来源：http://gdv.gzhubu.top

C#:   public / protected / private / internal
来源：http://ejn.shzxlz.cn

[G11] getter / setter
来源：http://ycr.shangyingyoupin.top

Py:   @property 与 @x.setter
来源：http://rbl.yuanzhike.top

PHP:  public function getName(): string { return $this->name; }
来源：http://veg.tianlin.xyz

JS:   get name() { return this._name; }
来源：http://peh.ybcxt.top

TS:   get name(): string { return this._name; }
来源：http://dvl.cucudq.cn

Java: public String getName() { return name; }
来源：http://qad.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mxf.aibaodan.cn

Ruby: attr_accessor :name
来源：http://vxb.cucudq.cn

C#:   public string Name { get; set; }
来源：http://rtr.jyoumei.cn

[G12] 对象转字符串
来源：http://lct.zdbjq.cn

Py:   def __str__(self): return self.name
来源：http://vko.jlsjyb.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jvi.nanxuanxn.top

JS:   toString() { return this.name; }
来源：http://bzr.ctjpmb.com

TS:   toString(): string { return this.name; }
来源：http://fou.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://lhy.wangdashe.top

Go:   func (u User) String() string { return u.Name }
来源：http://uao.jinghuilouyu.cn

Ruby: def to_s; @name; end
来源：http://gbn.yj202588.top

C#:   public override string ToString() => Name;
来源：http://ele.c1oappe.top

[G13] 判断对象类型
来源：http://moi.gaohongyu789.top

Py:   isinstance(u, User)
来源：http://zes.hnqzz.top

PHP:  $u instanceof User
来源：http://kmm.hammf.cn

JS:   u instanceof User
来源：http://ezm.svipenyu.cn

TS:   u instanceof User
来源：http://qbn.yj202588.top

Java: u instanceof User
来源：http://obg.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://eks.zycfv.cn

Ruby: u.is_a?(User)
来源：http://umq.hammf.cn

C#:   u is User
来源：http://xyy.sweek.top

[G14] 数据类 / record
来源：http://rzl.nwbrower.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://saz.vehdjk.com

PHP:  // 用 readonly 属性模拟
来源：http://yvf.yj20258888.top

JS:   // 无内置：普通类或对象字面量
来源：http://lba.daxiang520.top

TS:   type User = { name: string; age: number };
来源：http://dcq.cheryme.top

Java: record User(String name, int age) {}
来源：http://tma.shzxlz.cn

Go:   type User struct { Name string; Age int }
来源：http://lwx.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ywg.ydjk.org.cn

C#:   record User(string Name, int Age);
来源：http://qor.tarul.cn

[G15] 枚举
来源：http://nil.zhengqikj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fly.316326.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://eqn.hywenlv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vut.sweek.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eeq.feifeiyinyue.top

Java: enum Color { RED, GREEN }
来源：http://xvm.yuanzhike.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zyx.shanyushiyangtech.top

Ruby: Color = %i[red green].freeze
来源：http://olk.ehwqpu.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gxt.hnxiangtu.top

[G16] 对象转数组 / 字典
来源：http://itb.vqdsnc.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://twj.shanyushiyangkeji.top

PHP:  get_object_vars($obj);
来源：http://fwn.fehbvm.com

JS:   Object.entries(obj)
来源：http://hth.jqgufenzy.top

TS:   Object.entries(obj)
来源：http://qcx.hnxiangtu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jad.zhaomingkeji.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://soq.haohaochexian.top

Ruby: obj.instance_variables
来源：http://otg.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://pjl.52xcode.cn

================================================================================
来源：http://wml.nanxuanxn.top

H. 异常与错误处理
来源：http://gyi.hammf.cn

================================================================================
来源：http://osj.fktsv.cn

[H01] try / catch 基础
来源：http://wpf.fzhhl.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fis.bbcook.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jym.vqdsnc.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xju.jianghu66.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qxs.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cyl.yangfankeji.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hqv.zhongyouzk.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xqg.52xcode.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gxj.daxiang520.top

[H02] finally / ensure 收尾
来源：http://sas.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://rud.nanxinkj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ezf.hywenlv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yeq.52xcode.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://idr.dianchejie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nny.gzhubu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tbx.quarkkingdee.top

Ruby: begin; f; ensure; cleanup; end
来源：http://iml.shanyushiyangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ryh.ehwqpu.com

[H03] 主动抛出异常
来源：http://fgx.hcnkem.com

Py:   raise ValueError("错误信息")
来源：http://hqx.andypj.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qlw.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://lic.zhiwuduotai.top

TS:   throw new Error("错误信息");
来源：http://nse.feifeiyinyue.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://yrs.feifeiyinyue.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://imb.ppjwa.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://unj.yongpay.top

C#:   throw new ArgumentException("错误信息");
来源：http://arf.shuidangran.top

[H04] 自定义异常类型
来源：http://cbt.xylfe.cn

Py:   class MyError(Exception): pass
来源：http://aph.tanke756.top

PHP:  class MyError extends RuntimeException {}
来源：http://yzs.zhijiandao.cn

JS:   class MyError extends Error {}
来源：http://jdy.andypj.xyz

TS:   class MyError extends Error {}
来源：http://eyr.jinyuanbaomall.cn

Java: class MyException extends RuntimeException {}
来源：http://wpx.gotoacloud.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cho.jinyuanbaomall.cn

Ruby: class MyError < StandardError; end
来源：http://uak.c1oappe.top

C#:   class MyException : Exception {}
来源：http://jeb.hcnkem.com

[H05] 捕获特定类型
来源：http://iyk.hfpthk.cn

Py:   except ValueError as e:
来源：http://nrv.vehdjk.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jbq.smart0.xyz

JS:   if (e instanceof TypeError) {}
来源：http://vgh.epnwcf.com

TS:   if (e instanceof TypeError) {}
来源：http://nrz.pengpengdd.cyou

Java: catch (IOException | SQLException e) {}
来源：http://kph.nanxuanxn.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cvs.yj202588.top

Ruby: rescue ArgumentError => e
来源：http://rgr.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kvp.xuanzx.com

[H06] 可选值 / 空值安全访问
来源：http://onb.tianlin.xyz

Py:   value = d.get("k") or default
来源：http://lhc.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qpn.shzxlz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yat.ctjpmb.com

TS:   obj?.a?.b;  d ?? default
来源：http://pvs.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vpb.0kj1m.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://itn.wangdashe.top

Ruby: d&.dig(:a, :b)
来源：http://dnm.mhx1999.top

C#:   obj?.A?.B ?? default
来源：http://xnb.fehbvm.com

[H07] 断言
来源：http://duw.dashuyun.cn

Py:   assert x > 0, "必须为正"
来源：http://fxu.xziqi.cn

PHP:  assert($x > 0);
来源：http://vyh.fengsongda.top

JS:   console.assert(x > 0);
来源：http://wcu.ywan-chungtsiang.top

TS:   console.assert(x > 0);
来源：http://avb.chenlongwang.top

Java: assert x > 0 : "必须为正";
来源：http://mzn.bjfxy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ecn.jqgufenzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://urp.cucudq.cn

C#:   Debug.Assert(x > 0);
来源：http://mya.yongpay.top

[H08] 获取错误信息与堆栈
来源：http://uwg.sysykeji.top

Py:   str(e);  traceback.format_exc()
来源：http://eir.dashuyun.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zun.yj202588.top

JS:   e.message;  e.stack
来源：http://zzg.mhx1999.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xpf.feifeiyinyue.top

Java: e.getMessage();  e.printStackTrace()
来源：http://frw.yuxming.cn

Go:   err.Error()
来源：http://jej.vqdsnc.cn

Ruby: e.message;  e.backtrace
来源：http://akq.jinyuanbaomall.cn

C#:   e.Message;  e.StackTrace
来源：http://usv.dashuyun.cn

[H09] 带错误码的异常
来源：http://gfd.jyoumei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hgh.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://akm.shangyingyoupin.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hog.c1oappe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ckf.fengsongda.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bnc.cheryme.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mop.yangfankeji.com

Ruby: raise MyError.new("fail", 500)
来源：http://yll.gaohongyu789.top

C#:   // 自定义异常类中加 Code 属性
来源：http://teu.tian-w.cn

[H10] 资源自动释放
来源：http://fzk.sysykeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://crj.sufxvd.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rjx.hysaishi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://slj.vehdjk.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dhe.zdqjudy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://apm.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://wii.tianlin.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dnr.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dww.fehbvm.com


<!-- 参考信息 -->