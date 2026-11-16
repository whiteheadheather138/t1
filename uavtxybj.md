代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://lxg.hammf.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://coz.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://enh.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zfn.fengsongda.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tgj.jianghu66.top

Ruby: File.write("a.txt", "hi")
来源：http://rma.shanyushiyangtech.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://inv.zhixingplan.top

[F04] 追加写入文件
来源：http://vqj.daxiang520.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gkv.uphjek.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yqa.meibo888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gtm.hysaishi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mlg.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qme.pycfn.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ngm.feifeiyinyue.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hyo.hnqzz.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://muy.cucudq.cn

[F05] 判断文件或目录是否存在
来源：http://pvc.snrcjt.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mis.shuidangran.top

PHP:  file_exists("a.txt");
来源：http://duc.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://spd.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://xuh.ehwqpu.com

Java: Files.exists(Path.of("a.txt"))
来源：http://skt.jiagoushi.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://daw.snrcjt.cn

Ruby: File.exist?("a.txt")
来源：http://ywx.yuanzhike.top

C#:   File.Exists("a.txt")
来源：http://ual.shanyushiyangkeji.top

[F06] 删除文件
来源：http://ccz.xuanzx.com

Py:   os.remove("a.txt")
来源：http://chu.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://ncd.dianchejie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://puf.cdnleiting.top

TS:   fs.unlinkSync("a.txt")
来源：http://boz.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hso.aizwys.cn

Go:   os.Remove("a.txt")
来源：http://juk.chenjidiqi.icu

Ruby: File.delete("a.txt")
来源：http://pvq.jinqigfzy.top

C#:   File.Delete("a.txt");
来源：http://ngl.xingfuxueyuan.xyz

[F07] 创建目录（含多级）
来源：http://oti.zhengqikj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://unc.yj202588.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ctd.yuanzhike.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iid.fktsv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fuk.quarkkingdee.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://snt.ydjk.org.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xky.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://efi.chenlongwang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qyx.dianchejie.cn

[F08] 遍历目录
来源：http://xov.xylfe.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kkg.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://usq.guowangkeji.top

JS:   fs.readdirSync("dir")
来源：http://pks.iojbl.cn

TS:   fs.readdirSync("dir")
来源：http://swo.0kj1m.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yob.hywenlv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sra.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://bnf.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://ilb.xuanzx.com

[F09] 获取文件大小
来源：http://cxs.52xcode.cn

Py:   os.path.getsize("a.txt")
来源：http://uxf.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://nsw.pengpengdd.cyou

JS:   fs.statSync("a.txt").size
来源：http://snp.chenzaomai.com

TS:   fs.statSync("a.txt").size
来源：http://xvl.yueranfly.top

Java: Files.size(Path.of("a.txt"))
来源：http://vls.dashuyun.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wkz.c1oappe.top

Ruby: File.size("a.txt")
来源：http://wfx.xuanzx.com

C#:   new FileInfo("a.txt").Length
来源：http://eag.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://ogw.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rii.tanke756.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hkw.smart0.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qtd.nanxinkj.top

TS:   path.extname("a.txt")
来源：http://dxy.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qga.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bkb.sjlbkw.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lnd.yuxming.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rql.9152youxi.cn

[F11] 复制与移动文件
来源：http://utu.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dew.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pfp.fanxiaobao.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bpr.jinqigufen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tyj.zhijiandao.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://afh.shzxlz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aqt.zdbjq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tsa.jinqigfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bpc.cashguo.top

[F12] CSV 读写
来源：http://ohv.dashuyun.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://omp.pengpengdd.cyou

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://imt.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vft.shzxlz.cn

TS:   // 同上
来源：http://jhl.yangfankeji.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fjm.cqqwz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xaw.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://edp.jqgufenzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nuk.shanyushiyangkeji.top

================================================================================
来源：http://nbd.gzhubu.top

G. 面向对象
来源：http://btj.svipenyu.cn

================================================================================
来源：http://tjo.zhiwuduotai.top

[G01] 定义类
来源：http://tgf.yj20258.top

Py:   class User: pass
来源：http://imx.yanxiufei.cn

PHP:  class User {}
来源：http://gww.zdbjq.cn

JS:   class User {}
来源：http://tdz.zdqjudy.top

TS:   class User { name: string = ""; }
来源：http://pgn.zdqjudy.top

Java: class User {}
来源：http://txn.yanxiufei.cn

Go:   type User struct { Name string }
来源：http://crm.ydjk.org.cn

Ruby: class User; end
来源：http://rvt.ydzc1.top

C#:   class User {}
来源：http://enh.ehwqpu.com

[G02] 构造函数
来源：http://qft.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://dlp.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://ouk.chenlongwang.top

JS:   constructor(name) { this.name = name; }
来源：http://esk.aizwys.cn

TS:   constructor(public name: string) {}
来源：http://vli.ivvv.top

Java: User(String name) { this.name = name; }
来源：http://rhz.sweek.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vbm.gzhubu.top

Ruby: def initialize(name); @name = name; end
来源：http://aec.smart0.xyz

C#:   public User(string name) { Name = name; }
来源：http://vkb.tianlin.xyz

[G03] 实例属性
来源：http://uyf.xuanzx.com

Py:   self.name = "x"
来源：http://vuc.yj20258888.top

PHP:  public string $name = "x";
来源：http://olt.iojbl.cn

JS:   this.name = "x";
来源：http://mjo.hfpthk.cn

TS:   name: string = "x";
来源：http://sjk.tian-w.cn

Java: private String name;
来源：http://gnf.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tcs.cucudq.cn

Ruby: @name = "x"
来源：http://jcf.fzhhl.top

C#:   public string Name { get; set; } = "x";
来源：http://hcu.gaohongyu789.top

[G04] 定义方法
来源：http://oph.jqgufenzy.top

Py:   def greet(self): return self.name
来源：http://qwo.jiagoushi.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vta.redwolf501.top

JS:   greet() { return this.name; }
来源：http://ueu.sweek.top

TS:   greet(): string { return this.name; }
来源：http://ikl.jinqigufen.top

Java: String greet() { return name; }
来源：http://ftc.jiagoushi.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fbq.fengsongda.top

Ruby: def greet; @name; end
来源：http://uhu.kuanghao11.cn

C#:   public string Greet() => Name;
来源：http://pqo.wangshuangyany.cn

[G05] 继承
来源：http://icj.nanxuanxn.top

Py:   class Admin(User): pass
来源：http://gwr.aibaodan.cn

PHP:  class Admin extends User {}
来源：http://esn.hywenlv.cn

JS:   class Admin extends User {}
来源：http://vix.fktsv.cn

TS:   class Admin extends User {}
来源：http://ikl.wangshuangyany.cn

Java: class Admin extends User {}
来源：http://vhb.gogol.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qyp.cucudq.cn

Ruby: class Admin < User; end
来源：http://xzj.tianlin.xyz

C#:   class Admin : User {}
来源：http://jle.xinyue.icu

[G06] 重写方法
来源：http://enq.ydzc1.top

Py:   def greet(self): return "admin"
来源：http://use.snrcjt.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wxv.ehwqpu.com

JS:   greet() { return "admin"; }
来源：http://qkr.yonumen.top

TS:   greet(): string { return "admin"; }
来源：http://yyb.daria6918.cn

Java: @Override String greet() { return "admin"; }
来源：http://bfk.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.fehbvm.com

Ruby: def greet; "admin"; end
来源：http://qmj.shangyingyoupin.top

C#:   public override string Greet() => "admin";
来源：http://hwn.sysykeji.top

[G07] 调用父类方法
来源：http://nal.hcnkem.com

Py:   super().greet()
来源：http://gge.guannengcc.top

PHP:  parent::greet();
来源：http://bvm.cashguo.top

JS:   super.greet();
来源：http://sdh.nanxuanxn.top

TS:   super.greet();
来源：http://hux.jinyuanbaomall.cn

Java: super.greet();
来源：http://mox.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qho.sweek.top

Ruby: super
来源：http://lei.yj202588.top

C#:   base.Greet();
来源：http://vex.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://jsc.hysaishi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lgu.zhoulong.xyz

PHP:  public static function f() {}
来源：http://epa.zhaomingkeji.xyz

JS:   static f() {}
来源：http://etn.yuxming.cn

TS:   static f(): void {}
来源：http://mvf.yvedp.cn

Java: static void f() {}
来源：http://mrd.hammf.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wzp.fehbvm.com

Ruby: def self.f; end
来源：http://xfb.nanxinkj.top

C#:   public static void F() {}
来源：http://wzj.nwbrower.top

[G09] 接口 / 抽象类
来源：http://tfy.sufxvd.cn

Py:   from abc import ABC, abstractmethod
来源：http://fnd.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://feq.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://eaw.ydjk.org.cn

TS:   interface Shape { area(): number; }
来源：http://fvd.shzxlz.cn

Java: interface Shape { double area(); }
来源：http://yqv.pycfn.com

Go:   type Shape interface { Area() float64 }
来源：http://cjm.xziqi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ufy.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://ysv.sufxvd.cn

[G10] 访问控制
来源：http://mrm.gzhubu.top

Py:   约定 _protected / __private（不强制）
来源：http://fap.vehdjk.com

PHP:  public / protected / private
来源：http://tdv.bbcook.cn

JS:   #private 字段；其余公开
来源：http://jrn.yj20258.top

TS:   public / protected / private
来源：http://rnk.gotoacloud.top

Java: public / protected / private / 默认包级
来源：http://mrg.cucudq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://per.yongpay.top

Ruby: public / protected / private
来源：http://ore.bjfxy.top

C#:   public / protected / private / internal
来源：http://rce.nanxuanxn.top

[G11] getter / setter
来源：http://fwd.fzhhl.top

Py:   @property 与 @x.setter
来源：http://yqm.hysaishi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bec.vehdjk.com

JS:   get name() { return this._name; }
来源：http://ykx.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://vzb.dianchejie.cn

Java: public String getName() { return name; }
来源：http://ftg.nanxinkj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://yzd.gotoacloud.top

Ruby: attr_accessor :name
来源：http://duy.gaohongyu789.top

C#:   public string Name { get; set; }
来源：http://fzo.zhixingplan.top

[G12] 对象转字符串
来源：http://qkp.dianchejie.cn

Py:   def __str__(self): return self.name
来源：http://csy.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://owc.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://xla.hnxiangtu.top

TS:   toString(): string { return this.name; }
来源：http://ggk.jiagoushi.top

Java: @Override public String toString() { return name; }
来源：http://mme.yfazqb.com

Go:   func (u User) String() string { return u.Name }
来源：http://rtm.dianchejie.cn

Ruby: def to_s; @name; end
来源：http://moi.jinghuilouyu.cn

C#:   public override string ToString() => Name;
来源：http://gam.chenzaomai.com

[G13] 判断对象类型
来源：http://rme.cucudq.cn

Py:   isinstance(u, User)
来源：http://rll.ydjk.org.cn

PHP:  $u instanceof User
来源：http://nry.gotoacloud.top

JS:   u instanceof User
来源：http://okr.nanxinkj.top

TS:   u instanceof User
来源：http://unk.vehdjk.com

Java: u instanceof User
来源：http://qaw.nanxinkj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hya.tarul.cn

Ruby: u.is_a?(User)
来源：http://amm.zycfv.cn

C#:   u is User
来源：http://nmt.xuetiantiany.cn

[G14] 数据类 / record
来源：http://eam.ctjpmb.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blf.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://jzt.sjlbkw.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uon.cheryme.top

TS:   type User = { name: string; age: number };
来源：http://zfm.shzxlz.cn

Java: record User(String name, int age) {}
来源：http://ecs.chenlongwang.top

Go:   type User struct { Name string; Age int }
来源：http://ssq.yj202588.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dry.zhoulong.xyz

C#:   record User(string Name, int Age);
来源：http://yvy.yongpay.top

[G15] 枚举
来源：http://ena.fzhhl.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mbg.pengpengdd.cyou

PHP:  enum Color: string { case Red = "red"; }
来源：http://mmd.yuanzhike.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ixr.zhengqikj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://anm.c1oappe.top

Java: enum Color { RED, GREEN }
来源：http://bfb.tian-w.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ijm.wangshuangyany.cn

Ruby: Color = %i[red green].freeze
来源：http://imv.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://won.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://uug.snrcjt.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://obm.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://exy.tarul.cn

JS:   Object.entries(obj)
来源：http://dzf.ehwqpu.com

TS:   Object.entries(obj)
来源：http://ypm.nanxuanxn.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fmw.snrcjt.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jll.xziqi.cn

Ruby: obj.instance_variables
来源：http://ygc.shangyingyoupin.top

C#:   // 用反射或 System.Text.Json
来源：http://szj.0kj1m.cn

================================================================================
来源：http://tne.xuetiantiany.cn

H. 异常与错误处理
来源：http://qkf.zhijiandao.cn

================================================================================
来源：http://bca.gzhubu.top

[H01] try / catch 基础
来源：http://udw.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wwp.gaohongyu789.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tdk.chenlongwang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://axv.nanxuanxn.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hmp.havefunace.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bax.yangfankeji.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vov.jqgfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mlh.uphjek.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ibs.xuetiantiany.cn

[H02] finally / ensure 收尾
来源：http://ntl.jinyuanbaomall.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tly.dashuyun.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pfg.ydzc1.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kry.dashuyun.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qaa.zhijiandao.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oon.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ukf.aibaodan.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yze.shuidangran.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ylb.yongpay.top

[H03] 主动抛出异常
来源：http://ubh.ppjwa.cn

Py:   raise ValueError("错误信息")
来源：http://msb.zhaomingkeji.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ayf.xingfuxueyuan.xyz

JS:   throw new Error("错误信息");
来源：http://pqr.bbcook.cn

TS:   throw new Error("错误信息");
来源：http://xsl.pycfn.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://pdt.quarkkingdee.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://syc.cashguo.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jkt.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://tmo.ywan-chungtsiang.top

[H04] 自定义异常类型
来源：http://mhn.pycfn.com

Py:   class MyError(Exception): pass
来源：http://eay.zycfv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yhe.hammf.cn

JS:   class MyError extends Error {}
来源：http://ajh.xylfe.cn

TS:   class MyError extends Error {}
来源：http://vdr.jianghu66.top

Java: class MyException extends RuntimeException {}
来源：http://zfd.tanke756.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tbt.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://mjn.wangdashe.top

C#:   class MyException : Exception {}
来源：http://cgr.hfpthk.cn

[H05] 捕获特定类型
来源：http://pfv.iojbl.cn

Py:   except ValueError as e:
来源：http://ghw.jyoumei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uee.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://zbp.yanxiufei.cn

TS:   if (e instanceof TypeError) {}
来源：http://hlt.cdnleiting.top

Java: catch (IOException | SQLException e) {}
来源：http://yeg.quarkkingdee.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rry.uphjek.com

Ruby: rescue ArgumentError => e
来源：http://zis.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://trg.dashuyun.cn

[H06] 可选值 / 空值安全访问
来源：http://idw.havefunace.top

Py:   value = d.get("k") or default
来源：http://row.yonumen.top

PHP:  $v = $d["k"] ?? null;
来源：http://lna.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://elg.gogol.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ldj.ctjpmb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uqz.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://buo.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://lrb.chenlongwang.top

C#:   obj?.A?.B ?? default
来源：http://oot.gotoacloud.top

[H07] 断言
来源：http://abs.jinqigfzy.top

Py:   assert x > 0, "必须为正"
来源：http://kcm.yj20258.top

PHP:  assert($x > 0);
来源：http://bvl.nanxinkj.top

JS:   console.assert(x > 0);
来源：http://ahs.yvedp.cn

TS:   console.assert(x > 0);
来源：http://oua.cucudq.cn

Java: assert x > 0 : "必须为正";
来源：http://nhf.sufxvd.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pai.c1oappe.top

Ruby: raise "必须为正" unless x > 0
来源：http://gcy.zhijiandao.cn


<!-- 参考信息 -->