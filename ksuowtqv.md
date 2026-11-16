代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://wxn.jyoumei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://byn.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://fhk.hesvh.cn

JS:   fs.existsSync("a.txt")
来源：http://wpe.xinyue.icu

TS:   fs.existsSync("a.txt")
来源：http://aet.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tcd.sxryk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nhc.gaohongyu789.top

Ruby: File.exist?("a.txt")
来源：http://iqq.bjfxy.top

C#:   File.Exists("a.txt")
来源：http://dgi.jinqigufen.top

[F06] 删除文件
来源：http://csk.jinqigfzy.top

Py:   os.remove("a.txt")
来源：http://uei.cucudq.cn

PHP:  unlink("a.txt");
来源：http://qgh.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://aid.ywan-chungtsiang.top

TS:   fs.unlinkSync("a.txt")
来源：http://fop.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ugw.xylfe.cn

Go:   os.Remove("a.txt")
来源：http://hoe.xylfe.cn

Ruby: File.delete("a.txt")
来源：http://qjs.shzxlz.cn

C#:   File.Delete("a.txt");
来源：http://ssf.nanxinkj.top

[F07] 创建目录（含多级）
来源：http://hue.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qus.52xcode.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ctq.cqqwz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dfa.yongpay.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uqz.daria6918.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yls.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://efz.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://etl.snrcjt.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vmn.zdqjudy.top

[F08] 遍历目录
来源：http://wwl.xziqi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pvw.sufxvd.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rdg.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://psg.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://zfl.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dwq.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fvr.fktsv.cn

Ruby: Dir.children("dir")
来源：http://qyu.chenjidiqi.icu

C#:   Directory.GetFiles("dir")
来源：http://nym.yonumen.top

[F09] 获取文件大小
来源：http://fxj.aibaodan.cn

Py:   os.path.getsize("a.txt")
来源：http://ahm.yj202588.top

PHP:  filesize("a.txt");
来源：http://vmx.vehdjk.com

JS:   fs.statSync("a.txt").size
来源：http://wom.yangfankeji.com

TS:   fs.statSync("a.txt").size
来源：http://xsl.zhoulong.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://yvw.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fym.xingfuxueyuan.xyz

Ruby: File.size("a.txt")
来源：http://wvy.vqdsnc.cn

C#:   new FileInfo("a.txt").Length
来源：http://xwb.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://wcw.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hme.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uio.hysaishi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uwo.nwbrower.top

TS:   path.extname("a.txt")
来源：http://bdt.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kvn.xingfuxueyuan.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jqi.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mfr.fanxiaobao.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rsn.jlsjyb.cn

[F11] 复制与移动文件
来源：http://nvq.yangfankeji.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hpj.dashuyun.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://quu.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dnp.ctjpmb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://foa.yuxming.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jyl.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bmb.xuanzx.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://awi.jinqigfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pej.aizwys.cn

[F12] CSV 读写
来源：http://dof.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bka.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xmd.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sob.zhixingplan.top

TS:   // 同上
来源：http://nao.pengpengdd.cyou

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ckc.hywenlv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cfd.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kjn.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jrr.aizwys.cn

================================================================================
来源：http://adw.sjlbkw.cn

G. 面向对象
来源：http://owd.ivvv.top

================================================================================
来源：http://yfd.andypj.xyz

[G01] 定义类
来源：http://xlr.zhongyouzk.top

Py:   class User: pass
来源：http://umo.fengsongda.top

PHP:  class User {}
来源：http://ojg.yanxiufei.cn

JS:   class User {}
来源：http://hfn.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://cig.jinqigfzy.top

Java: class User {}
来源：http://obu.nanxuanxn.top

Go:   type User struct { Name string }
来源：http://mhv.jinyuanbaomall.cn

Ruby: class User; end
来源：http://odf.gogol.net.cn

C#:   class User {}
来源：http://hbb.yj202588.top

[G02] 构造函数
来源：http://jva.daxiang520.top

Py:   def __init__(self, name): self.name = name
来源：http://fhl.sxryk.cn

PHP:  public function __construct(public string $name) {}
来源：http://ctq.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://xac.zhoulong.xyz

TS:   constructor(public name: string) {}
来源：http://eqb.dashuyun.cn

Java: User(String name) { this.name = name; }
来源：http://ibs.ybcxt.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gsx.tanke756.top

Ruby: def initialize(name); @name = name; end
来源：http://oxl.jinqigfzy.top

C#:   public User(string name) { Name = name; }
来源：http://lwy.sweek.top

[G03] 实例属性
来源：http://hee.fzhhl.top

Py:   self.name = "x"
来源：http://flp.svipenyu.cn

PHP:  public string $name = "x";
来源：http://oaz.hnxiangtu.top

JS:   this.name = "x";
来源：http://bas.tanke756.top

TS:   name: string = "x";
来源：http://eko.xingfuxueyuan.xyz

Java: private String name;
来源：http://snv.zhengqikj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lfy.ydzc1.top

Ruby: @name = "x"
来源：http://dvu.hesvh.cn

C#:   public string Name { get; set; } = "x";
来源：http://qaq.shangyingyoupin.top

[G04] 定义方法
来源：http://xdn.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://tta.epnwcf.com

PHP:  public function greet(): string { return $this->name; }
来源：http://sak.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://nff.jianghu66.top

TS:   greet(): string { return this.name; }
来源：http://bfj.havefunace.top

Java: String greet() { return name; }
来源：http://ifd.fktsv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rui.sysykeji.top

Ruby: def greet; @name; end
来源：http://hyw.ehwqpu.com

C#:   public string Greet() => Name;
来源：http://oqv.yj20258888.top

[G05] 继承
来源：http://dqq.zdbjq.cn

Py:   class Admin(User): pass
来源：http://jhr.mhx1999.top

PHP:  class Admin extends User {}
来源：http://xaw.tarul.cn

JS:   class Admin extends User {}
来源：http://nql.hcnkem.com

TS:   class Admin extends User {}
来源：http://oaz.ydjk.org.cn

Java: class Admin extends User {}
来源：http://god.jyoumei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zaq.xylfe.cn

Ruby: class Admin < User; end
来源：http://apv.52xcode.cn

C#:   class Admin : User {}
来源：http://sdn.hongshengwenyu.top

[G06] 重写方法
来源：http://pqj.aizwys.cn

Py:   def greet(self): return "admin"
来源：http://cvz.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://ifn.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://tbm.yanxiufei.cn

TS:   greet(): string { return "admin"; }
来源：http://twj.xuanzx.com

Java: @Override String greet() { return "admin"; }
来源：http://qoz.cashguo.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dgn.iojbl.cn

Ruby: def greet; "admin"; end
来源：http://jwi.zycfv.cn

C#:   public override string Greet() => "admin";
来源：http://zcp.fzhhl.top

[G07] 调用父类方法
来源：http://ija.jiagoushi.top

Py:   super().greet()
来源：http://yun.uphjek.com

PHP:  parent::greet();
来源：http://lyw.zhaomingkeji.xyz

JS:   super.greet();
来源：http://dqq.zycfv.cn

TS:   super.greet();
来源：http://omw.shzxlz.cn

Java: super.greet();
来源：http://twz.shuidangran.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xqz.xylfe.cn

Ruby: super
来源：http://hax.cucudq.cn

C#:   base.Greet();
来源：http://eme.jlsjyb.cn

[G08] 静态方法与属性
来源：http://kvb.pengpengdd.cyou

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://laf.yangfankeji.com

PHP:  public static function f() {}
来源：http://dyg.yongpay.top

JS:   static f() {}
来源：http://xze.nanxuanxn.top

TS:   static f(): void {}
来源：http://mpy.jinqigfzy.top

Java: static void f() {}
来源：http://rbk.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://djf.tanke756.top

Ruby: def self.f; end
来源：http://ohv.daxiang520.top

C#:   public static void F() {}
来源：http://bwr.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://gmx.fanxiaobao.xyz

Py:   from abc import ABC, abstractmethod
来源：http://esl.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qhj.cheryme.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hnd.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://cra.cqqwz.cn

Java: interface Shape { double area(); }
来源：http://jre.yanxiufei.cn

Go:   type Shape interface { Area() float64 }
来源：http://rcx.yvedp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ikh.ywan-chungtsiang.top

C#:   interface IShape { double Area(); }
来源：http://mqc.aibaodan.cn

[G10] 访问控制
来源：http://jsi.vehdjk.com

Py:   约定 _protected / __private（不强制）
来源：http://gpk.hywenlv.cn

PHP:  public / protected / private
来源：http://amu.xinyue.icu

JS:   #private 字段；其余公开
来源：http://nor.bbcook.cn

TS:   public / protected / private
来源：http://aos.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://wlm.zycfv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lju.gotoacloud.top

Ruby: public / protected / private
来源：http://erj.hysaishi.cn

C#:   public / protected / private / internal
来源：http://eva.jqgfzy.top

[G11] getter / setter
来源：http://zrb.guowangkeji.top

Py:   @property 与 @x.setter
来源：http://nro.zhaomingkeji.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://mvk.xuetiantiany.cn

JS:   get name() { return this._name; }
来源：http://psh.xinyue.icu

TS:   get name(): string { return this._name; }
来源：http://rky.cucudq.cn

Java: public String getName() { return name; }
来源：http://ajd.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://roa.xylfe.cn

Ruby: attr_accessor :name
来源：http://tba.zhengqikj.top

C#:   public string Name { get; set; }
来源：http://thc.shzxlz.cn

[G12] 对象转字符串
来源：http://auh.mhx1999.top

Py:   def __str__(self): return self.name
来源：http://tcc.nanxinkj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yav.yj202588.top

JS:   toString() { return this.name; }
来源：http://ypl.yonumen.top

TS:   toString(): string { return this.name; }
来源：http://qnj.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://uxz.zdbjq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://elx.cqqwz.cn

Ruby: def to_s; @name; end
来源：http://zrs.xziqi.cn

C#:   public override string ToString() => Name;
来源：http://wny.yfazqb.com

[G13] 判断对象类型
来源：http://xpo.gaohongyu789.top

Py:   isinstance(u, User)
来源：http://ulg.hnqzz.top

PHP:  $u instanceof User
来源：http://igt.jlsjyb.cn

JS:   u instanceof User
来源：http://nrn.sweek.top

TS:   u instanceof User
来源：http://zbi.fzhhl.top

Java: u instanceof User
来源：http://pdm.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hbf.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://jyg.gotoacloud.top

C#:   u is User
来源：http://swu.fzhhl.top

[G14] 数据类 / record
来源：http://hgz.shzxlz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tpo.hongshengwenyu.top

PHP:  // 用 readonly 属性模拟
来源：http://afm.zycfv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tkf.ywan-chungtsiang.top

TS:   type User = { name: string; age: number };
来源：http://hyi.cucudq.cn

Java: record User(String name, int age) {}
来源：http://bcs.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://kyx.zhijiandao.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vdl.zhixingplan.top

C#:   record User(string Name, int Age);
来源：http://crh.gotoacloud.top

[G15] 枚举
来源：http://xpf.xinyue.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wuz.yj20258888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rcj.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ykq.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sju.zhixingplan.top

Java: enum Color { RED, GREEN }
来源：http://njm.kuanghao11.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kfc.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://rxp.svipenyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://emj.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://cgn.cdnleiting.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zje.zdbjq.cn

PHP:  get_object_vars($obj);
来源：http://hoq.mhx1999.top

JS:   Object.entries(obj)
来源：http://xna.xziqi.cn

TS:   Object.entries(obj)
来源：http://kaw.yj20258.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wth.zhijiandao.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cqr.gzhubu.top

Ruby: obj.instance_variables
来源：http://ecz.cqqwz.cn

C#:   // 用反射或 System.Text.Json
来源：http://tmf.iojbl.cn

================================================================================
来源：http://nhe.jyoumei.cn

H. 异常与错误处理
来源：http://cvt.aizwys.cn

================================================================================
来源：http://vxf.fanxiaobao.xyz

[H01] try / catch 基础
来源：http://ngk.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kwb.xziqi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://amn.fengsongda.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fak.yj202588.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xnh.yanxiufei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sry.mhx1999.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pvk.dianchejie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qil.ppjwa.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wlp.quarkkingdee.top

[H02] finally / ensure 收尾
来源：http://szc.sweek.top

Py:   try: f()⏎finally: cleanup()
来源：http://shg.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jpw.tanke756.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sem.aibaodan.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nvk.jinqigufen.top

Java: try { f(); } finally { cleanup(); }
来源：http://jpu.hysaishi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xmy.ivvv.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ddh.nanxuanxn.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rae.gotoacloud.top

[H03] 主动抛出异常
来源：http://ett.jqgfzy.top

Py:   raise ValueError("错误信息")
来源：http://syj.shzxlz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pyh.mhx1999.top

JS:   throw new Error("错误信息");
来源：http://znt.epnwcf.com

TS:   throw new Error("错误信息");
来源：http://wku.yj20258888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kba.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xup.yueranfly.top

Ruby: raise ArgumentError, "错误信息"
来源：http://oqh.xuanzx.com

C#:   throw new ArgumentException("错误信息");
来源：http://gqs.daxiang520.top

[H04] 自定义异常类型
来源：http://pug.zhiwuduotai.top

Py:   class MyError(Exception): pass
来源：http://evv.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hcs.yuanzhike.top

JS:   class MyError extends Error {}
来源：http://fxg.redwolf501.top

TS:   class MyError extends Error {}
来源：http://lvz.sxryk.cn

Java: class MyException extends RuntimeException {}
来源：http://skg.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zof.meibo888.top

Ruby: class MyError < StandardError; end
来源：http://poj.9152youxi.cn

C#:   class MyException : Exception {}
来源：http://cwa.havefunace.top

[H05] 捕获特定类型
来源：http://jnc.yueranfly.top

Py:   except ValueError as e:
来源：http://itg.haohaochexian.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vla.fehbvm.com

JS:   if (e instanceof TypeError) {}
来源：http://lpx.chenzaomai.com

TS:   if (e instanceof TypeError) {}
来源：http://yfa.cucudq.cn

Java: catch (IOException | SQLException e) {}
来源：http://lse.uphjek.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oyw.zdbjq.cn

Ruby: rescue ArgumentError => e
来源：http://red.52xcode.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vad.smart0.xyz

[H06] 可选值 / 空值安全访问
来源：http://qil.yfazqb.com

Py:   value = d.get("k") or default
来源：http://kdw.shzxlz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uym.xinyue.icu

JS:   obj?.a?.b;  d ?? default
来源：http://vqs.jinqigufen.top

TS:   obj?.a?.b;  d ?? default
来源：http://cxb.zycfv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lxd.zdqjudy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hdd.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://von.xylfe.cn

C#:   obj?.A?.B ?? default
来源：http://vcd.fzhhl.top

[H07] 断言
来源：http://ndn.wangshuangyany.cn

Py:   assert x > 0, "必须为正"
来源：http://fwh.jiagoushi.top

PHP:  assert($x > 0);
来源：http://tsq.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://lxt.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://dnw.tian-w.cn

Java: assert x > 0 : "必须为正";
来源：http://njz.jianghu66.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cxp.zdbjq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kji.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://mfh.nwbrower.top

[H08] 获取错误信息与堆栈
来源：http://edk.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://xyu.hcnkem.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mbd.andypj.xyz

JS:   e.message;  e.stack
来源：http://bww.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://neb.shanyushiyangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pdy.tanke756.top

Go:   err.Error()
来源：http://hvs.yuxming.cn

Ruby: e.message;  e.backtrace
来源：http://fvl.wangshuangyany.cn

C#:   e.Message;  e.StackTrace
来源：http://kvg.jqgfzy.top

[H09] 带错误码的异常
来源：http://kne.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://keo.smart0.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://mua.sufxvd.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://miy.xuanzx.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yeu.wangdashe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ziw.zhiwuduotai.top


<!-- 参考信息 -->