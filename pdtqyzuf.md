代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://txq.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cjm.ywan-chungtsiang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bhh.sweek.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aeg.yueranfly.top

[F05] 判断文件或目录是否存在
来源：http://iwg.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wdf.yj20258.top

PHP:  file_exists("a.txt");
来源：http://ovu.redwolf501.top

JS:   fs.existsSync("a.txt")
来源：http://tum.9152youxi.cn

TS:   fs.existsSync("a.txt")
来源：http://yko.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ict.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://enz.9152youxi.cn

Ruby: File.exist?("a.txt")
来源：http://cvg.fehbvm.com

C#:   File.Exists("a.txt")
来源：http://dbw.pengpengdd.cyou

[F06] 删除文件
来源：http://qeo.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://wmv.cucudq.cn

PHP:  unlink("a.txt");
来源：http://csd.sysykeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://ise.hammf.cn

TS:   fs.unlinkSync("a.txt")
来源：http://edf.svipenyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hvh.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://bfu.zycfv.cn

Ruby: File.delete("a.txt")
来源：http://dfg.dianchejie.cn

C#:   File.Delete("a.txt");
来源：http://glj.ywan-chungtsiang.top

[F07] 创建目录（含多级）
来源：http://tok.fanxiaobao.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lcx.wangshuangyany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jvi.aizwys.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fzy.jianghu66.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ros.fehbvm.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://roe.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tnp.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ikr.uphjek.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qvu.zdbjq.cn

[F08] 遍历目录
来源：http://cil.shangyingyoupin.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://auy.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yql.ydzc1.top

JS:   fs.readdirSync("dir")
来源：http://ecs.mhx1999.top

TS:   fs.readdirSync("dir")
来源：http://ywm.svipenyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://daa.yongpay.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wsk.ydzc1.top

Ruby: Dir.children("dir")
来源：http://lqt.zycfv.cn

C#:   Directory.GetFiles("dir")
来源：http://wyz.sufxvd.cn

[F09] 获取文件大小
来源：http://ygd.jqgufenzy.top

Py:   os.path.getsize("a.txt")
来源：http://stv.shangyingyoupin.top

PHP:  filesize("a.txt");
来源：http://cub.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://tlz.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://cjq.haohaochexian.top

Java: Files.size(Path.of("a.txt"))
来源：http://jzf.aibaodan.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wyr.shuidangran.top

Ruby: File.size("a.txt")
来源：http://iih.pycfn.com

C#:   new FileInfo("a.txt").Length
来源：http://aah.zhiwuduotai.top

[F10] 取文件扩展名 / 文件名
来源：http://urc.xuetiantiany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://usl.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ino.kuanghao11.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yaw.yongpay.top

TS:   path.extname("a.txt")
来源：http://pon.haohaochexian.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gea.ctjpmb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vcp.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yux.zhaomingkeji.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vwr.cashguo.top

[F11] 复制与移动文件
来源：http://diq.hesvh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uoi.sxryk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://esg.pengpengdd.cyou

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ipe.c1oappe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://udb.yj20258.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vbx.yj202588.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tsh.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hsz.zdbjq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gbt.hfpthk.cn

[F12] CSV 读写
来源：http://imd.nanxuanxn.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lxh.xuanzx.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lwq.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zvy.yongpay.top

TS:   // 同上
来源：http://for.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://crj.zhoulong.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jad.ydzc1.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lyt.feifeiyinyue.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jhj.nanxuanxn.top

================================================================================
来源：http://dij.nanxinkj.top

G. 面向对象
来源：http://gxr.pengpengdd.cyou

================================================================================
来源：http://sae.epnwcf.com

[G01] 定义类
来源：http://tdq.hongshengwenyu.top

Py:   class User: pass
来源：http://sde.sufxvd.cn

PHP:  class User {}
来源：http://ozo.gzhubu.top

JS:   class User {}
来源：http://skt.redwolf501.top

TS:   class User { name: string = ""; }
来源：http://bmv.jiagoushi.top

Java: class User {}
来源：http://uxx.daria6918.cn

Go:   type User struct { Name string }
来源：http://oid.epnwcf.com

Ruby: class User; end
来源：http://sos.hnxiangtu.top

C#:   class User {}
来源：http://lxv.fzhhl.top

[G02] 构造函数
来源：http://nnz.vehdjk.com

Py:   def __init__(self, name): self.name = name
来源：http://ksm.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://luk.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://arm.xuetiantiany.cn

TS:   constructor(public name: string) {}
来源：http://mhs.tarul.cn

Java: User(String name) { this.name = name; }
来源：http://tup.sysykeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jnm.fzhhl.top

Ruby: def initialize(name); @name = name; end
来源：http://apk.cqqwz.cn

C#:   public User(string name) { Name = name; }
来源：http://rsi.redwolf501.top

[G03] 实例属性
来源：http://kld.yanxiufei.cn

Py:   self.name = "x"
来源：http://kpj.chenjidiqi.icu

PHP:  public string $name = "x";
来源：http://mpd.meibo888.top

JS:   this.name = "x";
来源：http://fro.0kj1m.cn

TS:   name: string = "x";
来源：http://yev.dianchejie.cn

Java: private String name;
来源：http://ako.hysaishi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xio.cheryme.top

Ruby: @name = "x"
来源：http://xfa.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://juu.snrcjt.cn

[G04] 定义方法
来源：http://fbs.fehbvm.com

Py:   def greet(self): return self.name
来源：http://kum.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cdg.dashuyun.cn

JS:   greet() { return this.name; }
来源：http://bvx.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://hkr.dashuyun.cn

Java: String greet() { return name; }
来源：http://ewc.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dee.redwolf501.top

Ruby: def greet; @name; end
来源：http://zxy.fengsongda.top

C#:   public string Greet() => Name;
来源：http://lbv.zycfv.cn

[G05] 继承
来源：http://emn.haohaochexian.top

Py:   class Admin(User): pass
来源：http://bxy.dashuyun.cn

PHP:  class Admin extends User {}
来源：http://gop.xziqi.cn

JS:   class Admin extends User {}
来源：http://uhq.cqqwz.cn

TS:   class Admin extends User {}
来源：http://nmt.9152youxi.cn

Java: class Admin extends User {}
来源：http://dzt.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://frw.shuidangran.top

Ruby: class Admin < User; end
来源：http://pan.sysykeji.top

C#:   class Admin : User {}
来源：http://aol.aizwys.cn

[G06] 重写方法
来源：http://osw.tianlin.xyz

Py:   def greet(self): return "admin"
来源：http://tvb.fehbvm.com

PHP:  public function greet(): string { return "admin"; }
来源：http://ghi.shzxlz.cn

JS:   greet() { return "admin"; }
来源：http://wpt.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://lkf.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://yzh.0kj1m.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hvf.xuetiantiany.cn

Ruby: def greet; "admin"; end
来源：http://hrb.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://hro.cucudq.cn

[G07] 调用父类方法
来源：http://vyl.sufxvd.cn

Py:   super().greet()
来源：http://luv.nanxuanxn.top

PHP:  parent::greet();
来源：http://vro.bjfxy.top

JS:   super.greet();
来源：http://mzj.aizwys.cn

TS:   super.greet();
来源：http://xbq.hysaishi.cn

Java: super.greet();
来源：http://xal.shzxlz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://crl.tianlin.xyz

Ruby: super
来源：http://atx.aizwys.cn

C#:   base.Greet();
来源：http://wgs.cashguo.top

[G08] 静态方法与属性
来源：http://apf.nanxinkj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lds.yanxiufei.cn

PHP:  public static function f() {}
来源：http://xsm.jinghuilouyu.cn

JS:   static f() {}
来源：http://iis.yanxiufei.cn

TS:   static f(): void {}
来源：http://glc.zhoulong.xyz

Java: static void f() {}
来源：http://bkp.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dom.bbcook.cn

Ruby: def self.f; end
来源：http://tft.shzxlz.cn

C#:   public static void F() {}
来源：http://vdz.yangfankeji.com

[G09] 接口 / 抽象类
来源：http://nth.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://glw.hnqzz.top

PHP:  interface Shape { public function area(): float; }
来源：http://muw.jinghuilouyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fmh.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://gjs.pycfn.com

Java: interface Shape { double area(); }
来源：http://acz.mhx1999.top

Go:   type Shape interface { Area() float64 }
来源：http://tsw.uphjek.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mle.fengsongda.top

C#:   interface IShape { double Area(); }
来源：http://hzt.tanke756.top

[G10] 访问控制
来源：http://gja.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://gqv.ehwqpu.com

PHP:  public / protected / private
来源：http://tvs.hongshengwenyu.top

JS:   #private 字段；其余公开
来源：http://kxa.shuidangran.top

TS:   public / protected / private
来源：http://ttf.hnxiangtu.top

Java: public / protected / private / 默认包级
来源：http://vcd.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://spa.zhongyouzk.top

Ruby: public / protected / private
来源：http://jdo.svipenyu.cn

C#:   public / protected / private / internal
来源：http://kje.chenlongwang.top

[G11] getter / setter
来源：http://rfr.zhongyouzk.top

Py:   @property 与 @x.setter
来源：http://vyf.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ozg.jlsjyb.cn

JS:   get name() { return this._name; }
来源：http://hns.hnqzz.top

TS:   get name(): string { return this._name; }
来源：http://sar.havefunace.top

Java: public String getName() { return name; }
来源：http://alt.zhaomingkeji.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://rfl.yvedp.cn

Ruby: attr_accessor :name
来源：http://dzr.fzhhl.top

C#:   public string Name { get; set; }
来源：http://ggd.yj202588.top

[G12] 对象转字符串
来源：http://zws.zdbjq.cn

Py:   def __str__(self): return self.name
来源：http://tfa.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jsr.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://qtp.sufxvd.cn

TS:   toString(): string { return this.name; }
来源：http://rbt.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://kin.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://avf.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://dpw.tarul.cn

C#:   public override string ToString() => Name;
来源：http://mow.cdnleiting.top

[G13] 判断对象类型
来源：http://pou.shangyingyoupin.top

Py:   isinstance(u, User)
来源：http://zri.pycfn.com

PHP:  $u instanceof User
来源：http://mco.zdqjudy.top

JS:   u instanceof User
来源：http://wvs.cdnleiting.top

TS:   u instanceof User
来源：http://woe.pengpengdd.cyou

Java: u instanceof User
来源：http://wsv.shanyushiyangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zha.bbcook.cn

Ruby: u.is_a?(User)
来源：http://vud.jqgufenzy.top

C#:   u is User
来源：http://mml.mhx1999.top

[G14] 数据类 / record
来源：http://nun.jinghuilouyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://adl.fehbvm.com

PHP:  // 用 readonly 属性模拟
来源：http://vmo.redwolf501.top

JS:   // 无内置：普通类或对象字面量
来源：http://edl.yuxming.cn

TS:   type User = { name: string; age: number };
来源：http://btw.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://sfj.9152youxi.cn

Go:   type User struct { Name string; Age int }
来源：http://oyb.sysykeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wbt.yongpay.top

C#:   record User(string Name, int Age);
来源：http://nmo.kuanghao11.cn

[G15] 枚举
来源：http://kyz.shangyingyoupin.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lny.yongpay.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tzg.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uhx.zhaomingkeji.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iak.chenzaomai.com

Java: enum Color { RED, GREEN }
来源：http://tgx.wangshuangyany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aqv.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://xeg.tian-w.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kgq.sysykeji.top

[G16] 对象转数组 / 字典
来源：http://fqt.jqgufenzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://txn.zhiwuduotai.top

PHP:  get_object_vars($obj);
来源：http://ymi.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://nom.9152youxi.cn

TS:   Object.entries(obj)
来源：http://ygv.shanyushiyangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nfg.hcnkem.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://smt.9152youxi.cn

Ruby: obj.instance_variables
来源：http://ysg.yj20258888.top

C#:   // 用反射或 System.Text.Json
来源：http://qbx.meibo888.top

================================================================================
来源：http://elg.tian-w.cn

H. 异常与错误处理
来源：http://jhc.zhongyouzk.top

================================================================================
来源：http://itp.shuidangran.top

[H01] try / catch 基础
来源：http://pws.epnwcf.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nka.aibaodan.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ewz.jianghu66.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hpt.fzhhl.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cmj.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cgo.tanke756.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://osd.fktsv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rho.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xgn.xziqi.cn

[H02] finally / ensure 收尾
来源：http://kkh.xziqi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gwq.aibaodan.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ptt.smart0.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://wce.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nng.ehwqpu.com

Java: try { f(); } finally { cleanup(); }
来源：http://cjv.ydjk.org.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sym.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://drh.shanyushiyangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ooo.meibo888.top

[H03] 主动抛出异常
来源：http://bxb.wangshuangyany.cn

Py:   raise ValueError("错误信息")
来源：http://caj.zhixingplan.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rrw.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://frp.yonumen.top

TS:   throw new Error("错误信息");
来源：http://wmj.zhixingplan.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lqy.ehwqpu.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wzo.birdmap.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kbk.dianchejie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hml.cdnleiting.top

[H04] 自定义异常类型
来源：http://mpo.yj20258.top

Py:   class MyError(Exception): pass
来源：http://qvc.jqgufenzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://xqs.redwolf501.top

JS:   class MyError extends Error {}
来源：http://ejm.52xcode.cn

TS:   class MyError extends Error {}
来源：http://not.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://jne.jiagoushi.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dpg.shzxlz.cn

Ruby: class MyError < StandardError; end
来源：http://oqx.pycfn.com

C#:   class MyException : Exception {}
来源：http://vob.yj20258.top

[H05] 捕获特定类型
来源：http://uey.gzhubu.top

Py:   except ValueError as e:
来源：http://crj.hfpthk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cly.xylfe.cn

JS:   if (e instanceof TypeError) {}
来源：http://dce.aizwys.cn

TS:   if (e instanceof TypeError) {}
来源：http://uor.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://qod.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wac.jyoumei.cn

Ruby: rescue ArgumentError => e
来源：http://ewc.ivvv.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tor.gogol.net.cn

[H06] 可选值 / 空值安全访问
来源：http://taa.shuidangran.top

Py:   value = d.get("k") or default
来源：http://tct.yongpay.top

PHP:  $v = $d["k"] ?? null;
来源：http://tew.yvedp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mfb.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://aok.nanxuanxn.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ozz.jyoumei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eqx.fehbvm.com

Ruby: d&.dig(:a, :b)
来源：http://byp.hammf.cn

C#:   obj?.A?.B ?? default
来源：http://tga.sweek.top

[H07] 断言
来源：http://rap.yongpay.top

Py:   assert x > 0, "必须为正"
来源：http://puf.aibaodan.cn

PHP:  assert($x > 0);
来源：http://yrn.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://vpa.sxryk.cn

TS:   console.assert(x > 0);
来源：http://xri.hesvh.cn

Java: assert x > 0 : "必须为正";
来源：http://wkn.0kj1m.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qes.uphjek.com

Ruby: raise "必须为正" unless x > 0
来源：http://izg.sysykeji.top

C#:   Debug.Assert(x > 0);
来源：http://kqz.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://kfi.jinqigufen.top

Py:   str(e);  traceback.format_exc()
来源：http://psx.ybcxt.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xhj.zhongyouzk.top

JS:   e.message;  e.stack
来源：http://rfr.jinqigfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://shw.cucudq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oyh.wangdashe.top

Go:   err.Error()
来源：http://fgu.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://cwp.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://lgu.gaohongyu789.top

[H09] 带错误码的异常
来源：http://lsy.yuanzhike.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xfm.yanxiufei.cn


<!-- 参考信息 -->