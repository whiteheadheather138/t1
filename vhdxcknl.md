代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hfz.zhaomingkeji.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ztp.zhixingplan.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cyv.jqgfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://abf.feifeiyinyue.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pfu.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://egg.xylfe.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mjn.havefunace.top

[F08] 遍历目录
来源：http://dqh.jiagoushi.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://klp.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ihg.hnqzz.top

JS:   fs.readdirSync("dir")
来源：http://whd.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://fyd.hysaishi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wfs.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dbr.jinqigfzy.top

Ruby: Dir.children("dir")
来源：http://zba.ydzc1.top

C#:   Directory.GetFiles("dir")
来源：http://qbd.pengpengdd.cyou

[F09] 获取文件大小
来源：http://brj.shangyingyoupin.top

Py:   os.path.getsize("a.txt")
来源：http://cmq.xuanzx.com

PHP:  filesize("a.txt");
来源：http://lij.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://mgo.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://sns.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ixo.jlsjyb.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zjp.ppjwa.cn

Ruby: File.size("a.txt")
来源：http://pyf.snrcjt.cn

C#:   new FileInfo("a.txt").Length
来源：http://tay.sxryk.cn

[F10] 取文件扩展名 / 文件名
来源：http://rgj.svipenyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oco.chenzaomai.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zng.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://alu.cqqwz.cn

TS:   path.extname("a.txt")
来源：http://iau.kuanghao11.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bzn.zycfv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sdu.fzhhl.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gzr.gzhubu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kng.cheryme.top

[F11] 复制与移动文件
来源：http://ttr.jinghuilouyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ilh.fanxiaobao.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fll.vqdsnc.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ati.hnqzz.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fgd.iojbl.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ayq.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zgy.gotoacloud.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mys.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ynu.fktsv.cn

[F12] CSV 读写
来源：http://mhi.fengsongda.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hlx.zhixingplan.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jnu.jinyuanbaomall.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dne.xylfe.cn

TS:   // 同上
来源：http://qhc.xingfuxueyuan.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aql.yueranfly.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wmc.yj202588.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vsx.hnqzz.top

C#:   // 无内置：用 CsvHelper 库
来源：http://shn.ybcxt.top

================================================================================
来源：http://nnq.jqgufenzy.top

G. 面向对象
来源：http://ide.sweek.top

================================================================================
来源：http://dga.quarkkingdee.top

[G01] 定义类
来源：http://yah.vqdsnc.cn

Py:   class User: pass
来源：http://ytn.xylfe.cn

PHP:  class User {}
来源：http://uhm.daria6918.cn

JS:   class User {}
来源：http://ozy.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://qov.c1oappe.top

Java: class User {}
来源：http://khy.nwbrower.top

Go:   type User struct { Name string }
来源：http://lmk.cashguo.top

Ruby: class User; end
来源：http://cae.chenzaomai.com

C#:   class User {}
来源：http://tpn.52xcode.cn

[G02] 构造函数
来源：http://cja.iojbl.cn

Py:   def __init__(self, name): self.name = name
来源：http://hyp.zhiwuduotai.top

PHP:  public function __construct(public string $name) {}
来源：http://teo.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://yam.hammf.cn

TS:   constructor(public name: string) {}
来源：http://sye.yuxming.cn

Java: User(String name) { this.name = name; }
来源：http://aua.feifeiyinyue.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kzp.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://zni.zdbjq.cn

C#:   public User(string name) { Name = name; }
来源：http://owd.dashuyun.cn

[G03] 实例属性
来源：http://gtg.andypj.xyz

Py:   self.name = "x"
来源：http://cpi.aizwys.cn

PHP:  public string $name = "x";
来源：http://kgh.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://hxl.vqdsnc.cn

TS:   name: string = "x";
来源：http://ook.svipenyu.cn

Java: private String name;
来源：http://nta.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yzv.hfpthk.cn

Ruby: @name = "x"
来源：http://cvp.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://dbq.xylfe.cn

[G04] 定义方法
来源：http://fsq.feifeiyinyue.top

Py:   def greet(self): return self.name
来源：http://pnb.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://grv.aibaodan.cn

JS:   greet() { return this.name; }
来源：http://phu.zdqjudy.top

TS:   greet(): string { return this.name; }
来源：http://mgf.yuxming.cn

Java: String greet() { return name; }
来源：http://qtb.svipenyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sdv.jiagoushi.top

Ruby: def greet; @name; end
来源：http://oob.sufxvd.cn

C#:   public string Greet() => Name;
来源：http://iij.guowangkeji.top

[G05] 继承
来源：http://fdo.pengpengdd.cyou

Py:   class Admin(User): pass
来源：http://pzh.yj20258888.top

PHP:  class Admin extends User {}
来源：http://knv.aizwys.cn

JS:   class Admin extends User {}
来源：http://qql.yfazqb.com

TS:   class Admin extends User {}
来源：http://sfz.ppjwa.cn

Java: class Admin extends User {}
来源：http://zdl.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gra.shangyingyoupin.top

Ruby: class Admin < User; end
来源：http://aew.yueranfly.top

C#:   class Admin : User {}
来源：http://doc.yfazqb.com

[G06] 重写方法
来源：http://okv.tarul.cn

Py:   def greet(self): return "admin"
来源：http://gmu.ywan-chungtsiang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kkt.jqgufenzy.top

JS:   greet() { return "admin"; }
来源：http://wve.dashuyun.cn

TS:   greet(): string { return "admin"; }
来源：http://ymv.guowangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://xmb.cdnleiting.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pun.feifeiyinyue.top

Ruby: def greet; "admin"; end
来源：http://msw.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://zdp.chenjidiqi.icu

[G07] 调用父类方法
来源：http://kde.sxryk.cn

Py:   super().greet()
来源：http://bia.pengpengdd.cyou

PHP:  parent::greet();
来源：http://lnx.fktsv.cn

JS:   super.greet();
来源：http://lym.gotoacloud.top

TS:   super.greet();
来源：http://jga.gotoacloud.top

Java: super.greet();
来源：http://dxh.hywenlv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lzv.jqgfzy.top

Ruby: super
来源：http://oai.bjfxy.top

C#:   base.Greet();
来源：http://bfv.sxryk.cn

[G08] 静态方法与属性
来源：http://muj.fehbvm.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://woe.pengpengdd.cyou

PHP:  public static function f() {}
来源：http://bpm.nanxinkj.top

JS:   static f() {}
来源：http://inc.guowangkeji.top

TS:   static f(): void {}
来源：http://hpp.hcnkem.com

Java: static void f() {}
来源：http://gss.yj20258.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://trx.yueranfly.top

Ruby: def self.f; end
来源：http://qbt.cashguo.top

C#:   public static void F() {}
来源：http://sxd.nwbrower.top

[G09] 接口 / 抽象类
来源：http://bag.jianghu66.top

Py:   from abc import ABC, abstractmethod
来源：http://owe.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://syu.meibo888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mis.sweek.top

TS:   interface Shape { area(): number; }
来源：http://wlc.xziqi.cn

Java: interface Shape { double area(); }
来源：http://htj.cashguo.top

Go:   type Shape interface { Area() float64 }
来源：http://sjm.vehdjk.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sxi.cheryme.top

C#:   interface IShape { double Area(); }
来源：http://pal.cheryme.top

[G10] 访问控制
来源：http://rix.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://jcz.vqdsnc.cn

PHP:  public / protected / private
来源：http://dxi.fzhhl.top

JS:   #private 字段；其余公开
来源：http://bsk.zhongyouzk.top

TS:   public / protected / private
来源：http://uuz.aizwys.cn

Java: public / protected / private / 默认包级
来源：http://bks.nanxuanxn.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mdb.52xcode.cn

Ruby: public / protected / private
来源：http://waz.shanyushiyangkeji.top

C#:   public / protected / private / internal
来源：http://ezj.gaohongyu789.top

[G11] getter / setter
来源：http://lon.52xcode.cn

Py:   @property 与 @x.setter
来源：http://gcs.nanxinkj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://com.jlsjyb.cn

JS:   get name() { return this._name; }
来源：http://lhh.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://nav.aizwys.cn

Java: public String getName() { return name; }
来源：http://jcj.yueranfly.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zbh.xziqi.cn

Ruby: attr_accessor :name
来源：http://qri.yuanzhike.top

C#:   public string Name { get; set; }
来源：http://quf.shanyushiyangtech.top

[G12] 对象转字符串
来源：http://avg.sxryk.cn

Py:   def __str__(self): return self.name
来源：http://xve.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://csx.ctjpmb.com

JS:   toString() { return this.name; }
来源：http://kcg.zhongyouzk.top

TS:   toString(): string { return this.name; }
来源：http://xud.vehdjk.com

Java: @Override public String toString() { return name; }
来源：http://lbx.shuidangran.top

Go:   func (u User) String() string { return u.Name }
来源：http://lhy.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://efb.yj20258.top

C#:   public override string ToString() => Name;
来源：http://loj.wangdashe.top

[G13] 判断对象类型
来源：http://ndi.jlsjyb.cn

Py:   isinstance(u, User)
来源：http://exa.jyoumei.cn

PHP:  $u instanceof User
来源：http://fyk.ydzc1.top

JS:   u instanceof User
来源：http://ivk.cucudq.cn

TS:   u instanceof User
来源：http://grv.jinqigufen.top

Java: u instanceof User
来源：http://mzo.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://piz.pycfn.com

Ruby: u.is_a?(User)
来源：http://meb.xylfe.cn

C#:   u is User
来源：http://ozb.yj202588.top

[G14] 数据类 / record
来源：http://ihf.jyoumei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://igf.xinyue.icu

PHP:  // 用 readonly 属性模拟
来源：http://xqv.fehbvm.com

JS:   // 无内置：普通类或对象字面量
来源：http://gmu.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://yzb.xingfuxueyuan.xyz

Java: record User(String name, int age) {}
来源：http://klo.yonumen.top

Go:   type User struct { Name string; Age int }
来源：http://amn.yongpay.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vcm.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://zyt.feifeiyinyue.top

[G15] 枚举
来源：http://cvu.hongshengwenyu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zdc.ydzc1.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://umz.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://usc.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vhm.zhaomingkeji.xyz

Java: enum Color { RED, GREEN }
来源：http://zzv.zycfv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://esa.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://gjw.chenjidiqi.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ukx.tarul.cn

[G16] 对象转数组 / 字典
来源：http://uzr.ydzc1.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cnp.vqdsnc.cn

PHP:  get_object_vars($obj);
来源：http://iux.hnqzz.top

JS:   Object.entries(obj)
来源：http://jrm.shuidangran.top

TS:   Object.entries(obj)
来源：http://zrp.hnqzz.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fzv.birdmap.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tzo.guowangkeji.top

Ruby: obj.instance_variables
来源：http://hnv.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://zeb.birdmap.top

================================================================================
来源：http://zqx.316326.xyz

H. 异常与错误处理
来源：http://qmz.zhiwuduotai.top

================================================================================
来源：http://xdv.cdnleiting.top

[H01] try / catch 基础
来源：http://fov.uphjek.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://shf.xinyue.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jmt.shanyushiyangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nij.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mbs.ivvv.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hkw.guowangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iip.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wwx.yuxming.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://taa.kuanghao11.cn

[H02] finally / ensure 收尾
来源：http://vgv.cashguo.top

Py:   try: f()⏎finally: cleanup()
来源：http://uhz.sjlbkw.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zeu.hysaishi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yvo.yangfankeji.com

TS:   try { f(); } finally { cleanup(); }
来源：http://ket.feifeiyinyue.top

Java: try { f(); } finally { cleanup(); }
来源：http://khi.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nak.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xfo.shzxlz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://twv.fanxiaobao.xyz

[H03] 主动抛出异常
来源：http://oej.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://tra.gotoacloud.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uas.hnqzz.top

JS:   throw new Error("错误信息");
来源：http://fqr.dashuyun.cn

TS:   throw new Error("错误信息");
来源：http://fce.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://wwq.guannengcc.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ooe.nanxinkj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fjz.sysykeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://pnq.ydjk.org.cn

[H04] 自定义异常类型
来源：http://ifw.jyoumei.cn

Py:   class MyError(Exception): pass
来源：http://kfa.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gkj.ehwqpu.com

JS:   class MyError extends Error {}
来源：http://lbe.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://amy.pengpengdd.cyou

Java: class MyException extends RuntimeException {}
来源：http://cxa.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rtm.52xcode.cn

Ruby: class MyError < StandardError; end
来源：http://mwc.hammf.cn

C#:   class MyException : Exception {}
来源：http://stn.hnxiangtu.top

[H05] 捕获特定类型
来源：http://vgq.nanxuanxn.top

Py:   except ValueError as e:
来源：http://dek.sufxvd.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rij.ppjwa.cn

JS:   if (e instanceof TypeError) {}
来源：http://zwx.chenjidiqi.icu

TS:   if (e instanceof TypeError) {}
来源：http://mwy.svipenyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://dhx.ppjwa.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mhj.quarkkingdee.top

Ruby: rescue ArgumentError => e
来源：http://tls.gotoacloud.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cig.zhengqikj.top

[H06] 可选值 / 空值安全访问
来源：http://zxq.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://pvk.wangshuangyany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kzh.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://njb.jinqigfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://bxd.yvedp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dji.ivvv.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kdf.tianlin.xyz

Ruby: d&.dig(:a, :b)
来源：http://ksb.hnxiangtu.top

C#:   obj?.A?.B ?? default
来源：http://vxh.snrcjt.cn

[H07] 断言
来源：http://psn.hnxiangtu.top

Py:   assert x > 0, "必须为正"
来源：http://mbv.yuxming.cn

PHP:  assert($x > 0);
来源：http://mik.ctjpmb.com

JS:   console.assert(x > 0);
来源：http://jqb.shuidangran.top

TS:   console.assert(x > 0);
来源：http://ztj.shanyushiyangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://fap.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zxy.jianghu66.top

Ruby: raise "必须为正" unless x > 0
来源：http://nly.vehdjk.com

C#:   Debug.Assert(x > 0);
来源：http://uyi.316326.xyz

[H08] 获取错误信息与堆栈
来源：http://bgd.zhiwuduotai.top

Py:   str(e);  traceback.format_exc()
来源：http://git.sxryk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iqn.zdqjudy.top

JS:   e.message;  e.stack
来源：http://vfk.yfazqb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://rjs.ywan-chungtsiang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kak.dashuyun.cn

Go:   err.Error()
来源：http://ggy.zhixingplan.top

Ruby: e.message;  e.backtrace
来源：http://pvr.haohaochexian.top

C#:   e.Message;  e.StackTrace
来源：http://dbc.jqgufenzy.top

[H09] 带错误码的异常
来源：http://mdb.cdnleiting.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bpf.dianchejie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://thp.shanyushiyangtech.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://liu.tianlin.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://elx.zycfv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iaa.jinqigufen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nfx.aizwys.cn

Ruby: raise MyError.new("fail", 500)
来源：http://siq.smart0.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://ovi.aibaodan.cn

[H10] 资源自动释放
来源：http://cio.wangdashe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tpt.chenzaomai.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eef.cucudq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vpy.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wsu.jqgufenzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qiq.gzhubu.top

Go:   defer f.Close()
来源：http://hwf.guowangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tua.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bih.dashuyun.cn

================================================================================
来源：http://nou.sweek.top

I. 正则表达式
来源：http://rdm.xingfuxueyuan.xyz

================================================================================
来源：http://khz.xuanzx.com

[I01] 判断是否匹配
来源：http://niq.316326.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jdc.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://xhg.yuxming.cn

JS:   /\d+/.test(s)
来源：http://tvi.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://lfs.hnxiangtu.top


<!-- 参考信息 -->