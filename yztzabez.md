代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://dvv.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gmx.nwbrower.top

PHP:  file_exists("a.txt");
来源：http://ntg.yuxming.cn

JS:   fs.existsSync("a.txt")
来源：http://owz.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://jag.tanke756.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hjq.daxiang520.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bwr.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://btg.gaohongyu789.top

C#:   File.Exists("a.txt")
来源：http://eah.quarkkingdee.top

[F06] 删除文件
来源：http://suq.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://kxx.zhengqikj.top

PHP:  unlink("a.txt");
来源：http://nro.xziqi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ady.fzhhl.top

TS:   fs.unlinkSync("a.txt")
来源：http://fes.zycfv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aqt.uphjek.com

Go:   os.Remove("a.txt")
来源：http://czk.chenzaomai.com

Ruby: File.delete("a.txt")
来源：http://yut.xingfuxueyuan.xyz

C#:   File.Delete("a.txt");
来源：http://lnd.hfpthk.cn

[F07] 创建目录（含多级）
来源：http://rin.cqqwz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hqp.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fhj.ydjk.org.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wlm.pycfn.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ypq.9152youxi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jjk.ydjk.org.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wzg.kuanghao11.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kxa.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kpa.xziqi.cn

[F08] 遍历目录
来源：http://ngd.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://yvu.gogol.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vos.hnxiangtu.top

JS:   fs.readdirSync("dir")
来源：http://oiq.shanyushiyangtech.top

TS:   fs.readdirSync("dir")
来源：http://pym.guannengcc.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pjt.snrcjt.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://klw.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://vbp.vehdjk.com

C#:   Directory.GetFiles("dir")
来源：http://top.xziqi.cn

[F09] 获取文件大小
来源：http://lqw.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://nvz.xinyue.icu

PHP:  filesize("a.txt");
来源：http://rve.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://tdl.smart0.xyz

TS:   fs.statSync("a.txt").size
来源：http://jxh.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qht.fzhhl.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://szw.jianghu66.top

Ruby: File.size("a.txt")
来源：http://oqy.jinyuanbaomall.cn

C#:   new FileInfo("a.txt").Length
来源：http://kxp.dianchejie.cn

[F10] 取文件扩展名 / 文件名
来源：http://fdq.xinyue.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ank.xylfe.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gqy.haohaochexian.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sdo.yuxming.cn

TS:   path.extname("a.txt")
来源：http://rgu.sysykeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pmy.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gpw.snrcjt.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zwk.tianlin.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rza.jinyuanbaomall.cn

[F11] 复制与移动文件
来源：http://cub.hesvh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rda.hcnkem.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kfa.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ekl.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://akd.xziqi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eac.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://soj.hesvh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vli.shuidangran.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ctv.cdnleiting.top

[F12] CSV 读写
来源：http://pew.ybcxt.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yyi.jyoumei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ylz.chenzaomai.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ntn.jiagoushi.top

TS:   // 同上
来源：http://lrt.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kgx.c1oappe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://idr.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fyf.aibaodan.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tvv.cucudq.cn

================================================================================
来源：http://drj.quarkkingdee.top

G. 面向对象
来源：http://nfn.sxryk.cn

================================================================================
来源：http://ydn.daria6918.cn

[G01] 定义类
来源：http://odj.hongshengwenyu.top

Py:   class User: pass
来源：http://otp.jianghu66.top

PHP:  class User {}
来源：http://ucj.aibaodan.cn

JS:   class User {}
来源：http://kek.pengpengdd.cyou

TS:   class User { name: string = ""; }
来源：http://map.zhijiandao.cn

Java: class User {}
来源：http://qeq.sweek.top

Go:   type User struct { Name string }
来源：http://wbp.shuidangran.top

Ruby: class User; end
来源：http://zvv.jqgfzy.top

C#:   class User {}
来源：http://ncm.chenlongwang.top

[G02] 构造函数
来源：http://fah.52xcode.cn

Py:   def __init__(self, name): self.name = name
来源：http://bsc.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://jwb.aibaodan.cn

JS:   constructor(name) { this.name = name; }
来源：http://gcf.sjlbkw.cn

TS:   constructor(public name: string) {}
来源：http://kwd.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://ptv.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eva.jianghu66.top

Ruby: def initialize(name); @name = name; end
来源：http://sgx.guowangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://sey.ywan-chungtsiang.top

[G03] 实例属性
来源：http://nhs.wangshuangyany.cn

Py:   self.name = "x"
来源：http://ihm.c1oappe.top

PHP:  public string $name = "x";
来源：http://xhj.jiagoushi.top

JS:   this.name = "x";
来源：http://aev.hnqzz.top

TS:   name: string = "x";
来源：http://xzh.jianghu66.top

Java: private String name;
来源：http://pck.chenzaomai.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pyv.9152youxi.cn

Ruby: @name = "x"
来源：http://udk.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://htd.wangdashe.top

[G04] 定义方法
来源：http://jvt.xziqi.cn

Py:   def greet(self): return self.name
来源：http://icj.ppjwa.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cec.jinyuanbaomall.cn

JS:   greet() { return this.name; }
来源：http://xcd.xylfe.cn

TS:   greet(): string { return this.name; }
来源：http://hwh.zhixingplan.top

Java: String greet() { return name; }
来源：http://iok.hcnkem.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://qhw.jianghu66.top

Ruby: def greet; @name; end
来源：http://ihu.nanxuanxn.top

C#:   public string Greet() => Name;
来源：http://oeb.yangfankeji.com

[G05] 继承
来源：http://znz.yfazqb.com

Py:   class Admin(User): pass
来源：http://iux.yj202588.top

PHP:  class Admin extends User {}
来源：http://qrr.yj20258888.top

JS:   class Admin extends User {}
来源：http://flh.quarkkingdee.top

TS:   class Admin extends User {}
来源：http://rey.vqdsnc.cn

Java: class Admin extends User {}
来源：http://ucv.xuanzx.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ouc.jinqigfzy.top

Ruby: class Admin < User; end
来源：http://wtg.shanyushiyangtech.top

C#:   class Admin : User {}
来源：http://pbd.hongshengwenyu.top

[G06] 重写方法
来源：http://vih.guowangkeji.top

Py:   def greet(self): return "admin"
来源：http://obr.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ftm.yuanzhike.top

JS:   greet() { return "admin"; }
来源：http://mut.quarkkingdee.top

TS:   greet(): string { return "admin"; }
来源：http://xod.dianchejie.cn

Java: @Override String greet() { return "admin"; }
来源：http://ypw.ydjk.org.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nut.aibaodan.cn

Ruby: def greet; "admin"; end
来源：http://agn.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://kfv.xziqi.cn

[G07] 调用父类方法
来源：http://bdx.yuanzhike.top

Py:   super().greet()
来源：http://nki.pycfn.com

PHP:  parent::greet();
来源：http://jgn.gogol.net.cn

JS:   super.greet();
来源：http://ydb.daria6918.cn

TS:   super.greet();
来源：http://jiu.sxryk.cn

Java: super.greet();
来源：http://onc.vehdjk.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iki.yonumen.top

Ruby: super
来源：http://vdr.wangshuangyany.cn

C#:   base.Greet();
来源：http://xnk.ivvv.top

[G08] 静态方法与属性
来源：http://sgu.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pmi.yuanzhike.top

PHP:  public static function f() {}
来源：http://xxr.fengsongda.top

JS:   static f() {}
来源：http://xft.gaohongyu789.top

TS:   static f(): void {}
来源：http://heg.zhengqikj.top

Java: static void f() {}
来源：http://uzn.fzhhl.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pqh.xylfe.cn

Ruby: def self.f; end
来源：http://tmb.vehdjk.com

C#:   public static void F() {}
来源：http://gua.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://veo.hysaishi.cn

Py:   from abc import ABC, abstractmethod
来源：http://xgr.xinyue.icu

PHP:  interface Shape { public function area(): float; }
来源：http://bls.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://eve.cheryme.top

TS:   interface Shape { area(): number; }
来源：http://lzo.sysykeji.top

Java: interface Shape { double area(); }
来源：http://okr.ywan-chungtsiang.top

Go:   type Shape interface { Area() float64 }
来源：http://uln.fktsv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://prk.gogol.net.cn

C#:   interface IShape { double Area(); }
来源：http://lxk.hfpthk.cn

[G10] 访问控制
来源：http://hol.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://xnn.sxryk.cn

PHP:  public / protected / private
来源：http://auc.tianlin.xyz

JS:   #private 字段；其余公开
来源：http://ypn.ywan-chungtsiang.top

TS:   public / protected / private
来源：http://byi.svipenyu.cn

Java: public / protected / private / 默认包级
来源：http://nyg.hfpthk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://oan.dashuyun.cn

Ruby: public / protected / private
来源：http://dnh.yonumen.top

C#:   public / protected / private / internal
来源：http://cvq.feifeiyinyue.top

[G11] getter / setter
来源：http://wvt.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://jrw.xinyue.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://xgv.ywan-chungtsiang.top

JS:   get name() { return this._name; }
来源：http://xqi.iojbl.cn

TS:   get name(): string { return this._name; }
来源：http://doe.hnqzz.top

Java: public String getName() { return name; }
来源：http://hhv.hysaishi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kks.0kj1m.cn

Ruby: attr_accessor :name
来源：http://fkr.kuanghao11.cn

C#:   public string Name { get; set; }
来源：http://iya.zhijiandao.cn

[G12] 对象转字符串
来源：http://jmr.52xcode.cn

Py:   def __str__(self): return self.name
来源：http://mxi.yongpay.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mdc.andypj.xyz

JS:   toString() { return this.name; }
来源：http://ygy.tanke756.top

TS:   toString(): string { return this.name; }
来源：http://olt.zdqjudy.top

Java: @Override public String toString() { return name; }
来源：http://fuv.ydzc1.top

Go:   func (u User) String() string { return u.Name }
来源：http://typ.fzhhl.top

Ruby: def to_s; @name; end
来源：http://dtq.tanke756.top

C#:   public override string ToString() => Name;
来源：http://ooh.jyoumei.cn

[G13] 判断对象类型
来源：http://bgz.iojbl.cn

Py:   isinstance(u, User)
来源：http://bry.tianlin.xyz

PHP:  $u instanceof User
来源：http://xts.ydjk.org.cn

JS:   u instanceof User
来源：http://wei.snrcjt.cn

TS:   u instanceof User
来源：http://yhz.nanxinkj.top

Java: u instanceof User
来源：http://txd.guowangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://sai.shanyushiyangtech.top

Ruby: u.is_a?(User)
来源：http://nld.jinghuilouyu.cn

C#:   u is User
来源：http://btq.bbcook.cn

[G14] 数据类 / record
来源：http://isy.tarul.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bmq.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://iki.fehbvm.com

JS:   // 无内置：普通类或对象字面量
来源：http://fmh.hnxiangtu.top

TS:   type User = { name: string; age: number };
来源：http://jeq.gaohongyu789.top

Java: record User(String name, int age) {}
来源：http://ewu.pycfn.com

Go:   type User struct { Name string; Age int }
来源：http://nbm.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zqy.sxryk.cn

C#:   record User(string Name, int Age);
来源：http://zqc.nanxuanxn.top

[G15] 枚举
来源：http://qfo.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oyb.jinqigufen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tpb.fzhhl.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ume.epnwcf.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lbw.yueranfly.top

Java: enum Color { RED, GREEN }
来源：http://hts.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gqi.fanxiaobao.xyz

Ruby: Color = %i[red green].freeze
来源：http://xgr.chenlongwang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qoj.zhaomingkeji.xyz

[G16] 对象转数组 / 字典
来源：http://zhn.xingfuxueyuan.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rpd.nwbrower.top

PHP:  get_object_vars($obj);
来源：http://hfa.cheryme.top

JS:   Object.entries(obj)
来源：http://fox.smart0.xyz

TS:   Object.entries(obj)
来源：http://oue.bbcook.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://thn.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mhh.xuanzx.com

Ruby: obj.instance_variables
来源：http://qhi.52xcode.cn

C#:   // 用反射或 System.Text.Json
来源：http://dzw.ehwqpu.com

================================================================================
来源：http://qlf.gogol.net.cn

H. 异常与错误处理
来源：http://lts.0kj1m.cn

================================================================================
来源：http://qzh.jinyuanbaomall.cn

[H01] try / catch 基础
来源：http://jdq.dashuyun.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://txu.svipenyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://efh.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kru.52xcode.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lzo.ivvv.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rdn.jlsjyb.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vgh.nanxuanxn.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sru.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xdb.redwolf501.top

[H02] finally / ensure 收尾
来源：http://fed.jianghu66.top

Py:   try: f()⏎finally: cleanup()
来源：http://dsh.hammf.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://eic.zycfv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dqa.nanxinkj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ndy.smart0.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://exc.jinyuanbaomall.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ytv.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bom.feifeiyinyue.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bkm.ybcxt.top

[H03] 主动抛出异常
来源：http://nav.hcnkem.com

Py:   raise ValueError("错误信息")
来源：http://kpx.ydzc1.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qfa.jlsjyb.cn

JS:   throw new Error("错误信息");
来源：http://iuq.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://hoy.ybcxt.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fqt.sjlbkw.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oxa.fanxiaobao.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://gqt.svipenyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ali.hongshengwenyu.top

[H04] 自定义异常类型
来源：http://gxi.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://byg.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://iup.hfpthk.cn

JS:   class MyError extends Error {}
来源：http://rqe.tanke756.top

TS:   class MyError extends Error {}
来源：http://yep.c1oappe.top

Java: class MyException extends RuntimeException {}
来源：http://wkx.yj20258.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wza.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://zeu.tarul.cn

C#:   class MyException : Exception {}
来源：http://mlp.ivvv.top

[H05] 捕获特定类型
来源：http://hdy.bjfxy.top

Py:   except ValueError as e:
来源：http://xws.epnwcf.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ccg.chenzaomai.com

JS:   if (e instanceof TypeError) {}
来源：http://btj.9152youxi.cn

TS:   if (e instanceof TypeError) {}
来源：http://spe.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://jun.yuanzhike.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qnk.haohaochexian.top

Ruby: rescue ArgumentError => e
来源：http://imh.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lna.316326.xyz

[H06] 可选值 / 空值安全访问
来源：http://nal.bbcook.cn

Py:   value = d.get("k") or default
来源：http://yfp.yj20258888.top

PHP:  $v = $d["k"] ?? null;
来源：http://jda.zhongyouzk.top

JS:   obj?.a?.b;  d ?? default
来源：http://qjv.uphjek.com

TS:   obj?.a?.b;  d ?? default
来源：http://tfg.redwolf501.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cdq.zhengqikj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ndy.ydjk.org.cn

Ruby: d&.dig(:a, :b)
来源：http://jzu.shangyingyoupin.top

C#:   obj?.A?.B ?? default
来源：http://kwd.guowangkeji.top

[H07] 断言
来源：http://ylh.bbcook.cn

Py:   assert x > 0, "必须为正"
来源：http://dtq.ehwqpu.com

PHP:  assert($x > 0);
来源：http://rev.yj20258.top

JS:   console.assert(x > 0);
来源：http://brk.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://new.kuanghao11.cn

Java: assert x > 0 : "必须为正";
来源：http://bak.gotoacloud.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dze.hnxiangtu.top

Ruby: raise "必须为正" unless x > 0
来源：http://gde.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://wzx.sysykeji.top

[H08] 获取错误信息与堆栈
来源：http://udd.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://qlh.shangyingyoupin.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fip.tanke756.top

JS:   e.message;  e.stack
来源：http://fmt.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ylx.andypj.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://mdj.guowangkeji.top

Go:   err.Error()
来源：http://aau.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://zzp.xziqi.cn

C#:   e.Message;  e.StackTrace
来源：http://hfi.hnqzz.top

[H09] 带错误码的异常
来源：http://enk.yj202588.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://awr.tianlin.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://kmv.jinqigfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xoq.fehbvm.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://umr.shanyushiyangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tbw.yvedp.cn


<!-- 参考信息 -->