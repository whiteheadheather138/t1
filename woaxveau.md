代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://fft.jinqigfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jcg.jinqigfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kia.yongpay.top

Ruby: File.exist?("a.txt")
来源：http://zat.yj20258888.top

C#:   File.Exists("a.txt")
来源：http://xvk.xziqi.cn

[F06] 删除文件
来源：http://awj.52xcode.cn

Py:   os.remove("a.txt")
来源：http://kvm.haohaochexian.top

PHP:  unlink("a.txt");
来源：http://pqc.316326.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://zwi.yuanzhike.top

TS:   fs.unlinkSync("a.txt")
来源：http://bzv.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bnj.guowangkeji.top

Go:   os.Remove("a.txt")
来源：http://rek.bjfxy.top

Ruby: File.delete("a.txt")
来源：http://sdf.fanxiaobao.xyz

C#:   File.Delete("a.txt");
来源：http://jdz.jianghu66.top

[F07] 创建目录（含多级）
来源：http://qet.fzhhl.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://voj.meibo888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://egq.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://laj.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qck.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tuq.cucudq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fip.zhijiandao.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lhs.jqgufenzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jbz.hywenlv.cn

[F08] 遍历目录
来源：http://wnh.jlsjyb.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lqi.yuanzhike.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yzs.yueranfly.top

JS:   fs.readdirSync("dir")
来源：http://jab.aizwys.cn

TS:   fs.readdirSync("dir")
来源：http://cea.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oks.yvedp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://phk.yuanzhike.top

Ruby: Dir.children("dir")
来源：http://ipz.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://amg.cqqwz.cn

[F09] 获取文件大小
来源：http://ygg.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://tih.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://uny.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://cpr.9152youxi.cn

TS:   fs.statSync("a.txt").size
来源：http://nol.hcnkem.com

Java: Files.size(Path.of("a.txt"))
来源：http://jgh.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tlu.yuanzhike.top

Ruby: File.size("a.txt")
来源：http://imd.ydjk.org.cn

C#:   new FileInfo("a.txt").Length
来源：http://ink.jyoumei.cn

[F10] 取文件扩展名 / 文件名
来源：http://bai.guannengcc.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://khh.fehbvm.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zbu.vqdsnc.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pbn.yuxming.cn

TS:   path.extname("a.txt")
来源：http://fxj.jqgfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://niy.jyoumei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iih.zhixingplan.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ktp.yuanzhike.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://beo.hnxiangtu.top

[F11] 复制与移动文件
来源：http://fta.jinqigfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ykc.aizwys.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hbo.gaohongyu789.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dpr.ywan-chungtsiang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rla.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dit.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qdq.chenlongwang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sdj.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ruz.9152youxi.cn

[F12] CSV 读写
来源：http://qmj.sjlbkw.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zew.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://als.nanxuanxn.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://avt.zhixingplan.top

TS:   // 同上
来源：http://nbq.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qnx.xingfuxueyuan.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fjh.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ssl.daxiang520.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nuj.hesvh.cn

================================================================================
来源：http://skq.snrcjt.cn

G. 面向对象
来源：http://zws.gogol.net.cn

================================================================================
来源：http://yrc.tianlin.xyz

[G01] 定义类
来源：http://bdf.tian-w.cn

Py:   class User: pass
来源：http://czl.shanyushiyangtech.top

PHP:  class User {}
来源：http://cxw.quarkkingdee.top

JS:   class User {}
来源：http://kkv.ybcxt.top

TS:   class User { name: string = ""; }
来源：http://rzr.zdqjudy.top

Java: class User {}
来源：http://ick.cucudq.cn

Go:   type User struct { Name string }
来源：http://apo.yvedp.cn

Ruby: class User; end
来源：http://qbg.ybcxt.top

C#:   class User {}
来源：http://otx.tanke756.top

[G02] 构造函数
来源：http://mlz.ydzc1.top

Py:   def __init__(self, name): self.name = name
来源：http://vrh.0kj1m.cn

PHP:  public function __construct(public string $name) {}
来源：http://zeg.ivvv.top

JS:   constructor(name) { this.name = name; }
来源：http://kxe.snrcjt.cn

TS:   constructor(public name: string) {}
来源：http://urf.xinyue.icu

Java: User(String name) { this.name = name; }
来源：http://zez.quarkkingdee.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cyd.uphjek.com

Ruby: def initialize(name); @name = name; end
来源：http://kpn.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://pif.9152youxi.cn

[G03] 实例属性
来源：http://hsb.jinqigfzy.top

Py:   self.name = "x"
来源：http://xpf.sjlbkw.cn

PHP:  public string $name = "x";
来源：http://ory.52xcode.cn

JS:   this.name = "x";
来源：http://agh.gzhubu.top

TS:   name: string = "x";
来源：http://bgm.hysaishi.cn

Java: private String name;
来源：http://fja.jinyuanbaomall.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xfp.chenlongwang.top

Ruby: @name = "x"
来源：http://ksn.shzxlz.cn

C#:   public string Name { get; set; } = "x";
来源：http://nbu.gzhubu.top

[G04] 定义方法
来源：http://vbs.haohaochexian.top

Py:   def greet(self): return self.name
来源：http://mse.xuetiantiany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ntc.snrcjt.cn

JS:   greet() { return this.name; }
来源：http://sal.sxryk.cn

TS:   greet(): string { return this.name; }
来源：http://rvq.sjlbkw.cn

Java: String greet() { return name; }
来源：http://dwi.xuetiantiany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gdw.tianlin.xyz

Ruby: def greet; @name; end
来源：http://kty.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://snz.bbcook.cn

[G05] 继承
来源：http://sxt.hywenlv.cn

Py:   class Admin(User): pass
来源：http://ncc.shuidangran.top

PHP:  class Admin extends User {}
来源：http://emx.yueranfly.top

JS:   class Admin extends User {}
来源：http://mnj.guowangkeji.top

TS:   class Admin extends User {}
来源：http://poh.ctjpmb.com

Java: class Admin extends User {}
来源：http://uhd.hammf.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://swi.yongpay.top

Ruby: class Admin < User; end
来源：http://ttk.xingfuxueyuan.xyz

C#:   class Admin : User {}
来源：http://suo.meibo888.top

[G06] 重写方法
来源：http://ssw.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://fiw.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rgn.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://jbj.tarul.cn

TS:   greet(): string { return "admin"; }
来源：http://ltv.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://kte.iojbl.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cfo.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://nuj.52xcode.cn

C#:   public override string Greet() => "admin";
来源：http://ixw.xinyue.icu

[G07] 调用父类方法
来源：http://ytl.cucudq.cn

Py:   super().greet()
来源：http://jxg.9152youxi.cn

PHP:  parent::greet();
来源：http://ivx.yonumen.top

JS:   super.greet();
来源：http://tns.hongshengwenyu.top

TS:   super.greet();
来源：http://phq.c1oappe.top

Java: super.greet();
来源：http://wte.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://apb.52xcode.cn

Ruby: super
来源：http://hss.guannengcc.top

C#:   base.Greet();
来源：http://ilj.andypj.xyz

[G08] 静态方法与属性
来源：http://sme.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zdn.jiagoushi.top

PHP:  public static function f() {}
来源：http://nvy.yangfankeji.com

JS:   static f() {}
来源：http://jmr.fzhhl.top

TS:   static f(): void {}
来源：http://qqz.gotoacloud.top

Java: static void f() {}
来源：http://vgq.vehdjk.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://owz.jinqigufen.top

Ruby: def self.f; end
来源：http://fkv.dashuyun.cn

C#:   public static void F() {}
来源：http://oxa.sjlbkw.cn

[G09] 接口 / 抽象类
来源：http://cui.yj202588.top

Py:   from abc import ABC, abstractmethod
来源：http://hyg.tianlin.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://gvq.9152youxi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://aen.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://jok.ybcxt.top

Java: interface Shape { double area(); }
来源：http://xxm.ivvv.top

Go:   type Shape interface { Area() float64 }
来源：http://tty.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pea.ctjpmb.com

C#:   interface IShape { double Area(); }
来源：http://uqd.316326.xyz

[G10] 访问控制
来源：http://vqb.yuanzhike.top

Py:   约定 _protected / __private（不强制）
来源：http://pve.yj202588.top

PHP:  public / protected / private
来源：http://hhp.xylfe.cn

JS:   #private 字段；其余公开
来源：http://ijm.birdmap.top

TS:   public / protected / private
来源：http://auc.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://pnk.cdnleiting.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mac.quarkkingdee.top

Ruby: public / protected / private
来源：http://stp.shuidangran.top

C#:   public / protected / private / internal
来源：http://nwh.ppjwa.cn

[G11] getter / setter
来源：http://gat.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://xcp.tanke756.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cxv.nanxuanxn.top

JS:   get name() { return this._name; }
来源：http://aeq.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://efq.jlsjyb.cn

Java: public String getName() { return name; }
来源：http://pbc.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jjg.yj20258.top

Ruby: attr_accessor :name
来源：http://vwh.chenlongwang.top

C#:   public string Name { get; set; }
来源：http://osm.yj202588.top

[G12] 对象转字符串
来源：http://dxk.nanxuanxn.top

Py:   def __str__(self): return self.name
来源：http://vxp.aibaodan.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xnh.gotoacloud.top

JS:   toString() { return this.name; }
来源：http://yhq.aizwys.cn

TS:   toString(): string { return this.name; }
来源：http://zsc.dianchejie.cn

Java: @Override public String toString() { return name; }
来源：http://pwm.xuanzx.com

Go:   func (u User) String() string { return u.Name }
来源：http://fqr.bbcook.cn

Ruby: def to_s; @name; end
来源：http://zzi.havefunace.top

C#:   public override string ToString() => Name;
来源：http://bxc.hammf.cn

[G13] 判断对象类型
来源：http://yto.zhengqikj.top

Py:   isinstance(u, User)
来源：http://icx.hysaishi.cn

PHP:  $u instanceof User
来源：http://gin.andypj.xyz

JS:   u instanceof User
来源：http://niy.aibaodan.cn

TS:   u instanceof User
来源：http://gke.birdmap.top

Java: u instanceof User
来源：http://ncv.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xxq.fehbvm.com

Ruby: u.is_a?(User)
来源：http://tql.jqgufenzy.top

C#:   u is User
来源：http://nmv.xuetiantiany.cn

[G14] 数据类 / record
来源：http://vua.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vol.sjlbkw.cn

PHP:  // 用 readonly 属性模拟
来源：http://hty.shuidangran.top

JS:   // 无内置：普通类或对象字面量
来源：http://gix.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://qqz.ydzc1.top

Java: record User(String name, int age) {}
来源：http://acf.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://nvr.mhx1999.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kcn.jinyuanbaomall.cn

C#:   record User(string Name, int Age);
来源：http://gut.hywenlv.cn

[G15] 枚举
来源：http://qxd.fzhhl.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vet.sjlbkw.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hin.sjlbkw.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jrx.meibo888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yuq.andypj.xyz

Java: enum Color { RED, GREEN }
来源：http://rkp.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ral.bjfxy.top

Ruby: Color = %i[red green].freeze
来源：http://mmv.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dxg.havefunace.top

[G16] 对象转数组 / 字典
来源：http://ref.jlsjyb.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hiz.meibo888.top

PHP:  get_object_vars($obj);
来源：http://wmz.kuanghao11.cn

JS:   Object.entries(obj)
来源：http://oux.yj202588.top

TS:   Object.entries(obj)
来源：http://mhj.vehdjk.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qgw.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://chh.aibaodan.cn

Ruby: obj.instance_variables
来源：http://tlx.xinyue.icu

C#:   // 用反射或 System.Text.Json
来源：http://yiz.yuxming.cn

================================================================================
来源：http://gqd.xuetiantiany.cn

H. 异常与错误处理
来源：http://vcm.sxryk.cn

================================================================================
来源：http://gno.gogol.net.cn

[H01] try / catch 基础
来源：http://swp.guannengcc.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fzu.jianghu66.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hvp.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zpi.9152youxi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ayb.ivvv.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gmt.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pjy.yfazqb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jrc.cqqwz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kvr.yonumen.top

[H02] finally / ensure 收尾
来源：http://lho.jinyuanbaomall.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nye.zdbjq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hdp.shanyushiyangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://afw.jqgufenzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xox.c1oappe.top

Java: try { f(); } finally { cleanup(); }
来源：http://hlg.gogol.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dos.zhiwuduotai.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lex.yj20258.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://moz.haohaochexian.top

[H03] 主动抛出异常
来源：http://kzr.zhoulong.xyz

Py:   raise ValueError("错误信息")
来源：http://arl.jinyuanbaomall.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xrl.cucudq.cn

JS:   throw new Error("错误信息");
来源：http://jhe.haohaochexian.top

TS:   throw new Error("错误信息");
来源：http://iog.yj20258.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vil.yj20258888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xoz.yuanzhike.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dcj.jinghuilouyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hdi.yj20258888.top

[H04] 自定义异常类型
来源：http://mvf.0kj1m.cn

Py:   class MyError(Exception): pass
来源：http://pbu.fktsv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cqd.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://vnn.svipenyu.cn

TS:   class MyError extends Error {}
来源：http://lbm.quarkkingdee.top

Java: class MyException extends RuntimeException {}
来源：http://tji.jinyuanbaomall.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kup.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://rbs.yonumen.top

C#:   class MyException : Exception {}
来源：http://tjd.fktsv.cn

[H05] 捕获特定类型
来源：http://gtq.yfazqb.com

Py:   except ValueError as e:
来源：http://het.aibaodan.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yhk.chenzaomai.com

JS:   if (e instanceof TypeError) {}
来源：http://pti.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://bsr.shzxlz.cn

Java: catch (IOException | SQLException e) {}
来源：http://nvb.ydjk.org.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gcc.sjlbkw.cn

Ruby: rescue ArgumentError => e
来源：http://cgl.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rid.nwbrower.top

[H06] 可选值 / 空值安全访问
来源：http://cou.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://vns.sysykeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://ibp.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bcz.jianghu66.top

TS:   obj?.a?.b;  d ?? default
来源：http://rkp.gaohongyu789.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wdj.daria6918.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://svh.ctjpmb.com

Ruby: d&.dig(:a, :b)
来源：http://uff.meibo888.top

C#:   obj?.A?.B ?? default
来源：http://joo.jyoumei.cn

[H07] 断言
来源：http://jht.9152youxi.cn

Py:   assert x > 0, "必须为正"
来源：http://ofw.yueranfly.top

PHP:  assert($x > 0);
来源：http://wje.havefunace.top

JS:   console.assert(x > 0);
来源：http://jwk.jianghu66.top

TS:   console.assert(x > 0);
来源：http://yhf.shangyingyoupin.top

Java: assert x > 0 : "必须为正";
来源：http://whj.sysykeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://djn.jinyuanbaomall.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pxg.tanke756.top

C#:   Debug.Assert(x > 0);
来源：http://uks.9152youxi.cn

[H08] 获取错误信息与堆栈
来源：http://nzg.shanyushiyangtech.top

Py:   str(e);  traceback.format_exc()
来源：http://bpp.vqdsnc.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jsy.cheryme.top

JS:   e.message;  e.stack
来源：http://jwo.bjfxy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ypv.wangshuangyany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mqp.quarkkingdee.top

Go:   err.Error()
来源：http://lez.zhengqikj.top

Ruby: e.message;  e.backtrace
来源：http://crg.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://maj.jinqigfzy.top

[H09] 带错误码的异常
来源：http://cjh.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zpc.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://eym.chenzaomai.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yxu.haohaochexian.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kvv.hcnkem.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lds.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://knf.hysaishi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bzc.jiagoushi.top

C#:   // 自定义异常类中加 Code 属性
来源：http://aeb.ydjk.org.cn

[H10] 资源自动释放
来源：http://hfk.hongshengwenyu.top


<!-- 参考信息 -->