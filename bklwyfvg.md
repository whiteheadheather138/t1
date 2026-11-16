代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ceh.pycfn.com

Ruby: File.write("a.txt", "hi")
来源：http://ndo.hesvh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://egi.tian-w.cn

[F04] 追加写入文件
来源：http://pwb.aizwys.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lnu.ydjk.org.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ssi.xuanzx.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mtb.zhaomingkeji.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bdw.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ajt.hywenlv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wej.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ncz.aizwys.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://adq.vehdjk.com

[F05] 判断文件或目录是否存在
来源：http://ize.meibo888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wxq.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://fop.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://mvq.jyoumei.cn

TS:   fs.existsSync("a.txt")
来源：http://blw.ivvv.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kel.nanxinkj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nbn.ivvv.top

Ruby: File.exist?("a.txt")
来源：http://hnd.mhx1999.top

C#:   File.Exists("a.txt")
来源：http://ezy.ydjk.org.cn

[F06] 删除文件
来源：http://uvv.yj202588.top

Py:   os.remove("a.txt")
来源：http://rxx.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://mez.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://lox.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://hhb.zdbjq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lwz.shangyingyoupin.top

Go:   os.Remove("a.txt")
来源：http://zhu.dianchejie.cn

Ruby: File.delete("a.txt")
来源：http://rhz.haohaochexian.top

C#:   File.Delete("a.txt");
来源：http://zaa.dianchejie.cn

[F07] 创建目录（含多级）
来源：http://pwk.vqdsnc.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lbb.pycfn.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://psk.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bqo.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dle.gogol.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hyp.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vkd.tarul.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ovn.zhixingplan.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yxh.iojbl.cn

[F08] 遍历目录
来源：http://och.snrcjt.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://npn.zhaomingkeji.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hig.sxryk.cn

JS:   fs.readdirSync("dir")
来源：http://odx.pengpengdd.cyou

TS:   fs.readdirSync("dir")
来源：http://idk.daria6918.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wyp.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vzq.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://rmg.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://lpg.iojbl.cn

[F09] 获取文件大小
来源：http://dkk.ehwqpu.com

Py:   os.path.getsize("a.txt")
来源：http://hhi.wangdashe.top

PHP:  filesize("a.txt");
来源：http://hgy.ybcxt.top

JS:   fs.statSync("a.txt").size
来源：http://urj.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://uzb.zhixingplan.top

Java: Files.size(Path.of("a.txt"))
来源：http://ypl.sxryk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dtt.hongshengwenyu.top

Ruby: File.size("a.txt")
来源：http://grv.zhoulong.xyz

C#:   new FileInfo("a.txt").Length
来源：http://txg.jinqigfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://ubw.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mmo.jinqigfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hjp.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xza.zhoulong.xyz

TS:   path.extname("a.txt")
来源：http://bfd.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jyt.feifeiyinyue.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kgr.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kre.zhoulong.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nta.zhixingplan.top

[F11] 复制与移动文件
来源：http://apb.dianchejie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bbn.yfazqb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rak.ywan-chungtsiang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xhs.xziqi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://viq.zdbjq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kfz.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jyq.chenlongwang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ubb.aibaodan.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ond.yj20258.top

[F12] CSV 读写
来源：http://bsy.epnwcf.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ket.feifeiyinyue.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bxk.hywenlv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mdv.sweek.top

TS:   // 同上
来源：http://lqg.52xcode.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zfj.ivvv.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xeo.chenlongwang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jlm.jianghu66.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ams.sufxvd.cn

================================================================================
来源：http://eef.tarul.cn

G. 面向对象
来源：http://bca.sxryk.cn

================================================================================
来源：http://otq.nanxinkj.top

[G01] 定义类
来源：http://qfx.cdnleiting.top

Py:   class User: pass
来源：http://uqy.xinyue.icu

PHP:  class User {}
来源：http://zng.ywan-chungtsiang.top

JS:   class User {}
来源：http://ehu.ehwqpu.com

TS:   class User { name: string = ""; }
来源：http://ttq.aibaodan.cn

Java: class User {}
来源：http://uid.hongshengwenyu.top

Go:   type User struct { Name string }
来源：http://rgh.meibo888.top

Ruby: class User; end
来源：http://sci.c1oappe.top

C#:   class User {}
来源：http://ryk.ivvv.top

[G02] 构造函数
来源：http://shh.shangyingyoupin.top

Py:   def __init__(self, name): self.name = name
来源：http://knj.guannengcc.top

PHP:  public function __construct(public string $name) {}
来源：http://biu.yj202588.top

JS:   constructor(name) { this.name = name; }
来源：http://nmh.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://val.daria6918.cn

Java: User(String name) { this.name = name; }
来源：http://pra.fzhhl.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fga.yongpay.top

Ruby: def initialize(name); @name = name; end
来源：http://hod.havefunace.top

C#:   public User(string name) { Name = name; }
来源：http://sfo.ywan-chungtsiang.top

[G03] 实例属性
来源：http://ulw.jinqigufen.top

Py:   self.name = "x"
来源：http://kng.ydjk.org.cn

PHP:  public string $name = "x";
来源：http://bwk.fzhhl.top

JS:   this.name = "x";
来源：http://vwp.wangshuangyany.cn

TS:   name: string = "x";
来源：http://ini.chenzaomai.com

Java: private String name;
来源：http://uhj.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gqp.chenlongwang.top

Ruby: @name = "x"
来源：http://qsl.9152youxi.cn

C#:   public string Name { get; set; } = "x";
来源：http://spt.hywenlv.cn

[G04] 定义方法
来源：http://qyu.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://mml.gogol.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://srr.guowangkeji.top

JS:   greet() { return this.name; }
来源：http://juw.sxryk.cn

TS:   greet(): string { return this.name; }
来源：http://nqf.xinyue.icu

Java: String greet() { return name; }
来源：http://ibu.haohaochexian.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://epi.guannengcc.top

Ruby: def greet; @name; end
来源：http://mlm.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://xav.snrcjt.cn

[G05] 继承
来源：http://axg.zhongyouzk.top

Py:   class Admin(User): pass
来源：http://nuu.tarul.cn

PHP:  class Admin extends User {}
来源：http://nie.hfpthk.cn

JS:   class Admin extends User {}
来源：http://mog.xuanzx.com

TS:   class Admin extends User {}
来源：http://bax.chenzaomai.com

Java: class Admin extends User {}
来源：http://mvg.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yua.hysaishi.cn

Ruby: class Admin < User; end
来源：http://yud.yfazqb.com

C#:   class Admin : User {}
来源：http://nsg.gaohongyu789.top

[G06] 重写方法
来源：http://nks.shuidangran.top

Py:   def greet(self): return "admin"
来源：http://dqk.ctjpmb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://gdt.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://swc.pycfn.com

TS:   greet(): string { return "admin"; }
来源：http://gsf.jianghu66.top

Java: @Override String greet() { return "admin"; }
来源：http://fsm.ydjk.org.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vcg.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://sof.vehdjk.com

C#:   public override string Greet() => "admin";
来源：http://bdg.vqdsnc.cn

[G07] 调用父类方法
来源：http://ots.svipenyu.cn

Py:   super().greet()
来源：http://dyk.guannengcc.top

PHP:  parent::greet();
来源：http://npc.zhongyouzk.top

JS:   super.greet();
来源：http://erl.mhx1999.top

TS:   super.greet();
来源：http://orp.zhijiandao.cn

Java: super.greet();
来源：http://lsu.wangshuangyany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wum.ivvv.top

Ruby: super
来源：http://xaw.fengsongda.top

C#:   base.Greet();
来源：http://yhn.fzhhl.top

[G08] 静态方法与属性
来源：http://nfc.fzhhl.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mga.gogol.net.cn

PHP:  public static function f() {}
来源：http://blq.aizwys.cn

JS:   static f() {}
来源：http://fai.wangdashe.top

TS:   static f(): void {}
来源：http://exo.yongpay.top

Java: static void f() {}
来源：http://cyu.nwbrower.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jln.feifeiyinyue.top

Ruby: def self.f; end
来源：http://lwm.daria6918.cn

C#:   public static void F() {}
来源：http://cmr.shanyushiyangkeji.top

[G09] 接口 / 抽象类
来源：http://aki.mhx1999.top

Py:   from abc import ABC, abstractmethod
来源：http://awl.gzhubu.top

PHP:  interface Shape { public function area(): float; }
来源：http://bhn.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bxs.cheryme.top

TS:   interface Shape { area(): number; }
来源：http://odf.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://ljj.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://ysx.wangdashe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sup.ivvv.top

C#:   interface IShape { double Area(); }
来源：http://qak.ehwqpu.com

[G10] 访问控制
来源：http://gbd.jyoumei.cn

Py:   约定 _protected / __private（不强制）
来源：http://wnn.yanxiufei.cn

PHP:  public / protected / private
来源：http://sli.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://gkt.zhoulong.xyz

TS:   public / protected / private
来源：http://svi.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://yms.tanke756.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gvz.tianlin.xyz

Ruby: public / protected / private
来源：http://zbs.nanxinkj.top

C#:   public / protected / private / internal
来源：http://day.cheryme.top

[G11] getter / setter
来源：http://zrt.wangshuangyany.cn

Py:   @property 与 @x.setter
来源：http://jnh.fzhhl.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gif.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://tmx.jinqigufen.top

TS:   get name(): string { return this._name; }
来源：http://gxe.bbcook.cn

Java: public String getName() { return name; }
来源：http://tsk.xylfe.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bhy.hongshengwenyu.top

Ruby: attr_accessor :name
来源：http://ect.chenlongwang.top

C#:   public string Name { get; set; }
来源：http://wnt.tanke756.top

[G12] 对象转字符串
来源：http://wso.chenjidiqi.icu

Py:   def __str__(self): return self.name
来源：http://vcf.vqdsnc.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ndy.yueranfly.top

JS:   toString() { return this.name; }
来源：http://nru.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://hxr.zhongyouzk.top

Java: @Override public String toString() { return name; }
来源：http://lhg.guowangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://xtw.bbcook.cn

Ruby: def to_s; @name; end
来源：http://tlk.hnqzz.top

C#:   public override string ToString() => Name;
来源：http://btu.sweek.top

[G13] 判断对象类型
来源：http://ljo.zycfv.cn

Py:   isinstance(u, User)
来源：http://zzp.ydjk.org.cn

PHP:  $u instanceof User
来源：http://nxp.sufxvd.cn

JS:   u instanceof User
来源：http://cuy.shzxlz.cn

TS:   u instanceof User
来源：http://bab.aizwys.cn

Java: u instanceof User
来源：http://ofa.yueranfly.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nyf.9152youxi.cn

Ruby: u.is_a?(User)
来源：http://ayf.jiagoushi.top

C#:   u is User
来源：http://wou.daxiang520.top

[G14] 数据类 / record
来源：http://cig.jyoumei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qyy.sysykeji.top

PHP:  // 用 readonly 属性模拟
来源：http://puy.c1oappe.top

JS:   // 无内置：普通类或对象字面量
来源：http://tmz.cqqwz.cn

TS:   type User = { name: string; age: number };
来源：http://inq.hnqzz.top

Java: record User(String name, int age) {}
来源：http://qsr.ppjwa.cn

Go:   type User struct { Name string; Age int }
来源：http://xuo.shanyushiyangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ute.bbcook.cn

C#:   record User(string Name, int Age);
来源：http://cmg.sxryk.cn

[G15] 枚举
来源：http://hdf.yuxming.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qru.svipenyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qgu.yongpay.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wqh.zdqjudy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cem.ehwqpu.com

Java: enum Color { RED, GREEN }
来源：http://wpm.havefunace.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://phj.jinqigufen.top

Ruby: Color = %i[red green].freeze
来源：http://hhi.tian-w.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://spr.sweek.top

[G16] 对象转数组 / 字典
来源：http://ucj.tian-w.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://obk.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://eow.52xcode.cn

JS:   Object.entries(obj)
来源：http://ium.zhengqikj.top

TS:   Object.entries(obj)
来源：http://tex.hongshengwenyu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kxl.shuidangran.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ejp.fzhhl.top

Ruby: obj.instance_variables
来源：http://kgr.andypj.xyz

C#:   // 用反射或 System.Text.Json
来源：http://ucu.hongshengwenyu.top

================================================================================
来源：http://lia.nwbrower.top

H. 异常与错误处理
来源：http://vju.vehdjk.com

================================================================================
来源：http://xrj.havefunace.top

[H01] try / catch 基础
来源：http://cdk.fehbvm.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hdl.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xvn.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ecz.aibaodan.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fgu.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kgc.wangshuangyany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ffi.chenlongwang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qgk.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hcv.kuanghao11.cn

[H02] finally / ensure 收尾
来源：http://vqy.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://mhg.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qgk.dianchejie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ebz.epnwcf.com

TS:   try { f(); } finally { cleanup(); }
来源：http://dxt.zdbjq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://enu.aibaodan.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wla.daxiang520.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pmr.ywan-chungtsiang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gvm.cqqwz.cn

[H03] 主动抛出异常
来源：http://uan.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://xqf.zhoulong.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ciz.quarkkingdee.top

JS:   throw new Error("错误信息");
来源：http://slm.iojbl.cn

TS:   throw new Error("错误信息");
来源：http://hng.aizwys.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vhe.pengpengdd.cyou

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cim.ywan-chungtsiang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xxa.hysaishi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vhu.vehdjk.com

[H04] 自定义异常类型
来源：http://dof.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://kko.daria6918.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mxh.vqdsnc.cn

JS:   class MyError extends Error {}
来源：http://juy.guannengcc.top

TS:   class MyError extends Error {}
来源：http://ocr.ywan-chungtsiang.top

Java: class MyException extends RuntimeException {}
来源：http://wwh.jinyuanbaomall.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qwp.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://zkp.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://mpa.hnqzz.top

[H05] 捕获特定类型
来源：http://wkf.cdnleiting.top

Py:   except ValueError as e:
来源：http://ujs.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://atw.nanxinkj.top

JS:   if (e instanceof TypeError) {}
来源：http://uln.uphjek.com

TS:   if (e instanceof TypeError) {}
来源：http://ams.gotoacloud.top

Java: catch (IOException | SQLException e) {}
来源：http://hxa.yfazqb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hqr.nanxuanxn.top

Ruby: rescue ArgumentError => e
来源：http://osp.ehwqpu.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://typ.bjfxy.top

[H06] 可选值 / 空值安全访问
来源：http://xsn.gzhubu.top

Py:   value = d.get("k") or default
来源：http://lyo.shanyushiyangtech.top

PHP:  $v = $d["k"] ?? null;
来源：http://wdm.zhongyouzk.top

JS:   obj?.a?.b;  d ?? default
来源：http://czn.52xcode.cn

TS:   obj?.a?.b;  d ?? default
来源：http://knq.fzhhl.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vkl.shanyushiyangtech.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ahu.ywan-chungtsiang.top

Ruby: d&.dig(:a, :b)
来源：http://dzc.fzhhl.top

C#:   obj?.A?.B ?? default
来源：http://pkq.vehdjk.com

[H07] 断言
来源：http://klc.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://oad.iojbl.cn

PHP:  assert($x > 0);
来源：http://fkc.sysykeji.top

JS:   console.assert(x > 0);
来源：http://hep.52xcode.cn

TS:   console.assert(x > 0);
来源：http://lkx.yfazqb.com

Java: assert x > 0 : "必须为正";
来源：http://ltr.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kqv.uphjek.com

Ruby: raise "必须为正" unless x > 0
来源：http://sfp.gaohongyu789.top

C#:   Debug.Assert(x > 0);
来源：http://zgr.ydzc1.top

[H08] 获取错误信息与堆栈
来源：http://oon.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://tap.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zvu.guannengcc.top


<!-- 参考信息 -->