代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nhc.gaohongyu789.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nmt.xinyue.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mfs.jianghu66.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mmq.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qau.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hjq.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jcf.ppjwa.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xnp.yangfankeji.com

[F05] 判断文件或目录是否存在
来源：http://ofx.hongshengwenyu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qze.tarul.cn

PHP:  file_exists("a.txt");
来源：http://svj.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://fzu.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://old.quarkkingdee.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vsp.fengsongda.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://shz.uphjek.com

Ruby: File.exist?("a.txt")
来源：http://uop.chenzaomai.com

C#:   File.Exists("a.txt")
来源：http://xyv.ydzc1.top

[F06] 删除文件
来源：http://cto.wangshuangyany.cn

Py:   os.remove("a.txt")
来源：http://ktc.316326.xyz

PHP:  unlink("a.txt");
来源：http://wqj.yuanzhike.top

JS:   fs.unlinkSync("a.txt")
来源：http://smz.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fyu.jinqigufen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ogt.gotoacloud.top

Go:   os.Remove("a.txt")
来源：http://rxc.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://dfl.daxiang520.top

C#:   File.Delete("a.txt");
来源：http://kys.hesvh.cn

[F07] 创建目录（含多级）
来源：http://xqp.hnqzz.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yjp.sweek.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xrz.chenlongwang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hbc.ivvv.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sil.hysaishi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wrm.dashuyun.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://azp.xuetiantiany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qfz.fengsongda.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ewr.nanxinkj.top

[F08] 遍历目录
来源：http://otp.nanxuanxn.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qzf.hcnkem.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ufd.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://llt.yj20258.top

TS:   fs.readdirSync("dir")
来源：http://fkk.jianghu66.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zww.yvedp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ong.daxiang520.top

Ruby: Dir.children("dir")
来源：http://wjw.316326.xyz

C#:   Directory.GetFiles("dir")
来源：http://lzp.gaohongyu789.top

[F09] 获取文件大小
来源：http://yaf.vehdjk.com

Py:   os.path.getsize("a.txt")
来源：http://ann.316326.xyz

PHP:  filesize("a.txt");
来源：http://zmx.snrcjt.cn

JS:   fs.statSync("a.txt").size
来源：http://lgb.tianlin.xyz

TS:   fs.statSync("a.txt").size
来源：http://jkk.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://qyw.svipenyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lvo.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://qli.xziqi.cn

C#:   new FileInfo("a.txt").Length
来源：http://sju.zhiwuduotai.top

[F10] 取文件扩展名 / 文件名
来源：http://hkp.mhx1999.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ibl.nwbrower.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pzq.ehwqpu.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mee.zhiwuduotai.top

TS:   path.extname("a.txt")
来源：http://rhk.smart0.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tas.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bef.aibaodan.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bns.tanke756.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dgc.zdqjudy.top

[F11] 复制与移动文件
来源：http://xsw.cqqwz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ngu.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vrb.yj202588.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lwx.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zns.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sbu.sxryk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zau.jlsjyb.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://evk.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pud.cdnleiting.top

[F12] CSV 读写
来源：http://wqv.dianchejie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cfm.tarul.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rfg.yueranfly.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://abs.daxiang520.top

TS:   // 同上
来源：http://uua.sjlbkw.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fgr.tanke756.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ppd.hammf.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://faf.pengpengdd.cyou

C#:   // 无内置：用 CsvHelper 库
来源：http://amw.zhengqikj.top

================================================================================
来源：http://pjk.cdnleiting.top

G. 面向对象
来源：http://iew.gaohongyu789.top

================================================================================
来源：http://ehs.cashguo.top

[G01] 定义类
来源：http://bjh.wangshuangyany.cn

Py:   class User: pass
来源：http://kjw.sweek.top

PHP:  class User {}
来源：http://pax.sweek.top

JS:   class User {}
来源：http://tnx.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://tfq.chenjidiqi.icu

Java: class User {}
来源：http://vrz.hammf.cn

Go:   type User struct { Name string }
来源：http://ikj.pycfn.com

Ruby: class User; end
来源：http://pfn.pycfn.com

C#:   class User {}
来源：http://uir.meibo888.top

[G02] 构造函数
来源：http://zds.zhoulong.xyz

Py:   def __init__(self, name): self.name = name
来源：http://zev.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://xph.yj202588.top

JS:   constructor(name) { this.name = name; }
来源：http://nhx.shanyushiyangtech.top

TS:   constructor(public name: string) {}
来源：http://gui.pycfn.com

Java: User(String name) { this.name = name; }
来源：http://ioa.fktsv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ibw.kuanghao11.cn

Ruby: def initialize(name); @name = name; end
来源：http://soz.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://uqy.sufxvd.cn

[G03] 实例属性
来源：http://rbu.uphjek.com

Py:   self.name = "x"
来源：http://vsm.zhixingplan.top

PHP:  public string $name = "x";
来源：http://nnp.fengsongda.top

JS:   this.name = "x";
来源：http://tkt.xuanzx.com

TS:   name: string = "x";
来源：http://rua.yuanzhike.top

Java: private String name;
来源：http://wry.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gtc.xziqi.cn

Ruby: @name = "x"
来源：http://dyw.yj202588.top

C#:   public string Name { get; set; } = "x";
来源：http://gtb.ywan-chungtsiang.top

[G04] 定义方法
来源：http://ezt.snrcjt.cn

Py:   def greet(self): return self.name
来源：http://tgb.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lbz.xingfuxueyuan.xyz

JS:   greet() { return this.name; }
来源：http://fxk.jqgufenzy.top

TS:   greet(): string { return this.name; }
来源：http://toh.yfazqb.com

Java: String greet() { return name; }
来源：http://peq.tarul.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qkl.ppjwa.cn

Ruby: def greet; @name; end
来源：http://eat.cdnleiting.top

C#:   public string Greet() => Name;
来源：http://qkt.cheryme.top

[G05] 继承
来源：http://zmh.jyoumei.cn

Py:   class Admin(User): pass
来源：http://wsu.shuidangran.top

PHP:  class Admin extends User {}
来源：http://qsu.sufxvd.cn

JS:   class Admin extends User {}
来源：http://kxc.shanyushiyangtech.top

TS:   class Admin extends User {}
来源：http://hho.gotoacloud.top

Java: class Admin extends User {}
来源：http://kkf.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://giz.cashguo.top

Ruby: class Admin < User; end
来源：http://gch.ydzc1.top

C#:   class Admin : User {}
来源：http://uln.ivvv.top

[G06] 重写方法
来源：http://yvn.havefunace.top

Py:   def greet(self): return "admin"
来源：http://kmv.mhx1999.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hwy.pengpengdd.cyou

JS:   greet() { return "admin"; }
来源：http://qeb.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://ojt.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://oww.smart0.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wur.cashguo.top

Ruby: def greet; "admin"; end
来源：http://gwt.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://fqh.fktsv.cn

[G07] 调用父类方法
来源：http://ywf.chenjidiqi.icu

Py:   super().greet()
来源：http://jyu.iojbl.cn

PHP:  parent::greet();
来源：http://bcn.yfazqb.com

JS:   super.greet();
来源：http://jtx.daxiang520.top

TS:   super.greet();
来源：http://oas.hnxiangtu.top

Java: super.greet();
来源：http://acp.zhixingplan.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wnv.ywan-chungtsiang.top

Ruby: super
来源：http://mek.fengsongda.top

C#:   base.Greet();
来源：http://fae.zdbjq.cn

[G08] 静态方法与属性
来源：http://lkv.fehbvm.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kgs.ydzc1.top

PHP:  public static function f() {}
来源：http://xhp.bjfxy.top

JS:   static f() {}
来源：http://wfc.chenjidiqi.icu

TS:   static f(): void {}
来源：http://xqa.xziqi.cn

Java: static void f() {}
来源：http://nsd.hfpthk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://plu.gzhubu.top

Ruby: def self.f; end
来源：http://akf.tarul.cn

C#:   public static void F() {}
来源：http://zoc.sxryk.cn

[G09] 接口 / 抽象类
来源：http://fwe.yangfankeji.com

Py:   from abc import ABC, abstractmethod
来源：http://mpr.xuetiantiany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gyd.9152youxi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pww.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://ztn.pengpengdd.cyou

Java: interface Shape { double area(); }
来源：http://hea.nwbrower.top

Go:   type Shape interface { Area() float64 }
来源：http://uwe.zycfv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ytw.ivvv.top

C#:   interface IShape { double Area(); }
来源：http://gph.sufxvd.cn

[G10] 访问控制
来源：http://mmk.zhiwuduotai.top

Py:   约定 _protected / __private（不强制）
来源：http://nta.hcnkem.com

PHP:  public / protected / private
来源：http://jpo.epnwcf.com

JS:   #private 字段；其余公开
来源：http://kpu.jinyuanbaomall.cn

TS:   public / protected / private
来源：http://hoj.daria6918.cn

Java: public / protected / private / 默认包级
来源：http://yyg.jlsjyb.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://asw.kuanghao11.cn

Ruby: public / protected / private
来源：http://phd.epnwcf.com

C#:   public / protected / private / internal
来源：http://fzi.zhongyouzk.top

[G11] getter / setter
来源：http://shg.cheryme.top

Py:   @property 与 @x.setter
来源：http://zft.gotoacloud.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hky.wangdashe.top

JS:   get name() { return this._name; }
来源：http://kxm.yfazqb.com

TS:   get name(): string { return this._name; }
来源：http://bbz.zycfv.cn

Java: public String getName() { return name; }
来源：http://akh.sysykeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mai.daria6918.cn

Ruby: attr_accessor :name
来源：http://apa.epnwcf.com

C#:   public string Name { get; set; }
来源：http://nqa.yueranfly.top

[G12] 对象转字符串
来源：http://frp.ehwqpu.com

Py:   def __str__(self): return self.name
来源：http://eec.cqqwz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sae.hesvh.cn

JS:   toString() { return this.name; }
来源：http://kbf.yanxiufei.cn

TS:   toString(): string { return this.name; }
来源：http://nlt.hysaishi.cn

Java: @Override public String toString() { return name; }
来源：http://jev.xylfe.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ytj.xuetiantiany.cn

Ruby: def to_s; @name; end
来源：http://vbd.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://cta.zhongyouzk.top

[G13] 判断对象类型
来源：http://pdv.xziqi.cn

Py:   isinstance(u, User)
来源：http://snl.ywan-chungtsiang.top

PHP:  $u instanceof User
来源：http://drx.zhaomingkeji.xyz

JS:   u instanceof User
来源：http://brs.cashguo.top

TS:   u instanceof User
来源：http://nza.xuetiantiany.cn

Java: u instanceof User
来源：http://aij.svipenyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vzo.redwolf501.top

Ruby: u.is_a?(User)
来源：http://ivd.shuidangran.top

C#:   u is User
来源：http://faq.nwbrower.top

[G14] 数据类 / record
来源：http://udp.chenlongwang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bln.gotoacloud.top

PHP:  // 用 readonly 属性模拟
来源：http://uba.zhoulong.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://iov.guowangkeji.top

TS:   type User = { name: string; age: number };
来源：http://stg.sjlbkw.cn

Java: record User(String name, int age) {}
来源：http://lvf.gzhubu.top

Go:   type User struct { Name string; Age int }
来源：http://ftd.aizwys.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://guj.jlsjyb.cn

C#:   record User(string Name, int Age);
来源：http://roq.smart0.xyz

[G15] 枚举
来源：http://eyk.fehbvm.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zxk.zhiwuduotai.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nyk.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qlv.bbcook.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gme.jlsjyb.cn

Java: enum Color { RED, GREEN }
来源：http://npb.chenjidiqi.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kpk.zdbjq.cn

Ruby: Color = %i[red green].freeze
来源：http://xvq.hnqzz.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xmd.hfpthk.cn

[G16] 对象转数组 / 字典
来源：http://ghc.shanyushiyangtech.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wkq.jinqigfzy.top

PHP:  get_object_vars($obj);
来源：http://sbz.hfpthk.cn

JS:   Object.entries(obj)
来源：http://uxw.guowangkeji.top

TS:   Object.entries(obj)
来源：http://jbv.zhengqikj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ofm.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://umw.jiagoushi.top

Ruby: obj.instance_variables
来源：http://tsp.shanyushiyangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://hdj.chenzaomai.com

================================================================================
来源：http://rak.jiagoushi.top

H. 异常与错误处理
来源：http://rcg.xylfe.cn

================================================================================
来源：http://mvn.meibo888.top

[H01] try / catch 基础
来源：http://jhx.wangdashe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ahw.tianlin.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nls.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ytm.zhaomingkeji.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ehg.jlsjyb.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nbs.ydjk.org.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xtq.jinghuilouyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qyh.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ziq.cqqwz.cn

[H02] finally / ensure 收尾
来源：http://onj.daxiang520.top

Py:   try: f()⏎finally: cleanup()
来源：http://fqc.sxryk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://eaw.jinghuilouyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://spn.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://iql.tian-w.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jlb.wangshuangyany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oxf.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yyz.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://tsm.dianchejie.cn

[H03] 主动抛出异常
来源：http://nco.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://gfd.cucudq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oby.zdbjq.cn

JS:   throw new Error("错误信息");
来源：http://ssh.dianchejie.cn

TS:   throw new Error("错误信息");
来源：http://noi.yj20258.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bjz.sufxvd.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mkj.cqqwz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vac.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mnu.wangshuangyany.cn

[H04] 自定义异常类型
来源：http://wjf.pengpengdd.cyou

Py:   class MyError(Exception): pass
来源：http://ocd.gogol.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vjy.c1oappe.top

JS:   class MyError extends Error {}
来源：http://mwn.svipenyu.cn

TS:   class MyError extends Error {}
来源：http://uhx.pengpengdd.cyou

Java: class MyException extends RuntimeException {}
来源：http://rym.0kj1m.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zqn.cashguo.top

Ruby: class MyError < StandardError; end
来源：http://dmu.ybcxt.top

C#:   class MyException : Exception {}
来源：http://krm.hcnkem.com

[H05] 捕获特定类型
来源：http://vwb.fengsongda.top

Py:   except ValueError as e:
来源：http://tjs.zhiwuduotai.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zag.ybcxt.top

JS:   if (e instanceof TypeError) {}
来源：http://udo.epnwcf.com

TS:   if (e instanceof TypeError) {}
来源：http://sgb.xinyue.icu

Java: catch (IOException | SQLException e) {}
来源：http://nxc.zdqjudy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zvj.hongshengwenyu.top

Ruby: rescue ArgumentError => e
来源：http://dhq.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hjs.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://aaq.bjfxy.top

Py:   value = d.get("k") or default
来源：http://lpj.sxryk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://spv.jianghu66.top

JS:   obj?.a?.b;  d ?? default
来源：http://gqb.jqgufenzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://vvw.vqdsnc.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uvf.yfazqb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://mdc.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://icl.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://zpq.jinqigufen.top

[H07] 断言
来源：http://rof.hongshengwenyu.top

Py:   assert x > 0, "必须为正"
来源：http://udh.0kj1m.cn

PHP:  assert($x > 0);
来源：http://tvy.zdbjq.cn

JS:   console.assert(x > 0);
来源：http://agl.gogol.net.cn

TS:   console.assert(x > 0);
来源：http://hri.sweek.top

Java: assert x > 0 : "必须为正";
来源：http://ilv.smart0.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gox.shangyingyoupin.top

Ruby: raise "必须为正" unless x > 0
来源：http://cqs.zhiwuduotai.top

C#:   Debug.Assert(x > 0);
来源：http://afp.ydzc1.top

[H08] 获取错误信息与堆栈
来源：http://wvl.cqqwz.cn

Py:   str(e);  traceback.format_exc()
来源：http://eje.birdmap.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kin.gaohongyu789.top

JS:   e.message;  e.stack
来源：http://pvd.gaohongyu789.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zye.9152youxi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lfv.shanyushiyangkeji.top

Go:   err.Error()
来源：http://lei.xinyue.icu


<!-- 参考信息 -->