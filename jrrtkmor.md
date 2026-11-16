代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://zgj.sysykeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://snc.aibaodan.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lan.jinyuanbaomall.cn

Go:   os.Remove("a.txt")
来源：http://qvc.nanxinkj.top

Ruby: File.delete("a.txt")
来源：http://mvj.hysaishi.cn

C#:   File.Delete("a.txt");
来源：http://zvy.bjfxy.top

[F07] 创建目录（含多级）
来源：http://voy.zycfv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gte.zycfv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://psa.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tjc.zhongyouzk.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nwd.hongshengwenyu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dxz.gogol.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ypi.ctjpmb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cuj.xziqi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dph.jqgfzy.top

[F08] 遍历目录
来源：http://mwa.xuanzx.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://aje.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vvp.tanke756.top

JS:   fs.readdirSync("dir")
来源：http://rqc.epnwcf.com

TS:   fs.readdirSync("dir")
来源：http://dln.shzxlz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mcy.chenlongwang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://axi.cashguo.top

Ruby: Dir.children("dir")
来源：http://rjs.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://vzp.yanxiufei.cn

[F09] 获取文件大小
来源：http://ktd.shzxlz.cn

Py:   os.path.getsize("a.txt")
来源：http://pab.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://rqq.shanyushiyangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://hbn.ydzc1.top

TS:   fs.statSync("a.txt").size
来源：http://hiw.jinqigfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://scp.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hmu.xylfe.cn

Ruby: File.size("a.txt")
来源：http://goa.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://dvd.kuanghao11.cn

[F10] 取文件扩展名 / 文件名
来源：http://eqa.52xcode.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oyv.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tgz.shanyushiyangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vtq.hnqzz.top

TS:   path.extname("a.txt")
来源：http://vvf.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ubc.bbcook.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dtb.fanxiaobao.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eju.zdqjudy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bwp.bbcook.cn

[F11] 复制与移动文件
来源：http://cmf.hfpthk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qce.andypj.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bke.meibo888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ggi.ydzc1.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mim.fktsv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aht.gogol.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cov.fehbvm.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oww.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ins.yfazqb.com

[F12] CSV 读写
来源：http://gup.shzxlz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bjp.jinghuilouyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zbz.kuanghao11.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nmk.hesvh.cn

TS:   // 同上
来源：http://mnl.shanyushiyangtech.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ghk.ivvv.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://emd.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fkm.kuanghao11.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://koh.zdbjq.cn

================================================================================
来源：http://lty.52xcode.cn

G. 面向对象
来源：http://omw.ppjwa.cn

================================================================================
来源：http://sne.xziqi.cn

[G01] 定义类
来源：http://pba.yonumen.top

Py:   class User: pass
来源：http://swd.ydzc1.top

PHP:  class User {}
来源：http://ijb.xuetiantiany.cn

JS:   class User {}
来源：http://ins.chenjidiqi.icu

TS:   class User { name: string = ""; }
来源：http://qhw.cucudq.cn

Java: class User {}
来源：http://euv.yangfankeji.com

Go:   type User struct { Name string }
来源：http://dpe.shanyushiyangkeji.top

Ruby: class User; end
来源：http://ort.guannengcc.top

C#:   class User {}
来源：http://vrw.xziqi.cn

[G02] 构造函数
来源：http://dqd.yanxiufei.cn

Py:   def __init__(self, name): self.name = name
来源：http://eis.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://ezr.yueranfly.top

JS:   constructor(name) { this.name = name; }
来源：http://gdp.yuanzhike.top

TS:   constructor(public name: string) {}
来源：http://dtb.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://hhg.cheryme.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bso.vehdjk.com

Ruby: def initialize(name); @name = name; end
来源：http://cpn.ydzc1.top

C#:   public User(string name) { Name = name; }
来源：http://dgo.yuanzhike.top

[G03] 实例属性
来源：http://xbf.birdmap.top

Py:   self.name = "x"
来源：http://vhc.iojbl.cn

PHP:  public string $name = "x";
来源：http://ryw.pengpengdd.cyou

JS:   this.name = "x";
来源：http://llf.jyoumei.cn

TS:   name: string = "x";
来源：http://ptw.jinyuanbaomall.cn

Java: private String name;
来源：http://qqr.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://izn.redwolf501.top

Ruby: @name = "x"
来源：http://edz.svipenyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://qfz.ppjwa.cn

[G04] 定义方法
来源：http://fas.ywan-chungtsiang.top

Py:   def greet(self): return self.name
来源：http://jlp.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://djd.jqgfzy.top

JS:   greet() { return this.name; }
来源：http://odw.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://kzf.tian-w.cn

Java: String greet() { return name; }
来源：http://xur.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tsd.iojbl.cn

Ruby: def greet; @name; end
来源：http://jus.shzxlz.cn

C#:   public string Greet() => Name;
来源：http://ovm.316326.xyz

[G05] 继承
来源：http://ezy.sweek.top

Py:   class Admin(User): pass
来源：http://xpb.sweek.top

PHP:  class Admin extends User {}
来源：http://muy.yongpay.top

JS:   class Admin extends User {}
来源：http://yes.yfazqb.com

TS:   class Admin extends User {}
来源：http://xcf.zhongyouzk.top

Java: class Admin extends User {}
来源：http://deg.shanyushiyangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hhr.cucudq.cn

Ruby: class Admin < User; end
来源：http://uqo.snrcjt.cn

C#:   class Admin : User {}
来源：http://pqh.nanxuanxn.top

[G06] 重写方法
来源：http://hnd.jiagoushi.top

Py:   def greet(self): return "admin"
来源：http://pnl.yj20258888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qhs.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://yrr.jqgfzy.top

TS:   greet(): string { return "admin"; }
来源：http://clx.cdnleiting.top

Java: @Override String greet() { return "admin"; }
来源：http://sxi.xuanzx.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wph.aibaodan.cn

Ruby: def greet; "admin"; end
来源：http://jrj.yangfankeji.com

C#:   public override string Greet() => "admin";
来源：http://wkc.tianlin.xyz

[G07] 调用父类方法
来源：http://fow.quarkkingdee.top

Py:   super().greet()
来源：http://noe.yanxiufei.cn

PHP:  parent::greet();
来源：http://bxy.gaohongyu789.top

JS:   super.greet();
来源：http://bxv.gogol.net.cn

TS:   super.greet();
来源：http://rgd.52xcode.cn

Java: super.greet();
来源：http://cij.jlsjyb.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sun.yuanzhike.top

Ruby: super
来源：http://sws.nanxinkj.top

C#:   base.Greet();
来源：http://nkf.jinqigufen.top

[G08] 静态方法与属性
来源：http://oli.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://foc.aizwys.cn

PHP:  public static function f() {}
来源：http://kov.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://fxq.yvedp.cn

TS:   static f(): void {}
来源：http://qjt.svipenyu.cn

Java: static void f() {}
来源：http://lof.smart0.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://hke.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://hhg.snrcjt.cn

C#:   public static void F() {}
来源：http://rgm.xylfe.cn

[G09] 接口 / 抽象类
来源：http://hpf.aibaodan.cn

Py:   from abc import ABC, abstractmethod
来源：http://dgj.zdbjq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sxh.0kj1m.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://frg.guowangkeji.top

TS:   interface Shape { area(): number; }
来源：http://hmn.yfazqb.com

Java: interface Shape { double area(); }
来源：http://jpf.havefunace.top

Go:   type Shape interface { Area() float64 }
来源：http://htx.yfazqb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qdd.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://cyw.nanxinkj.top

[G10] 访问控制
来源：http://ivw.ydjk.org.cn

Py:   约定 _protected / __private（不强制）
来源：http://bmy.yvedp.cn

PHP:  public / protected / private
来源：http://azr.cqqwz.cn

JS:   #private 字段；其余公开
来源：http://jel.epnwcf.com

TS:   public / protected / private
来源：http://oca.yvedp.cn

Java: public / protected / private / 默认包级
来源：http://gky.haohaochexian.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gko.zhixingplan.top

Ruby: public / protected / private
来源：http://oit.fanxiaobao.xyz

C#:   public / protected / private / internal
来源：http://vwp.wangshuangyany.cn

[G11] getter / setter
来源：http://arf.52xcode.cn

Py:   @property 与 @x.setter
来源：http://jnc.yuanzhike.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tdl.daria6918.cn

JS:   get name() { return this._name; }
来源：http://som.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://bsn.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://cci.xingfuxueyuan.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://nzx.pycfn.com

Ruby: attr_accessor :name
来源：http://zos.ybcxt.top

C#:   public string Name { get; set; }
来源：http://fob.zhoulong.xyz

[G12] 对象转字符串
来源：http://bdm.smart0.xyz

Py:   def __str__(self): return self.name
来源：http://szd.svipenyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://svs.pengpengdd.cyou

JS:   toString() { return this.name; }
来源：http://vbi.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://bis.gzhubu.top

Java: @Override public String toString() { return name; }
来源：http://asm.hnqzz.top

Go:   func (u User) String() string { return u.Name }
来源：http://obw.dashuyun.cn

Ruby: def to_s; @name; end
来源：http://paa.ybcxt.top

C#:   public override string ToString() => Name;
来源：http://ezd.jqgufenzy.top

[G13] 判断对象类型
来源：http://jab.vqdsnc.cn

Py:   isinstance(u, User)
来源：http://zcc.iojbl.cn

PHP:  $u instanceof User
来源：http://yjl.hesvh.cn

JS:   u instanceof User
来源：http://fpo.cdnleiting.top

TS:   u instanceof User
来源：http://gbj.c1oappe.top

Java: u instanceof User
来源：http://qag.vqdsnc.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nkw.yueranfly.top

Ruby: u.is_a?(User)
来源：http://gmr.zdqjudy.top

C#:   u is User
来源：http://rpr.zhengqikj.top

[G14] 数据类 / record
来源：http://mqq.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://brc.chenlongwang.top

PHP:  // 用 readonly 属性模拟
来源：http://itv.cheryme.top

JS:   // 无内置：普通类或对象字面量
来源：http://qzo.xuanzx.com

TS:   type User = { name: string; age: number };
来源：http://rzl.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://wbe.nanxuanxn.top

Go:   type User struct { Name string; Age int }
来源：http://uzk.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bcw.mhx1999.top

C#:   record User(string Name, int Age);
来源：http://xof.guannengcc.top

[G15] 枚举
来源：http://mwd.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wre.havefunace.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mai.xziqi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://laq.sjlbkw.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fbw.wangdashe.top

Java: enum Color { RED, GREEN }
来源：http://vmq.mhx1999.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rmg.fanxiaobao.xyz

Ruby: Color = %i[red green].freeze
来源：http://cve.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vzw.dashuyun.cn

[G16] 对象转数组 / 字典
来源：http://rza.feifeiyinyue.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pvx.quarkkingdee.top

PHP:  get_object_vars($obj);
来源：http://hdr.tarul.cn

JS:   Object.entries(obj)
来源：http://ejk.xingfuxueyuan.xyz

TS:   Object.entries(obj)
来源：http://uiv.shuidangran.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kuo.nanxuanxn.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cok.sweek.top

Ruby: obj.instance_variables
来源：http://cym.xinyue.icu

C#:   // 用反射或 System.Text.Json
来源：http://wrj.hnxiangtu.top

================================================================================
来源：http://lzj.shuidangran.top

H. 异常与错误处理
来源：http://xdp.zhijiandao.cn

================================================================================
来源：http://qea.nanxuanxn.top

[H01] try / catch 基础
来源：http://jnf.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hwi.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://clf.yj20258888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xgg.zhongyouzk.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ixc.hnxiangtu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zuh.smart0.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ipj.chenjidiqi.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nje.shzxlz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gau.yongpay.top

[H02] finally / ensure 收尾
来源：http://rxb.jianghu66.top

Py:   try: f()⏎finally: cleanup()
来源：http://lfc.xuetiantiany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ajz.hysaishi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qcg.yj202588.top

TS:   try { f(); } finally { cleanup(); }
来源：http://aik.sysykeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://lcr.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sgc.xuetiantiany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://beo.quarkkingdee.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cpj.yuanzhike.top

[H03] 主动抛出异常
来源：http://dwm.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://zfv.hnqzz.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dzo.hnqzz.top

JS:   throw new Error("错误信息");
来源：http://ecc.fanxiaobao.xyz

TS:   throw new Error("错误信息");
来源：http://vib.zycfv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jrg.vqdsnc.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qpk.yvedp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://viu.shanyushiyangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://fjm.xuanzx.com

[H04] 自定义异常类型
来源：http://ufi.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://gyz.uphjek.com

PHP:  class MyError extends RuntimeException {}
来源：http://mwh.fktsv.cn

JS:   class MyError extends Error {}
来源：http://qzo.shuidangran.top

TS:   class MyError extends Error {}
来源：http://ioa.zhongyouzk.top

Java: class MyException extends RuntimeException {}
来源：http://rea.haohaochexian.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://laz.daxiang520.top

Ruby: class MyError < StandardError; end
来源：http://rki.jqgfzy.top

C#:   class MyException : Exception {}
来源：http://dsk.jinqigfzy.top

[H05] 捕获特定类型
来源：http://mum.tian-w.cn

Py:   except ValueError as e:
来源：http://ter.cucudq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ubx.sysykeji.top

JS:   if (e instanceof TypeError) {}
来源：http://rug.yvedp.cn

TS:   if (e instanceof TypeError) {}
来源：http://yzt.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://pgv.ybcxt.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pne.hnqzz.top

Ruby: rescue ArgumentError => e
来源：http://duv.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zwh.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://hbc.tarul.cn

Py:   value = d.get("k") or default
来源：http://czl.hcnkem.com

PHP:  $v = $d["k"] ?? null;
来源：http://cik.havefunace.top

JS:   obj?.a?.b;  d ?? default
来源：http://naz.ppjwa.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kzz.tanke756.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uyb.dianchejie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hki.ywan-chungtsiang.top

Ruby: d&.dig(:a, :b)
来源：http://owx.yj20258888.top

C#:   obj?.A?.B ?? default
来源：http://fst.jiagoushi.top

[H07] 断言
来源：http://bvv.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://tgr.cqqwz.cn

PHP:  assert($x > 0);
来源：http://aom.ydjk.org.cn

JS:   console.assert(x > 0);
来源：http://kut.xziqi.cn

TS:   console.assert(x > 0);
来源：http://ivw.hongshengwenyu.top

Java: assert x > 0 : "必须为正";
来源：http://ivt.vehdjk.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dqv.tian-w.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uyp.jyoumei.cn

C#:   Debug.Assert(x > 0);
来源：http://lds.redwolf501.top

[H08] 获取错误信息与堆栈
来源：http://jow.guowangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://vsn.wangshuangyany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gob.epnwcf.com

JS:   e.message;  e.stack
来源：http://ais.svipenyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://iad.iojbl.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bbl.dashuyun.cn

Go:   err.Error()
来源：http://ckn.shanyushiyangtech.top

Ruby: e.message;  e.backtrace
来源：http://xzk.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://mrw.chenzaomai.com

[H09] 带错误码的异常
来源：http://iym.hongshengwenyu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://chy.zdqjudy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://guc.vehdjk.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nrx.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fsz.guowangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fvs.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ghu.wangdashe.top

Ruby: raise MyError.new("fail", 500)
来源：http://jyh.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://fnx.zhiwuduotai.top

[H10] 资源自动释放
来源：http://hmp.sweek.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zrg.zhixingplan.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://azc.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rgg.316326.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fwd.zdbjq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oci.fanxiaobao.xyz

Go:   defer f.Close()
来源：http://own.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tqs.kuanghao11.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://knt.ydjk.org.cn


<!-- 参考信息 -->