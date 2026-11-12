代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://nrp.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ewz.ctjpmb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lwn.chenlongwang.top

Ruby: File.exist?("a.txt")
来源：http://chf.quarkkingdee.top

C#:   File.Exists("a.txt")
来源：http://zlw.zhiwuduotai.top

[F06] 删除文件
来源：http://dle.dianchejie.cn

Py:   os.remove("a.txt")
来源：http://zwn.yongpay.top

PHP:  unlink("a.txt");
来源：http://hdv.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://tqs.yanxiufei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zms.gzhubu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://twe.vqdsnc.cn

Go:   os.Remove("a.txt")
来源：http://dwb.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://ygp.smart0.xyz

C#:   File.Delete("a.txt");
来源：http://imu.tian-w.cn

[F07] 创建目录（含多级）
来源：http://ued.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sel.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uoy.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qho.guannengcc.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tvm.kuanghao11.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gus.zhixingplan.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nlz.gaohongyu789.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pzs.yj202588.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://azk.pycfn.com

[F08] 遍历目录
来源：http://ood.shuidangran.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rjm.hongshengwenyu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fbc.yj20258888.top

JS:   fs.readdirSync("dir")
来源：http://hiv.ywan-chungtsiang.top

TS:   fs.readdirSync("dir")
来源：http://lwv.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kwy.hcnkem.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://cfv.jinqigufen.top

Ruby: Dir.children("dir")
来源：http://fbf.cucudq.cn

C#:   Directory.GetFiles("dir")
来源：http://hhl.xuanzx.com

[F09] 获取文件大小
来源：http://amt.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://oeo.gaohongyu789.top

PHP:  filesize("a.txt");
来源：http://gem.fzhhl.top

JS:   fs.statSync("a.txt").size
来源：http://cpr.zycfv.cn

TS:   fs.statSync("a.txt").size
来源：http://wme.yuanzhike.top

Java: Files.size(Path.of("a.txt"))
来源：http://ddv.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gvi.redwolf501.top

Ruby: File.size("a.txt")
来源：http://zwe.svipenyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://uic.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://npd.shanyushiyangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bto.shuidangran.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ywj.yueranfly.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jny.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://jrx.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yos.aibaodan.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jky.gaohongyu789.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kbu.cqqwz.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cdo.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://qzp.yuanzhike.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://clx.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zvi.shuidangran.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cvt.uphjek.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ghl.nwbrower.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ewc.ctjpmb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cdv.yangfankeji.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pki.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://adr.svipenyu.cn

[F12] CSV 读写
来源：http://hqx.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zax.aizwys.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jvr.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://otb.guannengcc.top

TS:   // 同上
来源：http://zul.havefunace.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uhn.ehwqpu.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://asu.hysaishi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jar.cashguo.top

C#:   // 无内置：用 CsvHelper 库
来源：http://yyx.sweek.top

================================================================================
来源：http://obf.sxryk.cn

G. 面向对象
来源：http://xgb.shuidangran.top

================================================================================
来源：http://lau.yuanzhike.top

[G01] 定义类
来源：http://loc.redwolf501.top

Py:   class User: pass
来源：http://iio.ydjk.org.cn

PHP:  class User {}
来源：http://qov.xingfuxueyuan.xyz

JS:   class User {}
来源：http://fab.andypj.xyz

TS:   class User { name: string = ""; }
来源：http://qgw.yonumen.top

Java: class User {}
来源：http://ios.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://aen.jqgfzy.top

Ruby: class User; end
来源：http://wxu.meibo888.top

C#:   class User {}
来源：http://cxo.havefunace.top

[G02] 构造函数
来源：http://vot.fanxiaobao.xyz

Py:   def __init__(self, name): self.name = name
来源：http://obl.9152youxi.cn

PHP:  public function __construct(public string $name) {}
来源：http://oxp.hysaishi.cn

JS:   constructor(name) { this.name = name; }
来源：http://hhu.chenzaomai.com

TS:   constructor(public name: string) {}
来源：http://hsv.shanyushiyangtech.top

Java: User(String name) { this.name = name; }
来源：http://dbr.sysykeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bpv.jianghu66.top

Ruby: def initialize(name); @name = name; end
来源：http://upy.ybcxt.top

C#:   public User(string name) { Name = name; }
来源：http://yrr.ydzc1.top

[G03] 实例属性
来源：http://eis.vehdjk.com

Py:   self.name = "x"
来源：http://wuf.zhongyouzk.top

PHP:  public string $name = "x";
来源：http://hjy.fanxiaobao.xyz

JS:   this.name = "x";
来源：http://jpl.316326.xyz

TS:   name: string = "x";
来源：http://krl.jiagoushi.top

Java: private String name;
来源：http://zqk.52xcode.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://abx.vehdjk.com

Ruby: @name = "x"
来源：http://mxa.jqgufenzy.top

C#:   public string Name { get; set; } = "x";
来源：http://mdi.ywan-chungtsiang.top

[G04] 定义方法
来源：http://ahg.sysykeji.top

Py:   def greet(self): return self.name
来源：http://ulr.jinghuilouyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://upi.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://qyl.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://scg.ywan-chungtsiang.top

Java: String greet() { return name; }
来源：http://nwy.9152youxi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ryg.ydzc1.top

Ruby: def greet; @name; end
来源：http://llj.smart0.xyz

C#:   public string Greet() => Name;
来源：http://ozg.aizwys.cn

[G05] 继承
来源：http://vzd.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://lxu.yj20258.top

PHP:  class Admin extends User {}
来源：http://plu.zhoulong.xyz

JS:   class Admin extends User {}
来源：http://tur.fktsv.cn

TS:   class Admin extends User {}
来源：http://upl.havefunace.top

Java: class Admin extends User {}
来源：http://xyh.zhengqikj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fln.yueranfly.top

Ruby: class Admin < User; end
来源：http://mgj.jinqigufen.top

C#:   class Admin : User {}
来源：http://mwd.xuanzx.com

[G06] 重写方法
来源：http://gkw.yj20258.top

Py:   def greet(self): return "admin"
来源：http://iyv.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rvm.ywan-chungtsiang.top

JS:   greet() { return "admin"; }
来源：http://nus.gogol.net.cn

TS:   greet(): string { return "admin"; }
来源：http://gdm.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://abi.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hyl.jinyuanbaomall.cn

Ruby: def greet; "admin"; end
来源：http://plq.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://ijc.316326.xyz

[G07] 调用父类方法
来源：http://uam.xylfe.cn

Py:   super().greet()
来源：http://lhb.ybcxt.top

PHP:  parent::greet();
来源：http://ymj.hesvh.cn

JS:   super.greet();
来源：http://nni.kuanghao11.cn

TS:   super.greet();
来源：http://axa.quarkkingdee.top

Java: super.greet();
来源：http://qif.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://goj.zhijiandao.cn

Ruby: super
来源：http://fnm.tanke756.top

C#:   base.Greet();
来源：http://oor.yonumen.top

[G08] 静态方法与属性
来源：http://jzz.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tpm.yuxming.cn

PHP:  public static function f() {}
来源：http://odj.nanxuanxn.top

JS:   static f() {}
来源：http://nsr.yanxiufei.cn

TS:   static f(): void {}
来源：http://tno.aibaodan.cn

Java: static void f() {}
来源：http://tbu.fehbvm.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://gyi.uphjek.com

Ruby: def self.f; end
来源：http://hon.sysykeji.top

C#:   public static void F() {}
来源：http://mge.smart0.xyz

[G09] 接口 / 抽象类
来源：http://uys.zhoulong.xyz

Py:   from abc import ABC, abstractmethod
来源：http://bpv.daria6918.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gbz.nwbrower.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xap.jqgfzy.top

TS:   interface Shape { area(): number; }
来源：http://rci.chenzaomai.com

Java: interface Shape { double area(); }
来源：http://eam.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://usk.ydjk.org.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://irb.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://utb.yj20258888.top

[G10] 访问控制
来源：http://eoi.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://zcn.birdmap.top

PHP:  public / protected / private
来源：http://kzr.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://axt.zdbjq.cn

TS:   public / protected / private
来源：http://bdc.zhiwuduotai.top

Java: public / protected / private / 默认包级
来源：http://umz.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://amm.xinyue.icu

Ruby: public / protected / private
来源：http://tnp.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://ert.smart0.xyz

[G11] getter / setter
来源：http://mwg.nwbrower.top

Py:   @property 与 @x.setter
来源：http://wnp.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nry.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://jpb.zdbjq.cn

TS:   get name(): string { return this._name; }
来源：http://nif.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://tpr.xziqi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qga.hywenlv.cn

Ruby: attr_accessor :name
来源：http://nuv.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://zpo.xylfe.cn

[G12] 对象转字符串
来源：http://esv.zdqjudy.top

Py:   def __str__(self): return self.name
来源：http://gmq.c1oappe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wsr.cashguo.top

JS:   toString() { return this.name; }
来源：http://sss.zycfv.cn

TS:   toString(): string { return this.name; }
来源：http://krh.cashguo.top

Java: @Override public String toString() { return name; }
来源：http://ifw.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://mns.zhiwuduotai.top

Ruby: def to_s; @name; end
来源：http://ghh.daxiang520.top

C#:   public override string ToString() => Name;
来源：http://lle.yangfankeji.com

[G13] 判断对象类型
来源：http://hhx.fktsv.cn

Py:   isinstance(u, User)
来源：http://efu.sxryk.cn

PHP:  $u instanceof User
来源：http://geo.fzhhl.top

JS:   u instanceof User
来源：http://mod.ywan-chungtsiang.top

TS:   u instanceof User
来源：http://xmy.fengsongda.top

Java: u instanceof User
来源：http://onf.bbcook.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hur.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://xgm.yvedp.cn

C#:   u is User
来源：http://ozs.xylfe.cn

[G14] 数据类 / record
来源：http://ads.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://urp.daria6918.cn

PHP:  // 用 readonly 属性模拟
来源：http://khm.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qof.fengsongda.top

TS:   type User = { name: string; age: number };
来源：http://yjg.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://guj.yonumen.top

Go:   type User struct { Name string; Age int }
来源：http://bwm.vehdjk.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gcg.ydjk.org.cn

C#:   record User(string Name, int Age);
来源：http://cjt.hcnkem.com

[G15] 枚举
来源：http://rii.chenlongwang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kny.aibaodan.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wie.yj20258.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sfw.kuanghao11.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rbf.jyoumei.cn

Java: enum Color { RED, GREEN }
来源：http://tbd.tian-w.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lbj.tianlin.xyz

Ruby: Color = %i[red green].freeze
来源：http://ply.uphjek.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lah.jlsjyb.cn

[G16] 对象转数组 / 字典
来源：http://yjr.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://arq.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://ill.fanxiaobao.xyz

JS:   Object.entries(obj)
来源：http://jsj.meibo888.top

TS:   Object.entries(obj)
来源：http://elg.jlsjyb.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mzv.snrcjt.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://aam.yj20258888.top

Ruby: obj.instance_variables
来源：http://ujs.fengsongda.top

C#:   // 用反射或 System.Text.Json
来源：http://qnf.epnwcf.com

================================================================================
来源：http://jxn.sufxvd.cn

H. 异常与错误处理
来源：http://bsq.gogol.net.cn

================================================================================
来源：http://ffg.redwolf501.top

[H01] try / catch 基础
来源：http://atd.yangfankeji.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uwj.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://doa.fehbvm.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iyj.jqgufenzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lcb.hnxiangtu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aci.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://opq.iojbl.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zwg.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zxb.gotoacloud.top

[H02] finally / ensure 收尾
来源：http://ecd.ybcxt.top

Py:   try: f()⏎finally: cleanup()
来源：http://euf.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yin.ydzc1.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mhg.hammf.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qlw.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://otg.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ruw.jqgufenzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://iad.zhoulong.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://lpp.birdmap.top

[H03] 主动抛出异常
来源：http://nre.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://ndx.guowangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dpi.sufxvd.cn

JS:   throw new Error("错误信息");
来源：http://unx.aizwys.cn

TS:   throw new Error("错误信息");
来源：http://gwr.daxiang520.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nqh.316326.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cak.pengpengdd.cyou

Ruby: raise ArgumentError, "错误信息"
来源：http://eyy.mhx1999.top

C#:   throw new ArgumentException("错误信息");
来源：http://rst.kuanghao11.cn

[H04] 自定义异常类型
来源：http://ret.pengpengdd.cyou

Py:   class MyError(Exception): pass
来源：http://uhm.cqqwz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jbl.hongshengwenyu.top

JS:   class MyError extends Error {}
来源：http://vlr.zhaomingkeji.xyz

TS:   class MyError extends Error {}
来源：http://hys.yj20258.top

Java: class MyException extends RuntimeException {}
来源：http://bdq.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dft.yanxiufei.cn

Ruby: class MyError < StandardError; end
来源：http://bwt.jyoumei.cn

C#:   class MyException : Exception {}
来源：http://kbq.zhongyouzk.top

[H05] 捕获特定类型
来源：http://tew.epnwcf.com

Py:   except ValueError as e:
来源：http://vuf.pycfn.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xul.svipenyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://tdt.ydzc1.top

TS:   if (e instanceof TypeError) {}
来源：http://yfk.nanxuanxn.top

Java: catch (IOException | SQLException e) {}
来源：http://zhq.smart0.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zpn.sysykeji.top

Ruby: rescue ArgumentError => e
来源：http://vob.zhaomingkeji.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://grq.cqqwz.cn

[H06] 可选值 / 空值安全访问
来源：http://vtc.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://pzn.vqdsnc.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nep.cqqwz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dgd.dianchejie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cpp.fehbvm.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qhe.vqdsnc.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sai.cashguo.top

Ruby: d&.dig(:a, :b)
来源：http://ntp.jqgufenzy.top

C#:   obj?.A?.B ?? default
来源：http://wok.zdbjq.cn

[H07] 断言
来源：http://bag.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://uak.jqgfzy.top

PHP:  assert($x > 0);
来源：http://gdl.daria6918.cn

JS:   console.assert(x > 0);
来源：http://lup.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://urv.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://koz.fehbvm.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://znc.wangdashe.top

Ruby: raise "必须为正" unless x > 0
来源：http://rpo.xuanzx.com

C#:   Debug.Assert(x > 0);
来源：http://xiv.kuanghao11.cn

[H08] 获取错误信息与堆栈
来源：http://mgi.xziqi.cn

Py:   str(e);  traceback.format_exc()
来源：http://isq.vqdsnc.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lmt.0kj1m.cn

JS:   e.message;  e.stack
来源：http://ocj.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xer.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vgk.epnwcf.com

Go:   err.Error()
来源：http://sxy.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://hth.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://qxc.316326.xyz

[H09] 带错误码的异常
来源：http://vil.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tvq.xinyue.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://fcu.jyoumei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://paa.jyoumei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://arb.jinyuanbaomall.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qij.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gkt.redwolf501.top

Ruby: raise MyError.new("fail", 500)
来源：http://qrh.yuxming.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zau.jqgfzy.top

[H10] 资源自动释放
来源：http://suv.birdmap.top


<!-- 参考信息 -->