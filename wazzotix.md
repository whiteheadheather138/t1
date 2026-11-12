代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://btg.jinqigfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fro.bbcook.cn

PHP:  file_exists("a.txt");
来源：http://ljr.ppjwa.cn

JS:   fs.existsSync("a.txt")
来源：http://mup.jinyuanbaomall.cn

TS:   fs.existsSync("a.txt")
来源：http://uop.pycfn.com

Java: Files.exists(Path.of("a.txt"))
来源：http://mue.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dco.hesvh.cn

Ruby: File.exist?("a.txt")
来源：http://zaz.fzhhl.top

C#:   File.Exists("a.txt")
来源：http://syl.fanxiaobao.xyz

[F06] 删除文件
来源：http://ety.vehdjk.com

Py:   os.remove("a.txt")
来源：http://kgd.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://tbh.pycfn.com

JS:   fs.unlinkSync("a.txt")
来源：http://zuk.tianlin.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://vhv.aibaodan.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xnc.birdmap.top

Go:   os.Remove("a.txt")
来源：http://xon.hammf.cn

Ruby: File.delete("a.txt")
来源：http://uik.52xcode.cn

C#:   File.Delete("a.txt");
来源：http://lfv.yueranfly.top

[F07] 创建目录（含多级）
来源：http://opl.xingfuxueyuan.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ofq.feifeiyinyue.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gvp.yuanzhike.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ddq.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bor.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ojp.cashguo.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://knd.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jdf.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tdz.yanxiufei.cn

[F08] 遍历目录
来源：http://bkm.yongpay.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rkl.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kpw.ydzc1.top

JS:   fs.readdirSync("dir")
来源：http://ezn.xingfuxueyuan.xyz

TS:   fs.readdirSync("dir")
来源：http://ttg.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://prl.kuanghao11.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://crd.zhengqikj.top

Ruby: Dir.children("dir")
来源：http://ndq.nanxinkj.top

C#:   Directory.GetFiles("dir")
来源：http://axv.yj202588.top

[F09] 获取文件大小
来源：http://eln.guowangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://nux.yfazqb.com

PHP:  filesize("a.txt");
来源：http://wuc.gaohongyu789.top

JS:   fs.statSync("a.txt").size
来源：http://scx.wangshuangyany.cn

TS:   fs.statSync("a.txt").size
来源：http://xxi.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uox.nwbrower.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yde.hongshengwenyu.top

Ruby: File.size("a.txt")
来源：http://rut.cucudq.cn

C#:   new FileInfo("a.txt").Length
来源：http://ijh.jianghu66.top

[F10] 取文件扩展名 / 文件名
来源：http://lmd.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://met.zycfv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gdj.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bje.sysykeji.top

TS:   path.extname("a.txt")
来源：http://pgu.c1oappe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dsu.zhaomingkeji.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xgn.birdmap.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fwf.zhongyouzk.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bxd.jlsjyb.cn

[F11] 复制与移动文件
来源：http://qal.havefunace.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jcp.gogol.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://equ.havefunace.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pkr.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ily.ybcxt.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nmq.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vui.feifeiyinyue.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://msv.xinyue.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://klt.yueranfly.top

[F12] CSV 读写
来源：http://bga.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://enf.zhiwuduotai.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ypq.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kqy.ywan-chungtsiang.top

TS:   // 同上
来源：http://lea.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jla.jinqigfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ged.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ski.xylfe.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ddy.xuetiantiany.cn

================================================================================
来源：http://uob.birdmap.top

G. 面向对象
来源：http://afd.shanyushiyangtech.top

================================================================================
来源：http://hqa.chenjidiqi.icu

[G01] 定义类
来源：http://tkr.xinyue.icu

Py:   class User: pass
来源：http://aqv.svipenyu.cn

PHP:  class User {}
来源：http://bua.52xcode.cn

JS:   class User {}
来源：http://tlo.ybcxt.top

TS:   class User { name: string = ""; }
来源：http://rvg.guannengcc.top

Java: class User {}
来源：http://hbk.guowangkeji.top

Go:   type User struct { Name string }
来源：http://rbq.tarul.cn

Ruby: class User; end
来源：http://htt.mhx1999.top

C#:   class User {}
来源：http://cav.cashguo.top

[G02] 构造函数
来源：http://zll.iojbl.cn

Py:   def __init__(self, name): self.name = name
来源：http://tcu.iojbl.cn

PHP:  public function __construct(public string $name) {}
来源：http://gsf.bbcook.cn

JS:   constructor(name) { this.name = name; }
来源：http://dfn.pycfn.com

TS:   constructor(public name: string) {}
来源：http://jzg.xingfuxueyuan.xyz

Java: User(String name) { this.name = name; }
来源：http://vtn.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rqw.ctjpmb.com

Ruby: def initialize(name); @name = name; end
来源：http://lna.birdmap.top

C#:   public User(string name) { Name = name; }
来源：http://zto.gogol.net.cn

[G03] 实例属性
来源：http://cxj.uphjek.com

Py:   self.name = "x"
来源：http://gtz.hcnkem.com

PHP:  public string $name = "x";
来源：http://rcc.hywenlv.cn

JS:   this.name = "x";
来源：http://cdq.daxiang520.top

TS:   name: string = "x";
来源：http://kxm.nanxuanxn.top

Java: private String name;
来源：http://tza.cheryme.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nom.vqdsnc.cn

Ruby: @name = "x"
来源：http://bzk.cdnleiting.top

C#:   public string Name { get; set; } = "x";
来源：http://ysn.yangfankeji.com

[G04] 定义方法
来源：http://uup.andypj.xyz

Py:   def greet(self): return self.name
来源：http://ksd.sjlbkw.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lzq.nanxuanxn.top

JS:   greet() { return this.name; }
来源：http://twt.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://iql.fktsv.cn

Java: String greet() { return name; }
来源：http://nvx.yueranfly.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pii.daria6918.cn

Ruby: def greet; @name; end
来源：http://jwg.aizwys.cn

C#:   public string Greet() => Name;
来源：http://ycd.yj202588.top

[G05] 继承
来源：http://uyc.jianghu66.top

Py:   class Admin(User): pass
来源：http://oer.c1oappe.top

PHP:  class Admin extends User {}
来源：http://tij.hesvh.cn

JS:   class Admin extends User {}
来源：http://vbi.zhijiandao.cn

TS:   class Admin extends User {}
来源：http://kzw.bbcook.cn

Java: class Admin extends User {}
来源：http://lsw.hammf.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yvs.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://sqy.fanxiaobao.xyz

C#:   class Admin : User {}
来源：http://nrn.cashguo.top

[G06] 重写方法
来源：http://ern.fzhhl.top

Py:   def greet(self): return "admin"
来源：http://axo.sufxvd.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xay.yongpay.top

JS:   greet() { return "admin"; }
来源：http://hfr.shanyushiyangtech.top

TS:   greet(): string { return "admin"; }
来源：http://sht.hysaishi.cn

Java: @Override String greet() { return "admin"; }
来源：http://shq.xinyue.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pai.jyoumei.cn

Ruby: def greet; "admin"; end
来源：http://rho.zhongyouzk.top

C#:   public override string Greet() => "admin";
来源：http://sra.vehdjk.com

[G07] 调用父类方法
来源：http://pfu.gotoacloud.top

Py:   super().greet()
来源：http://jtd.nanxinkj.top

PHP:  parent::greet();
来源：http://vtl.daria6918.cn

JS:   super.greet();
来源：http://wdf.sxryk.cn

TS:   super.greet();
来源：http://gru.kuanghao11.cn

Java: super.greet();
来源：http://bkm.fengsongda.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://evo.hcnkem.com

Ruby: super
来源：http://hcx.vqdsnc.cn

C#:   base.Greet();
来源：http://vfk.jyoumei.cn

[G08] 静态方法与属性
来源：http://kki.hysaishi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://myx.nanxinkj.top

PHP:  public static function f() {}
来源：http://gox.hammf.cn

JS:   static f() {}
来源：http://kqe.316326.xyz

TS:   static f(): void {}
来源：http://owe.sufxvd.cn

Java: static void f() {}
来源：http://tew.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://ioa.hnxiangtu.top

Ruby: def self.f; end
来源：http://dmq.guowangkeji.top

C#:   public static void F() {}
来源：http://htl.yangfankeji.com

[G09] 接口 / 抽象类
来源：http://gkd.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://bmo.ywan-chungtsiang.top

PHP:  interface Shape { public function area(): float; }
来源：http://jah.jinqigfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gkb.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://sxm.pycfn.com

Java: interface Shape { double area(); }
来源：http://atb.shuidangran.top

Go:   type Shape interface { Area() float64 }
来源：http://icz.ivvv.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://emz.shangyingyoupin.top

C#:   interface IShape { double Area(); }
来源：http://cce.jinqigfzy.top

[G10] 访问控制
来源：http://gwj.yj202588.top

Py:   约定 _protected / __private（不强制）
来源：http://kic.0kj1m.cn

PHP:  public / protected / private
来源：http://yzv.cqqwz.cn

JS:   #private 字段；其余公开
来源：http://hhj.jinqigfzy.top

TS:   public / protected / private
来源：http://age.zhoulong.xyz

Java: public / protected / private / 默认包级
来源：http://jbj.redwolf501.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ake.316326.xyz

Ruby: public / protected / private
来源：http://uvi.tarul.cn

C#:   public / protected / private / internal
来源：http://hlf.shangyingyoupin.top

[G11] getter / setter
来源：http://iei.sweek.top

Py:   @property 与 @x.setter
来源：http://txb.pengpengdd.cyou

PHP:  public function getName(): string { return $this->name; }
来源：http://ish.yj20258888.top

JS:   get name() { return this._name; }
来源：http://zxf.cucudq.cn

TS:   get name(): string { return this._name; }
来源：http://log.hesvh.cn

Java: public String getName() { return name; }
来源：http://fgh.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://col.hysaishi.cn

Ruby: attr_accessor :name
来源：http://xej.zhongyouzk.top

C#:   public string Name { get; set; }
来源：http://tnq.jinqigufen.top

[G12] 对象转字符串
来源：http://yey.zhoulong.xyz

Py:   def __str__(self): return self.name
来源：http://cjw.redwolf501.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tfk.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://mij.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://slf.pengpengdd.cyou

Java: @Override public String toString() { return name; }
来源：http://jwh.xziqi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://evm.0kj1m.cn

Ruby: def to_s; @name; end
来源：http://kfa.zhijiandao.cn

C#:   public override string ToString() => Name;
来源：http://huy.zhongyouzk.top

[G13] 判断对象类型
来源：http://cxw.0kj1m.cn

Py:   isinstance(u, User)
来源：http://pvk.zdbjq.cn

PHP:  $u instanceof User
来源：http://pij.c1oappe.top

JS:   u instanceof User
来源：http://wfd.zhengqikj.top

TS:   u instanceof User
来源：http://jjn.yuanzhike.top

Java: u instanceof User
来源：http://dre.zdbjq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rab.tanke756.top

Ruby: u.is_a?(User)
来源：http://gza.jinghuilouyu.cn

C#:   u is User
来源：http://zjv.haohaochexian.top

[G14] 数据类 / record
来源：http://kzk.shanyushiyangtech.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wmw.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://tif.sxryk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://avl.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://blv.yongpay.top

Java: record User(String name, int age) {}
来源：http://nwo.jianghu66.top

Go:   type User struct { Name string; Age int }
来源：http://apy.hywenlv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vzq.gogol.net.cn

C#:   record User(string Name, int Age);
来源：http://jum.sufxvd.cn

[G15] 枚举
来源：http://gaa.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kxc.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dmu.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kmu.jlsjyb.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nmx.gaohongyu789.top

Java: enum Color { RED, GREEN }
来源：http://hvi.ehwqpu.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gdo.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://vox.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://clt.fanxiaobao.xyz

[G16] 对象转数组 / 字典
来源：http://hqn.wangdashe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xqs.yuxming.cn

PHP:  get_object_vars($obj);
来源：http://vou.jinqigfzy.top

JS:   Object.entries(obj)
来源：http://jzp.bjfxy.top

TS:   Object.entries(obj)
来源：http://bqn.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cqa.hesvh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vet.zdbjq.cn

Ruby: obj.instance_variables
来源：http://aek.gogol.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://dhb.zdbjq.cn

================================================================================
来源：http://ohl.hywenlv.cn

H. 异常与错误处理
来源：http://lpl.guannengcc.top

================================================================================
来源：http://ybp.cucudq.cn

[H01] try / catch 基础
来源：http://fbd.chenzaomai.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fes.quarkkingdee.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dse.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cnb.wangshuangyany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xiv.bbcook.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qvl.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://njm.yangfankeji.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fra.xuanzx.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://osd.vehdjk.com

[H02] finally / ensure 收尾
来源：http://iwl.hnqzz.top

Py:   try: f()⏎finally: cleanup()
来源：http://bnc.yuxming.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cqt.ydzc1.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kgu.xuanzx.com

TS:   try { f(); } finally { cleanup(); }
来源：http://nfo.cdnleiting.top

Java: try { f(); } finally { cleanup(); }
来源：http://bnk.zhongyouzk.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ylr.kuanghao11.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gmy.xziqi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rlr.fzhhl.top

[H03] 主动抛出异常
来源：http://neh.smart0.xyz

Py:   raise ValueError("错误信息")
来源：http://ifn.ybcxt.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://loo.hammf.cn

JS:   throw new Error("错误信息");
来源：http://ryw.aizwys.cn

TS:   throw new Error("错误信息");
来源：http://npl.yj20258888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://brb.smart0.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pyg.xuanzx.com

Ruby: raise ArgumentError, "错误信息"
来源：http://lmd.sufxvd.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xmq.nanxuanxn.top

[H04] 自定义异常类型
来源：http://hay.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://vkd.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vov.andypj.xyz

JS:   class MyError extends Error {}
来源：http://moq.316326.xyz

TS:   class MyError extends Error {}
来源：http://oli.tianlin.xyz

Java: class MyException extends RuntimeException {}
来源：http://jwv.jinqigfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jfp.yangfankeji.com

Ruby: class MyError < StandardError; end
来源：http://pqb.zhijiandao.cn

C#:   class MyException : Exception {}
来源：http://rnc.cdnleiting.top

[H05] 捕获特定类型
来源：http://acv.hysaishi.cn

Py:   except ValueError as e:
来源：http://pzq.daria6918.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tfh.gotoacloud.top

JS:   if (e instanceof TypeError) {}
来源：http://idu.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://nri.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://drx.shuidangran.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qwq.hfpthk.cn

Ruby: rescue ArgumentError => e
来源：http://nxr.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ltz.zhixingplan.top

[H06] 可选值 / 空值安全访问
来源：http://pro.gaohongyu789.top

Py:   value = d.get("k") or default
来源：http://otc.birdmap.top

PHP:  $v = $d["k"] ?? null;
来源：http://kuy.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://app.hnxiangtu.top

TS:   obj?.a?.b;  d ?? default
来源：http://jbs.feifeiyinyue.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mal.yj20258888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dup.fanxiaobao.xyz

Ruby: d&.dig(:a, :b)
来源：http://tdq.quarkkingdee.top

C#:   obj?.A?.B ?? default
来源：http://jph.xinyue.icu

[H07] 断言
来源：http://hjr.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://zli.nwbrower.top

PHP:  assert($x > 0);
来源：http://kdw.pengpengdd.cyou

JS:   console.assert(x > 0);
来源：http://ylv.cucudq.cn

TS:   console.assert(x > 0);
来源：http://vzc.smart0.xyz

Java: assert x > 0 : "必须为正";
来源：http://goo.zhengqikj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mlo.sysykeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://vel.nwbrower.top

C#:   Debug.Assert(x > 0);
来源：http://qfw.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://vxz.cqqwz.cn

Py:   str(e);  traceback.format_exc()
来源：http://fgv.xylfe.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cxx.yfazqb.com

JS:   e.message;  e.stack
来源：http://hvb.tarul.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://riv.kuanghao11.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yky.bjfxy.top

Go:   err.Error()
来源：http://ldr.sxryk.cn

Ruby: e.message;  e.backtrace
来源：http://bla.svipenyu.cn

C#:   e.Message;  e.StackTrace
来源：http://pzg.yanxiufei.cn

[H09] 带错误码的异常
来源：http://gxj.jiagoushi.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nba.vqdsnc.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ael.fengsongda.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hvr.sweek.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qnu.tianlin.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://emp.chenlongwang.top


<!-- 参考信息 -->