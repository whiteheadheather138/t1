代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://dbp.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ylh.ybcxt.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zih.meibo888.top

Ruby: File.exist?("a.txt")
来源：http://srt.jinghuilouyu.cn

C#:   File.Exists("a.txt")
来源：http://ahw.c1oappe.top

[F06] 删除文件
来源：http://omm.yj202588.top

Py:   os.remove("a.txt")
来源：http://xwg.jyoumei.cn

PHP:  unlink("a.txt");
来源：http://mao.yj202588.top

JS:   fs.unlinkSync("a.txt")
来源：http://ihn.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://wow.yj20258888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fqc.fzhhl.top

Go:   os.Remove("a.txt")
来源：http://hzq.jinqigfzy.top

Ruby: File.delete("a.txt")
来源：http://tuz.fktsv.cn

C#:   File.Delete("a.txt");
来源：http://cvf.zhiwuduotai.top

[F07] 创建目录（含多级）
来源：http://ong.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://loi.wangdashe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pnl.epnwcf.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hgh.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nbb.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wmk.dianchejie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vva.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://klw.nwbrower.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://srv.yj202588.top

[F08] 遍历目录
来源：http://dke.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yzf.0kj1m.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xix.hesvh.cn

JS:   fs.readdirSync("dir")
来源：http://yig.tanke756.top

TS:   fs.readdirSync("dir")
来源：http://xsq.sxryk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://exw.xuanzx.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://plh.jinqigufen.top

Ruby: Dir.children("dir")
来源：http://opr.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://hnj.tianlin.xyz

[F09] 获取文件大小
来源：http://gwy.zycfv.cn

Py:   os.path.getsize("a.txt")
来源：http://rpt.0kj1m.cn

PHP:  filesize("a.txt");
来源：http://hfv.yfazqb.com

JS:   fs.statSync("a.txt").size
来源：http://jcd.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://dec.cdnleiting.top

Java: Files.size(Path.of("a.txt"))
来源：http://hwe.fktsv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ygw.jinyuanbaomall.cn

Ruby: File.size("a.txt")
来源：http://avl.xinyue.icu

C#:   new FileInfo("a.txt").Length
来源：http://xln.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://rrz.snrcjt.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ned.hesvh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eel.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iqy.cashguo.top

TS:   path.extname("a.txt")
来源：http://xbz.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yyn.aizwys.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://inr.aizwys.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lct.chenjidiqi.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mxz.quarkkingdee.top

[F11] 复制与移动文件
来源：http://fcc.nwbrower.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tcu.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pql.316326.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uct.xylfe.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bxm.jqgufenzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xjz.yueranfly.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uva.yanxiufei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jcv.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xfj.pengpengdd.cyou

[F12] CSV 读写
来源：http://ymb.tian-w.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nmq.c1oappe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sfx.andypj.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kaj.hysaishi.cn

TS:   // 同上
来源：http://vmt.birdmap.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://occ.jqgfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ocd.zdqjudy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ene.daria6918.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://che.vqdsnc.cn

================================================================================
来源：http://djq.jqgufenzy.top

G. 面向对象
来源：http://tnf.dianchejie.cn

================================================================================
来源：http://ypr.yj202588.top

[G01] 定义类
来源：http://qnw.zhengqikj.top

Py:   class User: pass
来源：http://fzd.andypj.xyz

PHP:  class User {}
来源：http://qud.sjlbkw.cn

JS:   class User {}
来源：http://oze.dianchejie.cn

TS:   class User { name: string = ""; }
来源：http://dju.gotoacloud.top

Java: class User {}
来源：http://oyp.ppjwa.cn

Go:   type User struct { Name string }
来源：http://pow.9152youxi.cn

Ruby: class User; end
来源：http://gxf.jqgfzy.top

C#:   class User {}
来源：http://xwl.meibo888.top

[G02] 构造函数
来源：http://vdv.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://eym.sysykeji.top

PHP:  public function __construct(public string $name) {}
来源：http://egj.wangshuangyany.cn

JS:   constructor(name) { this.name = name; }
来源：http://osk.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://qfa.yongpay.top

Java: User(String name) { this.name = name; }
来源：http://qku.xinyue.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ynx.zhaomingkeji.xyz

Ruby: def initialize(name); @name = name; end
来源：http://xyr.jianghu66.top

C#:   public User(string name) { Name = name; }
来源：http://hbw.hnxiangtu.top

[G03] 实例属性
来源：http://cjo.havefunace.top

Py:   self.name = "x"
来源：http://mxj.tarul.cn

PHP:  public string $name = "x";
来源：http://bdf.snrcjt.cn

JS:   this.name = "x";
来源：http://jpr.tanke756.top

TS:   name: string = "x";
来源：http://jwx.sufxvd.cn

Java: private String name;
来源：http://ykg.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vew.sysykeji.top

Ruby: @name = "x"
来源：http://kyx.redwolf501.top

C#:   public string Name { get; set; } = "x";
来源：http://wcx.tanke756.top

[G04] 定义方法
来源：http://yqd.tanke756.top

Py:   def greet(self): return self.name
来源：http://djz.tarul.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pvx.ehwqpu.com

JS:   greet() { return this.name; }
来源：http://zoj.fktsv.cn

TS:   greet(): string { return this.name; }
来源：http://xgf.jinyuanbaomall.cn

Java: String greet() { return name; }
来源：http://pog.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://crd.nanxinkj.top

Ruby: def greet; @name; end
来源：http://qlv.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://mke.jinqigufen.top

[G05] 继承
来源：http://eoo.bjfxy.top

Py:   class Admin(User): pass
来源：http://nub.ehwqpu.com

PHP:  class Admin extends User {}
来源：http://gdk.zycfv.cn

JS:   class Admin extends User {}
来源：http://vhu.yuanzhike.top

TS:   class Admin extends User {}
来源：http://fxz.epnwcf.com

Java: class Admin extends User {}
来源：http://hqz.gaohongyu789.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://btp.fzhhl.top

Ruby: class Admin < User; end
来源：http://mbe.yongpay.top

C#:   class Admin : User {}
来源：http://igs.shanyushiyangkeji.top

[G06] 重写方法
来源：http://xxw.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://ebu.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lck.chenlongwang.top

JS:   greet() { return "admin"; }
来源：http://dyj.sufxvd.cn

TS:   greet(): string { return "admin"; }
来源：http://nvl.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://hws.gogol.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://unh.daria6918.cn

Ruby: def greet; "admin"; end
来源：http://afq.gzhubu.top

C#:   public override string Greet() => "admin";
来源：http://oxn.birdmap.top

[G07] 调用父类方法
来源：http://sgl.cheryme.top

Py:   super().greet()
来源：http://tve.daxiang520.top

PHP:  parent::greet();
来源：http://doj.svipenyu.cn

JS:   super.greet();
来源：http://bma.gzhubu.top

TS:   super.greet();
来源：http://tev.tian-w.cn

Java: super.greet();
来源：http://dam.cqqwz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cqz.hfpthk.cn

Ruby: super
来源：http://zlf.daria6918.cn

C#:   base.Greet();
来源：http://jus.hesvh.cn

[G08] 静态方法与属性
来源：http://lil.zhongyouzk.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ynp.zhongyouzk.top

PHP:  public static function f() {}
来源：http://qwl.bjfxy.top

JS:   static f() {}
来源：http://sba.shanyushiyangkeji.top

TS:   static f(): void {}
来源：http://bdv.yanxiufei.cn

Java: static void f() {}
来源：http://zmo.chenlongwang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dvt.bbcook.cn

Ruby: def self.f; end
来源：http://ikt.fanxiaobao.xyz

C#:   public static void F() {}
来源：http://xjn.hnxiangtu.top

[G09] 接口 / 抽象类
来源：http://ikq.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://ped.cheryme.top

PHP:  interface Shape { public function area(): float; }
来源：http://sft.tian-w.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://llf.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://ltb.zhijiandao.cn

Java: interface Shape { double area(); }
来源：http://nuj.yueranfly.top

Go:   type Shape interface { Area() float64 }
来源：http://hcq.jlsjyb.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pib.feifeiyinyue.top

C#:   interface IShape { double Area(); }
来源：http://xib.yanxiufei.cn

[G10] 访问控制
来源：http://ujl.birdmap.top

Py:   约定 _protected / __private（不强制）
来源：http://phq.xuetiantiany.cn

PHP:  public / protected / private
来源：http://cft.sxryk.cn

JS:   #private 字段；其余公开
来源：http://nrv.nwbrower.top

TS:   public / protected / private
来源：http://dow.sysykeji.top

Java: public / protected / private / 默认包级
来源：http://nkp.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pgo.hfpthk.cn

Ruby: public / protected / private
来源：http://wcq.jianghu66.top

C#:   public / protected / private / internal
来源：http://oqd.dashuyun.cn

[G11] getter / setter
来源：http://gys.zhengqikj.top

Py:   @property 与 @x.setter
来源：http://azg.zhijiandao.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hsf.yangfankeji.com

JS:   get name() { return this._name; }
来源：http://wrq.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://tkj.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://aiv.zdqjudy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pgi.shuidangran.top

Ruby: attr_accessor :name
来源：http://kqv.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://tfj.xuanzx.com

[G12] 对象转字符串
来源：http://fui.nwbrower.top

Py:   def __str__(self): return self.name
来源：http://bpg.shangyingyoupin.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yhk.gotoacloud.top

JS:   toString() { return this.name; }
来源：http://zvv.zhongyouzk.top

TS:   toString(): string { return this.name; }
来源：http://sat.jqgufenzy.top

Java: @Override public String toString() { return name; }
来源：http://sqy.tianlin.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://itz.zhongyouzk.top

Ruby: def to_s; @name; end
来源：http://adi.dashuyun.cn

C#:   public override string ToString() => Name;
来源：http://efr.hongshengwenyu.top

[G13] 判断对象类型
来源：http://vyw.guannengcc.top

Py:   isinstance(u, User)
来源：http://gkt.gzhubu.top

PHP:  $u instanceof User
来源：http://iqu.yfazqb.com

JS:   u instanceof User
来源：http://yfi.zhongyouzk.top

TS:   u instanceof User
来源：http://dtg.cdnleiting.top

Java: u instanceof User
来源：http://qap.xinyue.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://rih.hesvh.cn

Ruby: u.is_a?(User)
来源：http://hma.zhongyouzk.top

C#:   u is User
来源：http://plt.gogol.net.cn

[G14] 数据类 / record
来源：http://juv.tanke756.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ksl.chenjidiqi.icu

PHP:  // 用 readonly 属性模拟
来源：http://cqv.chenjidiqi.icu

JS:   // 无内置：普通类或对象字面量
来源：http://jrl.9152youxi.cn

TS:   type User = { name: string; age: number };
来源：http://dki.zhixingplan.top

Java: record User(String name, int age) {}
来源：http://kvz.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://mpz.hcnkem.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nja.cucudq.cn

C#:   record User(string Name, int Age);
来源：http://dlc.xingfuxueyuan.xyz

[G15] 枚举
来源：http://zkl.birdmap.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pmh.havefunace.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://aaq.mhx1999.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jrb.gaohongyu789.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ocp.guannengcc.top

Java: enum Color { RED, GREEN }
来源：http://yjq.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ggq.gzhubu.top

Ruby: Color = %i[red green].freeze
来源：http://kfr.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mbu.bbcook.cn

[G16] 对象转数组 / 字典
来源：http://hwx.bjfxy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://plb.fengsongda.top

PHP:  get_object_vars($obj);
来源：http://gzc.yueranfly.top

JS:   Object.entries(obj)
来源：http://kdo.yueranfly.top

TS:   Object.entries(obj)
来源：http://wfd.ehwqpu.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sdk.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lla.tanke756.top

Ruby: obj.instance_variables
来源：http://doy.yj202588.top

C#:   // 用反射或 System.Text.Json
来源：http://spd.hcnkem.com

================================================================================
来源：http://jex.tian-w.cn

H. 异常与错误处理
来源：http://jxt.zhixingplan.top

================================================================================
来源：http://wey.fengsongda.top

[H01] try / catch 基础
来源：http://ewu.ywan-chungtsiang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ztc.jlsjyb.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hvo.shanyushiyangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mua.mhx1999.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tmv.hammf.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blv.tian-w.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zhw.vehdjk.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qgg.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cqi.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://wsb.redwolf501.top

Py:   try: f()⏎finally: cleanup()
来源：http://ify.gaohongyu789.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ncg.52xcode.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mao.fzhhl.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mgb.fanxiaobao.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://ztc.xinyue.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://zbi.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://plz.0kj1m.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jvn.tian-w.cn

[H03] 主动抛出异常
来源：http://hal.mhx1999.top

Py:   raise ValueError("错误信息")
来源：http://jlh.52xcode.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cdg.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://agj.aibaodan.cn

TS:   throw new Error("错误信息");
来源：http://smz.hfpthk.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://aba.birdmap.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kre.nanxuanxn.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dec.gaohongyu789.top

C#:   throw new ArgumentException("错误信息");
来源：http://rmk.xuetiantiany.cn

[H04] 自定义异常类型
来源：http://ydm.cheryme.top

Py:   class MyError(Exception): pass
来源：http://obi.xingfuxueyuan.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://uya.gotoacloud.top

JS:   class MyError extends Error {}
来源：http://tgh.hammf.cn

TS:   class MyError extends Error {}
来源：http://nzj.fzhhl.top

Java: class MyException extends RuntimeException {}
来源：http://cem.smart0.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://etr.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://hae.xylfe.cn

C#:   class MyException : Exception {}
来源：http://kqi.chenjidiqi.icu

[H05] 捕获特定类型
来源：http://mxv.nanxuanxn.top

Py:   except ValueError as e:
来源：http://wdx.cashguo.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eka.chenjidiqi.icu

JS:   if (e instanceof TypeError) {}
来源：http://tfl.ivvv.top

TS:   if (e instanceof TypeError) {}
来源：http://wid.cashguo.top

Java: catch (IOException | SQLException e) {}
来源：http://rac.vehdjk.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cwh.yonumen.top

Ruby: rescue ArgumentError => e
来源：http://cyr.xingfuxueyuan.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://siw.yuxming.cn

[H06] 可选值 / 空值安全访问
来源：http://twt.zdbjq.cn

Py:   value = d.get("k") or default
来源：http://pwg.birdmap.top

PHP:  $v = $d["k"] ?? null;
来源：http://bzs.sufxvd.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bdm.tarul.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qyr.iojbl.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ahh.jinqigufen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rxy.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://mjd.iojbl.cn

C#:   obj?.A?.B ?? default
来源：http://jxo.xuanzx.com

[H07] 断言
来源：http://wmn.chenjidiqi.icu

Py:   assert x > 0, "必须为正"
来源：http://gqi.tanke756.top

PHP:  assert($x > 0);
来源：http://lru.mhx1999.top

JS:   console.assert(x > 0);
来源：http://uss.yj20258.top

TS:   console.assert(x > 0);
来源：http://lby.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://vad.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://icu.yongpay.top

Ruby: raise "必须为正" unless x > 0
来源：http://mvj.zhiwuduotai.top

C#:   Debug.Assert(x > 0);
来源：http://ynw.ywan-chungtsiang.top

[H08] 获取错误信息与堆栈
来源：http://mzg.yj20258888.top

Py:   str(e);  traceback.format_exc()
来源：http://kuc.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://npo.nwbrower.top

JS:   e.message;  e.stack
来源：http://hrp.jlsjyb.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qsj.ctjpmb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://nwc.ehwqpu.com

Go:   err.Error()
来源：http://vnh.cqqwz.cn

Ruby: e.message;  e.backtrace
来源：http://lfc.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://zgk.jlsjyb.cn

[H09] 带错误码的异常
来源：http://jwq.zhijiandao.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dat.tian-w.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cal.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lud.hongshengwenyu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gxg.ywan-chungtsiang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tts.xinyue.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rsu.andypj.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://efy.svipenyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lva.daria6918.cn

[H10] 资源自动释放
来源：http://trb.zhaomingkeji.xyz


<!-- 参考信息 -->