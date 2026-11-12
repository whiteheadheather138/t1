代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aat.hongshengwenyu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xho.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://txs.nanxinkj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iay.fktsv.cn

[F05] 判断文件或目录是否存在
来源：http://bjg.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gec.fengsongda.top

PHP:  file_exists("a.txt");
来源：http://pki.cdnleiting.top

JS:   fs.existsSync("a.txt")
来源：http://oai.fehbvm.com

TS:   fs.existsSync("a.txt")
来源：http://cjc.yueranfly.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tsu.pengpengdd.cyou

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qfv.jqgufenzy.top

Ruby: File.exist?("a.txt")
来源：http://fne.cdnleiting.top

C#:   File.Exists("a.txt")
来源：http://jnu.cqqwz.cn

[F06] 删除文件
来源：http://cds.hcnkem.com

Py:   os.remove("a.txt")
来源：http://tah.yfazqb.com

PHP:  unlink("a.txt");
来源：http://tip.andypj.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://ymq.yj20258.top

TS:   fs.unlinkSync("a.txt")
来源：http://kvk.nanxuanxn.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ihl.shzxlz.cn

Go:   os.Remove("a.txt")
来源：http://cqg.xuanzx.com

Ruby: File.delete("a.txt")
来源：http://hwr.andypj.xyz

C#:   File.Delete("a.txt");
来源：http://ulo.sxryk.cn

[F07] 创建目录（含多级）
来源：http://btv.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xul.sxryk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cap.chenzaomai.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gbk.gogol.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zxj.daria6918.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yvh.hammf.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uuh.xinyue.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nec.iojbl.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kpd.ehwqpu.com

[F08] 遍历目录
来源：http://pfz.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://luv.yangfankeji.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rba.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://fgw.shangyingyoupin.top

TS:   fs.readdirSync("dir")
来源：http://jzy.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ciw.hnxiangtu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xxw.yj20258.top

Ruby: Dir.children("dir")
来源：http://gjh.shanyushiyangtech.top

C#:   Directory.GetFiles("dir")
来源：http://kvt.zhiwuduotai.top

[F09] 获取文件大小
来源：http://dtr.yuxming.cn

Py:   os.path.getsize("a.txt")
来源：http://xak.jlsjyb.cn

PHP:  filesize("a.txt");
来源：http://lue.sysykeji.top

JS:   fs.statSync("a.txt").size
来源：http://nlr.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://ayu.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cqm.hysaishi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://app.yj20258.top

Ruby: File.size("a.txt")
来源：http://muq.jqgufenzy.top

C#:   new FileInfo("a.txt").Length
来源：http://whe.zdqjudy.top

[F10] 取文件扩展名 / 文件名
来源：http://wxo.cashguo.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ecl.sjlbkw.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://utw.ydjk.org.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lsi.quarkkingdee.top

TS:   path.extname("a.txt")
来源：http://mzv.fktsv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blj.jinqigufen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vnk.ehwqpu.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zqn.9152youxi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wus.redwolf501.top

[F11] 复制与移动文件
来源：http://hhm.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ama.birdmap.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vpx.guannengcc.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://scs.hysaishi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cfq.ydzc1.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hvc.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://btb.zdqjudy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mdh.vqdsnc.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gtv.xuetiantiany.cn

[F12] CSV 读写
来源：http://rff.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ibq.feifeiyinyue.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ugq.hesvh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sga.hnqzz.top

TS:   // 同上
来源：http://wkl.yangfankeji.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qrv.tarul.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://guf.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tii.fzhhl.top

C#:   // 无内置：用 CsvHelper 库
来源：http://goa.0kj1m.cn

================================================================================
来源：http://sta.zhongyouzk.top

G. 面向对象
来源：http://lbu.ehwqpu.com

================================================================================
来源：http://gzq.ydzc1.top

[G01] 定义类
来源：http://max.yj20258888.top

Py:   class User: pass
来源：http://xpr.gogol.net.cn

PHP:  class User {}
来源：http://uox.yanxiufei.cn

JS:   class User {}
来源：http://mce.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://bix.jinqigufen.top

Java: class User {}
来源：http://eru.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://bpm.ywan-chungtsiang.top

Ruby: class User; end
来源：http://zds.yj20258888.top

C#:   class User {}
来源：http://nyd.hnqzz.top

[G02] 构造函数
来源：http://mco.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://gfs.fanxiaobao.xyz

PHP:  public function __construct(public string $name) {}
来源：http://stq.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://tqs.tanke756.top

TS:   constructor(public name: string) {}
来源：http://jbf.ehwqpu.com

Java: User(String name) { this.name = name; }
来源：http://ess.guowangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ali.meibo888.top

Ruby: def initialize(name); @name = name; end
来源：http://jnl.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://scm.aizwys.cn

[G03] 实例属性
来源：http://alr.xingfuxueyuan.xyz

Py:   self.name = "x"
来源：http://orh.yonumen.top

PHP:  public string $name = "x";
来源：http://gyf.fktsv.cn

JS:   this.name = "x";
来源：http://vvr.shuidangran.top

TS:   name: string = "x";
来源：http://qtr.fzhhl.top

Java: private String name;
来源：http://jks.yangfankeji.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eoh.chenlongwang.top

Ruby: @name = "x"
来源：http://pan.mhx1999.top

C#:   public string Name { get; set; } = "x";
来源：http://ujw.zycfv.cn

[G04] 定义方法
来源：http://fwx.shzxlz.cn

Py:   def greet(self): return self.name
来源：http://lsj.fzhhl.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wzq.pycfn.com

JS:   greet() { return this.name; }
来源：http://kbi.sufxvd.cn

TS:   greet(): string { return this.name; }
来源：http://wcu.zhengqikj.top

Java: String greet() { return name; }
来源：http://otx.yvedp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lhw.zhongyouzk.top

Ruby: def greet; @name; end
来源：http://edv.hnqzz.top

C#:   public string Greet() => Name;
来源：http://gio.redwolf501.top

[G05] 继承
来源：http://qxy.bbcook.cn

Py:   class Admin(User): pass
来源：http://myl.cqqwz.cn

PHP:  class Admin extends User {}
来源：http://kzo.meibo888.top

JS:   class Admin extends User {}
来源：http://yqm.nwbrower.top

TS:   class Admin extends User {}
来源：http://ini.hcnkem.com

Java: class Admin extends User {}
来源：http://vtf.cdnleiting.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yxd.havefunace.top

Ruby: class Admin < User; end
来源：http://mna.zhixingplan.top

C#:   class Admin : User {}
来源：http://qcb.cucudq.cn

[G06] 重写方法
来源：http://tro.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://acq.tianlin.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://wcy.tianlin.xyz

JS:   greet() { return "admin"; }
来源：http://urh.mhx1999.top

TS:   greet(): string { return "admin"; }
来源：http://jki.svipenyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://ceq.sjlbkw.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kxo.jqgufenzy.top

Ruby: def greet; "admin"; end
来源：http://qcq.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://cfo.cheryme.top

[G07] 调用父类方法
来源：http://qwe.kuanghao11.cn

Py:   super().greet()
来源：http://tzn.jiagoushi.top

PHP:  parent::greet();
来源：http://mod.cashguo.top

JS:   super.greet();
来源：http://ipz.jqgfzy.top

TS:   super.greet();
来源：http://cda.kuanghao11.cn

Java: super.greet();
来源：http://aeg.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xbp.wangdashe.top

Ruby: super
来源：http://aay.svipenyu.cn

C#:   base.Greet();
来源：http://sog.ydzc1.top

[G08] 静态方法与属性
来源：http://gjl.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ouh.xinyue.icu

PHP:  public static function f() {}
来源：http://kej.yj20258888.top

JS:   static f() {}
来源：http://rqb.sysykeji.top

TS:   static f(): void {}
来源：http://man.daria6918.cn

Java: static void f() {}
来源：http://ntw.zycfv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lcm.xinyue.icu

Ruby: def self.f; end
来源：http://irc.jinghuilouyu.cn

C#:   public static void F() {}
来源：http://ayr.zdqjudy.top

[G09] 接口 / 抽象类
来源：http://dka.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://wgo.hysaishi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oex.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kwe.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://uht.dianchejie.cn

Java: interface Shape { double area(); }
来源：http://git.cqqwz.cn

Go:   type Shape interface { Area() float64 }
来源：http://aya.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fee.redwolf501.top

C#:   interface IShape { double Area(); }
来源：http://vfd.sweek.top

[G10] 访问控制
来源：http://ffe.shzxlz.cn

Py:   约定 _protected / __private（不强制）
来源：http://xbu.zdqjudy.top

PHP:  public / protected / private
来源：http://izi.bjfxy.top

JS:   #private 字段；其余公开
来源：http://kwz.yfazqb.com

TS:   public / protected / private
来源：http://rgf.gogol.net.cn

Java: public / protected / private / 默认包级
来源：http://ldu.xylfe.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zjv.bbcook.cn

Ruby: public / protected / private
来源：http://jha.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://imb.birdmap.top

[G11] getter / setter
来源：http://saz.tarul.cn

Py:   @property 与 @x.setter
来源：http://ynq.ivvv.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sai.shzxlz.cn

JS:   get name() { return this._name; }
来源：http://nmb.pycfn.com

TS:   get name(): string { return this._name; }
来源：http://eik.daxiang520.top

Java: public String getName() { return name; }
来源：http://dir.vqdsnc.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uoe.jiagoushi.top

Ruby: attr_accessor :name
来源：http://ivf.ybcxt.top

C#:   public string Name { get; set; }
来源：http://tvl.meibo888.top

[G12] 对象转字符串
来源：http://ucd.chenjidiqi.icu

Py:   def __str__(self): return self.name
来源：http://voq.nanxinkj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ket.chenjidiqi.icu

JS:   toString() { return this.name; }
来源：http://gte.aizwys.cn

TS:   toString(): string { return this.name; }
来源：http://dbk.fehbvm.com

Java: @Override public String toString() { return name; }
来源：http://fuj.hnqzz.top

Go:   func (u User) String() string { return u.Name }
来源：http://tzj.nanxinkj.top

Ruby: def to_s; @name; end
来源：http://ait.dianchejie.cn

C#:   public override string ToString() => Name;
来源：http://gzy.hesvh.cn

[G13] 判断对象类型
来源：http://tqw.ywan-chungtsiang.top

Py:   isinstance(u, User)
来源：http://oaf.jyoumei.cn

PHP:  $u instanceof User
来源：http://ptb.jiagoushi.top

JS:   u instanceof User
来源：http://ibf.316326.xyz

TS:   u instanceof User
来源：http://twu.cucudq.cn

Java: u instanceof User
来源：http://iyu.sysykeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kvy.zhijiandao.cn

Ruby: u.is_a?(User)
来源：http://qff.jinqigfzy.top

C#:   u is User
来源：http://hku.9152youxi.cn

[G14] 数据类 / record
来源：http://pgq.hcnkem.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qtb.shzxlz.cn

PHP:  // 用 readonly 属性模拟
来源：http://nav.bjfxy.top

JS:   // 无内置：普通类或对象字面量
来源：http://auo.jqgufenzy.top

TS:   type User = { name: string; age: number };
来源：http://aof.smart0.xyz

Java: record User(String name, int age) {}
来源：http://ixe.hnqzz.top

Go:   type User struct { Name string; Age int }
来源：http://nal.zhaomingkeji.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rkg.dashuyun.cn

C#:   record User(string Name, int Age);
来源：http://ooo.hnxiangtu.top

[G15] 枚举
来源：http://vty.bjfxy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ohp.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dhn.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jov.meibo888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bij.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://wkx.fehbvm.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mow.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://xdx.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wvg.hesvh.cn

[G16] 对象转数组 / 字典
来源：http://faf.sjlbkw.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eez.sysykeji.top

PHP:  get_object_vars($obj);
来源：http://qox.sufxvd.cn

JS:   Object.entries(obj)
来源：http://vjq.chenzaomai.com

TS:   Object.entries(obj)
来源：http://wrh.gzhubu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ajw.xylfe.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pzz.zhengqikj.top

Ruby: obj.instance_variables
来源：http://muj.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://cnj.yangfankeji.com

================================================================================
来源：http://goe.yj202588.top

H. 异常与错误处理
来源：http://mbu.ctjpmb.com

================================================================================
来源：http://nkh.jqgufenzy.top

[H01] try / catch 基础
来源：http://hvb.shanyushiyangtech.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gdz.jinqigufen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eud.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tqm.fktsv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bii.jlsjyb.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wxl.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sob.shanyushiyangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hyh.hesvh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rmv.yj20258.top

[H02] finally / ensure 收尾
来源：http://zfj.tanke756.top

Py:   try: f()⏎finally: cleanup()
来源：http://vdq.bjfxy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vjw.zhaomingkeji.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://ysh.smart0.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://mue.ehwqpu.com

Java: try { f(); } finally { cleanup(); }
来源：http://saq.zhongyouzk.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bjp.zycfv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xsi.hongshengwenyu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fmd.zhaomingkeji.xyz

[H03] 主动抛出异常
来源：http://kgg.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://wmr.pengpengdd.cyou

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fsn.hongshengwenyu.top

JS:   throw new Error("错误信息");
来源：http://hac.gogol.net.cn

TS:   throw new Error("错误信息");
来源：http://ith.wangshuangyany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dgr.yongpay.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pij.9152youxi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tcm.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fuc.nanxuanxn.top

[H04] 自定义异常类型
来源：http://ske.tanke756.top

Py:   class MyError(Exception): pass
来源：http://fmt.yfazqb.com

PHP:  class MyError extends RuntimeException {}
来源：http://tjm.shanyushiyangkeji.top

JS:   class MyError extends Error {}
来源：http://ddo.snrcjt.cn

TS:   class MyError extends Error {}
来源：http://upg.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://yrt.havefunace.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xxu.ctjpmb.com

Ruby: class MyError < StandardError; end
来源：http://lrv.guannengcc.top

C#:   class MyException : Exception {}
来源：http://qqp.ybcxt.top

[H05] 捕获特定类型
来源：http://lnn.wangdashe.top

Py:   except ValueError as e:
来源：http://hjy.ppjwa.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lxe.chenjidiqi.icu

JS:   if (e instanceof TypeError) {}
来源：http://jjt.ywan-chungtsiang.top

TS:   if (e instanceof TypeError) {}
来源：http://iep.yueranfly.top

Java: catch (IOException | SQLException e) {}
来源：http://ppv.zhixingplan.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iku.yfazqb.com

Ruby: rescue ArgumentError => e
来源：http://xkz.tarul.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dih.birdmap.top

[H06] 可选值 / 空值安全访问
来源：http://fnz.cdnleiting.top

Py:   value = d.get("k") or default
来源：http://nlq.zdbjq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://aph.sjlbkw.cn

JS:   obj?.a?.b;  d ?? default
来源：http://niv.jinyuanbaomall.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ghx.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://omb.jlsjyb.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nqh.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://wws.sweek.top

C#:   obj?.A?.B ?? default
来源：http://scg.gzhubu.top

[H07] 断言
来源：http://liu.dianchejie.cn

Py:   assert x > 0, "必须为正"
来源：http://jty.ehwqpu.com

PHP:  assert($x > 0);
来源：http://ctn.hnqzz.top

JS:   console.assert(x > 0);
来源：http://xgb.dashuyun.cn

TS:   console.assert(x > 0);
来源：http://mbo.fanxiaobao.xyz

Java: assert x > 0 : "必须为正";
来源：http://iuh.shangyingyoupin.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ddg.tanke756.top

Ruby: raise "必须为正" unless x > 0
来源：http://ruy.quarkkingdee.top

C#:   Debug.Assert(x > 0);
来源：http://ylc.iojbl.cn

[H08] 获取错误信息与堆栈
来源：http://wqw.gzhubu.top

Py:   str(e);  traceback.format_exc()
来源：http://lki.zhaomingkeji.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bow.shanyushiyangtech.top

JS:   e.message;  e.stack
来源：http://emv.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://eau.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zrn.yangfankeji.com

Go:   err.Error()
来源：http://lmu.aibaodan.cn

Ruby: e.message;  e.backtrace
来源：http://bps.andypj.xyz

C#:   e.Message;  e.StackTrace
来源：http://hpf.sufxvd.cn

[H09] 带错误码的异常
来源：http://fpk.tian-w.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://usq.jinyuanbaomall.cn


<!-- 参考信息 -->