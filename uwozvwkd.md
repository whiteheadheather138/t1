代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ayv.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://uve.zycfv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://odk.xingfuxueyuan.xyz

[F04] 追加写入文件
来源：http://ajp.cashguo.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vte.cheryme.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://grx.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://edo.jinqigfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://drn.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lre.epnwcf.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kxb.nwbrower.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://viv.dashuyun.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fnw.xingfuxueyuan.xyz

[F05] 判断文件或目录是否存在
来源：http://upn.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eis.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://ckv.ehwqpu.com

JS:   fs.existsSync("a.txt")
来源：http://aah.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://vck.hcnkem.com

Java: Files.exists(Path.of("a.txt"))
来源：http://hrd.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nda.quarkkingdee.top

Ruby: File.exist?("a.txt")
来源：http://twv.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://sra.cashguo.top

[F06] 删除文件
来源：http://uga.ydzc1.top

Py:   os.remove("a.txt")
来源：http://vdi.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://ucn.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zid.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vgb.dashuyun.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gsq.yongpay.top

Go:   os.Remove("a.txt")
来源：http://ord.sweek.top

Ruby: File.delete("a.txt")
来源：http://sgh.cheryme.top

C#:   File.Delete("a.txt");
来源：http://qjb.0kj1m.cn

[F07] 创建目录（含多级）
来源：http://mwl.yanxiufei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://maa.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mpn.yj20258888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ieo.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jba.ivvv.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vfq.yvedp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oif.zycfv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://onv.sjlbkw.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wug.yvedp.cn

[F08] 遍历目录
来源：http://ymk.redwolf501.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://sdv.xingfuxueyuan.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fxz.zhongyouzk.top

JS:   fs.readdirSync("dir")
来源：http://lnt.nwbrower.top

TS:   fs.readdirSync("dir")
来源：http://kff.xuanzx.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://icg.cheryme.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hhl.zhiwuduotai.top

Ruby: Dir.children("dir")
来源：http://uvp.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://ynq.fktsv.cn

[F09] 获取文件大小
来源：http://mlu.fanxiaobao.xyz

Py:   os.path.getsize("a.txt")
来源：http://xpi.ydjk.org.cn

PHP:  filesize("a.txt");
来源：http://bbr.kuanghao11.cn

JS:   fs.statSync("a.txt").size
来源：http://uur.dashuyun.cn

TS:   fs.statSync("a.txt").size
来源：http://wlp.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://mun.zdqjudy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fmc.316326.xyz

Ruby: File.size("a.txt")
来源：http://xvy.hongshengwenyu.top

C#:   new FileInfo("a.txt").Length
来源：http://hun.wangdashe.top

[F10] 取文件扩展名 / 文件名
来源：http://swz.ybcxt.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vte.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jua.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cvp.hnqzz.top

TS:   path.extname("a.txt")
来源：http://xdv.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hsf.zhaomingkeji.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rgq.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xhx.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cbd.shuidangran.top

[F11] 复制与移动文件
来源：http://dst.guowangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eli.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rgc.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://glk.jinqigufen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://odl.fehbvm.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tqw.havefunace.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kfl.dianchejie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ahw.aizwys.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kqa.yongpay.top

[F12] CSV 读写
来源：http://ssr.xuanzx.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tyz.pycfn.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mpk.zhoulong.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xjl.jianghu66.top

TS:   // 同上
来源：http://qaf.hcnkem.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fcj.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://amp.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bnb.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gji.pengpengdd.cyou

================================================================================
来源：http://fcu.hywenlv.cn

G. 面向对象
来源：http://vqv.guowangkeji.top

================================================================================
来源：http://cty.jqgufenzy.top

[G01] 定义类
来源：http://ayj.smart0.xyz

Py:   class User: pass
来源：http://wub.birdmap.top

PHP:  class User {}
来源：http://nbt.yuxming.cn

JS:   class User {}
来源：http://ftt.gaohongyu789.top

TS:   class User { name: string = ""; }
来源：http://ivs.jyoumei.cn

Java: class User {}
来源：http://zer.jiagoushi.top

Go:   type User struct { Name string }
来源：http://kfu.cheryme.top

Ruby: class User; end
来源：http://eje.nanxuanxn.top

C#:   class User {}
来源：http://yfn.daxiang520.top

[G02] 构造函数
来源：http://zqp.zhoulong.xyz

Py:   def __init__(self, name): self.name = name
来源：http://asb.shanyushiyangtech.top

PHP:  public function __construct(public string $name) {}
来源：http://fja.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://moi.yj20258888.top

TS:   constructor(public name: string) {}
来源：http://ezo.feifeiyinyue.top

Java: User(String name) { this.name = name; }
来源：http://jnj.ydzc1.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yxk.yj20258.top

Ruby: def initialize(name); @name = name; end
来源：http://ddp.shanyushiyangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://yqk.vehdjk.com

[G03] 实例属性
来源：http://ayj.aizwys.cn

Py:   self.name = "x"
来源：http://gkd.hammf.cn

PHP:  public string $name = "x";
来源：http://wuj.cucudq.cn

JS:   this.name = "x";
来源：http://mzv.tian-w.cn

TS:   name: string = "x";
来源：http://pqe.gogol.net.cn

Java: private String name;
来源：http://nin.zhixingplan.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jdh.kuanghao11.cn

Ruby: @name = "x"
来源：http://nxf.redwolf501.top

C#:   public string Name { get; set; } = "x";
来源：http://dpm.shzxlz.cn

[G04] 定义方法
来源：http://ean.shuidangran.top

Py:   def greet(self): return self.name
来源：http://hmh.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tlt.ctjpmb.com

JS:   greet() { return this.name; }
来源：http://fxj.kuanghao11.cn

TS:   greet(): string { return this.name; }
来源：http://mha.guowangkeji.top

Java: String greet() { return name; }
来源：http://tnx.yuanzhike.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://guo.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://mxb.haohaochexian.top

C#:   public string Greet() => Name;
来源：http://pht.fanxiaobao.xyz

[G05] 继承
来源：http://ggf.xylfe.cn

Py:   class Admin(User): pass
来源：http://hzt.nwbrower.top

PHP:  class Admin extends User {}
来源：http://pji.aizwys.cn

JS:   class Admin extends User {}
来源：http://fso.shangyingyoupin.top

TS:   class Admin extends User {}
来源：http://wsm.xuanzx.com

Java: class Admin extends User {}
来源：http://itj.vqdsnc.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.sysykeji.top

Ruby: class Admin < User; end
来源：http://soo.chenzaomai.com

C#:   class Admin : User {}
来源：http://jfj.ydzc1.top

[G06] 重写方法
来源：http://cwr.ydzc1.top

Py:   def greet(self): return "admin"
来源：http://prw.hongshengwenyu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nex.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://nyq.quarkkingdee.top

TS:   greet(): string { return "admin"; }
来源：http://rkx.guowangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://fzg.0kj1m.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fbn.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://yok.pycfn.com

C#:   public override string Greet() => "admin";
来源：http://bht.ivvv.top

[G07] 调用父类方法
来源：http://bey.52xcode.cn

Py:   super().greet()
来源：http://yxw.yj20258888.top

PHP:  parent::greet();
来源：http://jok.0kj1m.cn

JS:   super.greet();
来源：http://mzq.zhengqikj.top

TS:   super.greet();
来源：http://qfx.haohaochexian.top

Java: super.greet();
来源：http://eog.birdmap.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wia.fanxiaobao.xyz

Ruby: super
来源：http://izn.xziqi.cn

C#:   base.Greet();
来源：http://yzk.fengsongda.top

[G08] 静态方法与属性
来源：http://eig.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rpe.zhijiandao.cn

PHP:  public static function f() {}
来源：http://ufj.gogol.net.cn

JS:   static f() {}
来源：http://xes.guowangkeji.top

TS:   static f(): void {}
来源：http://jah.sweek.top

Java: static void f() {}
来源：http://war.gzhubu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ikb.zhoulong.xyz

Ruby: def self.f; end
来源：http://ojz.daria6918.cn

C#:   public static void F() {}
来源：http://cfl.yuxming.cn

[G09] 接口 / 抽象类
来源：http://mdf.mhx1999.top

Py:   from abc import ABC, abstractmethod
来源：http://aut.ivvv.top

PHP:  interface Shape { public function area(): float; }
来源：http://gcf.cqqwz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://oya.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://ufp.jinqigufen.top

Java: interface Shape { double area(); }
来源：http://puz.pengpengdd.cyou

Go:   type Shape interface { Area() float64 }
来源：http://xgk.yj202588.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fzc.xuanzx.com

C#:   interface IShape { double Area(); }
来源：http://uis.sysykeji.top

[G10] 访问控制
来源：http://tez.jqgufenzy.top

Py:   约定 _protected / __private（不强制）
来源：http://erx.fzhhl.top

PHP:  public / protected / private
来源：http://pkr.hongshengwenyu.top

JS:   #private 字段；其余公开
来源：http://cqf.jinqigfzy.top

TS:   public / protected / private
来源：http://dwn.ctjpmb.com

Java: public / protected / private / 默认包级
来源：http://enj.c1oappe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qjc.cucudq.cn

Ruby: public / protected / private
来源：http://rqy.bbcook.cn

C#:   public / protected / private / internal
来源：http://lqj.zhaomingkeji.xyz

[G11] getter / setter
来源：http://mfd.feifeiyinyue.top

Py:   @property 与 @x.setter
来源：http://bju.ehwqpu.com

PHP:  public function getName(): string { return $this->name; }
来源：http://lwr.shangyingyoupin.top

JS:   get name() { return this._name; }
来源：http://pxe.hywenlv.cn

TS:   get name(): string { return this._name; }
来源：http://qln.tian-w.cn

Java: public String getName() { return name; }
来源：http://bbg.sufxvd.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kof.uphjek.com

Ruby: attr_accessor :name
来源：http://eqa.zdqjudy.top

C#:   public string Name { get; set; }
来源：http://rzs.gotoacloud.top

[G12] 对象转字符串
来源：http://jgd.mhx1999.top

Py:   def __str__(self): return self.name
来源：http://lyn.zhengqikj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://efo.316326.xyz

JS:   toString() { return this.name; }
来源：http://agl.yuxming.cn

TS:   toString(): string { return this.name; }
来源：http://mgt.nanxinkj.top

Java: @Override public String toString() { return name; }
来源：http://pjp.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qcy.daria6918.cn

Ruby: def to_s; @name; end
来源：http://yjl.bbcook.cn

C#:   public override string ToString() => Name;
来源：http://yaj.zhoulong.xyz

[G13] 判断对象类型
来源：http://kfu.mhx1999.top

Py:   isinstance(u, User)
来源：http://xnp.chenlongwang.top

PHP:  $u instanceof User
来源：http://hlb.pycfn.com

JS:   u instanceof User
来源：http://lgi.pengpengdd.cyou

TS:   u instanceof User
来源：http://zmh.aizwys.cn

Java: u instanceof User
来源：http://jfd.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zza.epnwcf.com

Ruby: u.is_a?(User)
来源：http://qhl.9152youxi.cn

C#:   u is User
来源：http://ecq.jinqigufen.top

[G14] 数据类 / record
来源：http://wff.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xoy.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://ezp.gotoacloud.top

JS:   // 无内置：普通类或对象字面量
来源：http://vcl.haohaochexian.top

TS:   type User = { name: string; age: number };
来源：http://vdr.jinghuilouyu.cn

Java: record User(String name, int age) {}
来源：http://qwh.zhiwuduotai.top

Go:   type User struct { Name string; Age int }
来源：http://uxw.ehwqpu.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zkt.daxiang520.top

C#:   record User(string Name, int Age);
来源：http://wyz.kuanghao11.cn

[G15] 枚举
来源：http://vwi.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wtn.hcnkem.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://dhu.tarul.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rok.vehdjk.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fft.zhijiandao.cn

Java: enum Color { RED, GREEN }
来源：http://unf.wangshuangyany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zfy.chenzaomai.com

Ruby: Color = %i[red green].freeze
来源：http://krx.shuidangran.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bkn.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://tys.smart0.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rru.cdnleiting.top

PHP:  get_object_vars($obj);
来源：http://kzz.nwbrower.top

JS:   Object.entries(obj)
来源：http://ayu.xinyue.icu

TS:   Object.entries(obj)
来源：http://gak.yj20258888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yih.ydjk.org.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vmy.0kj1m.cn

Ruby: obj.instance_variables
来源：http://ukn.tian-w.cn

C#:   // 用反射或 System.Text.Json
来源：http://qun.bbcook.cn

================================================================================
来源：http://kfo.xuetiantiany.cn

H. 异常与错误处理
来源：http://gie.nanxuanxn.top

================================================================================
来源：http://guz.jqgufenzy.top

[H01] try / catch 基础
来源：http://gnd.yonumen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cdy.smart0.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fuy.fktsv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aed.guannengcc.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rck.ctjpmb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bxn.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dwx.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vna.yj202588.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fnd.fengsongda.top

[H02] finally / ensure 收尾
来源：http://ugy.zhaomingkeji.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://xfh.tarul.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://glu.gogol.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mas.9152youxi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://syz.quarkkingdee.top

Java: try { f(); } finally { cleanup(); }
来源：http://vhg.tianlin.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://utd.yanxiufei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tjb.nwbrower.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wfo.yj20258888.top

[H03] 主动抛出异常
来源：http://dun.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://nwf.tian-w.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ika.pycfn.com

JS:   throw new Error("错误信息");
来源：http://zpm.dianchejie.cn

TS:   throw new Error("错误信息");
来源：http://rta.aizwys.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://spo.shzxlz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://epk.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ygt.hesvh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ywi.snrcjt.cn

[H04] 自定义异常类型
来源：http://ykk.shuidangran.top

Py:   class MyError(Exception): pass
来源：http://rav.dianchejie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gyk.smart0.xyz

JS:   class MyError extends Error {}
来源：http://fby.tanke756.top

TS:   class MyError extends Error {}
来源：http://uqr.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://ksm.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://txh.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://kvz.ydjk.org.cn

C#:   class MyException : Exception {}
来源：http://lzn.aizwys.cn

[H05] 捕获特定类型
来源：http://jae.aibaodan.cn

Py:   except ValueError as e:
来源：http://qvb.zycfv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cur.jinqigufen.top

JS:   if (e instanceof TypeError) {}
来源：http://blc.52xcode.cn

TS:   if (e instanceof TypeError) {}
来源：http://uwy.zdqjudy.top

Java: catch (IOException | SQLException e) {}
来源：http://aig.haohaochexian.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jvf.hnqzz.top

Ruby: rescue ArgumentError => e
来源：http://hjb.xylfe.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://trs.jinyuanbaomall.cn

[H06] 可选值 / 空值安全访问
来源：http://cio.sxryk.cn

Py:   value = d.get("k") or default
来源：http://jkq.nwbrower.top

PHP:  $v = $d["k"] ?? null;
来源：http://mvs.sjlbkw.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wii.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://ajp.fanxiaobao.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xgi.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://omr.hysaishi.cn

Ruby: d&.dig(:a, :b)
来源：http://hjr.hongshengwenyu.top

C#:   obj?.A?.B ?? default
来源：http://ilg.tanke756.top

[H07] 断言
来源：http://phj.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://nij.zdqjudy.top

PHP:  assert($x > 0);
来源：http://clz.9152youxi.cn

JS:   console.assert(x > 0);
来源：http://jis.hnqzz.top

TS:   console.assert(x > 0);
来源：http://niq.shanyushiyangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://grn.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zdv.zhixingplan.top

Ruby: raise "必须为正" unless x > 0
来源：http://qyw.yvedp.cn

C#:   Debug.Assert(x > 0);
来源：http://vqe.zdqjudy.top

[H08] 获取错误信息与堆栈
来源：http://ksc.yfazqb.com

Py:   str(e);  traceback.format_exc()
来源：http://krc.fktsv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wqr.sufxvd.cn


<!-- 参考信息 -->