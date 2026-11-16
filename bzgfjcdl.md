代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yie.tianlin.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://twf.fehbvm.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dex.haohaochexian.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ppd.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wfv.sufxvd.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cnx.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://noe.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xnk.jianghu66.top

[F05] 判断文件或目录是否存在
来源：http://awi.ehwqpu.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hel.yanxiufei.cn

PHP:  file_exists("a.txt");
来源：http://hke.gaohongyu789.top

JS:   fs.existsSync("a.txt")
来源：http://jza.ywan-chungtsiang.top

TS:   fs.existsSync("a.txt")
来源：http://opi.feifeiyinyue.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bsn.hnxiangtu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://znl.yuxming.cn

Ruby: File.exist?("a.txt")
来源：http://mwu.shuidangran.top

C#:   File.Exists("a.txt")
来源：http://cgf.zhijiandao.cn

[F06] 删除文件
来源：http://qbh.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://jhw.xziqi.cn

PHP:  unlink("a.txt");
来源：http://izw.yangfankeji.com

JS:   fs.unlinkSync("a.txt")
来源：http://dtd.gzhubu.top

TS:   fs.unlinkSync("a.txt")
来源：http://uyd.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://een.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://ugh.yuanzhike.top

Ruby: File.delete("a.txt")
来源：http://fus.gaohongyu789.top

C#:   File.Delete("a.txt");
来源：http://wpg.shzxlz.cn

[F07] 创建目录（含多级）
来源：http://fcw.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://emt.yfazqb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ycb.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ccb.guowangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rox.hnqzz.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tpx.birdmap.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://htm.guowangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hxm.fanxiaobao.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wtc.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://mju.vqdsnc.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vbe.wangshuangyany.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dff.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://aqp.vehdjk.com

TS:   fs.readdirSync("dir")
来源：http://xiv.chenzaomai.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uvg.cucudq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xdi.gzhubu.top

Ruby: Dir.children("dir")
来源：http://nnq.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://gjk.kuanghao11.cn

[F09] 获取文件大小
来源：http://ihm.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://juw.nanxinkj.top

PHP:  filesize("a.txt");
来源：http://zgr.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://gas.cucudq.cn

TS:   fs.statSync("a.txt").size
来源：http://tox.dianchejie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hbh.xylfe.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fbs.quarkkingdee.top

Ruby: File.size("a.txt")
来源：http://obd.jqgufenzy.top

C#:   new FileInfo("a.txt").Length
来源：http://mtp.ydjk.org.cn

[F10] 取文件扩展名 / 文件名
来源：http://unn.epnwcf.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ygi.zdbjq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://laz.smart0.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uae.ydjk.org.cn

TS:   path.extname("a.txt")
来源：http://xqt.zhaomingkeji.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zdp.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dok.ydjk.org.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fus.hywenlv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nem.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://edj.yvedp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rdk.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bjc.yj20258.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ubl.haohaochexian.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ukn.wangshuangyany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mov.hesvh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xqa.yueranfly.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rbk.xinyue.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hnk.shanyushiyangtech.top

[F12] CSV 读写
来源：http://wmm.yuxming.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cgp.zhongyouzk.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aue.nanxinkj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uld.svipenyu.cn

TS:   // 同上
来源：http://alx.svipenyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qib.316326.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://asx.aibaodan.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://alv.jqgufenzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://caz.yuanzhike.top

================================================================================
来源：http://zad.xziqi.cn

G. 面向对象
来源：http://cse.c1oappe.top

================================================================================
来源：http://ryh.sxryk.cn

[G01] 定义类
来源：http://fyu.ydjk.org.cn

Py:   class User: pass
来源：http://tzc.c1oappe.top

PHP:  class User {}
来源：http://sfq.guowangkeji.top

JS:   class User {}
来源：http://fsn.zhaomingkeji.xyz

TS:   class User { name: string = ""; }
来源：http://pxm.xuetiantiany.cn

Java: class User {}
来源：http://rht.0kj1m.cn

Go:   type User struct { Name string }
来源：http://xdv.jianghu66.top

Ruby: class User; end
来源：http://ixx.c1oappe.top

C#:   class User {}
来源：http://hse.0kj1m.cn

[G02] 构造函数
来源：http://can.jiagoushi.top

Py:   def __init__(self, name): self.name = name
来源：http://ydv.zdbjq.cn

PHP:  public function __construct(public string $name) {}
来源：http://vcx.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://ioj.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://jay.wangshuangyany.cn

Java: User(String name) { this.name = name; }
来源：http://ouk.nwbrower.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hxm.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://boa.mhx1999.top

C#:   public User(string name) { Name = name; }
来源：http://hme.hnqzz.top

[G03] 实例属性
来源：http://unu.guowangkeji.top

Py:   self.name = "x"
来源：http://ijd.cdnleiting.top

PHP:  public string $name = "x";
来源：http://uwm.jqgfzy.top

JS:   this.name = "x";
来源：http://ewg.fehbvm.com

TS:   name: string = "x";
来源：http://ezm.uphjek.com

Java: private String name;
来源：http://wau.tian-w.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://olk.kuanghao11.cn

Ruby: @name = "x"
来源：http://egh.zycfv.cn

C#:   public string Name { get; set; } = "x";
来源：http://nca.dianchejie.cn

[G04] 定义方法
来源：http://rpr.tarul.cn

Py:   def greet(self): return self.name
来源：http://mco.daxiang520.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qag.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://wgm.fktsv.cn

TS:   greet(): string { return this.name; }
来源：http://tlh.zdbjq.cn

Java: String greet() { return name; }
来源：http://isg.ivvv.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bbz.yanxiufei.cn

Ruby: def greet; @name; end
来源：http://kmr.tianlin.xyz

C#:   public string Greet() => Name;
来源：http://mrl.316326.xyz

[G05] 继承
来源：http://tlg.dashuyun.cn

Py:   class Admin(User): pass
来源：http://ump.fehbvm.com

PHP:  class Admin extends User {}
来源：http://hrt.redwolf501.top

JS:   class Admin extends User {}
来源：http://ipy.sufxvd.cn

TS:   class Admin extends User {}
来源：http://cgo.cashguo.top

Java: class Admin extends User {}
来源：http://wmx.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wit.ydzc1.top

Ruby: class Admin < User; end
来源：http://ouu.shanyushiyangkeji.top

C#:   class Admin : User {}
来源：http://osi.uphjek.com

[G06] 重写方法
来源：http://obo.0kj1m.cn

Py:   def greet(self): return "admin"
来源：http://onu.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pmh.yfazqb.com

JS:   greet() { return "admin"; }
来源：http://ytx.epnwcf.com

TS:   greet(): string { return "admin"; }
来源：http://mdi.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://kap.zhaomingkeji.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://smq.iojbl.cn

Ruby: def greet; "admin"; end
来源：http://vfv.shanyushiyangtech.top

C#:   public override string Greet() => "admin";
来源：http://lmq.zhijiandao.cn

[G07] 调用父类方法
来源：http://obb.hongshengwenyu.top

Py:   super().greet()
来源：http://inx.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://whp.daxiang520.top

JS:   super.greet();
来源：http://wma.shangyingyoupin.top

TS:   super.greet();
来源：http://fvy.ppjwa.cn

Java: super.greet();
来源：http://kql.svipenyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xtv.fzhhl.top

Ruby: super
来源：http://gbm.xziqi.cn

C#:   base.Greet();
来源：http://ioa.meibo888.top

[G08] 静态方法与属性
来源：http://nht.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vre.yfazqb.com

PHP:  public static function f() {}
来源：http://ugd.pycfn.com

JS:   static f() {}
来源：http://oqj.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://jtp.ctjpmb.com

Java: static void f() {}
来源：http://kaz.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bgj.xylfe.cn

Ruby: def self.f; end
来源：http://hbp.cheryme.top

C#:   public static void F() {}
来源：http://sao.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://nth.daria6918.cn

Py:   from abc import ABC, abstractmethod
来源：http://fqz.aizwys.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wtq.zhiwuduotai.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jky.9152youxi.cn

TS:   interface Shape { area(): number; }
来源：http://tqf.redwolf501.top

Java: interface Shape { double area(); }
来源：http://lcc.jinqigfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://rhm.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fba.hammf.cn

C#:   interface IShape { double Area(); }
来源：http://dwh.shanyushiyangkeji.top

[G10] 访问控制
来源：http://apc.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://zcd.ctjpmb.com

PHP:  public / protected / private
来源：http://cqv.tianlin.xyz

JS:   #private 字段；其余公开
来源：http://mus.zhoulong.xyz

TS:   public / protected / private
来源：http://itx.jinghuilouyu.cn

Java: public / protected / private / 默认包级
来源：http://gou.dianchejie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lsb.aizwys.cn

Ruby: public / protected / private
来源：http://som.yj20258888.top

C#:   public / protected / private / internal
来源：http://pgn.fengsongda.top

[G11] getter / setter
来源：http://lnl.yuxming.cn

Py:   @property 与 @x.setter
来源：http://ufb.gaohongyu789.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wqx.hnqzz.top

JS:   get name() { return this._name; }
来源：http://jfe.tarul.cn

TS:   get name(): string { return this._name; }
来源：http://gku.zdqjudy.top

Java: public String getName() { return name; }
来源：http://nyy.hongshengwenyu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ozy.yonumen.top

Ruby: attr_accessor :name
来源：http://roe.ydjk.org.cn

C#:   public string Name { get; set; }
来源：http://yxd.xziqi.cn

[G12] 对象转字符串
来源：http://hgg.bjfxy.top

Py:   def __str__(self): return self.name
来源：http://ypt.jinyuanbaomall.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://iwz.yuanzhike.top

JS:   toString() { return this.name; }
来源：http://blf.hammf.cn

TS:   toString(): string { return this.name; }
来源：http://pgi.fengsongda.top

Java: @Override public String toString() { return name; }
来源：http://llh.bjfxy.top

Go:   func (u User) String() string { return u.Name }
来源：http://vnx.yj20258.top

Ruby: def to_s; @name; end
来源：http://gqx.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://yes.yuanzhike.top

[G13] 判断对象类型
来源：http://xfi.cashguo.top

Py:   isinstance(u, User)
来源：http://zny.tianlin.xyz

PHP:  $u instanceof User
来源：http://hes.52xcode.cn

JS:   u instanceof User
来源：http://aqs.xylfe.cn

TS:   u instanceof User
来源：http://pkd.shangyingyoupin.top

Java: u instanceof User
来源：http://qfp.zdbjq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gxr.gogol.net.cn

Ruby: u.is_a?(User)
来源：http://nsn.xylfe.cn

C#:   u is User
来源：http://pva.pengpengdd.cyou

[G14] 数据类 / record
来源：http://pvg.cashguo.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mul.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://apq.cucudq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://apx.hnxiangtu.top

TS:   type User = { name: string; age: number };
来源：http://nkj.nwbrower.top

Java: record User(String name, int age) {}
来源：http://rfi.yj202588.top

Go:   type User struct { Name string; Age int }
来源：http://ktz.iojbl.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cmg.zhixingplan.top

C#:   record User(string Name, int Age);
来源：http://sre.jlsjyb.cn

[G15] 枚举
来源：http://qhj.shangyingyoupin.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://srb.sweek.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tkb.gogol.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dkw.ctjpmb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://box.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://nhy.yanxiufei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kmx.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://cma.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gyn.cashguo.top

[G16] 对象转数组 / 字典
来源：http://slv.cheryme.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cjo.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://sva.aizwys.cn

JS:   Object.entries(obj)
来源：http://lvf.chenzaomai.com

TS:   Object.entries(obj)
来源：http://wty.wangshuangyany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pns.nanxuanxn.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://smw.ywan-chungtsiang.top

Ruby: obj.instance_variables
来源：http://jhp.tarul.cn

C#:   // 用反射或 System.Text.Json
来源：http://oel.kuanghao11.cn

================================================================================
来源：http://lkp.hesvh.cn

H. 异常与错误处理
来源：http://nkv.havefunace.top

================================================================================
来源：http://mcg.nwbrower.top

[H01] try / catch 基础
来源：http://vox.zdqjudy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rew.pengpengdd.cyou

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gus.yongpay.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ong.quarkkingdee.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fhk.yonumen.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xdi.jqgfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qnc.sxryk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://djo.ydjk.org.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blv.yj20258888.top

[H02] finally / ensure 收尾
来源：http://yte.yvedp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oyl.shangyingyoupin.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fev.xuetiantiany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mkz.hongshengwenyu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gag.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://pkr.jqgfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mmo.sweek.top

Ruby: begin; f; ensure; cleanup; end
来源：http://iks.jinqigufen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ugf.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://ozf.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://hng.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wjl.hesvh.cn

JS:   throw new Error("错误信息");
来源：http://hlw.chenzaomai.com

TS:   throw new Error("错误信息");
来源：http://uio.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nfl.cucudq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sae.haohaochexian.top

Ruby: raise ArgumentError, "错误信息"
来源：http://unh.tarul.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kaf.meibo888.top

[H04] 自定义异常类型
来源：http://swk.pengpengdd.cyou

Py:   class MyError(Exception): pass
来源：http://pmu.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ywp.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://hjx.mhx1999.top

TS:   class MyError extends Error {}
来源：http://bie.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://vfm.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kpz.shzxlz.cn

Ruby: class MyError < StandardError; end
来源：http://pkx.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://rjv.xinyue.icu

[H05] 捕获特定类型
来源：http://bvg.quarkkingdee.top

Py:   except ValueError as e:
来源：http://ura.aizwys.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nlq.gotoacloud.top

JS:   if (e instanceof TypeError) {}
来源：http://axu.yvedp.cn

TS:   if (e instanceof TypeError) {}
来源：http://wrf.iojbl.cn

Java: catch (IOException | SQLException e) {}
来源：http://knf.ybcxt.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nzb.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://hak.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://skl.cheryme.top

[H06] 可选值 / 空值安全访问
来源：http://oif.shangyingyoupin.top

Py:   value = d.get("k") or default
来源：http://zwc.316326.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://ggl.pycfn.com

JS:   obj?.a?.b;  d ?? default
来源：http://rsv.vehdjk.com

TS:   obj?.a?.b;  d ?? default
来源：http://ndl.yvedp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://snm.quarkkingdee.top

Go:   if v, ok := m["k"]; ok { }
来源：http://sxd.sweek.top

Ruby: d&.dig(:a, :b)
来源：http://bns.zhoulong.xyz

C#:   obj?.A?.B ?? default
来源：http://afu.uphjek.com

[H07] 断言
来源：http://lda.yuanzhike.top

Py:   assert x > 0, "必须为正"
来源：http://jke.pengpengdd.cyou

PHP:  assert($x > 0);
来源：http://obw.feifeiyinyue.top

JS:   console.assert(x > 0);
来源：http://rfz.cdnleiting.top

TS:   console.assert(x > 0);
来源：http://ago.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://puh.meibo888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dxc.gaohongyu789.top

Ruby: raise "必须为正" unless x > 0
来源：http://aew.pycfn.com

C#:   Debug.Assert(x > 0);
来源：http://zow.jinyuanbaomall.cn

[H08] 获取错误信息与堆栈
来源：http://oyi.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://rjv.jqgfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://job.jinghuilouyu.cn

JS:   e.message;  e.stack
来源：http://dox.smart0.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://uaw.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://ebp.jlsjyb.cn

Go:   err.Error()
来源：http://zyr.guannengcc.top


<!-- 参考信息 -->