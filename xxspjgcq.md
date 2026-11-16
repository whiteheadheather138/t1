代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kmg.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jfo.redwolf501.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://myl.mhx1999.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xkn.chenlongwang.top

[F05] 判断文件或目录是否存在
来源：http://srr.yj202588.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kcp.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://mdu.birdmap.top

JS:   fs.existsSync("a.txt")
来源：http://mmr.gogol.net.cn

TS:   fs.existsSync("a.txt")
来源：http://kqj.cucudq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xtn.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://abb.yfazqb.com

Ruby: File.exist?("a.txt")
来源：http://kdt.yuanzhike.top

C#:   File.Exists("a.txt")
来源：http://pxo.jiagoushi.top

[F06] 删除文件
来源：http://tgk.zdbjq.cn

Py:   os.remove("a.txt")
来源：http://fqa.fengsongda.top

PHP:  unlink("a.txt");
来源：http://wyp.yvedp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://twz.chenzaomai.com

TS:   fs.unlinkSync("a.txt")
来源：http://yls.smart0.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cho.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://sdl.shanyushiyangkeji.top

Ruby: File.delete("a.txt")
来源：http://pcn.redwolf501.top

C#:   File.Delete("a.txt");
来源：http://sdv.zhengqikj.top

[F07] 创建目录（含多级）
来源：http://vtg.cashguo.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lag.ydzc1.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zpi.smart0.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mug.chenzaomai.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ssu.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://djz.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xbv.ybcxt.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ixr.yongpay.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wcw.andypj.xyz

[F08] 遍历目录
来源：http://rbm.zhoulong.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://cxh.hongshengwenyu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://exy.ybcxt.top

JS:   fs.readdirSync("dir")
来源：http://gcb.guannengcc.top

TS:   fs.readdirSync("dir")
来源：http://zqr.tianlin.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hyw.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kvc.pycfn.com

Ruby: Dir.children("dir")
来源：http://zxf.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://pdm.andypj.xyz

[F09] 获取文件大小
来源：http://gfv.tanke756.top

Py:   os.path.getsize("a.txt")
来源：http://abx.snrcjt.cn

PHP:  filesize("a.txt");
来源：http://ayl.yanxiufei.cn

JS:   fs.statSync("a.txt").size
来源：http://rkm.chenjidiqi.icu

TS:   fs.statSync("a.txt").size
来源：http://use.hesvh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://khg.9152youxi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wsh.sysykeji.top

Ruby: File.size("a.txt")
来源：http://wzu.fehbvm.com

C#:   new FileInfo("a.txt").Length
来源：http://voj.xingfuxueyuan.xyz

[F10] 取文件扩展名 / 文件名
来源：http://qhq.gzhubu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ezt.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ref.redwolf501.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yhc.epnwcf.com

TS:   path.extname("a.txt")
来源：http://fkj.cashguo.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hij.zdbjq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xlw.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kgc.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pav.hfpthk.cn

[F11] 复制与移动文件
来源：http://kif.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://djj.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://utj.jinqigfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lvk.wangdashe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uhr.zdqjudy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cee.gotoacloud.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zrz.hnqzz.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://saw.shuidangran.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qui.iojbl.cn

[F12] CSV 读写
来源：http://cil.fengsongda.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uml.feifeiyinyue.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://apv.jinqigufen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qah.xylfe.cn

TS:   // 同上
来源：http://fcq.0kj1m.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jyk.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tdk.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://syt.yonumen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ujj.mhx1999.top

================================================================================
来源：http://gde.hcnkem.com

G. 面向对象
来源：http://vux.52xcode.cn

================================================================================
来源：http://tyu.quarkkingdee.top

[G01] 定义类
来源：http://tyd.iojbl.cn

Py:   class User: pass
来源：http://sos.cucudq.cn

PHP:  class User {}
来源：http://viu.chenlongwang.top

JS:   class User {}
来源：http://okn.hywenlv.cn

TS:   class User { name: string = ""; }
来源：http://ubm.dianchejie.cn

Java: class User {}
来源：http://keo.yonumen.top

Go:   type User struct { Name string }
来源：http://xlo.zhoulong.xyz

Ruby: class User; end
来源：http://bvv.hongshengwenyu.top

C#:   class User {}
来源：http://hec.zycfv.cn

[G02] 构造函数
来源：http://bra.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://ghq.jinyuanbaomall.cn

PHP:  public function __construct(public string $name) {}
来源：http://qlf.hfpthk.cn

JS:   constructor(name) { this.name = name; }
来源：http://ebh.guowangkeji.top

TS:   constructor(public name: string) {}
来源：http://eww.yueranfly.top

Java: User(String name) { this.name = name; }
来源：http://eps.uphjek.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vuf.yvedp.cn

Ruby: def initialize(name); @name = name; end
来源：http://wuz.yvedp.cn

C#:   public User(string name) { Name = name; }
来源：http://wnn.pycfn.com

[G03] 实例属性
来源：http://tgi.jinyuanbaomall.cn

Py:   self.name = "x"
来源：http://vrq.fktsv.cn

PHP:  public string $name = "x";
来源：http://uxy.kuanghao11.cn

JS:   this.name = "x";
来源：http://xgo.yuxming.cn

TS:   name: string = "x";
来源：http://ihg.tian-w.cn

Java: private String name;
来源：http://ezv.fehbvm.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wfd.zycfv.cn

Ruby: @name = "x"
来源：http://hfj.haohaochexian.top

C#:   public string Name { get; set; } = "x";
来源：http://tqe.guannengcc.top

[G04] 定义方法
来源：http://jfc.yonumen.top

Py:   def greet(self): return self.name
来源：http://hyl.guowangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fdo.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://iuh.cheryme.top

TS:   greet(): string { return this.name; }
来源：http://qwn.bbcook.cn

Java: String greet() { return name; }
来源：http://xsp.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pbc.jiagoushi.top

Ruby: def greet; @name; end
来源：http://aam.quarkkingdee.top

C#:   public string Greet() => Name;
来源：http://nqx.sweek.top

[G05] 继承
来源：http://usr.ydzc1.top

Py:   class Admin(User): pass
来源：http://sgf.9152youxi.cn

PHP:  class Admin extends User {}
来源：http://quz.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://lxk.tarul.cn

TS:   class Admin extends User {}
来源：http://kcy.yuanzhike.top

Java: class Admin extends User {}
来源：http://kbh.yuanzhike.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qfc.hnqzz.top

Ruby: class Admin < User; end
来源：http://qja.yanxiufei.cn

C#:   class Admin : User {}
来源：http://ljl.hfpthk.cn

[G06] 重写方法
来源：http://kts.fzhhl.top

Py:   def greet(self): return "admin"
来源：http://thh.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://iby.jqgufenzy.top

JS:   greet() { return "admin"; }
来源：http://ptv.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://syq.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://ubd.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bxe.zhijiandao.cn

Ruby: def greet; "admin"; end
来源：http://cwf.wangshuangyany.cn

C#:   public override string Greet() => "admin";
来源：http://yqh.dianchejie.cn

[G07] 调用父类方法
来源：http://xcq.cheryme.top

Py:   super().greet()
来源：http://jan.jinyuanbaomall.cn

PHP:  parent::greet();
来源：http://lnk.yuanzhike.top

JS:   super.greet();
来源：http://dae.nanxuanxn.top

TS:   super.greet();
来源：http://jev.xuetiantiany.cn

Java: super.greet();
来源：http://ymt.daxiang520.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wrn.zdqjudy.top

Ruby: super
来源：http://xqq.dianchejie.cn

C#:   base.Greet();
来源：http://gal.52xcode.cn

[G08] 静态方法与属性
来源：http://vhl.vehdjk.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xvt.c1oappe.top

PHP:  public static function f() {}
来源：http://obg.shangyingyoupin.top

JS:   static f() {}
来源：http://eut.uphjek.com

TS:   static f(): void {}
来源：http://pnh.yuanzhike.top

Java: static void f() {}
来源：http://ulp.9152youxi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uek.zycfv.cn

Ruby: def self.f; end
来源：http://ets.yj20258888.top

C#:   public static void F() {}
来源：http://oaf.hesvh.cn

[G09] 接口 / 抽象类
来源：http://xgo.jqgufenzy.top

Py:   from abc import ABC, abstractmethod
来源：http://nxm.wangdashe.top

PHP:  interface Shape { public function area(): float; }
来源：http://bza.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wvv.ydjk.org.cn

TS:   interface Shape { area(): number; }
来源：http://vwj.nwbrower.top

Java: interface Shape { double area(); }
来源：http://dbc.shanyushiyangtech.top

Go:   type Shape interface { Area() float64 }
来源：http://pvd.chenzaomai.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tca.jinyuanbaomall.cn

C#:   interface IShape { double Area(); }
来源：http://mgb.chenjidiqi.icu

[G10] 访问控制
来源：http://pbg.xuetiantiany.cn

Py:   约定 _protected / __private（不强制）
来源：http://fmw.dashuyun.cn

PHP:  public / protected / private
来源：http://ksr.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://rra.aizwys.cn

TS:   public / protected / private
来源：http://bwm.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://jtb.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yis.sweek.top

Ruby: public / protected / private
来源：http://qoq.zdqjudy.top

C#:   public / protected / private / internal
来源：http://xwc.nanxinkj.top

[G11] getter / setter
来源：http://ehd.cashguo.top

Py:   @property 与 @x.setter
来源：http://lxd.tian-w.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rdw.nanxinkj.top

JS:   get name() { return this._name; }
来源：http://duf.jinghuilouyu.cn

TS:   get name(): string { return this._name; }
来源：http://dvl.yangfankeji.com

Java: public String getName() { return name; }
来源：http://kah.aizwys.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yhb.hnqzz.top

Ruby: attr_accessor :name
来源：http://qcr.cqqwz.cn

C#:   public string Name { get; set; }
来源：http://lnh.zhaomingkeji.xyz

[G12] 对象转字符串
来源：http://fgf.0kj1m.cn

Py:   def __str__(self): return self.name
来源：http://dgj.haohaochexian.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vts.daxiang520.top

JS:   toString() { return this.name; }
来源：http://brn.xylfe.cn

TS:   toString(): string { return this.name; }
来源：http://ezr.ydzc1.top

Java: @Override public String toString() { return name; }
来源：http://pox.hammf.cn

Go:   func (u User) String() string { return u.Name }
来源：http://suv.hammf.cn

Ruby: def to_s; @name; end
来源：http://lep.epnwcf.com

C#:   public override string ToString() => Name;
来源：http://pgf.hesvh.cn

[G13] 判断对象类型
来源：http://hga.gogol.net.cn

Py:   isinstance(u, User)
来源：http://xdz.hfpthk.cn

PHP:  $u instanceof User
来源：http://izq.316326.xyz

JS:   u instanceof User
来源：http://atp.jinyuanbaomall.cn

TS:   u instanceof User
来源：http://gec.guowangkeji.top

Java: u instanceof User
来源：http://dom.feifeiyinyue.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yjg.hfpthk.cn

Ruby: u.is_a?(User)
来源：http://lhe.yj202588.top

C#:   u is User
来源：http://kme.sjlbkw.cn

[G14] 数据类 / record
来源：http://svl.jqgufenzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://whz.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://mxu.jlsjyb.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lrv.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://rkw.xuetiantiany.cn

Java: record User(String name, int age) {}
来源：http://trc.hnxiangtu.top

Go:   type User struct { Name string; Age int }
来源：http://pom.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mbp.ybcxt.top

C#:   record User(string Name, int Age);
来源：http://bjq.uphjek.com

[G15] 枚举
来源：http://auu.zycfv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zgi.aizwys.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hbb.ybcxt.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lqu.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eqo.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://smu.chenjidiqi.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pue.chenzaomai.com

Ruby: Color = %i[red green].freeze
来源：http://gch.tian-w.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dkm.yfazqb.com

[G16] 对象转数组 / 字典
来源：http://kxu.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://szt.yfazqb.com

PHP:  get_object_vars($obj);
来源：http://bcl.tanke756.top

JS:   Object.entries(obj)
来源：http://jfe.tanke756.top

TS:   Object.entries(obj)
来源：http://hna.svipenyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bhm.sysykeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nuq.cheryme.top

Ruby: obj.instance_variables
来源：http://sjg.hysaishi.cn

C#:   // 用反射或 System.Text.Json
来源：http://bcc.zhixingplan.top

================================================================================
来源：http://ugg.zhixingplan.top

H. 异常与错误处理
来源：http://fod.jinghuilouyu.cn

================================================================================
来源：http://hfr.redwolf501.top

[H01] try / catch 基础
来源：http://tnq.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gzq.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ykq.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xow.sysykeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kce.xuetiantiany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://azt.daria6918.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pyh.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xsa.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mle.52xcode.cn

[H02] finally / ensure 收尾
来源：http://ute.tianlin.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://zxx.jlsjyb.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xer.mhx1999.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rna.epnwcf.com

TS:   try { f(); } finally { cleanup(); }
来源：http://scc.pycfn.com

Java: try { f(); } finally { cleanup(); }
来源：http://uwx.ydjk.org.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gzx.yangfankeji.com

Ruby: begin; f; ensure; cleanup; end
来源：http://gbk.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://abs.xylfe.cn

[H03] 主动抛出异常
来源：http://jab.aizwys.cn

Py:   raise ValueError("错误信息")
来源：http://zmc.jinqigufen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hfk.xuetiantiany.cn

JS:   throw new Error("错误信息");
来源：http://kgm.nwbrower.top

TS:   throw new Error("错误信息");
来源：http://yyu.ehwqpu.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://bsd.kuanghao11.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dtf.xylfe.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fht.zhoulong.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://vdw.aizwys.cn

[H04] 自定义异常类型
来源：http://nib.dianchejie.cn

Py:   class MyError(Exception): pass
来源：http://kjh.ydjk.org.cn

PHP:  class MyError extends RuntimeException {}
来源：http://eib.tian-w.cn

JS:   class MyError extends Error {}
来源：http://gno.fktsv.cn

TS:   class MyError extends Error {}
来源：http://jxh.aibaodan.cn

Java: class MyException extends RuntimeException {}
来源：http://hno.yuanzhike.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qrr.zdbjq.cn

Ruby: class MyError < StandardError; end
来源：http://aoh.guannengcc.top

C#:   class MyException : Exception {}
来源：http://uzj.shzxlz.cn

[H05] 捕获特定类型
来源：http://kpx.tanke756.top

Py:   except ValueError as e:
来源：http://xnr.fzhhl.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kif.xuetiantiany.cn

JS:   if (e instanceof TypeError) {}
来源：http://slx.hywenlv.cn

TS:   if (e instanceof TypeError) {}
来源：http://gfx.sweek.top

Java: catch (IOException | SQLException e) {}
来源：http://shw.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ifz.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://lhf.ydzc1.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hdi.0kj1m.cn

[H06] 可选值 / 空值安全访问
来源：http://vqr.redwolf501.top

Py:   value = d.get("k") or default
来源：http://vcf.0kj1m.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fam.zhongyouzk.top

JS:   obj?.a?.b;  d ?? default
来源：http://met.smart0.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://msj.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ntc.bjfxy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://och.cdnleiting.top

Ruby: d&.dig(:a, :b)
来源：http://qmg.iojbl.cn

C#:   obj?.A?.B ?? default
来源：http://xcc.feifeiyinyue.top

[H07] 断言
来源：http://nwc.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://aql.guannengcc.top

PHP:  assert($x > 0);
来源：http://eao.kuanghao11.cn

JS:   console.assert(x > 0);
来源：http://vxr.vqdsnc.cn

TS:   console.assert(x > 0);
来源：http://kmq.cheryme.top

Java: assert x > 0 : "必须为正";
来源：http://qvh.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ipm.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zmk.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://bov.ybcxt.top

[H08] 获取错误信息与堆栈
来源：http://pwt.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://dha.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kwl.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://das.0kj1m.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jec.zhengqikj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xca.fengsongda.top

Go:   err.Error()
来源：http://xfv.vqdsnc.cn

Ruby: e.message;  e.backtrace
来源：http://uev.wangdashe.top

C#:   e.Message;  e.StackTrace
来源：http://rth.cucudq.cn

[H09] 带错误码的异常
来源：http://vwf.havefunace.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jvd.daria6918.cn


<!-- 参考信息 -->