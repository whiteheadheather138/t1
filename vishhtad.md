代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ama.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://vqg.gaohongyu789.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hsq.jianghu66.top

[F04] 追加写入文件
来源：http://feq.sxryk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aib.hcnkem.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xew.9152youxi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qzj.zdbjq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wur.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gcy.ydzc1.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iqq.zhiwuduotai.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kce.gogol.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uxm.pengpengdd.cyou

[F05] 判断文件或目录是否存在
来源：http://sfk.cheryme.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zqx.uphjek.com

PHP:  file_exists("a.txt");
来源：http://pwb.hfpthk.cn

JS:   fs.existsSync("a.txt")
来源：http://crt.xziqi.cn

TS:   fs.existsSync("a.txt")
来源：http://vcv.jinghuilouyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dlz.hesvh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lng.xuanzx.com

Ruby: File.exist?("a.txt")
来源：http://uml.epnwcf.com

C#:   File.Exists("a.txt")
来源：http://bly.fengsongda.top

[F06] 删除文件
来源：http://czx.cucudq.cn

Py:   os.remove("a.txt")
来源：http://gfx.ybcxt.top

PHP:  unlink("a.txt");
来源：http://xxl.hywenlv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hcw.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://hjr.havefunace.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xqu.hongshengwenyu.top

Go:   os.Remove("a.txt")
来源：http://kcs.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://gwq.zhijiandao.cn

C#:   File.Delete("a.txt");
来源：http://zth.gogol.net.cn

[F07] 创建目录（含多级）
来源：http://lvn.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mkb.shanyushiyangtech.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ofr.xuetiantiany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kaf.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kcr.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hps.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ucy.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bvs.ivvv.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lsw.birdmap.top

[F08] 遍历目录
来源：http://ybl.yangfankeji.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://pef.guowangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xjb.yj20258888.top

JS:   fs.readdirSync("dir")
来源：http://mee.birdmap.top

TS:   fs.readdirSync("dir")
来源：http://ufa.ydjk.org.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fhv.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nmb.andypj.xyz

Ruby: Dir.children("dir")
来源：http://vok.bbcook.cn

C#:   Directory.GetFiles("dir")
来源：http://gxo.yfazqb.com

[F09] 获取文件大小
来源：http://oew.jinyuanbaomall.cn

Py:   os.path.getsize("a.txt")
来源：http://wyd.havefunace.top

PHP:  filesize("a.txt");
来源：http://jyu.wangshuangyany.cn

JS:   fs.statSync("a.txt").size
来源：http://hdz.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://ezz.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://two.tarul.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xda.tanke756.top

Ruby: File.size("a.txt")
来源：http://hhj.zhixingplan.top

C#:   new FileInfo("a.txt").Length
来源：http://dti.aizwys.cn

[F10] 取文件扩展名 / 文件名
来源：http://lyk.52xcode.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ldk.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kxo.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mai.ehwqpu.com

TS:   path.extname("a.txt")
来源：http://rdk.hammf.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://plb.yj20258888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kna.gotoacloud.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rtd.tianlin.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xob.haohaochexian.top

[F11] 复制与移动文件
来源：http://jyy.smart0.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zwj.nwbrower.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lee.fktsv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sye.zhixingplan.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gde.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://due.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://soe.uphjek.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rop.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://afg.hesvh.cn

[F12] CSV 读写
来源：http://zpi.mhx1999.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://glu.aibaodan.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lxk.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ils.uphjek.com

TS:   // 同上
来源：http://vfx.chenjidiqi.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pty.fehbvm.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://srg.jqgufenzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pby.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mrt.sweek.top

================================================================================
来源：http://hue.yangfankeji.com

G. 面向对象
来源：http://qqn.havefunace.top

================================================================================
来源：http://phe.zhijiandao.cn

[G01] 定义类
来源：http://leo.yj20258888.top

Py:   class User: pass
来源：http://uua.daria6918.cn

PHP:  class User {}
来源：http://siy.fzhhl.top

JS:   class User {}
来源：http://zjd.shanyushiyangtech.top

TS:   class User { name: string = ""; }
来源：http://bxf.zhengqikj.top

Java: class User {}
来源：http://ztx.zhiwuduotai.top

Go:   type User struct { Name string }
来源：http://yqw.gotoacloud.top

Ruby: class User; end
来源：http://tkb.tanke756.top

C#:   class User {}
来源：http://aex.nanxuanxn.top

[G02] 构造函数
来源：http://cwt.haohaochexian.top

Py:   def __init__(self, name): self.name = name
来源：http://laa.havefunace.top

PHP:  public function __construct(public string $name) {}
来源：http://dzw.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://jsl.ppjwa.cn

TS:   constructor(public name: string) {}
来源：http://kip.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://wuh.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yrz.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://dfl.zhijiandao.cn

C#:   public User(string name) { Name = name; }
来源：http://ytw.c1oappe.top

[G03] 实例属性
来源：http://gfq.yanxiufei.cn

Py:   self.name = "x"
来源：http://jkb.xziqi.cn

PHP:  public string $name = "x";
来源：http://wdi.pycfn.com

JS:   this.name = "x";
来源：http://kgu.cdnleiting.top

TS:   name: string = "x";
来源：http://cnk.pycfn.com

Java: private String name;
来源：http://eip.cucudq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lda.meibo888.top

Ruby: @name = "x"
来源：http://aoc.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://nvn.zhijiandao.cn

[G04] 定义方法
来源：http://fbe.fzhhl.top

Py:   def greet(self): return self.name
来源：http://awy.yvedp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rjt.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://tlb.zycfv.cn

TS:   greet(): string { return this.name; }
来源：http://eet.daria6918.cn

Java: String greet() { return name; }
来源：http://rgk.jinqigufen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lzo.bjfxy.top

Ruby: def greet; @name; end
来源：http://mbg.sweek.top

C#:   public string Greet() => Name;
来源：http://dky.fehbvm.com

[G05] 继承
来源：http://gch.guannengcc.top

Py:   class Admin(User): pass
来源：http://ogg.shuidangran.top

PHP:  class Admin extends User {}
来源：http://uhb.c1oappe.top

JS:   class Admin extends User {}
来源：http://qln.zdbjq.cn

TS:   class Admin extends User {}
来源：http://tcs.yj202588.top

Java: class Admin extends User {}
来源：http://cqw.xuanzx.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://grj.daria6918.cn

Ruby: class Admin < User; end
来源：http://kif.ppjwa.cn

C#:   class Admin : User {}
来源：http://hgi.shuidangran.top

[G06] 重写方法
来源：http://mts.shuidangran.top

Py:   def greet(self): return "admin"
来源：http://vvi.havefunace.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rvd.gzhubu.top

JS:   greet() { return "admin"; }
来源：http://vpl.haohaochexian.top

TS:   greet(): string { return "admin"; }
来源：http://dek.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://mfh.guowangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nkk.tarul.cn

Ruby: def greet; "admin"; end
来源：http://vtl.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://mym.yuanzhike.top

[G07] 调用父类方法
来源：http://cuk.wangshuangyany.cn

Py:   super().greet()
来源：http://oxw.yvedp.cn

PHP:  parent::greet();
来源：http://nhm.gogol.net.cn

JS:   super.greet();
来源：http://rod.ybcxt.top

TS:   super.greet();
来源：http://vvs.zhengqikj.top

Java: super.greet();
来源：http://kai.cucudq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://taw.hongshengwenyu.top

Ruby: super
来源：http://hec.jinqigfzy.top

C#:   base.Greet();
来源：http://xqw.bjfxy.top

[G08] 静态方法与属性
来源：http://tel.dashuyun.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://noc.9152youxi.cn

PHP:  public static function f() {}
来源：http://fcz.ctjpmb.com

JS:   static f() {}
来源：http://efm.shangyingyoupin.top

TS:   static f(): void {}
来源：http://nmi.fengsongda.top

Java: static void f() {}
来源：http://tov.chenjidiqi.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://oht.316326.xyz

Ruby: def self.f; end
来源：http://fni.nanxinkj.top

C#:   public static void F() {}
来源：http://bbm.fengsongda.top

[G09] 接口 / 抽象类
来源：http://kqa.cdnleiting.top

Py:   from abc import ABC, abstractmethod
来源：http://xer.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nna.dianchejie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kwk.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://kcf.gzhubu.top

Java: interface Shape { double area(); }
来源：http://wsp.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://bxa.mhx1999.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://esk.fzhhl.top

C#:   interface IShape { double Area(); }
来源：http://jpr.9152youxi.cn

[G10] 访问控制
来源：http://wun.xylfe.cn

Py:   约定 _protected / __private（不强制）
来源：http://hxl.yfazqb.com

PHP:  public / protected / private
来源：http://igl.jinqigufen.top

JS:   #private 字段；其余公开
来源：http://anf.sweek.top

TS:   public / protected / private
来源：http://prn.kuanghao11.cn

Java: public / protected / private / 默认包级
来源：http://xhz.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://aod.xinyue.icu

Ruby: public / protected / private
来源：http://bzw.yj202588.top

C#:   public / protected / private / internal
来源：http://pjj.havefunace.top

[G11] getter / setter
来源：http://gnp.c1oappe.top

Py:   @property 与 @x.setter
来源：http://tyi.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://npg.shangyingyoupin.top

JS:   get name() { return this._name; }
来源：http://uin.ydjk.org.cn

TS:   get name(): string { return this._name; }
来源：http://rlf.zhongyouzk.top

Java: public String getName() { return name; }
来源：http://pgh.smart0.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://cud.fengsongda.top

Ruby: attr_accessor :name
来源：http://inc.shangyingyoupin.top

C#:   public string Name { get; set; }
来源：http://haw.jinyuanbaomall.cn

[G12] 对象转字符串
来源：http://nhj.fengsongda.top

Py:   def __str__(self): return self.name
来源：http://sjf.xuetiantiany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gye.nanxuanxn.top

JS:   toString() { return this.name; }
来源：http://wrb.9152youxi.cn

TS:   toString(): string { return this.name; }
来源：http://xpn.wangdashe.top

Java: @Override public String toString() { return name; }
来源：http://udx.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://aws.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://bky.jinqigufen.top

C#:   public override string ToString() => Name;
来源：http://cer.fzhhl.top

[G13] 判断对象类型
来源：http://rbq.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://qih.hnxiangtu.top

PHP:  $u instanceof User
来源：http://esj.zhiwuduotai.top

JS:   u instanceof User
来源：http://ktb.yanxiufei.cn

TS:   u instanceof User
来源：http://pbq.kuanghao11.cn

Java: u instanceof User
来源：http://vle.cdnleiting.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://irw.yj20258.top

Ruby: u.is_a?(User)
来源：http://srh.zhixingplan.top

C#:   u is User
来源：http://amp.birdmap.top

[G14] 数据类 / record
来源：http://zmi.ywan-chungtsiang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wxb.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://vag.xziqi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://eey.uphjek.com

TS:   type User = { name: string; age: number };
来源：http://gcl.yongpay.top

Java: record User(String name, int age) {}
来源：http://xin.tarul.cn

Go:   type User struct { Name string; Age int }
来源：http://raw.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wkw.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://prh.yvedp.cn

[G15] 枚举
来源：http://ekb.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xrr.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bef.cashguo.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://orz.epnwcf.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zbr.sysykeji.top

Java: enum Color { RED, GREEN }
来源：http://wwg.yongpay.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pco.zhongyouzk.top

Ruby: Color = %i[red green].freeze
来源：http://nne.hcnkem.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nrk.hnxiangtu.top

[G16] 对象转数组 / 字典
来源：http://tzj.feifeiyinyue.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iuw.sysykeji.top

PHP:  get_object_vars($obj);
来源：http://ycl.yvedp.cn

JS:   Object.entries(obj)
来源：http://bka.sxryk.cn

TS:   Object.entries(obj)
来源：http://dmi.shanyushiyangtech.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nkn.316326.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://fpi.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://tiz.aizwys.cn

C#:   // 用反射或 System.Text.Json
来源：http://yqk.sysykeji.top

================================================================================
来源：http://elr.fengsongda.top

H. 异常与错误处理
来源：http://lna.hywenlv.cn

================================================================================
来源：http://omp.haohaochexian.top

[H01] try / catch 基础
来源：http://fiq.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bzt.nwbrower.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://myj.daria6918.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dcq.smart0.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zjz.xziqi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gsf.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qqc.aizwys.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dmz.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://luz.dianchejie.cn

[H02] finally / ensure 收尾
来源：http://rga.gotoacloud.top

Py:   try: f()⏎finally: cleanup()
来源：http://jtj.gaohongyu789.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kfd.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bag.gotoacloud.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mxu.xziqi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eki.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bbi.jqgfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://res.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://lua.aibaodan.cn

[H03] 主动抛出异常
来源：http://wyc.yuxming.cn

Py:   raise ValueError("错误信息")
来源：http://wra.dashuyun.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cjf.ydjk.org.cn

JS:   throw new Error("错误信息");
来源：http://tvp.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://zss.dianchejie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qsi.dianchejie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hxx.smart0.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://ycn.zhixingplan.top

C#:   throw new ArgumentException("错误信息");
来源：http://iui.xylfe.cn

[H04] 自定义异常类型
来源：http://eaf.haohaochexian.top

Py:   class MyError(Exception): pass
来源：http://zec.jqgufenzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://bvr.sxryk.cn

JS:   class MyError extends Error {}
来源：http://heq.tianlin.xyz

TS:   class MyError extends Error {}
来源：http://hdr.dashuyun.cn

Java: class MyException extends RuntimeException {}
来源：http://tlg.zdqjudy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xpc.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://wnz.tanke756.top

C#:   class MyException : Exception {}
来源：http://zvh.bjfxy.top

[H05] 捕获特定类型
来源：http://dsu.yj202588.top

Py:   except ValueError as e:
来源：http://mfm.ehwqpu.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ilz.zdbjq.cn

JS:   if (e instanceof TypeError) {}
来源：http://lmt.cdnleiting.top

TS:   if (e instanceof TypeError) {}
来源：http://qyh.shzxlz.cn

Java: catch (IOException | SQLException e) {}
来源：http://dar.guowangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://psu.smart0.xyz

Ruby: rescue ArgumentError => e
来源：http://obd.gaohongyu789.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hfj.yongpay.top

[H06] 可选值 / 空值安全访问
来源：http://bmw.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://fdw.yj202588.top

PHP:  $v = $d["k"] ?? null;
来源：http://mby.dianchejie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://irn.cheryme.top

TS:   obj?.a?.b;  d ?? default
来源：http://jnj.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://quw.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://rqf.cucudq.cn

Ruby: d&.dig(:a, :b)
来源：http://sfp.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://vgg.zhijiandao.cn

[H07] 断言
来源：http://fgg.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://tms.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://hnm.cdnleiting.top

JS:   console.assert(x > 0);
来源：http://lhn.uphjek.com

TS:   console.assert(x > 0);
来源：http://fvt.shanyushiyangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://ghc.zhiwuduotai.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vcv.meibo888.top

Ruby: raise "必须为正" unless x > 0
来源：http://dqg.aibaodan.cn

C#:   Debug.Assert(x > 0);
来源：http://tei.tian-w.cn

[H08] 获取错误信息与堆栈
来源：http://iuj.yj20258888.top

Py:   str(e);  traceback.format_exc()
来源：http://fyz.zhaomingkeji.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kfd.yvedp.cn


<!-- 参考信息 -->