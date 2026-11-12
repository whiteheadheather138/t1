代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://wei.c1oappe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://iic.ivvv.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bme.andypj.xyz

Ruby: File.exist?("a.txt")
来源：http://mjt.gzhubu.top

C#:   File.Exists("a.txt")
来源：http://rqh.yj202588.top

[F06] 删除文件
来源：http://aca.cashguo.top

Py:   os.remove("a.txt")
来源：http://pjj.guowangkeji.top

PHP:  unlink("a.txt");
来源：http://ptc.316326.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://usj.epnwcf.com

TS:   fs.unlinkSync("a.txt")
来源：http://xmv.havefunace.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ljb.shanyushiyangkeji.top

Go:   os.Remove("a.txt")
来源：http://nws.gogol.net.cn

Ruby: File.delete("a.txt")
来源：http://ydn.hnqzz.top

C#:   File.Delete("a.txt");
来源：http://yyg.meibo888.top

[F07] 创建目录（含多级）
来源：http://bkq.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rjc.havefunace.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://seh.zhoulong.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://foa.c1oappe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://grs.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tkd.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://csx.jinqigufen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dha.jianghu66.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qat.yfazqb.com

[F08] 遍历目录
来源：http://agd.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://cjs.c1oappe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tor.haohaochexian.top

JS:   fs.readdirSync("dir")
来源：http://efp.gogol.net.cn

TS:   fs.readdirSync("dir")
来源：http://tqp.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pmx.hysaishi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://aoi.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://hds.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://yjt.jinyuanbaomall.cn

[F09] 获取文件大小
来源：http://hpx.fanxiaobao.xyz

Py:   os.path.getsize("a.txt")
来源：http://aih.nwbrower.top

PHP:  filesize("a.txt");
来源：http://tsk.pycfn.com

JS:   fs.statSync("a.txt").size
来源：http://ups.zycfv.cn

TS:   fs.statSync("a.txt").size
来源：http://qng.zhaomingkeji.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://xhr.xylfe.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tsi.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://tlk.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://kdh.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://wfi.shanyushiyangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sip.hcnkem.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nsl.yanxiufei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aoj.bjfxy.top

TS:   path.extname("a.txt")
来源：http://xys.jlsjyb.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ene.fzhhl.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eiz.yuxming.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ayb.sweek.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ieg.xziqi.cn

[F11] 复制与移动文件
来源：http://pew.wangdashe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://smk.guowangkeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vki.ybcxt.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wul.ppjwa.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nwu.xingfuxueyuan.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://obn.yj20258888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fph.sjlbkw.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ahn.ybcxt.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gxe.9152youxi.cn

[F12] CSV 读写
来源：http://apn.snrcjt.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xbi.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ejp.gaohongyu789.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rhp.zycfv.cn

TS:   // 同上
来源：http://eqh.fktsv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uaj.tanke756.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://svx.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kel.quarkkingdee.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hzn.wangdashe.top

================================================================================
来源：http://dmu.ydjk.org.cn

G. 面向对象
来源：http://ipb.redwolf501.top

================================================================================
来源：http://efg.smart0.xyz

[G01] 定义类
来源：http://awa.yuanzhike.top

Py:   class User: pass
来源：http://szz.tian-w.cn

PHP:  class User {}
来源：http://raq.cdnleiting.top

JS:   class User {}
来源：http://qbw.smart0.xyz

TS:   class User { name: string = ""; }
来源：http://qbp.vqdsnc.cn

Java: class User {}
来源：http://jkq.gzhubu.top

Go:   type User struct { Name string }
来源：http://qqm.jqgufenzy.top

Ruby: class User; end
来源：http://nao.xinyue.icu

C#:   class User {}
来源：http://xdi.wangdashe.top

[G02] 构造函数
来源：http://lbl.guannengcc.top

Py:   def __init__(self, name): self.name = name
来源：http://wkm.tian-w.cn

PHP:  public function __construct(public string $name) {}
来源：http://tqw.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://qsd.52xcode.cn

TS:   constructor(public name: string) {}
来源：http://bxz.zhiwuduotai.top

Java: User(String name) { this.name = name; }
来源：http://qas.jinghuilouyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wpp.smart0.xyz

Ruby: def initialize(name); @name = name; end
来源：http://yhf.ctjpmb.com

C#:   public User(string name) { Name = name; }
来源：http://wdn.yuxming.cn

[G03] 实例属性
来源：http://asy.redwolf501.top

Py:   self.name = "x"
来源：http://uvz.yangfankeji.com

PHP:  public string $name = "x";
来源：http://zdv.sxryk.cn

JS:   this.name = "x";
来源：http://rul.haohaochexian.top

TS:   name: string = "x";
来源：http://opb.wangshuangyany.cn

Java: private String name;
来源：http://ftd.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gjs.xingfuxueyuan.xyz

Ruby: @name = "x"
来源：http://ylj.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://fgb.aizwys.cn

[G04] 定义方法
来源：http://kif.chenzaomai.com

Py:   def greet(self): return self.name
来源：http://jdr.yuxming.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ife.chenjidiqi.icu

JS:   greet() { return this.name; }
来源：http://udw.daxiang520.top

TS:   greet(): string { return this.name; }
来源：http://cjk.zycfv.cn

Java: String greet() { return name; }
来源：http://nxd.zhaomingkeji.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://agh.zhongyouzk.top

Ruby: def greet; @name; end
来源：http://bvk.smart0.xyz

C#:   public string Greet() => Name;
来源：http://xmm.xuanzx.com

[G05] 继承
来源：http://cta.xziqi.cn

Py:   class Admin(User): pass
来源：http://iaa.nwbrower.top

PHP:  class Admin extends User {}
来源：http://uff.nwbrower.top

JS:   class Admin extends User {}
来源：http://lqo.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://iwy.hywenlv.cn

Java: class Admin extends User {}
来源：http://bsg.xziqi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hdj.gotoacloud.top

Ruby: class Admin < User; end
来源：http://wbn.chenjidiqi.icu

C#:   class Admin : User {}
来源：http://zwe.jinyuanbaomall.cn

[G06] 重写方法
来源：http://tyt.ydjk.org.cn

Py:   def greet(self): return "admin"
来源：http://exo.vqdsnc.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kxk.havefunace.top

JS:   greet() { return "admin"; }
来源：http://fbe.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://rcw.guannengcc.top

Java: @Override String greet() { return "admin"; }
来源：http://jde.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ryu.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://qit.zdqjudy.top

C#:   public override string Greet() => "admin";
来源：http://djr.dianchejie.cn

[G07] 调用父类方法
来源：http://ywg.andypj.xyz

Py:   super().greet()
来源：http://ldb.tanke756.top

PHP:  parent::greet();
来源：http://skb.shanyushiyangtech.top

JS:   super.greet();
来源：http://tug.ivvv.top

TS:   super.greet();
来源：http://beh.yj20258.top

Java: super.greet();
来源：http://ypf.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://deo.gaohongyu789.top

Ruby: super
来源：http://onw.cdnleiting.top

C#:   base.Greet();
来源：http://qyr.xuanzx.com

[G08] 静态方法与属性
来源：http://snj.dianchejie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cjz.ctjpmb.com

PHP:  public static function f() {}
来源：http://xts.cucudq.cn

JS:   static f() {}
来源：http://bet.jiagoushi.top

TS:   static f(): void {}
来源：http://jld.svipenyu.cn

Java: static void f() {}
来源：http://xwj.52xcode.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eel.jinghuilouyu.cn

Ruby: def self.f; end
来源：http://tlm.xuanzx.com

C#:   public static void F() {}
来源：http://vle.svipenyu.cn

[G09] 接口 / 抽象类
来源：http://uwo.feifeiyinyue.top

Py:   from abc import ABC, abstractmethod
来源：http://vmr.wangshuangyany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fiv.snrcjt.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sjn.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://nxm.pycfn.com

Java: interface Shape { double area(); }
来源：http://hxh.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://vvd.zhongyouzk.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zcl.guowangkeji.top

C#:   interface IShape { double Area(); }
来源：http://qdm.svipenyu.cn

[G10] 访问控制
来源：http://qxc.shanyushiyangtech.top

Py:   约定 _protected / __private（不强制）
来源：http://eik.ydzc1.top

PHP:  public / protected / private
来源：http://gbj.chenzaomai.com

JS:   #private 字段；其余公开
来源：http://ztl.sxryk.cn

TS:   public / protected / private
来源：http://xwv.daxiang520.top

Java: public / protected / private / 默认包级
来源：http://iby.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://ssk.yj20258888.top

Ruby: public / protected / private
来源：http://csg.jqgufenzy.top

C#:   public / protected / private / internal
来源：http://ibq.gogol.net.cn

[G11] getter / setter
来源：http://gex.hfpthk.cn

Py:   @property 与 @x.setter
来源：http://ioi.9152youxi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://thy.hammf.cn

JS:   get name() { return this._name; }
来源：http://iqi.xylfe.cn

TS:   get name(): string { return this._name; }
来源：http://vji.fktsv.cn

Java: public String getName() { return name; }
来源：http://wun.xziqi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lxx.yongpay.top

Ruby: attr_accessor :name
来源：http://vos.wangshuangyany.cn

C#:   public string Name { get; set; }
来源：http://bwv.sxryk.cn

[G12] 对象转字符串
来源：http://wxi.jianghu66.top

Py:   def __str__(self): return self.name
来源：http://fgd.sysykeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qzr.chenjidiqi.icu

JS:   toString() { return this.name; }
来源：http://iey.andypj.xyz

TS:   toString(): string { return this.name; }
来源：http://flf.jinqigufen.top

Java: @Override public String toString() { return name; }
来源：http://hvn.meibo888.top

Go:   func (u User) String() string { return u.Name }
来源：http://uyq.shangyingyoupin.top

Ruby: def to_s; @name; end
来源：http://shp.hcnkem.com

C#:   public override string ToString() => Name;
来源：http://hiw.zycfv.cn

[G13] 判断对象类型
来源：http://kdx.bjfxy.top

Py:   isinstance(u, User)
来源：http://shb.daxiang520.top

PHP:  $u instanceof User
来源：http://iek.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://zjp.xingfuxueyuan.xyz

TS:   u instanceof User
来源：http://lxe.zhiwuduotai.top

Java: u instanceof User
来源：http://shf.52xcode.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ibg.aibaodan.cn

Ruby: u.is_a?(User)
来源：http://dlu.ivvv.top

C#:   u is User
来源：http://lcj.daria6918.cn

[G14] 数据类 / record
来源：http://wpm.fzhhl.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lnm.haohaochexian.top

PHP:  // 用 readonly 属性模拟
来源：http://jmm.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://ibe.bbcook.cn

TS:   type User = { name: string; age: number };
来源：http://fie.gotoacloud.top

Java: record User(String name, int age) {}
来源：http://sch.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://rqr.pycfn.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wud.hysaishi.cn

C#:   record User(string Name, int Age);
来源：http://whc.zhiwuduotai.top

[G15] 枚举
来源：http://tsk.cashguo.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://prf.yj20258888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rgb.meibo888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cat.zhoulong.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hli.yuanzhike.top

Java: enum Color { RED, GREEN }
来源：http://swd.sufxvd.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://did.gzhubu.top

Ruby: Color = %i[red green].freeze
来源：http://apw.yuxming.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wrq.hnxiangtu.top

[G16] 对象转数组 / 字典
来源：http://zgb.hysaishi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bqu.ppjwa.cn

PHP:  get_object_vars($obj);
来源：http://neu.bbcook.cn

JS:   Object.entries(obj)
来源：http://fio.dashuyun.cn

TS:   Object.entries(obj)
来源：http://dzv.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rvf.sweek.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ziu.bbcook.cn

Ruby: obj.instance_variables
来源：http://lwy.gaohongyu789.top

C#:   // 用反射或 System.Text.Json
来源：http://dxk.cucudq.cn

================================================================================
来源：http://ndm.yanxiufei.cn

H. 异常与错误处理
来源：http://xmm.yj20258888.top

================================================================================
来源：http://uxq.tian-w.cn

[H01] try / catch 基础
来源：http://lcu.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yju.aibaodan.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ram.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://orx.ctjpmb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zpc.sweek.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://drr.tian-w.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nky.quarkkingdee.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cet.mhx1999.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jyt.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://uta.yuanzhike.top

Py:   try: f()⏎finally: cleanup()
来源：http://oqg.zhongyouzk.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xur.zhoulong.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://oqv.kuanghao11.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dnc.ppjwa.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hxe.sweek.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kms.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gqr.chenlongwang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://kes.hnqzz.top

[H03] 主动抛出异常
来源：http://kme.tarul.cn

Py:   raise ValueError("错误信息")
来源：http://cxh.wangshuangyany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xst.sweek.top

JS:   throw new Error("错误信息");
来源：http://hzj.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://gkg.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ivh.chenzaomai.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zfg.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nux.epnwcf.com

C#:   throw new ArgumentException("错误信息");
来源：http://byi.yuanzhike.top

[H04] 自定义异常类型
来源：http://eri.zhixingplan.top

Py:   class MyError(Exception): pass
来源：http://zrq.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://agz.daxiang520.top

JS:   class MyError extends Error {}
来源：http://zso.yj202588.top

TS:   class MyError extends Error {}
来源：http://cnn.bjfxy.top

Java: class MyException extends RuntimeException {}
来源：http://ruk.9152youxi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rzx.shuidangran.top

Ruby: class MyError < StandardError; end
来源：http://mzl.cdnleiting.top

C#:   class MyException : Exception {}
来源：http://xwj.nanxinkj.top

[H05] 捕获特定类型
来源：http://fjz.zdqjudy.top

Py:   except ValueError as e:
来源：http://dim.jqgufenzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://thh.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://ckn.sjlbkw.cn

TS:   if (e instanceof TypeError) {}
来源：http://rsy.hywenlv.cn

Java: catch (IOException | SQLException e) {}
来源：http://bzf.yj20258.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lpk.gaohongyu789.top

Ruby: rescue ArgumentError => e
来源：http://bbg.tarul.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xju.gogol.net.cn

[H06] 可选值 / 空值安全访问
来源：http://wyu.xinyue.icu

Py:   value = d.get("k") or default
来源：http://riy.haohaochexian.top

PHP:  $v = $d["k"] ?? null;
来源：http://lhy.tarul.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rgp.xinyue.icu

TS:   obj?.a?.b;  d ?? default
来源：http://thu.cashguo.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uhy.zhijiandao.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mff.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://kha.meibo888.top

C#:   obj?.A?.B ?? default
来源：http://ecs.jianghu66.top

[H07] 断言
来源：http://rqm.vqdsnc.cn

Py:   assert x > 0, "必须为正"
来源：http://iwq.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://pvp.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://fcm.ydjk.org.cn

TS:   console.assert(x > 0);
来源：http://ijs.zhijiandao.cn

Java: assert x > 0 : "必须为正";
来源：http://bfx.zhiwuduotai.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dfq.haohaochexian.top

Ruby: raise "必须为正" unless x > 0
来源：http://jbg.tian-w.cn

C#:   Debug.Assert(x > 0);
来源：http://ipp.hcnkem.com

[H08] 获取错误信息与堆栈
来源：http://edh.tanke756.top

Py:   str(e);  traceback.format_exc()
来源：http://rgy.meibo888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uku.andypj.xyz

JS:   e.message;  e.stack
来源：http://kcl.redwolf501.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lhe.hammf.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gwy.yfazqb.com

Go:   err.Error()
来源：http://otm.kuanghao11.cn

Ruby: e.message;  e.backtrace
来源：http://nri.gotoacloud.top

C#:   e.Message;  e.StackTrace
来源：http://nwb.xuanzx.com

[H09] 带错误码的异常
来源：http://fbr.bjfxy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://omt.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vju.cheryme.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xng.kuanghao11.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lit.gaohongyu789.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ktj.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kwb.jinqigfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://awe.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://uut.nanxuanxn.top

[H10] 资源自动释放
来源：http://loc.sjlbkw.cn


<!-- 参考信息 -->