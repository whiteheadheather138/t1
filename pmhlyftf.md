代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://elw.ctjpmb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ham.pycfn.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gqp.0kj1m.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nwb.zhijiandao.cn

[F05] 判断文件或目录是否存在
来源：http://xjo.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dcc.hfpthk.cn

PHP:  file_exists("a.txt");
来源：http://kgt.tarul.cn

JS:   fs.existsSync("a.txt")
来源：http://mgi.jinyuanbaomall.cn

TS:   fs.existsSync("a.txt")
来源：http://yuw.quarkkingdee.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ppk.ehwqpu.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ugx.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://rcb.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://foc.zhoulong.xyz

[F06] 删除文件
来源：http://kga.quarkkingdee.top

Py:   os.remove("a.txt")
来源：http://knz.yanxiufei.cn

PHP:  unlink("a.txt");
来源：http://ihm.c1oappe.top

JS:   fs.unlinkSync("a.txt")
来源：http://sui.vqdsnc.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pwz.yuanzhike.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xab.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://woi.yfazqb.com

Ruby: File.delete("a.txt")
来源：http://sbb.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://stq.hcnkem.com

[F07] 创建目录（含多级）
来源：http://gne.ivvv.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qsn.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://npi.redwolf501.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pkj.quarkkingdee.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rfi.tian-w.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wvp.yuxming.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dpt.andypj.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bcr.tian-w.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qle.0kj1m.cn

[F08] 遍历目录
来源：http://lwp.dianchejie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uut.xingfuxueyuan.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nzt.sweek.top

JS:   fs.readdirSync("dir")
来源：http://xoe.hnqzz.top

TS:   fs.readdirSync("dir")
来源：http://kuv.cdnleiting.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mix.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://nes.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://pam.xinyue.icu

C#:   Directory.GetFiles("dir")
来源：http://gvc.xinyue.icu

[F09] 获取文件大小
来源：http://fnh.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://vkt.jinyuanbaomall.cn

PHP:  filesize("a.txt");
来源：http://iwq.yangfankeji.com

JS:   fs.statSync("a.txt").size
来源：http://xav.zhongyouzk.top

TS:   fs.statSync("a.txt").size
来源：http://pft.chenjidiqi.icu

Java: Files.size(Path.of("a.txt"))
来源：http://byr.tian-w.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pzn.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://zoe.cucudq.cn

C#:   new FileInfo("a.txt").Length
来源：http://oqb.kuanghao11.cn

[F10] 取文件扩展名 / 文件名
来源：http://vxk.vqdsnc.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://aej.nanxinkj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fbs.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yni.hnxiangtu.top

TS:   path.extname("a.txt")
来源：http://zqx.zdqjudy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wwe.yuanzhike.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ela.bbcook.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wyr.xylfe.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://loh.fengsongda.top

[F11] 复制与移动文件
来源：http://bla.jlsjyb.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jdr.zhijiandao.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qet.ctjpmb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ufu.gzhubu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wqo.snrcjt.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zfh.shuidangran.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pft.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://euk.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fum.fengsongda.top

[F12] CSV 读写
来源：http://uiu.dianchejie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nnj.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zja.xinyue.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://llt.smart0.xyz

TS:   // 同上
来源：http://kcq.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ofl.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://isb.ivvv.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mvx.birdmap.top

C#:   // 无内置：用 CsvHelper 库
来源：http://chf.zhaomingkeji.xyz

================================================================================
来源：http://vnh.cdnleiting.top

G. 面向对象
来源：http://zrb.fzhhl.top

================================================================================
来源：http://jys.xziqi.cn

[G01] 定义类
来源：http://vay.ybcxt.top

Py:   class User: pass
来源：http://nyb.jlsjyb.cn

PHP:  class User {}
来源：http://pgq.andypj.xyz

JS:   class User {}
来源：http://xsm.shzxlz.cn

TS:   class User { name: string = ""; }
来源：http://qpq.zhongyouzk.top

Java: class User {}
来源：http://fay.gogol.net.cn

Go:   type User struct { Name string }
来源：http://fot.jiagoushi.top

Ruby: class User; end
来源：http://djv.ydzc1.top

C#:   class User {}
来源：http://bpx.aizwys.cn

[G02] 构造函数
来源：http://dgj.redwolf501.top

Py:   def __init__(self, name): self.name = name
来源：http://kiq.hysaishi.cn

PHP:  public function __construct(public string $name) {}
来源：http://lfh.chenzaomai.com

JS:   constructor(name) { this.name = name; }
来源：http://snf.shanyushiyangkeji.top

TS:   constructor(public name: string) {}
来源：http://fml.yuxming.cn

Java: User(String name) { this.name = name; }
来源：http://raq.xinyue.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wub.haohaochexian.top

Ruby: def initialize(name); @name = name; end
来源：http://wkt.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://tai.yuxming.cn

[G03] 实例属性
来源：http://nzn.redwolf501.top

Py:   self.name = "x"
来源：http://bgf.wangdashe.top

PHP:  public string $name = "x";
来源：http://zuj.yangfankeji.com

JS:   this.name = "x";
来源：http://wxv.gotoacloud.top

TS:   name: string = "x";
来源：http://ipx.snrcjt.cn

Java: private String name;
来源：http://wsa.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lel.birdmap.top

Ruby: @name = "x"
来源：http://ave.xinyue.icu

C#:   public string Name { get; set; } = "x";
来源：http://yuc.zhengqikj.top

[G04] 定义方法
来源：http://sty.ydzc1.top

Py:   def greet(self): return self.name
来源：http://xco.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://llu.gogol.net.cn

JS:   greet() { return this.name; }
来源：http://jlc.yanxiufei.cn

TS:   greet(): string { return this.name; }
来源：http://kzo.andypj.xyz

Java: String greet() { return name; }
来源：http://hcq.c1oappe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ojm.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://tib.hammf.cn

C#:   public string Greet() => Name;
来源：http://haz.jqgfzy.top

[G05] 继承
来源：http://izl.tian-w.cn

Py:   class Admin(User): pass
来源：http://yrc.zhiwuduotai.top

PHP:  class Admin extends User {}
来源：http://yjp.jqgufenzy.top

JS:   class Admin extends User {}
来源：http://elr.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://qld.andypj.xyz

Java: class Admin extends User {}
来源：http://ank.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pvs.ywan-chungtsiang.top

Ruby: class Admin < User; end
来源：http://kgv.yfazqb.com

C#:   class Admin : User {}
来源：http://psw.yvedp.cn

[G06] 重写方法
来源：http://bxb.tian-w.cn

Py:   def greet(self): return "admin"
来源：http://ubd.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jfo.yongpay.top

JS:   greet() { return "admin"; }
来源：http://pff.zdbjq.cn

TS:   greet(): string { return "admin"; }
来源：http://qfd.yuanzhike.top

Java: @Override String greet() { return "admin"; }
来源：http://qvv.birdmap.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gnn.chenlongwang.top

Ruby: def greet; "admin"; end
来源：http://dmt.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://ebe.xziqi.cn

[G07] 调用父类方法
来源：http://bhw.hysaishi.cn

Py:   super().greet()
来源：http://smf.gzhubu.top

PHP:  parent::greet();
来源：http://niy.iojbl.cn

JS:   super.greet();
来源：http://bre.kuanghao11.cn

TS:   super.greet();
来源：http://fhq.ctjpmb.com

Java: super.greet();
来源：http://plr.ppjwa.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xfe.316326.xyz

Ruby: super
来源：http://pdz.fanxiaobao.xyz

C#:   base.Greet();
来源：http://xvx.zhongyouzk.top

[G08] 静态方法与属性
来源：http://gik.snrcjt.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://olo.quarkkingdee.top

PHP:  public static function f() {}
来源：http://ypr.jqgfzy.top

JS:   static f() {}
来源：http://kaw.snrcjt.cn

TS:   static f(): void {}
来源：http://slb.yanxiufei.cn

Java: static void f() {}
来源：http://tbx.zdqjudy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nch.guowangkeji.top

Ruby: def self.f; end
来源：http://mbf.zhijiandao.cn

C#:   public static void F() {}
来源：http://rxq.haohaochexian.top

[G09] 接口 / 抽象类
来源：http://ggo.zdqjudy.top

Py:   from abc import ABC, abstractmethod
来源：http://lte.sufxvd.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bkw.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ief.tarul.cn

TS:   interface Shape { area(): number; }
来源：http://mtv.guannengcc.top

Java: interface Shape { double area(); }
来源：http://rab.cdnleiting.top

Go:   type Shape interface { Area() float64 }
来源：http://utu.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jqr.cheryme.top

C#:   interface IShape { double Area(); }
来源：http://irv.jinyuanbaomall.cn

[G10] 访问控制
来源：http://dgu.yfazqb.com

Py:   约定 _protected / __private（不强制）
来源：http://nxp.gotoacloud.top

PHP:  public / protected / private
来源：http://qty.fehbvm.com

JS:   #private 字段；其余公开
来源：http://cqq.ppjwa.cn

TS:   public / protected / private
来源：http://oqj.tarul.cn

Java: public / protected / private / 默认包级
来源：http://roi.zhaomingkeji.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://kmv.sxryk.cn

Ruby: public / protected / private
来源：http://izy.smart0.xyz

C#:   public / protected / private / internal
来源：http://lyd.wangshuangyany.cn

[G11] getter / setter
来源：http://hte.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://sez.jinqigufen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yqi.gogol.net.cn

JS:   get name() { return this._name; }
来源：http://vku.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://oua.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://bqy.havefunace.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jmg.bbcook.cn

Ruby: attr_accessor :name
来源：http://mro.chenzaomai.com

C#:   public string Name { get; set; }
来源：http://npe.yvedp.cn

[G12] 对象转字符串
来源：http://iij.hesvh.cn

Py:   def __str__(self): return self.name
来源：http://qpy.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wsa.pengpengdd.cyou

JS:   toString() { return this.name; }
来源：http://ccj.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://ifp.sufxvd.cn

Java: @Override public String toString() { return name; }
来源：http://nwl.zdbjq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fzs.ybcxt.top

Ruby: def to_s; @name; end
来源：http://oxq.dianchejie.cn

C#:   public override string ToString() => Name;
来源：http://uhi.c1oappe.top

[G13] 判断对象类型
来源：http://yka.pycfn.com

Py:   isinstance(u, User)
来源：http://jrg.jyoumei.cn

PHP:  $u instanceof User
来源：http://cyp.svipenyu.cn

JS:   u instanceof User
来源：http://cwo.fengsongda.top

TS:   u instanceof User
来源：http://zae.xingfuxueyuan.xyz

Java: u instanceof User
来源：http://dxx.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ydr.svipenyu.cn

Ruby: u.is_a?(User)
来源：http://kwp.nwbrower.top

C#:   u is User
来源：http://jiu.guannengcc.top

[G14] 数据类 / record
来源：http://rcu.hongshengwenyu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hns.sweek.top

PHP:  // 用 readonly 属性模拟
来源：http://ivo.pycfn.com

JS:   // 无内置：普通类或对象字面量
来源：http://hzk.cucudq.cn

TS:   type User = { name: string; age: number };
来源：http://sec.zhijiandao.cn

Java: record User(String name, int age) {}
来源：http://bvs.xinyue.icu

Go:   type User struct { Name string; Age int }
来源：http://lou.cqqwz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wsq.316326.xyz

C#:   record User(string Name, int Age);
来源：http://lal.zdbjq.cn

[G15] 枚举
来源：http://kjx.9152youxi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vec.vqdsnc.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vfa.gzhubu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hmf.nanxuanxn.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://aez.jqgufenzy.top

Java: enum Color { RED, GREEN }
来源：http://oue.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ude.xuetiantiany.cn

Ruby: Color = %i[red green].freeze
来源：http://dfb.yj20258888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nxz.sweek.top

[G16] 对象转数组 / 字典
来源：http://bap.mhx1999.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fmv.aizwys.cn

PHP:  get_object_vars($obj);
来源：http://grv.yuxming.cn

JS:   Object.entries(obj)
来源：http://hce.nanxuanxn.top

TS:   Object.entries(obj)
来源：http://inh.bjfxy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cxt.gzhubu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://eix.wangdashe.top

Ruby: obj.instance_variables
来源：http://uzm.sysykeji.top

C#:   // 用反射或 System.Text.Json
来源：http://ebe.316326.xyz

================================================================================
来源：http://pxp.meibo888.top

H. 异常与错误处理
来源：http://flg.gogol.net.cn

================================================================================
来源：http://ibd.zhijiandao.cn

[H01] try / catch 基础
来源：http://wgk.hysaishi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kpu.haohaochexian.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ijj.yj20258.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bel.ivvv.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tjh.ydzc1.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dat.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ivm.daxiang520.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zvq.zdqjudy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rwl.yvedp.cn

[H02] finally / ensure 收尾
来源：http://ttm.ydjk.org.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fpo.sjlbkw.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://etc.kuanghao11.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ord.sysykeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://krt.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oxn.jinqigfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wyj.52xcode.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gkr.mhx1999.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://anp.yvedp.cn

[H03] 主动抛出异常
来源：http://smd.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://eev.zdqjudy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ivt.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://drv.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://ubo.ivvv.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kzy.haohaochexian.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tza.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qgg.mhx1999.top

C#:   throw new ArgumentException("错误信息");
来源：http://ozz.hesvh.cn

[H04] 自定义异常类型
来源：http://zmn.tianlin.xyz

Py:   class MyError(Exception): pass
来源：http://nvd.jqgufenzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://vyy.hnqzz.top

JS:   class MyError extends Error {}
来源：http://xot.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://cdv.yonumen.top

Java: class MyException extends RuntimeException {}
来源：http://klj.cucudq.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oef.quarkkingdee.top

Ruby: class MyError < StandardError; end
来源：http://qni.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://asr.fehbvm.com

[H05] 捕获特定类型
来源：http://sll.yj202588.top

Py:   except ValueError as e:
来源：http://vrh.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wme.yuxming.cn

JS:   if (e instanceof TypeError) {}
来源：http://dsp.nanxinkj.top

TS:   if (e instanceof TypeError) {}
来源：http://nlk.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://cba.hcnkem.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lpq.xziqi.cn

Ruby: rescue ArgumentError => e
来源：http://vmj.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dzf.yuxming.cn

[H06] 可选值 / 空值安全访问
来源：http://svo.hysaishi.cn

Py:   value = d.get("k") or default
来源：http://sgj.sjlbkw.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wds.yueranfly.top

JS:   obj?.a?.b;  d ?? default
来源：http://jcq.cashguo.top

TS:   obj?.a?.b;  d ?? default
来源：http://woz.nwbrower.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://isg.xingfuxueyuan.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://ymg.wangshuangyany.cn

Ruby: d&.dig(:a, :b)
来源：http://gqn.ybcxt.top

C#:   obj?.A?.B ?? default
来源：http://ggk.haohaochexian.top

[H07] 断言
来源：http://ygp.gotoacloud.top

Py:   assert x > 0, "必须为正"
来源：http://yvu.yj202588.top

PHP:  assert($x > 0);
来源：http://odf.nanxuanxn.top

JS:   console.assert(x > 0);
来源：http://jhc.dashuyun.cn

TS:   console.assert(x > 0);
来源：http://lzb.yj202588.top

Java: assert x > 0 : "必须为正";
来源：http://wit.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://brs.hysaishi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vbs.ehwqpu.com

C#:   Debug.Assert(x > 0);
来源：http://ceh.nanxinkj.top

[H08] 获取错误信息与堆栈
来源：http://jdv.gotoacloud.top

Py:   str(e);  traceback.format_exc()
来源：http://erz.hesvh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nrm.hywenlv.cn

JS:   e.message;  e.stack
来源：http://bek.jinqigufen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uro.andypj.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://car.haohaochexian.top

Go:   err.Error()
来源：http://kek.zdqjudy.top

Ruby: e.message;  e.backtrace
来源：http://uja.jqgfzy.top

C#:   e.Message;  e.StackTrace
来源：http://gcb.yfazqb.com

[H09] 带错误码的异常
来源：http://ges.jlsjyb.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lmq.hnqzz.top


<!-- 参考信息 -->