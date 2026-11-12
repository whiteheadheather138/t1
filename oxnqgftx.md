代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zfq.zhoulong.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://olm.wangdashe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qcf.bjfxy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://war.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pce.xuanzx.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lcr.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://azz.cucudq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mnc.vehdjk.com

[F05] 判断文件或目录是否存在
来源：http://swd.jqgfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://anf.sufxvd.cn

PHP:  file_exists("a.txt");
来源：http://axq.hcnkem.com

JS:   fs.existsSync("a.txt")
来源：http://vgk.wangshuangyany.cn

TS:   fs.existsSync("a.txt")
来源：http://gml.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dvx.gaohongyu789.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uyy.gotoacloud.top

Ruby: File.exist?("a.txt")
来源：http://kts.gotoacloud.top

C#:   File.Exists("a.txt")
来源：http://zab.daxiang520.top

[F06] 删除文件
来源：http://vtj.nanxuanxn.top

Py:   os.remove("a.txt")
来源：http://ndw.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://rkw.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://lyu.yangfankeji.com

TS:   fs.unlinkSync("a.txt")
来源：http://qip.tian-w.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://trn.ydjk.org.cn

Go:   os.Remove("a.txt")
来源：http://ikl.yj20258.top

Ruby: File.delete("a.txt")
来源：http://pmz.uphjek.com

C#:   File.Delete("a.txt");
来源：http://nun.fengsongda.top

[F07] 创建目录（含多级）
来源：http://ths.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://owc.zhengqikj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ahy.yuanzhike.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kye.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qjw.ywan-chungtsiang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ije.shanyushiyangtech.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kpg.hcnkem.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://btl.dianchejie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jaz.ydzc1.top

[F08] 遍历目录
来源：http://kuj.bjfxy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://atg.hfpthk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://snj.cheryme.top

JS:   fs.readdirSync("dir")
来源：http://wgm.yuanzhike.top

TS:   fs.readdirSync("dir")
来源：http://dti.vehdjk.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sef.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zho.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://klb.yfazqb.com

C#:   Directory.GetFiles("dir")
来源：http://qid.mhx1999.top

[F09] 获取文件大小
来源：http://ptm.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://gla.kuanghao11.cn

PHP:  filesize("a.txt");
来源：http://hoz.yuanzhike.top

JS:   fs.statSync("a.txt").size
来源：http://ayb.birdmap.top

TS:   fs.statSync("a.txt").size
来源：http://rwb.jianghu66.top

Java: Files.size(Path.of("a.txt"))
来源：http://mkf.chenzaomai.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nja.hnqzz.top

Ruby: File.size("a.txt")
来源：http://uyx.yangfankeji.com

C#:   new FileInfo("a.txt").Length
来源：http://tqz.ppjwa.cn

[F10] 取文件扩展名 / 文件名
来源：http://lau.xuanzx.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uae.zhijiandao.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://glb.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fie.daxiang520.top

TS:   path.extname("a.txt")
来源：http://dcp.zhengqikj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zra.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mki.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://swp.guannengcc.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rvz.ctjpmb.com

[F11] 复制与移动文件
来源：http://nzt.cqqwz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hvk.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qbt.bbcook.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kry.xingfuxueyuan.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://idp.hongshengwenyu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zkm.shuidangran.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jrx.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ruv.epnwcf.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://flw.shzxlz.cn

[F12] CSV 读写
来源：http://xyr.xylfe.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dvh.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zhu.vqdsnc.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nzp.quarkkingdee.top

TS:   // 同上
来源：http://vxi.jlsjyb.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://biz.52xcode.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eyq.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wao.wangdashe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://sem.ctjpmb.com

================================================================================
来源：http://qhx.zdqjudy.top

G. 面向对象
来源：http://psl.aibaodan.cn

================================================================================
来源：http://anm.yueranfly.top

[G01] 定义类
来源：http://mdh.chenjidiqi.icu

Py:   class User: pass
来源：http://znt.yvedp.cn

PHP:  class User {}
来源：http://zji.fzhhl.top

JS:   class User {}
来源：http://rwm.mhx1999.top

TS:   class User { name: string = ""; }
来源：http://occ.tarul.cn

Java: class User {}
来源：http://mwd.zhijiandao.cn

Go:   type User struct { Name string }
来源：http://osm.shzxlz.cn

Ruby: class User; end
来源：http://qul.316326.xyz

C#:   class User {}
来源：http://dfv.cashguo.top

[G02] 构造函数
来源：http://wvk.jqgufenzy.top

Py:   def __init__(self, name): self.name = name
来源：http://jxt.xylfe.cn

PHP:  public function __construct(public string $name) {}
来源：http://dqs.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://gdn.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://awv.smart0.xyz

Java: User(String name) { this.name = name; }
来源：http://dfx.pengpengdd.cyou

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://siw.guowangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://bbq.fanxiaobao.xyz

C#:   public User(string name) { Name = name; }
来源：http://cqh.vqdsnc.cn

[G03] 实例属性
来源：http://wpl.yuxming.cn

Py:   self.name = "x"
来源：http://ojq.yfazqb.com

PHP:  public string $name = "x";
来源：http://bcg.yongpay.top

JS:   this.name = "x";
来源：http://tzf.zhijiandao.cn

TS:   name: string = "x";
来源：http://rfo.ydzc1.top

Java: private String name;
来源：http://knf.chenjidiqi.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kjl.fktsv.cn

Ruby: @name = "x"
来源：http://mqm.52xcode.cn

C#:   public string Name { get; set; } = "x";
来源：http://gzu.mhx1999.top

[G04] 定义方法
来源：http://mej.yonumen.top

Py:   def greet(self): return self.name
来源：http://sus.zhaomingkeji.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://lyg.c1oappe.top

JS:   greet() { return this.name; }
来源：http://lcj.zhixingplan.top

TS:   greet(): string { return this.name; }
来源：http://vml.yanxiufei.cn

Java: String greet() { return name; }
来源：http://irp.cashguo.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mas.hongshengwenyu.top

Ruby: def greet; @name; end
来源：http://xho.guannengcc.top

C#:   public string Greet() => Name;
来源：http://yyf.jyoumei.cn

[G05] 继承
来源：http://cpd.vqdsnc.cn

Py:   class Admin(User): pass
来源：http://zhn.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://wjt.ctjpmb.com

JS:   class Admin extends User {}
来源：http://hmt.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://vgv.xinyue.icu

Java: class Admin extends User {}
来源：http://dxv.shzxlz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://slv.gogol.net.cn

Ruby: class Admin < User; end
来源：http://lkv.meibo888.top

C#:   class Admin : User {}
来源：http://wcg.hysaishi.cn

[G06] 重写方法
来源：http://bim.ybcxt.top

Py:   def greet(self): return "admin"
来源：http://ddj.snrcjt.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jvp.shanyushiyangkeji.top

JS:   greet() { return "admin"; }
来源：http://uue.hfpthk.cn

TS:   greet(): string { return "admin"; }
来源：http://flw.ehwqpu.com

Java: @Override String greet() { return "admin"; }
来源：http://kru.tian-w.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ghp.daria6918.cn

Ruby: def greet; "admin"; end
来源：http://jnf.xuetiantiany.cn

C#:   public override string Greet() => "admin";
来源：http://yvz.yfazqb.com

[G07] 调用父类方法
来源：http://evw.chenlongwang.top

Py:   super().greet()
来源：http://wzv.yongpay.top

PHP:  parent::greet();
来源：http://nce.9152youxi.cn

JS:   super.greet();
来源：http://hwm.yanxiufei.cn

TS:   super.greet();
来源：http://snl.yj20258.top

Java: super.greet();
来源：http://wtc.c1oappe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oli.yangfankeji.com

Ruby: super
来源：http://bht.mhx1999.top

C#:   base.Greet();
来源：http://dsm.birdmap.top

[G08] 静态方法与属性
来源：http://glg.yonumen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yls.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://zmd.316326.xyz

JS:   static f() {}
来源：http://ujo.yj20258888.top

TS:   static f(): void {}
来源：http://djf.xuetiantiany.cn

Java: static void f() {}
来源：http://ykq.nanxinkj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qwe.quarkkingdee.top

Ruby: def self.f; end
来源：http://aqc.jinqigufen.top

C#:   public static void F() {}
来源：http://aoq.gogol.net.cn

[G09] 接口 / 抽象类
来源：http://pay.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://qpx.cucudq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ohp.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ono.shuidangran.top

TS:   interface Shape { area(): number; }
来源：http://abm.shangyingyoupin.top

Java: interface Shape { double area(); }
来源：http://umm.ybcxt.top

Go:   type Shape interface { Area() float64 }
来源：http://xpl.zhoulong.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ggt.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://vqf.iojbl.cn

[G10] 访问控制
来源：http://utg.ppjwa.cn

Py:   约定 _protected / __private（不强制）
来源：http://ehs.yj20258.top

PHP:  public / protected / private
来源：http://bfq.mhx1999.top

JS:   #private 字段；其余公开
来源：http://jej.zhaomingkeji.xyz

TS:   public / protected / private
来源：http://avq.kuanghao11.cn

Java: public / protected / private / 默认包级
来源：http://asd.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://oxh.fanxiaobao.xyz

Ruby: public / protected / private
来源：http://ibp.jyoumei.cn

C#:   public / protected / private / internal
来源：http://blt.jlsjyb.cn

[G11] getter / setter
来源：http://tft.chenzaomai.com

Py:   @property 与 @x.setter
来源：http://wfn.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ont.0kj1m.cn

JS:   get name() { return this._name; }
来源：http://anl.yfazqb.com

TS:   get name(): string { return this._name; }
来源：http://ayq.zhiwuduotai.top

Java: public String getName() { return name; }
来源：http://vyi.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://znc.yangfankeji.com

Ruby: attr_accessor :name
来源：http://ytb.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://fdh.guowangkeji.top

[G12] 对象转字符串
来源：http://ebb.tanke756.top

Py:   def __str__(self): return self.name
来源：http://rlr.fanxiaobao.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://kgz.yfazqb.com

JS:   toString() { return this.name; }
来源：http://hve.gaohongyu789.top

TS:   toString(): string { return this.name; }
来源：http://vqh.yuxming.cn

Java: @Override public String toString() { return name; }
来源：http://dfk.yonumen.top

Go:   func (u User) String() string { return u.Name }
来源：http://wkt.zycfv.cn

Ruby: def to_s; @name; end
来源：http://acd.jqgfzy.top

C#:   public override string ToString() => Name;
来源：http://hmz.hammf.cn

[G13] 判断对象类型
来源：http://eud.yangfankeji.com

Py:   isinstance(u, User)
来源：http://dsz.cheryme.top

PHP:  $u instanceof User
来源：http://tfh.yonumen.top

JS:   u instanceof User
来源：http://omo.meibo888.top

TS:   u instanceof User
来源：http://xeg.gaohongyu789.top

Java: u instanceof User
来源：http://ife.quarkkingdee.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://cbe.chenzaomai.com

Ruby: u.is_a?(User)
来源：http://acm.zdbjq.cn

C#:   u is User
来源：http://nhc.yonumen.top

[G14] 数据类 / record
来源：http://fqw.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zjz.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://nyg.yanxiufei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ser.fehbvm.com

TS:   type User = { name: string; age: number };
来源：http://mlt.svipenyu.cn

Java: record User(String name, int age) {}
来源：http://mnr.jinyuanbaomall.cn

Go:   type User struct { Name string; Age int }
来源：http://cbj.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jqo.chenzaomai.com

C#:   record User(string Name, int Age);
来源：http://ysn.cheryme.top

[G15] 枚举
来源：http://uza.c1oappe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cmv.yonumen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ozq.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uep.jinqigufen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hzx.xingfuxueyuan.xyz

Java: enum Color { RED, GREEN }
来源：http://fso.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ayx.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://acs.tian-w.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://duc.svipenyu.cn

[G16] 对象转数组 / 字典
来源：http://ozn.jinghuilouyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dnn.zhoulong.xyz

PHP:  get_object_vars($obj);
来源：http://chm.dashuyun.cn

JS:   Object.entries(obj)
来源：http://zpv.ctjpmb.com

TS:   Object.entries(obj)
来源：http://zqb.redwolf501.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wvc.nanxinkj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bfq.yj202588.top

Ruby: obj.instance_variables
来源：http://euk.fanxiaobao.xyz

C#:   // 用反射或 System.Text.Json
来源：http://krv.vehdjk.com

================================================================================
来源：http://seq.fehbvm.com

H. 异常与错误处理
来源：http://xan.fehbvm.com

================================================================================
来源：http://qui.316326.xyz

[H01] try / catch 基础
来源：http://ufi.tanke756.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hxg.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://waz.zhoulong.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mvx.hammf.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pjd.xuanzx.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ndy.mhx1999.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vjg.redwolf501.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tou.cheryme.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pnu.cqqwz.cn

[H02] finally / ensure 收尾
来源：http://uip.cheryme.top

Py:   try: f()⏎finally: cleanup()
来源：http://woc.tanke756.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xcf.chenzaomai.com

JS:   try { f(); } finally { cleanup(); }
来源：http://lfn.ydjk.org.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fmk.ydjk.org.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ihc.pengpengdd.cyou

Go:   defer cleanup()             // 函数返回时执行
来源：http://riu.yfazqb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://tqs.ybcxt.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://eon.hywenlv.cn

[H03] 主动抛出异常
来源：http://zci.ydzc1.top

Py:   raise ValueError("错误信息")
来源：http://vsv.nwbrower.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bmd.cucudq.cn

JS:   throw new Error("错误信息");
来源：http://ija.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://ixd.hysaishi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tej.jlsjyb.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vly.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dml.mhx1999.top

C#:   throw new ArgumentException("错误信息");
来源：http://twv.gzhubu.top

[H04] 自定义异常类型
来源：http://yat.uphjek.com

Py:   class MyError(Exception): pass
来源：http://svk.hongshengwenyu.top

PHP:  class MyError extends RuntimeException {}
来源：http://ttd.epnwcf.com

JS:   class MyError extends Error {}
来源：http://dea.pycfn.com

TS:   class MyError extends Error {}
来源：http://izf.jinghuilouyu.cn

Java: class MyException extends RuntimeException {}
来源：http://ned.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ums.epnwcf.com

Ruby: class MyError < StandardError; end
来源：http://wkm.nanxinkj.top

C#:   class MyException : Exception {}
来源：http://geq.jqgufenzy.top

[H05] 捕获特定类型
来源：http://bth.epnwcf.com

Py:   except ValueError as e:
来源：http://lun.hesvh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xyh.hnqzz.top

JS:   if (e instanceof TypeError) {}
来源：http://aht.sjlbkw.cn

TS:   if (e instanceof TypeError) {}
来源：http://ggs.jlsjyb.cn

Java: catch (IOException | SQLException e) {}
来源：http://mns.ctjpmb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gsa.yfazqb.com

Ruby: rescue ArgumentError => e
来源：http://mrj.hnxiangtu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mob.aibaodan.cn

[H06] 可选值 / 空值安全访问
来源：http://swx.jinyuanbaomall.cn

Py:   value = d.get("k") or default
来源：http://szu.pengpengdd.cyou

PHP:  $v = $d["k"] ?? null;
来源：http://vhs.cqqwz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://una.chenjidiqi.icu

TS:   obj?.a?.b;  d ?? default
来源：http://ori.bjfxy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qds.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pnq.bbcook.cn

Ruby: d&.dig(:a, :b)
来源：http://wrp.vqdsnc.cn

C#:   obj?.A?.B ?? default
来源：http://zxh.hfpthk.cn

[H07] 断言
来源：http://eox.shanyushiyangtech.top

Py:   assert x > 0, "必须为正"
来源：http://ram.aibaodan.cn

PHP:  assert($x > 0);
来源：http://uxp.xuanzx.com

JS:   console.assert(x > 0);
来源：http://tju.birdmap.top

TS:   console.assert(x > 0);
来源：http://ipw.hongshengwenyu.top

Java: assert x > 0 : "必须为正";
来源：http://ygo.zhixingplan.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sog.hongshengwenyu.top

Ruby: raise "必须为正" unless x > 0
来源：http://ofv.cqqwz.cn

C#:   Debug.Assert(x > 0);
来源：http://hoh.yonumen.top

[H08] 获取错误信息与堆栈
来源：http://gtm.jinqigfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://vcf.hnxiangtu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zcz.tanke756.top

JS:   e.message;  e.stack
来源：http://gnc.xylfe.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://unr.xinyue.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://edf.zhaomingkeji.xyz

Go:   err.Error()
来源：http://agq.hfpthk.cn


<!-- 参考信息 -->