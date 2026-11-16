代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qyx.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wwa.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bmv.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qin.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vya.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jcp.sufxvd.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yng.jianghu66.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vhr.sweek.top

[F05] 判断文件或目录是否存在
来源：http://vdw.yuanzhike.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hjf.jlsjyb.cn

PHP:  file_exists("a.txt");
来源：http://oyh.gotoacloud.top

JS:   fs.existsSync("a.txt")
来源：http://toz.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://nmc.vehdjk.com

Java: Files.exists(Path.of("a.txt"))
来源：http://bqs.nanxinkj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bol.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://prp.nanxinkj.top

C#:   File.Exists("a.txt")
来源：http://vpe.snrcjt.cn

[F06] 删除文件
来源：http://shy.haohaochexian.top

Py:   os.remove("a.txt")
来源：http://afk.fzhhl.top

PHP:  unlink("a.txt");
来源：http://vxk.52xcode.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nnh.xziqi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hvf.shangyingyoupin.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nrj.aizwys.cn

Go:   os.Remove("a.txt")
来源：http://ays.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://ugx.tanke756.top

C#:   File.Delete("a.txt");
来源：http://lgb.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://rkm.zdbjq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yyy.cheryme.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qpu.uphjek.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sya.hnxiangtu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mcy.hnxiangtu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aeh.c1oappe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ulr.guowangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eho.xuanzx.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uei.sxryk.cn

[F08] 遍历目录
来源：http://tjy.cdnleiting.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ukk.vehdjk.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vay.hywenlv.cn

JS:   fs.readdirSync("dir")
来源：http://odx.birdmap.top

TS:   fs.readdirSync("dir")
来源：http://xng.cqqwz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://abr.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jeo.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://ass.ydzc1.top

C#:   Directory.GetFiles("dir")
来源：http://cyl.chenlongwang.top

[F09] 获取文件大小
来源：http://zwg.feifeiyinyue.top

Py:   os.path.getsize("a.txt")
来源：http://xvq.sysykeji.top

PHP:  filesize("a.txt");
来源：http://bti.hongshengwenyu.top

JS:   fs.statSync("a.txt").size
来源：http://eao.0kj1m.cn

TS:   fs.statSync("a.txt").size
来源：http://tdv.ywan-chungtsiang.top

Java: Files.size(Path.of("a.txt"))
来源：http://fas.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vdz.zhoulong.xyz

Ruby: File.size("a.txt")
来源：http://qwz.daxiang520.top

C#:   new FileInfo("a.txt").Length
来源：http://rfz.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://czd.jqgfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://stg.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gna.vqdsnc.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yut.yueranfly.top

TS:   path.extname("a.txt")
来源：http://kgt.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zcv.guannengcc.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oum.hnxiangtu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ctp.xuanzx.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vmx.birdmap.top

[F11] 复制与移动文件
来源：http://rjd.jyoumei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eee.ctjpmb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ttj.xinyue.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iwx.yuanzhike.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xes.aibaodan.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://whd.aibaodan.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ajn.dashuyun.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sqo.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cuh.chenlongwang.top

[F12] CSV 读写
来源：http://knp.smart0.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hmq.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hnl.zdqjudy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rav.hammf.cn

TS:   // 同上
来源：http://csl.xinyue.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uzm.pycfn.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rcp.havefunace.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vhq.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://chw.zhiwuduotai.top

================================================================================
来源：http://hfc.daxiang520.top

G. 面向对象
来源：http://sdt.jqgfzy.top

================================================================================
来源：http://tbx.shuidangran.top

[G01] 定义类
来源：http://vqn.sufxvd.cn

Py:   class User: pass
来源：http://wli.jyoumei.cn

PHP:  class User {}
来源：http://orh.sweek.top

JS:   class User {}
来源：http://itb.cashguo.top

TS:   class User { name: string = ""; }
来源：http://wkf.bjfxy.top

Java: class User {}
来源：http://jdi.ctjpmb.com

Go:   type User struct { Name string }
来源：http://jcq.jlsjyb.cn

Ruby: class User; end
来源：http://atu.hammf.cn

C#:   class User {}
来源：http://flm.nwbrower.top

[G02] 构造函数
来源：http://ddh.fengsongda.top

Py:   def __init__(self, name): self.name = name
来源：http://lli.chenzaomai.com

PHP:  public function __construct(public string $name) {}
来源：http://ume.zdqjudy.top

JS:   constructor(name) { this.name = name; }
来源：http://ail.ivvv.top

TS:   constructor(public name: string) {}
来源：http://mhr.daxiang520.top

Java: User(String name) { this.name = name; }
来源：http://cbp.hnqzz.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lvv.zhijiandao.cn

Ruby: def initialize(name); @name = name; end
来源：http://ify.kuanghao11.cn

C#:   public User(string name) { Name = name; }
来源：http://orj.gaohongyu789.top

[G03] 实例属性
来源：http://bfm.yangfankeji.com

Py:   self.name = "x"
来源：http://ubj.yj20258.top

PHP:  public string $name = "x";
来源：http://nfj.cdnleiting.top

JS:   this.name = "x";
来源：http://xpg.shanyushiyangkeji.top

TS:   name: string = "x";
来源：http://yxk.shangyingyoupin.top

Java: private String name;
来源：http://dhf.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mql.epnwcf.com

Ruby: @name = "x"
来源：http://tos.yanxiufei.cn

C#:   public string Name { get; set; } = "x";
来源：http://cnm.hnxiangtu.top

[G04] 定义方法
来源：http://gnn.fehbvm.com

Py:   def greet(self): return self.name
来源：http://mpi.fktsv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jvz.cheryme.top

JS:   greet() { return this.name; }
来源：http://vox.ydzc1.top

TS:   greet(): string { return this.name; }
来源：http://qji.hnxiangtu.top

Java: String greet() { return name; }
来源：http://gtg.fzhhl.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://sgh.yvedp.cn

Ruby: def greet; @name; end
来源：http://ifn.nanxinkj.top

C#:   public string Greet() => Name;
来源：http://lty.snrcjt.cn

[G05] 继承
来源：http://jcl.ppjwa.cn

Py:   class Admin(User): pass
来源：http://lqc.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://knz.xuanzx.com

JS:   class Admin extends User {}
来源：http://qgs.zdbjq.cn

TS:   class Admin extends User {}
来源：http://izn.bjfxy.top

Java: class Admin extends User {}
来源：http://ggs.fehbvm.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bji.uphjek.com

Ruby: class Admin < User; end
来源：http://zwb.shanyushiyangkeji.top

C#:   class Admin : User {}
来源：http://uhp.hcnkem.com

[G06] 重写方法
来源：http://yvs.feifeiyinyue.top

Py:   def greet(self): return "admin"
来源：http://xzg.mhx1999.top

PHP:  public function greet(): string { return "admin"; }
来源：http://icw.ppjwa.cn

JS:   greet() { return "admin"; }
来源：http://sjv.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://rsa.cheryme.top

Java: @Override String greet() { return "admin"; }
来源：http://pxn.nanxinkj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wsj.pycfn.com

Ruby: def greet; "admin"; end
来源：http://fys.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://vpm.andypj.xyz

[G07] 调用父类方法
来源：http://kqj.shanyushiyangtech.top

Py:   super().greet()
来源：http://vcp.cheryme.top

PHP:  parent::greet();
来源：http://ejm.birdmap.top

JS:   super.greet();
来源：http://wor.yanxiufei.cn

TS:   super.greet();
来源：http://utw.hywenlv.cn

Java: super.greet();
来源：http://jcp.jqgufenzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tis.nanxinkj.top

Ruby: super
来源：http://sry.shanyushiyangtech.top

C#:   base.Greet();
来源：http://dmf.yuanzhike.top

[G08] 静态方法与属性
来源：http://cro.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wyt.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://uzu.yj20258.top

JS:   static f() {}
来源：http://mhf.xinyue.icu

TS:   static f(): void {}
来源：http://vra.sysykeji.top

Java: static void f() {}
来源：http://spc.sysykeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xic.jinyuanbaomall.cn

Ruby: def self.f; end
来源：http://yiq.chenzaomai.com

C#:   public static void F() {}
来源：http://ecn.zhengqikj.top

[G09] 接口 / 抽象类
来源：http://rka.cheryme.top

Py:   from abc import ABC, abstractmethod
来源：http://bbd.zhengqikj.top

PHP:  interface Shape { public function area(): float; }
来源：http://oad.tanke756.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cqz.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://atw.sweek.top

Java: interface Shape { double area(); }
来源：http://bdu.ydjk.org.cn

Go:   type Shape interface { Area() float64 }
来源：http://jhl.ydjk.org.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rsn.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://rgi.vehdjk.com

[G10] 访问控制
来源：http://zvp.jiagoushi.top

Py:   约定 _protected / __private（不强制）
来源：http://ksl.andypj.xyz

PHP:  public / protected / private
来源：http://ynn.jyoumei.cn

JS:   #private 字段；其余公开
来源：http://juc.jinyuanbaomall.cn

TS:   public / protected / private
来源：http://yho.wangshuangyany.cn

Java: public / protected / private / 默认包级
来源：http://ony.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://aai.xinyue.icu

Ruby: public / protected / private
来源：http://ket.xziqi.cn

C#:   public / protected / private / internal
来源：http://nsw.svipenyu.cn

[G11] getter / setter
来源：http://nva.gzhubu.top

Py:   @property 与 @x.setter
来源：http://rmx.jianghu66.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qjk.iojbl.cn

JS:   get name() { return this._name; }
来源：http://fel.daria6918.cn

TS:   get name(): string { return this._name; }
来源：http://rfb.sweek.top

Java: public String getName() { return name; }
来源：http://imc.sufxvd.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qqp.sweek.top

Ruby: attr_accessor :name
来源：http://vug.zhiwuduotai.top

C#:   public string Name { get; set; }
来源：http://evp.pengpengdd.cyou

[G12] 对象转字符串
来源：http://knj.chenzaomai.com

Py:   def __str__(self): return self.name
来源：http://vgs.gaohongyu789.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fyl.sysykeji.top

JS:   toString() { return this.name; }
来源：http://wtb.jinqigfzy.top

TS:   toString(): string { return this.name; }
来源：http://tcv.cashguo.top

Java: @Override public String toString() { return name; }
来源：http://tpd.yuxming.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wck.c1oappe.top

Ruby: def to_s; @name; end
来源：http://clw.shuidangran.top

C#:   public override string ToString() => Name;
来源：http://aen.dianchejie.cn

[G13] 判断对象类型
来源：http://jfc.vehdjk.com

Py:   isinstance(u, User)
来源：http://zpz.zdbjq.cn

PHP:  $u instanceof User
来源：http://cfl.tanke756.top

JS:   u instanceof User
来源：http://mrc.cdnleiting.top

TS:   u instanceof User
来源：http://djy.cdnleiting.top

Java: u instanceof User
来源：http://reu.andypj.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://bqv.ctjpmb.com

Ruby: u.is_a?(User)
来源：http://qtf.jianghu66.top

C#:   u is User
来源：http://grg.epnwcf.com

[G14] 数据类 / record
来源：http://jid.daria6918.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mob.xziqi.cn

PHP:  // 用 readonly 属性模拟
来源：http://tbt.fehbvm.com

JS:   // 无内置：普通类或对象字面量
来源：http://snr.dianchejie.cn

TS:   type User = { name: string; age: number };
来源：http://gmx.fanxiaobao.xyz

Java: record User(String name, int age) {}
来源：http://kqk.nanxuanxn.top

Go:   type User struct { Name string; Age int }
来源：http://rqj.feifeiyinyue.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ith.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://skj.chenzaomai.com

[G15] 枚举
来源：http://ehu.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://phr.redwolf501.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yrh.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ght.meibo888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://trj.jinqigufen.top

Java: enum Color { RED, GREEN }
来源：http://aeg.guowangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vvi.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://zki.zhengqikj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ipt.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://boe.meibo888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ppv.smart0.xyz

PHP:  get_object_vars($obj);
来源：http://xqo.jinqigfzy.top

JS:   Object.entries(obj)
来源：http://bnv.redwolf501.top

TS:   Object.entries(obj)
来源：http://dhn.jqgfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zmr.redwolf501.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rux.wangdashe.top

Ruby: obj.instance_variables
来源：http://ufc.hesvh.cn

C#:   // 用反射或 System.Text.Json
来源：http://sid.fanxiaobao.xyz

================================================================================
来源：http://yxy.aizwys.cn

H. 异常与错误处理
来源：http://wyh.yangfankeji.com

================================================================================
来源：http://ryk.bbcook.cn

[H01] try / catch 基础
来源：http://nez.chenjidiqi.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://paq.xuanzx.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rmk.vqdsnc.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://haa.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fya.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dsd.andypj.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pxj.vehdjk.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mrz.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jjm.guannengcc.top

[H02] finally / ensure 收尾
来源：http://tvo.hammf.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xym.hnqzz.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fun.yuanzhike.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zpc.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vom.cdnleiting.top

Java: try { f(); } finally { cleanup(); }
来源：http://thq.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ijg.bjfxy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://oqp.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cpc.hnxiangtu.top

[H03] 主动抛出异常
来源：http://ohx.hnqzz.top

Py:   raise ValueError("错误信息")
来源：http://bsc.epnwcf.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ipt.guowangkeji.top

JS:   throw new Error("错误信息");
来源：http://zpv.316326.xyz

TS:   throw new Error("错误信息");
来源：http://pgi.nanxinkj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://uqs.cashguo.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jbh.jianghu66.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zgm.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xnq.yanxiufei.cn

[H04] 自定义异常类型
来源：http://bgm.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://cjf.tian-w.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kze.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://drs.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://trj.yj20258.top

Java: class MyException extends RuntimeException {}
来源：http://hsa.hammf.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lqy.sweek.top

Ruby: class MyError < StandardError; end
来源：http://zdo.gaohongyu789.top

C#:   class MyException : Exception {}
来源：http://wee.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://oks.ywan-chungtsiang.top

Py:   except ValueError as e:
来源：http://rfc.shuidangran.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ert.snrcjt.cn

JS:   if (e instanceof TypeError) {}
来源：http://xab.xingfuxueyuan.xyz

TS:   if (e instanceof TypeError) {}
来源：http://pjp.nanxuanxn.top

Java: catch (IOException | SQLException e) {}
来源：http://bub.hywenlv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zra.uphjek.com

Ruby: rescue ArgumentError => e
来源：http://rot.wangdashe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://keu.snrcjt.cn

[H06] 可选值 / 空值安全访问
来源：http://ncc.birdmap.top

Py:   value = d.get("k") or default
来源：http://dcr.jqgfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://upn.sjlbkw.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ldv.shanyushiyangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://iiy.jianghu66.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dnm.yueranfly.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kwn.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://eym.jinqigfzy.top

C#:   obj?.A?.B ?? default
来源：http://iuy.yanxiufei.cn

[H07] 断言
来源：http://qep.cdnleiting.top

Py:   assert x > 0, "必须为正"
来源：http://ami.hywenlv.cn

PHP:  assert($x > 0);
来源：http://xax.hongshengwenyu.top

JS:   console.assert(x > 0);
来源：http://sdo.xingfuxueyuan.xyz

TS:   console.assert(x > 0);
来源：http://krj.nwbrower.top

Java: assert x > 0 : "必须为正";
来源：http://qtd.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dot.sweek.top

Ruby: raise "必须为正" unless x > 0
来源：http://sbm.yonumen.top

C#:   Debug.Assert(x > 0);
来源：http://dcb.ivvv.top

[H08] 获取错误信息与堆栈
来源：http://axl.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://kcc.hammf.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ezw.yueranfly.top

JS:   e.message;  e.stack
来源：http://eqr.cqqwz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pji.kuanghao11.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dtr.daria6918.cn

Go:   err.Error()
来源：http://lik.hnqzz.top


<!-- 参考信息 -->