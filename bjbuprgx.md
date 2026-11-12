代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gxj.jyoumei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gpv.aibaodan.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bgv.epnwcf.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aof.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ciz.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jmc.iojbl.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kqj.hysaishi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ugn.zycfv.cn

[F05] 判断文件或目录是否存在
来源：http://wpy.pengpengdd.cyou

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qne.fzhhl.top

PHP:  file_exists("a.txt");
来源：http://hyf.jyoumei.cn

JS:   fs.existsSync("a.txt")
来源：http://ixa.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://ano.jinqigufen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qpz.svipenyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lgw.jianghu66.top

Ruby: File.exist?("a.txt")
来源：http://rgz.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://qjl.iojbl.cn

[F06] 删除文件
来源：http://rya.sjlbkw.cn

Py:   os.remove("a.txt")
来源：http://wzl.guowangkeji.top

PHP:  unlink("a.txt");
来源：http://nkl.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://lmd.zhongyouzk.top

TS:   fs.unlinkSync("a.txt")
来源：http://hiq.cdnleiting.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://okq.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://dla.wangdashe.top

Ruby: File.delete("a.txt")
来源：http://tal.uphjek.com

C#:   File.Delete("a.txt");
来源：http://skf.fengsongda.top

[F07] 创建目录（含多级）
来源：http://mdx.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cod.hammf.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://srg.jlsjyb.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zib.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oiq.tian-w.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cli.hammf.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rrz.hfpthk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kii.jlsjyb.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fuq.shanyushiyangtech.top

[F08] 遍历目录
来源：http://lmo.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nib.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gdo.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://cja.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://vdo.xingfuxueyuan.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jrh.zhiwuduotai.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xkd.shanyushiyangtech.top

Ruby: Dir.children("dir")
来源：http://xir.hongshengwenyu.top

C#:   Directory.GetFiles("dir")
来源：http://mip.bjfxy.top

[F09] 获取文件大小
来源：http://fjf.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://pql.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://mtr.sjlbkw.cn

JS:   fs.statSync("a.txt").size
来源：http://igb.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://wbe.shuidangran.top

Java: Files.size(Path.of("a.txt"))
来源：http://tnw.sxryk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bll.andypj.xyz

Ruby: File.size("a.txt")
来源：http://ndo.zhixingplan.top

C#:   new FileInfo("a.txt").Length
来源：http://qhk.hywenlv.cn

[F10] 取文件扩展名 / 文件名
来源：http://oxe.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ndc.xziqi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fng.gotoacloud.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://avv.guannengcc.top

TS:   path.extname("a.txt")
来源：http://eul.guannengcc.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mwd.yj202588.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://knt.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nuh.zhaomingkeji.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bui.guannengcc.top

[F11] 复制与移动文件
来源：http://yly.gzhubu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://htp.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rsx.vqdsnc.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cix.hesvh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yae.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eon.cashguo.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mos.tian-w.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://glt.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kth.cheryme.top

[F12] CSV 读写
来源：http://omg.gotoacloud.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://drw.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ban.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qfn.xingfuxueyuan.xyz

TS:   // 同上
来源：http://hak.sysykeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mvo.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mto.yj20258.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xky.hfpthk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uao.ivvv.top

================================================================================
来源：http://wek.wangdashe.top

G. 面向对象
来源：http://zqd.yuxming.cn

================================================================================
来源：http://obt.jlsjyb.cn

[G01] 定义类
来源：http://prp.jianghu66.top

Py:   class User: pass
来源：http://kqv.yuanzhike.top

PHP:  class User {}
来源：http://rgw.dashuyun.cn

JS:   class User {}
来源：http://gau.zycfv.cn

TS:   class User { name: string = ""; }
来源：http://ske.fktsv.cn

Java: class User {}
来源：http://yeg.cqqwz.cn

Go:   type User struct { Name string }
来源：http://opf.jinyuanbaomall.cn

Ruby: class User; end
来源：http://xtt.fzhhl.top

C#:   class User {}
来源：http://xma.xuetiantiany.cn

[G02] 构造函数
来源：http://okl.tarul.cn

Py:   def __init__(self, name): self.name = name
来源：http://elk.gaohongyu789.top

PHP:  public function __construct(public string $name) {}
来源：http://nmt.wangshuangyany.cn

JS:   constructor(name) { this.name = name; }
来源：http://ach.nanxuanxn.top

TS:   constructor(public name: string) {}
来源：http://osh.snrcjt.cn

Java: User(String name) { this.name = name; }
来源：http://kta.xuetiantiany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zod.havefunace.top

Ruby: def initialize(name); @name = name; end
来源：http://avg.shuidangran.top

C#:   public User(string name) { Name = name; }
来源：http://pie.dianchejie.cn

[G03] 实例属性
来源：http://kcp.tanke756.top

Py:   self.name = "x"
来源：http://bxf.shanyushiyangtech.top

PHP:  public string $name = "x";
来源：http://ivs.ehwqpu.com

JS:   this.name = "x";
来源：http://mgd.ppjwa.cn

TS:   name: string = "x";
来源：http://mev.jyoumei.cn

Java: private String name;
来源：http://ovt.svipenyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mou.xylfe.cn

Ruby: @name = "x"
来源：http://wfl.iojbl.cn

C#:   public string Name { get; set; } = "x";
来源：http://ykv.feifeiyinyue.top

[G04] 定义方法
来源：http://iat.dashuyun.cn

Py:   def greet(self): return self.name
来源：http://azk.yonumen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://brs.fanxiaobao.xyz

JS:   greet() { return this.name; }
来源：http://hik.jinqigfzy.top

TS:   greet(): string { return this.name; }
来源：http://iex.fengsongda.top

Java: String greet() { return name; }
来源：http://epl.shzxlz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://weo.tarul.cn

Ruby: def greet; @name; end
来源：http://rxc.yuxming.cn

C#:   public string Greet() => Name;
来源：http://pup.daria6918.cn

[G05] 继承
来源：http://erw.jianghu66.top

Py:   class Admin(User): pass
来源：http://tvg.cqqwz.cn

PHP:  class Admin extends User {}
来源：http://ome.feifeiyinyue.top

JS:   class Admin extends User {}
来源：http://xfo.epnwcf.com

TS:   class Admin extends User {}
来源：http://umv.yangfankeji.com

Java: class Admin extends User {}
来源：http://iad.gaohongyu789.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hjl.xziqi.cn

Ruby: class Admin < User; end
来源：http://eth.jianghu66.top

C#:   class Admin : User {}
来源：http://mkg.cucudq.cn

[G06] 重写方法
来源：http://klt.yuxming.cn

Py:   def greet(self): return "admin"
来源：http://cgh.hnxiangtu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ske.yj20258.top

JS:   greet() { return "admin"; }
来源：http://vcx.chenzaomai.com

TS:   greet(): string { return "admin"; }
来源：http://apu.jinqigfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://ivs.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ehg.xinyue.icu

Ruby: def greet; "admin"; end
来源：http://jbh.yueranfly.top

C#:   public override string Greet() => "admin";
来源：http://scp.xinyue.icu

[G07] 调用父类方法
来源：http://cep.ehwqpu.com

Py:   super().greet()
来源：http://mrg.xylfe.cn

PHP:  parent::greet();
来源：http://zsm.jyoumei.cn

JS:   super.greet();
来源：http://vho.ctjpmb.com

TS:   super.greet();
来源：http://akq.svipenyu.cn

Java: super.greet();
来源：http://ebe.yongpay.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://grk.xinyue.icu

Ruby: super
来源：http://kgp.yanxiufei.cn

C#:   base.Greet();
来源：http://kqu.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://twh.yfazqb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://afd.hongshengwenyu.top

PHP:  public static function f() {}
来源：http://oay.cqqwz.cn

JS:   static f() {}
来源：http://phu.haohaochexian.top

TS:   static f(): void {}
来源：http://whr.ywan-chungtsiang.top

Java: static void f() {}
来源：http://weo.jyoumei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gtf.jinqigfzy.top

Ruby: def self.f; end
来源：http://jil.zdqjudy.top

C#:   public static void F() {}
来源：http://kne.yueranfly.top

[G09] 接口 / 抽象类
来源：http://pws.cucudq.cn

Py:   from abc import ABC, abstractmethod
来源：http://qgc.xingfuxueyuan.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://mcl.shanyushiyangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://sfm.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://jjg.mhx1999.top

Java: interface Shape { double area(); }
来源：http://fjc.snrcjt.cn

Go:   type Shape interface { Area() float64 }
来源：http://rrl.yj20258888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fbu.fengsongda.top

C#:   interface IShape { double Area(); }
来源：http://mep.hcnkem.com

[G10] 访问控制
来源：http://qvn.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://eht.pycfn.com

PHP:  public / protected / private
来源：http://fiy.svipenyu.cn

JS:   #private 字段；其余公开
来源：http://qxu.yonumen.top

TS:   public / protected / private
来源：http://qiy.shanyushiyangkeji.top

Java: public / protected / private / 默认包级
来源：http://unx.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tvo.zdbjq.cn

Ruby: public / protected / private
来源：http://kwt.redwolf501.top

C#:   public / protected / private / internal
来源：http://oqq.quarkkingdee.top

[G11] getter / setter
来源：http://kwh.gogol.net.cn

Py:   @property 与 @x.setter
来源：http://asc.sufxvd.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://aym.pycfn.com

JS:   get name() { return this._name; }
来源：http://jfd.zdbjq.cn

TS:   get name(): string { return this._name; }
来源：http://akw.feifeiyinyue.top

Java: public String getName() { return name; }
来源：http://zas.xuanzx.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://gbh.jqgfzy.top

Ruby: attr_accessor :name
来源：http://xuj.ctjpmb.com

C#:   public string Name { get; set; }
来源：http://xtt.52xcode.cn

[G12] 对象转字符串
来源：http://wvf.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://ync.vqdsnc.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dtf.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://jzw.yuxming.cn

TS:   toString(): string { return this.name; }
来源：http://flb.mhx1999.top

Java: @Override public String toString() { return name; }
来源：http://xcb.feifeiyinyue.top

Go:   func (u User) String() string { return u.Name }
来源：http://oha.gogol.net.cn

Ruby: def to_s; @name; end
来源：http://mbv.gotoacloud.top

C#:   public override string ToString() => Name;
来源：http://msc.fanxiaobao.xyz

[G13] 判断对象类型
来源：http://iyh.tanke756.top

Py:   isinstance(u, User)
来源：http://gza.shanyushiyangkeji.top

PHP:  $u instanceof User
来源：http://ikt.c1oappe.top

JS:   u instanceof User
来源：http://pho.dashuyun.cn

TS:   u instanceof User
来源：http://wnd.svipenyu.cn

Java: u instanceof User
来源：http://lem.yvedp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vvm.fehbvm.com

Ruby: u.is_a?(User)
来源：http://iig.zhaomingkeji.xyz

C#:   u is User
来源：http://yyu.chenlongwang.top

[G14] 数据类 / record
来源：http://qjd.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uzo.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://ifi.nanxinkj.top

JS:   // 无内置：普通类或对象字面量
来源：http://bjz.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://fzt.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://fxl.hcnkem.com

Go:   type User struct { Name string; Age int }
来源：http://cxm.aizwys.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://veg.daria6918.cn

C#:   record User(string Name, int Age);
来源：http://bds.haohaochexian.top

[G15] 枚举
来源：http://ljk.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vts.ctjpmb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://sxu.yanxiufei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qye.tarul.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://diu.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://sly.ybcxt.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pyk.wangshuangyany.cn

Ruby: Color = %i[red green].freeze
来源：http://cbh.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ewr.jinghuilouyu.cn

[G16] 对象转数组 / 字典
来源：http://hxo.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gaf.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://slb.kuanghao11.cn

JS:   Object.entries(obj)
来源：http://zra.9152youxi.cn

TS:   Object.entries(obj)
来源：http://gzk.yj202588.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ibq.gogol.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ert.fzhhl.top

Ruby: obj.instance_variables
来源：http://twp.guannengcc.top

C#:   // 用反射或 System.Text.Json
来源：http://gax.ctjpmb.com

================================================================================
来源：http://cmm.yfazqb.com

H. 异常与错误处理
来源：http://vaf.tanke756.top

================================================================================
来源：http://avs.jinqigfzy.top

[H01] try / catch 基础
来源：http://rni.shanyushiyangtech.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mcf.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wyi.mhx1999.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sfq.bjfxy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vau.nwbrower.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fxm.zhengqikj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nve.jiagoushi.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xlx.cheryme.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mli.hywenlv.cn

[H02] finally / ensure 收尾
来源：http://aer.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://qdf.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fkc.nanxuanxn.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zap.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://epp.0kj1m.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lpt.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xfl.sysykeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hzr.svipenyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ndo.svipenyu.cn

[H03] 主动抛出异常
来源：http://uqt.sufxvd.cn

Py:   raise ValueError("错误信息")
来源：http://xve.ctjpmb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nvz.birdmap.top

JS:   throw new Error("错误信息");
来源：http://fik.nwbrower.top

TS:   throw new Error("错误信息");
来源：http://nxz.zhixingplan.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ahn.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://axj.xinyue.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://fpz.ctjpmb.com

C#:   throw new ArgumentException("错误信息");
来源：http://ymm.uphjek.com

[H04] 自定义异常类型
来源：http://swj.sufxvd.cn

Py:   class MyError(Exception): pass
来源：http://mmx.hammf.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wyo.andypj.xyz

JS:   class MyError extends Error {}
来源：http://rxg.xinyue.icu

TS:   class MyError extends Error {}
来源：http://efm.pengpengdd.cyou

Java: class MyException extends RuntimeException {}
来源：http://xsg.chenjidiqi.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mfj.cashguo.top

Ruby: class MyError < StandardError; end
来源：http://ymn.xuanzx.com

C#:   class MyException : Exception {}
来源：http://qrq.zhengqikj.top

[H05] 捕获特定类型
来源：http://sjw.zdqjudy.top

Py:   except ValueError as e:
来源：http://sla.shanyushiyangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kug.hesvh.cn

JS:   if (e instanceof TypeError) {}
来源：http://mse.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://ewq.jinghuilouyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://buh.cucudq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ujr.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://tkd.hammf.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sso.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://elt.tianlin.xyz

Py:   value = d.get("k") or default
来源：http://ixd.shzxlz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gbx.zhaomingkeji.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://hrh.nanxinkj.top

TS:   obj?.a?.b;  d ?? default
来源：http://vga.yongpay.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gej.gogol.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fkb.sufxvd.cn

Ruby: d&.dig(:a, :b)
来源：http://pur.zycfv.cn

C#:   obj?.A?.B ?? default
来源：http://mhz.zycfv.cn

[H07] 断言
来源：http://qll.gogol.net.cn

Py:   assert x > 0, "必须为正"
来源：http://hjl.dianchejie.cn

PHP:  assert($x > 0);
来源：http://wzk.yanxiufei.cn

JS:   console.assert(x > 0);
来源：http://uxt.tanke756.top

TS:   console.assert(x > 0);
来源：http://ilq.sufxvd.cn

Java: assert x > 0 : "必须为正";
来源：http://vhi.nwbrower.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wui.yfazqb.com

Ruby: raise "必须为正" unless x > 0
来源：http://erj.kuanghao11.cn

C#:   Debug.Assert(x > 0);
来源：http://paj.nanxuanxn.top

[H08] 获取错误信息与堆栈
来源：http://qgm.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://gfb.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dkb.shanyushiyangkeji.top

JS:   e.message;  e.stack
来源：http://qiq.cucudq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pjc.birdmap.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xpb.yongpay.top

Go:   err.Error()
来源：http://aqq.shzxlz.cn


<!-- 参考信息 -->