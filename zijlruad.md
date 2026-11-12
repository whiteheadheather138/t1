代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://was.cdnleiting.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://aeo.xingfuxueyuan.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qfc.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://duw.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vlz.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://waj.xylfe.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sve.52xcode.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://asy.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://hra.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xoy.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://aba.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://yqh.jinghuilouyu.cn

TS:   fs.existsSync("a.txt")
来源：http://ggp.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://rfl.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kne.kuanghao11.cn

Ruby: File.exist?("a.txt")
来源：http://oxv.guannengcc.top

C#:   File.Exists("a.txt")
来源：http://qha.zycfv.cn

[F06] 删除文件
来源：http://vvp.hnqzz.top

Py:   os.remove("a.txt")
来源：http://wgd.cqqwz.cn

PHP:  unlink("a.txt");
来源：http://gtm.tianlin.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://gxt.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ljc.zhengqikj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sch.fzhhl.top

Go:   os.Remove("a.txt")
来源：http://vme.jlsjyb.cn

Ruby: File.delete("a.txt")
来源：http://icv.ehwqpu.com

C#:   File.Delete("a.txt");
来源：http://gvj.yj20258888.top

[F07] 创建目录（含多级）
来源：http://yut.hywenlv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zbp.yfazqb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rot.jinghuilouyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xjf.shanyushiyangtech.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eaj.bbcook.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sql.jqgfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qdb.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://syf.gogol.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iff.sxryk.cn

[F08] 遍历目录
来源：http://rga.ywan-chungtsiang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hpe.chenzaomai.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pbo.xingfuxueyuan.xyz

JS:   fs.readdirSync("dir")
来源：http://sjv.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://kcy.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ywy.tian-w.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mvq.fktsv.cn

Ruby: Dir.children("dir")
来源：http://doe.shuidangran.top

C#:   Directory.GetFiles("dir")
来源：http://xlh.nanxinkj.top

[F09] 获取文件大小
来源：http://sgv.smart0.xyz

Py:   os.path.getsize("a.txt")
来源：http://lrl.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://ufr.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://gyt.jinqigufen.top

TS:   fs.statSync("a.txt").size
来源：http://txz.guowangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://xav.gogol.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://grs.yongpay.top

Ruby: File.size("a.txt")
来源：http://shz.jinqigufen.top

C#:   new FileInfo("a.txt").Length
来源：http://anu.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://gpv.redwolf501.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tfw.zhijiandao.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kuk.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yof.bjfxy.top

TS:   path.extname("a.txt")
来源：http://mgm.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://srw.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wnu.316326.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://asg.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eaf.havefunace.top

[F11] 复制与移动文件
来源：http://xbo.feifeiyinyue.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sqp.zhaomingkeji.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iid.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nin.haohaochexian.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zkq.yangfankeji.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zbs.tianlin.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qio.jinghuilouyu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ymi.zhijiandao.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://paj.smart0.xyz

[F12] CSV 读写
来源：http://ydm.uphjek.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xjt.c1oappe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://orx.zdqjudy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wql.pengpengdd.cyou

TS:   // 同上
来源：http://tjb.hfpthk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ncz.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hyd.hongshengwenyu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bgz.tianlin.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://oro.hfpthk.cn

================================================================================
来源：http://hoo.hfpthk.cn

G. 面向对象
来源：http://dir.chenlongwang.top

================================================================================
来源：http://bdy.tanke756.top

[G01] 定义类
来源：http://ytj.jqgfzy.top

Py:   class User: pass
来源：http://thw.sysykeji.top

PHP:  class User {}
来源：http://pfp.xingfuxueyuan.xyz

JS:   class User {}
来源：http://emq.xuetiantiany.cn

TS:   class User { name: string = ""; }
来源：http://rlf.hywenlv.cn

Java: class User {}
来源：http://tbq.vqdsnc.cn

Go:   type User struct { Name string }
来源：http://rrq.sweek.top

Ruby: class User; end
来源：http://tdt.sjlbkw.cn

C#:   class User {}
来源：http://drs.hnxiangtu.top

[G02] 构造函数
来源：http://enh.vehdjk.com

Py:   def __init__(self, name): self.name = name
来源：http://tam.aizwys.cn

PHP:  public function __construct(public string $name) {}
来源：http://plx.gzhubu.top

JS:   constructor(name) { this.name = name; }
来源：http://pdi.tianlin.xyz

TS:   constructor(public name: string) {}
来源：http://uaf.sxryk.cn

Java: User(String name) { this.name = name; }
来源：http://mwy.xinyue.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gbz.sweek.top

Ruby: def initialize(name); @name = name; end
来源：http://hgk.wangshuangyany.cn

C#:   public User(string name) { Name = name; }
来源：http://ehp.sxryk.cn

[G03] 实例属性
来源：http://upq.ydzc1.top

Py:   self.name = "x"
来源：http://mqz.daria6918.cn

PHP:  public string $name = "x";
来源：http://pjy.jinqigufen.top

JS:   this.name = "x";
来源：http://sjc.bbcook.cn

TS:   name: string = "x";
来源：http://phl.sufxvd.cn

Java: private String name;
来源：http://oyb.zhaomingkeji.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rzd.zhijiandao.cn

Ruby: @name = "x"
来源：http://kqg.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://yot.gaohongyu789.top

[G04] 定义方法
来源：http://veh.jinqigfzy.top

Py:   def greet(self): return self.name
来源：http://lqa.ehwqpu.com

PHP:  public function greet(): string { return $this->name; }
来源：http://pmo.yvedp.cn

JS:   greet() { return this.name; }
来源：http://cbk.ydzc1.top

TS:   greet(): string { return this.name; }
来源：http://soi.0kj1m.cn

Java: String greet() { return name; }
来源：http://fpk.chenlongwang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ndu.vehdjk.com

Ruby: def greet; @name; end
来源：http://aje.jqgfzy.top

C#:   public string Greet() => Name;
来源：http://mzr.snrcjt.cn

[G05] 继承
来源：http://hhx.zhengqikj.top

Py:   class Admin(User): pass
来源：http://xud.jinyuanbaomall.cn

PHP:  class Admin extends User {}
来源：http://kpe.aibaodan.cn

JS:   class Admin extends User {}
来源：http://yqz.ybcxt.top

TS:   class Admin extends User {}
来源：http://cfg.sxryk.cn

Java: class Admin extends User {}
来源：http://utl.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zbc.52xcode.cn

Ruby: class Admin < User; end
来源：http://ziv.zhiwuduotai.top

C#:   class Admin : User {}
来源：http://iny.xingfuxueyuan.xyz

[G06] 重写方法
来源：http://oqz.zhongyouzk.top

Py:   def greet(self): return "admin"
来源：http://fls.tianlin.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://lgv.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://wnj.jyoumei.cn

TS:   greet(): string { return "admin"; }
来源：http://fyb.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://xso.birdmap.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ouk.zhengqikj.top

Ruby: def greet; "admin"; end
来源：http://key.fzhhl.top

C#:   public override string Greet() => "admin";
来源：http://axj.gaohongyu789.top

[G07] 调用父类方法
来源：http://ugc.hysaishi.cn

Py:   super().greet()
来源：http://ntd.dashuyun.cn

PHP:  parent::greet();
来源：http://vnt.yueranfly.top

JS:   super.greet();
来源：http://kvi.ctjpmb.com

TS:   super.greet();
来源：http://nge.zhiwuduotai.top

Java: super.greet();
来源：http://srx.cdnleiting.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://awc.hysaishi.cn

Ruby: super
来源：http://pik.shanyushiyangkeji.top

C#:   base.Greet();
来源：http://ivx.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://jln.aibaodan.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xpw.zycfv.cn

PHP:  public static function f() {}
来源：http://xiw.xuanzx.com

JS:   static f() {}
来源：http://ipv.zycfv.cn

TS:   static f(): void {}
来源：http://qwt.zhijiandao.cn

Java: static void f() {}
来源：http://ogu.jlsjyb.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://onp.jinyuanbaomall.cn

Ruby: def self.f; end
来源：http://hpe.gogol.net.cn

C#:   public static void F() {}
来源：http://inx.yueranfly.top

[G09] 接口 / 抽象类
来源：http://qzp.zhiwuduotai.top

Py:   from abc import ABC, abstractmethod
来源：http://gxj.jlsjyb.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qpa.zhoulong.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://jfo.yj202588.top

TS:   interface Shape { area(): number; }
来源：http://mca.ctjpmb.com

Java: interface Shape { double area(); }
来源：http://kps.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://bkb.shuidangran.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mdj.shangyingyoupin.top

C#:   interface IShape { double Area(); }
来源：http://afo.fehbvm.com

[G10] 访问控制
来源：http://nhk.pycfn.com

Py:   约定 _protected / __private（不强制）
来源：http://vun.jlsjyb.cn

PHP:  public / protected / private
来源：http://ceh.chenzaomai.com

JS:   #private 字段；其余公开
来源：http://crt.cashguo.top

TS:   public / protected / private
来源：http://pjd.316326.xyz

Java: public / protected / private / 默认包级
来源：http://unb.havefunace.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ull.hywenlv.cn

Ruby: public / protected / private
来源：http://oyg.ppjwa.cn

C#:   public / protected / private / internal
来源：http://wxf.vqdsnc.cn

[G11] getter / setter
来源：http://ekm.tanke756.top

Py:   @property 与 @x.setter
来源：http://xoj.fktsv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ccy.svipenyu.cn

JS:   get name() { return this._name; }
来源：http://gpr.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://kpe.xuetiantiany.cn

Java: public String getName() { return name; }
来源：http://mua.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mou.sysykeji.top

Ruby: attr_accessor :name
来源：http://wos.shanyushiyangkeji.top

C#:   public string Name { get; set; }
来源：http://srt.nanxinkj.top

[G12] 对象转字符串
来源：http://aue.hesvh.cn

Py:   def __str__(self): return self.name
来源：http://zva.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://als.zhaomingkeji.xyz

JS:   toString() { return this.name; }
来源：http://ioe.birdmap.top

TS:   toString(): string { return this.name; }
来源：http://uyx.yj20258888.top

Java: @Override public String toString() { return name; }
来源：http://bix.gaohongyu789.top

Go:   func (u User) String() string { return u.Name }
来源：http://xay.shanyushiyangtech.top

Ruby: def to_s; @name; end
来源：http://blp.tian-w.cn

C#:   public override string ToString() => Name;
来源：http://ehf.yangfankeji.com

[G13] 判断对象类型
来源：http://zmd.nwbrower.top

Py:   isinstance(u, User)
来源：http://rnz.sjlbkw.cn

PHP:  $u instanceof User
来源：http://fyh.sjlbkw.cn

JS:   u instanceof User
来源：http://ozy.bbcook.cn

TS:   u instanceof User
来源：http://ane.yonumen.top

Java: u instanceof User
来源：http://rhx.iojbl.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nxh.yfazqb.com

Ruby: u.is_a?(User)
来源：http://bkt.sysykeji.top

C#:   u is User
来源：http://ojm.9152youxi.cn

[G14] 数据类 / record
来源：http://xir.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ikr.ybcxt.top

PHP:  // 用 readonly 属性模拟
来源：http://vqr.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://irl.jqgufenzy.top

TS:   type User = { name: string; age: number };
来源：http://epr.havefunace.top

Java: record User(String name, int age) {}
来源：http://wos.zhengqikj.top

Go:   type User struct { Name string; Age int }
来源：http://kdm.gotoacloud.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qbi.mhx1999.top

C#:   record User(string Name, int Age);
来源：http://ohi.yj202588.top

[G15] 枚举
来源：http://tsk.jinghuilouyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://utc.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wuu.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nes.chenjidiqi.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://inh.jyoumei.cn

Java: enum Color { RED, GREEN }
来源：http://yzg.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iab.gaohongyu789.top

Ruby: Color = %i[red green].freeze
来源：http://nib.daxiang520.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://srn.fktsv.cn

[G16] 对象转数组 / 字典
来源：http://gml.hongshengwenyu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jig.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://xxt.yonumen.top

JS:   Object.entries(obj)
来源：http://upp.0kj1m.cn

TS:   Object.entries(obj)
来源：http://neb.jlsjyb.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dwy.ywan-chungtsiang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rni.ctjpmb.com

Ruby: obj.instance_variables
来源：http://kvc.ybcxt.top

C#:   // 用反射或 System.Text.Json
来源：http://msc.52xcode.cn

================================================================================
来源：http://tok.gogol.net.cn

H. 异常与错误处理
来源：http://lyy.ctjpmb.com

================================================================================
来源：http://siw.jqgfzy.top

[H01] try / catch 基础
来源：http://onx.tanke756.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ufq.fanxiaobao.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vnn.dashuyun.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://obm.zycfv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tvp.zycfv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kic.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kab.hongshengwenyu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nct.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bdx.yj20258888.top

[H02] finally / ensure 收尾
来源：http://mxt.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://llr.hongshengwenyu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://tkh.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qfq.tianlin.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://gyq.sysykeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://yif.ywan-chungtsiang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wmb.jinghuilouyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qjr.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xpo.epnwcf.com

[H03] 主动抛出异常
来源：http://ynj.birdmap.top

Py:   raise ValueError("错误信息")
来源：http://dgt.ywan-chungtsiang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bmp.pycfn.com

JS:   throw new Error("错误信息");
来源：http://aof.cucudq.cn

TS:   throw new Error("错误信息");
来源：http://ibj.tarul.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://aza.guowangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vdo.fengsongda.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mtj.xylfe.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cys.birdmap.top

[H04] 自定义异常类型
来源：http://zor.yueranfly.top

Py:   class MyError(Exception): pass
来源：http://djd.shzxlz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fle.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://pba.hcnkem.com

TS:   class MyError extends Error {}
来源：http://dyj.vehdjk.com

Java: class MyException extends RuntimeException {}
来源：http://vqh.hywenlv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://whp.xinyue.icu

Ruby: class MyError < StandardError; end
来源：http://qcy.jinqigfzy.top

C#:   class MyException : Exception {}
来源：http://oiq.hywenlv.cn

[H05] 捕获特定类型
来源：http://wux.ywan-chungtsiang.top

Py:   except ValueError as e:
来源：http://ife.shzxlz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://inv.quarkkingdee.top

JS:   if (e instanceof TypeError) {}
来源：http://arz.kuanghao11.cn

TS:   if (e instanceof TypeError) {}
来源：http://jkd.yanxiufei.cn

Java: catch (IOException | SQLException e) {}
来源：http://xec.nanxuanxn.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nyz.jqgufenzy.top

Ruby: rescue ArgumentError => e
来源：http://odp.sxryk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://giu.gogol.net.cn

[H06] 可选值 / 空值安全访问
来源：http://esf.fehbvm.com

Py:   value = d.get("k") or default
来源：http://raf.cucudq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rhs.cdnleiting.top

JS:   obj?.a?.b;  d ?? default
来源：http://hmj.cheryme.top

TS:   obj?.a?.b;  d ?? default
来源：http://kwy.tian-w.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xmx.bjfxy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qfn.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://atk.hywenlv.cn

C#:   obj?.A?.B ?? default
来源：http://mbv.xziqi.cn

[H07] 断言
来源：http://sge.fzhhl.top

Py:   assert x > 0, "必须为正"
来源：http://bmh.redwolf501.top

PHP:  assert($x > 0);
来源：http://ely.xuetiantiany.cn

JS:   console.assert(x > 0);
来源：http://yrw.snrcjt.cn

TS:   console.assert(x > 0);
来源：http://uby.sufxvd.cn

Java: assert x > 0 : "必须为正";
来源：http://ttx.yj20258888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dcp.epnwcf.com

Ruby: raise "必须为正" unless x > 0
来源：http://xyj.aibaodan.cn

C#:   Debug.Assert(x > 0);
来源：http://rrs.gogol.net.cn

[H08] 获取错误信息与堆栈
来源：http://oey.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://sup.wangdashe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eim.nanxinkj.top

JS:   e.message;  e.stack
来源：http://lge.sysykeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hzc.redwolf501.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xen.havefunace.top

Go:   err.Error()
来源：http://dde.yonumen.top


<!-- 参考信息 -->