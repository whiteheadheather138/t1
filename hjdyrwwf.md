代发 wailian999

Ruby: File.delete("a.txt")
来源：http://kgq.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://pch.cashguo.top

[F07] 创建目录（含多级）
来源：http://lev.zdqjudy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fza.birdmap.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fyc.fanxiaobao.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://doy.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ohx.guowangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lkk.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lam.chenjidiqi.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://znm.zhijiandao.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vaq.sweek.top

[F08] 遍历目录
来源：http://avd.yuxming.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vml.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://awy.yuxming.cn

JS:   fs.readdirSync("dir")
来源：http://xyz.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://cxr.zhaomingkeji.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xck.epnwcf.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://igb.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://fki.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://szn.316326.xyz

[F09] 获取文件大小
来源：http://vgl.shanyushiyangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://zaq.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://yod.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://ftz.sjlbkw.cn

TS:   fs.statSync("a.txt").size
来源：http://vxr.sjlbkw.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jni.ehwqpu.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://age.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://lkz.chenzaomai.com

C#:   new FileInfo("a.txt").Length
来源：http://hxj.zhixingplan.top

[F10] 取文件扩展名 / 文件名
来源：http://xmo.vehdjk.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mhe.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://thw.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tkk.andypj.xyz

TS:   path.extname("a.txt")
来源：http://sfa.sysykeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://syn.fzhhl.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xvz.xylfe.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fzx.jlsjyb.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mro.shzxlz.cn

[F11] 复制与移动文件
来源：http://pca.gzhubu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mlf.hfpthk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bru.yonumen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qms.vehdjk.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kfr.andypj.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://abz.ydzc1.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hqt.gogol.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://drh.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jtj.hywenlv.cn

[F12] CSV 读写
来源：http://zad.jianghu66.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uyz.vqdsnc.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://whv.zhiwuduotai.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wam.kuanghao11.cn

TS:   // 同上
来源：http://djc.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mkq.dashuyun.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cnj.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dbd.hesvh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://heb.nwbrower.top

================================================================================
来源：http://mbv.yfazqb.com

G. 面向对象
来源：http://tdp.daxiang520.top

================================================================================
来源：http://vzr.epnwcf.com

[G01] 定义类
来源：http://tzj.daria6918.cn

Py:   class User: pass
来源：http://xnu.c1oappe.top

PHP:  class User {}
来源：http://vuz.ehwqpu.com

JS:   class User {}
来源：http://pmt.xingfuxueyuan.xyz

TS:   class User { name: string = ""; }
来源：http://acy.bbcook.cn

Java: class User {}
来源：http://ucn.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://abr.hysaishi.cn

Ruby: class User; end
来源：http://lfd.yonumen.top

C#:   class User {}
来源：http://ooc.xingfuxueyuan.xyz

[G02] 构造函数
来源：http://oos.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://eqa.fehbvm.com

PHP:  public function __construct(public string $name) {}
来源：http://snl.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://cvb.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://ytj.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://qbx.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vup.fehbvm.com

Ruby: def initialize(name); @name = name; end
来源：http://mhx.andypj.xyz

C#:   public User(string name) { Name = name; }
来源：http://fuj.ywan-chungtsiang.top

[G03] 实例属性
来源：http://bhu.xylfe.cn

Py:   self.name = "x"
来源：http://fko.xylfe.cn

PHP:  public string $name = "x";
来源：http://guz.pengpengdd.cyou

JS:   this.name = "x";
来源：http://nfu.yj20258.top

TS:   name: string = "x";
来源：http://vzl.mhx1999.top

Java: private String name;
来源：http://qpd.hesvh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jax.hnxiangtu.top

Ruby: @name = "x"
来源：http://ude.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://uqh.zhoulong.xyz

[G04] 定义方法
来源：http://nzg.daxiang520.top

Py:   def greet(self): return self.name
来源：http://mby.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pwz.c1oappe.top

JS:   greet() { return this.name; }
来源：http://ucr.hesvh.cn

TS:   greet(): string { return this.name; }
来源：http://fub.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://afl.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hop.jinqigufen.top

Ruby: def greet; @name; end
来源：http://jfk.tanke756.top

C#:   public string Greet() => Name;
来源：http://ctp.haohaochexian.top

[G05] 继承
来源：http://hix.jinqigufen.top

Py:   class Admin(User): pass
来源：http://zol.tianlin.xyz

PHP:  class Admin extends User {}
来源：http://sby.nwbrower.top

JS:   class Admin extends User {}
来源：http://vqg.andypj.xyz

TS:   class Admin extends User {}
来源：http://pdi.jinqigufen.top

Java: class Admin extends User {}
来源：http://vvq.jianghu66.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://txm.zhaomingkeji.xyz

Ruby: class Admin < User; end
来源：http://mcx.epnwcf.com

C#:   class Admin : User {}
来源：http://txu.zhongyouzk.top

[G06] 重写方法
来源：http://xcd.52xcode.cn

Py:   def greet(self): return "admin"
来源：http://rqx.quarkkingdee.top

PHP:  public function greet(): string { return "admin"; }
来源：http://sss.yuxming.cn

JS:   greet() { return "admin"; }
来源：http://dsa.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://zlo.cqqwz.cn

Java: @Override String greet() { return "admin"; }
来源：http://qvp.chenjidiqi.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://odv.sysykeji.top

Ruby: def greet; "admin"; end
来源：http://tpc.hfpthk.cn

C#:   public override string Greet() => "admin";
来源：http://gcw.fengsongda.top

[G07] 调用父类方法
来源：http://bex.9152youxi.cn

Py:   super().greet()
来源：http://brv.haohaochexian.top

PHP:  parent::greet();
来源：http://uan.nanxinkj.top

JS:   super.greet();
来源：http://rmv.daxiang520.top

TS:   super.greet();
来源：http://upa.9152youxi.cn

Java: super.greet();
来源：http://gfc.0kj1m.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://abl.ppjwa.cn

Ruby: super
来源：http://fwh.zycfv.cn

C#:   base.Greet();
来源：http://gsw.zdqjudy.top

[G08] 静态方法与属性
来源：http://myh.pycfn.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://alk.birdmap.top

PHP:  public static function f() {}
来源：http://sje.ivvv.top

JS:   static f() {}
来源：http://seo.chenjidiqi.icu

TS:   static f(): void {}
来源：http://gjj.snrcjt.cn

Java: static void f() {}
来源：http://rja.svipenyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://frc.xuetiantiany.cn

Ruby: def self.f; end
来源：http://qlq.jinqigfzy.top

C#:   public static void F() {}
来源：http://nav.shanyushiyangtech.top

[G09] 接口 / 抽象类
来源：http://xwy.hnxiangtu.top

Py:   from abc import ABC, abstractmethod
来源：http://abi.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://unf.hywenlv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://anh.redwolf501.top

TS:   interface Shape { area(): number; }
来源：http://rct.yj20258888.top

Java: interface Shape { double area(); }
来源：http://imx.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://jdd.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rcy.hfpthk.cn

C#:   interface IShape { double Area(); }
来源：http://cry.jqgufenzy.top

[G10] 访问控制
来源：http://ixb.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://ayy.wangshuangyany.cn

PHP:  public / protected / private
来源：http://fzp.sysykeji.top

JS:   #private 字段；其余公开
来源：http://byv.zhengqikj.top

TS:   public / protected / private
来源：http://nao.gogol.net.cn

Java: public / protected / private / 默认包级
来源：http://mdh.hfpthk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jqo.tian-w.cn

Ruby: public / protected / private
来源：http://myb.sjlbkw.cn

C#:   public / protected / private / internal
来源：http://wyg.feifeiyinyue.top

[G11] getter / setter
来源：http://epo.andypj.xyz

Py:   @property 与 @x.setter
来源：http://jwm.ydzc1.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ulq.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://lfa.pycfn.com

TS:   get name(): string { return this._name; }
来源：http://dap.daxiang520.top

Java: public String getName() { return name; }
来源：http://riw.dashuyun.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://agy.52xcode.cn

Ruby: attr_accessor :name
来源：http://amt.sysykeji.top

C#:   public string Name { get; set; }
来源：http://ndm.yongpay.top

[G12] 对象转字符串
来源：http://brm.xuanzx.com

Py:   def __str__(self): return self.name
来源：http://vna.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lbg.sxryk.cn

JS:   toString() { return this.name; }
来源：http://jvo.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://nsp.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://upn.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gdd.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://bxr.yfazqb.com

C#:   public override string ToString() => Name;
来源：http://rra.pycfn.com

[G13] 判断对象类型
来源：http://gbx.xuanzx.com

Py:   isinstance(u, User)
来源：http://uwn.jinqigfzy.top

PHP:  $u instanceof User
来源：http://pgw.xuanzx.com

JS:   u instanceof User
来源：http://fpk.yvedp.cn

TS:   u instanceof User
来源：http://bup.gotoacloud.top

Java: u instanceof User
来源：http://gaa.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://abm.gogol.net.cn

Ruby: u.is_a?(User)
来源：http://iva.zhengqikj.top

C#:   u is User
来源：http://dci.pycfn.com

[G14] 数据类 / record
来源：http://cnc.gogol.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kte.bjfxy.top

PHP:  // 用 readonly 属性模拟
来源：http://dhk.vehdjk.com

JS:   // 无内置：普通类或对象字面量
来源：http://hhn.tarul.cn

TS:   type User = { name: string; age: number };
来源：http://aiy.sxryk.cn

Java: record User(String name, int age) {}
来源：http://ieu.yonumen.top

Go:   type User struct { Name string; Age int }
来源：http://lus.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xgj.daria6918.cn

C#:   record User(string Name, int Age);
来源：http://yuq.tarul.cn

[G15] 枚举
来源：http://uxl.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ypp.haohaochexian.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://art.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jab.ehwqpu.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oxp.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://qdo.guowangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sdd.52xcode.cn

Ruby: Color = %i[red green].freeze
来源：http://jlf.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wwp.daria6918.cn

[G16] 对象转数组 / 字典
来源：http://fua.nanxinkj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xbi.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://hcn.iojbl.cn

JS:   Object.entries(obj)
来源：http://gdb.pengpengdd.cyou

TS:   Object.entries(obj)
来源：http://dxc.xylfe.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dvi.dashuyun.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mot.xinyue.icu

Ruby: obj.instance_variables
来源：http://utx.tarul.cn

C#:   // 用反射或 System.Text.Json
来源：http://kbz.dianchejie.cn

================================================================================
来源：http://ztv.tian-w.cn

H. 异常与错误处理
来源：http://rmn.cucudq.cn

================================================================================
来源：http://piw.nanxuanxn.top

[H01] try / catch 基础
来源：http://aky.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kiz.fanxiaobao.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ntr.sjlbkw.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gtk.vqdsnc.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uxx.shanyushiyangtech.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zsl.zhaomingkeji.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yzf.yuanzhike.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hyj.ybcxt.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fml.tanke756.top

[H02] finally / ensure 收尾
来源：http://ata.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://qoe.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gvz.yj202588.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wex.ydzc1.top

TS:   try { f(); } finally { cleanup(); }
来源：http://uey.xinyue.icu

Java: try { f(); } finally { cleanup(); }
来源：http://ojy.feifeiyinyue.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mpz.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://doj.gotoacloud.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://myd.jlsjyb.cn

[H03] 主动抛出异常
来源：http://mcj.andypj.xyz

Py:   raise ValueError("错误信息")
来源：http://gjs.ydzc1.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vxx.jiagoushi.top

JS:   throw new Error("错误信息");
来源：http://ild.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://znd.tanke756.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gmz.yfazqb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fwc.ivvv.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ppw.wangshuangyany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jyg.fengsongda.top

[H04] 自定义异常类型
来源：http://yin.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://jrq.fengsongda.top

PHP:  class MyError extends RuntimeException {}
来源：http://eha.svipenyu.cn

JS:   class MyError extends Error {}
来源：http://wpg.316326.xyz

TS:   class MyError extends Error {}
来源：http://rgi.shanyushiyangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://exq.iojbl.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ssz.tanke756.top

Ruby: class MyError < StandardError; end
来源：http://mvq.jiagoushi.top

C#:   class MyException : Exception {}
来源：http://ypb.zhengqikj.top

[H05] 捕获特定类型
来源：http://zkg.xziqi.cn

Py:   except ValueError as e:
来源：http://rlg.yuanzhike.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ith.yvedp.cn

JS:   if (e instanceof TypeError) {}
来源：http://qhl.zhixingplan.top

TS:   if (e instanceof TypeError) {}
来源：http://diq.shanyushiyangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://yeb.zycfv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://esw.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://gyt.yvedp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pvs.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://kdz.guowangkeji.top

Py:   value = d.get("k") or default
来源：http://ref.fehbvm.com

PHP:  $v = $d["k"] ?? null;
来源：http://dcw.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://hvh.aibaodan.cn

TS:   obj?.a?.b;  d ?? default
来源：http://oxa.cdnleiting.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zzn.zhijiandao.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hnf.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://yhb.hcnkem.com

C#:   obj?.A?.B ?? default
来源：http://tov.xylfe.cn

[H07] 断言
来源：http://wlh.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://gow.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://agm.sweek.top

JS:   console.assert(x > 0);
来源：http://hba.hongshengwenyu.top

TS:   console.assert(x > 0);
来源：http://ega.ivvv.top

Java: assert x > 0 : "必须为正";
来源：http://oyw.aizwys.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nrk.xuanzx.com

Ruby: raise "必须为正" unless x > 0
来源：http://aml.gaohongyu789.top

C#:   Debug.Assert(x > 0);
来源：http://ovr.sjlbkw.cn

[H08] 获取错误信息与堆栈
来源：http://ohq.wangdashe.top

Py:   str(e);  traceback.format_exc()
来源：http://eim.smart0.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cdn.gaohongyu789.top

JS:   e.message;  e.stack
来源：http://jdp.pycfn.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://bhw.cheryme.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ygu.gaohongyu789.top

Go:   err.Error()
来源：http://uir.jianghu66.top

Ruby: e.message;  e.backtrace
来源：http://yxa.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://rdy.bjfxy.top

[H09] 带错误码的异常
来源：http://oga.yuxming.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cao.zhaomingkeji.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://mki.redwolf501.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rxh.redwolf501.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rvm.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lil.wangdashe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mtu.fanxiaobao.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://twv.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://pbi.bjfxy.top

[H10] 资源自动释放
来源：http://ras.jlsjyb.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gff.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wua.yj20258888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zbq.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hjg.9152youxi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bcs.xinyue.icu

Go:   defer f.Close()
来源：http://tic.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dvm.zhiwuduotai.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://erb.yongpay.top

================================================================================
来源：http://ayh.nanxinkj.top

I. 正则表达式
来源：http://gbj.yfazqb.com

================================================================================
来源：http://bnb.jinqigufen.top

[I01] 判断是否匹配
来源：http://pcb.chenlongwang.top


<!-- 参考信息 -->