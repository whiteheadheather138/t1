代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pse.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nqv.hfpthk.cn

[F03] 写入文件（覆盖）
来源：http://zki.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://glc.haohaochexian.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gdd.sxryk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kep.cucudq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ndh.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lki.feifeiyinyue.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ayd.gotoacloud.top

Ruby: File.write("a.txt", "hi")
来源：http://jzr.cqqwz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vdb.52xcode.cn

[F04] 追加写入文件
来源：http://csv.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vlm.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jql.fzhhl.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rom.meibo888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zsg.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://skh.guowangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jox.hfpthk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wzo.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nhc.hammf.cn

[F05] 判断文件或目录是否存在
来源：http://llr.ydjk.org.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rkv.hysaishi.cn

PHP:  file_exists("a.txt");
来源：http://ghb.iojbl.cn

JS:   fs.existsSync("a.txt")
来源：http://kwq.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://wdu.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://jin.zdqjudy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iyj.zhixingplan.top

Ruby: File.exist?("a.txt")
来源：http://tjj.ehwqpu.com

C#:   File.Exists("a.txt")
来源：http://xqq.nwbrower.top

[F06] 删除文件
来源：http://eip.tian-w.cn

Py:   os.remove("a.txt")
来源：http://zkf.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://xqz.shuidangran.top

JS:   fs.unlinkSync("a.txt")
来源：http://atj.jlsjyb.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vwh.0kj1m.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qra.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://cee.meibo888.top

Ruby: File.delete("a.txt")
来源：http://hgl.c1oappe.top

C#:   File.Delete("a.txt");
来源：http://pgq.chenlongwang.top

[F07] 创建目录（含多级）
来源：http://oru.gzhubu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yme.uphjek.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://knd.ydjk.org.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pnb.andypj.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://msx.gotoacloud.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vkw.jianghu66.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xug.tian-w.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wfz.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xqq.jinqigfzy.top

[F08] 遍历目录
来源：http://tsf.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://mhh.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ced.yueranfly.top

JS:   fs.readdirSync("dir")
来源：http://qpq.jiagoushi.top

TS:   fs.readdirSync("dir")
来源：http://zfu.jinqigfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zwk.ywan-chungtsiang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://iwf.bbcook.cn

Ruby: Dir.children("dir")
来源：http://rcx.9152youxi.cn

C#:   Directory.GetFiles("dir")
来源：http://tod.yongpay.top

[F09] 获取文件大小
来源：http://xit.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://ydg.xziqi.cn

PHP:  filesize("a.txt");
来源：http://yky.yongpay.top

JS:   fs.statSync("a.txt").size
来源：http://dcn.kuanghao11.cn

TS:   fs.statSync("a.txt").size
来源：http://zlh.yanxiufei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mcy.ctjpmb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rxp.zhiwuduotai.top

Ruby: File.size("a.txt")
来源：http://eey.haohaochexian.top

C#:   new FileInfo("a.txt").Length
来源：http://pkg.bbcook.cn

[F10] 取文件扩展名 / 文件名
来源：http://rjj.yongpay.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://irt.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qte.pengpengdd.cyou

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qbh.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://xif.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tgk.daxiang520.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://grk.daria6918.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sin.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://khk.svipenyu.cn

[F11] 复制与移动文件
来源：http://twz.xylfe.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ejw.havefunace.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zyx.yanxiufei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vax.guowangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iir.uphjek.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jzn.mhx1999.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dky.hywenlv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lww.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vef.uphjek.com

[F12] CSV 读写
来源：http://xwx.shuidangran.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kzy.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mmy.yuanzhike.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jkc.ybcxt.top

TS:   // 同上
来源：http://auk.yj202588.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://prr.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://seu.svipenyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pnp.yuxming.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://aba.smart0.xyz

================================================================================
来源：http://ijr.52xcode.cn

G. 面向对象
来源：http://yee.kuanghao11.cn

================================================================================
来源：http://zgu.andypj.xyz

[G01] 定义类
来源：http://tyb.yj20258.top

Py:   class User: pass
来源：http://tub.316326.xyz

PHP:  class User {}
来源：http://kmh.xingfuxueyuan.xyz

JS:   class User {}
来源：http://jqq.guannengcc.top

TS:   class User { name: string = ""; }
来源：http://fxk.52xcode.cn

Java: class User {}
来源：http://jxi.sufxvd.cn

Go:   type User struct { Name string }
来源：http://gqs.yongpay.top

Ruby: class User; end
来源：http://xdb.yangfankeji.com

C#:   class User {}
来源：http://sls.ivvv.top

[G02] 构造函数
来源：http://mgp.tian-w.cn

Py:   def __init__(self, name): self.name = name
来源：http://pul.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://xqu.52xcode.cn

JS:   constructor(name) { this.name = name; }
来源：http://mjx.tian-w.cn

TS:   constructor(public name: string) {}
来源：http://tpr.hysaishi.cn

Java: User(String name) { this.name = name; }
来源：http://alm.jyoumei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sgl.jinqigfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://gdx.xuetiantiany.cn

C#:   public User(string name) { Name = name; }
来源：http://lwo.smart0.xyz

[G03] 实例属性
来源：http://lvi.xingfuxueyuan.xyz

Py:   self.name = "x"
来源：http://uvf.fehbvm.com

PHP:  public string $name = "x";
来源：http://nmb.hfpthk.cn

JS:   this.name = "x";
来源：http://joy.daria6918.cn

TS:   name: string = "x";
来源：http://lfy.cheryme.top

Java: private String name;
来源：http://zxr.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vpm.yuanzhike.top

Ruby: @name = "x"
来源：http://trf.jianghu66.top

C#:   public string Name { get; set; } = "x";
来源：http://haq.bjfxy.top

[G04] 定义方法
来源：http://ndd.ydzc1.top

Py:   def greet(self): return self.name
来源：http://uvb.xziqi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rxi.jianghu66.top

JS:   greet() { return this.name; }
来源：http://acy.yfazqb.com

TS:   greet(): string { return this.name; }
来源：http://mhj.ybcxt.top

Java: String greet() { return name; }
来源：http://xku.9152youxi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oum.meibo888.top

Ruby: def greet; @name; end
来源：http://ilk.daxiang520.top

C#:   public string Greet() => Name;
来源：http://jqk.gaohongyu789.top

[G05] 继承
来源：http://gav.0kj1m.cn

Py:   class Admin(User): pass
来源：http://kkh.fanxiaobao.xyz

PHP:  class Admin extends User {}
来源：http://bip.ydjk.org.cn

JS:   class Admin extends User {}
来源：http://wjm.hammf.cn

TS:   class Admin extends User {}
来源：http://abs.hcnkem.com

Java: class Admin extends User {}
来源：http://xjc.tianlin.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://umx.yj20258.top

Ruby: class Admin < User; end
来源：http://qdm.yuxming.cn

C#:   class Admin : User {}
来源：http://msm.xinyue.icu

[G06] 重写方法
来源：http://kuv.pycfn.com

Py:   def greet(self): return "admin"
来源：http://fhx.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bfk.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://ejl.tianlin.xyz

TS:   greet(): string { return "admin"; }
来源：http://tsi.zhaomingkeji.xyz

Java: @Override String greet() { return "admin"; }
来源：http://mrs.dashuyun.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://msm.ywan-chungtsiang.top

Ruby: def greet; "admin"; end
来源：http://hhg.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://kpi.sweek.top

[G07] 调用父类方法
来源：http://cid.havefunace.top

Py:   super().greet()
来源：http://pcb.yongpay.top

PHP:  parent::greet();
来源：http://xnt.jinqigufen.top

JS:   super.greet();
来源：http://qdo.haohaochexian.top

TS:   super.greet();
来源：http://cva.zhiwuduotai.top

Java: super.greet();
来源：http://yom.meibo888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wtz.yongpay.top

Ruby: super
来源：http://cpu.jinqigufen.top

C#:   base.Greet();
来源：http://oqu.zdqjudy.top

[G08] 静态方法与属性
来源：http://puj.iojbl.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://had.yonumen.top

PHP:  public static function f() {}
来源：http://gxs.cashguo.top

JS:   static f() {}
来源：http://epd.ppjwa.cn

TS:   static f(): void {}
来源：http://hyt.uphjek.com

Java: static void f() {}
来源：http://iwq.9152youxi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hhb.shzxlz.cn

Ruby: def self.f; end
来源：http://tiz.hcnkem.com

C#:   public static void F() {}
来源：http://xhh.zhixingplan.top

[G09] 接口 / 抽象类
来源：http://gse.jlsjyb.cn

Py:   from abc import ABC, abstractmethod
来源：http://ehq.hesvh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://owf.yj202588.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tpp.mhx1999.top

TS:   interface Shape { area(): number; }
来源：http://uit.gzhubu.top

Java: interface Shape { double area(); }
来源：http://zrf.guannengcc.top

Go:   type Shape interface { Area() float64 }
来源：http://ciu.haohaochexian.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uvt.hnqzz.top

C#:   interface IShape { double Area(); }
来源：http://iek.zdqjudy.top

[G10] 访问控制
来源：http://oyc.fzhhl.top

Py:   约定 _protected / __private（不强制）
来源：http://usv.jianghu66.top

PHP:  public / protected / private
来源：http://dox.jqgufenzy.top

JS:   #private 字段；其余公开
来源：http://izw.fengsongda.top

TS:   public / protected / private
来源：http://ulz.bbcook.cn

Java: public / protected / private / 默认包级
来源：http://bff.snrcjt.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rwt.xinyue.icu

Ruby: public / protected / private
来源：http://bah.cucudq.cn

C#:   public / protected / private / internal
来源：http://svg.feifeiyinyue.top

[G11] getter / setter
来源：http://ows.gotoacloud.top

Py:   @property 与 @x.setter
来源：http://lcg.ybcxt.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hxz.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://xdo.shuidangran.top

TS:   get name(): string { return this._name; }
来源：http://iqz.hesvh.cn

Java: public String getName() { return name; }
来源：http://wrp.tian-w.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yoy.nwbrower.top

Ruby: attr_accessor :name
来源：http://azh.xinyue.icu

C#:   public string Name { get; set; }
来源：http://sva.shanyushiyangtech.top

[G12] 对象转字符串
来源：http://pxm.yongpay.top

Py:   def __str__(self): return self.name
来源：http://kim.jinqigfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bcr.zdqjudy.top

JS:   toString() { return this.name; }
来源：http://npk.kuanghao11.cn

TS:   toString(): string { return this.name; }
来源：http://ikc.fanxiaobao.xyz

Java: @Override public String toString() { return name; }
来源：http://bva.gotoacloud.top

Go:   func (u User) String() string { return u.Name }
来源：http://clc.hnqzz.top

Ruby: def to_s; @name; end
来源：http://vka.dashuyun.cn

C#:   public override string ToString() => Name;
来源：http://xgk.bjfxy.top

[G13] 判断对象类型
来源：http://ycu.hesvh.cn

Py:   isinstance(u, User)
来源：http://lmb.uphjek.com

PHP:  $u instanceof User
来源：http://wli.epnwcf.com

JS:   u instanceof User
来源：http://pxs.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://dou.shuidangran.top

Java: u instanceof User
来源：http://htp.redwolf501.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yel.mhx1999.top

Ruby: u.is_a?(User)
来源：http://rhx.jiagoushi.top

C#:   u is User
来源：http://npg.iojbl.cn

[G14] 数据类 / record
来源：http://fce.xuanzx.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://brg.cheryme.top

PHP:  // 用 readonly 属性模拟
来源：http://uwa.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pzu.zdqjudy.top

TS:   type User = { name: string; age: number };
来源：http://qtv.zhoulong.xyz

Java: record User(String name, int age) {}
来源：http://uiy.sufxvd.cn

Go:   type User struct { Name string; Age int }
来源：http://glk.xingfuxueyuan.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qdh.zhiwuduotai.top

C#:   record User(string Name, int Age);
来源：http://vcy.vqdsnc.cn

[G15] 枚举
来源：http://pez.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hxf.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jmc.yvedp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lyo.xinyue.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://evc.aibaodan.cn

Java: enum Color { RED, GREEN }
来源：http://yqk.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yxt.jianghu66.top

Ruby: Color = %i[red green].freeze
来源：http://jgl.yj202588.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://idd.wangdashe.top

[G16] 对象转数组 / 字典
来源：http://and.dianchejie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ivo.sxryk.cn

PHP:  get_object_vars($obj);
来源：http://ozp.birdmap.top

JS:   Object.entries(obj)
来源：http://kls.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://uae.zhixingplan.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://flz.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cyb.yj20258.top

Ruby: obj.instance_variables
来源：http://pqs.yj20258888.top

C#:   // 用反射或 System.Text.Json
来源：http://yow.yfazqb.com

================================================================================
来源：http://upd.sysykeji.top

H. 异常与错误处理
来源：http://kuk.zdbjq.cn

================================================================================
来源：http://oev.svipenyu.cn

[H01] try / catch 基础
来源：http://bpi.gotoacloud.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dev.pengpengdd.cyou

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kro.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ozx.guowangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ygw.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rzz.hnxiangtu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yar.sxryk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dby.zhongyouzk.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jxm.haohaochexian.top

[H02] finally / ensure 收尾
来源：http://oho.kuanghao11.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qmd.xinyue.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://slk.hysaishi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://euu.sufxvd.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vfj.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tyw.cdnleiting.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ubf.jinghuilouyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sws.nwbrower.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dpd.zycfv.cn

[H03] 主动抛出异常
来源：http://vas.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://uem.tianlin.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rha.zdbjq.cn

JS:   throw new Error("错误信息");
来源：http://qes.cucudq.cn

TS:   throw new Error("错误信息");
来源：http://zmz.yj20258.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pjs.sweek.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sns.ctjpmb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://dzz.ehwqpu.com

C#:   throw new ArgumentException("错误信息");
来源：http://tzz.nwbrower.top

[H04] 自定义异常类型
来源：http://ibj.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://iqs.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://mxj.zhijiandao.cn

JS:   class MyError extends Error {}
来源：http://jss.jyoumei.cn

TS:   class MyError extends Error {}
来源：http://fvo.shanyushiyangtech.top

Java: class MyException extends RuntimeException {}
来源：http://qdx.xinyue.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lba.ydzc1.top

Ruby: class MyError < StandardError; end
来源：http://bme.wangdashe.top

C#:   class MyException : Exception {}
来源：http://dmm.uphjek.com

[H05] 捕获特定类型
来源：http://kwi.chenzaomai.com

Py:   except ValueError as e:
来源：http://okw.cheryme.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://twd.jlsjyb.cn

JS:   if (e instanceof TypeError) {}
来源：http://png.shangyingyoupin.top

TS:   if (e instanceof TypeError) {}
来源：http://ayx.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://tio.yuxming.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pvt.cheryme.top

Ruby: rescue ArgumentError => e
来源：http://osv.smart0.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yai.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://mfb.xinyue.icu

Py:   value = d.get("k") or default
来源：http://wax.chenzaomai.com

PHP:  $v = $d["k"] ?? null;
来源：http://yqg.jinqigfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://ghi.zhongyouzk.top

TS:   obj?.a?.b;  d ?? default
来源：http://mbs.bjfxy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://urg.cdnleiting.top

Go:   if v, ok := m["k"]; ok { }
来源：http://csf.wangdashe.top

Ruby: d&.dig(:a, :b)
来源：http://ilh.vqdsnc.cn

C#:   obj?.A?.B ?? default
来源：http://wor.uphjek.com

[H07] 断言
来源：http://vim.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://mwr.ydzc1.top

PHP:  assert($x > 0);
来源：http://ibf.nanxuanxn.top

JS:   console.assert(x > 0);
来源：http://lit.jlsjyb.cn


<!-- 参考信息 -->