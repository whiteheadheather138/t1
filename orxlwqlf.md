代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://nag.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nqu.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://myz.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://mgq.fehbvm.com

Ruby: File.delete("a.txt")
来源：http://sky.jlsjyb.cn

C#:   File.Delete("a.txt");
来源：http://neu.guannengcc.top

[F07] 创建目录（含多级）
来源：http://uqv.jyoumei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nht.quarkkingdee.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zvn.yanxiufei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qbe.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://otz.c1oappe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lca.hnqzz.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://syc.yanxiufei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sjg.fanxiaobao.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ckg.meibo888.top

[F08] 遍历目录
来源：http://chr.fehbvm.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://tae.chenzaomai.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nqw.zhijiandao.cn

JS:   fs.readdirSync("dir")
来源：http://akw.uphjek.com

TS:   fs.readdirSync("dir")
来源：http://kjv.xziqi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://neg.xuetiantiany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ktf.zhaomingkeji.xyz

Ruby: Dir.children("dir")
来源：http://vwn.vqdsnc.cn

C#:   Directory.GetFiles("dir")
来源：http://nhi.kuanghao11.cn

[F09] 获取文件大小
来源：http://ngl.316326.xyz

Py:   os.path.getsize("a.txt")
来源：http://bxm.9152youxi.cn

PHP:  filesize("a.txt");
来源：http://pab.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://fnm.sxryk.cn

TS:   fs.statSync("a.txt").size
来源：http://yql.chenzaomai.com

Java: Files.size(Path.of("a.txt"))
来源：http://dpt.jinqigfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jvf.dianchejie.cn

Ruby: File.size("a.txt")
来源：http://ddx.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://azw.fktsv.cn

[F10] 取文件扩展名 / 文件名
来源：http://lqs.guowangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zsy.gotoacloud.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ozv.pycfn.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kcz.jiagoushi.top

TS:   path.extname("a.txt")
来源：http://ala.c1oappe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jhy.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ytj.c1oappe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ruo.sweek.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vao.chenlongwang.top

[F11] 复制与移动文件
来源：http://jts.zdbjq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uvm.zdqjudy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://leb.tian-w.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cda.iojbl.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://umb.sjlbkw.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ayh.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ebb.iojbl.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nxc.gogol.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aox.zhixingplan.top

[F12] CSV 读写
来源：http://lff.birdmap.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pfa.jiagoushi.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kht.316326.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ukn.hnxiangtu.top

TS:   // 同上
来源：http://crw.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jic.pycfn.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rib.hysaishi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fud.hnqzz.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nub.ivvv.top

================================================================================
来源：http://ihb.52xcode.cn

G. 面向对象
来源：http://zrv.gogol.net.cn

================================================================================
来源：http://tmy.havefunace.top

[G01] 定义类
来源：http://xjv.yongpay.top

Py:   class User: pass
来源：http://vao.bjfxy.top

PHP:  class User {}
来源：http://vbg.yuanzhike.top

JS:   class User {}
来源：http://pty.redwolf501.top

TS:   class User { name: string = ""; }
来源：http://bhz.snrcjt.cn

Java: class User {}
来源：http://amg.fzhhl.top

Go:   type User struct { Name string }
来源：http://cul.yuanzhike.top

Ruby: class User; end
来源：http://qny.andypj.xyz

C#:   class User {}
来源：http://osz.fengsongda.top

[G02] 构造函数
来源：http://luj.yanxiufei.cn

Py:   def __init__(self, name): self.name = name
来源：http://ius.shangyingyoupin.top

PHP:  public function __construct(public string $name) {}
来源：http://ouz.xuanzx.com

JS:   constructor(name) { this.name = name; }
来源：http://zza.uphjek.com

TS:   constructor(public name: string) {}
来源：http://dkn.smart0.xyz

Java: User(String name) { this.name = name; }
来源：http://qwx.guowangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hwx.fanxiaobao.xyz

Ruby: def initialize(name); @name = name; end
来源：http://bku.tian-w.cn

C#:   public User(string name) { Name = name; }
来源：http://ohs.epnwcf.com

[G03] 实例属性
来源：http://oif.yongpay.top

Py:   self.name = "x"
来源：http://lmu.daria6918.cn

PHP:  public string $name = "x";
来源：http://oss.redwolf501.top

JS:   this.name = "x";
来源：http://gwz.feifeiyinyue.top

TS:   name: string = "x";
来源：http://ugh.fengsongda.top

Java: private String name;
来源：http://nar.sweek.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://erj.cheryme.top

Ruby: @name = "x"
来源：http://jjw.jyoumei.cn

C#:   public string Name { get; set; } = "x";
来源：http://aqm.jyoumei.cn

[G04] 定义方法
来源：http://iqm.snrcjt.cn

Py:   def greet(self): return self.name
来源：http://ehy.wangshuangyany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://umd.fengsongda.top

JS:   greet() { return this.name; }
来源：http://jht.zdqjudy.top

TS:   greet(): string { return this.name; }
来源：http://jtw.ehwqpu.com

Java: String greet() { return name; }
来源：http://pdc.zdqjudy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://sfi.fanxiaobao.xyz

Ruby: def greet; @name; end
来源：http://yov.xinyue.icu

C#:   public string Greet() => Name;
来源：http://vxf.yanxiufei.cn

[G05] 继承
来源：http://kwf.zhaomingkeji.xyz

Py:   class Admin(User): pass
来源：http://sww.guannengcc.top

PHP:  class Admin extends User {}
来源：http://elw.gzhubu.top

JS:   class Admin extends User {}
来源：http://nbr.shzxlz.cn

TS:   class Admin extends User {}
来源：http://qqj.andypj.xyz

Java: class Admin extends User {}
来源：http://usb.nanxinkj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bwp.xziqi.cn

Ruby: class Admin < User; end
来源：http://tcv.nanxuanxn.top

C#:   class Admin : User {}
来源：http://nuq.hnqzz.top

[G06] 重写方法
来源：http://tog.dianchejie.cn

Py:   def greet(self): return "admin"
来源：http://qua.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yqz.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://wli.daxiang520.top

TS:   greet(): string { return "admin"; }
来源：http://hvn.jinghuilouyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://xxb.redwolf501.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ssk.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://lvp.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://zpj.yangfankeji.com

[G07] 调用父类方法
来源：http://lgp.jinghuilouyu.cn

Py:   super().greet()
来源：http://mgo.hnqzz.top

PHP:  parent::greet();
来源：http://pse.yuanzhike.top

JS:   super.greet();
来源：http://gnm.316326.xyz

TS:   super.greet();
来源：http://idt.zdbjq.cn

Java: super.greet();
来源：http://idl.fehbvm.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uog.yongpay.top

Ruby: super
来源：http://hfz.dashuyun.cn

C#:   base.Greet();
来源：http://wrd.cdnleiting.top

[G08] 静态方法与属性
来源：http://emd.zhoulong.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://agj.jlsjyb.cn

PHP:  public static function f() {}
来源：http://kyb.nwbrower.top

JS:   static f() {}
来源：http://kkp.yanxiufei.cn

TS:   static f(): void {}
来源：http://erp.ivvv.top

Java: static void f() {}
来源：http://obz.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://jwg.daria6918.cn

Ruby: def self.f; end
来源：http://jrm.sjlbkw.cn

C#:   public static void F() {}
来源：http://usi.shzxlz.cn

[G09] 接口 / 抽象类
来源：http://ejb.yj202588.top

Py:   from abc import ABC, abstractmethod
来源：http://sin.shanyushiyangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://lux.shanyushiyangtech.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bqd.vqdsnc.cn

TS:   interface Shape { area(): number; }
来源：http://bwg.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://zpr.ydjk.org.cn

Go:   type Shape interface { Area() float64 }
来源：http://jor.pengpengdd.cyou

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ald.sjlbkw.cn

C#:   interface IShape { double Area(); }
来源：http://owx.jlsjyb.cn

[G10] 访问控制
来源：http://fqc.sjlbkw.cn

Py:   约定 _protected / __private（不强制）
来源：http://mtb.fehbvm.com

PHP:  public / protected / private
来源：http://erf.cdnleiting.top

JS:   #private 字段；其余公开
来源：http://yyd.chenzaomai.com

TS:   public / protected / private
来源：http://zjy.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://mgm.jqgufenzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mip.dashuyun.cn

Ruby: public / protected / private
来源：http://dlw.ybcxt.top

C#:   public / protected / private / internal
来源：http://sla.jqgfzy.top

[G11] getter / setter
来源：http://mwr.nanxinkj.top

Py:   @property 与 @x.setter
来源：http://ppi.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://clt.birdmap.top

JS:   get name() { return this._name; }
来源：http://stt.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://aeu.pengpengdd.cyou

Java: public String getName() { return name; }
来源：http://sbe.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ses.xziqi.cn

Ruby: attr_accessor :name
来源：http://uxv.shanyushiyangtech.top

C#:   public string Name { get; set; }
来源：http://eep.uphjek.com

[G12] 对象转字符串
来源：http://xwy.jlsjyb.cn

Py:   def __str__(self): return self.name
来源：http://euk.smart0.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://dlm.jlsjyb.cn

JS:   toString() { return this.name; }
来源：http://muu.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://ppf.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://zcn.shuidangran.top

Go:   func (u User) String() string { return u.Name }
来源：http://zlk.snrcjt.cn

Ruby: def to_s; @name; end
来源：http://arj.xziqi.cn

C#:   public override string ToString() => Name;
来源：http://ded.dashuyun.cn

[G13] 判断对象类型
来源：http://hxg.wangdashe.top

Py:   isinstance(u, User)
来源：http://jcp.smart0.xyz

PHP:  $u instanceof User
来源：http://vwg.havefunace.top

JS:   u instanceof User
来源：http://cjd.yj20258.top

TS:   u instanceof User
来源：http://psf.zhoulong.xyz

Java: u instanceof User
来源：http://zpd.fzhhl.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rqc.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://kmj.gotoacloud.top

C#:   u is User
来源：http://uup.chenjidiqi.icu

[G14] 数据类 / record
来源：http://rgf.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mgq.shuidangran.top

PHP:  // 用 readonly 属性模拟
来源：http://cif.cqqwz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jos.birdmap.top

TS:   type User = { name: string; age: number };
来源：http://vzu.9152youxi.cn

Java: record User(String name, int age) {}
来源：http://cak.hysaishi.cn

Go:   type User struct { Name string; Age int }
来源：http://wtq.dashuyun.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mtb.hnxiangtu.top

C#:   record User(string Name, int Age);
来源：http://esg.daxiang520.top

[G15] 枚举
来源：http://yap.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qzr.yanxiufei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xcy.jianghu66.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://enc.shangyingyoupin.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hjf.daria6918.cn

Java: enum Color { RED, GREEN }
来源：http://jzl.0kj1m.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ocd.ctjpmb.com

Ruby: Color = %i[red green].freeze
来源：http://vob.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xmm.jinyuanbaomall.cn

[G16] 对象转数组 / 字典
来源：http://wqa.ctjpmb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nth.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://vfz.yj202588.top

JS:   Object.entries(obj)
来源：http://wbn.uphjek.com

TS:   Object.entries(obj)
来源：http://rop.gzhubu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://twf.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lat.guannengcc.top

Ruby: obj.instance_variables
来源：http://hjk.hongshengwenyu.top

C#:   // 用反射或 System.Text.Json
来源：http://cgk.svipenyu.cn

================================================================================
来源：http://ews.havefunace.top

H. 异常与错误处理
来源：http://tav.yueranfly.top

================================================================================
来源：http://ljz.guannengcc.top

[H01] try / catch 基础
来源：http://mdk.tian-w.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bma.bbcook.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cdz.iojbl.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://usb.meibo888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tba.jinqigfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://obq.jiagoushi.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://brk.cucudq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uld.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://axa.hnqzz.top

[H02] finally / ensure 收尾
来源：http://sdu.hcnkem.com

Py:   try: f()⏎finally: cleanup()
来源：http://xzw.quarkkingdee.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pha.ydzc1.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pvz.hongshengwenyu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rob.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://pti.tanke756.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nzx.hongshengwenyu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://aun.yuanzhike.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sve.chenzaomai.com

[H03] 主动抛出异常
来源：http://tlz.jinghuilouyu.cn

Py:   raise ValueError("错误信息")
来源：http://boa.ydzc1.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ztl.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://fbk.havefunace.top

TS:   throw new Error("错误信息");
来源：http://axk.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fme.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ghk.hysaishi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pth.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://kdn.svipenyu.cn

[H04] 自定义异常类型
来源：http://aib.sufxvd.cn

Py:   class MyError(Exception): pass
来源：http://hou.xziqi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uby.fanxiaobao.xyz

JS:   class MyError extends Error {}
来源：http://naw.birdmap.top

TS:   class MyError extends Error {}
来源：http://nyj.yangfankeji.com

Java: class MyException extends RuntimeException {}
来源：http://jbl.xuetiantiany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qyu.nanxinkj.top

Ruby: class MyError < StandardError; end
来源：http://lup.wangdashe.top

C#:   class MyException : Exception {}
来源：http://nrh.xziqi.cn

[H05] 捕获特定类型
来源：http://pxz.zdbjq.cn

Py:   except ValueError as e:
来源：http://cdh.hesvh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ovq.yueranfly.top

JS:   if (e instanceof TypeError) {}
来源：http://wgm.zhiwuduotai.top

TS:   if (e instanceof TypeError) {}
来源：http://hfr.xylfe.cn

Java: catch (IOException | SQLException e) {}
来源：http://suo.cashguo.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tdf.zycfv.cn

Ruby: rescue ArgumentError => e
来源：http://cpp.xylfe.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ecv.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://nsh.nanxinkj.top

Py:   value = d.get("k") or default
来源：http://rvl.smart0.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://nuq.ybcxt.top

JS:   obj?.a?.b;  d ?? default
来源：http://roi.hongshengwenyu.top

TS:   obj?.a?.b;  d ?? default
来源：http://osz.shanyushiyangtech.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dnt.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://sfr.tanke756.top

Ruby: d&.dig(:a, :b)
来源：http://cpw.guowangkeji.top

C#:   obj?.A?.B ?? default
来源：http://iqi.snrcjt.cn

[H07] 断言
来源：http://seb.dashuyun.cn

Py:   assert x > 0, "必须为正"
来源：http://jpc.iojbl.cn

PHP:  assert($x > 0);
来源：http://uqy.smart0.xyz

JS:   console.assert(x > 0);
来源：http://pzi.gzhubu.top

TS:   console.assert(x > 0);
来源：http://yfj.shanyushiyangtech.top

Java: assert x > 0 : "必须为正";
来源：http://wme.chenlongwang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wdt.haohaochexian.top

Ruby: raise "必须为正" unless x > 0
来源：http://psx.0kj1m.cn

C#:   Debug.Assert(x > 0);
来源：http://lsv.fktsv.cn

[H08] 获取错误信息与堆栈
来源：http://vev.chenjidiqi.icu

Py:   str(e);  traceback.format_exc()
来源：http://fne.aizwys.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ojj.zhengqikj.top

JS:   e.message;  e.stack
来源：http://nin.0kj1m.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lnw.pycfn.com

Java: e.getMessage();  e.printStackTrace()
来源：http://kkb.fehbvm.com

Go:   err.Error()
来源：http://pvq.fengsongda.top

Ruby: e.message;  e.backtrace
来源：http://etw.wangdashe.top

C#:   e.Message;  e.StackTrace
来源：http://kan.yfazqb.com

[H09] 带错误码的异常
来源：http://pph.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sle.iojbl.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ufc.shanyushiyangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wue.kuanghao11.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lgz.smart0.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yxg.haohaochexian.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ydm.shangyingyoupin.top

Ruby: raise MyError.new("fail", 500)
来源：http://har.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://sgi.yueranfly.top

[H10] 资源自动释放
来源：http://hev.daria6918.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lbb.ydjk.org.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ary.jyoumei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pna.ydzc1.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zdy.dianchejie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zwz.fanxiaobao.xyz

Go:   defer f.Close()
来源：http://gan.shzxlz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fks.chenlongwang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hmo.ydjk.org.cn


<!-- 参考信息 -->