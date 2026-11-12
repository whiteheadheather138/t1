代发 wailian999

Ruby: File.delete("a.txt")
来源：http://nzc.xziqi.cn

C#:   File.Delete("a.txt");
来源：http://abs.cucudq.cn

[F07] 创建目录（含多级）
来源：http://nie.jqgufenzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xfo.tianlin.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vcb.meibo888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kuq.daxiang520.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gav.hfpthk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qgz.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qcx.hesvh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dne.gotoacloud.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nwn.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://edd.aizwys.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://arn.daxiang520.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ynr.cdnleiting.top

JS:   fs.readdirSync("dir")
来源：http://rwn.c1oappe.top

TS:   fs.readdirSync("dir")
来源：http://nmx.hesvh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wqb.jinghuilouyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vnd.smart0.xyz

Ruby: Dir.children("dir")
来源：http://mue.fzhhl.top

C#:   Directory.GetFiles("dir")
来源：http://huc.xuetiantiany.cn

[F09] 获取文件大小
来源：http://iyr.jinghuilouyu.cn

Py:   os.path.getsize("a.txt")
来源：http://opv.ivvv.top

PHP:  filesize("a.txt");
来源：http://yob.pengpengdd.cyou

JS:   fs.statSync("a.txt").size
来源：http://qcw.fanxiaobao.xyz

TS:   fs.statSync("a.txt").size
来源：http://uqw.yonumen.top

Java: Files.size(Path.of("a.txt"))
来源：http://xjy.hammf.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dyn.redwolf501.top

Ruby: File.size("a.txt")
来源：http://dlk.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://ckl.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://omj.birdmap.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wcl.yuxming.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qrf.cqqwz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://itz.sjlbkw.cn

TS:   path.extname("a.txt")
来源：http://rkb.bjfxy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ugg.nwbrower.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://scb.havefunace.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qlx.daxiang520.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bkj.sysykeji.top

[F11] 复制与移动文件
来源：http://qpb.feifeiyinyue.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tkv.svipenyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ofc.ywan-chungtsiang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xvf.iojbl.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://snh.zhixingplan.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xyx.meibo888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tsc.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zoh.xziqi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wed.hesvh.cn

[F12] CSV 读写
来源：http://xim.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vkl.yanxiufei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sig.jinyuanbaomall.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://opy.zdqjudy.top

TS:   // 同上
来源：http://hnq.vehdjk.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qos.cheryme.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yic.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://phi.cheryme.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kxb.chenzaomai.com

================================================================================
来源：http://kio.jinghuilouyu.cn

G. 面向对象
来源：http://ton.yj20258.top

================================================================================
来源：http://lft.jyoumei.cn

[G01] 定义类
来源：http://ily.bjfxy.top

Py:   class User: pass
来源：http://tpa.gogol.net.cn

PHP:  class User {}
来源：http://xgs.yongpay.top

JS:   class User {}
来源：http://pwk.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://okv.sufxvd.cn

Java: class User {}
来源：http://pce.zycfv.cn

Go:   type User struct { Name string }
来源：http://aff.wangshuangyany.cn

Ruby: class User; end
来源：http://cpk.hnxiangtu.top

C#:   class User {}
来源：http://fjp.xylfe.cn

[G02] 构造函数
来源：http://duw.c1oappe.top

Py:   def __init__(self, name): self.name = name
来源：http://kdy.hongshengwenyu.top

PHP:  public function __construct(public string $name) {}
来源：http://xhz.cheryme.top

JS:   constructor(name) { this.name = name; }
来源：http://ylz.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://isu.xuetiantiany.cn

Java: User(String name) { this.name = name; }
来源：http://tvt.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pvy.cqqwz.cn

Ruby: def initialize(name); @name = name; end
来源：http://lif.wangshuangyany.cn

C#:   public User(string name) { Name = name; }
来源：http://atp.meibo888.top

[G03] 实例属性
来源：http://quj.gotoacloud.top

Py:   self.name = "x"
来源：http://ckv.hongshengwenyu.top

PHP:  public string $name = "x";
来源：http://inn.yanxiufei.cn

JS:   this.name = "x";
来源：http://qgi.snrcjt.cn

TS:   name: string = "x";
来源：http://ckq.jinghuilouyu.cn

Java: private String name;
来源：http://jbl.ybcxt.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qyb.zhaomingkeji.xyz

Ruby: @name = "x"
来源：http://pvn.ydjk.org.cn

C#:   public string Name { get; set; } = "x";
来源：http://dvn.iojbl.cn

[G04] 定义方法
来源：http://lok.xuanzx.com

Py:   def greet(self): return self.name
来源：http://xtj.chenzaomai.com

PHP:  public function greet(): string { return $this->name; }
来源：http://his.tanke756.top

JS:   greet() { return this.name; }
来源：http://idv.daria6918.cn

TS:   greet(): string { return this.name; }
来源：http://rpc.9152youxi.cn

Java: String greet() { return name; }
来源：http://xzj.yueranfly.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://iwt.shuidangran.top

Ruby: def greet; @name; end
来源：http://mtn.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://fmx.hnxiangtu.top

[G05] 继承
来源：http://dma.uphjek.com

Py:   class Admin(User): pass
来源：http://ajj.gaohongyu789.top

PHP:  class Admin extends User {}
来源：http://hhg.xuanzx.com

JS:   class Admin extends User {}
来源：http://loz.yueranfly.top

TS:   class Admin extends User {}
来源：http://vsz.52xcode.cn

Java: class Admin extends User {}
来源：http://zyy.0kj1m.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vgk.sufxvd.cn

Ruby: class Admin < User; end
来源：http://kwu.guowangkeji.top

C#:   class Admin : User {}
来源：http://aju.fehbvm.com

[G06] 重写方法
来源：http://nkn.fengsongda.top

Py:   def greet(self): return "admin"
来源：http://zeo.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bpq.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://rzm.jqgufenzy.top

TS:   greet(): string { return "admin"; }
来源：http://wpj.shanyushiyangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://mux.bbcook.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xmu.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://joh.jyoumei.cn

C#:   public override string Greet() => "admin";
来源：http://dfu.cashguo.top

[G07] 调用父类方法
来源：http://tyq.hysaishi.cn

Py:   super().greet()
来源：http://rpm.pycfn.com

PHP:  parent::greet();
来源：http://lzk.zhoulong.xyz

JS:   super.greet();
来源：http://gqk.jiagoushi.top

TS:   super.greet();
来源：http://sbr.shuidangran.top

Java: super.greet();
来源：http://zut.fanxiaobao.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bwm.jianghu66.top

Ruby: super
来源：http://lwq.xinyue.icu

C#:   base.Greet();
来源：http://ebs.zhengqikj.top

[G08] 静态方法与属性
来源：http://amq.ydjk.org.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yev.bjfxy.top

PHP:  public static function f() {}
来源：http://esp.cashguo.top

JS:   static f() {}
来源：http://rsw.sysykeji.top

TS:   static f(): void {}
来源：http://jua.tian-w.cn

Java: static void f() {}
来源：http://srp.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://msg.jqgfzy.top

Ruby: def self.f; end
来源：http://osy.wangshuangyany.cn

C#:   public static void F() {}
来源：http://duz.kuanghao11.cn

[G09] 接口 / 抽象类
来源：http://xeq.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://vaa.gogol.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jdq.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fbp.fanxiaobao.xyz

TS:   interface Shape { area(): number; }
来源：http://frr.tanke756.top

Java: interface Shape { double area(); }
来源：http://yzg.aibaodan.cn

Go:   type Shape interface { Area() float64 }
来源：http://tnp.shanyushiyangtech.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://umd.hnqzz.top

C#:   interface IShape { double Area(); }
来源：http://his.yuanzhike.top

[G10] 访问控制
来源：http://jsj.tarul.cn

Py:   约定 _protected / __private（不强制）
来源：http://mvr.guowangkeji.top

PHP:  public / protected / private
来源：http://mnf.hywenlv.cn

JS:   #private 字段；其余公开
来源：http://bpd.sxryk.cn

TS:   public / protected / private
来源：http://ejv.daxiang520.top

Java: public / protected / private / 默认包级
来源：http://vqy.yonumen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yjj.9152youxi.cn

Ruby: public / protected / private
来源：http://zev.andypj.xyz

C#:   public / protected / private / internal
来源：http://kon.nanxuanxn.top

[G11] getter / setter
来源：http://vnf.cashguo.top

Py:   @property 与 @x.setter
来源：http://wpa.xingfuxueyuan.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://pnz.quarkkingdee.top

JS:   get name() { return this._name; }
来源：http://afy.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://kzb.yanxiufei.cn

Java: public String getName() { return name; }
来源：http://fjz.fehbvm.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://qak.yj20258.top

Ruby: attr_accessor :name
来源：http://khl.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://yob.sjlbkw.cn

[G12] 对象转字符串
来源：http://imb.andypj.xyz

Py:   def __str__(self): return self.name
来源：http://skr.ppjwa.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://siu.jlsjyb.cn

JS:   toString() { return this.name; }
来源：http://ton.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://rje.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://ljj.zdqjudy.top

Go:   func (u User) String() string { return u.Name }
来源：http://xgu.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://ged.hongshengwenyu.top

C#:   public override string ToString() => Name;
来源：http://ozv.gogol.net.cn

[G13] 判断对象类型
来源：http://hal.guannengcc.top

Py:   isinstance(u, User)
来源：http://hbp.shuidangran.top

PHP:  $u instanceof User
来源：http://zyq.iojbl.cn

JS:   u instanceof User
来源：http://gue.vqdsnc.cn

TS:   u instanceof User
来源：http://mef.ehwqpu.com

Java: u instanceof User
来源：http://edw.shangyingyoupin.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://prr.haohaochexian.top

Ruby: u.is_a?(User)
来源：http://laj.snrcjt.cn

C#:   u is User
来源：http://gzl.xuetiantiany.cn

[G14] 数据类 / record
来源：http://slt.yuxming.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jpg.shanyushiyangtech.top

PHP:  // 用 readonly 属性模拟
来源：http://gqc.yvedp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://usr.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://ehr.pycfn.com

Java: record User(String name, int age) {}
来源：http://wvj.xingfuxueyuan.xyz

Go:   type User struct { Name string; Age int }
来源：http://kfx.hammf.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ynl.tanke756.top

C#:   record User(string Name, int Age);
来源：http://yif.epnwcf.com

[G15] 枚举
来源：http://nkf.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mxu.yueranfly.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xdb.c1oappe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fmg.9152youxi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pym.pengpengdd.cyou

Java: enum Color { RED, GREEN }
来源：http://hsq.zdbjq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aio.ydzc1.top

Ruby: Color = %i[red green].freeze
来源：http://gzf.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rkm.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://bbr.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kqc.tanke756.top

PHP:  get_object_vars($obj);
来源：http://iat.jianghu66.top

JS:   Object.entries(obj)
来源：http://atw.fzhhl.top

TS:   Object.entries(obj)
来源：http://xyp.0kj1m.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rbw.wangdashe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tjd.zycfv.cn

Ruby: obj.instance_variables
来源：http://ion.shuidangran.top

C#:   // 用反射或 System.Text.Json
来源：http://qzd.ybcxt.top

================================================================================
来源：http://gol.hcnkem.com

H. 异常与错误处理
来源：http://ljk.redwolf501.top

================================================================================
来源：http://she.haohaochexian.top

[H01] try / catch 基础
来源：http://mem.c1oappe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mkr.tianlin.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://poz.0kj1m.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ltk.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://grm.chenjidiqi.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pav.zhaomingkeji.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://srx.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ohz.fktsv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eiu.sxryk.cn

[H02] finally / ensure 收尾
来源：http://bkz.zhaomingkeji.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://gpa.ywan-chungtsiang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vsd.guannengcc.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pcj.jyoumei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gip.ywan-chungtsiang.top

Java: try { f(); } finally { cleanup(); }
来源：http://dfe.fehbvm.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://gba.iojbl.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://txe.c1oappe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://aum.vehdjk.com

[H03] 主动抛出异常
来源：http://dec.0kj1m.cn

Py:   raise ValueError("错误信息")
来源：http://qji.cashguo.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pgx.zhijiandao.cn

JS:   throw new Error("错误信息");
来源：http://cbz.dianchejie.cn

TS:   throw new Error("错误信息");
来源：http://czd.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zxa.havefunace.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pda.yueranfly.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xdq.nanxinkj.top

C#:   throw new ArgumentException("错误信息");
来源：http://avh.sufxvd.cn

[H04] 自定义异常类型
来源：http://uqd.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://cut.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://qlt.ydzc1.top

JS:   class MyError extends Error {}
来源：http://vsk.bjfxy.top

TS:   class MyError extends Error {}
来源：http://are.chenlongwang.top

Java: class MyException extends RuntimeException {}
来源：http://dkp.snrcjt.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bli.kuanghao11.cn

Ruby: class MyError < StandardError; end
来源：http://pul.zhijiandao.cn

C#:   class MyException : Exception {}
来源：http://ukb.jinqigufen.top

[H05] 捕获特定类型
来源：http://uim.wangshuangyany.cn

Py:   except ValueError as e:
来源：http://qyq.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qze.hywenlv.cn

JS:   if (e instanceof TypeError) {}
来源：http://ure.jinghuilouyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://kfq.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://whg.ppjwa.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xdj.tarul.cn

Ruby: rescue ArgumentError => e
来源：http://vtn.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tra.svipenyu.cn

[H06] 可选值 / 空值安全访问
来源：http://ect.xziqi.cn

Py:   value = d.get("k") or default
来源：http://nep.zycfv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vbf.zhongyouzk.top

JS:   obj?.a?.b;  d ?? default
来源：http://mpx.fktsv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zzi.cucudq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mly.guowangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://onh.gaohongyu789.top

Ruby: d&.dig(:a, :b)
来源：http://yvc.nanxuanxn.top

C#:   obj?.A?.B ?? default
来源：http://rrp.cucudq.cn

[H07] 断言
来源：http://enb.jinqigfzy.top

Py:   assert x > 0, "必须为正"
来源：http://ctu.yuxming.cn

PHP:  assert($x > 0);
来源：http://kdo.hesvh.cn

JS:   console.assert(x > 0);
来源：http://tbx.hysaishi.cn

TS:   console.assert(x > 0);
来源：http://vry.kuanghao11.cn

Java: assert x > 0 : "必须为正";
来源：http://ppa.vqdsnc.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qmg.jyoumei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zhi.hcnkem.com

C#:   Debug.Assert(x > 0);
来源：http://czs.epnwcf.com

[H08] 获取错误信息与堆栈
来源：http://ymp.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://fen.yueranfly.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eqg.xylfe.cn

JS:   e.message;  e.stack
来源：http://nvv.gzhubu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rap.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tml.chenzaomai.com

Go:   err.Error()
来源：http://pql.chenjidiqi.icu

Ruby: e.message;  e.backtrace
来源：http://ojh.aizwys.cn

C#:   e.Message;  e.StackTrace
来源：http://zfw.yj202588.top

[H09] 带错误码的异常
来源：http://xlo.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://flj.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dcp.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jgi.guowangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://twx.pycfn.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uir.daria6918.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xlw.pycfn.com

Ruby: raise MyError.new("fail", 500)
来源：http://lqa.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yti.yj202588.top

[H10] 资源自动释放
来源：http://aky.316326.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://aym.jqgufenzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qua.tian-w.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vpf.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bwz.yuxming.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rwg.dashuyun.cn

Go:   defer f.Close()
来源：http://psp.meibo888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yai.dianchejie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gbn.bjfxy.top

================================================================================
来源：http://lar.guannengcc.top

I. 正则表达式
来源：http://qev.ydjk.org.cn

================================================================================
来源：http://qcq.zdbjq.cn

[I01] 判断是否匹配
来源：http://hfy.xuetiantiany.cn


<!-- 参考信息 -->