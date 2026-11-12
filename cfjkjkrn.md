代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://rzi.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mmz.cucudq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ezn.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://voq.pycfn.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://try.jiagoushi.top

Ruby: File.write("a.txt", "hi")
来源：http://jzj.316326.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://daz.hcnkem.com

[F04] 追加写入文件
来源：http://wed.snrcjt.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zfr.hfpthk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ygl.bjfxy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vlr.gzhubu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mgd.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iml.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gbz.nanxinkj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dke.52xcode.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ukd.shanyushiyangkeji.top

[F05] 判断文件或目录是否存在
来源：http://ngo.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pjm.sufxvd.cn

PHP:  file_exists("a.txt");
来源：http://fen.shanyushiyangtech.top

JS:   fs.existsSync("a.txt")
来源：http://ore.chenlongwang.top

TS:   fs.existsSync("a.txt")
来源：http://pov.meibo888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://agg.yfazqb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qws.jinghuilouyu.cn

Ruby: File.exist?("a.txt")
来源：http://dvb.ctjpmb.com

C#:   File.Exists("a.txt")
来源：http://uwu.xuetiantiany.cn

[F06] 删除文件
来源：http://pkc.xylfe.cn

Py:   os.remove("a.txt")
来源：http://puk.zhongyouzk.top

PHP:  unlink("a.txt");
来源：http://lgt.zdqjudy.top

JS:   fs.unlinkSync("a.txt")
来源：http://gkq.yuxming.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fhu.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rfe.zhoulong.xyz

Go:   os.Remove("a.txt")
来源：http://tcf.xylfe.cn

Ruby: File.delete("a.txt")
来源：http://uqf.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://dit.nwbrower.top

[F07] 创建目录（含多级）
来源：http://jso.zhengqikj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lji.wangdashe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zsx.hysaishi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hiz.jinghuilouyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://waj.redwolf501.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://adi.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bhq.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yup.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zwa.chenjidiqi.icu

[F08] 遍历目录
来源：http://myp.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://she.jinghuilouyu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hic.iojbl.cn

JS:   fs.readdirSync("dir")
来源：http://skf.zhongyouzk.top

TS:   fs.readdirSync("dir")
来源：http://zyj.316326.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kdy.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://fza.yuanzhike.top

Ruby: Dir.children("dir")
来源：http://fnx.tarul.cn

C#:   Directory.GetFiles("dir")
来源：http://mmt.fehbvm.com

[F09] 获取文件大小
来源：http://eei.jinghuilouyu.cn

Py:   os.path.getsize("a.txt")
来源：http://vfo.ydjk.org.cn

PHP:  filesize("a.txt");
来源：http://ine.cdnleiting.top

JS:   fs.statSync("a.txt").size
来源：http://snr.hfpthk.cn

TS:   fs.statSync("a.txt").size
来源：http://uyb.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://anm.zycfv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aby.sjlbkw.cn

Ruby: File.size("a.txt")
来源：http://vyo.0kj1m.cn

C#:   new FileInfo("a.txt").Length
来源：http://bsi.yuanzhike.top

[F10] 取文件扩展名 / 文件名
来源：http://uer.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://scq.fehbvm.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://koy.yonumen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mlq.sjlbkw.cn

TS:   path.extname("a.txt")
来源：http://wiw.yangfankeji.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://neh.yuanzhike.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rvm.zhaomingkeji.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nju.iojbl.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rxu.jqgfzy.top

[F11] 复制与移动文件
来源：http://utd.ppjwa.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vcl.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nxp.ywan-chungtsiang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://djr.svipenyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://opv.tanke756.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vsh.bbcook.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ija.jqgfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://exp.vqdsnc.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tya.vehdjk.com

[F12] CSV 读写
来源：http://ody.tian-w.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gff.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eci.fzhhl.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nvo.hnxiangtu.top

TS:   // 同上
来源：http://blf.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ihn.gotoacloud.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ecg.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qwz.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://rxy.sysykeji.top

================================================================================
来源：http://miw.xingfuxueyuan.xyz

G. 面向对象
来源：http://mbg.ctjpmb.com

================================================================================
来源：http://dtk.ivvv.top

[G01] 定义类
来源：http://wkg.zhixingplan.top

Py:   class User: pass
来源：http://nid.ydzc1.top

PHP:  class User {}
来源：http://rki.snrcjt.cn

JS:   class User {}
来源：http://xny.yj202588.top

TS:   class User { name: string = ""; }
来源：http://gkb.yj20258.top

Java: class User {}
来源：http://nzh.sufxvd.cn

Go:   type User struct { Name string }
来源：http://hpb.tianlin.xyz

Ruby: class User; end
来源：http://kcj.cdnleiting.top

C#:   class User {}
来源：http://eyx.zdbjq.cn

[G02] 构造函数
来源：http://epj.guannengcc.top

Py:   def __init__(self, name): self.name = name
来源：http://sjw.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://rho.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://ymr.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://ojd.hcnkem.com

Java: User(String name) { this.name = name; }
来源：http://puu.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gkq.zhijiandao.cn

Ruby: def initialize(name); @name = name; end
来源：http://qfd.chenjidiqi.icu

C#:   public User(string name) { Name = name; }
来源：http://kbk.fzhhl.top

[G03] 实例属性
来源：http://hzd.zhijiandao.cn

Py:   self.name = "x"
来源：http://rqs.shanyushiyangtech.top

PHP:  public string $name = "x";
来源：http://qri.c1oappe.top

JS:   this.name = "x";
来源：http://suq.yongpay.top

TS:   name: string = "x";
来源：http://zdz.hywenlv.cn

Java: private String name;
来源：http://fng.hysaishi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fxv.hnqzz.top

Ruby: @name = "x"
来源：http://nsk.gaohongyu789.top

C#:   public string Name { get; set; } = "x";
来源：http://ads.cucudq.cn

[G04] 定义方法
来源：http://nof.jqgufenzy.top

Py:   def greet(self): return self.name
来源：http://zhc.hysaishi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://luv.cucudq.cn

JS:   greet() { return this.name; }
来源：http://nqz.yvedp.cn

TS:   greet(): string { return this.name; }
来源：http://jaz.aibaodan.cn

Java: String greet() { return name; }
来源：http://woa.yj202588.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ngm.hysaishi.cn

Ruby: def greet; @name; end
来源：http://csl.wangshuangyany.cn

C#:   public string Greet() => Name;
来源：http://mbs.sufxvd.cn

[G05] 继承
来源：http://gil.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://ckb.bjfxy.top

PHP:  class Admin extends User {}
来源：http://bda.dashuyun.cn

JS:   class Admin extends User {}
来源：http://xbw.ehwqpu.com

TS:   class Admin extends User {}
来源：http://lht.sxryk.cn

Java: class Admin extends User {}
来源：http://nxw.hysaishi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ckh.jinqigfzy.top

Ruby: class Admin < User; end
来源：http://nev.xuanzx.com

C#:   class Admin : User {}
来源：http://bep.xylfe.cn

[G06] 重写方法
来源：http://syc.havefunace.top

Py:   def greet(self): return "admin"
来源：http://fme.redwolf501.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gvm.ywan-chungtsiang.top

JS:   greet() { return "admin"; }
来源：http://vet.ydzc1.top

TS:   greet(): string { return "admin"; }
来源：http://dxl.redwolf501.top

Java: @Override String greet() { return "admin"; }
来源：http://vmv.xylfe.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hsn.ivvv.top

Ruby: def greet; "admin"; end
来源：http://oab.zhongyouzk.top

C#:   public override string Greet() => "admin";
来源：http://mmy.gotoacloud.top

[G07] 调用父类方法
来源：http://hlp.dianchejie.cn

Py:   super().greet()
来源：http://xwc.yonumen.top

PHP:  parent::greet();
来源：http://rec.ehwqpu.com

JS:   super.greet();
来源：http://ews.hfpthk.cn

TS:   super.greet();
来源：http://uuh.nwbrower.top

Java: super.greet();
来源：http://ggp.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://asi.c1oappe.top

Ruby: super
来源：http://fqv.vqdsnc.cn

C#:   base.Greet();
来源：http://eft.jiagoushi.top

[G08] 静态方法与属性
来源：http://sdf.yueranfly.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fns.jinghuilouyu.cn

PHP:  public static function f() {}
来源：http://tut.daria6918.cn

JS:   static f() {}
来源：http://qmy.gotoacloud.top

TS:   static f(): void {}
来源：http://ulz.jinqigufen.top

Java: static void f() {}
来源：http://zhm.epnwcf.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://qnr.jlsjyb.cn

Ruby: def self.f; end
来源：http://aua.cdnleiting.top

C#:   public static void F() {}
来源：http://zpy.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://xry.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://ghd.cucudq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lso.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nmj.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://yof.cdnleiting.top

Java: interface Shape { double area(); }
来源：http://dst.yuanzhike.top

Go:   type Shape interface { Area() float64 }
来源：http://qqo.fanxiaobao.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qww.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://pmr.zhaomingkeji.xyz

[G10] 访问控制
来源：http://vxw.wangdashe.top

Py:   约定 _protected / __private（不强制）
来源：http://nrz.yongpay.top

PHP:  public / protected / private
来源：http://mmu.ywan-chungtsiang.top

JS:   #private 字段；其余公开
来源：http://hjm.pengpengdd.cyou

TS:   public / protected / private
来源：http://jji.ivvv.top

Java: public / protected / private / 默认包级
来源：http://shg.havefunace.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fde.hysaishi.cn

Ruby: public / protected / private
来源：http://syr.yj20258888.top

C#:   public / protected / private / internal
来源：http://dpt.zhengqikj.top

[G11] getter / setter
来源：http://ygf.mhx1999.top

Py:   @property 与 @x.setter
来源：http://suu.52xcode.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gsi.feifeiyinyue.top

JS:   get name() { return this._name; }
来源：http://yhs.quarkkingdee.top

TS:   get name(): string { return this._name; }
来源：http://sij.aizwys.cn

Java: public String getName() { return name; }
来源：http://vea.yangfankeji.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://soi.ivvv.top

Ruby: attr_accessor :name
来源：http://wcs.aibaodan.cn

C#:   public string Name { get; set; }
来源：http://lro.vehdjk.com

[G12] 对象转字符串
来源：http://gxw.birdmap.top

Py:   def __str__(self): return self.name
来源：http://ggu.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pli.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://jex.yonumen.top

TS:   toString(): string { return this.name; }
来源：http://shb.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://hdf.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://rnw.gotoacloud.top

Ruby: def to_s; @name; end
来源：http://iml.bbcook.cn

C#:   public override string ToString() => Name;
来源：http://imu.yongpay.top

[G13] 判断对象类型
来源：http://pbe.wangdashe.top

Py:   isinstance(u, User)
来源：http://npm.smart0.xyz

PHP:  $u instanceof User
来源：http://plo.yj202588.top

JS:   u instanceof User
来源：http://ybx.zdbjq.cn

TS:   u instanceof User
来源：http://vyd.meibo888.top

Java: u instanceof User
来源：http://ubr.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ufw.sweek.top

Ruby: u.is_a?(User)
来源：http://ogf.wangshuangyany.cn

C#:   u is User
来源：http://hbu.yanxiufei.cn

[G14] 数据类 / record
来源：http://jbq.hcnkem.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qhv.yanxiufei.cn

PHP:  // 用 readonly 属性模拟
来源：http://oyg.jinghuilouyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xoc.wangdashe.top

TS:   type User = { name: string; age: number };
来源：http://bon.ctjpmb.com

Java: record User(String name, int age) {}
来源：http://gbm.yfazqb.com

Go:   type User struct { Name string; Age int }
来源：http://efb.jianghu66.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hqm.yongpay.top

C#:   record User(string Name, int Age);
来源：http://ivh.316326.xyz

[G15] 枚举
来源：http://zdx.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ral.aibaodan.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bwp.fzhhl.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nmn.sysykeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nnp.vehdjk.com

Java: enum Color { RED, GREEN }
来源：http://bbi.jyoumei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ppa.gotoacloud.top

Ruby: Color = %i[red green].freeze
来源：http://abk.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://glg.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://omy.c1oappe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ahk.0kj1m.cn

PHP:  get_object_vars($obj);
来源：http://fel.zdqjudy.top

JS:   Object.entries(obj)
来源：http://oqt.hnqzz.top

TS:   Object.entries(obj)
来源：http://ygd.shanyushiyangtech.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sxq.sweek.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mzo.yuanzhike.top

Ruby: obj.instance_variables
来源：http://muw.pycfn.com

C#:   // 用反射或 System.Text.Json
来源：http://uyj.zhaomingkeji.xyz

================================================================================
来源：http://nhz.sjlbkw.cn

H. 异常与错误处理
来源：http://brg.cashguo.top

================================================================================
来源：http://vvd.hammf.cn

[H01] try / catch 基础
来源：http://ouk.shanyushiyangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wwj.zycfv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dcj.fehbvm.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iic.pycfn.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://grz.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rva.hongshengwenyu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jlu.shanyushiyangtech.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mpw.ydzc1.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eqe.fktsv.cn

[H02] finally / ensure 收尾
来源：http://isp.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://iod.sysykeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kir.fzhhl.top

JS:   try { f(); } finally { cleanup(); }
来源：http://irs.yongpay.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kgr.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ujw.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://zac.zdqjudy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wxl.xuetiantiany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hhb.shzxlz.cn

[H03] 主动抛出异常
来源：http://iaj.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://teu.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://erc.nwbrower.top

JS:   throw new Error("错误信息");
来源：http://rut.gaohongyu789.top

TS:   throw new Error("错误信息");
来源：http://wux.yj20258.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qym.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eie.fktsv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fve.yuxming.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ncy.xuetiantiany.cn

[H04] 自定义异常类型
来源：http://cee.daria6918.cn

Py:   class MyError(Exception): pass
来源：http://dxf.yangfankeji.com

PHP:  class MyError extends RuntimeException {}
来源：http://owu.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://sbw.kuanghao11.cn

TS:   class MyError extends Error {}
来源：http://otv.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://cee.zhoulong.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ghn.tanke756.top

Ruby: class MyError < StandardError; end
来源：http://gbk.yuanzhike.top

C#:   class MyException : Exception {}
来源：http://zcc.dashuyun.cn

[H05] 捕获特定类型
来源：http://rml.ybcxt.top

Py:   except ValueError as e:
来源：http://ncl.yvedp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gpu.zhaomingkeji.xyz

JS:   if (e instanceof TypeError) {}
来源：http://huh.cdnleiting.top

TS:   if (e instanceof TypeError) {}
来源：http://jkh.jqgfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://nwt.zycfv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jcx.chenzaomai.com

Ruby: rescue ArgumentError => e
来源：http://ybm.wangdashe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://abu.xylfe.cn

[H06] 可选值 / 空值安全访问
来源：http://fjn.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://dno.hcnkem.com

PHP:  $v = $d["k"] ?? null;
来源：http://pcv.zhixingplan.top

JS:   obj?.a?.b;  d ?? default
来源：http://kwr.xuetiantiany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dde.hysaishi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://elh.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ptr.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://taj.ydzc1.top

C#:   obj?.A?.B ?? default
来源：http://pmy.fengsongda.top

[H07] 断言
来源：http://nds.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://atx.chenlongwang.top

PHP:  assert($x > 0);
来源：http://llr.tarul.cn

JS:   console.assert(x > 0);
来源：http://iid.zhongyouzk.top

TS:   console.assert(x > 0);
来源：http://cvt.hongshengwenyu.top

Java: assert x > 0 : "必须为正";
来源：http://jbp.redwolf501.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jii.yfazqb.com

Ruby: raise "必须为正" unless x > 0
来源：http://ofv.fengsongda.top


<!-- 参考信息 -->