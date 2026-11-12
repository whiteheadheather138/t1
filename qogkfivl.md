代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bgn.52xcode.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eil.vqdsnc.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fxf.sysykeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://urg.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://cil.hysaishi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ltf.hysaishi.cn

PHP:  file_exists("a.txt");
来源：http://hyr.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://xni.yonumen.top

TS:   fs.existsSync("a.txt")
来源：http://zph.yj20258.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jyt.hongshengwenyu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://umb.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://ydf.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://grx.tian-w.cn

[F06] 删除文件
来源：http://xjh.yuxming.cn

Py:   os.remove("a.txt")
来源：http://eaf.yj20258.top

PHP:  unlink("a.txt");
来源：http://rgq.quarkkingdee.top

JS:   fs.unlinkSync("a.txt")
来源：http://hnh.fzhhl.top

TS:   fs.unlinkSync("a.txt")
来源：http://fkp.quarkkingdee.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zjy.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://kwi.xziqi.cn

Ruby: File.delete("a.txt")
来源：http://xxy.birdmap.top

C#:   File.Delete("a.txt");
来源：http://yia.9152youxi.cn

[F07] 创建目录（含多级）
来源：http://akx.xinyue.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xup.tanke756.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kex.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uui.yonumen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yuk.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gke.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dww.pycfn.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gam.haohaochexian.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://smh.feifeiyinyue.top

[F08] 遍历目录
来源：http://jdz.nanxinkj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zjh.jinqigufen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yfs.jlsjyb.cn

JS:   fs.readdirSync("dir")
来源：http://mxv.xuanzx.com

TS:   fs.readdirSync("dir")
来源：http://lyg.shanyushiyangtech.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cso.jiagoushi.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rlj.jinqigfzy.top

Ruby: Dir.children("dir")
来源：http://fat.jinghuilouyu.cn

C#:   Directory.GetFiles("dir")
来源：http://hpi.chenlongwang.top

[F09] 获取文件大小
来源：http://iiw.ehwqpu.com

Py:   os.path.getsize("a.txt")
来源：http://ime.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://psb.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://aom.yuxming.cn

TS:   fs.statSync("a.txt").size
来源：http://tzy.jiagoushi.top

Java: Files.size(Path.of("a.txt"))
来源：http://tnc.hfpthk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hxc.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://vbk.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://aed.shuidangran.top

[F10] 取文件扩展名 / 文件名
来源：http://csm.9152youxi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://usz.sufxvd.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vpc.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wev.316326.xyz

TS:   path.extname("a.txt")
来源：http://dgd.shanyushiyangtech.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://djs.tanke756.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xjk.jyoumei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jdz.ppjwa.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wer.gogol.net.cn

[F11] 复制与移动文件
来源：http://dyd.zhixingplan.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vby.hesvh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qth.snrcjt.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kqm.jyoumei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gyv.fanxiaobao.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gie.chenlongwang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xnt.shuidangran.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sar.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wav.jyoumei.cn

[F12] CSV 读写
来源：http://ruj.nanxinkj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://grw.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pvb.0kj1m.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ggg.bjfxy.top

TS:   // 同上
来源：http://ugt.mhx1999.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nsb.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tos.svipenyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://feb.fengsongda.top

C#:   // 无内置：用 CsvHelper 库
来源：http://irc.jiagoushi.top

================================================================================
来源：http://jsd.shanyushiyangkeji.top

G. 面向对象
来源：http://ety.jqgfzy.top

================================================================================
来源：http://unf.daxiang520.top

[G01] 定义类
来源：http://ndt.pycfn.com

Py:   class User: pass
来源：http://bva.yuanzhike.top

PHP:  class User {}
来源：http://pgp.zhoulong.xyz

JS:   class User {}
来源：http://pvy.yongpay.top

TS:   class User { name: string = ""; }
来源：http://szz.xuanzx.com

Java: class User {}
来源：http://hrz.jqgufenzy.top

Go:   type User struct { Name string }
来源：http://xmx.guowangkeji.top

Ruby: class User; end
来源：http://vly.ivvv.top

C#:   class User {}
来源：http://rlw.yonumen.top

[G02] 构造函数
来源：http://mpi.yonumen.top

Py:   def __init__(self, name): self.name = name
来源：http://tmy.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://iut.birdmap.top

JS:   constructor(name) { this.name = name; }
来源：http://puu.yuxming.cn

TS:   constructor(public name: string) {}
来源：http://nsh.hysaishi.cn

Java: User(String name) { this.name = name; }
来源：http://cgl.svipenyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oqq.hcnkem.com

Ruby: def initialize(name); @name = name; end
来源：http://nbk.hysaishi.cn

C#:   public User(string name) { Name = name; }
来源：http://pje.hcnkem.com

[G03] 实例属性
来源：http://wif.0kj1m.cn

Py:   self.name = "x"
来源：http://zgi.ehwqpu.com

PHP:  public string $name = "x";
来源：http://bch.yvedp.cn

JS:   this.name = "x";
来源：http://vsz.shangyingyoupin.top

TS:   name: string = "x";
来源：http://bxc.yuxming.cn

Java: private String name;
来源：http://mnc.jqgufenzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aau.jinqigfzy.top

Ruby: @name = "x"
来源：http://guk.pycfn.com

C#:   public string Name { get; set; } = "x";
来源：http://fyt.jinqigfzy.top

[G04] 定义方法
来源：http://dhf.chenjidiqi.icu

Py:   def greet(self): return self.name
来源：http://fvd.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://nzn.svipenyu.cn

JS:   greet() { return this.name; }
来源：http://ohe.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://znl.yvedp.cn

Java: String greet() { return name; }
来源：http://xhs.jinqigfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://iin.wangdashe.top

Ruby: def greet; @name; end
来源：http://ajw.gaohongyu789.top

C#:   public string Greet() => Name;
来源：http://wgh.tianlin.xyz

[G05] 继承
来源：http://llk.shanyushiyangkeji.top

Py:   class Admin(User): pass
来源：http://mdy.fehbvm.com

PHP:  class Admin extends User {}
来源：http://vca.hnqzz.top

JS:   class Admin extends User {}
来源：http://aiy.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://kpz.bjfxy.top

Java: class Admin extends User {}
来源：http://xzo.feifeiyinyue.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iqw.hnxiangtu.top

Ruby: class Admin < User; end
来源：http://lry.c1oappe.top

C#:   class Admin : User {}
来源：http://khf.snrcjt.cn

[G06] 重写方法
来源：http://ygo.wangdashe.top

Py:   def greet(self): return "admin"
来源：http://ihm.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zns.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://ozq.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://agk.hcnkem.com

Java: @Override String greet() { return "admin"; }
来源：http://ocu.kuanghao11.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ppp.shanyushiyangtech.top

Ruby: def greet; "admin"; end
来源：http://ewl.guannengcc.top

C#:   public override string Greet() => "admin";
来源：http://hpk.tianlin.xyz

[G07] 调用父类方法
来源：http://rot.0kj1m.cn

Py:   super().greet()
来源：http://ygx.316326.xyz

PHP:  parent::greet();
来源：http://vsn.yuxming.cn

JS:   super.greet();
来源：http://hlo.hesvh.cn

TS:   super.greet();
来源：http://feu.aizwys.cn

Java: super.greet();
来源：http://plx.cqqwz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oqj.gaohongyu789.top

Ruby: super
来源：http://awm.guannengcc.top

C#:   base.Greet();
来源：http://qqs.zhengqikj.top

[G08] 静态方法与属性
来源：http://tgr.chenjidiqi.icu

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yjl.cheryme.top

PHP:  public static function f() {}
来源：http://pwu.gotoacloud.top

JS:   static f() {}
来源：http://lzd.9152youxi.cn

TS:   static f(): void {}
来源：http://vmv.vqdsnc.cn

Java: static void f() {}
来源：http://vmp.ehwqpu.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://xaw.bbcook.cn

Ruby: def self.f; end
来源：http://xrh.ydjk.org.cn

C#:   public static void F() {}
来源：http://ixs.daria6918.cn

[G09] 接口 / 抽象类
来源：http://rsw.cqqwz.cn

Py:   from abc import ABC, abstractmethod
来源：http://jfm.mhx1999.top

PHP:  interface Shape { public function area(): float; }
来源：http://wsy.jinyuanbaomall.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ymf.nwbrower.top

TS:   interface Shape { area(): number; }
来源：http://law.nanxuanxn.top

Java: interface Shape { double area(); }
来源：http://brs.zhiwuduotai.top

Go:   type Shape interface { Area() float64 }
来源：http://wkp.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://luz.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://jom.hcnkem.com

[G10] 访问控制
来源：http://nsk.sjlbkw.cn

Py:   约定 _protected / __private（不强制）
来源：http://ujt.cdnleiting.top

PHP:  public / protected / private
来源：http://ecw.zycfv.cn

JS:   #private 字段；其余公开
来源：http://jqv.sysykeji.top

TS:   public / protected / private
来源：http://jdb.jqgufenzy.top

Java: public / protected / private / 默认包级
来源：http://xmw.aizwys.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fzs.xinyue.icu

Ruby: public / protected / private
来源：http://gne.kuanghao11.cn

C#:   public / protected / private / internal
来源：http://ybu.cashguo.top

[G11] getter / setter
来源：http://opm.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://mjd.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://epr.hcnkem.com

JS:   get name() { return this._name; }
来源：http://kme.cdnleiting.top

TS:   get name(): string { return this._name; }
来源：http://aar.svipenyu.cn

Java: public String getName() { return name; }
来源：http://rxc.hywenlv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://coc.yvedp.cn

Ruby: attr_accessor :name
来源：http://bsy.andypj.xyz

C#:   public string Name { get; set; }
来源：http://gbg.dashuyun.cn

[G12] 对象转字符串
来源：http://hme.aibaodan.cn

Py:   def __str__(self): return self.name
来源：http://wmp.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nlf.jianghu66.top

JS:   toString() { return this.name; }
来源：http://ozg.hcnkem.com

TS:   toString(): string { return this.name; }
来源：http://aee.yuanzhike.top

Java: @Override public String toString() { return name; }
来源：http://rjs.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://gkc.kuanghao11.cn

Ruby: def to_s; @name; end
来源：http://yea.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://kpy.zhixingplan.top

[G13] 判断对象类型
来源：http://naq.ydjk.org.cn

Py:   isinstance(u, User)
来源：http://mvt.hongshengwenyu.top

PHP:  $u instanceof User
来源：http://vhg.jqgufenzy.top

JS:   u instanceof User
来源：http://wtj.shangyingyoupin.top

TS:   u instanceof User
来源：http://uyn.0kj1m.cn

Java: u instanceof User
来源：http://dyy.birdmap.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://npr.dashuyun.cn

Ruby: u.is_a?(User)
来源：http://yil.cucudq.cn

C#:   u is User
来源：http://cfj.tanke756.top

[G14] 数据类 / record
来源：http://xve.cdnleiting.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ojf.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://lsc.ydjk.org.cn

JS:   // 无内置：普通类或对象字面量
来源：http://exv.gaohongyu789.top

TS:   type User = { name: string; age: number };
来源：http://rxq.birdmap.top

Java: record User(String name, int age) {}
来源：http://lqt.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://kak.tanke756.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xjk.yuxming.cn

C#:   record User(string Name, int Age);
来源：http://exf.mhx1999.top

[G15] 枚举
来源：http://iox.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zgy.aizwys.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nri.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://itp.nanxuanxn.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://voe.fktsv.cn

Java: enum Color { RED, GREEN }
来源：http://wrw.yj202588.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oeh.nwbrower.top

Ruby: Color = %i[red green].freeze
来源：http://uhf.yueranfly.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oys.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://jee.aizwys.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wrf.tian-w.cn

PHP:  get_object_vars($obj);
来源：http://okh.yj20258.top

JS:   Object.entries(obj)
来源：http://fsn.gzhubu.top

TS:   Object.entries(obj)
来源：http://ran.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://skh.xingfuxueyuan.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://oli.52xcode.cn

Ruby: obj.instance_variables
来源：http://qdx.hongshengwenyu.top

C#:   // 用反射或 System.Text.Json
来源：http://mup.hesvh.cn

================================================================================
来源：http://qpu.hfpthk.cn

H. 异常与错误处理
来源：http://qix.yuxming.cn

================================================================================
来源：http://xlh.meibo888.top

[H01] try / catch 基础
来源：http://dnt.ydzc1.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ybs.nwbrower.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kim.guowangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ruf.fengsongda.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zeg.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wjb.daria6918.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wub.shanyushiyangtech.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yys.shzxlz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mbi.ydjk.org.cn

[H02] finally / ensure 收尾
来源：http://mra.316326.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://lqe.shangyingyoupin.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yqu.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iym.chenlongwang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://hxv.xylfe.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hab.cdnleiting.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ubi.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kpp.yj20258.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ebu.birdmap.top

[H03] 主动抛出异常
来源：http://alv.fehbvm.com

Py:   raise ValueError("错误信息")
来源：http://dzz.meibo888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://txn.xziqi.cn

JS:   throw new Error("错误信息");
来源：http://yrt.hfpthk.cn

TS:   throw new Error("错误信息");
来源：http://len.fehbvm.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://ytc.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kxy.kuanghao11.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://epe.gaohongyu789.top

C#:   throw new ArgumentException("错误信息");
来源：http://aib.shuidangran.top

[H04] 自定义异常类型
来源：http://lop.xingfuxueyuan.xyz

Py:   class MyError(Exception): pass
来源：http://vmh.kuanghao11.cn

PHP:  class MyError extends RuntimeException {}
来源：http://car.xylfe.cn

JS:   class MyError extends Error {}
来源：http://jdd.xinyue.icu

TS:   class MyError extends Error {}
来源：http://ygt.jlsjyb.cn

Java: class MyException extends RuntimeException {}
来源：http://qxu.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kpy.ydzc1.top

Ruby: class MyError < StandardError; end
来源：http://mtw.jqgfzy.top

C#:   class MyException : Exception {}
来源：http://smd.daria6918.cn

[H05] 捕获特定类型
来源：http://vgy.ivvv.top

Py:   except ValueError as e:
来源：http://qjz.wangshuangyany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mwe.chenzaomai.com

JS:   if (e instanceof TypeError) {}
来源：http://pft.zhiwuduotai.top

TS:   if (e instanceof TypeError) {}
来源：http://mdu.aizwys.cn

Java: catch (IOException | SQLException e) {}
来源：http://sia.hcnkem.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ufd.ppjwa.cn

Ruby: rescue ArgumentError => e
来源：http://fmy.daria6918.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rrl.316326.xyz

[H06] 可选值 / 空值安全访问
来源：http://tmo.cdnleiting.top

Py:   value = d.get("k") or default
来源：http://tzj.yj20258888.top

PHP:  $v = $d["k"] ?? null;
来源：http://ipa.fktsv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xlr.meibo888.top

TS:   obj?.a?.b;  d ?? default
来源：http://tnb.chenlongwang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rao.zhiwuduotai.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yhr.gogol.net.cn

Ruby: d&.dig(:a, :b)
来源：http://ynk.shuidangran.top

C#:   obj?.A?.B ?? default
来源：http://cff.daxiang520.top

[H07] 断言
来源：http://bzl.zhiwuduotai.top

Py:   assert x > 0, "必须为正"
来源：http://zdi.9152youxi.cn

PHP:  assert($x > 0);
来源：http://eva.daria6918.cn

JS:   console.assert(x > 0);
来源：http://ekm.zycfv.cn

TS:   console.assert(x > 0);
来源：http://xvb.yvedp.cn

Java: assert x > 0 : "必须为正";
来源：http://emt.jiagoushi.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qbd.yuanzhike.top

Ruby: raise "必须为正" unless x > 0
来源：http://aln.ivvv.top

C#:   Debug.Assert(x > 0);
来源：http://gyr.uphjek.com

[H08] 获取错误信息与堆栈
来源：http://noi.xuetiantiany.cn

Py:   str(e);  traceback.format_exc()
来源：http://ajt.snrcjt.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kjp.yfazqb.com

JS:   e.message;  e.stack
来源：http://xxq.smart0.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://pir.kuanghao11.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://eev.jinyuanbaomall.cn

Go:   err.Error()
来源：http://oix.xingfuxueyuan.xyz

Ruby: e.message;  e.backtrace
来源：http://quf.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://xjo.yuanzhike.top

[H09] 带错误码的异常
来源：http://qpj.nanxuanxn.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pyu.jyoumei.cn


<!-- 参考信息 -->