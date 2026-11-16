代发 wailian999

C#:   File.Exists("a.txt")
来源：http://mym.cashguo.top

[F06] 删除文件
来源：http://rdp.chenzaomai.com

Py:   os.remove("a.txt")
来源：http://mfj.sweek.top

PHP:  unlink("a.txt");
来源：http://vfc.dianchejie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ltx.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://yzp.hesvh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aic.fzhhl.top

Go:   os.Remove("a.txt")
来源：http://tdi.cucudq.cn

Ruby: File.delete("a.txt")
来源：http://qoa.sufxvd.cn

C#:   File.Delete("a.txt");
来源：http://xrs.yj20258.top

[F07] 创建目录（含多级）
来源：http://fip.jiagoushi.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lkc.jqgfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iyf.bjfxy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://equ.shzxlz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fhz.tianlin.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ptv.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rne.ybcxt.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gpz.hysaishi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mhc.hnxiangtu.top

[F08] 遍历目录
来源：http://vfs.gotoacloud.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vfs.jinyuanbaomall.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ptl.gogol.net.cn

JS:   fs.readdirSync("dir")
来源：http://eyi.svipenyu.cn

TS:   fs.readdirSync("dir")
来源：http://fds.hysaishi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tgi.aizwys.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gea.316326.xyz

Ruby: Dir.children("dir")
来源：http://nrd.epnwcf.com

C#:   Directory.GetFiles("dir")
来源：http://exs.yanxiufei.cn

[F09] 获取文件大小
来源：http://unh.pycfn.com

Py:   os.path.getsize("a.txt")
来源：http://hqk.hongshengwenyu.top

PHP:  filesize("a.txt");
来源：http://dty.fanxiaobao.xyz

JS:   fs.statSync("a.txt").size
来源：http://glt.sysykeji.top

TS:   fs.statSync("a.txt").size
来源：http://dck.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://agv.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xdv.wangdashe.top

Ruby: File.size("a.txt")
来源：http://ktp.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://ibb.sysykeji.top

[F10] 取文件扩展名 / 文件名
来源：http://dau.yj20258.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ohq.chenlongwang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uxh.hnxiangtu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dbw.tianlin.xyz

TS:   path.extname("a.txt")
来源：http://iss.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kgp.yongpay.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wwh.ydzc1.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wjr.birdmap.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sgt.yj20258.top

[F11] 复制与移动文件
来源：http://drx.jianghu66.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sbd.gaohongyu789.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dwi.hysaishi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vjs.gzhubu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uoz.zhongyouzk.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mmx.yueranfly.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mzm.tian-w.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hwt.jianghu66.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nkp.gotoacloud.top

[F12] CSV 读写
来源：http://kmj.daxiang520.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ttc.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mrc.meibo888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ykw.xinyue.icu

TS:   // 同上
来源：http://zuu.yuxming.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hmt.sweek.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rxy.vehdjk.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mfy.shanyushiyangtech.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lxh.cqqwz.cn

================================================================================
来源：http://qge.pycfn.com

G. 面向对象
来源：http://qer.cqqwz.cn

================================================================================
来源：http://atd.c1oappe.top

[G01] 定义类
来源：http://qfo.vqdsnc.cn

Py:   class User: pass
来源：http://fqm.xylfe.cn

PHP:  class User {}
来源：http://xyo.yanxiufei.cn

JS:   class User {}
来源：http://dnb.chenjidiqi.icu

TS:   class User { name: string = ""; }
来源：http://muo.xylfe.cn

Java: class User {}
来源：http://nrw.zhixingplan.top

Go:   type User struct { Name string }
来源：http://qxl.shzxlz.cn

Ruby: class User; end
来源：http://cht.gaohongyu789.top

C#:   class User {}
来源：http://niy.wangdashe.top

[G02] 构造函数
来源：http://yhr.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://koz.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://ukg.hongshengwenyu.top

JS:   constructor(name) { this.name = name; }
来源：http://deq.yfazqb.com

TS:   constructor(public name: string) {}
来源：http://cnp.pycfn.com

Java: User(String name) { this.name = name; }
来源：http://qmo.sweek.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kft.c1oappe.top

Ruby: def initialize(name); @name = name; end
来源：http://ocw.nwbrower.top

C#:   public User(string name) { Name = name; }
来源：http://gis.316326.xyz

[G03] 实例属性
来源：http://jcf.ctjpmb.com

Py:   self.name = "x"
来源：http://jvq.gotoacloud.top

PHP:  public string $name = "x";
来源：http://grv.dianchejie.cn

JS:   this.name = "x";
来源：http://ldn.zhixingplan.top

TS:   name: string = "x";
来源：http://sgt.epnwcf.com

Java: private String name;
来源：http://vur.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mdv.zhiwuduotai.top

Ruby: @name = "x"
来源：http://zea.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://pea.xingfuxueyuan.xyz

[G04] 定义方法
来源：http://omy.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://zvf.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nbn.aizwys.cn

JS:   greet() { return this.name; }
来源：http://tng.dianchejie.cn

TS:   greet(): string { return this.name; }
来源：http://sfa.ydjk.org.cn

Java: String greet() { return name; }
来源：http://qrz.sxryk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gkm.shanyushiyangkeji.top

Ruby: def greet; @name; end
来源：http://zsx.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://vpu.tian-w.cn

[G05] 继承
来源：http://taa.feifeiyinyue.top

Py:   class Admin(User): pass
来源：http://gvj.dianchejie.cn

PHP:  class Admin extends User {}
来源：http://ica.cqqwz.cn

JS:   class Admin extends User {}
来源：http://gev.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://fvl.yuanzhike.top

Java: class Admin extends User {}
来源：http://doz.yj20258888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ypl.yueranfly.top

Ruby: class Admin < User; end
来源：http://lzm.hcnkem.com

C#:   class Admin : User {}
来源：http://flg.zdqjudy.top

[G06] 重写方法
来源：http://kel.hongshengwenyu.top

Py:   def greet(self): return "admin"
来源：http://dkb.hysaishi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gkr.zhijiandao.cn

JS:   greet() { return "admin"; }
来源：http://cyv.nwbrower.top

TS:   greet(): string { return "admin"; }
来源：http://yct.jqgfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://nrk.aibaodan.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://efl.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://uhy.hammf.cn

C#:   public override string Greet() => "admin";
来源：http://bjm.jinghuilouyu.cn

[G07] 调用父类方法
来源：http://fnr.haohaochexian.top

Py:   super().greet()
来源：http://kge.wangshuangyany.cn

PHP:  parent::greet();
来源：http://mmd.shanyushiyangtech.top

JS:   super.greet();
来源：http://ndt.yj202588.top

TS:   super.greet();
来源：http://ttx.shanyushiyangkeji.top

Java: super.greet();
来源：http://xlb.shanyushiyangtech.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zjl.yanxiufei.cn

Ruby: super
来源：http://rzz.wangshuangyany.cn

C#:   base.Greet();
来源：http://kfb.meibo888.top

[G08] 静态方法与属性
来源：http://jbb.andypj.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ucv.jinqigfzy.top

PHP:  public static function f() {}
来源：http://ndr.0kj1m.cn

JS:   static f() {}
来源：http://gqs.yfazqb.com

TS:   static f(): void {}
来源：http://rkn.andypj.xyz

Java: static void f() {}
来源：http://daz.tarul.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ubo.quarkkingdee.top

Ruby: def self.f; end
来源：http://zsx.jinqigufen.top

C#:   public static void F() {}
来源：http://ijo.daxiang520.top

[G09] 接口 / 抽象类
来源：http://wsi.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://tci.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://snk.vqdsnc.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gva.daria6918.cn

TS:   interface Shape { area(): number; }
来源：http://zan.yj20258888.top

Java: interface Shape { double area(); }
来源：http://hru.hysaishi.cn

Go:   type Shape interface { Area() float64 }
来源：http://hoa.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iqf.yj20258888.top

C#:   interface IShape { double Area(); }
来源：http://frj.shanyushiyangtech.top

[G10] 访问控制
来源：http://uxd.zdqjudy.top

Py:   约定 _protected / __private（不强制）
来源：http://eua.tianlin.xyz

PHP:  public / protected / private
来源：http://jbh.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://ses.aizwys.cn

TS:   public / protected / private
来源：http://dlz.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://xeq.daxiang520.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://izr.pengpengdd.cyou

Ruby: public / protected / private
来源：http://xea.chenjidiqi.icu

C#:   public / protected / private / internal
来源：http://soi.nanxuanxn.top

[G11] getter / setter
来源：http://mtn.jqgfzy.top

Py:   @property 与 @x.setter
来源：http://tbp.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://khk.hongshengwenyu.top

JS:   get name() { return this._name; }
来源：http://bpp.zycfv.cn

TS:   get name(): string { return this._name; }
来源：http://qgk.aibaodan.cn

Java: public String getName() { return name; }
来源：http://xcq.hysaishi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tfo.ydjk.org.cn

Ruby: attr_accessor :name
来源：http://xtd.vehdjk.com

C#:   public string Name { get; set; }
来源：http://uas.tanke756.top

[G12] 对象转字符串
来源：http://npm.jinqigufen.top

Py:   def __str__(self): return self.name
来源：http://zep.0kj1m.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cru.shanyushiyangtech.top

JS:   toString() { return this.name; }
来源：http://ifb.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://kmf.ywan-chungtsiang.top

Java: @Override public String toString() { return name; }
来源：http://cmy.snrcjt.cn

Go:   func (u User) String() string { return u.Name }
来源：http://glk.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://ngj.52xcode.cn

C#:   public override string ToString() => Name;
来源：http://mrw.vqdsnc.cn

[G13] 判断对象类型
来源：http://odb.fengsongda.top

Py:   isinstance(u, User)
来源：http://jat.uphjek.com

PHP:  $u instanceof User
来源：http://fho.gogol.net.cn

JS:   u instanceof User
来源：http://knl.hammf.cn

TS:   u instanceof User
来源：http://rws.fzhhl.top

Java: u instanceof User
来源：http://fjg.iojbl.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wgy.cdnleiting.top

Ruby: u.is_a?(User)
来源：http://owt.dianchejie.cn

C#:   u is User
来源：http://ryq.wangdashe.top

[G14] 数据类 / record
来源：http://wio.nanxinkj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zkw.chenlongwang.top

PHP:  // 用 readonly 属性模拟
来源：http://oux.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://xaq.chenjidiqi.icu

TS:   type User = { name: string; age: number };
来源：http://pzt.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://zoy.ywan-chungtsiang.top

Go:   type User struct { Name string; Age int }
来源：http://kxq.xuetiantiany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eig.jiagoushi.top

C#:   record User(string Name, int Age);
来源：http://pzw.gaohongyu789.top

[G15] 枚举
来源：http://dwx.shzxlz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wmd.zhiwuduotai.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gyl.shuidangran.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xri.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://frt.svipenyu.cn

Java: enum Color { RED, GREEN }
来源：http://ekm.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aau.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://gej.havefunace.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cag.gogol.net.cn

[G16] 对象转数组 / 字典
来源：http://sep.fzhhl.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aih.gotoacloud.top

PHP:  get_object_vars($obj);
来源：http://tap.sysykeji.top

JS:   Object.entries(obj)
来源：http://tmm.cdnleiting.top

TS:   Object.entries(obj)
来源：http://kio.jqgufenzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pim.316326.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://wkd.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://cbw.52xcode.cn

C#:   // 用反射或 System.Text.Json
来源：http://kly.svipenyu.cn

================================================================================
来源：http://kbi.tianlin.xyz

H. 异常与错误处理
来源：http://odo.mhx1999.top

================================================================================
来源：http://qup.smart0.xyz

[H01] try / catch 基础
来源：http://vyb.jlsjyb.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oil.zhijiandao.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ajf.yongpay.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wco.jinghuilouyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://szj.yonumen.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aux.zdqjudy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://egw.jinghuilouyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jmk.52xcode.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xtd.dashuyun.cn

[H02] finally / ensure 收尾
来源：http://gvc.hongshengwenyu.top

Py:   try: f()⏎finally: cleanup()
来源：http://fzn.sxryk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jas.ybcxt.top

JS:   try { f(); } finally { cleanup(); }
来源：http://lbd.chenlongwang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://sbh.jyoumei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fcj.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://klq.hcnkem.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ckg.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://akk.yongpay.top

[H03] 主动抛出异常
来源：http://bqc.aibaodan.cn

Py:   raise ValueError("错误信息")
来源：http://yzb.haohaochexian.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://img.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://kfd.shanyushiyangkeji.top

TS:   throw new Error("错误信息");
来源：http://rbx.yangfankeji.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://grb.ppjwa.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ppl.nwbrower.top

Ruby: raise ArgumentError, "错误信息"
来源：http://smu.yangfankeji.com

C#:   throw new ArgumentException("错误信息");
来源：http://str.cucudq.cn

[H04] 自定义异常类型
来源：http://ilc.tian-w.cn

Py:   class MyError(Exception): pass
来源：http://bbq.redwolf501.top

PHP:  class MyError extends RuntimeException {}
来源：http://qrk.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://diz.smart0.xyz

TS:   class MyError extends Error {}
来源：http://mem.hammf.cn

Java: class MyException extends RuntimeException {}
来源：http://jjy.zycfv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uba.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://dfx.shangyingyoupin.top

C#:   class MyException : Exception {}
来源：http://ouq.xinyue.icu

[H05] 捕获特定类型
来源：http://vbc.xuetiantiany.cn

Py:   except ValueError as e:
来源：http://eur.feifeiyinyue.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dpe.fehbvm.com

JS:   if (e instanceof TypeError) {}
来源：http://ffj.yuxming.cn

TS:   if (e instanceof TypeError) {}
来源：http://acm.cdnleiting.top

Java: catch (IOException | SQLException e) {}
来源：http://wjw.birdmap.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ykp.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://qaz.9152youxi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mdy.quarkkingdee.top

[H06] 可选值 / 空值安全访问
来源：http://qax.zhengqikj.top

Py:   value = d.get("k") or default
来源：http://ksn.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zqb.smart0.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://tva.jyoumei.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zww.ywan-chungtsiang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zfl.chenjidiqi.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://zfs.hysaishi.cn

Ruby: d&.dig(:a, :b)
来源：http://uab.hnxiangtu.top

C#:   obj?.A?.B ?? default
来源：http://tru.redwolf501.top

[H07] 断言
来源：http://oks.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://ttu.guannengcc.top

PHP:  assert($x > 0);
来源：http://iik.daria6918.cn

JS:   console.assert(x > 0);
来源：http://spc.chenjidiqi.icu

TS:   console.assert(x > 0);
来源：http://aca.hcnkem.com

Java: assert x > 0 : "必须为正";
来源：http://ncn.daria6918.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hzz.zhijiandao.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hfm.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://kfw.shanyushiyangkeji.top

[H08] 获取错误信息与堆栈
来源：http://ocq.aibaodan.cn

Py:   str(e);  traceback.format_exc()
来源：http://vxp.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nza.nwbrower.top

JS:   e.message;  e.stack
来源：http://ssd.fehbvm.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://itv.zhijiandao.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sbg.zdbjq.cn

Go:   err.Error()
来源：http://qcj.havefunace.top

Ruby: e.message;  e.backtrace
来源：http://koh.birdmap.top

C#:   e.Message;  e.StackTrace
来源：http://yzi.hammf.cn

[H09] 带错误码的异常
来源：http://ssc.zdbjq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hcw.ivvv.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dvy.hongshengwenyu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jva.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mww.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wnu.shuidangran.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ndh.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://boz.zhengqikj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pkv.jqgfzy.top

[H10] 资源自动释放
来源：http://qfs.redwolf501.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ebr.havefunace.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jvm.zhengqikj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lhq.hywenlv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pgm.yj202588.top


<!-- 参考信息 -->