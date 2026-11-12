代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://btc.havefunace.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kac.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jty.nanxinkj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rhp.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://ovp.hywenlv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dwf.hywenlv.cn

PHP:  file_exists("a.txt");
来源：http://scd.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://dkv.bjfxy.top

TS:   fs.existsSync("a.txt")
来源：http://kjp.yj20258888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qxf.feifeiyinyue.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sdk.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://tay.bbcook.cn

C#:   File.Exists("a.txt")
来源：http://lxy.yj20258.top

[F06] 删除文件
来源：http://rye.ivvv.top

Py:   os.remove("a.txt")
来源：http://zhe.fehbvm.com

PHP:  unlink("a.txt");
来源：http://dol.sufxvd.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rvy.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://hma.nanxuanxn.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://twn.zhongyouzk.top

Go:   os.Remove("a.txt")
来源：http://wru.kuanghao11.cn

Ruby: File.delete("a.txt")
来源：http://gwl.yvedp.cn

C#:   File.Delete("a.txt");
来源：http://ino.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://gvn.daxiang520.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gux.cucudq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lev.andypj.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://owz.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xda.shanyushiyangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jtw.hesvh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gre.nanxuanxn.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fhb.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://crp.zhiwuduotai.top

[F08] 遍历目录
来源：http://jrl.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://acc.c1oappe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gyf.aibaodan.cn

JS:   fs.readdirSync("dir")
来源：http://ygg.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://uem.yj20258888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qqj.hfpthk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zax.nwbrower.top

Ruby: Dir.children("dir")
来源：http://gjg.ctjpmb.com

C#:   Directory.GetFiles("dir")
来源：http://amf.yfazqb.com

[F09] 获取文件大小
来源：http://yfm.hywenlv.cn

Py:   os.path.getsize("a.txt")
来源：http://zvn.yuanzhike.top

PHP:  filesize("a.txt");
来源：http://sjl.xuanzx.com

JS:   fs.statSync("a.txt").size
来源：http://fjy.xylfe.cn

TS:   fs.statSync("a.txt").size
来源：http://rvq.zdqjudy.top

Java: Files.size(Path.of("a.txt"))
来源：http://oup.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cnr.ydzc1.top

Ruby: File.size("a.txt")
来源：http://jag.feifeiyinyue.top

C#:   new FileInfo("a.txt").Length
来源：http://iia.hcnkem.com

[F10] 取文件扩展名 / 文件名
来源：http://qme.jinghuilouyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sej.316326.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gey.zhaomingkeji.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ldu.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://kim.zhongyouzk.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://szi.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rfc.snrcjt.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vae.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bhm.hammf.cn

[F11] 复制与移动文件
来源：http://gim.yanxiufei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ulh.hywenlv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wgx.bjfxy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dos.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yzc.cucudq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hkz.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://isg.yuxming.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ugq.andypj.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zra.hysaishi.cn

[F12] CSV 读写
来源：http://rct.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mld.shanyushiyangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sqw.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ltd.gzhubu.top

TS:   // 同上
来源：http://cxl.xuetiantiany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://geh.yangfankeji.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ipe.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ewq.ehwqpu.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ehb.yuxming.cn

================================================================================
来源：http://ldm.ivvv.top

G. 面向对象
来源：http://faq.hfpthk.cn

================================================================================
来源：http://ksw.fengsongda.top

[G01] 定义类
来源：http://dru.hywenlv.cn

Py:   class User: pass
来源：http://uus.jyoumei.cn

PHP:  class User {}
来源：http://lad.cqqwz.cn

JS:   class User {}
来源：http://bvp.fzhhl.top

TS:   class User { name: string = ""; }
来源：http://tak.ppjwa.cn

Java: class User {}
来源：http://fix.sufxvd.cn

Go:   type User struct { Name string }
来源：http://ukp.xuanzx.com

Ruby: class User; end
来源：http://hne.yj20258888.top

C#:   class User {}
来源：http://wvs.jqgfzy.top

[G02] 构造函数
来源：http://hdj.andypj.xyz

Py:   def __init__(self, name): self.name = name
来源：http://hxv.fzhhl.top

PHP:  public function __construct(public string $name) {}
来源：http://wzh.hfpthk.cn

JS:   constructor(name) { this.name = name; }
来源：http://iwh.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://rfy.tian-w.cn

Java: User(String name) { this.name = name; }
来源：http://nlw.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qpn.yuanzhike.top

Ruby: def initialize(name); @name = name; end
来源：http://ued.zhiwuduotai.top

C#:   public User(string name) { Name = name; }
来源：http://lcd.yonumen.top

[G03] 实例属性
来源：http://tmi.dianchejie.cn

Py:   self.name = "x"
来源：http://xee.yuxming.cn

PHP:  public string $name = "x";
来源：http://ibx.nanxuanxn.top

JS:   this.name = "x";
来源：http://cft.yfazqb.com

TS:   name: string = "x";
来源：http://zgw.bbcook.cn

Java: private String name;
来源：http://ent.feifeiyinyue.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qua.cucudq.cn

Ruby: @name = "x"
来源：http://sjc.fktsv.cn

C#:   public string Name { get; set; } = "x";
来源：http://hhk.yongpay.top

[G04] 定义方法
来源：http://tqz.yuxming.cn

Py:   def greet(self): return self.name
来源：http://ofh.jqgufenzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ilc.zhengqikj.top

JS:   greet() { return this.name; }
来源：http://goh.yongpay.top

TS:   greet(): string { return this.name; }
来源：http://czw.chenjidiqi.icu

Java: String greet() { return name; }
来源：http://nds.xinyue.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://zfn.bbcook.cn

Ruby: def greet; @name; end
来源：http://gyd.zycfv.cn

C#:   public string Greet() => Name;
来源：http://tpk.ivvv.top

[G05] 继承
来源：http://lgy.kuanghao11.cn

Py:   class Admin(User): pass
来源：http://bxt.gzhubu.top

PHP:  class Admin extends User {}
来源：http://slq.yuanzhike.top

JS:   class Admin extends User {}
来源：http://evv.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://dzq.gaohongyu789.top

Java: class Admin extends User {}
来源：http://alt.epnwcf.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oir.hcnkem.com

Ruby: class Admin < User; end
来源：http://wal.yangfankeji.com

C#:   class Admin : User {}
来源：http://zix.tian-w.cn

[G06] 重写方法
来源：http://ard.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://exl.sxryk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sqq.birdmap.top

JS:   greet() { return "admin"; }
来源：http://rnv.sysykeji.top

TS:   greet(): string { return "admin"; }
来源：http://biq.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://uif.zhongyouzk.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://apq.iojbl.cn

Ruby: def greet; "admin"; end
来源：http://oyr.xylfe.cn

C#:   public override string Greet() => "admin";
来源：http://eka.tarul.cn

[G07] 调用父类方法
来源：http://esi.hnxiangtu.top

Py:   super().greet()
来源：http://jdv.xingfuxueyuan.xyz

PHP:  parent::greet();
来源：http://bmm.yj20258888.top

JS:   super.greet();
来源：http://zxg.epnwcf.com

TS:   super.greet();
来源：http://duz.aibaodan.cn

Java: super.greet();
来源：http://too.ydzc1.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pav.zhongyouzk.top

Ruby: super
来源：http://qzs.hywenlv.cn

C#:   base.Greet();
来源：http://fba.svipenyu.cn

[G08] 静态方法与属性
来源：http://ovv.pengpengdd.cyou

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nmg.jqgfzy.top

PHP:  public static function f() {}
来源：http://nwl.ywan-chungtsiang.top

JS:   static f() {}
来源：http://wlu.yj202588.top

TS:   static f(): void {}
来源：http://sbh.cheryme.top

Java: static void f() {}
来源：http://ojf.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://pic.gotoacloud.top

Ruby: def self.f; end
来源：http://anx.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://mbf.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://unf.chenlongwang.top

Py:   from abc import ABC, abstractmethod
来源：http://dnr.shanyushiyangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://ajh.shanyushiyangtech.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rsn.zhaomingkeji.xyz

TS:   interface Shape { area(): number; }
来源：http://wah.wangshuangyany.cn

Java: interface Shape { double area(); }
来源：http://ivh.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://oln.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rss.ydjk.org.cn

C#:   interface IShape { double Area(); }
来源：http://hns.yj20258.top

[G10] 访问控制
来源：http://eaz.mhx1999.top

Py:   约定 _protected / __private（不强制）
来源：http://tcm.jqgfzy.top

PHP:  public / protected / private
来源：http://sah.vqdsnc.cn

JS:   #private 字段；其余公开
来源：http://fnu.9152youxi.cn

TS:   public / protected / private
来源：http://xuw.shzxlz.cn

Java: public / protected / private / 默认包级
来源：http://dqi.hcnkem.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://zut.yj202588.top

Ruby: public / protected / private
来源：http://zxj.yj20258888.top

C#:   public / protected / private / internal
来源：http://hcd.chenzaomai.com

[G11] getter / setter
来源：http://msw.nanxinkj.top

Py:   @property 与 @x.setter
来源：http://smp.yvedp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yjb.nanxinkj.top

JS:   get name() { return this._name; }
来源：http://zxc.tanke756.top

TS:   get name(): string { return this._name; }
来源：http://vsd.jiagoushi.top

Java: public String getName() { return name; }
来源：http://bwu.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bwj.zhoulong.xyz

Ruby: attr_accessor :name
来源：http://rrk.redwolf501.top

C#:   public string Name { get; set; }
来源：http://ksd.jinghuilouyu.cn

[G12] 对象转字符串
来源：http://bio.yvedp.cn

Py:   def __str__(self): return self.name
来源：http://uqc.hcnkem.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://blf.tanke756.top

JS:   toString() { return this.name; }
来源：http://swj.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://lpy.quarkkingdee.top

Java: @Override public String toString() { return name; }
来源：http://kom.0kj1m.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ivs.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://nhq.vehdjk.com

C#:   public override string ToString() => Name;
来源：http://bfr.sweek.top

[G13] 判断对象类型
来源：http://nfl.xingfuxueyuan.xyz

Py:   isinstance(u, User)
来源：http://qld.jinqigufen.top

PHP:  $u instanceof User
来源：http://lvm.smart0.xyz

JS:   u instanceof User
来源：http://afx.ivvv.top

TS:   u instanceof User
来源：http://wgi.ehwqpu.com

Java: u instanceof User
来源：http://mxe.yuanzhike.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dbm.gaohongyu789.top

Ruby: u.is_a?(User)
来源：http://uzz.tianlin.xyz

C#:   u is User
来源：http://rvp.ydjk.org.cn

[G14] 数据类 / record
来源：http://sfc.c1oappe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fvu.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://tuf.hywenlv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kwl.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://sgs.gotoacloud.top

Java: record User(String name, int age) {}
来源：http://gkn.zdqjudy.top

Go:   type User struct { Name string; Age int }
来源：http://zzu.nanxuanxn.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://imk.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://fal.ydzc1.top

[G15] 枚举
来源：http://pms.ydzc1.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hns.tianlin.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://emp.jinqigufen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rgd.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mpl.yj202588.top

Java: enum Color { RED, GREEN }
来源：http://otz.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zcj.vqdsnc.cn

Ruby: Color = %i[red green].freeze
来源：http://ijh.zhixingplan.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cha.yj20258.top

[G16] 对象转数组 / 字典
来源：http://bjj.jyoumei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xaf.sjlbkw.cn

PHP:  get_object_vars($obj);
来源：http://kpc.ppjwa.cn

JS:   Object.entries(obj)
来源：http://yuj.bbcook.cn

TS:   Object.entries(obj)
来源：http://oxn.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hxg.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ybv.fktsv.cn

Ruby: obj.instance_variables
来源：http://snk.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://ytn.xingfuxueyuan.xyz

================================================================================
来源：http://lti.hysaishi.cn

H. 异常与错误处理
来源：http://oyd.redwolf501.top

================================================================================
来源：http://dvw.c1oappe.top

[H01] try / catch 基础
来源：http://buz.yangfankeji.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vwe.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sch.andypj.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dlu.havefunace.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zom.fehbvm.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://klh.gzhubu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iyp.yfazqb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xer.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dqw.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://ssq.tarul.cn

Py:   try: f()⏎finally: cleanup()
来源：http://acz.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gpa.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://bmf.hysaishi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mhh.zycfv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bgt.wangshuangyany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bki.hfpthk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yfr.quarkkingdee.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xel.zhijiandao.cn

[H03] 主动抛出异常
来源：http://fyh.yfazqb.com

Py:   raise ValueError("错误信息")
来源：http://acz.yongpay.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://naa.nwbrower.top

JS:   throw new Error("错误信息");
来源：http://iij.tian-w.cn

TS:   throw new Error("错误信息");
来源：http://rgo.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nrx.hfpthk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://idx.bbcook.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dbi.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://mjj.ctjpmb.com

[H04] 自定义异常类型
来源：http://twb.shzxlz.cn

Py:   class MyError(Exception): pass
来源：http://cjw.jianghu66.top

PHP:  class MyError extends RuntimeException {}
来源：http://hpy.cashguo.top

JS:   class MyError extends Error {}
来源：http://gqz.yanxiufei.cn

TS:   class MyError extends Error {}
来源：http://zfc.hcnkem.com

Java: class MyException extends RuntimeException {}
来源：http://xlq.52xcode.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lgn.c1oappe.top

Ruby: class MyError < StandardError; end
来源：http://jmd.shuidangran.top

C#:   class MyException : Exception {}
来源：http://hca.chenjidiqi.icu

[H05] 捕获特定类型
来源：http://ssp.epnwcf.com

Py:   except ValueError as e:
来源：http://bbn.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yqo.hnxiangtu.top

JS:   if (e instanceof TypeError) {}
来源：http://xcp.xziqi.cn

TS:   if (e instanceof TypeError) {}
来源：http://ers.sweek.top

Java: catch (IOException | SQLException e) {}
来源：http://cha.sjlbkw.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xhy.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://grr.yueranfly.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yim.shanyushiyangtech.top

[H06] 可选值 / 空值安全访问
来源：http://sxw.sufxvd.cn

Py:   value = d.get("k") or default
来源：http://tbv.9152youxi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pib.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://wjt.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://vwg.pengpengdd.cyou

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qfc.ehwqpu.com

Go:   if v, ok := m["k"]; ok { }
来源：http://jaj.meibo888.top

Ruby: d&.dig(:a, :b)
来源：http://kux.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://xrq.ybcxt.top

[H07] 断言
来源：http://czl.cheryme.top

Py:   assert x > 0, "必须为正"
来源：http://avj.ctjpmb.com

PHP:  assert($x > 0);
来源：http://pjv.fehbvm.com

JS:   console.assert(x > 0);
来源：http://knc.bjfxy.top

TS:   console.assert(x > 0);
来源：http://isj.jinyuanbaomall.cn

Java: assert x > 0 : "必须为正";
来源：http://vvh.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uyd.yangfankeji.com

Ruby: raise "必须为正" unless x > 0
来源：http://nvd.yonumen.top

C#:   Debug.Assert(x > 0);
来源：http://zwu.zhiwuduotai.top

[H08] 获取错误信息与堆栈
来源：http://qgs.bbcook.cn

Py:   str(e);  traceback.format_exc()
来源：http://rgb.nwbrower.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ehi.cheryme.top

JS:   e.message;  e.stack
来源：http://ijg.fengsongda.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ttg.zhongyouzk.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jty.gzhubu.top

Go:   err.Error()
来源：http://wsn.bjfxy.top

Ruby: e.message;  e.backtrace
来源：http://jxe.zhiwuduotai.top

C#:   e.Message;  e.StackTrace
来源：http://npu.ctjpmb.com

[H09] 带错误码的异常
来源：http://zxs.yongpay.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mdu.tian-w.cn


<!-- 参考信息 -->