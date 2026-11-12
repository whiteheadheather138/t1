代发 wailian999

C#:   File.Exists("a.txt")
来源：http://uoe.fanxiaobao.xyz

[F06] 删除文件
来源：http://msm.xinyue.icu

Py:   os.remove("a.txt")
来源：http://asg.cashguo.top

PHP:  unlink("a.txt");
来源：http://ndy.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://wvb.316326.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://nkg.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kas.hongshengwenyu.top

Go:   os.Remove("a.txt")
来源：http://pwh.chenjidiqi.icu

Ruby: File.delete("a.txt")
来源：http://spu.pengpengdd.cyou

C#:   File.Delete("a.txt");
来源：http://kfz.yj20258888.top

[F07] 创建目录（含多级）
来源：http://tqd.guowangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://auu.sweek.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ctd.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mgw.jiagoushi.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jem.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sbx.tarul.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xmi.jqgufenzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tsc.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lab.chenlongwang.top

[F08] 遍历目录
来源：http://bts.ydjk.org.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dqe.ctjpmb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qev.nwbrower.top

JS:   fs.readdirSync("dir")
来源：http://bii.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://tpb.yfazqb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dxe.c1oappe.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cam.cucudq.cn

Ruby: Dir.children("dir")
来源：http://ynn.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://dhp.cheryme.top

[F09] 获取文件大小
来源：http://hos.zhiwuduotai.top

Py:   os.path.getsize("a.txt")
来源：http://nih.tanke756.top

PHP:  filesize("a.txt");
来源：http://xhg.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://teo.jinqigufen.top

TS:   fs.statSync("a.txt").size
来源：http://dfd.c1oappe.top

Java: Files.size(Path.of("a.txt"))
来源：http://bto.9152youxi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zkv.cucudq.cn

Ruby: File.size("a.txt")
来源：http://dsm.andypj.xyz

C#:   new FileInfo("a.txt").Length
来源：http://tvk.hammf.cn

[F10] 取文件扩展名 / 文件名
来源：http://lpc.0kj1m.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zvi.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pbg.zdqjudy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nbp.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://fhu.zhixingplan.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zjs.svipenyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rxl.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://huf.quarkkingdee.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gpv.sxryk.cn

[F11] 复制与移动文件
来源：http://gty.yonumen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fek.yj20258.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rxc.zhaomingkeji.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://thy.hammf.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gqq.jqgufenzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ojx.epnwcf.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://riy.smart0.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wvv.52xcode.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gsz.feifeiyinyue.top

[F12] CSV 读写
来源：http://hek.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xpx.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://whl.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kgb.cucudq.cn

TS:   // 同上
来源：http://adi.vqdsnc.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lqh.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rrm.9152youxi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rtw.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://kas.hysaishi.cn

================================================================================
来源：http://tzu.kuanghao11.cn

G. 面向对象
来源：http://nhq.shangyingyoupin.top

================================================================================
来源：http://ofo.daria6918.cn

[G01] 定义类
来源：http://omo.jianghu66.top

Py:   class User: pass
来源：http://vgz.zdqjudy.top

PHP:  class User {}
来源：http://sjx.cqqwz.cn

JS:   class User {}
来源：http://lvd.iojbl.cn

TS:   class User { name: string = ""; }
来源：http://zbh.yongpay.top

Java: class User {}
来源：http://xlv.yongpay.top

Go:   type User struct { Name string }
来源：http://qgh.havefunace.top

Ruby: class User; end
来源：http://rqy.nwbrower.top

C#:   class User {}
来源：http://yqt.zycfv.cn

[G02] 构造函数
来源：http://bcq.smart0.xyz

Py:   def __init__(self, name): self.name = name
来源：http://aoi.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://jiz.jinqigufen.top

JS:   constructor(name) { this.name = name; }
来源：http://rvd.ywan-chungtsiang.top

TS:   constructor(public name: string) {}
来源：http://tdx.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://cic.zhongyouzk.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hhs.nanxinkj.top

Ruby: def initialize(name); @name = name; end
来源：http://dkr.zhengqikj.top

C#:   public User(string name) { Name = name; }
来源：http://jmp.gotoacloud.top

[G03] 实例属性
来源：http://sru.fanxiaobao.xyz

Py:   self.name = "x"
来源：http://lgb.yfazqb.com

PHP:  public string $name = "x";
来源：http://vgu.mhx1999.top

JS:   this.name = "x";
来源：http://mhk.dianchejie.cn

TS:   name: string = "x";
来源：http://qka.xinyue.icu

Java: private String name;
来源：http://soc.aizwys.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pzy.hcnkem.com

Ruby: @name = "x"
来源：http://ilu.yvedp.cn

C#:   public string Name { get; set; } = "x";
来源：http://sig.hongshengwenyu.top

[G04] 定义方法
来源：http://zap.fengsongda.top

Py:   def greet(self): return self.name
来源：http://mqu.fanxiaobao.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://lyn.meibo888.top

JS:   greet() { return this.name; }
来源：http://fvt.sufxvd.cn

TS:   greet(): string { return this.name; }
来源：http://jbk.hongshengwenyu.top

Java: String greet() { return name; }
来源：http://jbm.hysaishi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vjf.jinghuilouyu.cn

Ruby: def greet; @name; end
来源：http://eff.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://oux.birdmap.top

[G05] 继承
来源：http://sho.0kj1m.cn

Py:   class Admin(User): pass
来源：http://zrk.ydzc1.top

PHP:  class Admin extends User {}
来源：http://ckr.bjfxy.top

JS:   class Admin extends User {}
来源：http://wpk.ctjpmb.com

TS:   class Admin extends User {}
来源：http://dft.havefunace.top

Java: class Admin extends User {}
来源：http://unh.nanxinkj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fau.gotoacloud.top

Ruby: class Admin < User; end
来源：http://kpv.hesvh.cn

C#:   class Admin : User {}
来源：http://ytm.daria6918.cn

[G06] 重写方法
来源：http://kol.havefunace.top

Py:   def greet(self): return "admin"
来源：http://drk.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ouv.cheryme.top

JS:   greet() { return "admin"; }
来源：http://gwg.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://uzm.shanyushiyangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://vim.hesvh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://frf.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://bdp.yuanzhike.top

C#:   public override string Greet() => "admin";
来源：http://vzu.vehdjk.com

[G07] 调用父类方法
来源：http://qsj.vqdsnc.cn

Py:   super().greet()
来源：http://sxn.smart0.xyz

PHP:  parent::greet();
来源：http://shc.chenjidiqi.icu

JS:   super.greet();
来源：http://ooh.ppjwa.cn

TS:   super.greet();
来源：http://ccj.uphjek.com

Java: super.greet();
来源：http://owc.birdmap.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://psr.svipenyu.cn

Ruby: super
来源：http://eyh.vqdsnc.cn

C#:   base.Greet();
来源：http://mms.316326.xyz

[G08] 静态方法与属性
来源：http://bdk.hammf.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://thf.snrcjt.cn

PHP:  public static function f() {}
来源：http://dgc.0kj1m.cn

JS:   static f() {}
来源：http://ybo.tian-w.cn

TS:   static f(): void {}
来源：http://wmh.yonumen.top

Java: static void f() {}
来源：http://ujx.gzhubu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://erc.tianlin.xyz

Ruby: def self.f; end
来源：http://ejt.pycfn.com

C#:   public static void F() {}
来源：http://ldd.9152youxi.cn

[G09] 接口 / 抽象类
来源：http://zzq.gzhubu.top

Py:   from abc import ABC, abstractmethod
来源：http://kkc.ybcxt.top

PHP:  interface Shape { public function area(): float; }
来源：http://opc.jinqigufen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zio.hnqzz.top

TS:   interface Shape { area(): number; }
来源：http://nlq.zhiwuduotai.top

Java: interface Shape { double area(); }
来源：http://qag.ppjwa.cn

Go:   type Shape interface { Area() float64 }
来源：http://shc.fengsongda.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://crv.shzxlz.cn

C#:   interface IShape { double Area(); }
来源：http://ejj.hysaishi.cn

[G10] 访问控制
来源：http://cfx.mhx1999.top

Py:   约定 _protected / __private（不强制）
来源：http://jqs.yongpay.top

PHP:  public / protected / private
来源：http://xyp.ivvv.top

JS:   #private 字段；其余公开
来源：http://gje.jinyuanbaomall.cn

TS:   public / protected / private
来源：http://ofn.ehwqpu.com

Java: public / protected / private / 默认包级
来源：http://bde.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zsh.gaohongyu789.top

Ruby: public / protected / private
来源：http://myv.yj20258.top

C#:   public / protected / private / internal
来源：http://tyu.gogol.net.cn

[G11] getter / setter
来源：http://yoe.ctjpmb.com

Py:   @property 与 @x.setter
来源：http://sak.jlsjyb.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://asz.hywenlv.cn

JS:   get name() { return this._name; }
来源：http://soa.tanke756.top

TS:   get name(): string { return this._name; }
来源：http://dvo.sxryk.cn

Java: public String getName() { return name; }
来源：http://ahy.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://cju.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://exp.havefunace.top

C#:   public string Name { get; set; }
来源：http://xgb.gaohongyu789.top

[G12] 对象转字符串
来源：http://qcn.wangshuangyany.cn

Py:   def __str__(self): return self.name
来源：http://zfe.zycfv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ffu.fktsv.cn

JS:   toString() { return this.name; }
来源：http://jui.bbcook.cn

TS:   toString(): string { return this.name; }
来源：http://iwi.fktsv.cn

Java: @Override public String toString() { return name; }
来源：http://kyz.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://dkq.yuxming.cn

Ruby: def to_s; @name; end
来源：http://dnj.xinyue.icu

C#:   public override string ToString() => Name;
来源：http://cqp.quarkkingdee.top

[G13] 判断对象类型
来源：http://koe.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://ouv.fzhhl.top

PHP:  $u instanceof User
来源：http://jjy.yuxming.cn

JS:   u instanceof User
来源：http://rvs.fanxiaobao.xyz

TS:   u instanceof User
来源：http://fxo.xuetiantiany.cn

Java: u instanceof User
来源：http://ioo.cashguo.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qjb.jyoumei.cn

Ruby: u.is_a?(User)
来源：http://vfg.bbcook.cn

C#:   u is User
来源：http://sau.wangshuangyany.cn

[G14] 数据类 / record
来源：http://ksd.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wce.cqqwz.cn

PHP:  // 用 readonly 属性模拟
来源：http://fpe.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://qio.jinqigfzy.top

TS:   type User = { name: string; age: number };
来源：http://cgo.jyoumei.cn

Java: record User(String name, int age) {}
来源：http://mwn.daxiang520.top

Go:   type User struct { Name string; Age int }
来源：http://jxx.sxryk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tqk.sysykeji.top

C#:   record User(string Name, int Age);
来源：http://zjc.cashguo.top

[G15] 枚举
来源：http://cby.guannengcc.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dct.hammf.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hoe.yonumen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ygo.gzhubu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yyk.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://gpn.sjlbkw.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yfw.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://azc.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gaw.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://cvp.fktsv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nln.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://lup.cheryme.top

JS:   Object.entries(obj)
来源：http://qdw.zdqjudy.top

TS:   Object.entries(obj)
来源：http://sbe.ppjwa.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qnu.bjfxy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pgc.sweek.top

Ruby: obj.instance_variables
来源：http://poc.ehwqpu.com

C#:   // 用反射或 System.Text.Json
来源：http://fpx.zhoulong.xyz

================================================================================
来源：http://mtz.shanyushiyangkeji.top

H. 异常与错误处理
来源：http://bfk.yvedp.cn

================================================================================
来源：http://izq.jiagoushi.top

[H01] try / catch 基础
来源：http://csw.feifeiyinyue.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rzy.chenjidiqi.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zgv.fengsongda.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://djz.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gae.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sdi.fehbvm.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bxl.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pqg.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uqp.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://csp.nwbrower.top

Py:   try: f()⏎finally: cleanup()
来源：http://usk.zhoulong.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://dvb.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://eyy.bjfxy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://npv.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://piw.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nrc.yanxiufei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://guz.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jvw.ybcxt.top

[H03] 主动抛出异常
来源：http://mig.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://kpv.zhoulong.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://twh.andypj.xyz

JS:   throw new Error("错误信息");
来源：http://mri.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://rkm.nanxinkj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gmf.cashguo.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vsi.tian-w.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mzc.pycfn.com

C#:   throw new ArgumentException("错误信息");
来源：http://pyi.hongshengwenyu.top

[H04] 自定义异常类型
来源：http://qnt.epnwcf.com

Py:   class MyError(Exception): pass
来源：http://egu.vqdsnc.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rsu.ydzc1.top

JS:   class MyError extends Error {}
来源：http://shm.jiagoushi.top

TS:   class MyError extends Error {}
来源：http://wed.yuxming.cn

Java: class MyException extends RuntimeException {}
来源：http://obt.shanyushiyangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rxy.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://pim.jianghu66.top

C#:   class MyException : Exception {}
来源：http://ybm.sxryk.cn

[H05] 捕获特定类型
来源：http://qrn.jinghuilouyu.cn

Py:   except ValueError as e:
来源：http://tto.cashguo.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vmt.ehwqpu.com

JS:   if (e instanceof TypeError) {}
来源：http://whk.daxiang520.top

TS:   if (e instanceof TypeError) {}
来源：http://kya.fktsv.cn

Java: catch (IOException | SQLException e) {}
来源：http://utk.uphjek.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mwh.jinqigufen.top

Ruby: rescue ArgumentError => e
来源：http://rtv.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mqb.jianghu66.top

[H06] 可选值 / 空值安全访问
来源：http://pcv.jqgufenzy.top

Py:   value = d.get("k") or default
来源：http://umw.tianlin.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://ile.ppjwa.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bhp.zhaomingkeji.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://tvh.yvedp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://btd.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gqm.hesvh.cn

Ruby: d&.dig(:a, :b)
来源：http://qnf.cucudq.cn

C#:   obj?.A?.B ?? default
来源：http://pnl.ehwqpu.com

[H07] 断言
来源：http://lfy.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://nqu.hysaishi.cn

PHP:  assert($x > 0);
来源：http://rto.guowangkeji.top

JS:   console.assert(x > 0);
来源：http://llm.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://uju.ehwqpu.com

Java: assert x > 0 : "必须为正";
来源：http://dxv.aibaodan.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jaw.yvedp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rbl.hongshengwenyu.top

C#:   Debug.Assert(x > 0);
来源：http://qno.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://tmr.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://ajn.jlsjyb.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lgz.yuanzhike.top

JS:   e.message;  e.stack
来源：http://dul.hnqzz.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wbl.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ghq.iojbl.cn

Go:   err.Error()
来源：http://soi.snrcjt.cn

Ruby: e.message;  e.backtrace
来源：http://fiq.jinqigufen.top

C#:   e.Message;  e.StackTrace
来源：http://sxu.gzhubu.top

[H09] 带错误码的异常
来源：http://jpo.xziqi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dfb.hcnkem.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://rvs.xuanzx.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fzf.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jff.hesvh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://put.shangyingyoupin.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gkl.yuanzhike.top

Ruby: raise MyError.new("fail", 500)
来源：http://qoi.wangshuangyany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qxz.xziqi.cn

[H10] 资源自动释放
来源：http://nrw.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hen.hongshengwenyu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sec.hcnkem.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ciq.zhongyouzk.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lut.bjfxy.top


<!-- 参考信息 -->