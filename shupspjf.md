代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eth.vehdjk.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jbz.nanxuanxn.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qgi.ywan-chungtsiang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qdi.nanxinkj.top

[F05] 判断文件或目录是否存在
来源：http://kxh.snrcjt.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hyb.xylfe.cn

PHP:  file_exists("a.txt");
来源：http://yru.jinyuanbaomall.cn

JS:   fs.existsSync("a.txt")
来源：http://wgx.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://hjr.hnqzz.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ads.nanxinkj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://myf.pycfn.com

Ruby: File.exist?("a.txt")
来源：http://yif.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://lxl.ydjk.org.cn

[F06] 删除文件
来源：http://hmr.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://yqs.yvedp.cn

PHP:  unlink("a.txt");
来源：http://oim.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cmf.yongpay.top

TS:   fs.unlinkSync("a.txt")
来源：http://dog.gzhubu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://djh.vqdsnc.cn

Go:   os.Remove("a.txt")
来源：http://buh.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://rqs.zhengqikj.top

C#:   File.Delete("a.txt");
来源：http://tdk.52xcode.cn

[F07] 创建目录（含多级）
来源：http://him.zhongyouzk.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://flc.svipenyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fod.cashguo.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ssr.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gzd.bjfxy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rxh.fktsv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bop.iojbl.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zzr.chenzaomai.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zcj.fzhhl.top

[F08] 遍历目录
来源：http://lbc.shangyingyoupin.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jbk.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ufp.kuanghao11.cn

JS:   fs.readdirSync("dir")
来源：http://nzy.shuidangran.top

TS:   fs.readdirSync("dir")
来源：http://rhh.vqdsnc.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cvp.ppjwa.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ajp.yj20258.top

Ruby: Dir.children("dir")
来源：http://ijr.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://mpk.sjlbkw.cn

[F09] 获取文件大小
来源：http://kkj.ivvv.top

Py:   os.path.getsize("a.txt")
来源：http://tfb.smart0.xyz

PHP:  filesize("a.txt");
来源：http://eig.yuxming.cn

JS:   fs.statSync("a.txt").size
来源：http://yeh.snrcjt.cn

TS:   fs.statSync("a.txt").size
来源：http://rni.ybcxt.top

Java: Files.size(Path.of("a.txt"))
来源：http://awy.chenlongwang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tek.cheryme.top

Ruby: File.size("a.txt")
来源：http://kin.zhijiandao.cn

C#:   new FileInfo("a.txt").Length
来源：http://stt.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://lqe.tianlin.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pux.jqgufenzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gek.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dei.jqgfzy.top

TS:   path.extname("a.txt")
来源：http://gtp.mhx1999.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wuv.sxryk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bfd.gotoacloud.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qlx.yj20258.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fvp.fengsongda.top

[F11] 复制与移动文件
来源：http://yzk.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nnm.mhx1999.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fqs.xinyue.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mae.guowangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mjd.fehbvm.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qzi.jyoumei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wvn.mhx1999.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ggy.cashguo.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ish.ivvv.top

[F12] CSV 读写
来源：http://ybc.shanyushiyangtech.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gmp.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nqu.tarul.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cmk.ppjwa.cn

TS:   // 同上
来源：http://llx.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lec.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://het.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ewk.hfpthk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vot.gzhubu.top

================================================================================
来源：http://xpn.chenzaomai.com

G. 面向对象
来源：http://vtw.gzhubu.top

================================================================================
来源：http://evm.jinqigfzy.top

[G01] 定义类
来源：http://nrh.quarkkingdee.top

Py:   class User: pass
来源：http://mcn.daxiang520.top

PHP:  class User {}
来源：http://jea.gotoacloud.top

JS:   class User {}
来源：http://dvw.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://uiy.hesvh.cn

Java: class User {}
来源：http://arx.dianchejie.cn

Go:   type User struct { Name string }
来源：http://tgi.pycfn.com

Ruby: class User; end
来源：http://ccp.bbcook.cn

C#:   class User {}
来源：http://uwi.xinyue.icu

[G02] 构造函数
来源：http://ntv.sjlbkw.cn

Py:   def __init__(self, name): self.name = name
来源：http://oiy.fehbvm.com

PHP:  public function __construct(public string $name) {}
来源：http://rhs.zhixingplan.top

JS:   constructor(name) { this.name = name; }
来源：http://heb.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://cgw.xinyue.icu

Java: User(String name) { this.name = name; }
来源：http://jrb.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://euq.zhoulong.xyz

Ruby: def initialize(name); @name = name; end
来源：http://hws.gogol.net.cn

C#:   public User(string name) { Name = name; }
来源：http://lvi.yj20258.top

[G03] 实例属性
来源：http://ies.xinyue.icu

Py:   self.name = "x"
来源：http://hcx.cucudq.cn

PHP:  public string $name = "x";
来源：http://lib.cheryme.top

JS:   this.name = "x";
来源：http://kvl.nanxinkj.top

TS:   name: string = "x";
来源：http://rqu.fktsv.cn

Java: private String name;
来源：http://gzp.hfpthk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eas.aizwys.cn

Ruby: @name = "x"
来源：http://vax.mhx1999.top

C#:   public string Name { get; set; } = "x";
来源：http://ccc.shanyushiyangtech.top

[G04] 定义方法
来源：http://cbp.52xcode.cn

Py:   def greet(self): return self.name
来源：http://pee.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://puk.chenjidiqi.icu

JS:   greet() { return this.name; }
来源：http://zcq.fktsv.cn

TS:   greet(): string { return this.name; }
来源：http://voa.yfazqb.com

Java: String greet() { return name; }
来源：http://zdy.vqdsnc.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://iom.yj20258888.top

Ruby: def greet; @name; end
来源：http://frm.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://ozp.xuanzx.com

[G05] 继承
来源：http://bht.shanyushiyangtech.top

Py:   class Admin(User): pass
来源：http://amm.zycfv.cn

PHP:  class Admin extends User {}
来源：http://bda.meibo888.top

JS:   class Admin extends User {}
来源：http://eaq.yj20258.top

TS:   class Admin extends User {}
来源：http://hek.cucudq.cn

Java: class Admin extends User {}
来源：http://eop.nanxuanxn.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://epk.wangdashe.top

Ruby: class Admin < User; end
来源：http://tog.mhx1999.top

C#:   class Admin : User {}
来源：http://ysc.yanxiufei.cn

[G06] 重写方法
来源：http://khz.birdmap.top

Py:   def greet(self): return "admin"
来源：http://fll.nanxinkj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jwa.daxiang520.top

JS:   greet() { return "admin"; }
来源：http://wte.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://dqp.xziqi.cn

Java: @Override String greet() { return "admin"; }
来源：http://eer.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vcz.hysaishi.cn

Ruby: def greet; "admin"; end
来源：http://xyj.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://rax.cheryme.top

[G07] 调用父类方法
来源：http://nam.hywenlv.cn

Py:   super().greet()
来源：http://pgd.yj20258.top

PHP:  parent::greet();
来源：http://asj.vehdjk.com

JS:   super.greet();
来源：http://kiz.tian-w.cn

TS:   super.greet();
来源：http://kyy.yangfankeji.com

Java: super.greet();
来源：http://yfu.hammf.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://saw.cheryme.top

Ruby: super
来源：http://sod.hongshengwenyu.top

C#:   base.Greet();
来源：http://aqj.zhongyouzk.top

[G08] 静态方法与属性
来源：http://nyp.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xjp.sxryk.cn

PHP:  public static function f() {}
来源：http://sqg.cucudq.cn

JS:   static f() {}
来源：http://cfv.ctjpmb.com

TS:   static f(): void {}
来源：http://ong.guannengcc.top

Java: static void f() {}
来源：http://cjp.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://opv.cucudq.cn

Ruby: def self.f; end
来源：http://azm.zhixingplan.top

C#:   public static void F() {}
来源：http://qlz.daxiang520.top

[G09] 接口 / 抽象类
来源：http://ztc.xuanzx.com

Py:   from abc import ABC, abstractmethod
来源：http://gsi.pengpengdd.cyou

PHP:  interface Shape { public function area(): float; }
来源：http://kln.jqgufenzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ofq.zdbjq.cn

TS:   interface Shape { area(): number; }
来源：http://cmw.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://cja.9152youxi.cn

Go:   type Shape interface { Area() float64 }
来源：http://mvl.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xyu.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://fgr.yj20258.top

[G10] 访问控制
来源：http://gph.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://vhz.shangyingyoupin.top

PHP:  public / protected / private
来源：http://eoe.vehdjk.com

JS:   #private 字段；其余公开
来源：http://vzn.yj202588.top

TS:   public / protected / private
来源：http://exj.vqdsnc.cn

Java: public / protected / private / 默认包级
来源：http://hra.hysaishi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://isi.cashguo.top

Ruby: public / protected / private
来源：http://tqm.shzxlz.cn

C#:   public / protected / private / internal
来源：http://kvq.mhx1999.top

[G11] getter / setter
来源：http://xgl.jiagoushi.top

Py:   @property 与 @x.setter
来源：http://ihp.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://imx.ybcxt.top

JS:   get name() { return this._name; }
来源：http://wqe.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://jel.smart0.xyz

Java: public String getName() { return name; }
来源：http://nvd.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kcv.sweek.top

Ruby: attr_accessor :name
来源：http://ddt.ydjk.org.cn

C#:   public string Name { get; set; }
来源：http://kfy.ivvv.top

[G12] 对象转字符串
来源：http://wts.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://kqj.ppjwa.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bru.shzxlz.cn

JS:   toString() { return this.name; }
来源：http://cpz.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://rdf.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://aud.xuanzx.com

Go:   func (u User) String() string { return u.Name }
来源：http://gyi.sweek.top

Ruby: def to_s; @name; end
来源：http://icf.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://yda.9152youxi.cn

[G13] 判断对象类型
来源：http://esz.haohaochexian.top

Py:   isinstance(u, User)
来源：http://ojt.nwbrower.top

PHP:  $u instanceof User
来源：http://ccr.pengpengdd.cyou

JS:   u instanceof User
来源：http://mat.gaohongyu789.top

TS:   u instanceof User
来源：http://cmg.zhoulong.xyz

Java: u instanceof User
来源：http://xqw.zhiwuduotai.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://cej.cqqwz.cn

Ruby: u.is_a?(User)
来源：http://usi.aizwys.cn

C#:   u is User
来源：http://sqt.ybcxt.top

[G14] 数据类 / record
来源：http://mbr.cheryme.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://glb.tian-w.cn

PHP:  // 用 readonly 属性模拟
来源：http://smf.hysaishi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zow.hammf.cn

TS:   type User = { name: string; age: number };
来源：http://chi.snrcjt.cn

Java: record User(String name, int age) {}
来源：http://rnv.epnwcf.com

Go:   type User struct { Name string; Age int }
来源：http://hml.ehwqpu.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ypb.guowangkeji.top

C#:   record User(string Name, int Age);
来源：http://mrp.pycfn.com

[G15] 枚举
来源：http://ofp.ehwqpu.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wyd.jinqigfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yic.tarul.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vyf.zhiwuduotai.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dsq.cdnleiting.top

Java: enum Color { RED, GREEN }
来源：http://gqi.hywenlv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rnw.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://pjr.yanxiufei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tfg.yfazqb.com

[G16] 对象转数组 / 字典
来源：http://wbi.zdqjudy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wlc.ybcxt.top

PHP:  get_object_vars($obj);
来源：http://ngl.hcnkem.com

JS:   Object.entries(obj)
来源：http://iad.wangdashe.top

TS:   Object.entries(obj)
来源：http://tpr.zhongyouzk.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bks.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wwg.c1oappe.top

Ruby: obj.instance_variables
来源：http://tpo.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://bjy.sufxvd.cn

================================================================================
来源：http://dmk.yanxiufei.cn

H. 异常与错误处理
来源：http://wlc.vehdjk.com

================================================================================
来源：http://qod.yvedp.cn

[H01] try / catch 基础
来源：http://xfc.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bls.xziqi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nas.tian-w.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wum.meibo888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aaj.ppjwa.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xpr.cdnleiting.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mdt.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yht.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wbn.jqgfzy.top

[H02] finally / ensure 收尾
来源：http://dgf.yongpay.top

Py:   try: f()⏎finally: cleanup()
来源：http://yvl.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xhv.ybcxt.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cmg.chenlongwang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gfo.jiagoushi.top

Java: try { f(); } finally { cleanup(); }
来源：http://lvh.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://pjp.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://fao.shangyingyoupin.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://tlt.shanyushiyangkeji.top

[H03] 主动抛出异常
来源：http://qeu.feifeiyinyue.top

Py:   raise ValueError("错误信息")
来源：http://aks.hfpthk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hfp.yueranfly.top

JS:   throw new Error("错误信息");
来源：http://lbx.jinyuanbaomall.cn

TS:   throw new Error("错误信息");
来源：http://cno.haohaochexian.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ola.yfazqb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tdy.xuanzx.com

Ruby: raise ArgumentError, "错误信息"
来源：http://ztc.xingfuxueyuan.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://sfj.cashguo.top

[H04] 自定义异常类型
来源：http://vet.zhaomingkeji.xyz

Py:   class MyError(Exception): pass
来源：http://hag.shuidangran.top

PHP:  class MyError extends RuntimeException {}
来源：http://wea.tian-w.cn

JS:   class MyError extends Error {}
来源：http://eef.pycfn.com

TS:   class MyError extends Error {}
来源：http://nmo.fktsv.cn

Java: class MyException extends RuntimeException {}
来源：http://hsl.epnwcf.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ent.jyoumei.cn

Ruby: class MyError < StandardError; end
来源：http://dbt.chenzaomai.com

C#:   class MyException : Exception {}
来源：http://ops.zhiwuduotai.top

[H05] 捕获特定类型
来源：http://uhu.shzxlz.cn

Py:   except ValueError as e:
来源：http://tdl.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kdr.cheryme.top

JS:   if (e instanceof TypeError) {}
来源：http://qqe.ybcxt.top

TS:   if (e instanceof TypeError) {}
来源：http://xzd.nanxuanxn.top

Java: catch (IOException | SQLException e) {}
来源：http://xsc.hesvh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cnz.zdbjq.cn

Ruby: rescue ArgumentError => e
来源：http://jfe.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hjb.chenlongwang.top

[H06] 可选值 / 空值安全访问
来源：http://zwa.fzhhl.top

Py:   value = d.get("k") or default
来源：http://jzq.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://hvt.ehwqpu.com

JS:   obj?.a?.b;  d ?? default
来源：http://kbf.ybcxt.top

TS:   obj?.a?.b;  d ?? default
来源：http://rio.chenjidiqi.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fhi.hnqzz.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xlm.snrcjt.cn

Ruby: d&.dig(:a, :b)
来源：http://axq.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://sbl.dashuyun.cn

[H07] 断言
来源：http://frb.guowangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://jui.chenlongwang.top

PHP:  assert($x > 0);
来源：http://sqr.shanyushiyangkeji.top

JS:   console.assert(x > 0);
来源：http://dpz.hfpthk.cn

TS:   console.assert(x > 0);
来源：http://zsp.jianghu66.top

Java: assert x > 0 : "必须为正";
来源：http://tde.svipenyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://btq.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wko.birdmap.top

C#:   Debug.Assert(x > 0);
来源：http://utr.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://cma.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://cky.jinghuilouyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bqs.yangfankeji.com

JS:   e.message;  e.stack
来源：http://uhk.gzhubu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ydb.zhoulong.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://cet.gaohongyu789.top

Go:   err.Error()
来源：http://bwj.zhaomingkeji.xyz

Ruby: e.message;  e.backtrace
来源：http://opv.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://xwp.vehdjk.com

[H09] 带错误码的异常
来源：http://vbl.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ylf.cdnleiting.top


<!-- 参考信息 -->