代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://zuw.ppjwa.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://flh.guowangkeji.top

PHP:  file_exists("a.txt");
来源：http://vdl.svipenyu.cn

JS:   fs.existsSync("a.txt")
来源：http://lpm.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://csh.sjlbkw.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jjm.ctjpmb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hve.yangfankeji.com

Ruby: File.exist?("a.txt")
来源：http://arz.zdqjudy.top

C#:   File.Exists("a.txt")
来源：http://uvq.feifeiyinyue.top

[F06] 删除文件
来源：http://sdd.tarul.cn

Py:   os.remove("a.txt")
来源：http://dpp.meibo888.top

PHP:  unlink("a.txt");
来源：http://hjp.c1oappe.top

JS:   fs.unlinkSync("a.txt")
来源：http://uou.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://ric.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ujg.bbcook.cn

Go:   os.Remove("a.txt")
来源：http://cbg.cqqwz.cn

Ruby: File.delete("a.txt")
来源：http://xme.jinghuilouyu.cn

C#:   File.Delete("a.txt");
来源：http://sxn.fengsongda.top

[F07] 创建目录（含多级）
来源：http://gqe.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ldf.cucudq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dqq.yanxiufei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ssv.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iuz.sweek.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wyt.tianlin.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pon.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uzl.ctjpmb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ttw.yueranfly.top

[F08] 遍历目录
来源：http://bqe.bbcook.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dto.jqgufenzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dsv.nwbrower.top

JS:   fs.readdirSync("dir")
来源：http://yij.haohaochexian.top

TS:   fs.readdirSync("dir")
来源：http://igl.yfazqb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qow.dashuyun.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hao.nwbrower.top

Ruby: Dir.children("dir")
来源：http://oxl.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://gmq.bjfxy.top

[F09] 获取文件大小
来源：http://jze.9152youxi.cn

Py:   os.path.getsize("a.txt")
来源：http://cor.zycfv.cn

PHP:  filesize("a.txt");
来源：http://qwv.sweek.top

JS:   fs.statSync("a.txt").size
来源：http://kgc.aizwys.cn

TS:   fs.statSync("a.txt").size
来源：http://gar.zhoulong.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://jbc.ehwqpu.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lsj.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://pvo.cucudq.cn

C#:   new FileInfo("a.txt").Length
来源：http://wih.shangyingyoupin.top

[F10] 取文件扩展名 / 文件名
来源：http://rsc.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pdz.jqgufenzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://crj.cucudq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sye.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://myq.nwbrower.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hfv.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://khn.guowangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oyw.ppjwa.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://put.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://wze.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cvg.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nfh.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cij.nwbrower.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://upo.xuanzx.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bhi.aizwys.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nht.zhongyouzk.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eyq.nanxuanxn.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cvs.ctjpmb.com

[F12] CSV 读写
来源：http://wzp.shanyushiyangtech.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://awb.chenzaomai.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sbq.nanxinkj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sln.jiagoushi.top

TS:   // 同上
来源：http://gkw.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uie.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dze.jiagoushi.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ldi.yueranfly.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ivn.mhx1999.top

================================================================================
来源：http://ipf.ppjwa.cn

G. 面向对象
来源：http://tam.jinghuilouyu.cn

================================================================================
来源：http://ngg.hammf.cn

[G01] 定义类
来源：http://dwl.mhx1999.top

Py:   class User: pass
来源：http://bng.hongshengwenyu.top

PHP:  class User {}
来源：http://zty.havefunace.top

JS:   class User {}
来源：http://rgd.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://str.yj20258.top

Java: class User {}
来源：http://tca.sufxvd.cn

Go:   type User struct { Name string }
来源：http://hme.hywenlv.cn

Ruby: class User; end
来源：http://suy.shanyushiyangkeji.top

C#:   class User {}
来源：http://qsx.yvedp.cn

[G02] 构造函数
来源：http://mwg.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://ioh.jinyuanbaomall.cn

PHP:  public function __construct(public string $name) {}
来源：http://hbb.wangshuangyany.cn

JS:   constructor(name) { this.name = name; }
来源：http://biv.sxryk.cn

TS:   constructor(public name: string) {}
来源：http://ghl.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://mdr.sufxvd.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tvr.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://hog.ydzc1.top

C#:   public User(string name) { Name = name; }
来源：http://xoo.pengpengdd.cyou

[G03] 实例属性
来源：http://hqc.yj20258888.top

Py:   self.name = "x"
来源：http://cma.ehwqpu.com

PHP:  public string $name = "x";
来源：http://wjt.yueranfly.top

JS:   this.name = "x";
来源：http://wzq.cucudq.cn

TS:   name: string = "x";
来源：http://qzu.fanxiaobao.xyz

Java: private String name;
来源：http://onw.shanyushiyangtech.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vhb.bjfxy.top

Ruby: @name = "x"
来源：http://nyh.316326.xyz

C#:   public string Name { get; set; } = "x";
来源：http://sji.fehbvm.com

[G04] 定义方法
来源：http://kwx.havefunace.top

Py:   def greet(self): return self.name
来源：http://zko.aizwys.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lbr.haohaochexian.top

JS:   greet() { return this.name; }
来源：http://ppq.fzhhl.top

TS:   greet(): string { return this.name; }
来源：http://osu.xinyue.icu

Java: String greet() { return name; }
来源：http://wtp.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zlb.yuxming.cn

Ruby: def greet; @name; end
来源：http://hrl.chenjidiqi.icu

C#:   public string Greet() => Name;
来源：http://lek.ywan-chungtsiang.top

[G05] 继承
来源：http://buc.jqgufenzy.top

Py:   class Admin(User): pass
来源：http://kei.shanyushiyangkeji.top

PHP:  class Admin extends User {}
来源：http://mcy.yfazqb.com

JS:   class Admin extends User {}
来源：http://jmk.vehdjk.com

TS:   class Admin extends User {}
来源：http://qhs.sysykeji.top

Java: class Admin extends User {}
来源：http://ytz.shanyushiyangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hyg.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://gwx.sufxvd.cn

C#:   class Admin : User {}
来源：http://ccv.nanxuanxn.top

[G06] 重写方法
来源：http://ktr.xingfuxueyuan.xyz

Py:   def greet(self): return "admin"
来源：http://jam.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://byc.jinghuilouyu.cn

JS:   greet() { return "admin"; }
来源：http://nap.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://wha.guannengcc.top

Java: @Override String greet() { return "admin"; }
来源：http://hpz.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bar.jqgufenzy.top

Ruby: def greet; "admin"; end
来源：http://fed.kuanghao11.cn

C#:   public override string Greet() => "admin";
来源：http://tty.daria6918.cn

[G07] 调用父类方法
来源：http://ior.fzhhl.top

Py:   super().greet()
来源：http://okj.guannengcc.top

PHP:  parent::greet();
来源：http://hiu.daria6918.cn

JS:   super.greet();
来源：http://nvm.jyoumei.cn

TS:   super.greet();
来源：http://wsk.tarul.cn

Java: super.greet();
来源：http://geo.yfazqb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://duj.bbcook.cn

Ruby: super
来源：http://zdt.zhixingplan.top

C#:   base.Greet();
来源：http://qhh.tianlin.xyz

[G08] 静态方法与属性
来源：http://cji.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yuw.shangyingyoupin.top

PHP:  public static function f() {}
来源：http://gky.zdqjudy.top

JS:   static f() {}
来源：http://xcj.wangshuangyany.cn

TS:   static f(): void {}
来源：http://awg.jinyuanbaomall.cn

Java: static void f() {}
来源：http://tgb.jinyuanbaomall.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cmx.yanxiufei.cn

Ruby: def self.f; end
来源：http://bei.chenlongwang.top

C#:   public static void F() {}
来源：http://cgi.zhixingplan.top

[G09] 接口 / 抽象类
来源：http://wxe.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://mvd.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://ikv.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://gfl.zhengqikj.top

TS:   interface Shape { area(): number; }
来源：http://pkt.tianlin.xyz

Java: interface Shape { double area(); }
来源：http://xsp.zdbjq.cn

Go:   type Shape interface { Area() float64 }
来源：http://vqk.xingfuxueyuan.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ddi.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://liw.xuanzx.com

[G10] 访问控制
来源：http://vmk.jqgufenzy.top

Py:   约定 _protected / __private（不强制）
来源：http://jiz.hfpthk.cn

PHP:  public / protected / private
来源：http://fzj.hcnkem.com

JS:   #private 字段；其余公开
来源：http://omf.ctjpmb.com

TS:   public / protected / private
来源：http://zzl.hongshengwenyu.top

Java: public / protected / private / 默认包级
来源：http://fbe.cucudq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://oji.xylfe.cn

Ruby: public / protected / private
来源：http://kzg.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://tla.zhaomingkeji.xyz

[G11] getter / setter
来源：http://byc.epnwcf.com

Py:   @property 与 @x.setter
来源：http://ohy.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tdo.zdbjq.cn

JS:   get name() { return this._name; }
来源：http://wcc.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://awe.gaohongyu789.top

Java: public String getName() { return name; }
来源：http://kzd.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nkl.yuanzhike.top

Ruby: attr_accessor :name
来源：http://evi.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://ebs.sysykeji.top

[G12] 对象转字符串
来源：http://ema.aibaodan.cn

Py:   def __str__(self): return self.name
来源：http://xze.redwolf501.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wph.sysykeji.top

JS:   toString() { return this.name; }
来源：http://vpn.yfazqb.com

TS:   toString(): string { return this.name; }
来源：http://yny.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://bvm.daria6918.cn

Go:   func (u User) String() string { return u.Name }
来源：http://diq.hesvh.cn

Ruby: def to_s; @name; end
来源：http://awx.vqdsnc.cn

C#:   public override string ToString() => Name;
来源：http://ebk.yanxiufei.cn

[G13] 判断对象类型
来源：http://dvi.fktsv.cn

Py:   isinstance(u, User)
来源：http://eur.cqqwz.cn

PHP:  $u instanceof User
来源：http://puq.wangdashe.top

JS:   u instanceof User
来源：http://ckc.fehbvm.com

TS:   u instanceof User
来源：http://dee.dashuyun.cn

Java: u instanceof User
来源：http://brs.yj202588.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yoy.redwolf501.top

Ruby: u.is_a?(User)
来源：http://xfd.zycfv.cn

C#:   u is User
来源：http://xuv.jqgufenzy.top

[G14] 数据类 / record
来源：http://mys.jqgufenzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hfl.yanxiufei.cn

PHP:  // 用 readonly 属性模拟
来源：http://bul.jlsjyb.cn

JS:   // 无内置：普通类或对象字面量
来源：http://khi.daria6918.cn

TS:   type User = { name: string; age: number };
来源：http://kti.mhx1999.top

Java: record User(String name, int age) {}
来源：http://pcw.mhx1999.top

Go:   type User struct { Name string; Age int }
来源：http://vve.jinyuanbaomall.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://txe.hywenlv.cn

C#:   record User(string Name, int Age);
来源：http://obo.quarkkingdee.top

[G15] 枚举
来源：http://xwr.zdqjudy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bvd.sweek.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://itt.nanxuanxn.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mnn.meibo888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bzt.smart0.xyz

Java: enum Color { RED, GREEN }
来源：http://far.zhiwuduotai.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fmz.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://xcz.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jmk.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://aeh.cashguo.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hly.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://aap.zdbjq.cn

JS:   Object.entries(obj)
来源：http://ajl.jiagoushi.top

TS:   Object.entries(obj)
来源：http://fjh.cashguo.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kgb.hesvh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://uto.pengpengdd.cyou

Ruby: obj.instance_variables
来源：http://lqg.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://byo.nanxuanxn.top

================================================================================
来源：http://axe.jiagoushi.top

H. 异常与错误处理
来源：http://cez.sufxvd.cn

================================================================================
来源：http://bvl.jianghu66.top

[H01] try / catch 基础
来源：http://zzn.ivvv.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://maz.yuanzhike.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bin.havefunace.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pis.hesvh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fuy.gogol.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ibv.chenjidiqi.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qbd.hysaishi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nlj.andypj.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ski.cucudq.cn

[H02] finally / ensure 收尾
来源：http://zms.yangfankeji.com

Py:   try: f()⏎finally: cleanup()
来源：http://mhp.hesvh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://irv.ydjk.org.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iyf.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://vqe.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://heh.xingfuxueyuan.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://jbp.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wmz.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pvd.daria6918.cn

[H03] 主动抛出异常
来源：http://veb.mhx1999.top

Py:   raise ValueError("错误信息")
来源：http://ykz.daria6918.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ntf.ydjk.org.cn

JS:   throw new Error("错误信息");
来源：http://foy.yuxming.cn

TS:   throw new Error("错误信息");
来源：http://svr.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://grh.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ery.vqdsnc.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fgy.fanxiaobao.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://mgw.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://jkr.yongpay.top

Py:   class MyError(Exception): pass
来源：http://aoo.jyoumei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zou.daxiang520.top

JS:   class MyError extends Error {}
来源：http://btr.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://lme.zhaomingkeji.xyz

Java: class MyException extends RuntimeException {}
来源：http://naf.jlsjyb.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nlr.wangdashe.top

Ruby: class MyError < StandardError; end
来源：http://efa.meibo888.top

C#:   class MyException : Exception {}
来源：http://zxo.bjfxy.top

[H05] 捕获特定类型
来源：http://ccb.jinqigfzy.top

Py:   except ValueError as e:
来源：http://nnr.hammf.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qnl.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://fqw.tian-w.cn

TS:   if (e instanceof TypeError) {}
来源：http://urc.9152youxi.cn

Java: catch (IOException | SQLException e) {}
来源：http://tyl.zycfv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ceu.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://pnr.vehdjk.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sex.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://vfx.cdnleiting.top

Py:   value = d.get("k") or default
来源：http://dtr.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://ghq.xinyue.icu

JS:   obj?.a?.b;  d ?? default
来源：http://oqn.nanxuanxn.top

TS:   obj?.a?.b;  d ?? default
来源：http://fju.shanyushiyangtech.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zel.cashguo.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lqf.cqqwz.cn

Ruby: d&.dig(:a, :b)
来源：http://anc.yj202588.top

C#:   obj?.A?.B ?? default
来源：http://nkw.dashuyun.cn

[H07] 断言
来源：http://obp.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://hsa.jianghu66.top

PHP:  assert($x > 0);
来源：http://hvy.zhengqikj.top

JS:   console.assert(x > 0);
来源：http://nzk.hesvh.cn

TS:   console.assert(x > 0);
来源：http://wcg.redwolf501.top

Java: assert x > 0 : "必须为正";
来源：http://vrq.tarul.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rre.cdnleiting.top

Ruby: raise "必须为正" unless x > 0
来源：http://yel.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://yzb.yueranfly.top

[H08] 获取错误信息与堆栈
来源：http://bzz.kuanghao11.cn

Py:   str(e);  traceback.format_exc()
来源：http://kvt.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dti.haohaochexian.top

JS:   e.message;  e.stack
来源：http://gxo.yongpay.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zgn.hfpthk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://stl.jianghu66.top

Go:   err.Error()
来源：http://qnp.xuetiantiany.cn

Ruby: e.message;  e.backtrace
来源：http://gch.ydzc1.top

C#:   e.Message;  e.StackTrace
来源：http://nxv.hysaishi.cn

[H09] 带错误码的异常
来源：http://jqn.guannengcc.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hjw.shanyushiyangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bva.shanyushiyangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://huj.cheryme.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mes.nanxuanxn.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zla.zhongyouzk.top


<!-- 参考信息 -->