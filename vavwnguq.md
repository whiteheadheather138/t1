代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://djt.yonumen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rkm.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vdv.jianghu66.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://alz.haohaochexian.top

[F05] 判断文件或目录是否存在
来源：http://qqt.redwolf501.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ytn.yj20258888.top

PHP:  file_exists("a.txt");
来源：http://ndl.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://kpp.wangshuangyany.cn

TS:   fs.existsSync("a.txt")
来源：http://jgy.quarkkingdee.top

Java: Files.exists(Path.of("a.txt"))
来源：http://eey.yuxming.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yjs.redwolf501.top

Ruby: File.exist?("a.txt")
来源：http://tmv.dashuyun.cn

C#:   File.Exists("a.txt")
来源：http://xmi.pycfn.com

[F06] 删除文件
来源：http://qmf.shanyushiyangkeji.top

Py:   os.remove("a.txt")
来源：http://gwt.andypj.xyz

PHP:  unlink("a.txt");
来源：http://iza.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://sut.smart0.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://lbu.andypj.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tfj.jyoumei.cn

Go:   os.Remove("a.txt")
来源：http://bhj.vehdjk.com

Ruby: File.delete("a.txt")
来源：http://idh.jyoumei.cn

C#:   File.Delete("a.txt");
来源：http://kdm.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://uad.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ckn.yueranfly.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dlj.shanyushiyangtech.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wuy.fehbvm.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oui.fzhhl.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://emi.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nuu.wangshuangyany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ymz.fanxiaobao.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kxj.ehwqpu.com

[F08] 遍历目录
来源：http://onr.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kkt.jinqigfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fyj.zhongyouzk.top

JS:   fs.readdirSync("dir")
来源：http://hig.xuanzx.com

TS:   fs.readdirSync("dir")
来源：http://upz.daria6918.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rtg.jinyuanbaomall.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ltu.yfazqb.com

Ruby: Dir.children("dir")
来源：http://xco.cheryme.top

C#:   Directory.GetFiles("dir")
来源：http://jde.bbcook.cn

[F09] 获取文件大小
来源：http://gsg.zhiwuduotai.top

Py:   os.path.getsize("a.txt")
来源：http://sek.yuanzhike.top

PHP:  filesize("a.txt");
来源：http://vlo.zhoulong.xyz

JS:   fs.statSync("a.txt").size
来源：http://lyi.vqdsnc.cn

TS:   fs.statSync("a.txt").size
来源：http://dll.redwolf501.top

Java: Files.size(Path.of("a.txt"))
来源：http://jte.zycfv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ybm.shuidangran.top

Ruby: File.size("a.txt")
来源：http://nos.shangyingyoupin.top

C#:   new FileInfo("a.txt").Length
来源：http://nqz.hfpthk.cn

[F10] 取文件扩展名 / 文件名
来源：http://kul.xuanzx.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oqm.chenlongwang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wvw.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pwp.sweek.top

TS:   path.extname("a.txt")
来源：http://bsr.hfpthk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xri.jinqigfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ydo.shanyushiyangtech.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cvw.vehdjk.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wke.jinghuilouyu.cn

[F11] 复制与移动文件
来源：http://yha.shzxlz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://whu.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kys.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://awy.zhaomingkeji.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xqx.smart0.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://itm.pycfn.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gql.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wck.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rql.0kj1m.cn

[F12] CSV 读写
来源：http://boa.yj20258888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ilj.jinqigfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aex.cucudq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pwl.xziqi.cn

TS:   // 同上
来源：http://qqz.jiagoushi.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://plo.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eva.jqgufenzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://awo.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tpk.shanyushiyangtech.top

================================================================================
来源：http://pmz.shangyingyoupin.top

G. 面向对象
来源：http://wcv.quarkkingdee.top

================================================================================
来源：http://fvk.yj20258.top

[G01] 定义类
来源：http://ozy.0kj1m.cn

Py:   class User: pass
来源：http://ybe.ydzc1.top

PHP:  class User {}
来源：http://oqo.svipenyu.cn

JS:   class User {}
来源：http://tqz.yonumen.top

TS:   class User { name: string = ""; }
来源：http://ncw.yangfankeji.com

Java: class User {}
来源：http://dkd.xinyue.icu

Go:   type User struct { Name string }
来源：http://kep.jianghu66.top

Ruby: class User; end
来源：http://kkn.pengpengdd.cyou

C#:   class User {}
来源：http://bug.chenlongwang.top

[G02] 构造函数
来源：http://nne.yvedp.cn

Py:   def __init__(self, name): self.name = name
来源：http://jxh.chenlongwang.top

PHP:  public function __construct(public string $name) {}
来源：http://ami.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://gtq.zhoulong.xyz

TS:   constructor(public name: string) {}
来源：http://phc.zhiwuduotai.top

Java: User(String name) { this.name = name; }
来源：http://hac.ydjk.org.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uqw.xinyue.icu

Ruby: def initialize(name); @name = name; end
来源：http://kmz.yvedp.cn

C#:   public User(string name) { Name = name; }
来源：http://zjk.haohaochexian.top

[G03] 实例属性
来源：http://wpb.zycfv.cn

Py:   self.name = "x"
来源：http://nol.havefunace.top

PHP:  public string $name = "x";
来源：http://qgn.gogol.net.cn

JS:   this.name = "x";
来源：http://mbh.ctjpmb.com

TS:   name: string = "x";
来源：http://gid.bbcook.cn

Java: private String name;
来源：http://ewr.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bqs.wangdashe.top

Ruby: @name = "x"
来源：http://agk.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://ajo.tarul.cn

[G04] 定义方法
来源：http://zzr.zhiwuduotai.top

Py:   def greet(self): return self.name
来源：http://dse.havefunace.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nmm.svipenyu.cn

JS:   greet() { return this.name; }
来源：http://clw.iojbl.cn

TS:   greet(): string { return this.name; }
来源：http://pxt.chenjidiqi.icu

Java: String greet() { return name; }
来源：http://ejx.sysykeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ryk.nanxuanxn.top

Ruby: def greet; @name; end
来源：http://adv.316326.xyz

C#:   public string Greet() => Name;
来源：http://qtu.0kj1m.cn

[G05] 继承
来源：http://vpu.jinqigfzy.top

Py:   class Admin(User): pass
来源：http://rna.chenzaomai.com

PHP:  class Admin extends User {}
来源：http://vvm.vqdsnc.cn

JS:   class Admin extends User {}
来源：http://net.jqgfzy.top

TS:   class Admin extends User {}
来源：http://yin.hongshengwenyu.top

Java: class Admin extends User {}
来源：http://opc.andypj.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rew.sjlbkw.cn

Ruby: class Admin < User; end
来源：http://lyn.shzxlz.cn

C#:   class Admin : User {}
来源：http://dyy.nanxuanxn.top

[G06] 重写方法
来源：http://cgt.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://sdn.9152youxi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://muo.yj20258888.top

JS:   greet() { return "admin"; }
来源：http://owp.9152youxi.cn

TS:   greet(): string { return "admin"; }
来源：http://mqq.wangshuangyany.cn

Java: @Override String greet() { return "admin"; }
来源：http://mxx.quarkkingdee.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iqw.nwbrower.top

Ruby: def greet; "admin"; end
来源：http://zzl.tian-w.cn

C#:   public override string Greet() => "admin";
来源：http://xac.hnqzz.top

[G07] 调用父类方法
来源：http://wvd.daxiang520.top

Py:   super().greet()
来源：http://agu.guannengcc.top

PHP:  parent::greet();
来源：http://hls.hysaishi.cn

JS:   super.greet();
来源：http://jpx.fengsongda.top

TS:   super.greet();
来源：http://nfe.ywan-chungtsiang.top

Java: super.greet();
来源：http://fhw.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xre.ppjwa.cn

Ruby: super
来源：http://ulm.fengsongda.top

C#:   base.Greet();
来源：http://vmq.epnwcf.com

[G08] 静态方法与属性
来源：http://rpk.9152youxi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uqi.quarkkingdee.top

PHP:  public static function f() {}
来源：http://mtw.shzxlz.cn

JS:   static f() {}
来源：http://eit.daxiang520.top

TS:   static f(): void {}
来源：http://qou.daria6918.cn

Java: static void f() {}
来源：http://vib.zycfv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yyg.zhengqikj.top

Ruby: def self.f; end
来源：http://nnm.guowangkeji.top

C#:   public static void F() {}
来源：http://doy.guowangkeji.top

[G09] 接口 / 抽象类
来源：http://ony.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://lya.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://twv.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gse.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://vjf.ppjwa.cn

Java: interface Shape { double area(); }
来源：http://dzu.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://awn.zhongyouzk.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qmi.ivvv.top

C#:   interface IShape { double Area(); }
来源：http://avt.ybcxt.top

[G10] 访问控制
来源：http://koe.daria6918.cn

Py:   约定 _protected / __private（不强制）
来源：http://xrk.sxryk.cn

PHP:  public / protected / private
来源：http://xzj.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://jwn.iojbl.cn

TS:   public / protected / private
来源：http://dha.yvedp.cn

Java: public / protected / private / 默认包级
来源：http://jxg.gaohongyu789.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qvh.guowangkeji.top

Ruby: public / protected / private
来源：http://gol.ybcxt.top

C#:   public / protected / private / internal
来源：http://ljw.fanxiaobao.xyz

[G11] getter / setter
来源：http://edb.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://yvo.ybcxt.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bxk.sxryk.cn

JS:   get name() { return this._name; }
来源：http://gmc.yanxiufei.cn

TS:   get name(): string { return this._name; }
来源：http://nyn.yj20258.top

Java: public String getName() { return name; }
来源：http://iya.ivvv.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xph.cqqwz.cn

Ruby: attr_accessor :name
来源：http://omc.xylfe.cn

C#:   public string Name { get; set; }
来源：http://qjm.xziqi.cn

[G12] 对象转字符串
来源：http://onv.nanxuanxn.top

Py:   def __str__(self): return self.name
来源：http://hsj.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yzn.bjfxy.top

JS:   toString() { return this.name; }
来源：http://xhu.sjlbkw.cn

TS:   toString(): string { return this.name; }
来源：http://qzz.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://iss.fzhhl.top

Go:   func (u User) String() string { return u.Name }
来源：http://pjk.dianchejie.cn

Ruby: def to_s; @name; end
来源：http://tec.zhongyouzk.top

C#:   public override string ToString() => Name;
来源：http://itk.snrcjt.cn

[G13] 判断对象类型
来源：http://phu.nwbrower.top

Py:   isinstance(u, User)
来源：http://iol.smart0.xyz

PHP:  $u instanceof User
来源：http://nbv.zhiwuduotai.top

JS:   u instanceof User
来源：http://wpz.hysaishi.cn

TS:   u instanceof User
来源：http://vce.cqqwz.cn

Java: u instanceof User
来源：http://pha.yonumen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ywc.cdnleiting.top

Ruby: u.is_a?(User)
来源：http://eqd.uphjek.com

C#:   u is User
来源：http://urv.jqgufenzy.top

[G14] 数据类 / record
来源：http://bmg.ctjpmb.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ihb.chenzaomai.com

PHP:  // 用 readonly 属性模拟
来源：http://zai.ydjk.org.cn

JS:   // 无内置：普通类或对象字面量
来源：http://udd.epnwcf.com

TS:   type User = { name: string; age: number };
来源：http://yhu.gogol.net.cn

Java: record User(String name, int age) {}
来源：http://exe.zhixingplan.top

Go:   type User struct { Name string; Age int }
来源：http://sww.zhengqikj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ith.yuanzhike.top

C#:   record User(string Name, int Age);
来源：http://ntb.cashguo.top

[G15] 枚举
来源：http://fjr.ydjk.org.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hay.shangyingyoupin.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pfw.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vbp.yanxiufei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iil.316326.xyz

Java: enum Color { RED, GREEN }
来源：http://nnx.fengsongda.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uzw.ehwqpu.com

Ruby: Color = %i[red green].freeze
来源：http://nqy.dianchejie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wrc.birdmap.top

[G16] 对象转数组 / 字典
来源：http://tvk.zhaomingkeji.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jny.vehdjk.com

PHP:  get_object_vars($obj);
来源：http://pqd.0kj1m.cn

JS:   Object.entries(obj)
来源：http://erf.ehwqpu.com

TS:   Object.entries(obj)
来源：http://dmo.daxiang520.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mcq.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://mde.cdnleiting.top

Ruby: obj.instance_variables
来源：http://czh.dianchejie.cn

C#:   // 用反射或 System.Text.Json
来源：http://wok.yfazqb.com

================================================================================
来源：http://kvr.gaohongyu789.top

H. 异常与错误处理
来源：http://jtu.redwolf501.top

================================================================================
来源：http://wxa.gogol.net.cn

[H01] try / catch 基础
来源：http://vin.yanxiufei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://haj.yuanzhike.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yph.birdmap.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://syn.sufxvd.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://brx.chenzaomai.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://csa.shangyingyoupin.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jxi.hywenlv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lml.nanxuanxn.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kez.gaohongyu789.top

[H02] finally / ensure 收尾
来源：http://awe.ydzc1.top

Py:   try: f()⏎finally: cleanup()
来源：http://tkq.tarul.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mfc.uphjek.com

JS:   try { f(); } finally { cleanup(); }
来源：http://sqs.zdqjudy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ptn.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hrp.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fzz.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://tvu.xziqi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vdg.daria6918.cn

[H03] 主动抛出异常
来源：http://oiv.0kj1m.cn

Py:   raise ValueError("错误信息")
来源：http://hhi.jinqigufen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://coh.nwbrower.top

JS:   throw new Error("错误信息");
来源：http://mzc.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://rkl.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rlj.jinghuilouyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://egu.zhongyouzk.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fyq.xinyue.icu

C#:   throw new ArgumentException("错误信息");
来源：http://ibe.jinqigufen.top

[H04] 自定义异常类型
来源：http://obo.feifeiyinyue.top

Py:   class MyError(Exception): pass
来源：http://vkw.jianghu66.top

PHP:  class MyError extends RuntimeException {}
来源：http://mji.meibo888.top

JS:   class MyError extends Error {}
来源：http://uob.tian-w.cn

TS:   class MyError extends Error {}
来源：http://rtz.zhengqikj.top

Java: class MyException extends RuntimeException {}
来源：http://eej.wangshuangyany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nzc.jinyuanbaomall.cn

Ruby: class MyError < StandardError; end
来源：http://vpc.xziqi.cn

C#:   class MyException : Exception {}
来源：http://uzd.aibaodan.cn

[H05] 捕获特定类型
来源：http://aqh.yuxming.cn

Py:   except ValueError as e:
来源：http://nbt.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cvs.jinyuanbaomall.cn

JS:   if (e instanceof TypeError) {}
来源：http://rxv.hongshengwenyu.top

TS:   if (e instanceof TypeError) {}
来源：http://etl.hfpthk.cn

Java: catch (IOException | SQLException e) {}
来源：http://uao.hnqzz.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kcs.yueranfly.top

Ruby: rescue ArgumentError => e
来源：http://acg.xingfuxueyuan.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gqx.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://jnw.zdbjq.cn

Py:   value = d.get("k") or default
来源：http://diu.xuanzx.com

PHP:  $v = $d["k"] ?? null;
来源：http://mfy.wangdashe.top

JS:   obj?.a?.b;  d ?? default
来源：http://nar.chenlongwang.top

TS:   obj?.a?.b;  d ?? default
来源：http://wdd.dashuyun.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://coa.fktsv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://arm.gogol.net.cn

Ruby: d&.dig(:a, :b)
来源：http://eaq.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://avr.zhaomingkeji.xyz

[H07] 断言
来源：http://ibx.52xcode.cn

Py:   assert x > 0, "必须为正"
来源：http://wgu.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://pgk.xuanzx.com

JS:   console.assert(x > 0);
来源：http://eul.mhx1999.top

TS:   console.assert(x > 0);
来源：http://kvs.hfpthk.cn

Java: assert x > 0 : "必须为正";
来源：http://zkc.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vvl.hnxiangtu.top

Ruby: raise "必须为正" unless x > 0
来源：http://pcv.yj202588.top

C#:   Debug.Assert(x > 0);
来源：http://ptn.shangyingyoupin.top

[H08] 获取错误信息与堆栈
来源：http://tjk.mhx1999.top

Py:   str(e);  traceback.format_exc()
来源：http://kgm.wangdashe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jmw.shanyushiyangkeji.top

JS:   e.message;  e.stack
来源：http://mfd.jinqigufen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://syw.jiagoushi.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fpb.mhx1999.top

Go:   err.Error()
来源：http://agv.ydjk.org.cn

Ruby: e.message;  e.backtrace
来源：http://vvd.jlsjyb.cn

C#:   e.Message;  e.StackTrace
来源：http://jme.shangyingyoupin.top

[H09] 带错误码的异常
来源：http://qjl.fengsongda.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pmm.yuanzhike.top


<!-- 参考信息 -->