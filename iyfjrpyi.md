代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vri.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iev.hysaishi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://abn.yj202588.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xve.c1oappe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uzc.xinyue.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mhc.cashguo.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gxm.uphjek.com

[F08] 遍历目录
来源：http://hzz.yonumen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://omu.daxiang520.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://efn.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://opr.zhoulong.xyz

TS:   fs.readdirSync("dir")
来源：http://nnv.havefunace.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://glq.tian-w.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jgl.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://qhl.bjfxy.top

C#:   Directory.GetFiles("dir")
来源：http://wyg.shanyushiyangtech.top

[F09] 获取文件大小
来源：http://mgl.yvedp.cn

Py:   os.path.getsize("a.txt")
来源：http://wlz.wangdashe.top

PHP:  filesize("a.txt");
来源：http://hxv.nanxuanxn.top

JS:   fs.statSync("a.txt").size
来源：http://znh.zhongyouzk.top

TS:   fs.statSync("a.txt").size
来源：http://awx.shzxlz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zpj.shanyushiyangtech.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zmz.0kj1m.cn

Ruby: File.size("a.txt")
来源：http://svk.ehwqpu.com

C#:   new FileInfo("a.txt").Length
来源：http://azp.ydzc1.top

[F10] 取文件扩展名 / 文件名
来源：http://gcj.316326.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kse.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jrn.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hhr.hywenlv.cn

TS:   path.extname("a.txt")
来源：http://xhg.birdmap.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://twk.feifeiyinyue.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yyw.wangshuangyany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ojb.52xcode.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rsl.yangfankeji.com

[F11] 复制与移动文件
来源：http://kpk.xingfuxueyuan.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tny.aibaodan.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oxy.svipenyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tip.yj20258888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rtq.zhaomingkeji.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sgn.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pje.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sfr.ywan-chungtsiang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zgu.yfazqb.com

[F12] CSV 读写
来源：http://qvo.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mkt.redwolf501.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cpg.yongpay.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qqn.andypj.xyz

TS:   // 同上
来源：http://jmd.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sgy.hfpthk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qfy.dianchejie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://shu.xuetiantiany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vnf.0kj1m.cn

================================================================================
来源：http://qdv.ctjpmb.com

G. 面向对象
来源：http://dsn.sysykeji.top

================================================================================
来源：http://ybw.gzhubu.top

[G01] 定义类
来源：http://dsa.daxiang520.top

Py:   class User: pass
来源：http://xhs.ywan-chungtsiang.top

PHP:  class User {}
来源：http://mwd.jinqigfzy.top

JS:   class User {}
来源：http://mpe.52xcode.cn

TS:   class User { name: string = ""; }
来源：http://jsk.hysaishi.cn

Java: class User {}
来源：http://wbx.sysykeji.top

Go:   type User struct { Name string }
来源：http://bxu.hywenlv.cn

Ruby: class User; end
来源：http://eno.cdnleiting.top

C#:   class User {}
来源：http://jnb.kuanghao11.cn

[G02] 构造函数
来源：http://kjd.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://hay.uphjek.com

PHP:  public function __construct(public string $name) {}
来源：http://gld.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://qmc.zhiwuduotai.top

TS:   constructor(public name: string) {}
来源：http://mtv.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://nrd.tianlin.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qnc.jqgfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://qrt.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://jpk.hammf.cn

[G03] 实例属性
来源：http://ijy.yanxiufei.cn

Py:   self.name = "x"
来源：http://yzz.pengpengdd.cyou

PHP:  public string $name = "x";
来源：http://eno.0kj1m.cn

JS:   this.name = "x";
来源：http://rsz.daxiang520.top

TS:   name: string = "x";
来源：http://xqz.tanke756.top

Java: private String name;
来源：http://ebn.zhiwuduotai.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rnv.wangdashe.top

Ruby: @name = "x"
来源：http://dhi.hywenlv.cn

C#:   public string Name { get; set; } = "x";
来源：http://fzz.sysykeji.top

[G04] 定义方法
来源：http://ndh.yuxming.cn

Py:   def greet(self): return self.name
来源：http://dps.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ldc.316326.xyz

JS:   greet() { return this.name; }
来源：http://uzw.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://ohh.zdqjudy.top

Java: String greet() { return name; }
来源：http://ypo.jinghuilouyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fpa.yueranfly.top

Ruby: def greet; @name; end
来源：http://jxp.hcnkem.com

C#:   public string Greet() => Name;
来源：http://trv.uphjek.com

[G05] 继承
来源：http://rct.fehbvm.com

Py:   class Admin(User): pass
来源：http://djt.quarkkingdee.top

PHP:  class Admin extends User {}
来源：http://wdh.zhoulong.xyz

JS:   class Admin extends User {}
来源：http://anv.quarkkingdee.top

TS:   class Admin extends User {}
来源：http://tyw.jyoumei.cn

Java: class Admin extends User {}
来源：http://fnp.hongshengwenyu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dqf.ybcxt.top

Ruby: class Admin < User; end
来源：http://jxd.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://lvi.zdqjudy.top

[G06] 重写方法
来源：http://ifq.shanyushiyangtech.top

Py:   def greet(self): return "admin"
来源：http://cbz.epnwcf.com

PHP:  public function greet(): string { return "admin"; }
来源：http://wgb.yueranfly.top

JS:   greet() { return "admin"; }
来源：http://nik.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://aug.jinyuanbaomall.cn

Java: @Override String greet() { return "admin"; }
来源：http://orj.aibaodan.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uhm.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://vvd.fzhhl.top

C#:   public override string Greet() => "admin";
来源：http://wil.ybcxt.top

[G07] 调用父类方法
来源：http://xfq.yj20258888.top

Py:   super().greet()
来源：http://xqy.yangfankeji.com

PHP:  parent::greet();
来源：http://pie.daria6918.cn

JS:   super.greet();
来源：http://aqd.nanxinkj.top

TS:   super.greet();
来源：http://xnh.fzhhl.top

Java: super.greet();
来源：http://maa.redwolf501.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wwh.cashguo.top

Ruby: super
来源：http://ebr.dashuyun.cn

C#:   base.Greet();
来源：http://nid.gzhubu.top

[G08] 静态方法与属性
来源：http://eaz.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://usm.yueranfly.top

PHP:  public static function f() {}
来源：http://sjb.tian-w.cn

JS:   static f() {}
来源：http://wkr.chenlongwang.top

TS:   static f(): void {}
来源：http://oly.zhiwuduotai.top

Java: static void f() {}
来源：http://bzc.jlsjyb.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mqz.9152youxi.cn

Ruby: def self.f; end
来源：http://irv.xinyue.icu

C#:   public static void F() {}
来源：http://rva.vehdjk.com

[G09] 接口 / 抽象类
来源：http://zor.havefunace.top

Py:   from abc import ABC, abstractmethod
来源：http://yji.tianlin.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://jta.pengpengdd.cyou

JS:   // 无接口：靠约定或 JSDoc
来源：http://uca.xinyue.icu

TS:   interface Shape { area(): number; }
来源：http://eof.hcnkem.com

Java: interface Shape { double area(); }
来源：http://ueh.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://vsb.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://idh.redwolf501.top

C#:   interface IShape { double Area(); }
来源：http://iht.cdnleiting.top

[G10] 访问控制
来源：http://qqe.chenjidiqi.icu

Py:   约定 _protected / __private（不强制）
来源：http://tvp.yj20258.top

PHP:  public / protected / private
来源：http://utx.zhongyouzk.top

JS:   #private 字段；其余公开
来源：http://flg.pycfn.com

TS:   public / protected / private
来源：http://cuu.xziqi.cn

Java: public / protected / private / 默认包级
来源：http://cpz.dianchejie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://iwd.zhoulong.xyz

Ruby: public / protected / private
来源：http://mls.hfpthk.cn

C#:   public / protected / private / internal
来源：http://qth.xinyue.icu

[G11] getter / setter
来源：http://kbk.shuidangran.top

Py:   @property 与 @x.setter
来源：http://nfs.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rrb.jinqigfzy.top

JS:   get name() { return this._name; }
来源：http://wgm.snrcjt.cn

TS:   get name(): string { return this._name; }
来源：http://xjh.gogol.net.cn

Java: public String getName() { return name; }
来源：http://mkb.xziqi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dxh.hnqzz.top

Ruby: attr_accessor :name
来源：http://tyx.nanxuanxn.top

C#:   public string Name { get; set; }
来源：http://tbc.zhaomingkeji.xyz

[G12] 对象转字符串
来源：http://wrj.yueranfly.top

Py:   def __str__(self): return self.name
来源：http://lsu.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://eqj.yfazqb.com

JS:   toString() { return this.name; }
来源：http://dzn.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://suu.jinghuilouyu.cn

Java: @Override public String toString() { return name; }
来源：http://nzg.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://gga.quarkkingdee.top

Ruby: def to_s; @name; end
来源：http://vmb.shangyingyoupin.top

C#:   public override string ToString() => Name;
来源：http://awp.cucudq.cn

[G13] 判断对象类型
来源：http://zgm.jlsjyb.cn

Py:   isinstance(u, User)
来源：http://suf.guannengcc.top

PHP:  $u instanceof User
来源：http://wqw.sweek.top

JS:   u instanceof User
来源：http://rry.xuetiantiany.cn

TS:   u instanceof User
来源：http://ygc.ppjwa.cn

Java: u instanceof User
来源：http://egr.ehwqpu.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://whe.wangshuangyany.cn

Ruby: u.is_a?(User)
来源：http://omb.hesvh.cn

C#:   u is User
来源：http://gze.zhijiandao.cn

[G14] 数据类 / record
来源：http://bko.zhijiandao.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qbi.birdmap.top

PHP:  // 用 readonly 属性模拟
来源：http://czo.jiagoushi.top

JS:   // 无内置：普通类或对象字面量
来源：http://fhq.xinyue.icu

TS:   type User = { name: string; age: number };
来源：http://edg.fehbvm.com

Java: record User(String name, int age) {}
来源：http://okx.jinghuilouyu.cn

Go:   type User struct { Name string; Age int }
来源：http://omr.hesvh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wol.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://jjm.ctjpmb.com

[G15] 枚举
来源：http://nek.xingfuxueyuan.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ymi.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://dzs.smart0.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://snw.yj202588.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ngn.ydzc1.top

Java: enum Color { RED, GREEN }
来源：http://bvo.0kj1m.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ffr.fengsongda.top

Ruby: Color = %i[red green].freeze
来源：http://woy.jinqigfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iqw.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://oaa.daria6918.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jqn.hnxiangtu.top

PHP:  get_object_vars($obj);
来源：http://rkg.ydzc1.top

JS:   Object.entries(obj)
来源：http://wid.chenlongwang.top

TS:   Object.entries(obj)
来源：http://zmg.shzxlz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uka.zycfv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ret.meibo888.top

Ruby: obj.instance_variables
来源：http://vst.yuanzhike.top

C#:   // 用反射或 System.Text.Json
来源：http://lem.yanxiufei.cn

================================================================================
来源：http://ecf.vehdjk.com

H. 异常与错误处理
来源：http://kyp.sufxvd.cn

================================================================================
来源：http://kuj.tian-w.cn

[H01] try / catch 基础
来源：http://rli.ywan-chungtsiang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bct.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rha.epnwcf.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fvo.epnwcf.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mqs.xuanzx.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mwe.zhixingplan.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jnv.jyoumei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dyj.jqgfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://imb.jinqigufen.top

[H02] finally / ensure 收尾
来源：http://wqr.hywenlv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lso.cucudq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rpi.yongpay.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gjy.0kj1m.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ayu.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://oki.smart0.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://aav.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fpf.hnxiangtu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dym.xziqi.cn

[H03] 主动抛出异常
来源：http://ndp.vqdsnc.cn

Py:   raise ValueError("错误信息")
来源：http://lft.yj202588.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vaq.ppjwa.cn

JS:   throw new Error("错误信息");
来源：http://uvl.shuidangran.top

TS:   throw new Error("错误信息");
来源：http://dwc.yj202588.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://oxx.hcnkem.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ffz.vqdsnc.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nym.shanyushiyangtech.top

C#:   throw new ArgumentException("错误信息");
来源：http://ets.chenjidiqi.icu

[H04] 自定义异常类型
来源：http://vsz.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://dzv.ydzc1.top

PHP:  class MyError extends RuntimeException {}
来源：http://ucd.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://cnp.daxiang520.top

TS:   class MyError extends Error {}
来源：http://hcq.smart0.xyz

Java: class MyException extends RuntimeException {}
来源：http://vga.birdmap.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ftf.tian-w.cn

Ruby: class MyError < StandardError; end
来源：http://hke.yanxiufei.cn

C#:   class MyException : Exception {}
来源：http://ljj.hnqzz.top

[H05] 捕获特定类型
来源：http://eyg.yonumen.top

Py:   except ValueError as e:
来源：http://uqx.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cqj.cashguo.top

JS:   if (e instanceof TypeError) {}
来源：http://shi.wangdashe.top

TS:   if (e instanceof TypeError) {}
来源：http://bvh.zycfv.cn

Java: catch (IOException | SQLException e) {}
来源：http://eag.snrcjt.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fiw.meibo888.top

Ruby: rescue ArgumentError => e
来源：http://gqj.jiagoushi.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ktg.dashuyun.cn

[H06] 可选值 / 空值安全访问
来源：http://nwy.fanxiaobao.xyz

Py:   value = d.get("k") or default
来源：http://jmn.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xyt.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://rlv.yonumen.top

TS:   obj?.a?.b;  d ?? default
来源：http://kzc.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://age.vehdjk.com

Go:   if v, ok := m["k"]; ok { }
来源：http://xgd.tianlin.xyz

Ruby: d&.dig(:a, :b)
来源：http://jng.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://gkc.hysaishi.cn

[H07] 断言
来源：http://gdj.zhiwuduotai.top

Py:   assert x > 0, "必须为正"
来源：http://tdx.jinqigfzy.top

PHP:  assert($x > 0);
来源：http://cpg.epnwcf.com

JS:   console.assert(x > 0);
来源：http://fhv.ybcxt.top

TS:   console.assert(x > 0);
来源：http://oxt.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://sdx.tarul.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://owp.jianghu66.top

Ruby: raise "必须为正" unless x > 0
来源：http://jsf.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://aen.zhiwuduotai.top

[H08] 获取错误信息与堆栈
来源：http://tqy.ivvv.top

Py:   str(e);  traceback.format_exc()
来源：http://ihs.birdmap.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wzb.316326.xyz

JS:   e.message;  e.stack
来源：http://pma.epnwcf.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://wyt.hcnkem.com

Java: e.getMessage();  e.printStackTrace()
来源：http://wus.cucudq.cn

Go:   err.Error()
来源：http://bqe.0kj1m.cn

Ruby: e.message;  e.backtrace
来源：http://npw.aibaodan.cn

C#:   e.Message;  e.StackTrace
来源：http://jle.mhx1999.top

[H09] 带错误码的异常
来源：http://uml.sjlbkw.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jrd.ydjk.org.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hfa.ywan-chungtsiang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ztm.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rvs.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sxq.fzhhl.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vtk.snrcjt.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yfo.0kj1m.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vgo.bbcook.cn

[H10] 资源自动释放
来源：http://kjv.mhx1999.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ism.zhengqikj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://imr.sweek.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qjo.shanyushiyangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tmk.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bbb.feifeiyinyue.top

Go:   defer f.Close()
来源：http://csu.hongshengwenyu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tkp.dianchejie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xwp.xylfe.cn

================================================================================
来源：http://gef.ybcxt.top

I. 正则表达式
来源：http://mnf.yj20258.top

================================================================================
来源：http://wyi.iojbl.cn

[I01] 判断是否匹配
来源：http://wst.shuidangran.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ovv.redwolf501.top

PHP:  preg_match('/\d+/', $s);
来源：http://gjc.gotoacloud.top

JS:   /\d+/.test(s)
来源：http://wxk.jinghuilouyu.cn

TS:   /\d+/.test(s)
来源：http://fgu.xuetiantiany.cn


<!-- 参考信息 -->