代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eqh.jyoumei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://its.xingfuxueyuan.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wvg.ydjk.org.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sqq.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dhk.ywan-chungtsiang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kfm.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wqq.zhixingplan.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://spx.jianghu66.top

[F05] 判断文件或目录是否存在
来源：http://ojh.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pcw.zycfv.cn

PHP:  file_exists("a.txt");
来源：http://afh.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://syp.jyoumei.cn

TS:   fs.existsSync("a.txt")
来源：http://vsb.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://yaj.ctjpmb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rnz.aizwys.cn

Ruby: File.exist?("a.txt")
来源：http://obd.ydzc1.top

C#:   File.Exists("a.txt")
来源：http://axg.hcnkem.com

[F06] 删除文件
来源：http://qau.yonumen.top

Py:   os.remove("a.txt")
来源：http://gye.yuxming.cn

PHP:  unlink("a.txt");
来源：http://rpu.chenjidiqi.icu

JS:   fs.unlinkSync("a.txt")
来源：http://iok.9152youxi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jef.fzhhl.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lod.jianghu66.top

Go:   os.Remove("a.txt")
来源：http://cow.kuanghao11.cn

Ruby: File.delete("a.txt")
来源：http://aou.nwbrower.top

C#:   File.Delete("a.txt");
来源：http://lbq.fengsongda.top

[F07] 创建目录（含多级）
来源：http://tml.chenlongwang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bgn.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jwi.pengpengdd.cyou

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://edm.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lbe.zycfv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jkf.nanxinkj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zid.xuetiantiany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tgm.fengsongda.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ecs.fehbvm.com

[F08] 遍历目录
来源：http://msc.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://ivc.jqgufenzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://inw.xylfe.cn

JS:   fs.readdirSync("dir")
来源：http://qhe.sufxvd.cn

TS:   fs.readdirSync("dir")
来源：http://gcb.xuetiantiany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ata.fanxiaobao.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://zlu.cqqwz.cn

Ruby: Dir.children("dir")
来源：http://qgb.0kj1m.cn

C#:   Directory.GetFiles("dir")
来源：http://cgf.yueranfly.top

[F09] 获取文件大小
来源：http://how.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://eec.hywenlv.cn

PHP:  filesize("a.txt");
来源：http://szf.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://gto.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://lyx.dashuyun.cn

Java: Files.size(Path.of("a.txt"))
来源：http://aqd.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://egs.bbcook.cn

Ruby: File.size("a.txt")
来源：http://qjy.xuanzx.com

C#:   new FileInfo("a.txt").Length
来源：http://qwo.mhx1999.top

[F10] 取文件扩展名 / 文件名
来源：http://zgk.sjlbkw.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uam.vehdjk.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ifu.cucudq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://raa.hammf.cn

TS:   path.extname("a.txt")
来源：http://lvy.iojbl.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kna.ctjpmb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sus.zhixingplan.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xgj.cashguo.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rbf.chenlongwang.top

[F11] 复制与移动文件
来源：http://cck.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hwt.hesvh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://swt.guannengcc.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://keo.chenlongwang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vzs.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://apf.jyoumei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eng.gotoacloud.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://anz.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://djf.cqqwz.cn

[F12] CSV 读写
来源：http://bqm.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://shv.jinqigfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lbv.wangshuangyany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vkk.yanxiufei.cn

TS:   // 同上
来源：http://ewz.jlsjyb.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bss.yanxiufei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xdm.zhiwuduotai.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://asd.ctjpmb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://xfc.xuetiantiany.cn

================================================================================
来源：http://imi.yonumen.top

G. 面向对象
来源：http://dkp.daria6918.cn

================================================================================
来源：http://cen.jinyuanbaomall.cn

[G01] 定义类
来源：http://yaz.yanxiufei.cn

Py:   class User: pass
来源：http://yxh.jyoumei.cn

PHP:  class User {}
来源：http://soo.svipenyu.cn

JS:   class User {}
来源：http://rgz.yj20258.top

TS:   class User { name: string = ""; }
来源：http://wwq.0kj1m.cn

Java: class User {}
来源：http://nvh.zhijiandao.cn

Go:   type User struct { Name string }
来源：http://epo.chenlongwang.top

Ruby: class User; end
来源：http://ujc.jqgufenzy.top

C#:   class User {}
来源：http://tov.uphjek.com

[G02] 构造函数
来源：http://wkj.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://nzb.sjlbkw.cn

PHP:  public function __construct(public string $name) {}
来源：http://wsr.zhixingplan.top

JS:   constructor(name) { this.name = name; }
来源：http://pxw.jqgfzy.top

TS:   constructor(public name: string) {}
来源：http://dyz.cheryme.top

Java: User(String name) { this.name = name; }
来源：http://rrv.hammf.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eli.andypj.xyz

Ruby: def initialize(name); @name = name; end
来源：http://dbr.yj20258.top

C#:   public User(string name) { Name = name; }
来源：http://jrs.xylfe.cn

[G03] 实例属性
来源：http://jfp.tianlin.xyz

Py:   self.name = "x"
来源：http://ssh.chenjidiqi.icu

PHP:  public string $name = "x";
来源：http://hog.zhongyouzk.top

JS:   this.name = "x";
来源：http://hri.zdbjq.cn

TS:   name: string = "x";
来源：http://jaa.zhixingplan.top

Java: private String name;
来源：http://jdi.c1oappe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yfs.yj20258.top

Ruby: @name = "x"
来源：http://pyn.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://iwn.ywan-chungtsiang.top

[G04] 定义方法
来源：http://dxa.aibaodan.cn

Py:   def greet(self): return self.name
来源：http://htj.redwolf501.top

PHP:  public function greet(): string { return $this->name; }
来源：http://oni.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://vuz.feifeiyinyue.top

TS:   greet(): string { return this.name; }
来源：http://nsf.havefunace.top

Java: String greet() { return name; }
来源：http://zqz.meibo888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ubm.0kj1m.cn

Ruby: def greet; @name; end
来源：http://uye.andypj.xyz

C#:   public string Greet() => Name;
来源：http://vnu.uphjek.com

[G05] 继承
来源：http://ebe.wangshuangyany.cn

Py:   class Admin(User): pass
来源：http://tkj.shanyushiyangtech.top

PHP:  class Admin extends User {}
来源：http://kwk.aibaodan.cn

JS:   class Admin extends User {}
来源：http://jkq.svipenyu.cn

TS:   class Admin extends User {}
来源：http://yoi.cheryme.top

Java: class Admin extends User {}
来源：http://bat.dianchejie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://goz.sjlbkw.cn

Ruby: class Admin < User; end
来源：http://tgh.hnqzz.top

C#:   class Admin : User {}
来源：http://ohd.sufxvd.cn

[G06] 重写方法
来源：http://vee.316326.xyz

Py:   def greet(self): return "admin"
来源：http://szb.mhx1999.top

PHP:  public function greet(): string { return "admin"; }
来源：http://uxl.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://onn.bjfxy.top

TS:   greet(): string { return "admin"; }
来源：http://vhw.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://bdk.fehbvm.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cvf.uphjek.com

Ruby: def greet; "admin"; end
来源：http://pxd.ywan-chungtsiang.top

C#:   public override string Greet() => "admin";
来源：http://xdq.aibaodan.cn

[G07] 调用父类方法
来源：http://ybt.smart0.xyz

Py:   super().greet()
来源：http://zuy.zhijiandao.cn

PHP:  parent::greet();
来源：http://rhw.hesvh.cn

JS:   super.greet();
来源：http://ffn.ehwqpu.com

TS:   super.greet();
来源：http://fpi.mhx1999.top

Java: super.greet();
来源：http://gso.hnqzz.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kzt.zhiwuduotai.top

Ruby: super
来源：http://efy.yangfankeji.com

C#:   base.Greet();
来源：http://lfi.hesvh.cn

[G08] 静态方法与属性
来源：http://vtp.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ndi.yangfankeji.com

PHP:  public static function f() {}
来源：http://rlj.zhijiandao.cn

JS:   static f() {}
来源：http://njk.ppjwa.cn

TS:   static f(): void {}
来源：http://jlm.hfpthk.cn

Java: static void f() {}
来源：http://zza.yj20258.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kvz.zdqjudy.top

Ruby: def self.f; end
来源：http://vlc.jianghu66.top

C#:   public static void F() {}
来源：http://unw.havefunace.top

[G09] 接口 / 抽象类
来源：http://pwt.zycfv.cn

Py:   from abc import ABC, abstractmethod
来源：http://dms.tarul.cn

PHP:  interface Shape { public function area(): float; }
来源：http://eiy.tanke756.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rha.vqdsnc.cn

TS:   interface Shape { area(): number; }
来源：http://jlz.fktsv.cn

Java: interface Shape { double area(); }
来源：http://uob.yuanzhike.top

Go:   type Shape interface { Area() float64 }
来源：http://sbv.yangfankeji.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dxz.pycfn.com

C#:   interface IShape { double Area(); }
来源：http://ebf.nwbrower.top

[G10] 访问控制
来源：http://kmh.feifeiyinyue.top

Py:   约定 _protected / __private（不强制）
来源：http://avt.jqgufenzy.top

PHP:  public / protected / private
来源：http://mna.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://cuk.yfazqb.com

TS:   public / protected / private
来源：http://oge.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://xbc.ctjpmb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://rie.bbcook.cn

Ruby: public / protected / private
来源：http://cov.vehdjk.com

C#:   public / protected / private / internal
来源：http://anl.wangdashe.top

[G11] getter / setter
来源：http://adb.fzhhl.top

Py:   @property 与 @x.setter
来源：http://jmo.daxiang520.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pcl.yfazqb.com

JS:   get name() { return this._name; }
来源：http://jbl.quarkkingdee.top

TS:   get name(): string { return this._name; }
来源：http://ivt.c1oappe.top

Java: public String getName() { return name; }
来源：http://rav.havefunace.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jkg.ivvv.top

Ruby: attr_accessor :name
来源：http://jvs.bbcook.cn

C#:   public string Name { get; set; }
来源：http://grh.zhaomingkeji.xyz

[G12] 对象转字符串
来源：http://xcj.vqdsnc.cn

Py:   def __str__(self): return self.name
来源：http://bcu.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://skj.yj202588.top

JS:   toString() { return this.name; }
来源：http://mwr.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://uep.cashguo.top

Java: @Override public String toString() { return name; }
来源：http://pad.shzxlz.cn

Go:   func (u User) String() string { return u.Name }
来源：http://asj.hywenlv.cn

Ruby: def to_s; @name; end
来源：http://vtn.ybcxt.top

C#:   public override string ToString() => Name;
来源：http://bjv.zhoulong.xyz

[G13] 判断对象类型
来源：http://dfr.zycfv.cn

Py:   isinstance(u, User)
来源：http://sbf.zhoulong.xyz

PHP:  $u instanceof User
来源：http://bbd.sufxvd.cn

JS:   u instanceof User
来源：http://hzv.sysykeji.top

TS:   u instanceof User
来源：http://ywf.fktsv.cn

Java: u instanceof User
来源：http://tgy.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://eav.xuetiantiany.cn

Ruby: u.is_a?(User)
来源：http://iiq.redwolf501.top

C#:   u is User
来源：http://yrd.shzxlz.cn

[G14] 数据类 / record
来源：http://rqm.yanxiufei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rdl.nwbrower.top

PHP:  // 用 readonly 属性模拟
来源：http://shl.chenzaomai.com

JS:   // 无内置：普通类或对象字面量
来源：http://dnk.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://kve.nanxuanxn.top

Java: record User(String name, int age) {}
来源：http://fjd.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://nrt.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dhp.zycfv.cn

C#:   record User(string Name, int Age);
来源：http://org.aizwys.cn

[G15] 枚举
来源：http://afj.fengsongda.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vac.ydzc1.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bat.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xmd.sxryk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cyf.hysaishi.cn

Java: enum Color { RED, GREEN }
来源：http://lwk.sufxvd.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vvz.0kj1m.cn

Ruby: Color = %i[red green].freeze
来源：http://dnd.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ccq.yangfankeji.com

[G16] 对象转数组 / 字典
来源：http://kia.316326.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rex.ybcxt.top

PHP:  get_object_vars($obj);
来源：http://tub.chenzaomai.com

JS:   Object.entries(obj)
来源：http://emu.gzhubu.top

TS:   Object.entries(obj)
来源：http://arm.dashuyun.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wjh.ydzc1.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tri.aibaodan.cn

Ruby: obj.instance_variables
来源：http://ezx.hammf.cn

C#:   // 用反射或 System.Text.Json
来源：http://pio.zhijiandao.cn

================================================================================
来源：http://zgx.316326.xyz

H. 异常与错误处理
来源：http://mti.jqgfzy.top

================================================================================
来源：http://wej.daxiang520.top

[H01] try / catch 基础
来源：http://mhm.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hlk.tian-w.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jcg.ywan-chungtsiang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xxv.feifeiyinyue.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fpo.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oph.zhiwuduotai.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://svl.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ots.jinghuilouyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://arb.chenjidiqi.icu

[H02] finally / ensure 收尾
来源：http://svy.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://lmg.iojbl.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://akr.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ewf.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gtr.hysaishi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vpc.fanxiaobao.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://axt.cdnleiting.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qdf.nwbrower.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://azr.nwbrower.top

[H03] 主动抛出异常
来源：http://piu.tianlin.xyz

Py:   raise ValueError("错误信息")
来源：http://vih.yongpay.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zpu.tian-w.cn

JS:   throw new Error("错误信息");
来源：http://wnp.xylfe.cn

TS:   throw new Error("错误信息");
来源：http://una.0kj1m.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lmv.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://paq.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ceo.zycfv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://csf.yueranfly.top

[H04] 自定义异常类型
来源：http://epr.shanyushiyangtech.top

Py:   class MyError(Exception): pass
来源：http://ydf.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ljw.fktsv.cn

JS:   class MyError extends Error {}
来源：http://twu.vqdsnc.cn

TS:   class MyError extends Error {}
来源：http://rrr.cucudq.cn

Java: class MyException extends RuntimeException {}
来源：http://wbc.fzhhl.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zoq.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://mno.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://zet.haohaochexian.top

[H05] 捕获特定类型
来源：http://yrb.shzxlz.cn

Py:   except ValueError as e:
来源：http://roj.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qlf.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://rla.chenzaomai.com

TS:   if (e instanceof TypeError) {}
来源：http://ggr.jqgufenzy.top

Java: catch (IOException | SQLException e) {}
来源：http://pbc.nanxuanxn.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xdt.316326.xyz

Ruby: rescue ArgumentError => e
来源：http://vms.zhiwuduotai.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ggo.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://zds.snrcjt.cn

Py:   value = d.get("k") or default
来源：http://lir.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wmz.yongpay.top

JS:   obj?.a?.b;  d ?? default
来源：http://vnz.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uhk.ehwqpu.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://aua.dianchejie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xbx.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://osy.zhengqikj.top

C#:   obj?.A?.B ?? default
来源：http://kto.yuxming.cn

[H07] 断言
来源：http://qes.yonumen.top

Py:   assert x > 0, "必须为正"
来源：http://rlh.0kj1m.cn

PHP:  assert($x > 0);
来源：http://jtg.xingfuxueyuan.xyz

JS:   console.assert(x > 0);
来源：http://rbw.meibo888.top

TS:   console.assert(x > 0);
来源：http://hef.daxiang520.top

Java: assert x > 0 : "必须为正";
来源：http://ert.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iuo.jqgfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://hya.epnwcf.com

C#:   Debug.Assert(x > 0);
来源：http://sgx.guowangkeji.top

[H08] 获取错误信息与堆栈
来源：http://xcy.jlsjyb.cn

Py:   str(e);  traceback.format_exc()
来源：http://ssp.zdqjudy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bdi.yfazqb.com

JS:   e.message;  e.stack
来源：http://bar.yj202588.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ovu.chenjidiqi.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://tvt.chenjidiqi.icu

Go:   err.Error()
来源：http://irl.dashuyun.cn


<!-- 参考信息 -->