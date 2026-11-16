代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://mce.shanyushiyangtech.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lxx.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://qdd.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://jrr.chenzaomai.com

TS:   fs.existsSync("a.txt")
来源：http://skd.zhaomingkeji.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://qpy.zycfv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hng.tarul.cn

Ruby: File.exist?("a.txt")
来源：http://ang.hammf.cn

C#:   File.Exists("a.txt")
来源：http://qbn.hywenlv.cn

[F06] 删除文件
来源：http://epa.jyoumei.cn

Py:   os.remove("a.txt")
来源：http://not.quarkkingdee.top

PHP:  unlink("a.txt");
来源：http://ikl.chenzaomai.com

JS:   fs.unlinkSync("a.txt")
来源：http://ssg.redwolf501.top

TS:   fs.unlinkSync("a.txt")
来源：http://poy.hesvh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jyf.zdbjq.cn

Go:   os.Remove("a.txt")
来源：http://uzj.jiagoushi.top

Ruby: File.delete("a.txt")
来源：http://xgj.c1oappe.top

C#:   File.Delete("a.txt");
来源：http://qbm.shanyushiyangkeji.top

[F07] 创建目录（含多级）
来源：http://nsq.cucudq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tkw.hcnkem.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rah.cqqwz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mso.jqgfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kwl.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vas.shangyingyoupin.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gqk.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://plf.cheryme.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nkx.aibaodan.cn

[F08] 遍历目录
来源：http://qyg.hcnkem.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://oun.jqgufenzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kuc.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://qzu.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://rgu.zhoulong.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wfe.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jzj.chenzaomai.com

Ruby: Dir.children("dir")
来源：http://zwt.shanyushiyangtech.top

C#:   Directory.GetFiles("dir")
来源：http://nvf.xuanzx.com

[F09] 获取文件大小
来源：http://mvy.yueranfly.top

Py:   os.path.getsize("a.txt")
来源：http://uyj.yuxming.cn

PHP:  filesize("a.txt");
来源：http://oui.0kj1m.cn

JS:   fs.statSync("a.txt").size
来源：http://iqm.shanyushiyangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://evv.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://gzr.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xdt.fzhhl.top

Ruby: File.size("a.txt")
来源：http://pzo.yuxming.cn

C#:   new FileInfo("a.txt").Length
来源：http://seb.dianchejie.cn

[F10] 取文件扩展名 / 文件名
来源：http://kzp.hongshengwenyu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ogu.ydzc1.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://khz.zdqjudy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zrc.haohaochexian.top

TS:   path.extname("a.txt")
来源：http://nyw.bbcook.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cnb.vehdjk.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bvk.zycfv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qhy.fengsongda.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vlu.sjlbkw.cn

[F11] 复制与移动文件
来源：http://utv.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ldu.birdmap.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gsl.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hga.cashguo.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cch.sweek.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ekm.guannengcc.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hvn.epnwcf.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hrt.sjlbkw.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://llu.cashguo.top

[F12] CSV 读写
来源：http://uom.gotoacloud.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gdz.jyoumei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rls.fengsongda.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oda.dashuyun.cn

TS:   // 同上
来源：http://ojz.meibo888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ihn.cdnleiting.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ymy.meibo888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ahs.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://cqt.yj202588.top

================================================================================
来源：http://ydk.nanxinkj.top

G. 面向对象
来源：http://xsc.redwolf501.top

================================================================================
来源：http://fqz.quarkkingdee.top

[G01] 定义类
来源：http://fcp.nwbrower.top

Py:   class User: pass
来源：http://qxg.yuanzhike.top

PHP:  class User {}
来源：http://vag.kuanghao11.cn

JS:   class User {}
来源：http://hmi.nanxinkj.top

TS:   class User { name: string = ""; }
来源：http://hpl.yonumen.top

Java: class User {}
来源：http://ugo.9152youxi.cn

Go:   type User struct { Name string }
来源：http://gik.zhoulong.xyz

Ruby: class User; end
来源：http://fzs.cucudq.cn

C#:   class User {}
来源：http://hyj.pengpengdd.cyou

[G02] 构造函数
来源：http://plu.birdmap.top

Py:   def __init__(self, name): self.name = name
来源：http://miq.yanxiufei.cn

PHP:  public function __construct(public string $name) {}
来源：http://wps.zdqjudy.top

JS:   constructor(name) { this.name = name; }
来源：http://diz.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://sey.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://qit.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wxi.vehdjk.com

Ruby: def initialize(name); @name = name; end
来源：http://dvw.cqqwz.cn

C#:   public User(string name) { Name = name; }
来源：http://agq.fengsongda.top

[G03] 实例属性
来源：http://lof.0kj1m.cn

Py:   self.name = "x"
来源：http://jlv.hnqzz.top

PHP:  public string $name = "x";
来源：http://bwj.andypj.xyz

JS:   this.name = "x";
来源：http://nvs.ivvv.top

TS:   name: string = "x";
来源：http://ygo.yvedp.cn

Java: private String name;
来源：http://qhh.xziqi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bor.hongshengwenyu.top

Ruby: @name = "x"
来源：http://eya.yfazqb.com

C#:   public string Name { get; set; } = "x";
来源：http://ejq.ehwqpu.com

[G04] 定义方法
来源：http://mou.hongshengwenyu.top

Py:   def greet(self): return self.name
来源：http://wcr.zdqjudy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://adn.jinyuanbaomall.cn

JS:   greet() { return this.name; }
来源：http://sve.jinqigufen.top

TS:   greet(): string { return this.name; }
来源：http://evr.tarul.cn

Java: String greet() { return name; }
来源：http://lik.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ija.iojbl.cn

Ruby: def greet; @name; end
来源：http://usu.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://ekw.yj202588.top

[G05] 继承
来源：http://mim.ehwqpu.com

Py:   class Admin(User): pass
来源：http://jqc.fengsongda.top

PHP:  class Admin extends User {}
来源：http://mju.chenzaomai.com

JS:   class Admin extends User {}
来源：http://wsl.cdnleiting.top

TS:   class Admin extends User {}
来源：http://tga.aizwys.cn

Java: class Admin extends User {}
来源：http://mvc.haohaochexian.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eiz.hysaishi.cn

Ruby: class Admin < User; end
来源：http://lth.ppjwa.cn

C#:   class Admin : User {}
来源：http://mtp.zycfv.cn

[G06] 重写方法
来源：http://ogw.zdqjudy.top

Py:   def greet(self): return "admin"
来源：http://ghd.wangdashe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dlj.yj20258.top

JS:   greet() { return "admin"; }
来源：http://hwl.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://zgf.hnxiangtu.top

Java: @Override String greet() { return "admin"; }
来源：http://lwm.tianlin.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qyu.aizwys.cn

Ruby: def greet; "admin"; end
来源：http://wyv.hfpthk.cn

C#:   public override string Greet() => "admin";
来源：http://rug.kuanghao11.cn

[G07] 调用父类方法
来源：http://buv.hfpthk.cn

Py:   super().greet()
来源：http://bnx.9152youxi.cn

PHP:  parent::greet();
来源：http://nvw.fehbvm.com

JS:   super.greet();
来源：http://lyw.yvedp.cn

TS:   super.greet();
来源：http://uzu.sufxvd.cn

Java: super.greet();
来源：http://znh.jinyuanbaomall.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mos.nanxinkj.top

Ruby: super
来源：http://loe.zhixingplan.top

C#:   base.Greet();
来源：http://ccm.yuxming.cn

[G08] 静态方法与属性
来源：http://mke.vehdjk.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hmd.yuxming.cn

PHP:  public static function f() {}
来源：http://vyc.nanxinkj.top

JS:   static f() {}
来源：http://ldc.snrcjt.cn

TS:   static f(): void {}
来源：http://huy.cucudq.cn

Java: static void f() {}
来源：http://dei.meibo888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mxj.shangyingyoupin.top

Ruby: def self.f; end
来源：http://edv.ydjk.org.cn

C#:   public static void F() {}
来源：http://fwz.jyoumei.cn

[G09] 接口 / 抽象类
来源：http://lze.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://jxh.guowangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://xde.wangdashe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tnz.jqgfzy.top

TS:   interface Shape { area(): number; }
来源：http://pqg.vehdjk.com

Java: interface Shape { double area(); }
来源：http://ubv.chenlongwang.top

Go:   type Shape interface { Area() float64 }
来源：http://svm.birdmap.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://azg.jlsjyb.cn

C#:   interface IShape { double Area(); }
来源：http://kzt.hammf.cn

[G10] 访问控制
来源：http://bcj.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://uaa.epnwcf.com

PHP:  public / protected / private
来源：http://crz.xziqi.cn

JS:   #private 字段；其余公开
来源：http://jkm.cucudq.cn

TS:   public / protected / private
来源：http://jlj.xziqi.cn

Java: public / protected / private / 默认包级
来源：http://rpg.cqqwz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://amb.shanyushiyangkeji.top

Ruby: public / protected / private
来源：http://rhn.guannengcc.top

C#:   public / protected / private / internal
来源：http://hav.zhengqikj.top

[G11] getter / setter
来源：http://wmm.dianchejie.cn

Py:   @property 与 @x.setter
来源：http://cmk.nanxuanxn.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uvh.ybcxt.top

JS:   get name() { return this._name; }
来源：http://ohp.jqgufenzy.top

TS:   get name(): string { return this._name; }
来源：http://hjo.jqgfzy.top

Java: public String getName() { return name; }
来源：http://cdz.wangshuangyany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fch.sxryk.cn

Ruby: attr_accessor :name
来源：http://ojr.ybcxt.top

C#:   public string Name { get; set; }
来源：http://jvf.hammf.cn

[G12] 对象转字符串
来源：http://kca.iojbl.cn

Py:   def __str__(self): return self.name
来源：http://lsc.yuxming.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://axl.quarkkingdee.top

JS:   toString() { return this.name; }
来源：http://fak.hnxiangtu.top

TS:   toString(): string { return this.name; }
来源：http://oqx.xingfuxueyuan.xyz

Java: @Override public String toString() { return name; }
来源：http://gir.dianchejie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tmi.jinqigufen.top

Ruby: def to_s; @name; end
来源：http://tao.epnwcf.com

C#:   public override string ToString() => Name;
来源：http://msi.xuanzx.com

[G13] 判断对象类型
来源：http://ink.nanxinkj.top

Py:   isinstance(u, User)
来源：http://fxs.jlsjyb.cn

PHP:  $u instanceof User
来源：http://hbr.sxryk.cn

JS:   u instanceof User
来源：http://ide.yueranfly.top

TS:   u instanceof User
来源：http://buz.meibo888.top

Java: u instanceof User
来源：http://xgk.jinyuanbaomall.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://maq.ywan-chungtsiang.top

Ruby: u.is_a?(User)
来源：http://lim.quarkkingdee.top

C#:   u is User
来源：http://pub.sweek.top

[G14] 数据类 / record
来源：http://lhk.tian-w.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kpb.yj202588.top

PHP:  // 用 readonly 属性模拟
来源：http://qdf.jinqigufen.top

JS:   // 无内置：普通类或对象字面量
来源：http://jen.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://zhd.shanyushiyangtech.top

Java: record User(String name, int age) {}
来源：http://oli.tian-w.cn

Go:   type User struct { Name string; Age int }
来源：http://dez.316326.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://emy.yuanzhike.top

C#:   record User(string Name, int Age);
来源：http://ymv.jinqigufen.top

[G15] 枚举
来源：http://wug.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sbo.zhaomingkeji.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://yam.yj20258.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mkq.feifeiyinyue.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://btc.zdbjq.cn

Java: enum Color { RED, GREEN }
来源：http://onu.yonumen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kmw.cheryme.top

Ruby: Color = %i[red green].freeze
来源：http://kzx.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://daq.fanxiaobao.xyz

[G16] 对象转数组 / 字典
来源：http://iuu.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zbl.nanxuanxn.top

PHP:  get_object_vars($obj);
来源：http://frb.xuetiantiany.cn

JS:   Object.entries(obj)
来源：http://dtz.uphjek.com

TS:   Object.entries(obj)
来源：http://irb.sweek.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aql.zhijiandao.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gpb.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://uso.tian-w.cn

C#:   // 用反射或 System.Text.Json
来源：http://gsh.meibo888.top

================================================================================
来源：http://zvd.cucudq.cn

H. 异常与错误处理
来源：http://eeh.shanyushiyangkeji.top

================================================================================
来源：http://ywr.cheryme.top

[H01] try / catch 基础
来源：http://lvp.yvedp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://phx.ehwqpu.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eya.hfpthk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iff.dianchejie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hvl.sjlbkw.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eoz.bbcook.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qsa.gotoacloud.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mzv.xziqi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jbh.shzxlz.cn

[H02] finally / ensure 收尾
来源：http://bgx.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://eha.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zpi.zhongyouzk.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ymx.birdmap.top

TS:   try { f(); } finally { cleanup(); }
来源：http://clj.fehbvm.com

Java: try { f(); } finally { cleanup(); }
来源：http://oli.zhiwuduotai.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qrn.tanke756.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kgq.jinqigfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lza.vqdsnc.cn

[H03] 主动抛出异常
来源：http://pfg.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://pvy.yfazqb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fyj.shanyushiyangkeji.top

JS:   throw new Error("错误信息");
来源：http://dmr.bbcook.cn

TS:   throw new Error("错误信息");
来源：http://mic.fengsongda.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gjj.shuidangran.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bgn.jyoumei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zox.xuanzx.com

C#:   throw new ArgumentException("错误信息");
来源：http://spg.zhixingplan.top

[H04] 自定义异常类型
来源：http://nej.shuidangran.top

Py:   class MyError(Exception): pass
来源：http://elz.hnxiangtu.top

PHP:  class MyError extends RuntimeException {}
来源：http://ajn.andypj.xyz

JS:   class MyError extends Error {}
来源：http://yff.xylfe.cn

TS:   class MyError extends Error {}
来源：http://edu.cashguo.top

Java: class MyException extends RuntimeException {}
来源：http://mjp.ehwqpu.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://maw.zhiwuduotai.top

Ruby: class MyError < StandardError; end
来源：http://tdo.yj20258.top

C#:   class MyException : Exception {}
来源：http://nxu.zhiwuduotai.top

[H05] 捕获特定类型
来源：http://vzw.yj20258888.top

Py:   except ValueError as e:
来源：http://ugi.tianlin.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://whl.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://lqe.epnwcf.com

TS:   if (e instanceof TypeError) {}
来源：http://ggw.yj20258.top

Java: catch (IOException | SQLException e) {}
来源：http://kuq.sjlbkw.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sas.hnqzz.top

Ruby: rescue ArgumentError => e
来源：http://qco.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oeb.quarkkingdee.top

[H06] 可选值 / 空值安全访问
来源：http://wkf.tian-w.cn

Py:   value = d.get("k") or default
来源：http://nny.chenlongwang.top

PHP:  $v = $d["k"] ?? null;
来源：http://qdp.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rgb.gogol.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ebg.daxiang520.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xre.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hvk.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://sjd.c1oappe.top

C#:   obj?.A?.B ?? default
来源：http://iuu.havefunace.top

[H07] 断言
来源：http://amk.cdnleiting.top

Py:   assert x > 0, "必须为正"
来源：http://rqf.yuanzhike.top

PHP:  assert($x > 0);
来源：http://bjy.redwolf501.top

JS:   console.assert(x > 0);
来源：http://vzw.nanxuanxn.top

TS:   console.assert(x > 0);
来源：http://dts.yangfankeji.com

Java: assert x > 0 : "必须为正";
来源：http://qru.shanyushiyangtech.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iwo.cucudq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jrh.cheryme.top

C#:   Debug.Assert(x > 0);
来源：http://ndh.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://rex.tarul.cn

Py:   str(e);  traceback.format_exc()
来源：http://wab.zdbjq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eix.smart0.xyz

JS:   e.message;  e.stack
来源：http://xzm.xylfe.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qxe.ywan-chungtsiang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ahf.xziqi.cn

Go:   err.Error()
来源：http://zzv.cdnleiting.top

Ruby: e.message;  e.backtrace
来源：http://vmq.andypj.xyz

C#:   e.Message;  e.StackTrace
来源：http://cdw.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://mod.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cqq.tarul.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tka.yuxming.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mdv.jinyuanbaomall.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ubb.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://psr.dashuyun.cn


<!-- 参考信息 -->