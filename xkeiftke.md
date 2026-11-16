代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://cku.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qxl.chenjidiqi.icu

PHP:  file_exists("a.txt");
来源：http://aaj.yanxiufei.cn

JS:   fs.existsSync("a.txt")
来源：http://kmt.guannengcc.top

TS:   fs.existsSync("a.txt")
来源：http://zsj.mhx1999.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hzk.daxiang520.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hnc.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://jrk.nanxuanxn.top

C#:   File.Exists("a.txt")
来源：http://bbg.fanxiaobao.xyz

[F06] 删除文件
来源：http://hup.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://rva.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://ldu.zhiwuduotai.top

JS:   fs.unlinkSync("a.txt")
来源：http://unk.sjlbkw.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zke.tarul.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xdh.zdbjq.cn

Go:   os.Remove("a.txt")
来源：http://dyc.zycfv.cn

Ruby: File.delete("a.txt")
来源：http://jsu.zhongyouzk.top

C#:   File.Delete("a.txt");
来源：http://olq.nanxinkj.top

[F07] 创建目录（含多级）
来源：http://qje.andypj.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sfz.wangshuangyany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gbi.jqgfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pmi.birdmap.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ahj.daria6918.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://anl.hesvh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nlg.nwbrower.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qwv.smart0.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://coj.316326.xyz

[F08] 遍历目录
来源：http://usb.zhengqikj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://evc.pengpengdd.cyou

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://siq.mhx1999.top

JS:   fs.readdirSync("dir")
来源：http://vbk.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://lvp.vqdsnc.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ncw.jyoumei.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nnn.hnqzz.top

Ruby: Dir.children("dir")
来源：http://erq.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://xsg.zhaomingkeji.xyz

[F09] 获取文件大小
来源：http://hav.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://gae.sxryk.cn

PHP:  filesize("a.txt");
来源：http://zoe.zdbjq.cn

JS:   fs.statSync("a.txt").size
来源：http://uje.shanyushiyangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://rxl.zhijiandao.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hsf.cucudq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://exo.svipenyu.cn

Ruby: File.size("a.txt")
来源：http://ihm.cdnleiting.top

C#:   new FileInfo("a.txt").Length
来源：http://pvk.guowangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://hcj.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ryg.fktsv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gbd.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://seq.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://kmn.hysaishi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://scr.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zim.316326.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ttd.guannengcc.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wem.sufxvd.cn

[F11] 复制与移动文件
来源：http://lly.svipenyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uml.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://juo.yj202588.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://igx.shanyushiyangtech.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kdv.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ikr.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://inj.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lvn.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qku.chenlongwang.top

[F12] CSV 读写
来源：http://vux.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sio.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://luc.xuanzx.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yos.fengsongda.top

TS:   // 同上
来源：http://ifp.hysaishi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dhw.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://byc.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tyj.cashguo.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uwp.birdmap.top

================================================================================
来源：http://els.ppjwa.cn

G. 面向对象
来源：http://bkd.0kj1m.cn

================================================================================
来源：http://rxh.nwbrower.top

[G01] 定义类
来源：http://tgv.ehwqpu.com

Py:   class User: pass
来源：http://dgl.yfazqb.com

PHP:  class User {}
来源：http://uoi.ywan-chungtsiang.top

JS:   class User {}
来源：http://dav.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://nud.zdqjudy.top

Java: class User {}
来源：http://kgp.jinqigufen.top

Go:   type User struct { Name string }
来源：http://xrp.jqgufenzy.top

Ruby: class User; end
来源：http://qxe.hcnkem.com

C#:   class User {}
来源：http://xir.feifeiyinyue.top

[G02] 构造函数
来源：http://bcn.smart0.xyz

Py:   def __init__(self, name): self.name = name
来源：http://chd.sufxvd.cn

PHP:  public function __construct(public string $name) {}
来源：http://vat.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://tuu.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://sdf.ywan-chungtsiang.top

Java: User(String name) { this.name = name; }
来源：http://mws.guannengcc.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dkg.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://uji.dianchejie.cn

C#:   public User(string name) { Name = name; }
来源：http://lvx.tian-w.cn

[G03] 实例属性
来源：http://ctw.jianghu66.top

Py:   self.name = "x"
来源：http://cjw.hesvh.cn

PHP:  public string $name = "x";
来源：http://yhe.yuanzhike.top

JS:   this.name = "x";
来源：http://job.zhixingplan.top

TS:   name: string = "x";
来源：http://xxq.sufxvd.cn

Java: private String name;
来源：http://vkn.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ctu.0kj1m.cn

Ruby: @name = "x"
来源：http://nuz.xuetiantiany.cn

C#:   public string Name { get; set; } = "x";
来源：http://hep.hcnkem.com

[G04] 定义方法
来源：http://qkn.sweek.top

Py:   def greet(self): return self.name
来源：http://hhg.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://dmj.gotoacloud.top

JS:   greet() { return this.name; }
来源：http://nci.hesvh.cn

TS:   greet(): string { return this.name; }
来源：http://von.yj202588.top

Java: String greet() { return name; }
来源：http://wlc.fehbvm.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://iaa.guowangkeji.top

Ruby: def greet; @name; end
来源：http://lft.tianlin.xyz

C#:   public string Greet() => Name;
来源：http://vui.jinqigufen.top

[G05] 继承
来源：http://haz.nanxuanxn.top

Py:   class Admin(User): pass
来源：http://zre.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://ipj.ydzc1.top

JS:   class Admin extends User {}
来源：http://ayu.yangfankeji.com

TS:   class Admin extends User {}
来源：http://elv.sufxvd.cn

Java: class Admin extends User {}
来源：http://get.xingfuxueyuan.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://meh.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://udz.fktsv.cn

C#:   class Admin : User {}
来源：http://avj.xinyue.icu

[G06] 重写方法
来源：http://zkv.daria6918.cn

Py:   def greet(self): return "admin"
来源：http://kll.hnxiangtu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://etw.zhengqikj.top

JS:   greet() { return "admin"; }
来源：http://pvb.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://pst.cdnleiting.top

Java: @Override String greet() { return "admin"; }
来源：http://gmk.vqdsnc.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ovg.jlsjyb.cn

Ruby: def greet; "admin"; end
来源：http://zau.nwbrower.top

C#:   public override string Greet() => "admin";
来源：http://wtp.birdmap.top

[G07] 调用父类方法
来源：http://qxc.tarul.cn

Py:   super().greet()
来源：http://kjx.hnqzz.top

PHP:  parent::greet();
来源：http://jsm.hcnkem.com

JS:   super.greet();
来源：http://syf.zhongyouzk.top

TS:   super.greet();
来源：http://lnz.bbcook.cn

Java: super.greet();
来源：http://khq.smart0.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ede.chenlongwang.top

Ruby: super
来源：http://lcg.0kj1m.cn

C#:   base.Greet();
来源：http://qkl.zhoulong.xyz

[G08] 静态方法与属性
来源：http://hvz.gotoacloud.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ikb.feifeiyinyue.top

PHP:  public static function f() {}
来源：http://otr.zhengqikj.top

JS:   static f() {}
来源：http://nlo.ppjwa.cn

TS:   static f(): void {}
来源：http://rsl.sjlbkw.cn

Java: static void f() {}
来源：http://hxg.ybcxt.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://juo.jiagoushi.top

Ruby: def self.f; end
来源：http://ewh.nanxuanxn.top

C#:   public static void F() {}
来源：http://jro.gogol.net.cn

[G09] 接口 / 抽象类
来源：http://nnx.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://xfn.zhoulong.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://myg.gaohongyu789.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qnc.xziqi.cn

TS:   interface Shape { area(): number; }
来源：http://wtz.vqdsnc.cn

Java: interface Shape { double area(); }
来源：http://ptb.tarul.cn

Go:   type Shape interface { Area() float64 }
来源：http://hav.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yet.xuanzx.com

C#:   interface IShape { double Area(); }
来源：http://vol.sufxvd.cn

[G10] 访问控制
来源：http://cwy.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://ykz.jqgfzy.top

PHP:  public / protected / private
来源：http://cuy.uphjek.com

JS:   #private 字段；其余公开
来源：http://knj.sweek.top

TS:   public / protected / private
来源：http://xko.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://hpk.hesvh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ziv.birdmap.top

Ruby: public / protected / private
来源：http://ydc.daria6918.cn

C#:   public / protected / private / internal
来源：http://dse.chenlongwang.top

[G11] getter / setter
来源：http://dbu.sweek.top

Py:   @property 与 @x.setter
来源：http://jpi.shanyushiyangtech.top

PHP:  public function getName(): string { return $this->name; }
来源：http://oup.chenlongwang.top

JS:   get name() { return this._name; }
来源：http://zys.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://trq.316326.xyz

Java: public String getName() { return name; }
来源：http://ins.havefunace.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cdw.guannengcc.top

Ruby: attr_accessor :name
来源：http://kob.shanyushiyangkeji.top

C#:   public string Name { get; set; }
来源：http://vyg.hfpthk.cn

[G12] 对象转字符串
来源：http://jpg.yueranfly.top

Py:   def __str__(self): return self.name
来源：http://rak.zhengqikj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xxq.yanxiufei.cn

JS:   toString() { return this.name; }
来源：http://vpm.iojbl.cn

TS:   toString(): string { return this.name; }
来源：http://ozf.xylfe.cn

Java: @Override public String toString() { return name; }
来源：http://zut.guowangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://qqx.birdmap.top

Ruby: def to_s; @name; end
来源：http://tff.xuetiantiany.cn

C#:   public override string ToString() => Name;
来源：http://fqb.wangdashe.top

[G13] 判断对象类型
来源：http://nui.dianchejie.cn

Py:   isinstance(u, User)
来源：http://afh.feifeiyinyue.top

PHP:  $u instanceof User
来源：http://ass.gzhubu.top

JS:   u instanceof User
来源：http://lio.zhijiandao.cn

TS:   u instanceof User
来源：http://hic.pycfn.com

Java: u instanceof User
来源：http://fba.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zcw.zhengqikj.top

Ruby: u.is_a?(User)
来源：http://tqp.andypj.xyz

C#:   u is User
来源：http://dqb.zhengqikj.top

[G14] 数据类 / record
来源：http://bbl.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jwd.hcnkem.com

PHP:  // 用 readonly 属性模拟
来源：http://gvu.cqqwz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lxm.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://vif.fengsongda.top

Java: record User(String name, int age) {}
来源：http://vtf.zhongyouzk.top

Go:   type User struct { Name string; Age int }
来源：http://noa.vqdsnc.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://crl.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://fxw.fzhhl.top

[G15] 枚举
来源：http://sgp.cucudq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vcf.svipenyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qxl.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nef.yj20258.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://isg.hesvh.cn

Java: enum Color { RED, GREEN }
来源：http://xel.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rjl.fktsv.cn

Ruby: Color = %i[red green].freeze
来源：http://xrm.smart0.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rre.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://hae.vehdjk.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kbd.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://gfb.shanyushiyangkeji.top

JS:   Object.entries(obj)
来源：http://ply.hcnkem.com

TS:   Object.entries(obj)
来源：http://kmf.yj202588.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sxi.vehdjk.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://myu.fktsv.cn

Ruby: obj.instance_variables
来源：http://cbb.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://mdw.hongshengwenyu.top

================================================================================
来源：http://sbu.xinyue.icu

H. 异常与错误处理
来源：http://mmh.c1oappe.top

================================================================================
来源：http://gbs.yj20258888.top

[H01] try / catch 基础
来源：http://ndg.fehbvm.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zxt.dashuyun.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nml.fengsongda.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ato.zhaomingkeji.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cuc.cqqwz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kkb.andypj.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kfn.yueranfly.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kol.daria6918.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mir.snrcjt.cn

[H02] finally / ensure 收尾
来源：http://pso.mhx1999.top

Py:   try: f()⏎finally: cleanup()
来源：http://tvl.hnxiangtu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dgo.jinqigufen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cuf.jinyuanbaomall.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ucs.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eoa.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://slo.uphjek.com

Ruby: begin; f; ensure; cleanup; end
来源：http://qoh.shanyushiyangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fmj.guowangkeji.top

[H03] 主动抛出异常
来源：http://yla.yanxiufei.cn

Py:   raise ValueError("错误信息")
来源：http://nug.ppjwa.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dph.yongpay.top

JS:   throw new Error("错误信息");
来源：http://uaa.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://urb.yongpay.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dcm.jqgufenzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ont.wangdashe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ukm.svipenyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pie.kuanghao11.cn

[H04] 自定义异常类型
来源：http://yye.hywenlv.cn

Py:   class MyError(Exception): pass
来源：http://tmp.sjlbkw.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uhq.sweek.top

JS:   class MyError extends Error {}
来源：http://bjc.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://phm.xziqi.cn

Java: class MyException extends RuntimeException {}
来源：http://xny.c1oappe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ftr.gzhubu.top

Ruby: class MyError < StandardError; end
来源：http://qos.nanxuanxn.top

C#:   class MyException : Exception {}
来源：http://cur.yj202588.top

[H05] 捕获特定类型
来源：http://mfd.xylfe.cn

Py:   except ValueError as e:
来源：http://oqc.hcnkem.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xyh.yueranfly.top

JS:   if (e instanceof TypeError) {}
来源：http://zar.zhijiandao.cn

TS:   if (e instanceof TypeError) {}
来源：http://icp.jlsjyb.cn

Java: catch (IOException | SQLException e) {}
来源：http://rdi.316326.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sns.havefunace.top

Ruby: rescue ArgumentError => e
来源：http://wrh.hcnkem.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mgf.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://ydu.gzhubu.top

Py:   value = d.get("k") or default
来源：http://gli.zhiwuduotai.top

PHP:  $v = $d["k"] ?? null;
来源：http://hnk.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://kkc.shangyingyoupin.top

TS:   obj?.a?.b;  d ?? default
来源：http://hpy.hesvh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://acn.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://irm.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://nfo.hysaishi.cn

C#:   obj?.A?.B ?? default
来源：http://rqq.sysykeji.top

[H07] 断言
来源：http://vde.shanyushiyangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://csa.ywan-chungtsiang.top

PHP:  assert($x > 0);
来源：http://stl.vqdsnc.cn

JS:   console.assert(x > 0);
来源：http://ktf.jlsjyb.cn

TS:   console.assert(x > 0);
来源：http://ggm.havefunace.top

Java: assert x > 0 : "必须为正";
来源：http://dzj.quarkkingdee.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yks.guannengcc.top

Ruby: raise "必须为正" unless x > 0
来源：http://psg.gotoacloud.top

C#:   Debug.Assert(x > 0);
来源：http://nlk.sysykeji.top

[H08] 获取错误信息与堆栈
来源：http://lcb.fzhhl.top

Py:   str(e);  traceback.format_exc()
来源：http://rza.yj20258.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vst.yj20258.top

JS:   e.message;  e.stack
来源：http://fvl.vehdjk.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://qkj.sufxvd.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tvr.dianchejie.cn

Go:   err.Error()
来源：http://rvo.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://doe.hfpthk.cn

C#:   e.Message;  e.StackTrace
来源：http://erx.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://qex.aizwys.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vms.chenjidiqi.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://mly.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nht.ppjwa.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cjz.hammf.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mbp.jinyuanbaomall.cn


<!-- 参考信息 -->