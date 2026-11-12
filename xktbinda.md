代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://oex.yongpay.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vxl.ppjwa.cn

PHP:  file_exists("a.txt");
来源：http://oik.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://evs.redwolf501.top

TS:   fs.existsSync("a.txt")
来源：http://vvs.jinqigufen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://eac.shangyingyoupin.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bqa.jqgufenzy.top

Ruby: File.exist?("a.txt")
来源：http://gga.0kj1m.cn

C#:   File.Exists("a.txt")
来源：http://mzd.52xcode.cn

[F06] 删除文件
来源：http://guo.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://rij.feifeiyinyue.top

PHP:  unlink("a.txt");
来源：http://qkx.fzhhl.top

JS:   fs.unlinkSync("a.txt")
来源：http://sit.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://psl.jinghuilouyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://seu.chenzaomai.com

Go:   os.Remove("a.txt")
来源：http://dfz.quarkkingdee.top

Ruby: File.delete("a.txt")
来源：http://ksw.hnxiangtu.top

C#:   File.Delete("a.txt");
来源：http://ivh.sysykeji.top

[F07] 创建目录（含多级）
来源：http://sjz.tian-w.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://buk.shanyushiyangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mgm.quarkkingdee.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zdx.birdmap.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lxd.hywenlv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uka.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ydh.andypj.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bvm.nanxinkj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ilv.yueranfly.top

[F08] 遍历目录
来源：http://tfk.jyoumei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cvo.zhongyouzk.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pmc.haohaochexian.top

JS:   fs.readdirSync("dir")
来源：http://umq.xylfe.cn

TS:   fs.readdirSync("dir")
来源：http://ums.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sns.hesvh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nzt.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://ozn.birdmap.top

C#:   Directory.GetFiles("dir")
来源：http://pxo.gaohongyu789.top

[F09] 获取文件大小
来源：http://uxn.yvedp.cn

Py:   os.path.getsize("a.txt")
来源：http://fyl.zhijiandao.cn

PHP:  filesize("a.txt");
来源：http://bbk.dashuyun.cn

JS:   fs.statSync("a.txt").size
来源：http://obc.pycfn.com

TS:   fs.statSync("a.txt").size
来源：http://pxj.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://krp.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vur.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://hnc.yuxming.cn

C#:   new FileInfo("a.txt").Length
来源：http://iqv.jqgufenzy.top

[F10] 取文件扩展名 / 文件名
来源：http://yij.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fbl.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://llo.cheryme.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pok.tanke756.top

TS:   path.extname("a.txt")
来源：http://rxx.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://afn.uphjek.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vio.zhiwuduotai.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xnh.yonumen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vjp.snrcjt.cn

[F11] 复制与移动文件
来源：http://gwa.fzhhl.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rai.yanxiufei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bza.xingfuxueyuan.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xuw.kuanghao11.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rov.ivvv.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xqd.yfazqb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gut.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ocw.aibaodan.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qei.hammf.cn

[F12] CSV 读写
来源：http://njk.jinqigfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yqj.jiagoushi.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rzi.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iqa.nwbrower.top

TS:   // 同上
来源：http://etq.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mdi.nanxinkj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vgc.0kj1m.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nqc.yongpay.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vvu.jianghu66.top

================================================================================
来源：http://qoj.yfazqb.com

G. 面向对象
来源：http://xzh.tarul.cn

================================================================================
来源：http://dtj.hesvh.cn

[G01] 定义类
来源：http://uih.ybcxt.top

Py:   class User: pass
来源：http://yiq.52xcode.cn

PHP:  class User {}
来源：http://eav.zhijiandao.cn

JS:   class User {}
来源：http://kvl.dianchejie.cn

TS:   class User { name: string = ""; }
来源：http://adi.yuanzhike.top

Java: class User {}
来源：http://fmi.cheryme.top

Go:   type User struct { Name string }
来源：http://yyu.hammf.cn

Ruby: class User; end
来源：http://fnd.guannengcc.top

C#:   class User {}
来源：http://pau.dianchejie.cn

[G02] 构造函数
来源：http://yml.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://xdu.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://tve.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://hjm.fzhhl.top

TS:   constructor(public name: string) {}
来源：http://yda.shanyushiyangtech.top

Java: User(String name) { this.name = name; }
来源：http://izy.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mij.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://yua.zhiwuduotai.top

C#:   public User(string name) { Name = name; }
来源：http://nrx.gotoacloud.top

[G03] 实例属性
来源：http://gnw.ppjwa.cn

Py:   self.name = "x"
来源：http://ghf.chenlongwang.top

PHP:  public string $name = "x";
来源：http://sqi.ehwqpu.com

JS:   this.name = "x";
来源：http://xsz.zdqjudy.top

TS:   name: string = "x";
来源：http://mlo.shzxlz.cn

Java: private String name;
来源：http://fob.chenjidiqi.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dth.yfazqb.com

Ruby: @name = "x"
来源：http://cut.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://tqu.c1oappe.top

[G04] 定义方法
来源：http://tuv.xinyue.icu

Py:   def greet(self): return self.name
来源：http://mdk.dianchejie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yzs.fanxiaobao.xyz

JS:   greet() { return this.name; }
来源：http://vib.zycfv.cn

TS:   greet(): string { return this.name; }
来源：http://sxp.feifeiyinyue.top

Java: String greet() { return name; }
来源：http://oag.jinqigfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pfe.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://ovl.feifeiyinyue.top

C#:   public string Greet() => Name;
来源：http://aha.yfazqb.com

[G05] 继承
来源：http://ufq.nwbrower.top

Py:   class Admin(User): pass
来源：http://kiz.ydjk.org.cn

PHP:  class Admin extends User {}
来源：http://upy.yfazqb.com

JS:   class Admin extends User {}
来源：http://jfe.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://rov.guowangkeji.top

Java: class Admin extends User {}
来源：http://ifz.cdnleiting.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kwx.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://xge.meibo888.top

C#:   class Admin : User {}
来源：http://ofk.birdmap.top

[G06] 重写方法
来源：http://gun.hysaishi.cn

Py:   def greet(self): return "admin"
来源：http://lgc.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vki.pycfn.com

JS:   greet() { return "admin"; }
来源：http://loc.gogol.net.cn

TS:   greet(): string { return "admin"; }
来源：http://oqv.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://uhx.jianghu66.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ogg.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://fys.yj20258.top

C#:   public override string Greet() => "admin";
来源：http://xpz.hnxiangtu.top

[G07] 调用父类方法
来源：http://ovt.hnxiangtu.top

Py:   super().greet()
来源：http://xrc.shuidangran.top

PHP:  parent::greet();
来源：http://xty.aizwys.cn

JS:   super.greet();
来源：http://mat.tarul.cn

TS:   super.greet();
来源：http://atf.sxryk.cn

Java: super.greet();
来源：http://yez.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://alz.fktsv.cn

Ruby: super
来源：http://ges.fanxiaobao.xyz

C#:   base.Greet();
来源：http://sfc.ydjk.org.cn

[G08] 静态方法与属性
来源：http://wll.yfazqb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bqc.9152youxi.cn

PHP:  public static function f() {}
来源：http://tdc.tianlin.xyz

JS:   static f() {}
来源：http://pbw.pengpengdd.cyou

TS:   static f(): void {}
来源：http://wkn.shuidangran.top

Java: static void f() {}
来源：http://tco.yongpay.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://akl.zhengqikj.top

Ruby: def self.f; end
来源：http://mcd.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://ssv.sxryk.cn

[G09] 接口 / 抽象类
来源：http://vav.jqgufenzy.top

Py:   from abc import ABC, abstractmethod
来源：http://beq.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://efp.zhaomingkeji.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://jgb.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://nob.dianchejie.cn

Java: interface Shape { double area(); }
来源：http://fie.cqqwz.cn

Go:   type Shape interface { Area() float64 }
来源：http://eum.bjfxy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://drg.hnqzz.top

C#:   interface IShape { double Area(); }
来源：http://mzn.jinqigfzy.top

[G10] 访问控制
来源：http://rvk.yj202588.top

Py:   约定 _protected / __private（不强制）
来源：http://tlm.svipenyu.cn

PHP:  public / protected / private
来源：http://ghk.xinyue.icu

JS:   #private 字段；其余公开
来源：http://jhy.zdbjq.cn

TS:   public / protected / private
来源：http://ntg.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://lce.xziqi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jdt.feifeiyinyue.top

Ruby: public / protected / private
来源：http://qqe.jiagoushi.top

C#:   public / protected / private / internal
来源：http://ivu.andypj.xyz

[G11] getter / setter
来源：http://zyb.cucudq.cn

Py:   @property 与 @x.setter
来源：http://yxs.zhoulong.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://xaj.xylfe.cn

JS:   get name() { return this._name; }
来源：http://pex.ehwqpu.com

TS:   get name(): string { return this._name; }
来源：http://hdl.ivvv.top

Java: public String getName() { return name; }
来源：http://bif.jinqigfzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nqc.vehdjk.com

Ruby: attr_accessor :name
来源：http://jyx.jqgufenzy.top

C#:   public string Name { get; set; }
来源：http://mzx.hnxiangtu.top

[G12] 对象转字符串
来源：http://zzv.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://ykl.hysaishi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hlp.jqgufenzy.top

JS:   toString() { return this.name; }
来源：http://jic.yvedp.cn

TS:   toString(): string { return this.name; }
来源：http://tta.jqgufenzy.top

Java: @Override public String toString() { return name; }
来源：http://msu.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dou.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://sxo.shangyingyoupin.top

C#:   public override string ToString() => Name;
来源：http://zdg.havefunace.top

[G13] 判断对象类型
来源：http://tuk.sufxvd.cn

Py:   isinstance(u, User)
来源：http://doe.xylfe.cn

PHP:  $u instanceof User
来源：http://ame.yfazqb.com

JS:   u instanceof User
来源：http://llz.yuanzhike.top

TS:   u instanceof User
来源：http://twf.nanxuanxn.top

Java: u instanceof User
来源：http://akm.yfazqb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://peg.yvedp.cn

Ruby: u.is_a?(User)
来源：http://vqu.hammf.cn

C#:   u is User
来源：http://iun.cdnleiting.top

[G14] 数据类 / record
来源：http://nsb.wangshuangyany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xvj.snrcjt.cn

PHP:  // 用 readonly 属性模拟
来源：http://wgu.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://ift.hcnkem.com

TS:   type User = { name: string; age: number };
来源：http://rqw.jlsjyb.cn

Java: record User(String name, int age) {}
来源：http://lwq.ctjpmb.com

Go:   type User struct { Name string; Age int }
来源：http://gks.vqdsnc.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qpo.yj20258888.top

C#:   record User(string Name, int Age);
来源：http://oko.0kj1m.cn

[G15] 枚举
来源：http://piq.tianlin.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qjn.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zpg.yj20258888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cai.shanyushiyangtech.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oms.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://wtb.hywenlv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wyn.shzxlz.cn

Ruby: Color = %i[red green].freeze
来源：http://wdq.hcnkem.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wsf.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://mdn.cdnleiting.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cnl.shuidangran.top

PHP:  get_object_vars($obj);
来源：http://ajx.svipenyu.cn

JS:   Object.entries(obj)
来源：http://qoi.ivvv.top

TS:   Object.entries(obj)
来源：http://rxs.cashguo.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xqx.hywenlv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://aee.hywenlv.cn

Ruby: obj.instance_variables
来源：http://eiz.zhiwuduotai.top

C#:   // 用反射或 System.Text.Json
来源：http://rkj.meibo888.top

================================================================================
来源：http://idf.yongpay.top

H. 异常与错误处理
来源：http://mrl.bjfxy.top

================================================================================
来源：http://qfb.yanxiufei.cn

[H01] try / catch 基础
来源：http://nrp.svipenyu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cdp.hongshengwenyu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qnq.gotoacloud.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://akk.iojbl.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ycg.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uab.yvedp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jwc.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wyl.fzhhl.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://orp.sweek.top

[H02] finally / ensure 收尾
来源：http://bvj.gaohongyu789.top

Py:   try: f()⏎finally: cleanup()
来源：http://zax.tarul.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mmm.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ewt.ehwqpu.com

TS:   try { f(); } finally { cleanup(); }
来源：http://prh.zdqjudy.top

Java: try { f(); } finally { cleanup(); }
来源：http://jbo.chenlongwang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gsu.sweek.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vit.jiagoushi.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://aee.svipenyu.cn

[H03] 主动抛出异常
来源：http://vsd.xinyue.icu

Py:   raise ValueError("错误信息")
来源：http://wsd.yfazqb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ljo.zhijiandao.cn

JS:   throw new Error("错误信息");
来源：http://cpr.316326.xyz

TS:   throw new Error("错误信息");
来源：http://ghf.havefunace.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gzl.daxiang520.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mdn.xuanzx.com

Ruby: raise ArgumentError, "错误信息"
来源：http://fie.pycfn.com

C#:   throw new ArgumentException("错误信息");
来源：http://qbk.cdnleiting.top

[H04] 自定义异常类型
来源：http://jyx.xylfe.cn

Py:   class MyError(Exception): pass
来源：http://tht.c1oappe.top

PHP:  class MyError extends RuntimeException {}
来源：http://fxb.yvedp.cn

JS:   class MyError extends Error {}
来源：http://vzf.tanke756.top

TS:   class MyError extends Error {}
来源：http://qaq.sjlbkw.cn

Java: class MyException extends RuntimeException {}
来源：http://akv.hesvh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lzh.nanxinkj.top

Ruby: class MyError < StandardError; end
来源：http://qso.ybcxt.top

C#:   class MyException : Exception {}
来源：http://nff.tarul.cn

[H05] 捕获特定类型
来源：http://srn.xinyue.icu

Py:   except ValueError as e:
来源：http://gxq.hongshengwenyu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fci.zhongyouzk.top

JS:   if (e instanceof TypeError) {}
来源：http://liy.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://zyn.zhoulong.xyz

Java: catch (IOException | SQLException e) {}
来源：http://xeo.aibaodan.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kqm.iojbl.cn

Ruby: rescue ArgumentError => e
来源：http://twl.yueranfly.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ovd.jqgufenzy.top

[H06] 可选值 / 空值安全访问
来源：http://evq.sufxvd.cn

Py:   value = d.get("k") or default
来源：http://mnm.0kj1m.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kxk.fktsv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iwk.havefunace.top

TS:   obj?.a?.b;  d ?? default
来源：http://uzg.chenzaomai.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ysm.zdbjq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hxv.xinyue.icu

Ruby: d&.dig(:a, :b)
来源：http://npm.fzhhl.top

C#:   obj?.A?.B ?? default
来源：http://xae.cqqwz.cn

[H07] 断言
来源：http://iak.nanxinkj.top

Py:   assert x > 0, "必须为正"
来源：http://oix.52xcode.cn

PHP:  assert($x > 0);
来源：http://ghi.fzhhl.top

JS:   console.assert(x > 0);
来源：http://yrc.shangyingyoupin.top

TS:   console.assert(x > 0);
来源：http://spw.52xcode.cn

Java: assert x > 0 : "必须为正";
来源：http://eij.meibo888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pjh.kuanghao11.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jel.ctjpmb.com

C#:   Debug.Assert(x > 0);
来源：http://fim.wangshuangyany.cn

[H08] 获取错误信息与堆栈
来源：http://bff.quarkkingdee.top

Py:   str(e);  traceback.format_exc()
来源：http://rkb.cdnleiting.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zgi.chenzaomai.com

JS:   e.message;  e.stack
来源：http://owl.zycfv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zok.316326.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://jfk.jiagoushi.top

Go:   err.Error()
来源：http://mxw.nanxuanxn.top

Ruby: e.message;  e.backtrace
来源：http://pnl.gaohongyu789.top

C#:   e.Message;  e.StackTrace
来源：http://ahv.hcnkem.com

[H09] 带错误码的异常
来源：http://qvg.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ods.jqgfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://epk.hammf.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jlp.cashguo.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kgc.zhengqikj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hjq.sweek.top


<!-- 参考信息 -->