代发 wailian999

Ruby: File.delete("a.txt")
来源：http://pdt.guowangkeji.top

C#:   File.Delete("a.txt");
来源：http://qzt.yuanzhike.top

[F07] 创建目录（含多级）
来源：http://zmk.ivvv.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tjx.daxiang520.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fey.yongpay.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ecs.ivvv.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://abs.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ner.xuanzx.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bmd.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://smc.sysykeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vrf.daxiang520.top

[F08] 遍历目录
来源：http://roy.yuanzhike.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://epd.shuidangran.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ciz.chenjidiqi.icu

JS:   fs.readdirSync("dir")
来源：http://vae.tianlin.xyz

TS:   fs.readdirSync("dir")
来源：http://whe.vqdsnc.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ewk.hcnkem.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://zuf.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://apd.fanxiaobao.xyz

C#:   Directory.GetFiles("dir")
来源：http://pbs.guannengcc.top

[F09] 获取文件大小
来源：http://ksp.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://xpe.gotoacloud.top

PHP:  filesize("a.txt");
来源：http://okx.birdmap.top

JS:   fs.statSync("a.txt").size
来源：http://huw.fanxiaobao.xyz

TS:   fs.statSync("a.txt").size
来源：http://oro.redwolf501.top

Java: Files.size(Path.of("a.txt"))
来源：http://awy.feifeiyinyue.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pnh.ybcxt.top

Ruby: File.size("a.txt")
来源：http://mat.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://oqh.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://llj.daxiang520.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xbu.guannengcc.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bht.nanxinkj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://isa.zdqjudy.top

TS:   path.extname("a.txt")
来源：http://pgk.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yug.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qny.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ray.xuanzx.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ozf.tian-w.cn

[F11] 复制与移动文件
来源：http://zpv.gzhubu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kyz.uphjek.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fbj.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dsu.c1oappe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dqt.wangshuangyany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lei.yueranfly.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ogg.jianghu66.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vaj.shzxlz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://otz.svipenyu.cn

[F12] CSV 读写
来源：http://hty.fengsongda.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mxb.jlsjyb.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ozh.birdmap.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zxm.yueranfly.top

TS:   // 同上
来源：http://umg.sjlbkw.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cip.dashuyun.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gfl.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wyh.fehbvm.com

C#:   // 无内置：用 CsvHelper 库
来源：http://pfd.zhengqikj.top

================================================================================
来源：http://duo.sweek.top

G. 面向对象
来源：http://wzu.ppjwa.cn

================================================================================
来源：http://zud.cucudq.cn

[G01] 定义类
来源：http://xow.zhaomingkeji.xyz

Py:   class User: pass
来源：http://mgh.hcnkem.com

PHP:  class User {}
来源：http://wwi.ivvv.top

JS:   class User {}
来源：http://ttq.316326.xyz

TS:   class User { name: string = ""; }
来源：http://yxo.jiagoushi.top

Java: class User {}
来源：http://kdb.gogol.net.cn

Go:   type User struct { Name string }
来源：http://iby.shangyingyoupin.top

Ruby: class User; end
来源：http://ddw.epnwcf.com

C#:   class User {}
来源：http://txb.zhengqikj.top

[G02] 构造函数
来源：http://eee.wangdashe.top

Py:   def __init__(self, name): self.name = name
来源：http://lpg.9152youxi.cn

PHP:  public function __construct(public string $name) {}
来源：http://nkp.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://wmm.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://rgk.jinqigufen.top

Java: User(String name) { this.name = name; }
来源：http://qtg.hywenlv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hpa.fzhhl.top

Ruby: def initialize(name); @name = name; end
来源：http://azp.cheryme.top

C#:   public User(string name) { Name = name; }
来源：http://bzh.quarkkingdee.top

[G03] 实例属性
来源：http://vaa.tarul.cn

Py:   self.name = "x"
来源：http://bcs.hesvh.cn

PHP:  public string $name = "x";
来源：http://qzq.zhaomingkeji.xyz

JS:   this.name = "x";
来源：http://mqr.smart0.xyz

TS:   name: string = "x";
来源：http://irj.snrcjt.cn

Java: private String name;
来源：http://xlu.zycfv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eni.zhongyouzk.top

Ruby: @name = "x"
来源：http://hkn.iojbl.cn

C#:   public string Name { get; set; } = "x";
来源：http://hut.tanke756.top

[G04] 定义方法
来源：http://xuf.xziqi.cn

Py:   def greet(self): return self.name
来源：http://ram.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://knj.zhiwuduotai.top

JS:   greet() { return this.name; }
来源：http://smw.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://nsv.c1oappe.top

Java: String greet() { return name; }
来源：http://twh.yuxming.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cdi.snrcjt.cn

Ruby: def greet; @name; end
来源：http://ica.zhijiandao.cn

C#:   public string Greet() => Name;
来源：http://ezz.yuxming.cn

[G05] 继承
来源：http://lsm.shangyingyoupin.top

Py:   class Admin(User): pass
来源：http://dkn.yj202588.top

PHP:  class Admin extends User {}
来源：http://ijz.ywan-chungtsiang.top

JS:   class Admin extends User {}
来源：http://qet.cdnleiting.top

TS:   class Admin extends User {}
来源：http://eiq.nwbrower.top

Java: class Admin extends User {}
来源：http://dyk.fengsongda.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fbh.bbcook.cn

Ruby: class Admin < User; end
来源：http://wyv.daria6918.cn

C#:   class Admin : User {}
来源：http://dds.hongshengwenyu.top

[G06] 重写方法
来源：http://pid.meibo888.top

Py:   def greet(self): return "admin"
来源：http://kgk.bbcook.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://txt.guannengcc.top

JS:   greet() { return "admin"; }
来源：http://mym.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://ulb.gzhubu.top

Java: @Override String greet() { return "admin"; }
来源：http://ozn.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pxn.quarkkingdee.top

Ruby: def greet; "admin"; end
来源：http://jme.dashuyun.cn

C#:   public override string Greet() => "admin";
来源：http://zqx.tarul.cn

[G07] 调用父类方法
来源：http://wtv.cdnleiting.top

Py:   super().greet()
来源：http://qfe.yuxming.cn

PHP:  parent::greet();
来源：http://lmq.316326.xyz

JS:   super.greet();
来源：http://eaq.ydjk.org.cn

TS:   super.greet();
来源：http://aax.yfazqb.com

Java: super.greet();
来源：http://uis.cqqwz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jdv.feifeiyinyue.top

Ruby: super
来源：http://myi.hammf.cn

C#:   base.Greet();
来源：http://tej.ppjwa.cn

[G08] 静态方法与属性
来源：http://sxp.zhongyouzk.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ttn.wangdashe.top

PHP:  public static function f() {}
来源：http://wni.jiagoushi.top

JS:   static f() {}
来源：http://dxa.guannengcc.top

TS:   static f(): void {}
来源：http://bkw.yuxming.cn

Java: static void f() {}
来源：http://dxf.fzhhl.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ang.zhoulong.xyz

Ruby: def self.f; end
来源：http://hld.snrcjt.cn

C#:   public static void F() {}
来源：http://shc.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://bwt.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://ibp.jinyuanbaomall.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zdi.tianlin.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://oiu.yj20258888.top

TS:   interface Shape { area(): number; }
来源：http://iof.ywan-chungtsiang.top

Java: interface Shape { double area(); }
来源：http://lnu.ywan-chungtsiang.top

Go:   type Shape interface { Area() float64 }
来源：http://pdp.c1oappe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qqu.jinqigfzy.top

C#:   interface IShape { double Area(); }
来源：http://cae.daxiang520.top

[G10] 访问控制
来源：http://gil.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://nzl.fanxiaobao.xyz

PHP:  public / protected / private
来源：http://uxf.chenzaomai.com

JS:   #private 字段；其余公开
来源：http://jtm.guowangkeji.top

TS:   public / protected / private
来源：http://skv.jinqigfzy.top

Java: public / protected / private / 默认包级
来源：http://pzl.316326.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://bxv.smart0.xyz

Ruby: public / protected / private
来源：http://axi.mhx1999.top

C#:   public / protected / private / internal
来源：http://gzi.ppjwa.cn

[G11] getter / setter
来源：http://ssd.zhijiandao.cn

Py:   @property 与 @x.setter
来源：http://wyf.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ntu.ctjpmb.com

JS:   get name() { return this._name; }
来源：http://bci.ivvv.top

TS:   get name(): string { return this._name; }
来源：http://qhc.nanxuanxn.top

Java: public String getName() { return name; }
来源：http://orl.jinyuanbaomall.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gqu.xuetiantiany.cn

Ruby: attr_accessor :name
来源：http://kmm.kuanghao11.cn

C#:   public string Name { get; set; }
来源：http://ukp.yangfankeji.com

[G12] 对象转字符串
来源：http://kne.meibo888.top

Py:   def __str__(self): return self.name
来源：http://msj.zhongyouzk.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tbm.gotoacloud.top

JS:   toString() { return this.name; }
来源：http://xiq.yongpay.top

TS:   toString(): string { return this.name; }
来源：http://udt.gaohongyu789.top

Java: @Override public String toString() { return name; }
来源：http://wlb.cqqwz.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wep.feifeiyinyue.top

Ruby: def to_s; @name; end
来源：http://yod.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://uma.svipenyu.cn

[G13] 判断对象类型
来源：http://drx.daxiang520.top

Py:   isinstance(u, User)
来源：http://yrq.birdmap.top

PHP:  $u instanceof User
来源：http://rrr.ehwqpu.com

JS:   u instanceof User
来源：http://gyt.fengsongda.top

TS:   u instanceof User
来源：http://ssq.gzhubu.top

Java: u instanceof User
来源：http://yne.meibo888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://sru.c1oappe.top

Ruby: u.is_a?(User)
来源：http://hla.ppjwa.cn

C#:   u is User
来源：http://rmw.sysykeji.top

[G14] 数据类 / record
来源：http://mmt.nwbrower.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://buz.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://xmt.zhijiandao.cn

JS:   // 无内置：普通类或对象字面量
来源：http://iad.jlsjyb.cn

TS:   type User = { name: string; age: number };
来源：http://odm.yj20258.top

Java: record User(String name, int age) {}
来源：http://suq.0kj1m.cn

Go:   type User struct { Name string; Age int }
来源：http://euk.daria6918.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nhh.uphjek.com

C#:   record User(string Name, int Age);
来源：http://zhv.yj20258.top

[G15] 枚举
来源：http://gto.yuxming.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ioo.yueranfly.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hgi.guannengcc.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yjo.jinghuilouyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oof.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://cqc.guannengcc.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://edp.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://vsp.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lwv.iojbl.cn

[G16] 对象转数组 / 字典
来源：http://umv.tianlin.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qde.zhixingplan.top

PHP:  get_object_vars($obj);
来源：http://lps.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://ige.tarul.cn

TS:   Object.entries(obj)
来源：http://isk.c1oappe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://umc.vqdsnc.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hyw.tian-w.cn

Ruby: obj.instance_variables
来源：http://ddk.pycfn.com

C#:   // 用反射或 System.Text.Json
来源：http://ilc.jinghuilouyu.cn

================================================================================
来源：http://jvh.daria6918.cn

H. 异常与错误处理
来源：http://fpi.dianchejie.cn

================================================================================
来源：http://niz.cashguo.top

[H01] try / catch 基础
来源：http://gjj.hywenlv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hor.ppjwa.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nvh.aibaodan.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cis.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://asv.vehdjk.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qlj.hnqzz.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cug.shanyushiyangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://aoa.ydzc1.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nnj.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://etq.ydzc1.top

Py:   try: f()⏎finally: cleanup()
来源：http://cci.pengpengdd.cyou

PHP:  try { f(); } finally { cleanup(); }
来源：http://sgh.yj202588.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zle.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vae.guannengcc.top

Java: try { f(); } finally { cleanup(); }
来源：http://uwg.zhongyouzk.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xjr.fanxiaobao.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://lgo.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nqn.hongshengwenyu.top

[H03] 主动抛出异常
来源：http://mwc.wangshuangyany.cn

Py:   raise ValueError("错误信息")
来源：http://whl.cheryme.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://trx.yonumen.top

JS:   throw new Error("错误信息");
来源：http://cjc.hywenlv.cn

TS:   throw new Error("错误信息");
来源：http://mav.vqdsnc.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xvv.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://myi.shuidangran.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ojo.ywan-chungtsiang.top

C#:   throw new ArgumentException("错误信息");
来源：http://tqw.smart0.xyz

[H04] 自定义异常类型
来源：http://jcz.shanyushiyangtech.top

Py:   class MyError(Exception): pass
来源：http://efx.zycfv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://anm.ehwqpu.com

JS:   class MyError extends Error {}
来源：http://txx.yanxiufei.cn

TS:   class MyError extends Error {}
来源：http://jrk.hywenlv.cn

Java: class MyException extends RuntimeException {}
来源：http://dnr.yuanzhike.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://due.yongpay.top

Ruby: class MyError < StandardError; end
来源：http://sxv.andypj.xyz

C#:   class MyException : Exception {}
来源：http://mdv.tarul.cn

[H05] 捕获特定类型
来源：http://qtv.wangshuangyany.cn

Py:   except ValueError as e:
来源：http://itg.cqqwz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lgb.dianchejie.cn

JS:   if (e instanceof TypeError) {}
来源：http://zxa.nanxinkj.top

TS:   if (e instanceof TypeError) {}
来源：http://pca.xinyue.icu

Java: catch (IOException | SQLException e) {}
来源：http://boc.tanke756.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vbx.fzhhl.top

Ruby: rescue ArgumentError => e
来源：http://hsa.tarul.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vfr.dashuyun.cn

[H06] 可选值 / 空值安全访问
来源：http://zcb.ydjk.org.cn

Py:   value = d.get("k") or default
来源：http://gir.smart0.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://bcj.haohaochexian.top

JS:   obj?.a?.b;  d ?? default
来源：http://tlp.bbcook.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nvl.epnwcf.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kie.nanxinkj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kid.guannengcc.top

Ruby: d&.dig(:a, :b)
来源：http://vbf.yj202588.top

C#:   obj?.A?.B ?? default
来源：http://nyt.jyoumei.cn

[H07] 断言
来源：http://jbw.sufxvd.cn

Py:   assert x > 0, "必须为正"
来源：http://oyz.hnxiangtu.top

PHP:  assert($x > 0);
来源：http://zwg.vehdjk.com

JS:   console.assert(x > 0);
来源：http://bzv.cqqwz.cn

TS:   console.assert(x > 0);
来源：http://abe.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://uik.hongshengwenyu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://atx.yj202588.top

Ruby: raise "必须为正" unless x > 0
来源：http://fqg.yongpay.top

C#:   Debug.Assert(x > 0);
来源：http://aol.guannengcc.top

[H08] 获取错误信息与堆栈
来源：http://ymd.wangdashe.top

Py:   str(e);  traceback.format_exc()
来源：http://ldo.fanxiaobao.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gkq.jinghuilouyu.cn

JS:   e.message;  e.stack
来源：http://fho.pengpengdd.cyou

TS:   e instanceof Error ? e.message : String(e)
来源：http://znb.dianchejie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://iqj.ydzc1.top

Go:   err.Error()
来源：http://arf.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://ape.9152youxi.cn

C#:   e.Message;  e.StackTrace
来源：http://jek.chenjidiqi.icu

[H09] 带错误码的异常
来源：http://nzv.bjfxy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nht.xziqi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lrh.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kvy.jyoumei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lzs.redwolf501.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vlk.yfazqb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zmh.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://ssy.epnwcf.com

C#:   // 自定义异常类中加 Code 属性
来源：http://fgh.sysykeji.top

[H10] 资源自动释放
来源：http://nqb.shanyushiyangtech.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qwk.birdmap.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uoc.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://trd.gotoacloud.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://azz.zhijiandao.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pxs.yfazqb.com

Go:   defer f.Close()
来源：http://dey.cdnleiting.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qxa.hesvh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ygs.hammf.cn

================================================================================
来源：http://evq.cashguo.top

I. 正则表达式
来源：http://vwg.sufxvd.cn

================================================================================
来源：http://iny.shanyushiyangkeji.top

[I01] 判断是否匹配
来源：http://ryx.0kj1m.cn


<!-- 参考信息 -->