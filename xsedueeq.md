代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kgp.yj20258.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bas.xuanzx.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kqg.wangshuangyany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xdb.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dcs.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://njb.nanxuanxn.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://npn.yueranfly.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cjt.jiagoushi.top

[F05] 判断文件或目录是否存在
来源：http://cvi.yvedp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hks.fzhhl.top

PHP:  file_exists("a.txt");
来源：http://lxi.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://ycf.feifeiyinyue.top

TS:   fs.existsSync("a.txt")
来源：http://xbk.ivvv.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lco.ppjwa.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mcp.fzhhl.top

Ruby: File.exist?("a.txt")
来源：http://hzv.hammf.cn

C#:   File.Exists("a.txt")
来源：http://ham.snrcjt.cn

[F06] 删除文件
来源：http://wev.yuanzhike.top

Py:   os.remove("a.txt")
来源：http://oie.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://dbj.fktsv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://osj.wangshuangyany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tvu.sufxvd.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dvi.sweek.top

Go:   os.Remove("a.txt")
来源：http://chz.dashuyun.cn

Ruby: File.delete("a.txt")
来源：http://bcs.cqqwz.cn

C#:   File.Delete("a.txt");
来源：http://gkf.yonumen.top

[F07] 创建目录（含多级）
来源：http://jft.sysykeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fcz.guowangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pwa.fktsv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rfu.chenzaomai.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bia.jianghu66.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://deu.feifeiyinyue.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yao.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://syx.hcnkem.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fph.havefunace.top

[F08] 遍历目录
来源：http://xzy.yueranfly.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wmw.fzhhl.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ntw.jinqigufen.top

JS:   fs.readdirSync("dir")
来源：http://lwj.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://eht.andypj.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://epf.andypj.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://aea.zdbjq.cn

Ruby: Dir.children("dir")
来源：http://era.daxiang520.top

C#:   Directory.GetFiles("dir")
来源：http://ako.wangdashe.top

[F09] 获取文件大小
来源：http://qbv.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://wou.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://uyz.9152youxi.cn

JS:   fs.statSync("a.txt").size
来源：http://swb.daxiang520.top

TS:   fs.statSync("a.txt").size
来源：http://wtc.hcnkem.com

Java: Files.size(Path.of("a.txt"))
来源：http://qpn.zhixingplan.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xvg.sweek.top

Ruby: File.size("a.txt")
来源：http://jci.yangfankeji.com

C#:   new FileInfo("a.txt").Length
来源：http://fxw.hywenlv.cn

[F10] 取文件扩展名 / 文件名
来源：http://cgl.andypj.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vdj.chenlongwang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://obp.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mpm.cqqwz.cn

TS:   path.extname("a.txt")
来源：http://szp.jinyuanbaomall.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hwl.xingfuxueyuan.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lxs.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gep.pycfn.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bmg.bbcook.cn

[F11] 复制与移动文件
来源：http://ubl.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dht.cashguo.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hpq.fanxiaobao.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yly.daxiang520.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cdm.ivvv.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hps.fehbvm.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oky.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cts.gzhubu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mlx.smart0.xyz

[F12] CSV 读写
来源：http://dga.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lwd.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zij.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://joj.fanxiaobao.xyz

TS:   // 同上
来源：http://ncm.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ofg.hesvh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dai.sjlbkw.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jox.ppjwa.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sss.aizwys.cn

================================================================================
来源：http://jbe.yangfankeji.com

G. 面向对象
来源：http://tfr.havefunace.top

================================================================================
来源：http://jjr.ivvv.top

[G01] 定义类
来源：http://tps.birdmap.top

Py:   class User: pass
来源：http://feh.pengpengdd.cyou

PHP:  class User {}
来源：http://lem.gaohongyu789.top

JS:   class User {}
来源：http://mvy.hfpthk.cn

TS:   class User { name: string = ""; }
来源：http://gau.zdqjudy.top

Java: class User {}
来源：http://rgf.tarul.cn

Go:   type User struct { Name string }
来源：http://gbv.cqqwz.cn

Ruby: class User; end
来源：http://hrw.jyoumei.cn

C#:   class User {}
来源：http://nxw.bbcook.cn

[G02] 构造函数
来源：http://fdd.tanke756.top

Py:   def __init__(self, name): self.name = name
来源：http://ukh.shanyushiyangtech.top

PHP:  public function __construct(public string $name) {}
来源：http://ydu.bbcook.cn

JS:   constructor(name) { this.name = name; }
来源：http://att.yj20258.top

TS:   constructor(public name: string) {}
来源：http://iov.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://grz.daria6918.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jyf.0kj1m.cn

Ruby: def initialize(name); @name = name; end
来源：http://dvj.bbcook.cn

C#:   public User(string name) { Name = name; }
来源：http://tgz.jinqigfzy.top

[G03] 实例属性
来源：http://wfh.yvedp.cn

Py:   self.name = "x"
来源：http://yoq.hcnkem.com

PHP:  public string $name = "x";
来源：http://oto.xinyue.icu

JS:   this.name = "x";
来源：http://byq.sjlbkw.cn

TS:   name: string = "x";
来源：http://tgn.daria6918.cn

Java: private String name;
来源：http://wdi.fanxiaobao.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ybv.yueranfly.top

Ruby: @name = "x"
来源：http://orv.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://ism.guowangkeji.top

[G04] 定义方法
来源：http://dwa.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://zzz.tarul.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://daz.smart0.xyz

JS:   greet() { return this.name; }
来源：http://yqr.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://avb.yj202588.top

Java: String greet() { return name; }
来源：http://dqf.nanxinkj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kna.yanxiufei.cn

Ruby: def greet; @name; end
来源：http://qym.sxryk.cn

C#:   public string Greet() => Name;
来源：http://gun.nwbrower.top

[G05] 继承
来源：http://dqk.sysykeji.top

Py:   class Admin(User): pass
来源：http://cju.hesvh.cn

PHP:  class Admin extends User {}
来源：http://zsg.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://wvb.zhaomingkeji.xyz

TS:   class Admin extends User {}
来源：http://pfq.ydzc1.top

Java: class Admin extends User {}
来源：http://tmj.shzxlz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cbq.tian-w.cn

Ruby: class Admin < User; end
来源：http://woa.ivvv.top

C#:   class Admin : User {}
来源：http://kel.ydjk.org.cn

[G06] 重写方法
来源：http://rax.vqdsnc.cn

Py:   def greet(self): return "admin"
来源：http://gzy.sxryk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rwr.yj20258.top

JS:   greet() { return "admin"; }
来源：http://tuo.mhx1999.top

TS:   greet(): string { return "admin"; }
来源：http://ppe.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://jcp.havefunace.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vbv.yj20258.top

Ruby: def greet; "admin"; end
来源：http://fav.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://dpr.yuanzhike.top

[G07] 调用父类方法
来源：http://wom.snrcjt.cn

Py:   super().greet()
来源：http://pyt.bbcook.cn

PHP:  parent::greet();
来源：http://unw.jiagoushi.top

JS:   super.greet();
来源：http://xbf.hesvh.cn

TS:   super.greet();
来源：http://lje.fengsongda.top

Java: super.greet();
来源：http://anl.gotoacloud.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xal.ivvv.top

Ruby: super
来源：http://voo.cqqwz.cn

C#:   base.Greet();
来源：http://ifg.jqgfzy.top

[G08] 静态方法与属性
来源：http://xvt.9152youxi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aba.tian-w.cn

PHP:  public static function f() {}
来源：http://yqs.bjfxy.top

JS:   static f() {}
来源：http://tvd.dianchejie.cn

TS:   static f(): void {}
来源：http://nxf.meibo888.top

Java: static void f() {}
来源：http://smz.aibaodan.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gni.jinyuanbaomall.cn

Ruby: def self.f; end
来源：http://rvm.wangshuangyany.cn

C#:   public static void F() {}
来源：http://xcm.hnqzz.top

[G09] 接口 / 抽象类
来源：http://mvt.tian-w.cn

Py:   from abc import ABC, abstractmethod
来源：http://xwl.jyoumei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gui.yvedp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dca.ppjwa.cn

TS:   interface Shape { area(): number; }
来源：http://cmj.svipenyu.cn

Java: interface Shape { double area(); }
来源：http://qih.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://iye.daxiang520.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://srh.yj20258888.top

C#:   interface IShape { double Area(); }
来源：http://tat.hcnkem.com

[G10] 访问控制
来源：http://ecq.tianlin.xyz

Py:   约定 _protected / __private（不强制）
来源：http://ouz.dianchejie.cn

PHP:  public / protected / private
来源：http://dnu.andypj.xyz

JS:   #private 字段；其余公开
来源：http://unq.cqqwz.cn

TS:   public / protected / private
来源：http://odv.gaohongyu789.top

Java: public / protected / private / 默认包级
来源：http://xaj.xinyue.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://vig.wangdashe.top

Ruby: public / protected / private
来源：http://rqe.ivvv.top

C#:   public / protected / private / internal
来源：http://fab.fanxiaobao.xyz

[G11] getter / setter
来源：http://tzp.wangdashe.top

Py:   @property 与 @x.setter
来源：http://ryv.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ezl.aibaodan.cn

JS:   get name() { return this._name; }
来源：http://luo.jqgfzy.top

TS:   get name(): string { return this._name; }
来源：http://nst.vehdjk.com

Java: public String getName() { return name; }
来源：http://ynd.cdnleiting.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tma.kuanghao11.cn

Ruby: attr_accessor :name
来源：http://sph.jianghu66.top

C#:   public string Name { get; set; }
来源：http://ftm.jyoumei.cn

[G12] 对象转字符串
来源：http://ecq.hammf.cn

Py:   def __str__(self): return self.name
来源：http://fly.ctjpmb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://qdv.52xcode.cn

JS:   toString() { return this.name; }
来源：http://qow.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://sdb.ppjwa.cn

Java: @Override public String toString() { return name; }
来源：http://wqy.fengsongda.top

Go:   func (u User) String() string { return u.Name }
来源：http://fqo.guannengcc.top

Ruby: def to_s; @name; end
来源：http://bly.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://ygv.0kj1m.cn

[G13] 判断对象类型
来源：http://lds.aibaodan.cn

Py:   isinstance(u, User)
来源：http://oam.quarkkingdee.top

PHP:  $u instanceof User
来源：http://sgq.jianghu66.top

JS:   u instanceof User
来源：http://kvx.hysaishi.cn

TS:   u instanceof User
来源：http://acl.jlsjyb.cn

Java: u instanceof User
来源：http://qlg.xinyue.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://xur.daxiang520.top

Ruby: u.is_a?(User)
来源：http://lnq.fzhhl.top

C#:   u is User
来源：http://pbb.zhoulong.xyz

[G14] 数据类 / record
来源：http://azw.jyoumei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dkh.yj20258888.top

PHP:  // 用 readonly 属性模拟
来源：http://zdc.cucudq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://irv.haohaochexian.top

TS:   type User = { name: string; age: number };
来源：http://cpv.zhoulong.xyz

Java: record User(String name, int age) {}
来源：http://eei.redwolf501.top

Go:   type User struct { Name string; Age int }
来源：http://mzk.bbcook.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rhb.chenzaomai.com

C#:   record User(string Name, int Age);
来源：http://wdv.daxiang520.top

[G15] 枚举
来源：http://ikz.hysaishi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://drr.svipenyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bnp.yj202588.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gai.zhaomingkeji.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gqy.ydjk.org.cn

Java: enum Color { RED, GREEN }
来源：http://myb.zhixingplan.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pwr.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://kli.chenzaomai.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xty.c1oappe.top

[G16] 对象转数组 / 字典
来源：http://zrp.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://plz.fehbvm.com

PHP:  get_object_vars($obj);
来源：http://qbg.ctjpmb.com

JS:   Object.entries(obj)
来源：http://tmj.hcnkem.com

TS:   Object.entries(obj)
来源：http://wqi.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jfx.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vkv.xuanzx.com

Ruby: obj.instance_variables
来源：http://wzj.ybcxt.top

C#:   // 用反射或 System.Text.Json
来源：http://jwz.9152youxi.cn

================================================================================
来源：http://vmc.sxryk.cn

H. 异常与错误处理
来源：http://cwo.smart0.xyz

================================================================================
来源：http://ixk.xingfuxueyuan.xyz

[H01] try / catch 基础
来源：http://sww.yangfankeji.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://idz.fzhhl.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pde.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rgl.yuxming.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rak.vqdsnc.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eoq.xziqi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hnp.52xcode.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vrb.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://szb.yonumen.top

[H02] finally / ensure 收尾
来源：http://ngt.hywenlv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nwt.kuanghao11.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xjk.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jrh.yj202588.top

TS:   try { f(); } finally { cleanup(); }
来源：http://eio.9152youxi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qah.hammf.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nhw.gaohongyu789.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fwc.cashguo.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wwu.guowangkeji.top

[H03] 主动抛出异常
来源：http://zfo.zhijiandao.cn

Py:   raise ValueError("错误信息")
来源：http://ete.jiagoushi.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bik.jinghuilouyu.cn

JS:   throw new Error("错误信息");
来源：http://omt.hammf.cn

TS:   throw new Error("错误信息");
来源：http://way.quarkkingdee.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://iyz.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://joc.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jah.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lsy.nwbrower.top

[H04] 自定义异常类型
来源：http://qhp.tianlin.xyz

Py:   class MyError(Exception): pass
来源：http://qsy.ctjpmb.com

PHP:  class MyError extends RuntimeException {}
来源：http://eyu.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://gft.fzhhl.top

TS:   class MyError extends Error {}
来源：http://zim.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://qjf.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oxi.hnqzz.top

Ruby: class MyError < StandardError; end
来源：http://sfg.zhongyouzk.top

C#:   class MyException : Exception {}
来源：http://eyv.cdnleiting.top

[H05] 捕获特定类型
来源：http://oys.9152youxi.cn

Py:   except ValueError as e:
来源：http://fon.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://skp.redwolf501.top

JS:   if (e instanceof TypeError) {}
来源：http://sym.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://rsf.jinyuanbaomall.cn

Java: catch (IOException | SQLException e) {}
来源：http://uuw.aizwys.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kfh.vehdjk.com

Ruby: rescue ArgumentError => e
来源：http://jpe.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wgv.pycfn.com

[H06] 可选值 / 空值安全访问
来源：http://mom.wangdashe.top

Py:   value = d.get("k") or default
来源：http://ivh.quarkkingdee.top

PHP:  $v = $d["k"] ?? null;
来源：http://htj.iojbl.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sld.chenlongwang.top

TS:   obj?.a?.b;  d ?? default
来源：http://ifv.uphjek.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sot.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://okg.shanyushiyangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://hzs.uphjek.com

C#:   obj?.A?.B ?? default
来源：http://xit.hongshengwenyu.top

[H07] 断言
来源：http://oxo.aibaodan.cn

Py:   assert x > 0, "必须为正"
来源：http://jix.tanke756.top

PHP:  assert($x > 0);
来源：http://ysr.aibaodan.cn

JS:   console.assert(x > 0);
来源：http://cmd.ivvv.top

TS:   console.assert(x > 0);
来源：http://ave.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://uxa.havefunace.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jvu.guowangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://oeu.shzxlz.cn

C#:   Debug.Assert(x > 0);
来源：http://pcf.sysykeji.top

[H08] 获取错误信息与堆栈
来源：http://dou.meibo888.top

Py:   str(e);  traceback.format_exc()
来源：http://qsp.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uid.redwolf501.top

JS:   e.message;  e.stack
来源：http://vka.fanxiaobao.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://ngp.yanxiufei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gpr.sweek.top

Go:   err.Error()
来源：http://eab.ybcxt.top


<!-- 参考信息 -->