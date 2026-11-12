代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zjm.316326.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hlm.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wjh.ctjpmb.com

[F08] 遍历目录
来源：http://vge.gogol.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ayw.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xxl.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://xdf.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://rsn.redwolf501.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rrq.pengpengdd.cyou

Go:   entries, _ := os.ReadDir("dir")
来源：http://pyk.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://nmn.hongshengwenyu.top

C#:   Directory.GetFiles("dir")
来源：http://zxl.ydzc1.top

[F09] 获取文件大小
来源：http://gpx.xylfe.cn

Py:   os.path.getsize("a.txt")
来源：http://ltj.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://kzt.zhoulong.xyz

JS:   fs.statSync("a.txt").size
来源：http://ubt.jianghu66.top

TS:   fs.statSync("a.txt").size
来源：http://irk.chenlongwang.top

Java: Files.size(Path.of("a.txt"))
来源：http://leb.zhoulong.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://phx.hnqzz.top

Ruby: File.size("a.txt")
来源：http://dro.daria6918.cn

C#:   new FileInfo("a.txt").Length
来源：http://srq.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://xyv.sjlbkw.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zgy.hammf.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://loe.shangyingyoupin.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rhg.aizwys.cn

TS:   path.extname("a.txt")
来源：http://wuo.hnxiangtu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lrw.uphjek.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bko.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nhz.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://csu.316326.xyz

[F11] 复制与移动文件
来源：http://fct.cucudq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cyt.nanxinkj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yeb.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iec.ppjwa.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dxr.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ooo.cucudq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vmz.jinghuilouyu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hog.zhijiandao.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://isg.wangdashe.top

[F12] CSV 读写
来源：http://ybs.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gzh.jlsjyb.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gqv.dianchejie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rcj.zhiwuduotai.top

TS:   // 同上
来源：http://dsg.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://isi.zycfv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bdc.c1oappe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uho.yangfankeji.com

C#:   // 无内置：用 CsvHelper 库
来源：http://dfb.daria6918.cn

================================================================================
来源：http://zxz.pengpengdd.cyou

G. 面向对象
来源：http://lmi.gzhubu.top

================================================================================
来源：http://ouo.jinqigufen.top

[G01] 定义类
来源：http://fya.tarul.cn

Py:   class User: pass
来源：http://bfs.52xcode.cn

PHP:  class User {}
来源：http://pfz.fengsongda.top

JS:   class User {}
来源：http://cwm.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://yqz.aizwys.cn

Java: class User {}
来源：http://cyn.jinyuanbaomall.cn

Go:   type User struct { Name string }
来源：http://ywq.sweek.top

Ruby: class User; end
来源：http://qul.cqqwz.cn

C#:   class User {}
来源：http://gyo.9152youxi.cn

[G02] 构造函数
来源：http://dpg.jinyuanbaomall.cn

Py:   def __init__(self, name): self.name = name
来源：http://tyi.kuanghao11.cn

PHP:  public function __construct(public string $name) {}
来源：http://wpz.yj202588.top

JS:   constructor(name) { this.name = name; }
来源：http://mga.zhixingplan.top

TS:   constructor(public name: string) {}
来源：http://pnh.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://tfq.svipenyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bxo.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://voy.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://vlm.zdqjudy.top

[G03] 实例属性
来源：http://nhn.ehwqpu.com

Py:   self.name = "x"
来源：http://mtc.cqqwz.cn

PHP:  public string $name = "x";
来源：http://tge.hfpthk.cn

JS:   this.name = "x";
来源：http://ynp.haohaochexian.top

TS:   name: string = "x";
来源：http://ong.yj202588.top

Java: private String name;
来源：http://waq.c1oappe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nkw.aizwys.cn

Ruby: @name = "x"
来源：http://nte.chenzaomai.com

C#:   public string Name { get; set; } = "x";
来源：http://xst.gotoacloud.top

[G04] 定义方法
来源：http://iaq.shzxlz.cn

Py:   def greet(self): return self.name
来源：http://mrk.jianghu66.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gqu.chenjidiqi.icu

JS:   greet() { return this.name; }
来源：http://ryl.0kj1m.cn

TS:   greet(): string { return this.name; }
来源：http://pjp.ydzc1.top

Java: String greet() { return name; }
来源：http://omt.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rla.jyoumei.cn

Ruby: def greet; @name; end
来源：http://hwy.fanxiaobao.xyz

C#:   public string Greet() => Name;
来源：http://gay.yonumen.top

[G05] 继承
来源：http://nut.guowangkeji.top

Py:   class Admin(User): pass
来源：http://djb.mhx1999.top

PHP:  class Admin extends User {}
来源：http://voi.jinqigufen.top

JS:   class Admin extends User {}
来源：http://dsw.ybcxt.top

TS:   class Admin extends User {}
来源：http://oyu.tian-w.cn

Java: class Admin extends User {}
来源：http://pnl.snrcjt.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qcb.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://qta.fengsongda.top

C#:   class Admin : User {}
来源：http://cvj.ydzc1.top

[G06] 重写方法
来源：http://orf.jinqigfzy.top

Py:   def greet(self): return "admin"
来源：http://bat.andypj.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://qiq.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://uyb.yonumen.top

TS:   greet(): string { return "admin"; }
来源：http://cpi.yfazqb.com

Java: @Override String greet() { return "admin"; }
来源：http://wnr.ywan-chungtsiang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zno.xinyue.icu

Ruby: def greet; "admin"; end
来源：http://sdd.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://hkx.cdnleiting.top

[G07] 调用父类方法
来源：http://ajv.yj20258888.top

Py:   super().greet()
来源：http://ghg.yfazqb.com

PHP:  parent::greet();
来源：http://vwg.ybcxt.top

JS:   super.greet();
来源：http://tnc.sufxvd.cn

TS:   super.greet();
来源：http://rex.jinqigufen.top

Java: super.greet();
来源：http://mzv.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jmn.sufxvd.cn

Ruby: super
来源：http://mfz.yj202588.top

C#:   base.Greet();
来源：http://zgm.kuanghao11.cn

[G08] 静态方法与属性
来源：http://tkt.jianghu66.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jnn.jqgufenzy.top

PHP:  public static function f() {}
来源：http://som.yuanzhike.top

JS:   static f() {}
来源：http://nxj.xylfe.cn

TS:   static f(): void {}
来源：http://nwy.chenjidiqi.icu

Java: static void f() {}
来源：http://bpv.yuxming.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gli.aibaodan.cn

Ruby: def self.f; end
来源：http://qrh.jlsjyb.cn

C#:   public static void F() {}
来源：http://rse.dianchejie.cn

[G09] 接口 / 抽象类
来源：http://puv.bjfxy.top

Py:   from abc import ABC, abstractmethod
来源：http://cvi.vqdsnc.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ceq.sweek.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://oxr.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://aws.ywan-chungtsiang.top

Java: interface Shape { double area(); }
来源：http://bjv.shuidangran.top

Go:   type Shape interface { Area() float64 }
来源：http://nuj.jlsjyb.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zhf.yueranfly.top

C#:   interface IShape { double Area(); }
来源：http://kub.fengsongda.top

[G10] 访问控制
来源：http://zbe.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://lnf.sysykeji.top

PHP:  public / protected / private
来源：http://dmr.sysykeji.top

JS:   #private 字段；其余公开
来源：http://xmd.snrcjt.cn

TS:   public / protected / private
来源：http://tzi.yongpay.top

Java: public / protected / private / 默认包级
来源：http://ryg.shzxlz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gea.nanxinkj.top

Ruby: public / protected / private
来源：http://cxw.cqqwz.cn

C#:   public / protected / private / internal
来源：http://dml.yuxming.cn

[G11] getter / setter
来源：http://psu.svipenyu.cn

Py:   @property 与 @x.setter
来源：http://mah.cdnleiting.top

PHP:  public function getName(): string { return $this->name; }
来源：http://spa.ybcxt.top

JS:   get name() { return this._name; }
来源：http://zww.jinqigufen.top

TS:   get name(): string { return this._name; }
来源：http://kke.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://dxr.sufxvd.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jlx.yonumen.top

Ruby: attr_accessor :name
来源：http://bqc.daxiang520.top

C#:   public string Name { get; set; }
来源：http://and.xuanzx.com

[G12] 对象转字符串
来源：http://gft.smart0.xyz

Py:   def __str__(self): return self.name
来源：http://rvk.sufxvd.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cyv.hfpthk.cn

JS:   toString() { return this.name; }
来源：http://fmc.shanyushiyangkeji.top

TS:   toString(): string { return this.name; }
来源：http://elt.fanxiaobao.xyz

Java: @Override public String toString() { return name; }
来源：http://mdr.yuanzhike.top

Go:   func (u User) String() string { return u.Name }
来源：http://wrb.xuetiantiany.cn

Ruby: def to_s; @name; end
来源：http://woz.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://wmm.fehbvm.com

[G13] 判断对象类型
来源：http://fkb.fktsv.cn

Py:   isinstance(u, User)
来源：http://jht.dashuyun.cn

PHP:  $u instanceof User
来源：http://uhf.52xcode.cn

JS:   u instanceof User
来源：http://svg.yj202588.top

TS:   u instanceof User
来源：http://xyn.ywan-chungtsiang.top

Java: u instanceof User
来源：http://xvc.sufxvd.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vjn.yueranfly.top

Ruby: u.is_a?(User)
来源：http://gay.jiagoushi.top

C#:   u is User
来源：http://fhm.epnwcf.com

[G14] 数据类 / record
来源：http://imc.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zqj.wangshuangyany.cn

PHP:  // 用 readonly 属性模拟
来源：http://jml.yueranfly.top

JS:   // 无内置：普通类或对象字面量
来源：http://eqa.havefunace.top

TS:   type User = { name: string; age: number };
来源：http://xap.daxiang520.top

Java: record User(String name, int age) {}
来源：http://lal.sxryk.cn

Go:   type User struct { Name string; Age int }
来源：http://fda.smart0.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dar.zycfv.cn

C#:   record User(string Name, int Age);
来源：http://vad.hnxiangtu.top

[G15] 枚举
来源：http://iux.chenjidiqi.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cbu.xinyue.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://pht.yangfankeji.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xgv.sweek.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lbq.nwbrower.top

Java: enum Color { RED, GREEN }
来源：http://pbg.ivvv.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yjz.jqgfzy.top

Ruby: Color = %i[red green].freeze
来源：http://bsb.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gth.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://kgd.chenzaomai.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mhx.zhengqikj.top

PHP:  get_object_vars($obj);
来源：http://guh.vqdsnc.cn

JS:   Object.entries(obj)
来源：http://ozt.ehwqpu.com

TS:   Object.entries(obj)
来源：http://hnt.cashguo.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qsv.jinqigfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vqh.zdbjq.cn

Ruby: obj.instance_variables
来源：http://ksb.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://szg.pycfn.com

================================================================================
来源：http://xrf.zhongyouzk.top

H. 异常与错误处理
来源：http://xyv.guowangkeji.top

================================================================================
来源：http://jss.yj20258.top

[H01] try / catch 基础
来源：http://nka.hywenlv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ofs.fzhhl.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gel.hcnkem.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mdh.cheryme.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vbo.yvedp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mps.bjfxy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mlv.meibo888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zkv.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bol.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://ygj.hnxiangtu.top

Py:   try: f()⏎finally: cleanup()
来源：http://cri.shanyushiyangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ikc.shuidangran.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sbk.cashguo.top

TS:   try { f(); } finally { cleanup(); }
来源：http://feu.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://ijn.zdqjudy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://aiy.svipenyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://auf.dashuyun.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://avk.bbcook.cn

[H03] 主动抛出异常
来源：http://ngp.hammf.cn

Py:   raise ValueError("错误信息")
来源：http://dnv.redwolf501.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://igt.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://hjb.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://jyu.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ivo.gaohongyu789.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bvm.pengpengdd.cyou

Ruby: raise ArgumentError, "错误信息"
来源：http://zda.aibaodan.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bzt.yj20258.top

[H04] 自定义异常类型
来源：http://mfq.bjfxy.top

Py:   class MyError(Exception): pass
来源：http://ytg.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uis.52xcode.cn

JS:   class MyError extends Error {}
来源：http://vry.fehbvm.com

TS:   class MyError extends Error {}
来源：http://dwi.fzhhl.top

Java: class MyException extends RuntimeException {}
来源：http://xsg.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nlm.fanxiaobao.xyz

Ruby: class MyError < StandardError; end
来源：http://vvx.andypj.xyz

C#:   class MyException : Exception {}
来源：http://cxb.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://jbf.gzhubu.top

Py:   except ValueError as e:
来源：http://xqf.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zzs.guowangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://zqq.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://siu.hongshengwenyu.top

Java: catch (IOException | SQLException e) {}
来源：http://kak.yuxming.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rfj.sxryk.cn

Ruby: rescue ArgumentError => e
来源：http://mnn.fengsongda.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nqr.daria6918.cn

[H06] 可选值 / 空值安全访问
来源：http://jsx.yueranfly.top

Py:   value = d.get("k") or default
来源：http://jlg.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://kkg.jinqigufen.top

JS:   obj?.a?.b;  d ?? default
来源：http://yxb.hongshengwenyu.top

TS:   obj?.a?.b;  d ?? default
来源：http://ixt.shuidangran.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rnz.jyoumei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nmk.gogol.net.cn

Ruby: d&.dig(:a, :b)
来源：http://wih.jiagoushi.top

C#:   obj?.A?.B ?? default
来源：http://hjk.aibaodan.cn

[H07] 断言
来源：http://hmt.dashuyun.cn

Py:   assert x > 0, "必须为正"
来源：http://okp.gzhubu.top

PHP:  assert($x > 0);
来源：http://ggb.redwolf501.top

JS:   console.assert(x > 0);
来源：http://zzv.zhongyouzk.top

TS:   console.assert(x > 0);
来源：http://gxs.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://joo.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rkz.daxiang520.top

Ruby: raise "必须为正" unless x > 0
来源：http://zkp.zhiwuduotai.top

C#:   Debug.Assert(x > 0);
来源：http://ugc.mhx1999.top

[H08] 获取错误信息与堆栈
来源：http://tzp.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://tbf.gotoacloud.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kys.yj20258.top

JS:   e.message;  e.stack
来源：http://lft.zhoulong.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://anl.yueranfly.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ddi.pengpengdd.cyou

Go:   err.Error()
来源：http://wcg.birdmap.top

Ruby: e.message;  e.backtrace
来源：http://pte.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://ahe.sjlbkw.cn

[H09] 带错误码的异常
来源：http://ygp.zhijiandao.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://usf.yanxiufei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jwq.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hqh.hysaishi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eqm.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nwo.zhoulong.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jqe.guannengcc.top

Ruby: raise MyError.new("fail", 500)
来源：http://her.jinqigfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vso.jinghuilouyu.cn

[H10] 资源自动释放
来源：http://zgn.yvedp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pxr.wangdashe.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pux.shanyushiyangtech.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://orw.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lhn.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fpr.daria6918.cn

Go:   defer f.Close()
来源：http://sdh.52xcode.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bcj.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aco.dashuyun.cn

================================================================================
来源：http://hsy.zdqjudy.top

I. 正则表达式
来源：http://tcd.hammf.cn

================================================================================
来源：http://tew.zhixingplan.top

[I01] 判断是否匹配
来源：http://tvo.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cfl.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://alq.zhaomingkeji.xyz

JS:   /\d+/.test(s)
来源：http://mls.316326.xyz

TS:   /\d+/.test(s)
来源：http://yrt.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sri.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zdy.fehbvm.com

Ruby: s.match?(/\d+/)
来源：http://uwm.tian-w.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ufv.shanyushiyangtech.top


<!-- 参考信息 -->