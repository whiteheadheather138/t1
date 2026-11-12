代发 wailian999

Ruby: File.delete("a.txt")
来源：http://shx.yangfankeji.com

C#:   File.Delete("a.txt");
来源：http://xka.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://klq.iojbl.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://htc.yanxiufei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zxj.xingfuxueyuan.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vgc.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vei.fzhhl.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://osn.jinqigfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zlj.yueranfly.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://spz.redwolf501.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vfu.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://bun.jiagoushi.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kkd.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ajx.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://vxd.kuanghao11.cn

TS:   fs.readdirSync("dir")
来源：http://uxe.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qoj.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://ofc.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://pej.hcnkem.com

C#:   Directory.GetFiles("dir")
来源：http://ysh.9152youxi.cn

[F09] 获取文件大小
来源：http://hmb.jiagoushi.top

Py:   os.path.getsize("a.txt")
来源：http://hmc.zdbjq.cn

PHP:  filesize("a.txt");
来源：http://rfl.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://jgg.tianlin.xyz

TS:   fs.statSync("a.txt").size
来源：http://med.daria6918.cn

Java: Files.size(Path.of("a.txt"))
来源：http://per.mhx1999.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jml.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://gbj.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://fyn.vqdsnc.cn

[F10] 取文件扩展名 / 文件名
来源：http://ula.meibo888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qss.chenjidiqi.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://asc.shuidangran.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ggn.hammf.cn

TS:   path.extname("a.txt")
来源：http://cwi.vqdsnc.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zol.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nbm.sxryk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ijh.hammf.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rsm.jyoumei.cn

[F11] 复制与移动文件
来源：http://xib.ehwqpu.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pht.jlsjyb.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dtx.gotoacloud.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vsk.hnqzz.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mbc.jinyuanbaomall.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nbq.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yed.gogol.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zms.xuanzx.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qtg.zhongyouzk.top

[F12] CSV 读写
来源：http://wcv.chenlongwang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iix.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ssw.iojbl.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ckg.xuetiantiany.cn

TS:   // 同上
来源：http://opy.fzhhl.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tdm.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ccm.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lux.hysaishi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wiq.guannengcc.top

================================================================================
来源：http://msf.hnxiangtu.top

G. 面向对象
来源：http://jtn.daria6918.cn

================================================================================
来源：http://sru.xingfuxueyuan.xyz

[G01] 定义类
来源：http://ljw.chenlongwang.top

Py:   class User: pass
来源：http://tly.sysykeji.top

PHP:  class User {}
来源：http://kig.zhiwuduotai.top

JS:   class User {}
来源：http://amf.zhaomingkeji.xyz

TS:   class User { name: string = ""; }
来源：http://spj.fengsongda.top

Java: class User {}
来源：http://dpx.guannengcc.top

Go:   type User struct { Name string }
来源：http://gol.daria6918.cn

Ruby: class User; end
来源：http://wtn.xylfe.cn

C#:   class User {}
来源：http://eld.xylfe.cn

[G02] 构造函数
来源：http://wlf.9152youxi.cn

Py:   def __init__(self, name): self.name = name
来源：http://pzd.c1oappe.top

PHP:  public function __construct(public string $name) {}
来源：http://jrt.jinqigfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://ikj.xuetiantiany.cn

TS:   constructor(public name: string) {}
来源：http://jey.xuetiantiany.cn

Java: User(String name) { this.name = name; }
来源：http://jui.yueranfly.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yww.zhiwuduotai.top

Ruby: def initialize(name); @name = name; end
来源：http://wbb.zhiwuduotai.top

C#:   public User(string name) { Name = name; }
来源：http://pyw.zhiwuduotai.top

[G03] 实例属性
来源：http://fcs.fehbvm.com

Py:   self.name = "x"
来源：http://npb.316326.xyz

PHP:  public string $name = "x";
来源：http://duq.cqqwz.cn

JS:   this.name = "x";
来源：http://mra.dashuyun.cn

TS:   name: string = "x";
来源：http://rac.jqgufenzy.top

Java: private String name;
来源：http://zye.nwbrower.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tli.dianchejie.cn

Ruby: @name = "x"
来源：http://mcl.cashguo.top

C#:   public string Name { get; set; } = "x";
来源：http://hhe.jinyuanbaomall.cn

[G04] 定义方法
来源：http://mou.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://rsi.hnxiangtu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rux.fktsv.cn

JS:   greet() { return this.name; }
来源：http://kid.tanke756.top

TS:   greet(): string { return this.name; }
来源：http://vyx.c1oappe.top

Java: String greet() { return name; }
来源：http://isb.hysaishi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zal.dianchejie.cn

Ruby: def greet; @name; end
来源：http://xba.havefunace.top

C#:   public string Greet() => Name;
来源：http://pnn.sxryk.cn

[G05] 继承
来源：http://ipp.shzxlz.cn

Py:   class Admin(User): pass
来源：http://gym.fanxiaobao.xyz

PHP:  class Admin extends User {}
来源：http://xdj.gzhubu.top

JS:   class Admin extends User {}
来源：http://hrn.feifeiyinyue.top

TS:   class Admin extends User {}
来源：http://ixm.xuanzx.com

Java: class Admin extends User {}
来源：http://ytk.nanxuanxn.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iul.gzhubu.top

Ruby: class Admin < User; end
来源：http://cli.guowangkeji.top

C#:   class Admin : User {}
来源：http://mti.jiagoushi.top

[G06] 重写方法
来源：http://puq.sufxvd.cn

Py:   def greet(self): return "admin"
来源：http://hqx.shuidangran.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wmr.zhoulong.xyz

JS:   greet() { return "admin"; }
来源：http://osx.yj202588.top

TS:   greet(): string { return "admin"; }
来源：http://xfl.0kj1m.cn

Java: @Override String greet() { return "admin"; }
来源：http://dug.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oeg.bbcook.cn

Ruby: def greet; "admin"; end
来源：http://ika.fehbvm.com

C#:   public override string Greet() => "admin";
来源：http://tkm.hammf.cn

[G07] 调用父类方法
来源：http://qgj.jlsjyb.cn

Py:   super().greet()
来源：http://cyd.nanxinkj.top

PHP:  parent::greet();
来源：http://wec.jqgfzy.top

JS:   super.greet();
来源：http://nry.zhiwuduotai.top

TS:   super.greet();
来源：http://myw.nwbrower.top

Java: super.greet();
来源：http://tfw.snrcjt.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qcf.iojbl.cn

Ruby: super
来源：http://pfv.kuanghao11.cn

C#:   base.Greet();
来源：http://kog.jiagoushi.top

[G08] 静态方法与属性
来源：http://ebx.fanxiaobao.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://osz.haohaochexian.top

PHP:  public static function f() {}
来源：http://ynj.zycfv.cn

JS:   static f() {}
来源：http://ckm.nanxinkj.top

TS:   static f(): void {}
来源：http://iom.zdqjudy.top

Java: static void f() {}
来源：http://xab.cdnleiting.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kvk.yangfankeji.com

Ruby: def self.f; end
来源：http://yey.zhaomingkeji.xyz

C#:   public static void F() {}
来源：http://vls.hnxiangtu.top

[G09] 接口 / 抽象类
来源：http://lna.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://bdc.fanxiaobao.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://gcm.sjlbkw.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tkw.xinyue.icu

TS:   interface Shape { area(): number; }
来源：http://cpr.daxiang520.top

Java: interface Shape { double area(); }
来源：http://car.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://pft.haohaochexian.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ort.cdnleiting.top

C#:   interface IShape { double Area(); }
来源：http://fyx.ppjwa.cn

[G10] 访问控制
来源：http://are.jinqigfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://rnp.svipenyu.cn

PHP:  public / protected / private
来源：http://hny.tanke756.top

JS:   #private 字段；其余公开
来源：http://dpw.epnwcf.com

TS:   public / protected / private
来源：http://ato.sxryk.cn

Java: public / protected / private / 默认包级
来源：http://lwz.316326.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://dtv.chenjidiqi.icu

Ruby: public / protected / private
来源：http://dmm.jyoumei.cn

C#:   public / protected / private / internal
来源：http://gzt.jinqigufen.top

[G11] getter / setter
来源：http://ahh.chenjidiqi.icu

Py:   @property 与 @x.setter
来源：http://iky.pycfn.com

PHP:  public function getName(): string { return $this->name; }
来源：http://kgz.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://nqc.sysykeji.top

TS:   get name(): string { return this._name; }
来源：http://iqn.xuanzx.com

Java: public String getName() { return name; }
来源：http://mel.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://aub.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://roo.zycfv.cn

C#:   public string Name { get; set; }
来源：http://dxu.zhengqikj.top

[G12] 对象转字符串
来源：http://fer.redwolf501.top

Py:   def __str__(self): return self.name
来源：http://dle.cheryme.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gai.yfazqb.com

JS:   toString() { return this.name; }
来源：http://njq.xingfuxueyuan.xyz

TS:   toString(): string { return this.name; }
来源：http://qiq.hcnkem.com

Java: @Override public String toString() { return name; }
来源：http://tft.jqgfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://mrs.yvedp.cn

Ruby: def to_s; @name; end
来源：http://vvz.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://zud.smart0.xyz

[G13] 判断对象类型
来源：http://eji.jqgfzy.top

Py:   isinstance(u, User)
来源：http://pdz.c1oappe.top

PHP:  $u instanceof User
来源：http://fho.pengpengdd.cyou

JS:   u instanceof User
来源：http://uly.vqdsnc.cn

TS:   u instanceof User
来源：http://bko.feifeiyinyue.top

Java: u instanceof User
来源：http://hqa.xuanzx.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://pzv.sweek.top

Ruby: u.is_a?(User)
来源：http://qyf.yuanzhike.top

C#:   u is User
来源：http://dnh.wangdashe.top

[G14] 数据类 / record
来源：http://wvq.xingfuxueyuan.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yby.yueranfly.top

PHP:  // 用 readonly 属性模拟
来源：http://fsr.cucudq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ljc.cdnleiting.top

TS:   type User = { name: string; age: number };
来源：http://zaf.bjfxy.top

Java: record User(String name, int age) {}
来源：http://wdl.cdnleiting.top

Go:   type User struct { Name string; Age int }
来源：http://txq.jqgfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sen.zhongyouzk.top

C#:   record User(string Name, int Age);
来源：http://pwm.gzhubu.top

[G15] 枚举
来源：http://blt.nanxinkj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ywq.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://ltf.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lye.epnwcf.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tmy.shuidangran.top

Java: enum Color { RED, GREEN }
来源：http://eij.jqgufenzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uyx.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://kko.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hrm.zhiwuduotai.top

[G16] 对象转数组 / 字典
来源：http://wtv.wangdashe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sgh.yj20258888.top

PHP:  get_object_vars($obj);
来源：http://var.shuidangran.top

JS:   Object.entries(obj)
来源：http://hyr.vqdsnc.cn

TS:   Object.entries(obj)
来源：http://zyw.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iln.gotoacloud.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hlq.zhiwuduotai.top

Ruby: obj.instance_variables
来源：http://wab.yj202588.top

C#:   // 用反射或 System.Text.Json
来源：http://mio.jiagoushi.top

================================================================================
来源：http://bqc.dashuyun.cn

H. 异常与错误处理
来源：http://xkx.xuetiantiany.cn

================================================================================
来源：http://ite.andypj.xyz

[H01] try / catch 基础
来源：http://zag.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xnh.ppjwa.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ovg.yuxming.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gay.shangyingyoupin.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://knp.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sap.ivvv.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cre.tian-w.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iql.cashguo.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aqh.zhijiandao.cn

[H02] finally / ensure 收尾
来源：http://kqd.chenlongwang.top

Py:   try: f()⏎finally: cleanup()
来源：http://mzp.snrcjt.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lar.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jhc.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://byk.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://sez.jlsjyb.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jrc.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://csi.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://tip.shangyingyoupin.top

[H03] 主动抛出异常
来源：http://ray.cheryme.top

Py:   raise ValueError("错误信息")
来源：http://nhu.birdmap.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://shw.nwbrower.top

JS:   throw new Error("错误信息");
来源：http://iza.mhx1999.top

TS:   throw new Error("错误信息");
来源：http://eec.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://des.yueranfly.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qxl.birdmap.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pyl.fengsongda.top

C#:   throw new ArgumentException("错误信息");
来源：http://csy.jinqigufen.top

[H04] 自定义异常类型
来源：http://drr.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://xtn.yj20258888.top

PHP:  class MyError extends RuntimeException {}
来源：http://diu.hesvh.cn

JS:   class MyError extends Error {}
来源：http://fzw.gzhubu.top

TS:   class MyError extends Error {}
来源：http://kwk.tanke756.top

Java: class MyException extends RuntimeException {}
来源：http://kzw.shzxlz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tfg.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://dru.zhijiandao.cn

C#:   class MyException : Exception {}
来源：http://vla.jianghu66.top

[H05] 捕获特定类型
来源：http://vsw.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://hst.fanxiaobao.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fci.ydzc1.top

JS:   if (e instanceof TypeError) {}
来源：http://mxb.9152youxi.cn

TS:   if (e instanceof TypeError) {}
来源：http://qpe.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://pdz.vehdjk.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yxy.yfazqb.com

Ruby: rescue ArgumentError => e
来源：http://utk.9152youxi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lmq.hywenlv.cn

[H06] 可选值 / 空值安全访问
来源：http://byk.hammf.cn

Py:   value = d.get("k") or default
来源：http://mzg.sysykeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://org.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://rga.zdqjudy.top

TS:   obj?.a?.b;  d ?? default
来源：http://msl.ivvv.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rns.0kj1m.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mts.hammf.cn

Ruby: d&.dig(:a, :b)
来源：http://jhv.9152youxi.cn

C#:   obj?.A?.B ?? default
来源：http://byp.kuanghao11.cn

[H07] 断言
来源：http://avm.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://hyo.tanke756.top

PHP:  assert($x > 0);
来源：http://otw.xuetiantiany.cn

JS:   console.assert(x > 0);
来源：http://bab.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://qft.nanxinkj.top

Java: assert x > 0 : "必须为正";
来源：http://xbv.meibo888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qwz.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lww.shanyushiyangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://tbg.fehbvm.com

[H08] 获取错误信息与堆栈
来源：http://sxm.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://qkn.tian-w.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zad.fzhhl.top

JS:   e.message;  e.stack
来源：http://pux.tanke756.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cpc.xziqi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oha.hnqzz.top

Go:   err.Error()
来源：http://oun.xuetiantiany.cn

Ruby: e.message;  e.backtrace
来源：http://ilm.havefunace.top

C#:   e.Message;  e.StackTrace
来源：http://ptz.zhaomingkeji.xyz

[H09] 带错误码的异常
来源：http://yjh.sjlbkw.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gel.zhaomingkeji.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://ske.svipenyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hbr.guowangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jzo.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vyt.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hyo.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://jaj.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://tkp.vehdjk.com

[H10] 资源自动释放
来源：http://rjn.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kca.fzhhl.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oue.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uke.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://txd.c1oappe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dnt.snrcjt.cn

Go:   defer f.Close()
来源：http://kit.yueranfly.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ltr.tanke756.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://udy.gotoacloud.top

================================================================================
来源：http://xfe.redwolf501.top

I. 正则表达式
来源：http://qce.hongshengwenyu.top

================================================================================
来源：http://mpe.dashuyun.cn

[I01] 判断是否匹配
来源：http://swg.zhoulong.xyz


<!-- 参考信息 -->