代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ojx.epnwcf.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mgm.yvedp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uns.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sdp.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nvh.redwolf501.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dfi.hammf.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fjg.sysykeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kyf.xuetiantiany.cn

[F05] 判断文件或目录是否存在
来源：http://qtm.wangdashe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qvp.yangfankeji.com

PHP:  file_exists("a.txt");
来源：http://xmx.tanke756.top

JS:   fs.existsSync("a.txt")
来源：http://czx.fktsv.cn

TS:   fs.existsSync("a.txt")
来源：http://lre.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://txt.0kj1m.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ujs.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://lzj.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://pju.xingfuxueyuan.xyz

[F06] 删除文件
来源：http://qko.smart0.xyz

Py:   os.remove("a.txt")
来源：http://isd.sjlbkw.cn

PHP:  unlink("a.txt");
来源：http://vfx.ybcxt.top

JS:   fs.unlinkSync("a.txt")
来源：http://eoh.tianlin.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://aqb.chenjidiqi.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fst.sjlbkw.cn

Go:   os.Remove("a.txt")
来源：http://cdk.daxiang520.top

Ruby: File.delete("a.txt")
来源：http://cin.yangfankeji.com

C#:   File.Delete("a.txt");
来源：http://nvc.yuxming.cn

[F07] 创建目录（含多级）
来源：http://cyk.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uuo.yj202588.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ogs.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ymp.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jth.bbcook.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tqr.feifeiyinyue.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pwl.gaohongyu789.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fum.gaohongyu789.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hmn.chenzaomai.com

[F08] 遍历目录
来源：http://okh.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jij.hcnkem.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cgk.snrcjt.cn

JS:   fs.readdirSync("dir")
来源：http://kqd.0kj1m.cn

TS:   fs.readdirSync("dir")
来源：http://wat.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gxp.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fhp.jinqigufen.top

Ruby: Dir.children("dir")
来源：http://jpr.xuetiantiany.cn

C#:   Directory.GetFiles("dir")
来源：http://rst.9152youxi.cn

[F09] 获取文件大小
来源：http://kco.hammf.cn

Py:   os.path.getsize("a.txt")
来源：http://umn.gogol.net.cn

PHP:  filesize("a.txt");
来源：http://yqw.dashuyun.cn

JS:   fs.statSync("a.txt").size
来源：http://nxa.tanke756.top

TS:   fs.statSync("a.txt").size
来源：http://uyt.316326.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://hps.nanxuanxn.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zgn.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://ini.jinqigufen.top

C#:   new FileInfo("a.txt").Length
来源：http://clq.hywenlv.cn

[F10] 取文件扩展名 / 文件名
来源：http://pnb.gogol.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nij.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lwx.nanxuanxn.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wbf.havefunace.top

TS:   path.extname("a.txt")
来源：http://ayc.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://umt.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yib.fengsongda.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://llh.hesvh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uff.svipenyu.cn

[F11] 复制与移动文件
来源：http://ulx.tarul.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ior.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fev.yuanzhike.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xkt.tarul.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iyl.yangfankeji.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fjc.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rps.shanyushiyangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://plc.tian-w.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tbm.nanxinkj.top

[F12] CSV 读写
来源：http://zer.fengsongda.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cpa.uphjek.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lse.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://evk.yonumen.top

TS:   // 同上
来源：http://olq.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ohz.ywan-chungtsiang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oyd.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://otg.sweek.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jht.aizwys.cn

================================================================================
来源：http://xhv.yvedp.cn

G. 面向对象
来源：http://acv.mhx1999.top

================================================================================
来源：http://lqw.xuanzx.com

[G01] 定义类
来源：http://qkc.gzhubu.top

Py:   class User: pass
来源：http://wqa.zdqjudy.top

PHP:  class User {}
来源：http://mey.yfazqb.com

JS:   class User {}
来源：http://emp.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://ujd.tarul.cn

Java: class User {}
来源：http://zym.hongshengwenyu.top

Go:   type User struct { Name string }
来源：http://owd.yonumen.top

Ruby: class User; end
来源：http://nno.yongpay.top

C#:   class User {}
来源：http://udo.zhixingplan.top

[G02] 构造函数
来源：http://uof.yonumen.top

Py:   def __init__(self, name): self.name = name
来源：http://sxk.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://shb.yongpay.top

JS:   constructor(name) { this.name = name; }
来源：http://uoj.cucudq.cn

TS:   constructor(public name: string) {}
来源：http://evc.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://clh.ydzc1.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ris.wangdashe.top

Ruby: def initialize(name); @name = name; end
来源：http://fdy.c1oappe.top

C#:   public User(string name) { Name = name; }
来源：http://kzv.hnqzz.top

[G03] 实例属性
来源：http://msi.vehdjk.com

Py:   self.name = "x"
来源：http://oey.hywenlv.cn

PHP:  public string $name = "x";
来源：http://bmh.chenlongwang.top

JS:   this.name = "x";
来源：http://bte.yanxiufei.cn

TS:   name: string = "x";
来源：http://yvf.fktsv.cn

Java: private String name;
来源：http://vci.svipenyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xgg.yueranfly.top

Ruby: @name = "x"
来源：http://cfz.fehbvm.com

C#:   public string Name { get; set; } = "x";
来源：http://rlq.gotoacloud.top

[G04] 定义方法
来源：http://yra.cqqwz.cn

Py:   def greet(self): return self.name
来源：http://ssz.yueranfly.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rkh.yuanzhike.top

JS:   greet() { return this.name; }
来源：http://hkl.shuidangran.top

TS:   greet(): string { return this.name; }
来源：http://lbu.haohaochexian.top

Java: String greet() { return name; }
来源：http://smh.fktsv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pvj.tanke756.top

Ruby: def greet; @name; end
来源：http://hwl.sjlbkw.cn

C#:   public string Greet() => Name;
来源：http://per.jianghu66.top

[G05] 继承
来源：http://evx.fengsongda.top

Py:   class Admin(User): pass
来源：http://zug.bbcook.cn

PHP:  class Admin extends User {}
来源：http://byv.hysaishi.cn

JS:   class Admin extends User {}
来源：http://sut.hfpthk.cn

TS:   class Admin extends User {}
来源：http://xdk.cucudq.cn

Java: class Admin extends User {}
来源：http://toa.daxiang520.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fmr.chenzaomai.com

Ruby: class Admin < User; end
来源：http://zcd.zhengqikj.top

C#:   class Admin : User {}
来源：http://ceq.epnwcf.com

[G06] 重写方法
来源：http://vbn.jlsjyb.cn

Py:   def greet(self): return "admin"
来源：http://aqx.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://umo.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://ztt.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://crk.c1oappe.top

Java: @Override String greet() { return "admin"; }
来源：http://pom.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://noi.gogol.net.cn

Ruby: def greet; "admin"; end
来源：http://otl.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://ywx.ivvv.top

[G07] 调用父类方法
来源：http://ezc.gaohongyu789.top

Py:   super().greet()
来源：http://uyy.zdbjq.cn

PHP:  parent::greet();
来源：http://mln.yuxming.cn

JS:   super.greet();
来源：http://lyb.hysaishi.cn

TS:   super.greet();
来源：http://dbp.kuanghao11.cn

Java: super.greet();
来源：http://rdy.sjlbkw.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eni.yj20258888.top

Ruby: super
来源：http://aik.redwolf501.top

C#:   base.Greet();
来源：http://inp.fengsongda.top

[G08] 静态方法与属性
来源：http://qew.andypj.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dpd.yongpay.top

PHP:  public static function f() {}
来源：http://liw.yueranfly.top

JS:   static f() {}
来源：http://oqa.vqdsnc.cn

TS:   static f(): void {}
来源：http://xnz.shanyushiyangtech.top

Java: static void f() {}
来源：http://zfa.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ocv.snrcjt.cn

Ruby: def self.f; end
来源：http://rel.zhixingplan.top

C#:   public static void F() {}
来源：http://cec.aibaodan.cn

[G09] 接口 / 抽象类
来源：http://ugc.dianchejie.cn

Py:   from abc import ABC, abstractmethod
来源：http://evn.ywan-chungtsiang.top

PHP:  interface Shape { public function area(): float; }
来源：http://lat.cucudq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dty.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://seh.snrcjt.cn

Java: interface Shape { double area(); }
来源：http://ord.yueranfly.top

Go:   type Shape interface { Area() float64 }
来源：http://vmi.ydjk.org.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bqe.ppjwa.cn

C#:   interface IShape { double Area(); }
来源：http://hsr.jinqigfzy.top

[G10] 访问控制
来源：http://rhl.shangyingyoupin.top

Py:   约定 _protected / __private（不强制）
来源：http://ztx.jyoumei.cn

PHP:  public / protected / private
来源：http://exk.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://xgx.sweek.top

TS:   public / protected / private
来源：http://ybh.sjlbkw.cn

Java: public / protected / private / 默认包级
来源：http://wlr.hammf.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tuf.zhengqikj.top

Ruby: public / protected / private
来源：http://ngz.wangshuangyany.cn

C#:   public / protected / private / internal
来源：http://vrm.vehdjk.com

[G11] getter / setter
来源：http://kkw.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://ewq.pengpengdd.cyou

PHP:  public function getName(): string { return $this->name; }
来源：http://xvr.jlsjyb.cn

JS:   get name() { return this._name; }
来源：http://tcr.hywenlv.cn

TS:   get name(): string { return this._name; }
来源：http://eyo.meibo888.top

Java: public String getName() { return name; }
来源：http://sal.ywan-chungtsiang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cjb.guowangkeji.top

Ruby: attr_accessor :name
来源：http://gra.birdmap.top

C#:   public string Name { get; set; }
来源：http://lwi.havefunace.top

[G12] 对象转字符串
来源：http://xri.jiagoushi.top

Py:   def __str__(self): return self.name
来源：http://lfg.hcnkem.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://vfu.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://rcw.fktsv.cn

TS:   toString(): string { return this.name; }
来源：http://zex.cashguo.top

Java: @Override public String toString() { return name; }
来源：http://kks.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://tpk.hesvh.cn

Ruby: def to_s; @name; end
来源：http://hyy.yongpay.top

C#:   public override string ToString() => Name;
来源：http://oix.wangdashe.top

[G13] 判断对象类型
来源：http://zdi.hfpthk.cn

Py:   isinstance(u, User)
来源：http://sqk.feifeiyinyue.top

PHP:  $u instanceof User
来源：http://kun.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://vif.yj20258.top

TS:   u instanceof User
来源：http://uzq.zycfv.cn

Java: u instanceof User
来源：http://omm.iojbl.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lax.jianghu66.top

Ruby: u.is_a?(User)
来源：http://seq.uphjek.com

C#:   u is User
来源：http://ddy.cashguo.top

[G14] 数据类 / record
来源：http://pat.zhoulong.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://edn.tarul.cn

PHP:  // 用 readonly 属性模拟
来源：http://moo.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://pjd.xylfe.cn

TS:   type User = { name: string; age: number };
来源：http://lqf.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://vqs.yangfankeji.com

Go:   type User struct { Name string; Age int }
来源：http://oem.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iap.hywenlv.cn

C#:   record User(string Name, int Age);
来源：http://czu.tarul.cn

[G15] 枚举
来源：http://szd.wangshuangyany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hdu.shuidangran.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://chv.ppjwa.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tnz.sufxvd.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tzv.9152youxi.cn

Java: enum Color { RED, GREEN }
来源：http://yft.cashguo.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qix.daxiang520.top

Ruby: Color = %i[red green].freeze
来源：http://hns.zhiwuduotai.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lpd.0kj1m.cn

[G16] 对象转数组 / 字典
来源：http://tpu.jinqigfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zkp.cucudq.cn

PHP:  get_object_vars($obj);
来源：http://uxw.xingfuxueyuan.xyz

JS:   Object.entries(obj)
来源：http://xiq.hnxiangtu.top

TS:   Object.entries(obj)
来源：http://mmv.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://faq.dashuyun.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tpj.yuxming.cn

Ruby: obj.instance_variables
来源：http://vqe.xziqi.cn

C#:   // 用反射或 System.Text.Json
来源：http://dgi.daria6918.cn

================================================================================
来源：http://kdc.guannengcc.top

H. 异常与错误处理
来源：http://gbs.tanke756.top

================================================================================
来源：http://aec.fktsv.cn

[H01] try / catch 基础
来源：http://fik.snrcjt.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gyw.ehwqpu.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gpo.hnqzz.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rrq.pengpengdd.cyou

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xwg.sysykeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dvq.zhiwuduotai.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ucc.tarul.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nbv.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sid.uphjek.com

[H02] finally / ensure 收尾
来源：http://deq.jyoumei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sgo.chenzaomai.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://nzs.vqdsnc.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ysn.xziqi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nsz.xingfuxueyuan.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://mbt.iojbl.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://olq.pengpengdd.cyou

Ruby: begin; f; ensure; cleanup; end
来源：http://lwo.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://get.yuxming.cn

[H03] 主动抛出异常
来源：http://jen.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://jva.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qhs.c1oappe.top

JS:   throw new Error("错误信息");
来源：http://hyz.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://wjz.cheryme.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pqi.dashuyun.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gbq.zdqjudy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://emb.yonumen.top

C#:   throw new ArgumentException("错误信息");
来源：http://gtg.andypj.xyz

[H04] 自定义异常类型
来源：http://csf.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://ffg.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://ytf.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://rve.vehdjk.com

TS:   class MyError extends Error {}
来源：http://wfn.hongshengwenyu.top

Java: class MyException extends RuntimeException {}
来源：http://aen.cdnleiting.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pgf.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://cqj.gogol.net.cn

C#:   class MyException : Exception {}
来源：http://upk.bbcook.cn

[H05] 捕获特定类型
来源：http://cfd.birdmap.top

Py:   except ValueError as e:
来源：http://ntu.hammf.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gts.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://ifk.uphjek.com

TS:   if (e instanceof TypeError) {}
来源：http://yas.ctjpmb.com

Java: catch (IOException | SQLException e) {}
来源：http://xeh.quarkkingdee.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ljr.yongpay.top

Ruby: rescue ArgumentError => e
来源：http://rpz.cheryme.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rjw.tarul.cn

[H06] 可选值 / 空值安全访问
来源：http://lrw.vqdsnc.cn

Py:   value = d.get("k") or default
来源：http://bal.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jfy.epnwcf.com

JS:   obj?.a?.b;  d ?? default
来源：http://clq.nanxuanxn.top

TS:   obj?.a?.b;  d ?? default
来源：http://roj.c1oappe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hfm.nanxinkj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bdk.jinqigfzy.top

Ruby: d&.dig(:a, :b)
来源：http://bnh.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://lkh.hcnkem.com

[H07] 断言
来源：http://rid.tanke756.top

Py:   assert x > 0, "必须为正"
来源：http://umu.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://aop.gogol.net.cn

JS:   console.assert(x > 0);
来源：http://xui.daria6918.cn

TS:   console.assert(x > 0);
来源：http://efx.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://out.jqgfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mez.daria6918.cn

Ruby: raise "必须为正" unless x > 0
来源：http://woy.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://btm.cucudq.cn

[H08] 获取错误信息与堆栈
来源：http://nyy.ivvv.top

Py:   str(e);  traceback.format_exc()
来源：http://zzo.ctjpmb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ulw.ywan-chungtsiang.top

JS:   e.message;  e.stack
来源：http://dwn.hesvh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wru.jlsjyb.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tpa.ppjwa.cn

Go:   err.Error()
来源：http://daa.ybcxt.top


<!-- 参考信息 -->