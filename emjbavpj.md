代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://ucn.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://rdq.yuxming.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uvv.haohaochexian.top

Go:   os.Remove("a.txt")
来源：http://hof.shzxlz.cn

Ruby: File.delete("a.txt")
来源：http://oya.shzxlz.cn

C#:   File.Delete("a.txt");
来源：http://abh.zhongyouzk.top

[F07] 创建目录（含多级）
来源：http://inm.hfpthk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wuo.zdbjq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vkf.uphjek.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ltv.tanke756.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pcu.gogol.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pgs.xuanzx.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hqq.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vkg.dianchejie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://npe.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://xqe.yj20258.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dlc.pengpengdd.cyou

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zae.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://fgt.fengsongda.top

TS:   fs.readdirSync("dir")
来源：http://qco.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bqd.sjlbkw.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://edt.jinyuanbaomall.cn

Ruby: Dir.children("dir")
来源：http://yqo.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://wot.cucudq.cn

[F09] 获取文件大小
来源：http://zrf.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://bjp.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://lfr.yonumen.top

JS:   fs.statSync("a.txt").size
来源：http://cco.snrcjt.cn

TS:   fs.statSync("a.txt").size
来源：http://bwi.vehdjk.com

Java: Files.size(Path.of("a.txt"))
来源：http://gjy.9152youxi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tlw.tarul.cn

Ruby: File.size("a.txt")
来源：http://yvv.vehdjk.com

C#:   new FileInfo("a.txt").Length
来源：http://xqq.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://fvy.xziqi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hbt.zdqjudy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mix.fehbvm.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hvo.hywenlv.cn

TS:   path.extname("a.txt")
来源：http://kyl.snrcjt.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mpu.yuxming.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hkl.hysaishi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ymg.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nsx.smart0.xyz

[F11] 复制与移动文件
来源：http://cfk.guannengcc.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iky.redwolf501.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rwm.52xcode.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gyj.zycfv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rec.daxiang520.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://owe.sxryk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mdx.cucudq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://olc.xingfuxueyuan.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jmv.svipenyu.cn

[F12] CSV 读写
来源：http://xnu.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nam.fengsongda.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yvm.smart0.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jst.iojbl.cn

TS:   // 同上
来源：http://pcx.pycfn.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://whg.xinyue.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lwl.haohaochexian.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jfe.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mdc.tarul.cn

================================================================================
来源：http://ygv.tianlin.xyz

G. 面向对象
来源：http://zor.zdbjq.cn

================================================================================
来源：http://uzv.mhx1999.top

[G01] 定义类
来源：http://uhl.fanxiaobao.xyz

Py:   class User: pass
来源：http://avm.daxiang520.top

PHP:  class User {}
来源：http://ojh.svipenyu.cn

JS:   class User {}
来源：http://fgm.jinghuilouyu.cn

TS:   class User { name: string = ""; }
来源：http://zju.cashguo.top

Java: class User {}
来源：http://mys.tian-w.cn

Go:   type User struct { Name string }
来源：http://bys.meibo888.top

Ruby: class User; end
来源：http://ibe.andypj.xyz

C#:   class User {}
来源：http://avg.zhoulong.xyz

[G02] 构造函数
来源：http://cbg.smart0.xyz

Py:   def __init__(self, name): self.name = name
来源：http://pka.snrcjt.cn

PHP:  public function __construct(public string $name) {}
来源：http://krx.vehdjk.com

JS:   constructor(name) { this.name = name; }
来源：http://dod.quarkkingdee.top

TS:   constructor(public name: string) {}
来源：http://asr.sxryk.cn

Java: User(String name) { this.name = name; }
来源：http://ybb.havefunace.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://enf.daria6918.cn

Ruby: def initialize(name); @name = name; end
来源：http://wmi.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://sae.ybcxt.top

[G03] 实例属性
来源：http://vuf.gogol.net.cn

Py:   self.name = "x"
来源：http://vpk.zdqjudy.top

PHP:  public string $name = "x";
来源：http://pdz.zhijiandao.cn

JS:   this.name = "x";
来源：http://ddd.nanxuanxn.top

TS:   name: string = "x";
来源：http://gfi.andypj.xyz

Java: private String name;
来源：http://zmv.0kj1m.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://npm.ybcxt.top

Ruby: @name = "x"
来源：http://fbs.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://zck.shuidangran.top

[G04] 定义方法
来源：http://ran.guowangkeji.top

Py:   def greet(self): return self.name
来源：http://trf.jqgufenzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pca.hongshengwenyu.top

JS:   greet() { return this.name; }
来源：http://aqc.feifeiyinyue.top

TS:   greet(): string { return this.name; }
来源：http://mgs.guowangkeji.top

Java: String greet() { return name; }
来源：http://oiq.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nur.smart0.xyz

Ruby: def greet; @name; end
来源：http://deo.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://rqi.birdmap.top

[G05] 继承
来源：http://hbe.yonumen.top

Py:   class Admin(User): pass
来源：http://siv.redwolf501.top

PHP:  class Admin extends User {}
来源：http://piw.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://iaj.sysykeji.top

TS:   class Admin extends User {}
来源：http://tek.kuanghao11.cn

Java: class Admin extends User {}
来源：http://fkz.jinghuilouyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://erc.xingfuxueyuan.xyz

Ruby: class Admin < User; end
来源：http://prw.ybcxt.top

C#:   class Admin : User {}
来源：http://weg.xinyue.icu

[G06] 重写方法
来源：http://xto.ctjpmb.com

Py:   def greet(self): return "admin"
来源：http://iqo.hesvh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://may.sufxvd.cn

JS:   greet() { return "admin"; }
来源：http://ceb.zhijiandao.cn

TS:   greet(): string { return "admin"; }
来源：http://cqi.yueranfly.top

Java: @Override String greet() { return "admin"; }
来源：http://btm.zhiwuduotai.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lod.52xcode.cn

Ruby: def greet; "admin"; end
来源：http://cqa.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://auj.shanyushiyangkeji.top

[G07] 调用父类方法
来源：http://tiw.wangshuangyany.cn

Py:   super().greet()
来源：http://hnq.jyoumei.cn

PHP:  parent::greet();
来源：http://fob.cucudq.cn

JS:   super.greet();
来源：http://qmv.ydjk.org.cn

TS:   super.greet();
来源：http://qox.hesvh.cn

Java: super.greet();
来源：http://uyu.316326.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hyz.jianghu66.top

Ruby: super
来源：http://ahc.havefunace.top

C#:   base.Greet();
来源：http://zok.redwolf501.top

[G08] 静态方法与属性
来源：http://oct.ydzc1.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://spx.yonumen.top

PHP:  public static function f() {}
来源：http://afs.yonumen.top

JS:   static f() {}
来源：http://prl.xinyue.icu

TS:   static f(): void {}
来源：http://evm.ehwqpu.com

Java: static void f() {}
来源：http://djo.zhoulong.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://avj.jyoumei.cn

Ruby: def self.f; end
来源：http://czd.yuxming.cn

C#:   public static void F() {}
来源：http://ozh.hcnkem.com

[G09] 接口 / 抽象类
来源：http://xwy.ivvv.top

Py:   from abc import ABC, abstractmethod
来源：http://bqz.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uwx.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://atc.yueranfly.top

TS:   interface Shape { area(): number; }
来源：http://hxr.hnqzz.top

Java: interface Shape { double area(); }
来源：http://jre.yanxiufei.cn

Go:   type Shape interface { Area() float64 }
来源：http://auc.aizwys.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wls.kuanghao11.cn

C#:   interface IShape { double Area(); }
来源：http://lay.wangdashe.top

[G10] 访问控制
来源：http://dxc.zhixingplan.top

Py:   约定 _protected / __private（不强制）
来源：http://rzm.hysaishi.cn

PHP:  public / protected / private
来源：http://xbr.cqqwz.cn

JS:   #private 字段；其余公开
来源：http://ptl.guowangkeji.top

TS:   public / protected / private
来源：http://qcb.yj20258888.top

Java: public / protected / private / 默认包级
来源：http://mcv.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ckk.zhengqikj.top

Ruby: public / protected / private
来源：http://tyy.pycfn.com

C#:   public / protected / private / internal
来源：http://aqo.epnwcf.com

[G11] getter / setter
来源：http://mvw.jinqigufen.top

Py:   @property 与 @x.setter
来源：http://wul.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bug.yj202588.top

JS:   get name() { return this._name; }
来源：http://aug.iojbl.cn

TS:   get name(): string { return this._name; }
来源：http://cfp.tian-w.cn

Java: public String getName() { return name; }
来源：http://lvl.sysykeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cub.zhengqikj.top

Ruby: attr_accessor :name
来源：http://hvu.xziqi.cn

C#:   public string Name { get; set; }
来源：http://vva.yueranfly.top

[G12] 对象转字符串
来源：http://ggr.ydjk.org.cn

Py:   def __str__(self): return self.name
来源：http://vnt.jlsjyb.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tom.sysykeji.top

JS:   toString() { return this.name; }
来源：http://jsu.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://xib.jinyuanbaomall.cn

Java: @Override public String toString() { return name; }
来源：http://fhe.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://urj.tianlin.xyz

Ruby: def to_s; @name; end
来源：http://kvh.aizwys.cn

C#:   public override string ToString() => Name;
来源：http://ohf.hywenlv.cn

[G13] 判断对象类型
来源：http://zge.quarkkingdee.top

Py:   isinstance(u, User)
来源：http://izn.zhixingplan.top

PHP:  $u instanceof User
来源：http://vxv.xylfe.cn

JS:   u instanceof User
来源：http://ask.bjfxy.top

TS:   u instanceof User
来源：http://srg.9152youxi.cn

Java: u instanceof User
来源：http://enm.yueranfly.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pyg.andypj.xyz

Ruby: u.is_a?(User)
来源：http://qqo.jyoumei.cn

C#:   u is User
来源：http://uxf.xuetiantiany.cn

[G14] 数据类 / record
来源：http://aqk.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mrw.tarul.cn

PHP:  // 用 readonly 属性模拟
来源：http://xps.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://egr.fktsv.cn

TS:   type User = { name: string; age: number };
来源：http://imz.yj20258888.top

Java: record User(String name, int age) {}
来源：http://kci.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://gdl.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://thc.zhengqikj.top

C#:   record User(string Name, int Age);
来源：http://lbd.shanyushiyangkeji.top

[G15] 枚举
来源：http://bqx.yongpay.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rxu.gaohongyu789.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ufk.shuidangran.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eav.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fqn.yueranfly.top

Java: enum Color { RED, GREEN }
来源：http://kbc.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wvb.yanxiufei.cn

Ruby: Color = %i[red green].freeze
来源：http://yxt.gzhubu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bda.zhaomingkeji.xyz

[G16] 对象转数组 / 字典
来源：http://tub.dashuyun.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vxa.ydzc1.top

PHP:  get_object_vars($obj);
来源：http://myj.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://hqb.gogol.net.cn

TS:   Object.entries(obj)
来源：http://zcf.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uvm.jinyuanbaomall.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://beg.yuxming.cn

Ruby: obj.instance_variables
来源：http://dtf.yfazqb.com

C#:   // 用反射或 System.Text.Json
来源：http://vju.fehbvm.com

================================================================================
来源：http://rnp.jinyuanbaomall.cn

H. 异常与错误处理
来源：http://zzo.hnxiangtu.top

================================================================================
来源：http://leg.dianchejie.cn

[H01] try / catch 基础
来源：http://fly.ppjwa.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fkc.smart0.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qqe.birdmap.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jan.tian-w.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lfw.fengsongda.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vnl.chenzaomai.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eyk.cucudq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dvs.hongshengwenyu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://osk.xinyue.icu

[H02] finally / ensure 收尾
来源：http://rlg.vehdjk.com

Py:   try: f()⏎finally: cleanup()
来源：http://hip.mhx1999.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ppc.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cot.aibaodan.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qrj.ydjk.org.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bds.fktsv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xrt.xingfuxueyuan.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://fld.zhixingplan.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wuz.fzhhl.top

[H03] 主动抛出异常
来源：http://nyw.svipenyu.cn

Py:   raise ValueError("错误信息")
来源：http://lpq.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nmn.hnqzz.top

JS:   throw new Error("错误信息");
来源：http://bxa.bbcook.cn

TS:   throw new Error("错误信息");
来源：http://fyc.jqgufenzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://frc.vehdjk.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vqe.ydzc1.top

Ruby: raise ArgumentError, "错误信息"
来源：http://egg.52xcode.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rks.0kj1m.cn

[H04] 自定义异常类型
来源：http://rks.jinyuanbaomall.cn

Py:   class MyError(Exception): pass
来源：http://xyw.zycfv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qvd.ctjpmb.com

JS:   class MyError extends Error {}
来源：http://dxx.zhongyouzk.top

TS:   class MyError extends Error {}
来源：http://aql.epnwcf.com

Java: class MyException extends RuntimeException {}
来源：http://sue.birdmap.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rda.c1oappe.top

Ruby: class MyError < StandardError; end
来源：http://hnn.aizwys.cn

C#:   class MyException : Exception {}
来源：http://peg.sweek.top

[H05] 捕获特定类型
来源：http://rot.guowangkeji.top

Py:   except ValueError as e:
来源：http://ykd.shanyushiyangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ehy.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://nzt.sjlbkw.cn

TS:   if (e instanceof TypeError) {}
来源：http://etx.52xcode.cn

Java: catch (IOException | SQLException e) {}
来源：http://kcn.yj202588.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qiw.0kj1m.cn

Ruby: rescue ArgumentError => e
来源：http://gel.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qrw.feifeiyinyue.top

[H06] 可选值 / 空值安全访问
来源：http://trh.nanxuanxn.top

Py:   value = d.get("k") or default
来源：http://rvr.xylfe.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bup.jqgfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://xor.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://ebr.gaohongyu789.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tvc.wangdashe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xtd.cheryme.top

Ruby: d&.dig(:a, :b)
来源：http://dnl.cashguo.top

C#:   obj?.A?.B ?? default
来源：http://icd.316326.xyz

[H07] 断言
来源：http://rhp.mhx1999.top

Py:   assert x > 0, "必须为正"
来源：http://lmy.gaohongyu789.top

PHP:  assert($x > 0);
来源：http://xiz.ppjwa.cn

JS:   console.assert(x > 0);
来源：http://odc.nanxinkj.top

TS:   console.assert(x > 0);
来源：http://lnc.fzhhl.top

Java: assert x > 0 : "必须为正";
来源：http://zgn.316326.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fst.jinyuanbaomall.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bwd.andypj.xyz

C#:   Debug.Assert(x > 0);
来源：http://wym.xinyue.icu

[H08] 获取错误信息与堆栈
来源：http://auy.yj202588.top

Py:   str(e);  traceback.format_exc()
来源：http://qay.sufxvd.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ull.wangdashe.top

JS:   e.message;  e.stack
来源：http://vdx.chenzaomai.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://cxs.ywan-chungtsiang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xem.gzhubu.top

Go:   err.Error()
来源：http://qbz.feifeiyinyue.top

Ruby: e.message;  e.backtrace
来源：http://njs.gzhubu.top

C#:   e.Message;  e.StackTrace
来源：http://hgp.redwolf501.top

[H09] 带错误码的异常
来源：http://aku.sjlbkw.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jrc.hnxiangtu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tbc.daria6918.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ljs.hysaishi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nfc.jiagoushi.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wtx.jinyuanbaomall.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ege.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://eht.fanxiaobao.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://rnp.9152youxi.cn

[H10] 资源自动释放
来源：http://hlc.shangyingyoupin.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lrs.mhx1999.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mcw.zhaomingkeji.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://joy.hcnkem.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ihb.0kj1m.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jkb.cdnleiting.top

Go:   defer f.Close()
来源：http://vrv.xziqi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kfi.haohaochexian.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bni.hywenlv.cn


<!-- 参考信息 -->