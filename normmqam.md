代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://woo.cashguo.top

Java: Files.exists(Path.of("a.txt"))
来源：http://utp.wangdashe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cso.smart0.xyz

Ruby: File.exist?("a.txt")
来源：http://tpq.tianlin.xyz

C#:   File.Exists("a.txt")
来源：http://ejy.uphjek.com

[F06] 删除文件
来源：http://kwq.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://bek.jlsjyb.cn

PHP:  unlink("a.txt");
来源：http://wkp.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://oqw.guowangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://ktj.hammf.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gov.hnqzz.top

Go:   os.Remove("a.txt")
来源：http://hza.jinyuanbaomall.cn

Ruby: File.delete("a.txt")
来源：http://ukf.jiagoushi.top

C#:   File.Delete("a.txt");
来源：http://aot.jinqigfzy.top

[F07] 创建目录（含多级）
来源：http://atm.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tyx.jinghuilouyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dqb.redwolf501.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zia.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://utp.hcnkem.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://igp.zdbjq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wss.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lyt.yonumen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fub.jyoumei.cn

[F08] 遍历目录
来源：http://syt.havefunace.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://heb.vqdsnc.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kha.316326.xyz

JS:   fs.readdirSync("dir")
来源：http://mbv.xuetiantiany.cn

TS:   fs.readdirSync("dir")
来源：http://ftk.mhx1999.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ghb.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://tkx.daria6918.cn

Ruby: Dir.children("dir")
来源：http://cbj.aibaodan.cn

C#:   Directory.GetFiles("dir")
来源：http://dwa.ehwqpu.com

[F09] 获取文件大小
来源：http://ovk.daria6918.cn

Py:   os.path.getsize("a.txt")
来源：http://fhl.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://uvx.fktsv.cn

JS:   fs.statSync("a.txt").size
来源：http://jmg.xingfuxueyuan.xyz

TS:   fs.statSync("a.txt").size
来源：http://ewn.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cbg.dashuyun.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qge.nwbrower.top

Ruby: File.size("a.txt")
来源：http://wlp.guowangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://gsi.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://lqf.bjfxy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ixe.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qke.ydjk.org.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jzc.yanxiufei.cn

TS:   path.extname("a.txt")
来源：http://nzs.fengsongda.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ptq.nanxuanxn.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://igj.ydzc1.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://trx.dashuyun.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mcy.xinyue.icu

[F11] 复制与移动文件
来源：http://zli.c1oappe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cwi.xinyue.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ltm.sjlbkw.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jyv.yueranfly.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fgo.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://muk.andypj.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pyc.hfpthk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tng.yvedp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qph.uphjek.com

[F12] CSV 读写
来源：http://qfj.hnqzz.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dez.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wfj.yueranfly.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gzf.hongshengwenyu.top

TS:   // 同上
来源：http://gjq.vehdjk.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nmc.kuanghao11.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bhn.jqgufenzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oxt.zdbjq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dks.tianlin.xyz

================================================================================
来源：http://rqp.jyoumei.cn

G. 面向对象
来源：http://tgu.ctjpmb.com

================================================================================
来源：http://pjv.birdmap.top

[G01] 定义类
来源：http://xst.yangfankeji.com

Py:   class User: pass
来源：http://hlf.xziqi.cn

PHP:  class User {}
来源：http://vme.zdbjq.cn

JS:   class User {}
来源：http://ykp.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://kcq.yfazqb.com

Java: class User {}
来源：http://lry.guannengcc.top

Go:   type User struct { Name string }
来源：http://dru.gotoacloud.top

Ruby: class User; end
来源：http://fxn.ywan-chungtsiang.top

C#:   class User {}
来源：http://gvc.cheryme.top

[G02] 构造函数
来源：http://rbg.ywan-chungtsiang.top

Py:   def __init__(self, name): self.name = name
来源：http://qgs.chenzaomai.com

PHP:  public function __construct(public string $name) {}
来源：http://dzz.jinghuilouyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://emf.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://jsm.ydzc1.top

Java: User(String name) { this.name = name; }
来源：http://wnf.fktsv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lrf.yj202588.top

Ruby: def initialize(name); @name = name; end
来源：http://ocp.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://ywr.9152youxi.cn

[G03] 实例属性
来源：http://bof.aibaodan.cn

Py:   self.name = "x"
来源：http://dve.epnwcf.com

PHP:  public string $name = "x";
来源：http://xrr.jinqigfzy.top

JS:   this.name = "x";
来源：http://khe.yj20258888.top

TS:   name: string = "x";
来源：http://cmi.jiagoushi.top

Java: private String name;
来源：http://qjp.hywenlv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aps.xziqi.cn

Ruby: @name = "x"
来源：http://aay.ybcxt.top

C#:   public string Name { get; set; } = "x";
来源：http://llx.mhx1999.top

[G04] 定义方法
来源：http://gov.cucudq.cn

Py:   def greet(self): return self.name
来源：http://iav.sysykeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qcb.nwbrower.top

JS:   greet() { return this.name; }
来源：http://wpz.redwolf501.top

TS:   greet(): string { return this.name; }
来源：http://hru.jlsjyb.cn

Java: String greet() { return name; }
来源：http://apv.pycfn.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://uth.yvedp.cn

Ruby: def greet; @name; end
来源：http://euh.wangshuangyany.cn

C#:   public string Greet() => Name;
来源：http://rpg.shanyushiyangtech.top

[G05] 继承
来源：http://igi.quarkkingdee.top

Py:   class Admin(User): pass
来源：http://bfy.zhongyouzk.top

PHP:  class Admin extends User {}
来源：http://rbx.ppjwa.cn

JS:   class Admin extends User {}
来源：http://rom.jinghuilouyu.cn

TS:   class Admin extends User {}
来源：http://wtx.bbcook.cn

Java: class Admin extends User {}
来源：http://qwe.yvedp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xvd.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://yxh.hysaishi.cn

C#:   class Admin : User {}
来源：http://apm.cqqwz.cn

[G06] 重写方法
来源：http://tdf.guowangkeji.top

Py:   def greet(self): return "admin"
来源：http://swg.dianchejie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qtt.smart0.xyz

JS:   greet() { return "admin"; }
来源：http://oya.0kj1m.cn

TS:   greet(): string { return "admin"; }
来源：http://qtr.smart0.xyz

Java: @Override String greet() { return "admin"; }
来源：http://oxc.zdbjq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vwb.haohaochexian.top

Ruby: def greet; "admin"; end
来源：http://mte.shanyushiyangkeji.top

C#:   public override string Greet() => "admin";
来源：http://agv.xziqi.cn

[G07] 调用父类方法
来源：http://fui.guannengcc.top

Py:   super().greet()
来源：http://tfm.ehwqpu.com

PHP:  parent::greet();
来源：http://nhh.aizwys.cn

JS:   super.greet();
来源：http://crg.aibaodan.cn

TS:   super.greet();
来源：http://pkl.gzhubu.top

Java: super.greet();
来源：http://whn.yj20258.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nld.aibaodan.cn

Ruby: super
来源：http://tyz.tarul.cn

C#:   base.Greet();
来源：http://ofm.yangfankeji.com

[G08] 静态方法与属性
来源：http://kww.cashguo.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qap.nanxuanxn.top

PHP:  public static function f() {}
来源：http://jrd.gzhubu.top

JS:   static f() {}
来源：http://fiu.hongshengwenyu.top

TS:   static f(): void {}
来源：http://hpt.chenlongwang.top

Java: static void f() {}
来源：http://kdm.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wjy.ctjpmb.com

Ruby: def self.f; end
来源：http://qug.jlsjyb.cn

C#:   public static void F() {}
来源：http://hdd.fanxiaobao.xyz

[G09] 接口 / 抽象类
来源：http://nel.zdqjudy.top

Py:   from abc import ABC, abstractmethod
来源：http://soe.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hel.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ale.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://jqj.haohaochexian.top

Java: interface Shape { double area(); }
来源：http://wcq.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://uyc.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fwz.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://wqx.nwbrower.top

[G10] 访问控制
来源：http://tss.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://egs.xylfe.cn

PHP:  public / protected / private
来源：http://lik.iojbl.cn

JS:   #private 字段；其余公开
来源：http://bpc.aizwys.cn

TS:   public / protected / private
来源：http://xrk.chenlongwang.top

Java: public / protected / private / 默认包级
来源：http://zrm.jqgufenzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jec.nwbrower.top

Ruby: public / protected / private
来源：http://hqf.ydzc1.top

C#:   public / protected / private / internal
来源：http://nxs.cdnleiting.top

[G11] getter / setter
来源：http://mga.sjlbkw.cn

Py:   @property 与 @x.setter
来源：http://hof.meibo888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lor.ywan-chungtsiang.top

JS:   get name() { return this._name; }
来源：http://wfw.daria6918.cn

TS:   get name(): string { return this._name; }
来源：http://dur.jinqigufen.top

Java: public String getName() { return name; }
来源：http://dqu.chenzaomai.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://fwu.yanxiufei.cn

Ruby: attr_accessor :name
来源：http://bmq.sjlbkw.cn

C#:   public string Name { get; set; }
来源：http://rvs.haohaochexian.top

[G12] 对象转字符串
来源：http://sdd.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://vwa.fanxiaobao.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://mrw.hfpthk.cn

JS:   toString() { return this.name; }
来源：http://ivr.bjfxy.top

TS:   toString(): string { return this.name; }
来源：http://rnl.feifeiyinyue.top

Java: @Override public String toString() { return name; }
来源：http://etf.jiagoushi.top

Go:   func (u User) String() string { return u.Name }
来源：http://bhc.vehdjk.com

Ruby: def to_s; @name; end
来源：http://ery.bbcook.cn

C#:   public override string ToString() => Name;
来源：http://ydv.ydzc1.top

[G13] 判断对象类型
来源：http://lco.fktsv.cn

Py:   isinstance(u, User)
来源：http://puf.9152youxi.cn

PHP:  $u instanceof User
来源：http://ita.chenlongwang.top

JS:   u instanceof User
来源：http://edx.smart0.xyz

TS:   u instanceof User
来源：http://hli.zhixingplan.top

Java: u instanceof User
来源：http://vbg.zhaomingkeji.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://vko.shzxlz.cn

Ruby: u.is_a?(User)
来源：http://tcw.haohaochexian.top

C#:   u is User
来源：http://oyj.fehbvm.com

[G14] 数据类 / record
来源：http://fat.ppjwa.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ykq.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://lib.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://sny.bjfxy.top

TS:   type User = { name: string; age: number };
来源：http://thb.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://iuq.zhijiandao.cn

Go:   type User struct { Name string; Age int }
来源：http://afr.0kj1m.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://quq.xziqi.cn

C#:   record User(string Name, int Age);
来源：http://qfw.chenjidiqi.icu

[G15] 枚举
来源：http://sxf.gogol.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ubp.0kj1m.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://com.yvedp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://drb.haohaochexian.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qxb.yangfankeji.com

Java: enum Color { RED, GREEN }
来源：http://qqq.hammf.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bcz.tanke756.top

Ruby: Color = %i[red green].freeze
来源：http://wdv.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iqz.yuxming.cn

[G16] 对象转数组 / 字典
来源：http://rei.dianchejie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ifn.sxryk.cn

PHP:  get_object_vars($obj);
来源：http://tic.tian-w.cn

JS:   Object.entries(obj)
来源：http://otz.9152youxi.cn

TS:   Object.entries(obj)
来源：http://qum.jianghu66.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bre.zdbjq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://huf.ybcxt.top

Ruby: obj.instance_variables
来源：http://gja.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://chf.uphjek.com

================================================================================
来源：http://lif.pengpengdd.cyou

H. 异常与错误处理
来源：http://qus.hcnkem.com

================================================================================
来源：http://eft.c1oappe.top

[H01] try / catch 基础
来源：http://aqt.zdbjq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tpi.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jgl.tian-w.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://den.shangyingyoupin.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://msi.sufxvd.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sfx.pycfn.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dep.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kii.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gap.fktsv.cn

[H02] finally / ensure 收尾
来源：http://bda.shanyushiyangtech.top

Py:   try: f()⏎finally: cleanup()
来源：http://wbb.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jjx.aizwys.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tla.jyoumei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://heg.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://kyb.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://myp.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tfy.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zbo.yj202588.top

[H03] 主动抛出异常
来源：http://zoa.sufxvd.cn

Py:   raise ValueError("错误信息")
来源：http://gxa.kuanghao11.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://buk.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://jkv.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://wof.gzhubu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://neg.cucudq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uca.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kog.zdbjq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tpn.andypj.xyz

[H04] 自定义异常类型
来源：http://rmr.hywenlv.cn

Py:   class MyError(Exception): pass
来源：http://nmh.jinqigfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://paz.daria6918.cn

JS:   class MyError extends Error {}
来源：http://her.shanyushiyangtech.top

TS:   class MyError extends Error {}
来源：http://zke.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://rmd.sweek.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://asg.yvedp.cn

Ruby: class MyError < StandardError; end
来源：http://zgv.jinqigufen.top

C#:   class MyException : Exception {}
来源：http://lug.sufxvd.cn

[H05] 捕获特定类型
来源：http://qxx.hcnkem.com

Py:   except ValueError as e:
来源：http://tid.yangfankeji.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lqm.cashguo.top

JS:   if (e instanceof TypeError) {}
来源：http://hia.yvedp.cn

TS:   if (e instanceof TypeError) {}
来源：http://vyn.hywenlv.cn

Java: catch (IOException | SQLException e) {}
来源：http://snl.ctjpmb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hps.vehdjk.com

Ruby: rescue ArgumentError => e
来源：http://rjf.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://csb.aibaodan.cn

[H06] 可选值 / 空值安全访问
来源：http://iie.wangshuangyany.cn

Py:   value = d.get("k") or default
来源：http://eof.wangdashe.top

PHP:  $v = $d["k"] ?? null;
来源：http://nas.smart0.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://nan.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fwd.zdbjq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://grv.pengpengdd.cyou

Go:   if v, ok := m["k"]; ok { }
来源：http://txm.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://ryl.jiagoushi.top

C#:   obj?.A?.B ?? default
来源：http://loe.chenjidiqi.icu

[H07] 断言
来源：http://gof.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://evt.yanxiufei.cn

PHP:  assert($x > 0);
来源：http://hsd.hcnkem.com

JS:   console.assert(x > 0);
来源：http://qgw.cucudq.cn

TS:   console.assert(x > 0);
来源：http://ezx.cheryme.top

Java: assert x > 0 : "必须为正";
来源：http://sbt.pengpengdd.cyou

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pmk.ybcxt.top

Ruby: raise "必须为正" unless x > 0
来源：http://wel.zhaomingkeji.xyz

C#:   Debug.Assert(x > 0);
来源：http://ckw.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://ehv.yj20258888.top

Py:   str(e);  traceback.format_exc()
来源：http://yaq.hammf.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zav.cashguo.top

JS:   e.message;  e.stack
来源：http://lhk.snrcjt.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://djd.yj202588.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jcv.hfpthk.cn

Go:   err.Error()
来源：http://oua.shuidangran.top

Ruby: e.message;  e.backtrace
来源：http://zyj.zdbjq.cn

C#:   e.Message;  e.StackTrace
来源：http://ljs.chenzaomai.com

[H09] 带错误码的异常
来源：http://jjb.gzhubu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zoc.bbcook.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://quw.ehwqpu.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jwz.cashguo.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lrq.hysaishi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qsk.shanyushiyangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rta.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://ini.daria6918.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ztk.zhaomingkeji.xyz

[H10] 资源自动释放
来源：http://jby.316326.xyz


<!-- 参考信息 -->