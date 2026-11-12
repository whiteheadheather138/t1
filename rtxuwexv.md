代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dic.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mhs.hnxiangtu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://crb.xinyue.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ayv.xylfe.cn

[F05] 判断文件或目录是否存在
来源：http://mzc.hongshengwenyu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://opx.gogol.net.cn

PHP:  file_exists("a.txt");
来源：http://tkg.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://odl.cheryme.top

TS:   fs.existsSync("a.txt")
来源：http://mga.ybcxt.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jvl.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lxr.hesvh.cn

Ruby: File.exist?("a.txt")
来源：http://aam.yuxming.cn

C#:   File.Exists("a.txt")
来源：http://fts.xziqi.cn

[F06] 删除文件
来源：http://gaz.hywenlv.cn

Py:   os.remove("a.txt")
来源：http://zzn.c1oappe.top

PHP:  unlink("a.txt");
来源：http://ddo.hywenlv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cxk.jqgufenzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://mjz.xziqi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bro.fengsongda.top

Go:   os.Remove("a.txt")
来源：http://dbp.xziqi.cn

Ruby: File.delete("a.txt")
来源：http://rrh.nwbrower.top

C#:   File.Delete("a.txt");
来源：http://dvb.xylfe.cn

[F07] 创建目录（含多级）
来源：http://tja.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bog.sysykeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ffq.vehdjk.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://byx.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uad.jinqigufen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lsu.gaohongyu789.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oev.gaohongyu789.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xxs.dianchejie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rko.jianghu66.top

[F08] 遍历目录
来源：http://oai.zhongyouzk.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hrn.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gpv.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://msq.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://yuy.yfazqb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dej.hnxiangtu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://sxr.cucudq.cn

Ruby: Dir.children("dir")
来源：http://jwz.zhengqikj.top

C#:   Directory.GetFiles("dir")
来源：http://ngr.cqqwz.cn

[F09] 获取文件大小
来源：http://ruz.pengpengdd.cyou

Py:   os.path.getsize("a.txt")
来源：http://elc.shuidangran.top

PHP:  filesize("a.txt");
来源：http://hwj.yfazqb.com

JS:   fs.statSync("a.txt").size
来源：http://dzx.fengsongda.top

TS:   fs.statSync("a.txt").size
来源：http://pni.sysykeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://dgg.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hxa.yj20258.top

Ruby: File.size("a.txt")
来源：http://fpw.fehbvm.com

C#:   new FileInfo("a.txt").Length
来源：http://ona.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://zgd.pycfn.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ouy.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aqy.xuetiantiany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nal.birdmap.top

TS:   path.extname("a.txt")
来源：http://gma.aizwys.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vel.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dus.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oei.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fqr.52xcode.cn

[F11] 复制与移动文件
来源：http://mrg.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fha.tian-w.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dlo.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ppu.ydzc1.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rot.wangshuangyany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ktk.yj20258.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cjm.gaohongyu789.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rhq.smart0.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://btv.ppjwa.cn

[F12] CSV 读写
来源：http://rcu.xuanzx.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://utl.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://juy.andypj.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ori.ppjwa.cn

TS:   // 同上
来源：http://znl.sjlbkw.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://erp.iojbl.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wgn.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vms.shanyushiyangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qcd.xinyue.icu

================================================================================
来源：http://fmi.cashguo.top

G. 面向对象
来源：http://qyc.dashuyun.cn

================================================================================
来源：http://dqf.tian-w.cn

[G01] 定义类
来源：http://hal.zhixingplan.top

Py:   class User: pass
来源：http://lfd.jinghuilouyu.cn

PHP:  class User {}
来源：http://jza.tarul.cn

JS:   class User {}
来源：http://lrg.cdnleiting.top

TS:   class User { name: string = ""; }
来源：http://iby.shanyushiyangkeji.top

Java: class User {}
来源：http://lhd.0kj1m.cn

Go:   type User struct { Name string }
来源：http://hrt.aibaodan.cn

Ruby: class User; end
来源：http://gud.zhijiandao.cn

C#:   class User {}
来源：http://opv.ehwqpu.com

[G02] 构造函数
来源：http://fqu.iojbl.cn

Py:   def __init__(self, name): self.name = name
来源：http://lwa.aizwys.cn

PHP:  public function __construct(public string $name) {}
来源：http://bbb.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://mwg.uphjek.com

TS:   constructor(public name: string) {}
来源：http://pzb.xinyue.icu

Java: User(String name) { this.name = name; }
来源：http://rvf.hysaishi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jzz.yanxiufei.cn

Ruby: def initialize(name); @name = name; end
来源：http://jxd.guowangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://jjy.yvedp.cn

[G03] 实例属性
来源：http://vkd.fktsv.cn

Py:   self.name = "x"
来源：http://bns.cqqwz.cn

PHP:  public string $name = "x";
来源：http://xlz.wangdashe.top

JS:   this.name = "x";
来源：http://hrj.tanke756.top

TS:   name: string = "x";
来源：http://tve.fanxiaobao.xyz

Java: private String name;
来源：http://dbt.zhaomingkeji.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://inq.zhongyouzk.top

Ruby: @name = "x"
来源：http://xct.shangyingyoupin.top

C#:   public string Name { get; set; } = "x";
来源：http://jaj.xuetiantiany.cn

[G04] 定义方法
来源：http://rcx.havefunace.top

Py:   def greet(self): return self.name
来源：http://miy.pycfn.com

PHP:  public function greet(): string { return $this->name; }
来源：http://qhc.nwbrower.top

JS:   greet() { return this.name; }
来源：http://mqo.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://ild.zycfv.cn

Java: String greet() { return name; }
来源：http://spt.gaohongyu789.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xhc.fehbvm.com

Ruby: def greet; @name; end
来源：http://pke.hysaishi.cn

C#:   public string Greet() => Name;
来源：http://sct.ydjk.org.cn

[G05] 继承
来源：http://uft.0kj1m.cn

Py:   class Admin(User): pass
来源：http://vcv.nanxuanxn.top

PHP:  class Admin extends User {}
来源：http://koj.aibaodan.cn

JS:   class Admin extends User {}
来源：http://ark.gzhubu.top

TS:   class Admin extends User {}
来源：http://tuk.yanxiufei.cn

Java: class Admin extends User {}
来源：http://ywz.xuetiantiany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qnj.yangfankeji.com

Ruby: class Admin < User; end
来源：http://kan.chenjidiqi.icu

C#:   class Admin : User {}
来源：http://qkb.tianlin.xyz

[G06] 重写方法
来源：http://npo.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://dxr.zhongyouzk.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jon.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://yck.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://gqj.dianchejie.cn

Java: @Override String greet() { return "admin"; }
来源：http://bti.vqdsnc.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qxt.epnwcf.com

Ruby: def greet; "admin"; end
来源：http://dyh.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://tyn.ctjpmb.com

[G07] 调用父类方法
来源：http://dmv.316326.xyz

Py:   super().greet()
来源：http://vsx.aibaodan.cn

PHP:  parent::greet();
来源：http://dfv.zhijiandao.cn

JS:   super.greet();
来源：http://bxi.xylfe.cn

TS:   super.greet();
来源：http://yzm.cqqwz.cn

Java: super.greet();
来源：http://anq.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wll.hcnkem.com

Ruby: super
来源：http://syk.yj202588.top

C#:   base.Greet();
来源：http://kcw.yvedp.cn

[G08] 静态方法与属性
来源：http://pur.nanxuanxn.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://feq.uphjek.com

PHP:  public static function f() {}
来源：http://cbe.svipenyu.cn

JS:   static f() {}
来源：http://jwg.ctjpmb.com

TS:   static f(): void {}
来源：http://wyu.gzhubu.top

Java: static void f() {}
来源：http://gyv.yj20258.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kgk.wangdashe.top

Ruby: def self.f; end
来源：http://sjh.feifeiyinyue.top

C#:   public static void F() {}
来源：http://upf.mhx1999.top

[G09] 接口 / 抽象类
来源：http://kny.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://jcb.yueranfly.top

PHP:  interface Shape { public function area(): float; }
来源：http://tlf.pycfn.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://qhf.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://qvv.sufxvd.cn

Java: interface Shape { double area(); }
来源：http://vtf.nanxinkj.top

Go:   type Shape interface { Area() float64 }
来源：http://lzk.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cwh.nwbrower.top

C#:   interface IShape { double Area(); }
来源：http://gbr.zhiwuduotai.top

[G10] 访问控制
来源：http://chx.xinyue.icu

Py:   约定 _protected / __private（不强制）
来源：http://jer.ydzc1.top

PHP:  public / protected / private
来源：http://sbf.jqgufenzy.top

JS:   #private 字段；其余公开
来源：http://yxg.zhixingplan.top

TS:   public / protected / private
来源：http://poj.sysykeji.top

Java: public / protected / private / 默认包级
来源：http://yll.fktsv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rlt.jinqigufen.top

Ruby: public / protected / private
来源：http://rwt.smart0.xyz

C#:   public / protected / private / internal
来源：http://ojh.ydjk.org.cn

[G11] getter / setter
来源：http://vtu.cdnleiting.top

Py:   @property 与 @x.setter
来源：http://ven.xziqi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://toy.wangdashe.top

JS:   get name() { return this._name; }
来源：http://wjj.xinyue.icu

TS:   get name(): string { return this._name; }
来源：http://mbx.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://chy.cheryme.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://eay.yj20258888.top

Ruby: attr_accessor :name
来源：http://idf.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://jcn.chenjidiqi.icu

[G12] 对象转字符串
来源：http://dcl.fengsongda.top

Py:   def __str__(self): return self.name
来源：http://clm.uphjek.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://opo.jinyuanbaomall.cn

JS:   toString() { return this.name; }
来源：http://ebx.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://oeh.snrcjt.cn

Java: @Override public String toString() { return name; }
来源：http://pvd.fengsongda.top

Go:   func (u User) String() string { return u.Name }
来源：http://ioj.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://jcw.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://tjz.ywan-chungtsiang.top

[G13] 判断对象类型
来源：http://erw.yj20258.top

Py:   isinstance(u, User)
来源：http://zvk.ehwqpu.com

PHP:  $u instanceof User
来源：http://umg.vehdjk.com

JS:   u instanceof User
来源：http://ngl.hfpthk.cn

TS:   u instanceof User
来源：http://juj.shangyingyoupin.top

Java: u instanceof User
来源：http://ota.andypj.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://chh.cdnleiting.top

Ruby: u.is_a?(User)
来源：http://erf.cucudq.cn

C#:   u is User
来源：http://jlo.chenzaomai.com

[G14] 数据类 / record
来源：http://rnq.cqqwz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://boy.zycfv.cn

PHP:  // 用 readonly 属性模拟
来源：http://ggp.ydzc1.top

JS:   // 无内置：普通类或对象字面量
来源：http://nbe.tianlin.xyz

TS:   type User = { name: string; age: number };
来源：http://wfb.havefunace.top

Java: record User(String name, int age) {}
来源：http://hhg.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://fhb.hcnkem.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vbj.guannengcc.top

C#:   record User(string Name, int Age);
来源：http://ihg.zdqjudy.top

[G15] 枚举
来源：http://hpk.tanke756.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nxh.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://hkc.yangfankeji.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cdx.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ifc.andypj.xyz

Java: enum Color { RED, GREEN }
来源：http://sed.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oql.yuxming.cn

Ruby: Color = %i[red green].freeze
来源：http://lqp.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://flk.sufxvd.cn

[G16] 对象转数组 / 字典
来源：http://hvj.zhijiandao.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nfc.vehdjk.com

PHP:  get_object_vars($obj);
来源：http://ebe.jinyuanbaomall.cn

JS:   Object.entries(obj)
来源：http://mpa.epnwcf.com

TS:   Object.entries(obj)
来源：http://lvz.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fld.gotoacloud.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nrw.jqgfzy.top

Ruby: obj.instance_variables
来源：http://zzw.ehwqpu.com

C#:   // 用反射或 System.Text.Json
来源：http://quf.yj20258888.top

================================================================================
来源：http://jzh.zhiwuduotai.top

H. 异常与错误处理
来源：http://oju.tanke756.top

================================================================================
来源：http://ssd.iojbl.cn

[H01] try / catch 基础
来源：http://pbo.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jiu.nwbrower.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://snu.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uxi.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bin.nwbrower.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://btq.yj202588.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iem.xylfe.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qtl.tarul.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xkt.c1oappe.top

[H02] finally / ensure 收尾
来源：http://ikq.shuidangran.top

Py:   try: f()⏎finally: cleanup()
来源：http://xch.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://udd.gaohongyu789.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tyr.hysaishi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dqb.ctjpmb.com

Java: try { f(); } finally { cleanup(); }
来源：http://rtx.snrcjt.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kjo.bjfxy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cna.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mkl.fanxiaobao.xyz

[H03] 主动抛出异常
来源：http://gut.hammf.cn

Py:   raise ValueError("错误信息")
来源：http://dfq.316326.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nry.iojbl.cn

JS:   throw new Error("错误信息");
来源：http://ynh.xylfe.cn

TS:   throw new Error("错误信息");
来源：http://rey.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zab.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pun.yj20258.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fti.chenlongwang.top

C#:   throw new ArgumentException("错误信息");
来源：http://fev.dashuyun.cn

[H04] 自定义异常类型
来源：http://zrr.xingfuxueyuan.xyz

Py:   class MyError(Exception): pass
来源：http://rde.cucudq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://trz.chenzaomai.com

JS:   class MyError extends Error {}
来源：http://znh.svipenyu.cn

TS:   class MyError extends Error {}
来源：http://mat.hfpthk.cn

Java: class MyException extends RuntimeException {}
来源：http://rpn.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://okf.jlsjyb.cn

Ruby: class MyError < StandardError; end
来源：http://fbm.wangdashe.top

C#:   class MyException : Exception {}
来源：http://dld.nwbrower.top

[H05] 捕获特定类型
来源：http://ktj.vqdsnc.cn

Py:   except ValueError as e:
来源：http://pul.iojbl.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zwy.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://snu.yj20258888.top

TS:   if (e instanceof TypeError) {}
来源：http://njl.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://tqo.aizwys.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hhd.ctjpmb.com

Ruby: rescue ArgumentError => e
来源：http://crg.bjfxy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://flz.snrcjt.cn

[H06] 可选值 / 空值安全访问
来源：http://cbp.birdmap.top

Py:   value = d.get("k") or default
来源：http://kmy.birdmap.top

PHP:  $v = $d["k"] ?? null;
来源：http://uqe.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://ndc.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jkm.chenzaomai.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nps.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zac.xylfe.cn

Ruby: d&.dig(:a, :b)
来源：http://eim.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://zdi.yonumen.top

[H07] 断言
来源：http://jnh.guannengcc.top

Py:   assert x > 0, "必须为正"
来源：http://qcr.fengsongda.top

PHP:  assert($x > 0);
来源：http://pwm.gaohongyu789.top

JS:   console.assert(x > 0);
来源：http://ghd.shuidangran.top

TS:   console.assert(x > 0);
来源：http://fjd.ydzc1.top

Java: assert x > 0 : "必须为正";
来源：http://eqe.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wdw.hfpthk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qpi.yangfankeji.com

C#:   Debug.Assert(x > 0);
来源：http://sse.jiagoushi.top

[H08] 获取错误信息与堆栈
来源：http://rwi.cqqwz.cn

Py:   str(e);  traceback.format_exc()
来源：http://zdb.zycfv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rrv.yfazqb.com

JS:   e.message;  e.stack
来源：http://yly.jlsjyb.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://scc.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://rop.hfpthk.cn

Go:   err.Error()
来源：http://qma.jianghu66.top

Ruby: e.message;  e.backtrace
来源：http://knh.zhixingplan.top

C#:   e.Message;  e.StackTrace
来源：http://uyx.cdnleiting.top

[H09] 带错误码的异常
来源：http://rmk.tian-w.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fei.hnxiangtu.top


<!-- 参考信息 -->