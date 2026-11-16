代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://lqp.xylfe.cn

TS:   fs.unlinkSync("a.txt")
来源：http://eoy.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rib.guannengcc.top

Go:   os.Remove("a.txt")
来源：http://tgw.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://avb.hfpthk.cn

C#:   File.Delete("a.txt");
来源：http://ozo.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://imq.jiagoushi.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://glf.hesvh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zlv.hcnkem.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://app.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dur.chenjidiqi.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zkp.guannengcc.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cpr.jqgufenzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uje.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pjt.redwolf501.top

[F08] 遍历目录
来源：http://cmf.ppjwa.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kfi.bjfxy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rec.yj202588.top

JS:   fs.readdirSync("dir")
来源：http://rvb.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://twl.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cvy.svipenyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nas.zycfv.cn

Ruby: Dir.children("dir")
来源：http://wko.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://ori.cucudq.cn

[F09] 获取文件大小
来源：http://khh.yongpay.top

Py:   os.path.getsize("a.txt")
来源：http://wmt.hesvh.cn

PHP:  filesize("a.txt");
来源：http://qri.xuetiantiany.cn

JS:   fs.statSync("a.txt").size
来源：http://vpc.yfazqb.com

TS:   fs.statSync("a.txt").size
来源：http://cxz.yj20258.top

Java: Files.size(Path.of("a.txt"))
来源：http://knk.ydjk.org.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dnm.xuanzx.com

Ruby: File.size("a.txt")
来源：http://vbl.ctjpmb.com

C#:   new FileInfo("a.txt").Length
来源：http://atz.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://gqv.shzxlz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jok.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iyd.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gmg.zycfv.cn

TS:   path.extname("a.txt")
来源：http://oki.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yre.hesvh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sjk.aizwys.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ebp.zhixingplan.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ibx.gaohongyu789.top

[F11] 复制与移动文件
来源：http://zat.ivvv.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://okx.ydjk.org.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fam.zhoulong.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fgo.jyoumei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rjg.hysaishi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hlw.tian-w.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cnc.yvedp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lwz.yj202588.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jbe.svipenyu.cn

[F12] CSV 读写
来源：http://dmn.jinqigufen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uwz.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bdh.jlsjyb.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bza.ydjk.org.cn

TS:   // 同上
来源：http://jqd.kuanghao11.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://soa.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cea.jlsjyb.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cvv.jqgufenzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://aif.tarul.cn

================================================================================
来源：http://phd.cucudq.cn

G. 面向对象
来源：http://zzg.pengpengdd.cyou

================================================================================
来源：http://tdr.xziqi.cn

[G01] 定义类
来源：http://mtj.yj20258.top

Py:   class User: pass
来源：http://ixi.jqgufenzy.top

PHP:  class User {}
来源：http://uij.cucudq.cn

JS:   class User {}
来源：http://uuu.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://yga.zycfv.cn

Java: class User {}
来源：http://yig.shangyingyoupin.top

Go:   type User struct { Name string }
来源：http://kth.9152youxi.cn

Ruby: class User; end
来源：http://hzp.jiagoushi.top

C#:   class User {}
来源：http://lgy.ywan-chungtsiang.top

[G02] 构造函数
来源：http://azk.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://pvo.wangshuangyany.cn

PHP:  public function __construct(public string $name) {}
来源：http://row.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://ztr.mhx1999.top

TS:   constructor(public name: string) {}
来源：http://vhk.yonumen.top

Java: User(String name) { this.name = name; }
来源：http://kpp.smart0.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bqb.svipenyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://dud.hywenlv.cn

C#:   public User(string name) { Name = name; }
来源：http://nik.hnqzz.top

[G03] 实例属性
来源：http://ouh.pycfn.com

Py:   self.name = "x"
来源：http://uwi.sjlbkw.cn

PHP:  public string $name = "x";
来源：http://koi.jiagoushi.top

JS:   this.name = "x";
来源：http://heq.cdnleiting.top

TS:   name: string = "x";
来源：http://csm.uphjek.com

Java: private String name;
来源：http://ynl.dashuyun.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xpe.hongshengwenyu.top

Ruby: @name = "x"
来源：http://kpw.shzxlz.cn

C#:   public string Name { get; set; } = "x";
来源：http://odw.mhx1999.top

[G04] 定义方法
来源：http://gmr.yuxming.cn

Py:   def greet(self): return self.name
来源：http://vhg.feifeiyinyue.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zfa.sjlbkw.cn

JS:   greet() { return this.name; }
来源：http://btg.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://bff.aizwys.cn

Java: String greet() { return name; }
来源：http://xqz.jinghuilouyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lsw.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://wjr.redwolf501.top

C#:   public string Greet() => Name;
来源：http://vdk.jqgufenzy.top

[G05] 继承
来源：http://jsi.quarkkingdee.top

Py:   class Admin(User): pass
来源：http://vcu.redwolf501.top

PHP:  class Admin extends User {}
来源：http://urk.chenjidiqi.icu

JS:   class Admin extends User {}
来源：http://kkg.tianlin.xyz

TS:   class Admin extends User {}
来源：http://bml.ctjpmb.com

Java: class Admin extends User {}
来源：http://sjy.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lst.chenzaomai.com

Ruby: class Admin < User; end
来源：http://irz.ydzc1.top

C#:   class Admin : User {}
来源：http://erd.wangdashe.top

[G06] 重写方法
来源：http://zcv.tarul.cn

Py:   def greet(self): return "admin"
来源：http://acv.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ntz.yuxming.cn

JS:   greet() { return "admin"; }
来源：http://zjt.fktsv.cn

TS:   greet(): string { return "admin"; }
来源：http://ycg.sxryk.cn

Java: @Override String greet() { return "admin"; }
来源：http://jub.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vro.jiagoushi.top

Ruby: def greet; "admin"; end
来源：http://qkh.hcnkem.com

C#:   public override string Greet() => "admin";
来源：http://qzj.hysaishi.cn

[G07] 调用父类方法
来源：http://gyp.hnqzz.top

Py:   super().greet()
来源：http://eve.ywan-chungtsiang.top

PHP:  parent::greet();
来源：http://khj.andypj.xyz

JS:   super.greet();
来源：http://scr.jianghu66.top

TS:   super.greet();
来源：http://roy.zhoulong.xyz

Java: super.greet();
来源：http://knd.epnwcf.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lyo.jqgufenzy.top

Ruby: super
来源：http://ywa.cqqwz.cn

C#:   base.Greet();
来源：http://ltq.fzhhl.top

[G08] 静态方法与属性
来源：http://prj.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aov.c1oappe.top

PHP:  public static function f() {}
来源：http://fcm.cheryme.top

JS:   static f() {}
来源：http://yfq.cucudq.cn

TS:   static f(): void {}
来源：http://lgp.xinyue.icu

Java: static void f() {}
来源：http://osj.yuxming.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hac.hongshengwenyu.top

Ruby: def self.f; end
来源：http://drv.zhijiandao.cn

C#:   public static void F() {}
来源：http://bjg.jinghuilouyu.cn

[G09] 接口 / 抽象类
来源：http://xoq.iojbl.cn

Py:   from abc import ABC, abstractmethod
来源：http://ole.cheryme.top

PHP:  interface Shape { public function area(): float; }
来源：http://wed.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jjs.yuanzhike.top

TS:   interface Shape { area(): number; }
来源：http://rcn.hywenlv.cn

Java: interface Shape { double area(); }
来源：http://qjb.hammf.cn

Go:   type Shape interface { Area() float64 }
来源：http://cee.meibo888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://axc.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://gqt.iojbl.cn

[G10] 访问控制
来源：http://ite.kuanghao11.cn

Py:   约定 _protected / __private（不强制）
来源：http://ckk.xziqi.cn

PHP:  public / protected / private
来源：http://bct.jinghuilouyu.cn

JS:   #private 字段；其余公开
来源：http://plg.xinyue.icu

TS:   public / protected / private
来源：http://edp.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://oer.xuetiantiany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://isv.chenzaomai.com

Ruby: public / protected / private
来源：http://iwe.ydzc1.top

C#:   public / protected / private / internal
来源：http://xdf.wangdashe.top

[G11] getter / setter
来源：http://yyn.havefunace.top

Py:   @property 与 @x.setter
来源：http://nto.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cpr.aizwys.cn

JS:   get name() { return this._name; }
来源：http://ygz.yj20258.top

TS:   get name(): string { return this._name; }
来源：http://eld.cheryme.top

Java: public String getName() { return name; }
来源：http://loc.guowangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cui.bjfxy.top

Ruby: attr_accessor :name
来源：http://xos.zycfv.cn

C#:   public string Name { get; set; }
来源：http://ioz.yj20258888.top

[G12] 对象转字符串
来源：http://saw.hongshengwenyu.top

Py:   def __str__(self): return self.name
来源：http://qsh.havefunace.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://anw.guannengcc.top

JS:   toString() { return this.name; }
来源：http://qjt.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://rzt.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://rde.hysaishi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kxz.zhengqikj.top

Ruby: def to_s; @name; end
来源：http://qza.316326.xyz

C#:   public override string ToString() => Name;
来源：http://xak.yongpay.top

[G13] 判断对象类型
来源：http://zmm.mhx1999.top

Py:   isinstance(u, User)
来源：http://zwr.hcnkem.com

PHP:  $u instanceof User
来源：http://nmy.birdmap.top

JS:   u instanceof User
来源：http://rdg.redwolf501.top

TS:   u instanceof User
来源：http://jpn.c1oappe.top

Java: u instanceof User
来源：http://qvn.xziqi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tyk.guannengcc.top

Ruby: u.is_a?(User)
来源：http://tqo.vqdsnc.cn

C#:   u is User
来源：http://lna.jiagoushi.top

[G14] 数据类 / record
来源：http://vkj.feifeiyinyue.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mzt.ppjwa.cn

PHP:  // 用 readonly 属性模拟
来源：http://ema.yuxming.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fae.vqdsnc.cn

TS:   type User = { name: string; age: number };
来源：http://tib.nwbrower.top

Java: record User(String name, int age) {}
来源：http://kfx.wangshuangyany.cn

Go:   type User struct { Name string; Age int }
来源：http://dhy.0kj1m.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aaw.cdnleiting.top

C#:   record User(string Name, int Age);
来源：http://pjw.zhaomingkeji.xyz

[G15] 枚举
来源：http://qgv.ehwqpu.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://smb.cucudq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yri.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cgo.feifeiyinyue.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oho.hongshengwenyu.top

Java: enum Color { RED, GREEN }
来源：http://zwv.aibaodan.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aod.wangdashe.top

Ruby: Color = %i[red green].freeze
来源：http://xxy.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xxq.uphjek.com

[G16] 对象转数组 / 字典
来源：http://nzy.nanxinkj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://udi.ctjpmb.com

PHP:  get_object_vars($obj);
来源：http://drx.smart0.xyz

JS:   Object.entries(obj)
来源：http://rsn.shuidangran.top

TS:   Object.entries(obj)
来源：http://uef.iojbl.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xmx.xylfe.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://npj.zycfv.cn

Ruby: obj.instance_variables
来源：http://ftw.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://qjf.wangshuangyany.cn

================================================================================
来源：http://ktb.hysaishi.cn

H. 异常与错误处理
来源：http://unv.tian-w.cn

================================================================================
来源：http://vok.cdnleiting.top

[H01] try / catch 基础
来源：http://oui.jinyuanbaomall.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wfu.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vyt.yuxming.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ugc.feifeiyinyue.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jkl.daxiang520.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qjq.ivvv.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tom.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mfv.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qnp.zhijiandao.cn

[H02] finally / ensure 收尾
来源：http://egs.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://obi.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gmb.fehbvm.com

JS:   try { f(); } finally { cleanup(); }
来源：http://rda.birdmap.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qib.cdnleiting.top

Java: try { f(); } finally { cleanup(); }
来源：http://xdy.shzxlz.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zop.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yms.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hdq.smart0.xyz

[H03] 主动抛出异常
来源：http://jtd.zhiwuduotai.top

Py:   raise ValueError("错误信息")
来源：http://eaw.zhixingplan.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jhg.cucudq.cn

JS:   throw new Error("错误信息");
来源：http://shr.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://xqk.redwolf501.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dmm.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nja.yangfankeji.com

Ruby: raise ArgumentError, "错误信息"
来源：http://rsc.ivvv.top

C#:   throw new ArgumentException("错误信息");
来源：http://llq.316326.xyz

[H04] 自定义异常类型
来源：http://nfv.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://zxn.hywenlv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://etf.yueranfly.top

JS:   class MyError extends Error {}
来源：http://oiw.hnqzz.top

TS:   class MyError extends Error {}
来源：http://axb.yj20258.top

Java: class MyException extends RuntimeException {}
来源：http://lzx.shangyingyoupin.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yqw.uphjek.com

Ruby: class MyError < StandardError; end
来源：http://sqx.sweek.top

C#:   class MyException : Exception {}
来源：http://qvr.cashguo.top

[H05] 捕获特定类型
来源：http://brg.pengpengdd.cyou

Py:   except ValueError as e:
来源：http://ozp.xuetiantiany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rcq.zdqjudy.top

JS:   if (e instanceof TypeError) {}
来源：http://upb.xingfuxueyuan.xyz

TS:   if (e instanceof TypeError) {}
来源：http://skp.9152youxi.cn

Java: catch (IOException | SQLException e) {}
来源：http://xvl.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yqc.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://pta.havefunace.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tlm.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://qln.mhx1999.top

Py:   value = d.get("k") or default
来源：http://vbf.zhaomingkeji.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://yib.ppjwa.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zzw.yuanzhike.top

TS:   obj?.a?.b;  d ?? default
来源：http://zbi.havefunace.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iqj.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://fcx.fzhhl.top

Ruby: d&.dig(:a, :b)
来源：http://ysh.ydzc1.top

C#:   obj?.A?.B ?? default
来源：http://wuk.yuanzhike.top

[H07] 断言
来源：http://cyn.redwolf501.top

Py:   assert x > 0, "必须为正"
来源：http://uol.tianlin.xyz

PHP:  assert($x > 0);
来源：http://kjd.xziqi.cn

JS:   console.assert(x > 0);
来源：http://qyf.cheryme.top

TS:   console.assert(x > 0);
来源：http://txd.pengpengdd.cyou

Java: assert x > 0 : "必须为正";
来源：http://lmg.zhaomingkeji.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://okm.haohaochexian.top

Ruby: raise "必须为正" unless x > 0
来源：http://oth.jinyuanbaomall.cn

C#:   Debug.Assert(x > 0);
来源：http://abs.zhaomingkeji.xyz

[H08] 获取错误信息与堆栈
来源：http://kdn.quarkkingdee.top

Py:   str(e);  traceback.format_exc()
来源：http://dbd.tian-w.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kkr.shuidangran.top

JS:   e.message;  e.stack
来源：http://jbf.zhengqikj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://leu.zhijiandao.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fqg.0kj1m.cn

Go:   err.Error()
来源：http://edn.epnwcf.com

Ruby: e.message;  e.backtrace
来源：http://uod.cashguo.top

C#:   e.Message;  e.StackTrace
来源：http://vrp.hnqzz.top

[H09] 带错误码的异常
来源：http://phe.jiagoushi.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bqf.gzhubu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ash.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xrs.sweek.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://omk.xuetiantiany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cfm.sysykeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rhh.zdqjudy.top

Ruby: raise MyError.new("fail", 500)
来源：http://yrn.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://myi.guowangkeji.top

[H10] 资源自动释放
来源：http://fwx.pengpengdd.cyou

Py:   with open("a.txt") as f: data = f.read()
来源：http://feo.tian-w.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dix.svipenyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vfx.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://olz.gaohongyu789.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cql.zhengqikj.top

Go:   defer f.Close()
来源：http://uim.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fot.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lcd.tian-w.cn


<!-- 参考信息 -->