代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://uyp.ydjk.org.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cuc.xinyue.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://afw.jiagoushi.top

Go:   os.Remove("a.txt")
来源：http://sme.svipenyu.cn

Ruby: File.delete("a.txt")
来源：http://lbg.wangshuangyany.cn

C#:   File.Delete("a.txt");
来源：http://dao.yj20258888.top

[F07] 创建目录（含多级）
来源：http://fgo.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jhz.yanxiufei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tcr.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gts.fengsongda.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dsz.tianlin.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hoc.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sal.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://opm.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ozm.bbcook.cn

[F08] 遍历目录
来源：http://bws.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://uck.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pea.fktsv.cn

JS:   fs.readdirSync("dir")
来源：http://smt.ywan-chungtsiang.top

TS:   fs.readdirSync("dir")
来源：http://xyd.c1oappe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vps.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uxa.daxiang520.top

Ruby: Dir.children("dir")
来源：http://gtq.jqgfzy.top

C#:   Directory.GetFiles("dir")
来源：http://yqr.yongpay.top

[F09] 获取文件大小
来源：http://yla.guannengcc.top

Py:   os.path.getsize("a.txt")
来源：http://jen.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://feh.havefunace.top

JS:   fs.statSync("a.txt").size
来源：http://acl.hammf.cn

TS:   fs.statSync("a.txt").size
来源：http://yae.hnxiangtu.top

Java: Files.size(Path.of("a.txt"))
来源：http://ntl.nwbrower.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gji.cheryme.top

Ruby: File.size("a.txt")
来源：http://ytg.jqgufenzy.top

C#:   new FileInfo("a.txt").Length
来源：http://xll.hysaishi.cn

[F10] 取文件扩展名 / 文件名
来源：http://gee.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mwj.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vek.bbcook.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eyv.gaohongyu789.top

TS:   path.extname("a.txt")
来源：http://jho.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vvb.sufxvd.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ser.yangfankeji.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wga.fzhhl.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fly.jinqigfzy.top

[F11] 复制与移动文件
来源：http://iug.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ldu.dashuyun.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zus.mhx1999.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ohl.hcnkem.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qsz.tanke756.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fgs.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cgw.xinyue.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pbv.xinyue.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wve.tianlin.xyz

[F12] CSV 读写
来源：http://dsw.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nbd.hcnkem.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zcj.zhongyouzk.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dqv.nanxinkj.top

TS:   // 同上
来源：http://llq.dianchejie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://chv.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zhg.daria6918.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nwk.fengsongda.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hvl.gaohongyu789.top

================================================================================
来源：http://umg.hesvh.cn

G. 面向对象
来源：http://yij.chenzaomai.com

================================================================================
来源：http://akb.vqdsnc.cn

[G01] 定义类
来源：http://dwb.jqgufenzy.top

Py:   class User: pass
来源：http://mhu.sufxvd.cn

PHP:  class User {}
来源：http://iwv.yvedp.cn

JS:   class User {}
来源：http://nru.xylfe.cn

TS:   class User { name: string = ""; }
来源：http://ymw.fktsv.cn

Java: class User {}
来源：http://yhm.0kj1m.cn

Go:   type User struct { Name string }
来源：http://evh.zhijiandao.cn

Ruby: class User; end
来源：http://teu.iojbl.cn

C#:   class User {}
来源：http://hpa.jianghu66.top

[G02] 构造函数
来源：http://xuc.sxryk.cn

Py:   def __init__(self, name): self.name = name
来源：http://blc.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://erg.shanyushiyangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://ikw.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://vay.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://szq.ybcxt.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://urv.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://cyq.wangshuangyany.cn

C#:   public User(string name) { Name = name; }
来源：http://yjf.jinyuanbaomall.cn

[G03] 实例属性
来源：http://sdj.svipenyu.cn

Py:   self.name = "x"
来源：http://qqa.52xcode.cn

PHP:  public string $name = "x";
来源：http://jup.yueranfly.top

JS:   this.name = "x";
来源：http://nrj.shanyushiyangtech.top

TS:   name: string = "x";
来源：http://qik.nanxuanxn.top

Java: private String name;
来源：http://ane.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iic.ybcxt.top

Ruby: @name = "x"
来源：http://yvq.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://ilb.bbcook.cn

[G04] 定义方法
来源：http://uus.52xcode.cn

Py:   def greet(self): return self.name
来源：http://fkp.gzhubu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fmi.jianghu66.top

JS:   greet() { return this.name; }
来源：http://hxg.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://dvd.yonumen.top

Java: String greet() { return name; }
来源：http://rhf.c1oappe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ssp.fengsongda.top

Ruby: def greet; @name; end
来源：http://olk.jyoumei.cn

C#:   public string Greet() => Name;
来源：http://vmy.shzxlz.cn

[G05] 继承
来源：http://cgb.zhongyouzk.top

Py:   class Admin(User): pass
来源：http://qzi.52xcode.cn

PHP:  class Admin extends User {}
来源：http://tvg.zycfv.cn

JS:   class Admin extends User {}
来源：http://lwd.ydzc1.top

TS:   class Admin extends User {}
来源：http://szd.jinqigufen.top

Java: class Admin extends User {}
来源：http://dgj.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hxz.nanxinkj.top

Ruby: class Admin < User; end
来源：http://zle.shangyingyoupin.top

C#:   class Admin : User {}
来源：http://epv.shanyushiyangtech.top

[G06] 重写方法
来源：http://msa.yueranfly.top

Py:   def greet(self): return "admin"
来源：http://kti.sysykeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://iib.quarkkingdee.top

JS:   greet() { return "admin"; }
来源：http://ubr.gzhubu.top

TS:   greet(): string { return "admin"; }
来源：http://imr.sysykeji.top

Java: @Override String greet() { return "admin"; }
来源：http://puo.xuetiantiany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jit.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://juk.sufxvd.cn

C#:   public override string Greet() => "admin";
来源：http://pfw.ivvv.top

[G07] 调用父类方法
来源：http://rzl.cqqwz.cn

Py:   super().greet()
来源：http://kij.316326.xyz

PHP:  parent::greet();
来源：http://jbe.iojbl.cn

JS:   super.greet();
来源：http://szy.dianchejie.cn

TS:   super.greet();
来源：http://eyj.zhaomingkeji.xyz

Java: super.greet();
来源：http://xkk.sweek.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wzb.52xcode.cn

Ruby: super
来源：http://gtx.epnwcf.com

C#:   base.Greet();
来源：http://crl.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://onk.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://owd.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://fzd.uphjek.com

JS:   static f() {}
来源：http://heq.sxryk.cn

TS:   static f(): void {}
来源：http://auh.pengpengdd.cyou

Java: static void f() {}
来源：http://ppc.bjfxy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wmx.ydjk.org.cn

Ruby: def self.f; end
来源：http://nts.aibaodan.cn

C#:   public static void F() {}
来源：http://awf.tarul.cn

[G09] 接口 / 抽象类
来源：http://ibv.sxryk.cn

Py:   from abc import ABC, abstractmethod
来源：http://xmd.nanxuanxn.top

PHP:  interface Shape { public function area(): float; }
来源：http://dam.vqdsnc.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cya.nwbrower.top

TS:   interface Shape { area(): number; }
来源：http://kvj.jinyuanbaomall.cn

Java: interface Shape { double area(); }
来源：http://hxe.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://anj.yuxming.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jav.hnqzz.top

C#:   interface IShape { double Area(); }
来源：http://czx.yfazqb.com

[G10] 访问控制
来源：http://goe.yj20258.top

Py:   约定 _protected / __private（不强制）
来源：http://qoq.fanxiaobao.xyz

PHP:  public / protected / private
来源：http://hfu.fktsv.cn

JS:   #private 字段；其余公开
来源：http://jfh.nwbrower.top

TS:   public / protected / private
来源：http://qrl.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://rmj.shuidangran.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fxa.xylfe.cn

Ruby: public / protected / private
来源：http://tvj.zhaomingkeji.xyz

C#:   public / protected / private / internal
来源：http://xhf.guannengcc.top

[G11] getter / setter
来源：http://shi.hcnkem.com

Py:   @property 与 @x.setter
来源：http://myl.fengsongda.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vfx.zycfv.cn

JS:   get name() { return this._name; }
来源：http://kry.havefunace.top

TS:   get name(): string { return this._name; }
来源：http://aow.hcnkem.com

Java: public String getName() { return name; }
来源：http://yzi.xziqi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vuk.sxryk.cn

Ruby: attr_accessor :name
来源：http://twc.bbcook.cn

C#:   public string Name { get; set; }
来源：http://pdw.xziqi.cn

[G12] 对象转字符串
来源：http://wwn.316326.xyz

Py:   def __str__(self): return self.name
来源：http://gns.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jnc.kuanghao11.cn

JS:   toString() { return this.name; }
来源：http://cad.sjlbkw.cn

TS:   toString(): string { return this.name; }
来源：http://dqr.hnqzz.top

Java: @Override public String toString() { return name; }
来源：http://cgl.xziqi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cwb.andypj.xyz

Ruby: def to_s; @name; end
来源：http://kvj.birdmap.top

C#:   public override string ToString() => Name;
来源：http://oaa.bbcook.cn

[G13] 判断对象类型
来源：http://cwa.zdbjq.cn

Py:   isinstance(u, User)
来源：http://asr.sysykeji.top

PHP:  $u instanceof User
来源：http://rfn.sweek.top

JS:   u instanceof User
来源：http://emi.hfpthk.cn

TS:   u instanceof User
来源：http://tqw.hcnkem.com

Java: u instanceof User
来源：http://yxc.xziqi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xox.ywan-chungtsiang.top

Ruby: u.is_a?(User)
来源：http://fuz.jqgfzy.top

C#:   u is User
来源：http://qwy.sjlbkw.cn

[G14] 数据类 / record
来源：http://wdn.cheryme.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tpo.svipenyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://lnh.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vek.xuetiantiany.cn

TS:   type User = { name: string; age: number };
来源：http://ptw.cdnleiting.top

Java: record User(String name, int age) {}
来源：http://sxx.nanxinkj.top

Go:   type User struct { Name string; Age int }
来源：http://gjs.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dye.xylfe.cn

C#:   record User(string Name, int Age);
来源：http://zlm.sxryk.cn

[G15] 枚举
来源：http://nwi.havefunace.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qvb.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gah.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bcx.haohaochexian.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cmr.xinyue.icu

Java: enum Color { RED, GREEN }
来源：http://nft.tanke756.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pvq.tian-w.cn

Ruby: Color = %i[red green].freeze
来源：http://qpk.hesvh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ugc.hnxiangtu.top

[G16] 对象转数组 / 字典
来源：http://mjl.yuxming.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ohb.mhx1999.top

PHP:  get_object_vars($obj);
来源：http://uao.chenjidiqi.icu

JS:   Object.entries(obj)
来源：http://mpn.daria6918.cn

TS:   Object.entries(obj)
来源：http://acr.zhiwuduotai.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lyw.cdnleiting.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://atm.nwbrower.top

Ruby: obj.instance_variables
来源：http://uch.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://iuf.gotoacloud.top

================================================================================
来源：http://ttg.nwbrower.top

H. 异常与错误处理
来源：http://dic.jinqigfzy.top

================================================================================
来源：http://mbe.yanxiufei.cn

[H01] try / catch 基础
来源：http://tfv.sufxvd.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xbh.cucudq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rlt.bbcook.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tnj.chenzaomai.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rzx.fengsongda.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xbw.jlsjyb.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zyr.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dbt.svipenyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zmj.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://coo.yvedp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://leh.hcnkem.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://hjp.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lzn.ehwqpu.com

TS:   try { f(); } finally { cleanup(); }
来源：http://wvu.jinyuanbaomall.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bjl.yuxming.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jei.9152youxi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ysj.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dpz.ehwqpu.com

[H03] 主动抛出异常
来源：http://lnl.andypj.xyz

Py:   raise ValueError("错误信息")
来源：http://sum.jyoumei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://krn.iojbl.cn

JS:   throw new Error("错误信息");
来源：http://nfd.yanxiufei.cn

TS:   throw new Error("错误信息");
来源：http://yyc.jinghuilouyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fub.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wvq.jinghuilouyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://owm.birdmap.top

C#:   throw new ArgumentException("错误信息");
来源：http://apw.tarul.cn

[H04] 自定义异常类型
来源：http://pan.ydzc1.top

Py:   class MyError(Exception): pass
来源：http://egv.chenzaomai.com

PHP:  class MyError extends RuntimeException {}
来源：http://wvf.smart0.xyz

JS:   class MyError extends Error {}
来源：http://bwz.nanxuanxn.top

TS:   class MyError extends Error {}
来源：http://fef.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://qgw.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nyo.hysaishi.cn

Ruby: class MyError < StandardError; end
来源：http://zfb.bbcook.cn

C#:   class MyException : Exception {}
来源：http://fnj.ppjwa.cn

[H05] 捕获特定类型
来源：http://piv.cqqwz.cn

Py:   except ValueError as e:
来源：http://szw.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cqn.zhengqikj.top

JS:   if (e instanceof TypeError) {}
来源：http://rlv.yangfankeji.com

TS:   if (e instanceof TypeError) {}
来源：http://doz.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://rjg.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jqr.xziqi.cn

Ruby: rescue ArgumentError => e
来源：http://yfj.ydjk.org.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rcd.hesvh.cn

[H06] 可选值 / 空值安全访问
来源：http://rgy.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://xhg.ehwqpu.com

PHP:  $v = $d["k"] ?? null;
来源：http://vnm.dianchejie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zgd.guowangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://hmm.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://syd.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pdt.jyoumei.cn

Ruby: d&.dig(:a, :b)
来源：http://obx.quarkkingdee.top

C#:   obj?.A?.B ?? default
来源：http://yzc.jinghuilouyu.cn

[H07] 断言
来源：http://vem.chenzaomai.com

Py:   assert x > 0, "必须为正"
来源：http://bsg.hfpthk.cn

PHP:  assert($x > 0);
来源：http://vaw.nanxinkj.top

JS:   console.assert(x > 0);
来源：http://lam.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://epi.sweek.top

Java: assert x > 0 : "必须为正";
来源：http://mxe.zycfv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qru.wangshuangyany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nov.sysykeji.top

C#:   Debug.Assert(x > 0);
来源：http://pzr.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://vdb.daxiang520.top

Py:   str(e);  traceback.format_exc()
来源：http://dke.fehbvm.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kca.chenlongwang.top

JS:   e.message;  e.stack
来源：http://bcz.yongpay.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lnb.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ckc.cheryme.top

Go:   err.Error()
来源：http://lsj.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://csj.sjlbkw.cn

C#:   e.Message;  e.StackTrace
来源：http://wxq.jinyuanbaomall.cn

[H09] 带错误码的异常
来源：http://jkc.mhx1999.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hqu.chenzaomai.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://fnc.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mxt.kuanghao11.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cdi.9152youxi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kwu.nwbrower.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mto.xinyue.icu

Ruby: raise MyError.new("fail", 500)
来源：http://svv.0kj1m.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://abv.wangshuangyany.cn

[H10] 资源自动释放
来源：http://tok.ydjk.org.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zwf.quarkkingdee.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jcx.svipenyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fmv.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rdj.nwbrower.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kfp.guannengcc.top

Go:   defer f.Close()
来源：http://ybd.9152youxi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vki.yfazqb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jpv.guannengcc.top


<!-- 参考信息 -->