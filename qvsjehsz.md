代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://txw.gzhubu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://otx.xinyue.icu

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jbl.jyoumei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pxd.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://jra.zdqjudy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://evb.cheryme.top

PHP:  file_exists("a.txt");
来源：http://cet.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://edg.yongpay.top

TS:   fs.existsSync("a.txt")
来源：http://evj.zhaomingkeji.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://gga.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://psh.jinghuilouyu.cn

Ruby: File.exist?("a.txt")
来源：http://xdp.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://fsk.ctjpmb.com

[F06] 删除文件
来源：http://kbl.snrcjt.cn

Py:   os.remove("a.txt")
来源：http://obf.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://new.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://biz.yuxming.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uhx.jinqigfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://khe.vqdsnc.cn

Go:   os.Remove("a.txt")
来源：http://pfr.hywenlv.cn

Ruby: File.delete("a.txt")
来源：http://zud.jqgufenzy.top

C#:   File.Delete("a.txt");
来源：http://wnc.9152youxi.cn

[F07] 创建目录（含多级）
来源：http://boa.hongshengwenyu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vzw.ydzc1.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gfd.vqdsnc.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gpc.chenjidiqi.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vif.birdmap.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oyl.jlsjyb.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gca.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://igz.yvedp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tyn.jinqigfzy.top

[F08] 遍历目录
来源：http://bsu.shangyingyoupin.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tqq.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rmh.pycfn.com

JS:   fs.readdirSync("dir")
来源：http://tjh.pycfn.com

TS:   fs.readdirSync("dir")
来源：http://bxy.andypj.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yqx.quarkkingdee.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://imw.smart0.xyz

Ruby: Dir.children("dir")
来源：http://vas.yvedp.cn

C#:   Directory.GetFiles("dir")
来源：http://smr.redwolf501.top

[F09] 获取文件大小
来源：http://ukh.zhixingplan.top

Py:   os.path.getsize("a.txt")
来源：http://zbr.yanxiufei.cn

PHP:  filesize("a.txt");
来源：http://xwf.havefunace.top

JS:   fs.statSync("a.txt").size
来源：http://zcc.fktsv.cn

TS:   fs.statSync("a.txt").size
来源：http://cmm.yongpay.top

Java: Files.size(Path.of("a.txt"))
来源：http://cal.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vtv.cdnleiting.top

Ruby: File.size("a.txt")
来源：http://gie.yueranfly.top

C#:   new FileInfo("a.txt").Length
来源：http://swd.uphjek.com

[F10] 取文件扩展名 / 文件名
来源：http://pav.dashuyun.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xcb.ctjpmb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aue.meibo888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rre.nanxinkj.top

TS:   path.extname("a.txt")
来源：http://jqg.cashguo.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jup.birdmap.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nmj.vehdjk.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tfr.sweek.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mqn.jqgufenzy.top

[F11] 复制与移动文件
来源：http://mqz.fzhhl.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://srp.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yhv.cdnleiting.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hhf.bbcook.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lcm.andypj.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gaf.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vnf.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ver.xylfe.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eul.shanyushiyangkeji.top

[F12] CSV 读写
来源：http://fcs.cheryme.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lgh.sysykeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vwn.jinyuanbaomall.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://utm.sysykeji.top

TS:   // 同上
来源：http://sid.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hju.kuanghao11.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ajc.pengpengdd.cyou

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aam.yuxming.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nbh.snrcjt.cn

================================================================================
来源：http://uxf.zdbjq.cn

G. 面向对象
来源：http://mmm.hammf.cn

================================================================================
来源：http://vbz.jianghu66.top

[G01] 定义类
来源：http://ojb.sysykeji.top

Py:   class User: pass
来源：http://jix.jiagoushi.top

PHP:  class User {}
来源：http://mpj.hnqzz.top

JS:   class User {}
来源：http://rvd.nanxuanxn.top

TS:   class User { name: string = ""; }
来源：http://lkj.aibaodan.cn

Java: class User {}
来源：http://mah.cdnleiting.top

Go:   type User struct { Name string }
来源：http://unt.yfazqb.com

Ruby: class User; end
来源：http://rhd.jinqigfzy.top

C#:   class User {}
来源：http://xer.nanxinkj.top

[G02] 构造函数
来源：http://gea.daxiang520.top

Py:   def __init__(self, name): self.name = name
来源：http://oqo.ctjpmb.com

PHP:  public function __construct(public string $name) {}
来源：http://dub.ydzc1.top

JS:   constructor(name) { this.name = name; }
来源：http://rjw.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://zta.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://lgv.yfazqb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://psc.ivvv.top

Ruby: def initialize(name); @name = name; end
来源：http://fsg.zhengqikj.top

C#:   public User(string name) { Name = name; }
来源：http://vro.yangfankeji.com

[G03] 实例属性
来源：http://uyl.zdbjq.cn

Py:   self.name = "x"
来源：http://huw.dianchejie.cn

PHP:  public string $name = "x";
来源：http://pom.jinyuanbaomall.cn

JS:   this.name = "x";
来源：http://rrj.yfazqb.com

TS:   name: string = "x";
来源：http://xnz.snrcjt.cn

Java: private String name;
来源：http://rng.hammf.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ggg.vehdjk.com

Ruby: @name = "x"
来源：http://blz.svipenyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://tde.xingfuxueyuan.xyz

[G04] 定义方法
来源：http://jgl.yuxming.cn

Py:   def greet(self): return self.name
来源：http://aao.hfpthk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hse.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://cye.yonumen.top

TS:   greet(): string { return this.name; }
来源：http://vem.xinyue.icu

Java: String greet() { return name; }
来源：http://hyb.fanxiaobao.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://jxn.pycfn.com

Ruby: def greet; @name; end
来源：http://ruv.shanyushiyangkeji.top

C#:   public string Greet() => Name;
来源：http://qfa.cucudq.cn

[G05] 继承
来源：http://nqb.yueranfly.top

Py:   class Admin(User): pass
来源：http://lbo.nanxuanxn.top

PHP:  class Admin extends User {}
来源：http://yqo.fanxiaobao.xyz

JS:   class Admin extends User {}
来源：http://zde.c1oappe.top

TS:   class Admin extends User {}
来源：http://pju.sufxvd.cn

Java: class Admin extends User {}
来源：http://dit.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://azl.ybcxt.top

Ruby: class Admin < User; end
来源：http://oka.gotoacloud.top

C#:   class Admin : User {}
来源：http://ymg.yj202588.top

[G06] 重写方法
来源：http://ewf.snrcjt.cn

Py:   def greet(self): return "admin"
来源：http://udg.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pej.wangdashe.top

JS:   greet() { return "admin"; }
来源：http://oco.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://kqg.jqgufenzy.top

Java: @Override String greet() { return "admin"; }
来源：http://wnt.c1oappe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dzj.zdbjq.cn

Ruby: def greet; "admin"; end
来源：http://irg.zhijiandao.cn

C#:   public override string Greet() => "admin";
来源：http://fwm.mhx1999.top

[G07] 调用父类方法
来源：http://ghr.zdbjq.cn

Py:   super().greet()
来源：http://yhs.yuanzhike.top

PHP:  parent::greet();
来源：http://lni.epnwcf.com

JS:   super.greet();
来源：http://bzr.daxiang520.top

TS:   super.greet();
来源：http://azv.fehbvm.com

Java: super.greet();
来源：http://gqp.yfazqb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://opo.hcnkem.com

Ruby: super
来源：http://cdk.haohaochexian.top

C#:   base.Greet();
来源：http://bva.sweek.top

[G08] 静态方法与属性
来源：http://lvi.jinyuanbaomall.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hfm.tianlin.xyz

PHP:  public static function f() {}
来源：http://xzk.zdqjudy.top

JS:   static f() {}
来源：http://tcj.feifeiyinyue.top

TS:   static f(): void {}
来源：http://nzp.9152youxi.cn

Java: static void f() {}
来源：http://qzw.hnqzz.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://khs.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://djp.wangdashe.top

C#:   public static void F() {}
来源：http://qwg.ctjpmb.com

[G09] 接口 / 抽象类
来源：http://dba.aizwys.cn

Py:   from abc import ABC, abstractmethod
来源：http://yzp.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://zpy.daxiang520.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://czq.nanxuanxn.top

TS:   interface Shape { area(): number; }
来源：http://lxw.sweek.top

Java: interface Shape { double area(); }
来源：http://aiz.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://tyy.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aap.jinghuilouyu.cn

C#:   interface IShape { double Area(); }
来源：http://wix.52xcode.cn

[G10] 访问控制
来源：http://fqb.gotoacloud.top

Py:   约定 _protected / __private（不强制）
来源：http://pqo.cheryme.top

PHP:  public / protected / private
来源：http://bdb.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://awk.fanxiaobao.xyz

TS:   public / protected / private
来源：http://pxq.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://kup.gogol.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cle.guowangkeji.top

Ruby: public / protected / private
来源：http://poi.fanxiaobao.xyz

C#:   public / protected / private / internal
来源：http://pei.pengpengdd.cyou

[G11] getter / setter
来源：http://cys.cdnleiting.top

Py:   @property 与 @x.setter
来源：http://gpw.chenlongwang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wfu.gogol.net.cn

JS:   get name() { return this._name; }
来源：http://ynr.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://bnw.yonumen.top

Java: public String getName() { return name; }
来源：http://vop.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://deb.nanxuanxn.top

Ruby: attr_accessor :name
来源：http://dsa.hnqzz.top

C#:   public string Name { get; set; }
来源：http://vbm.ivvv.top

[G12] 对象转字符串
来源：http://abf.zhixingplan.top

Py:   def __str__(self): return self.name
来源：http://iib.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://nia.smart0.xyz

JS:   toString() { return this.name; }
来源：http://nzk.hysaishi.cn

TS:   toString(): string { return this.name; }
来源：http://lmo.hcnkem.com

Java: @Override public String toString() { return name; }
来源：http://sdn.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://cze.ydjk.org.cn

Ruby: def to_s; @name; end
来源：http://btr.meibo888.top

C#:   public override string ToString() => Name;
来源：http://lod.shanyushiyangkeji.top

[G13] 判断对象类型
来源：http://ibj.yj20258888.top

Py:   isinstance(u, User)
来源：http://jtv.316326.xyz

PHP:  $u instanceof User
来源：http://iji.9152youxi.cn

JS:   u instanceof User
来源：http://lwo.haohaochexian.top

TS:   u instanceof User
来源：http://ame.shangyingyoupin.top

Java: u instanceof User
来源：http://ddv.yj20258888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://swv.hesvh.cn

Ruby: u.is_a?(User)
来源：http://oeu.sufxvd.cn

C#:   u is User
来源：http://scg.yj20258888.top

[G14] 数据类 / record
来源：http://sok.daxiang520.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ouo.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://yws.meibo888.top

JS:   // 无内置：普通类或对象字面量
来源：http://fol.fengsongda.top

TS:   type User = { name: string; age: number };
来源：http://uaw.smart0.xyz

Java: record User(String name, int age) {}
来源：http://rqx.vehdjk.com

Go:   type User struct { Name string; Age int }
来源：http://xzp.ivvv.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lur.andypj.xyz

C#:   record User(string Name, int Age);
来源：http://hvj.nwbrower.top

[G15] 枚举
来源：http://iav.316326.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wtl.fzhhl.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lks.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dej.ppjwa.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ghf.fehbvm.com

Java: enum Color { RED, GREEN }
来源：http://asy.fengsongda.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ids.hywenlv.cn

Ruby: Color = %i[red green].freeze
来源：http://sdy.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zkq.aizwys.cn

[G16] 对象转数组 / 字典
来源：http://fvv.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rkg.yj202588.top

PHP:  get_object_vars($obj);
来源：http://ddv.cqqwz.cn

JS:   Object.entries(obj)
来源：http://akt.haohaochexian.top

TS:   Object.entries(obj)
来源：http://sny.snrcjt.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fcl.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zfz.316326.xyz

Ruby: obj.instance_variables
来源：http://hdi.dashuyun.cn

C#:   // 用反射或 System.Text.Json
来源：http://sdx.zhongyouzk.top

================================================================================
来源：http://wox.havefunace.top

H. 异常与错误处理
来源：http://jcf.yangfankeji.com

================================================================================
来源：http://xbn.birdmap.top

[H01] try / catch 基础
来源：http://pyg.tanke756.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qre.snrcjt.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jip.xinyue.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iph.jqgufenzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nsx.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dri.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kus.guannengcc.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qyw.cheryme.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xev.yongpay.top

[H02] finally / ensure 收尾
来源：http://vxl.yvedp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bov.epnwcf.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://jkq.quarkkingdee.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wum.xingfuxueyuan.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://kxt.cucudq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qth.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://grs.meibo888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kal.daria6918.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mof.bbcook.cn

[H03] 主动抛出异常
来源：http://jan.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://wgc.ppjwa.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cvu.meibo888.top

JS:   throw new Error("错误信息");
来源：http://icq.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://dnx.daria6918.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kkx.kuanghao11.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bue.aizwys.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://epl.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://qpy.aizwys.cn

[H04] 自定义异常类型
来源：http://eyk.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://wtc.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://kye.xylfe.cn

JS:   class MyError extends Error {}
来源：http://scw.316326.xyz

TS:   class MyError extends Error {}
来源：http://ubw.316326.xyz

Java: class MyException extends RuntimeException {}
来源：http://lsm.chenlongwang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gwt.yonumen.top

Ruby: class MyError < StandardError; end
来源：http://atu.svipenyu.cn

C#:   class MyException : Exception {}
来源：http://kqw.fktsv.cn

[H05] 捕获特定类型
来源：http://hli.fengsongda.top

Py:   except ValueError as e:
来源：http://tya.hongshengwenyu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mrd.fehbvm.com

JS:   if (e instanceof TypeError) {}
来源：http://ggh.shuidangran.top

TS:   if (e instanceof TypeError) {}
来源：http://akr.kuanghao11.cn

Java: catch (IOException | SQLException e) {}
来源：http://vnb.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iri.sysykeji.top

Ruby: rescue ArgumentError => e
来源：http://iak.iojbl.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vhr.52xcode.cn

[H06] 可选值 / 空值安全访问
来源：http://wal.zhixingplan.top

Py:   value = d.get("k") or default
来源：http://rvo.gzhubu.top

PHP:  $v = $d["k"] ?? null;
来源：http://rwp.jinghuilouyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rjv.hfpthk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://khv.cheryme.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ztf.fzhhl.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wsw.zhaomingkeji.xyz

Ruby: d&.dig(:a, :b)
来源：http://mlm.cqqwz.cn

C#:   obj?.A?.B ?? default
来源：http://cfh.jqgufenzy.top

[H07] 断言
来源：http://dgr.316326.xyz

Py:   assert x > 0, "必须为正"
来源：http://tzf.zhixingplan.top

PHP:  assert($x > 0);
来源：http://qmo.nanxinkj.top

JS:   console.assert(x > 0);
来源：http://okx.jinqigfzy.top

TS:   console.assert(x > 0);
来源：http://fcz.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://prm.sufxvd.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qrq.havefunace.top

Ruby: raise "必须为正" unless x > 0
来源：http://xhj.yangfankeji.com

C#:   Debug.Assert(x > 0);
来源：http://gtq.zhixingplan.top

[H08] 获取错误信息与堆栈
来源：http://wlu.yj20258.top

Py:   str(e);  traceback.format_exc()
来源：http://nxk.hcnkem.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bcq.chenjidiqi.icu

JS:   e.message;  e.stack
来源：http://pkz.redwolf501.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://djq.yj20258.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ygk.jinqigfzy.top

Go:   err.Error()
来源：http://rzg.fengsongda.top

Ruby: e.message;  e.backtrace
来源：http://pyx.shangyingyoupin.top

C#:   e.Message;  e.StackTrace
来源：http://roi.fzhhl.top

[H09] 带错误码的异常
来源：http://puc.jinyuanbaomall.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ioy.feifeiyinyue.top


<!-- 参考信息 -->