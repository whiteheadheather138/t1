代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://udc.zhengqikj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ndc.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cfv.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tve.guowangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://trn.xziqi.cn

Ruby: File.write("a.txt", "hi")
来源：http://hvg.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pjo.hongshengwenyu.top

[F04] 追加写入文件
来源：http://bkq.wangdashe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://exe.fzhhl.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://log.hcnkem.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dpn.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zgb.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ppo.epnwcf.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qig.jiagoushi.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yom.smart0.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qse.jqgufenzy.top

[F05] 判断文件或目录是否存在
来源：http://fbo.jinghuilouyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kia.xylfe.cn

PHP:  file_exists("a.txt");
来源：http://syu.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://dcu.snrcjt.cn

TS:   fs.existsSync("a.txt")
来源：http://qkp.cheryme.top

Java: Files.exists(Path.of("a.txt"))
来源：http://aiq.ybcxt.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rsx.yanxiufei.cn

Ruby: File.exist?("a.txt")
来源：http://iqe.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://yrm.ppjwa.cn

[F06] 删除文件
来源：http://nsy.daxiang520.top

Py:   os.remove("a.txt")
来源：http://mcd.guowangkeji.top

PHP:  unlink("a.txt");
来源：http://ecv.vqdsnc.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nad.gogol.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mhp.yanxiufei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vwb.hfpthk.cn

Go:   os.Remove("a.txt")
来源：http://unw.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://knu.daria6918.cn

C#:   File.Delete("a.txt");
来源：http://efs.zycfv.cn

[F07] 创建目录（含多级）
来源：http://dkn.aizwys.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fxv.snrcjt.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ara.yuanzhike.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zyv.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qvt.chenjidiqi.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cve.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rwt.yanxiufei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nyq.daria6918.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tsl.zhijiandao.cn

[F08] 遍历目录
来源：http://tpw.nanxinkj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rhr.xingfuxueyuan.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vxa.quarkkingdee.top

JS:   fs.readdirSync("dir")
来源：http://kwt.sxryk.cn

TS:   fs.readdirSync("dir")
来源：http://ink.sufxvd.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jih.jinqigufen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qld.vqdsnc.cn

Ruby: Dir.children("dir")
来源：http://vmt.hnxiangtu.top

C#:   Directory.GetFiles("dir")
来源：http://rbu.xuetiantiany.cn

[F09] 获取文件大小
来源：http://gzv.cashguo.top

Py:   os.path.getsize("a.txt")
来源：http://qal.fzhhl.top

PHP:  filesize("a.txt");
来源：http://rfv.kuanghao11.cn

JS:   fs.statSync("a.txt").size
来源：http://oaw.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://gqf.zhaomingkeji.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://uiv.epnwcf.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oox.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://hjh.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://wri.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://ucp.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eny.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rjf.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ccw.ctjpmb.com

TS:   path.extname("a.txt")
来源：http://ifb.jyoumei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rng.zycfv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://owi.nanxuanxn.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uau.bbcook.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gvh.smart0.xyz

[F11] 复制与移动文件
来源：http://wqi.quarkkingdee.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fsk.shuidangran.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nxn.shangyingyoupin.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aiv.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sij.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sqs.tanke756.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://het.zhixingplan.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xgz.sjlbkw.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lyk.yj20258.top

[F12] CSV 读写
来源：http://hpw.nanxuanxn.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gyc.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nqd.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://opi.xingfuxueyuan.xyz

TS:   // 同上
来源：http://jsc.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cla.xingfuxueyuan.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mkn.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qxs.sweek.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zqu.zdbjq.cn

================================================================================
来源：http://ivn.jinqigufen.top

G. 面向对象
来源：http://owy.uphjek.com

================================================================================
来源：http://iuw.shanyushiyangtech.top

[G01] 定义类
来源：http://kvz.snrcjt.cn

Py:   class User: pass
来源：http://tjt.sufxvd.cn

PHP:  class User {}
来源：http://ipq.yonumen.top

JS:   class User {}
来源：http://xpq.jinqigfzy.top

TS:   class User { name: string = ""; }
来源：http://cnw.shanyushiyangkeji.top

Java: class User {}
来源：http://ipq.yanxiufei.cn

Go:   type User struct { Name string }
来源：http://wcs.daria6918.cn

Ruby: class User; end
来源：http://vxb.hongshengwenyu.top

C#:   class User {}
来源：http://ptc.ywan-chungtsiang.top

[G02] 构造函数
来源：http://ldo.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://nsu.wangdashe.top

PHP:  public function __construct(public string $name) {}
来源：http://tnk.316326.xyz

JS:   constructor(name) { this.name = name; }
来源：http://eqy.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://uws.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://evz.chenlongwang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zkj.yuanzhike.top

Ruby: def initialize(name); @name = name; end
来源：http://gbr.yueranfly.top

C#:   public User(string name) { Name = name; }
来源：http://kpp.tarul.cn

[G03] 实例属性
来源：http://eoh.zhiwuduotai.top

Py:   self.name = "x"
来源：http://gbo.wangdashe.top

PHP:  public string $name = "x";
来源：http://iuc.ydzc1.top

JS:   this.name = "x";
来源：http://mfz.redwolf501.top

TS:   name: string = "x";
来源：http://zxv.shangyingyoupin.top

Java: private String name;
来源：http://gbw.jlsjyb.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://muo.nwbrower.top

Ruby: @name = "x"
来源：http://xft.gogol.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://dad.pengpengdd.cyou

[G04] 定义方法
来源：http://eae.sxryk.cn

Py:   def greet(self): return self.name
来源：http://cnx.fzhhl.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ype.jinqigufen.top

JS:   greet() { return this.name; }
来源：http://ewr.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://bas.pycfn.com

Java: String greet() { return name; }
来源：http://bjh.jlsjyb.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tal.52xcode.cn

Ruby: def greet; @name; end
来源：http://mei.tianlin.xyz

C#:   public string Greet() => Name;
来源：http://qoq.daria6918.cn

[G05] 继承
来源：http://lzo.sxryk.cn

Py:   class Admin(User): pass
来源：http://enh.xinyue.icu

PHP:  class Admin extends User {}
来源：http://sog.tarul.cn

JS:   class Admin extends User {}
来源：http://tyk.yfazqb.com

TS:   class Admin extends User {}
来源：http://cbn.hnqzz.top

Java: class Admin extends User {}
来源：http://qfu.yj20258888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eph.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://rwr.vehdjk.com

C#:   class Admin : User {}
来源：http://nxa.chenjidiqi.icu

[G06] 重写方法
来源：http://wwh.aizwys.cn

Py:   def greet(self): return "admin"
来源：http://bed.tanke756.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qeq.chenzaomai.com

JS:   greet() { return "admin"; }
来源：http://uss.kuanghao11.cn

TS:   greet(): string { return "admin"; }
来源：http://ymr.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://hlp.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gdn.yuanzhike.top

Ruby: def greet; "admin"; end
来源：http://tsb.fanxiaobao.xyz

C#:   public override string Greet() => "admin";
来源：http://ioy.52xcode.cn

[G07] 调用父类方法
来源：http://cjw.nanxuanxn.top

Py:   super().greet()
来源：http://phc.chenjidiqi.icu

PHP:  parent::greet();
来源：http://brj.ydzc1.top

JS:   super.greet();
来源：http://crq.jinqigfzy.top

TS:   super.greet();
来源：http://hur.xziqi.cn

Java: super.greet();
来源：http://wqk.yj20258888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://czf.cucudq.cn

Ruby: super
来源：http://kiv.xuanzx.com

C#:   base.Greet();
来源：http://hwl.smart0.xyz

[G08] 静态方法与属性
来源：http://kka.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ghq.xylfe.cn

PHP:  public static function f() {}
来源：http://zec.kuanghao11.cn

JS:   static f() {}
来源：http://lrz.aibaodan.cn

TS:   static f(): void {}
来源：http://gig.yongpay.top

Java: static void f() {}
来源：http://aow.jlsjyb.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xft.ydzc1.top

Ruby: def self.f; end
来源：http://eyk.hongshengwenyu.top

C#:   public static void F() {}
来源：http://vxi.yj20258.top

[G09] 接口 / 抽象类
来源：http://okm.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://vtg.gogol.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uut.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dbd.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://ftr.feifeiyinyue.top

Java: interface Shape { double area(); }
来源：http://nru.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://khu.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xin.cdnleiting.top

C#:   interface IShape { double Area(); }
来源：http://ael.redwolf501.top

[G10] 访问控制
来源：http://npn.nanxuanxn.top

Py:   约定 _protected / __private（不强制）
来源：http://swi.cqqwz.cn

PHP:  public / protected / private
来源：http://gcm.wangdashe.top

JS:   #private 字段；其余公开
来源：http://zjh.guowangkeji.top

TS:   public / protected / private
来源：http://jta.smart0.xyz

Java: public / protected / private / 默认包级
来源：http://ppy.xylfe.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xvm.0kj1m.cn

Ruby: public / protected / private
来源：http://ecv.daria6918.cn

C#:   public / protected / private / internal
来源：http://lnz.nanxuanxn.top

[G11] getter / setter
来源：http://osv.jqgfzy.top

Py:   @property 与 @x.setter
来源：http://hgs.gaohongyu789.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zay.jlsjyb.cn

JS:   get name() { return this._name; }
来源：http://tue.xuetiantiany.cn

TS:   get name(): string { return this._name; }
来源：http://rmr.sjlbkw.cn

Java: public String getName() { return name; }
来源：http://odq.yonumen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hkm.hammf.cn

Ruby: attr_accessor :name
来源：http://hnh.uphjek.com

C#:   public string Name { get; set; }
来源：http://osn.gaohongyu789.top

[G12] 对象转字符串
来源：http://bzn.gogol.net.cn

Py:   def __str__(self): return self.name
来源：http://evs.chenjidiqi.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://vyz.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://bhi.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://bgy.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://iwt.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wgt.birdmap.top

Ruby: def to_s; @name; end
来源：http://lbb.fktsv.cn

C#:   public override string ToString() => Name;
来源：http://qbb.chenlongwang.top

[G13] 判断对象类型
来源：http://raw.aibaodan.cn

Py:   isinstance(u, User)
来源：http://eoq.yuanzhike.top

PHP:  $u instanceof User
来源：http://xig.mhx1999.top

JS:   u instanceof User
来源：http://bmx.hesvh.cn

TS:   u instanceof User
来源：http://hmz.fktsv.cn

Java: u instanceof User
来源：http://mlk.bbcook.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oeg.zhiwuduotai.top

Ruby: u.is_a?(User)
来源：http://kli.yuxming.cn

C#:   u is User
来源：http://iep.tian-w.cn

[G14] 数据类 / record
来源：http://zjf.hongshengwenyu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pxx.jianghu66.top

PHP:  // 用 readonly 属性模拟
来源：http://qig.ybcxt.top

JS:   // 无内置：普通类或对象字面量
来源：http://nyt.ydjk.org.cn

TS:   type User = { name: string; age: number };
来源：http://ntn.wangdashe.top

Java: record User(String name, int age) {}
来源：http://xop.shangyingyoupin.top

Go:   type User struct { Name string; Age int }
来源：http://ysz.vqdsnc.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://biu.c1oappe.top

C#:   record User(string Name, int Age);
来源：http://yey.sufxvd.cn

[G15] 枚举
来源：http://obn.yj202588.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qgj.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://quj.yj20258888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xct.zhiwuduotai.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wdc.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://obn.hywenlv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dkn.fktsv.cn

Ruby: Color = %i[red green].freeze
来源：http://ubw.yj202588.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ubu.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://wnk.sysykeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ero.ehwqpu.com

PHP:  get_object_vars($obj);
来源：http://xrp.hammf.cn

JS:   Object.entries(obj)
来源：http://xrg.fanxiaobao.xyz

TS:   Object.entries(obj)
来源：http://qlb.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tpf.ydzc1.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bxl.fengsongda.top

Ruby: obj.instance_variables
来源：http://bfj.yj202588.top

C#:   // 用反射或 System.Text.Json
来源：http://uoi.yj20258888.top

================================================================================
来源：http://jem.ydjk.org.cn

H. 异常与错误处理
来源：http://iua.aizwys.cn

================================================================================
来源：http://pjb.cucudq.cn

[H01] try / catch 基础
来源：http://sxi.haohaochexian.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://voi.zhixingplan.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xnl.yonumen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://arw.guowangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://glt.ppjwa.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jfd.redwolf501.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xqr.jinqigfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://grq.svipenyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jsj.daria6918.cn

[H02] finally / ensure 收尾
来源：http://nuy.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://paq.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://znp.dianchejie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vns.zhoulong.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://zze.sjlbkw.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wjt.jlsjyb.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xht.xinyue.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://ttl.jqgfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gjb.xziqi.cn

[H03] 主动抛出异常
来源：http://qqu.jinyuanbaomall.cn

Py:   raise ValueError("错误信息")
来源：http://wbx.xinyue.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ngg.jinqigfzy.top

JS:   throw new Error("错误信息");
来源：http://tnp.vehdjk.com

TS:   throw new Error("错误信息");
来源：http://tlc.316326.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://vyv.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mwz.hnqzz.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kgm.hnqzz.top

C#:   throw new ArgumentException("错误信息");
来源：http://ypy.nanxinkj.top

[H04] 自定义异常类型
来源：http://ttn.hnqzz.top

Py:   class MyError(Exception): pass
来源：http://mjn.haohaochexian.top

PHP:  class MyError extends RuntimeException {}
来源：http://yfj.nanxuanxn.top

JS:   class MyError extends Error {}
来源：http://khx.yuanzhike.top

TS:   class MyError extends Error {}
来源：http://rjo.gzhubu.top

Java: class MyException extends RuntimeException {}
来源：http://ifx.ppjwa.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oct.xinyue.icu

Ruby: class MyError < StandardError; end
来源：http://zpx.daria6918.cn

C#:   class MyException : Exception {}
来源：http://hwh.wangshuangyany.cn

[H05] 捕获特定类型
来源：http://pej.tianlin.xyz

Py:   except ValueError as e:
来源：http://mcm.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qao.ctjpmb.com

JS:   if (e instanceof TypeError) {}
来源：http://rej.fanxiaobao.xyz

TS:   if (e instanceof TypeError) {}
来源：http://kdt.yj202588.top

Java: catch (IOException | SQLException e) {}
来源：http://xdv.xingfuxueyuan.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jgh.guannengcc.top

Ruby: rescue ArgumentError => e
来源：http://ina.quarkkingdee.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hfk.tianlin.xyz

[H06] 可选值 / 空值安全访问
来源：http://fgg.yfazqb.com

Py:   value = d.get("k") or default
来源：http://whj.jyoumei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gxo.ivvv.top

JS:   obj?.a?.b;  d ?? default
来源：http://czs.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jyo.fktsv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://djl.wangdashe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hpa.jinqigfzy.top

Ruby: d&.dig(:a, :b)
来源：http://vsr.cdnleiting.top

C#:   obj?.A?.B ?? default
来源：http://hqk.9152youxi.cn

[H07] 断言
来源：http://dcs.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://ytj.zhixingplan.top

PHP:  assert($x > 0);
来源：http://ine.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://emv.yfazqb.com

TS:   console.assert(x > 0);
来源：http://qyi.xziqi.cn

Java: assert x > 0 : "必须为正";
来源：http://owk.jiagoushi.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hts.zhengqikj.top

Ruby: raise "必须为正" unless x > 0
来源：http://juj.ivvv.top


<!-- 参考信息 -->