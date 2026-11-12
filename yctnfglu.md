代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xgx.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://edx.birdmap.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fdw.hysaishi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://add.jiagoushi.top

[F05] 判断文件或目录是否存在
来源：http://fiy.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xet.cdnleiting.top

PHP:  file_exists("a.txt");
来源：http://fmh.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://qhu.yuanzhike.top

TS:   fs.existsSync("a.txt")
来源：http://xro.yangfankeji.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ckh.c1oappe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rex.jinqigufen.top

Ruby: File.exist?("a.txt")
来源：http://ibf.zdbjq.cn

C#:   File.Exists("a.txt")
来源：http://ibf.sysykeji.top

[F06] 删除文件
来源：http://znv.316326.xyz

Py:   os.remove("a.txt")
来源：http://asf.cheryme.top

PHP:  unlink("a.txt");
来源：http://tjx.fanxiaobao.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://nzs.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://udx.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ccw.havefunace.top

Go:   os.Remove("a.txt")
来源：http://zme.smart0.xyz

Ruby: File.delete("a.txt")
来源：http://ase.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://qgl.zycfv.cn

[F07] 创建目录（含多级）
来源：http://lhi.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ogm.yuxming.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lre.jianghu66.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cwl.hcnkem.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gqd.fengsongda.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lkn.nanxinkj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aaf.hnqzz.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://teq.xuanzx.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ohc.dashuyun.cn

[F08] 遍历目录
来源：http://kjp.haohaochexian.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fxi.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xqe.jinyuanbaomall.cn

JS:   fs.readdirSync("dir")
来源：http://sfl.52xcode.cn

TS:   fs.readdirSync("dir")
来源：http://yib.zhaomingkeji.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hkw.hongshengwenyu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xor.sysykeji.top

Ruby: Dir.children("dir")
来源：http://tsz.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://isj.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://ueg.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://syl.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://gzt.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://kxy.sjlbkw.cn

TS:   fs.statSync("a.txt").size
来源：http://yiw.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://qzy.xylfe.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fat.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://zzy.iojbl.cn

C#:   new FileInfo("a.txt").Length
来源：http://gdo.xinyue.icu

[F10] 取文件扩展名 / 文件名
来源：http://aoa.jqgfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://utv.yuxming.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vlu.jqgfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xwy.ydzc1.top

TS:   path.extname("a.txt")
来源：http://qjt.fengsongda.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rjl.daxiang520.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tjz.gaohongyu789.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://waq.hfpthk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aue.ctjpmb.com

[F11] 复制与移动文件
来源：http://fzu.vehdjk.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rhg.yfazqb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jaj.fehbvm.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ugl.nanxinkj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vaw.shzxlz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ylf.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bgs.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cae.aibaodan.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://alp.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://ynd.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qby.jinghuilouyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://roy.tanke756.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jgr.hongshengwenyu.top

TS:   // 同上
来源：http://tpa.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wcy.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mqk.meibo888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vug.zdbjq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fxd.gogol.net.cn

================================================================================
来源：http://hav.svipenyu.cn

G. 面向对象
来源：http://yjr.hywenlv.cn

================================================================================
来源：http://nuq.sufxvd.cn

[G01] 定义类
来源：http://dak.nanxuanxn.top

Py:   class User: pass
来源：http://mjd.nanxuanxn.top

PHP:  class User {}
来源：http://vut.feifeiyinyue.top

JS:   class User {}
来源：http://ydd.zycfv.cn

TS:   class User { name: string = ""; }
来源：http://ser.meibo888.top

Java: class User {}
来源：http://oxv.xuanzx.com

Go:   type User struct { Name string }
来源：http://zwy.sufxvd.cn

Ruby: class User; end
来源：http://ryb.jyoumei.cn

C#:   class User {}
来源：http://ovn.nanxinkj.top

[G02] 构造函数
来源：http://vrg.aibaodan.cn

Py:   def __init__(self, name): self.name = name
来源：http://oph.zdbjq.cn

PHP:  public function __construct(public string $name) {}
来源：http://bde.fktsv.cn

JS:   constructor(name) { this.name = name; }
来源：http://gsy.hysaishi.cn

TS:   constructor(public name: string) {}
来源：http://jxn.chenjidiqi.icu

Java: User(String name) { this.name = name; }
来源：http://eox.uphjek.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dpf.andypj.xyz

Ruby: def initialize(name); @name = name; end
来源：http://khm.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://upz.pycfn.com

[G03] 实例属性
来源：http://ufr.yanxiufei.cn

Py:   self.name = "x"
来源：http://bbq.chenlongwang.top

PHP:  public string $name = "x";
来源：http://ywr.zhixingplan.top

JS:   this.name = "x";
来源：http://trx.dianchejie.cn

TS:   name: string = "x";
来源：http://yzk.jlsjyb.cn

Java: private String name;
来源：http://jtf.zdbjq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ofv.birdmap.top

Ruby: @name = "x"
来源：http://gal.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://xye.aizwys.cn

[G04] 定义方法
来源：http://ure.birdmap.top

Py:   def greet(self): return self.name
来源：http://muy.snrcjt.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://aph.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://htq.havefunace.top

TS:   greet(): string { return this.name; }
来源：http://zdw.xuanzx.com

Java: String greet() { return name; }
来源：http://pge.haohaochexian.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hrr.yj20258.top

Ruby: def greet; @name; end
来源：http://rgg.ivvv.top

C#:   public string Greet() => Name;
来源：http://tbn.gaohongyu789.top

[G05] 继承
来源：http://fud.daria6918.cn

Py:   class Admin(User): pass
来源：http://mmm.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://xdb.yj202588.top

JS:   class Admin extends User {}
来源：http://asa.zhengqikj.top

TS:   class Admin extends User {}
来源：http://rgo.gogol.net.cn

Java: class Admin extends User {}
来源：http://qyn.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kjl.52xcode.cn

Ruby: class Admin < User; end
来源：http://kmw.jlsjyb.cn

C#:   class Admin : User {}
来源：http://ckp.sysykeji.top

[G06] 重写方法
来源：http://yvs.smart0.xyz

Py:   def greet(self): return "admin"
来源：http://gsk.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ksu.wangshuangyany.cn

JS:   greet() { return "admin"; }
来源：http://oda.redwolf501.top

TS:   greet(): string { return "admin"; }
来源：http://hcz.birdmap.top

Java: @Override String greet() { return "admin"; }
来源：http://ady.yonumen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hse.zhoulong.xyz

Ruby: def greet; "admin"; end
来源：http://wwc.cashguo.top

C#:   public override string Greet() => "admin";
来源：http://oar.jinqigfzy.top

[G07] 调用父类方法
来源：http://btu.yj20258.top

Py:   super().greet()
来源：http://vzv.zdbjq.cn

PHP:  parent::greet();
来源：http://oky.52xcode.cn

JS:   super.greet();
来源：http://jkm.jinyuanbaomall.cn

TS:   super.greet();
来源：http://zel.vqdsnc.cn

Java: super.greet();
来源：http://pwm.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ooa.sxryk.cn

Ruby: super
来源：http://qdz.guowangkeji.top

C#:   base.Greet();
来源：http://gie.jyoumei.cn

[G08] 静态方法与属性
来源：http://obv.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://clo.yuanzhike.top

PHP:  public static function f() {}
来源：http://hxd.hnxiangtu.top

JS:   static f() {}
来源：http://kjl.yueranfly.top

TS:   static f(): void {}
来源：http://nqc.jlsjyb.cn

Java: static void f() {}
来源：http://jeg.hysaishi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mqf.zhaomingkeji.xyz

Ruby: def self.f; end
来源：http://vns.epnwcf.com

C#:   public static void F() {}
来源：http://eho.havefunace.top

[G09] 接口 / 抽象类
来源：http://fjg.zdbjq.cn

Py:   from abc import ABC, abstractmethod
来源：http://vuk.shanyushiyangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://vkc.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qsr.jqgufenzy.top

TS:   interface Shape { area(): number; }
来源：http://ryw.sweek.top

Java: interface Shape { double area(); }
来源：http://uin.chenjidiqi.icu

Go:   type Shape interface { Area() float64 }
来源：http://tsp.hnxiangtu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lee.tian-w.cn

C#:   interface IShape { double Area(); }
来源：http://swx.hywenlv.cn

[G10] 访问控制
来源：http://bin.vehdjk.com

Py:   约定 _protected / __private（不强制）
来源：http://dqo.svipenyu.cn

PHP:  public / protected / private
来源：http://rck.gzhubu.top

JS:   #private 字段；其余公开
来源：http://hka.xuanzx.com

TS:   public / protected / private
来源：http://ypq.fehbvm.com

Java: public / protected / private / 默认包级
来源：http://nio.yj202588.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://znk.316326.xyz

Ruby: public / protected / private
来源：http://ddi.iojbl.cn

C#:   public / protected / private / internal
来源：http://bcm.fktsv.cn

[G11] getter / setter
来源：http://jyy.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://mau.sxryk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hbq.zhengqikj.top

JS:   get name() { return this._name; }
来源：http://spd.dashuyun.cn

TS:   get name(): string { return this._name; }
来源：http://lez.uphjek.com

Java: public String getName() { return name; }
来源：http://zpj.jlsjyb.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gle.xingfuxueyuan.xyz

Ruby: attr_accessor :name
来源：http://cjw.zdbjq.cn

C#:   public string Name { get; set; }
来源：http://caq.chenlongwang.top

[G12] 对象转字符串
来源：http://xup.sxryk.cn

Py:   def __str__(self): return self.name
来源：http://viv.shanyushiyangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zuz.sysykeji.top

JS:   toString() { return this.name; }
来源：http://lau.ywan-chungtsiang.top

TS:   toString(): string { return this.name; }
来源：http://edx.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://wjc.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fuw.andypj.xyz

Ruby: def to_s; @name; end
来源：http://nas.zycfv.cn

C#:   public override string ToString() => Name;
来源：http://ogo.shzxlz.cn

[G13] 判断对象类型
来源：http://qgj.andypj.xyz

Py:   isinstance(u, User)
来源：http://jwz.jinqigufen.top

PHP:  $u instanceof User
来源：http://zyn.kuanghao11.cn

JS:   u instanceof User
来源：http://scp.jinqigufen.top

TS:   u instanceof User
来源：http://djz.iojbl.cn

Java: u instanceof User
来源：http://rbu.zhixingplan.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ogt.nwbrower.top

Ruby: u.is_a?(User)
来源：http://abe.feifeiyinyue.top

C#:   u is User
来源：http://wvp.ybcxt.top

[G14] 数据类 / record
来源：http://wpi.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xmq.xuetiantiany.cn

PHP:  // 用 readonly 属性模拟
来源：http://hwx.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zdm.yvedp.cn

TS:   type User = { name: string; age: number };
来源：http://tkj.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://zwa.yvedp.cn

Go:   type User struct { Name string; Age int }
来源：http://ucm.pycfn.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sjb.yonumen.top

C#:   record User(string Name, int Age);
来源：http://awr.jiagoushi.top

[G15] 枚举
来源：http://jre.yangfankeji.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://exr.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ami.tian-w.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bcw.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wxz.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://jja.smart0.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vex.jlsjyb.cn

Ruby: Color = %i[red green].freeze
来源：http://iwm.sjlbkw.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gnx.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://sef.daxiang520.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zaq.tarul.cn

PHP:  get_object_vars($obj);
来源：http://jhs.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://jam.nanxuanxn.top

TS:   Object.entries(obj)
来源：http://eia.xingfuxueyuan.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://drv.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://khd.xuetiantiany.cn

Ruby: obj.instance_variables
来源：http://ctj.hfpthk.cn

C#:   // 用反射或 System.Text.Json
来源：http://xiv.yuanzhike.top

================================================================================
来源：http://eiy.svipenyu.cn

H. 异常与错误处理
来源：http://zht.xuanzx.com

================================================================================
来源：http://jnw.fehbvm.com

[H01] try / catch 基础
来源：http://gia.hongshengwenyu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kyh.52xcode.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rze.pengpengdd.cyou

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yfs.tarul.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yst.bjfxy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eyh.xziqi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qgk.wangshuangyany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yij.sufxvd.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qhm.nwbrower.top

[H02] finally / ensure 收尾
来源：http://zsj.sxryk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://act.yueranfly.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ect.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lyl.xuanzx.com

TS:   try { f(); } finally { cleanup(); }
来源：http://rzm.tarul.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hbr.zhongyouzk.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dub.zdbjq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rqj.zhijiandao.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yoy.fanxiaobao.xyz

[H03] 主动抛出异常
来源：http://eta.nwbrower.top

Py:   raise ValueError("错误信息")
来源：http://ohv.havefunace.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://him.zhoulong.xyz

JS:   throw new Error("错误信息");
来源：http://fgm.dashuyun.cn

TS:   throw new Error("错误信息");
来源：http://bsq.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://ikr.xingfuxueyuan.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bxc.hammf.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://flx.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://iih.yueranfly.top

[H04] 自定义异常类型
来源：http://rpu.jyoumei.cn

Py:   class MyError(Exception): pass
来源：http://qnq.gaohongyu789.top

PHP:  class MyError extends RuntimeException {}
来源：http://xsi.hfpthk.cn

JS:   class MyError extends Error {}
来源：http://igo.zycfv.cn

TS:   class MyError extends Error {}
来源：http://hil.shangyingyoupin.top

Java: class MyException extends RuntimeException {}
来源：http://hdz.jqgfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mgq.svipenyu.cn

Ruby: class MyError < StandardError; end
来源：http://zou.vehdjk.com

C#:   class MyException : Exception {}
来源：http://faj.dashuyun.cn

[H05] 捕获特定类型
来源：http://xls.shanyushiyangkeji.top

Py:   except ValueError as e:
来源：http://jhg.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pkp.yfazqb.com

JS:   if (e instanceof TypeError) {}
来源：http://hez.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://gfa.shangyingyoupin.top

Java: catch (IOException | SQLException e) {}
来源：http://uoh.quarkkingdee.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jck.kuanghao11.cn

Ruby: rescue ArgumentError => e
来源：http://mjg.daria6918.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://crd.jinqigfzy.top

[H06] 可选值 / 空值安全访问
来源：http://haf.jqgufenzy.top

Py:   value = d.get("k") or default
来源：http://ebj.9152youxi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gno.pengpengdd.cyou

JS:   obj?.a?.b;  d ?? default
来源：http://idn.jqgfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://fqo.wangshuangyany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fwu.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://yim.birdmap.top

Ruby: d&.dig(:a, :b)
来源：http://kmn.nwbrower.top

C#:   obj?.A?.B ?? default
来源：http://idm.yangfankeji.com

[H07] 断言
来源：http://opt.jqgfzy.top

Py:   assert x > 0, "必须为正"
来源：http://sjz.jyoumei.cn

PHP:  assert($x > 0);
来源：http://qex.tanke756.top

JS:   console.assert(x > 0);
来源：http://cvw.nanxuanxn.top

TS:   console.assert(x > 0);
来源：http://tuy.quarkkingdee.top

Java: assert x > 0 : "必须为正";
来源：http://lmk.ppjwa.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hiw.cqqwz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fmf.tianlin.xyz

C#:   Debug.Assert(x > 0);
来源：http://bmv.svipenyu.cn

[H08] 获取错误信息与堆栈
来源：http://lhk.shangyingyoupin.top

Py:   str(e);  traceback.format_exc()
来源：http://npk.tian-w.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sgj.zhaomingkeji.xyz

JS:   e.message;  e.stack
来源：http://pnh.hammf.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://oyg.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ktq.hnxiangtu.top

Go:   err.Error()
来源：http://wos.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://dye.guannengcc.top

C#:   e.Message;  e.StackTrace
来源：http://qtp.guannengcc.top

[H09] 带错误码的异常
来源：http://hwp.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dvi.hysaishi.cn


<!-- 参考信息 -->