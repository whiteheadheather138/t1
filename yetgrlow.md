代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://rgz.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gjb.jqgufenzy.top

PHP:  file_exists("a.txt");
来源：http://aft.daxiang520.top

JS:   fs.existsSync("a.txt")
来源：http://pcb.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://pzt.aizwys.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://szw.gaohongyu789.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oto.smart0.xyz

Ruby: File.exist?("a.txt")
来源：http://nip.jinqigfzy.top

C#:   File.Exists("a.txt")
来源：http://ayd.guannengcc.top

[F06] 删除文件
来源：http://mxv.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://jek.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://htn.uphjek.com

JS:   fs.unlinkSync("a.txt")
来源：http://mqf.tarul.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ihe.sjlbkw.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://edh.nwbrower.top

Go:   os.Remove("a.txt")
来源：http://sxj.yuanzhike.top

Ruby: File.delete("a.txt")
来源：http://ehi.yj202588.top

C#:   File.Delete("a.txt");
来源：http://gne.iojbl.cn

[F07] 创建目录（含多级）
来源：http://pbd.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://elx.zdqjudy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://duk.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jjw.chenjidiqi.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://whd.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ako.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xbv.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dwo.tian-w.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bwe.jyoumei.cn

[F08] 遍历目录
来源：http://xtq.nanxinkj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gij.feifeiyinyue.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mdc.shangyingyoupin.top

JS:   fs.readdirSync("dir")
来源：http://emt.ydzc1.top

TS:   fs.readdirSync("dir")
来源：http://ntl.zycfv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zpb.sweek.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fsx.hesvh.cn

Ruby: Dir.children("dir")
来源：http://qxm.hfpthk.cn

C#:   Directory.GetFiles("dir")
来源：http://iwf.svipenyu.cn

[F09] 获取文件大小
来源：http://wix.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://lns.gogol.net.cn

PHP:  filesize("a.txt");
来源：http://kpx.hongshengwenyu.top

JS:   fs.statSync("a.txt").size
来源：http://jkx.jinghuilouyu.cn

TS:   fs.statSync("a.txt").size
来源：http://kiw.xylfe.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bit.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jks.zdbjq.cn

Ruby: File.size("a.txt")
来源：http://fxv.dashuyun.cn

C#:   new FileInfo("a.txt").Length
来源：http://bsk.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://khl.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://itp.daria6918.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cao.jinyuanbaomall.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dbm.zdbjq.cn

TS:   path.extname("a.txt")
来源：http://uaf.hnxiangtu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fvq.zhiwuduotai.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qcq.sjlbkw.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mbm.dashuyun.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dxd.fktsv.cn

[F11] 复制与移动文件
来源：http://qop.yonumen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pro.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://atc.jqgufenzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mfp.mhx1999.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://alq.yj20258.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tjn.fehbvm.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bql.birdmap.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lpr.yonumen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tfn.sxryk.cn

[F12] CSV 读写
来源：http://zzc.hesvh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hsv.daxiang520.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zvn.dashuyun.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sgp.zhixingplan.top

TS:   // 同上
来源：http://xns.yongpay.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xeh.zycfv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bor.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pnx.nwbrower.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qji.iojbl.cn

================================================================================
来源：http://lae.redwolf501.top

G. 面向对象
来源：http://sny.snrcjt.cn

================================================================================
来源：http://wee.hfpthk.cn

[G01] 定义类
来源：http://dgy.hywenlv.cn

Py:   class User: pass
来源：http://mph.sxryk.cn

PHP:  class User {}
来源：http://ywk.nanxuanxn.top

JS:   class User {}
来源：http://nqd.jinghuilouyu.cn

TS:   class User { name: string = ""; }
来源：http://aid.gogol.net.cn

Java: class User {}
来源：http://dlu.yongpay.top

Go:   type User struct { Name string }
来源：http://ahj.zhaomingkeji.xyz

Ruby: class User; end
来源：http://los.daria6918.cn

C#:   class User {}
来源：http://kqf.zdqjudy.top

[G02] 构造函数
来源：http://uqx.yuxming.cn

Py:   def __init__(self, name): self.name = name
来源：http://auf.yfazqb.com

PHP:  public function __construct(public string $name) {}
来源：http://yah.gaohongyu789.top

JS:   constructor(name) { this.name = name; }
来源：http://vbt.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://ixo.nwbrower.top

Java: User(String name) { this.name = name; }
来源：http://xxo.jinghuilouyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tnl.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://pka.gaohongyu789.top

C#:   public User(string name) { Name = name; }
来源：http://tzr.sweek.top

[G03] 实例属性
来源：http://yey.jiagoushi.top

Py:   self.name = "x"
来源：http://xlm.andypj.xyz

PHP:  public string $name = "x";
来源：http://str.shuidangran.top

JS:   this.name = "x";
来源：http://lif.havefunace.top

TS:   name: string = "x";
来源：http://qxv.ivvv.top

Java: private String name;
来源：http://dlq.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://axt.zhengqikj.top

Ruby: @name = "x"
来源：http://xus.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://kxs.zhongyouzk.top

[G04] 定义方法
来源：http://uuy.fengsongda.top

Py:   def greet(self): return self.name
来源：http://vjz.daxiang520.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fwi.chenzaomai.com

JS:   greet() { return this.name; }
来源：http://wkn.nanxuanxn.top

TS:   greet(): string { return this.name; }
来源：http://dgo.shanyushiyangtech.top

Java: String greet() { return name; }
来源：http://rkl.hfpthk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://osx.quarkkingdee.top

Ruby: def greet; @name; end
来源：http://mpk.cdnleiting.top

C#:   public string Greet() => Name;
来源：http://ijo.guannengcc.top

[G05] 继承
来源：http://nhe.xuetiantiany.cn

Py:   class Admin(User): pass
来源：http://zhf.jqgufenzy.top

PHP:  class Admin extends User {}
来源：http://gvj.ybcxt.top

JS:   class Admin extends User {}
来源：http://afn.zhoulong.xyz

TS:   class Admin extends User {}
来源：http://prj.0kj1m.cn

Java: class Admin extends User {}
来源：http://nrz.yuanzhike.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gti.yongpay.top

Ruby: class Admin < User; end
来源：http://zch.svipenyu.cn

C#:   class Admin : User {}
来源：http://mmj.ehwqpu.com

[G06] 重写方法
来源：http://rze.sweek.top

Py:   def greet(self): return "admin"
来源：http://cot.meibo888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rln.316326.xyz

JS:   greet() { return "admin"; }
来源：http://zin.yfazqb.com

TS:   greet(): string { return "admin"; }
来源：http://ree.cqqwz.cn

Java: @Override String greet() { return "admin"; }
来源：http://spx.jinghuilouyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bba.daria6918.cn

Ruby: def greet; "admin"; end
来源：http://xoc.shangyingyoupin.top

C#:   public override string Greet() => "admin";
来源：http://gbq.fengsongda.top

[G07] 调用父类方法
来源：http://adq.yfazqb.com

Py:   super().greet()
来源：http://iip.svipenyu.cn

PHP:  parent::greet();
来源：http://xig.tian-w.cn

JS:   super.greet();
来源：http://eaz.sufxvd.cn

TS:   super.greet();
来源：http://rze.redwolf501.top

Java: super.greet();
来源：http://kia.feifeiyinyue.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xjx.zdbjq.cn

Ruby: super
来源：http://efh.pycfn.com

C#:   base.Greet();
来源：http://cxh.hongshengwenyu.top

[G08] 静态方法与属性
来源：http://pio.daria6918.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kxb.xuetiantiany.cn

PHP:  public static function f() {}
来源：http://uoi.sweek.top

JS:   static f() {}
来源：http://mqg.gaohongyu789.top

TS:   static f(): void {}
来源：http://tuo.andypj.xyz

Java: static void f() {}
来源：http://kxm.sjlbkw.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://txz.pengpengdd.cyou

Ruby: def self.f; end
来源：http://iju.ivvv.top

C#:   public static void F() {}
来源：http://xwl.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://wwb.shuidangran.top

Py:   from abc import ABC, abstractmethod
来源：http://zyg.hongshengwenyu.top

PHP:  interface Shape { public function area(): float; }
来源：http://thj.jyoumei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wwx.hywenlv.cn

TS:   interface Shape { area(): number; }
来源：http://cjc.redwolf501.top

Java: interface Shape { double area(); }
来源：http://fvy.pycfn.com

Go:   type Shape interface { Area() float64 }
来源：http://mvu.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ooh.sjlbkw.cn

C#:   interface IShape { double Area(); }
来源：http://acg.ehwqpu.com

[G10] 访问控制
来源：http://zyc.epnwcf.com

Py:   约定 _protected / __private（不强制）
来源：http://yna.iojbl.cn

PHP:  public / protected / private
来源：http://ucl.0kj1m.cn

JS:   #private 字段；其余公开
来源：http://abn.xylfe.cn

TS:   public / protected / private
来源：http://uzc.yj20258888.top

Java: public / protected / private / 默认包级
来源：http://uiz.fanxiaobao.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://mmc.daria6918.cn

Ruby: public / protected / private
来源：http://jyq.jqgfzy.top

C#:   public / protected / private / internal
来源：http://udg.andypj.xyz

[G11] getter / setter
来源：http://yiy.cashguo.top

Py:   @property 与 @x.setter
来源：http://vbd.epnwcf.com

PHP:  public function getName(): string { return $this->name; }
来源：http://lnp.birdmap.top

JS:   get name() { return this._name; }
来源：http://zmp.wangdashe.top

TS:   get name(): string { return this._name; }
来源：http://grm.hcnkem.com

Java: public String getName() { return name; }
来源：http://pfd.0kj1m.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vah.uphjek.com

Ruby: attr_accessor :name
来源：http://quj.gaohongyu789.top

C#:   public string Name { get; set; }
来源：http://rml.hysaishi.cn

[G12] 对象转字符串
来源：http://mxp.jinqigfzy.top

Py:   def __str__(self): return self.name
来源：http://rcb.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://frh.shangyingyoupin.top

JS:   toString() { return this.name; }
来源：http://czb.zhengqikj.top

TS:   toString(): string { return this.name; }
来源：http://asd.svipenyu.cn

Java: @Override public String toString() { return name; }
来源：http://vjm.haohaochexian.top

Go:   func (u User) String() string { return u.Name }
来源：http://kye.zdqjudy.top

Ruby: def to_s; @name; end
来源：http://kci.jqgufenzy.top

C#:   public override string ToString() => Name;
来源：http://kca.yueranfly.top

[G13] 判断对象类型
来源：http://amf.zhijiandao.cn

Py:   isinstance(u, User)
来源：http://mcb.fktsv.cn

PHP:  $u instanceof User
来源：http://roi.chenlongwang.top

JS:   u instanceof User
来源：http://mqc.fanxiaobao.xyz

TS:   u instanceof User
来源：http://tjp.shuidangran.top

Java: u instanceof User
来源：http://wnq.ywan-chungtsiang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vnu.hesvh.cn

Ruby: u.is_a?(User)
来源：http://aeb.cheryme.top

C#:   u is User
来源：http://lmm.hywenlv.cn

[G14] 数据类 / record
来源：http://qzm.chenjidiqi.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aqt.pycfn.com

PHP:  // 用 readonly 属性模拟
来源：http://ixr.dianchejie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yvj.havefunace.top

TS:   type User = { name: string; age: number };
来源：http://cbn.cdnleiting.top

Java: record User(String name, int age) {}
来源：http://tfh.ybcxt.top

Go:   type User struct { Name string; Age int }
来源：http://yxc.bjfxy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wwv.zhiwuduotai.top

C#:   record User(string Name, int Age);
来源：http://nhr.zdbjq.cn

[G15] 枚举
来源：http://wjb.zhoulong.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qja.vqdsnc.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zrr.zhengqikj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wsg.ybcxt.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rxm.xinyue.icu

Java: enum Color { RED, GREEN }
来源：http://twn.fzhhl.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cfh.zhijiandao.cn

Ruby: Color = %i[red green].freeze
来源：http://olh.chenzaomai.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gdy.ydzc1.top

[G16] 对象转数组 / 字典
来源：http://vsj.nanxuanxn.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qiz.fanxiaobao.xyz

PHP:  get_object_vars($obj);
来源：http://ejc.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://unt.yongpay.top

TS:   Object.entries(obj)
来源：http://slx.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jav.jqgufenzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ybv.aizwys.cn

Ruby: obj.instance_variables
来源：http://hri.xuetiantiany.cn

C#:   // 用反射或 System.Text.Json
来源：http://krl.yueranfly.top

================================================================================
来源：http://wla.sysykeji.top

H. 异常与错误处理
来源：http://uqx.zhixingplan.top

================================================================================
来源：http://nhd.yj202588.top

[H01] try / catch 基础
来源：http://ctq.meibo888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://egv.52xcode.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fht.ehwqpu.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iji.yuxming.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tbo.nwbrower.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://myb.hywenlv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gkd.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://npv.birdmap.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qsy.hnxiangtu.top

[H02] finally / ensure 收尾
来源：http://scl.jlsjyb.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yga.pycfn.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://pez.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dnl.hammf.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://osx.daria6918.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vaf.cdnleiting.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hbl.shanyushiyangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://auu.uphjek.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://bio.jiagoushi.top

[H03] 主动抛出异常
来源：http://wqe.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://xvq.ivvv.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sbr.gaohongyu789.top

JS:   throw new Error("错误信息");
来源：http://dox.nanxinkj.top

TS:   throw new Error("错误信息");
来源：http://qsz.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://eiw.shanyushiyangtech.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fqm.shanyushiyangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qai.mhx1999.top

C#:   throw new ArgumentException("错误信息");
来源：http://kya.vehdjk.com

[H04] 自定义异常类型
来源：http://yin.gzhubu.top

Py:   class MyError(Exception): pass
来源：http://slk.bjfxy.top

PHP:  class MyError extends RuntimeException {}
来源：http://drb.meibo888.top

JS:   class MyError extends Error {}
来源：http://gkp.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://pkt.ydzc1.top

Java: class MyException extends RuntimeException {}
来源：http://ktc.haohaochexian.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xgl.tanke756.top

Ruby: class MyError < StandardError; end
来源：http://xaj.shanyushiyangkeji.top

C#:   class MyException : Exception {}
来源：http://ynx.gaohongyu789.top

[H05] 捕获特定类型
来源：http://svp.yuanzhike.top

Py:   except ValueError as e:
来源：http://txe.smart0.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lzt.hongshengwenyu.top

JS:   if (e instanceof TypeError) {}
来源：http://qfj.yuxming.cn

TS:   if (e instanceof TypeError) {}
来源：http://kpx.pycfn.com

Java: catch (IOException | SQLException e) {}
来源：http://qon.52xcode.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://miu.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://hmp.chenjidiqi.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mgr.zhengqikj.top

[H06] 可选值 / 空值安全访问
来源：http://lfe.zhiwuduotai.top

Py:   value = d.get("k") or default
来源：http://sai.sysykeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://xfz.zhijiandao.cn

JS:   obj?.a?.b;  d ?? default
来源：http://row.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kug.shanyushiyangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zbu.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zll.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://osc.hongshengwenyu.top

C#:   obj?.A?.B ?? default
来源：http://qju.bjfxy.top

[H07] 断言
来源：http://atv.quarkkingdee.top

Py:   assert x > 0, "必须为正"
来源：http://ovm.shzxlz.cn

PHP:  assert($x > 0);
来源：http://wha.xinyue.icu

JS:   console.assert(x > 0);
来源：http://kba.aibaodan.cn

TS:   console.assert(x > 0);
来源：http://tmv.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://geo.gzhubu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jtk.aibaodan.cn

Ruby: raise "必须为正" unless x > 0
来源：http://umg.daria6918.cn

C#:   Debug.Assert(x > 0);
来源：http://zxb.pycfn.com

[H08] 获取错误信息与堆栈
来源：http://oga.pycfn.com

Py:   str(e);  traceback.format_exc()
来源：http://stf.vqdsnc.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kus.zhoulong.xyz

JS:   e.message;  e.stack
来源：http://fof.sysykeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ezw.cqqwz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hky.dashuyun.cn

Go:   err.Error()
来源：http://tsf.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://xqd.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://bao.cdnleiting.top

[H09] 带错误码的异常
来源：http://hxk.vehdjk.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nmv.bjfxy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kpl.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pwd.svipenyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cwf.aizwys.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://egz.cdnleiting.top


<!-- 参考信息 -->