代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rng.havefunace.top

Ruby: File.write("a.txt", "hi")
来源：http://vrm.ivvv.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ouk.uphjek.com

[F04] 追加写入文件
来源：http://don.hesvh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ycl.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yxb.andypj.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lgn.yfazqb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xti.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iup.yfazqb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dag.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gpt.yuxming.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lxb.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://tyb.tian-w.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dsf.tarul.cn

PHP:  file_exists("a.txt");
来源：http://aft.redwolf501.top

JS:   fs.existsSync("a.txt")
来源：http://gra.fzhhl.top

TS:   fs.existsSync("a.txt")
来源：http://iuo.fktsv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hoj.jianghu66.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://anu.cashguo.top

Ruby: File.exist?("a.txt")
来源：http://oja.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://kty.xuetiantiany.cn

[F06] 删除文件
来源：http://epc.aizwys.cn

Py:   os.remove("a.txt")
来源：http://dai.tianlin.xyz

PHP:  unlink("a.txt");
来源：http://gbl.yanxiufei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://oxu.dashuyun.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zic.yuxming.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://byg.ydzc1.top

Go:   os.Remove("a.txt")
来源：http://nsh.sufxvd.cn

Ruby: File.delete("a.txt")
来源：http://ufu.ydzc1.top

C#:   File.Delete("a.txt");
来源：http://fgr.xziqi.cn

[F07] 创建目录（含多级）
来源：http://jug.gaohongyu789.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ytn.vqdsnc.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://amh.daria6918.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zya.chenjidiqi.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eqt.zhixingplan.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mwx.fengsongda.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ewf.zhijiandao.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bjg.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://upw.haohaochexian.top

[F08] 遍历目录
来源：http://sar.yj20258888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hnf.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vmz.pengpengdd.cyou

JS:   fs.readdirSync("dir")
来源：http://sjv.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://olv.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hsv.jinghuilouyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jjf.xuanzx.com

Ruby: Dir.children("dir")
来源：http://zad.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://plv.pycfn.com

[F09] 获取文件大小
来源：http://uab.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://ezt.yj202588.top

PHP:  filesize("a.txt");
来源：http://hcz.snrcjt.cn

JS:   fs.statSync("a.txt").size
来源：http://njx.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://agd.hywenlv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://akm.xingfuxueyuan.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lyc.smart0.xyz

Ruby: File.size("a.txt")
来源：http://wuk.meibo888.top

C#:   new FileInfo("a.txt").Length
来源：http://cpo.nwbrower.top

[F10] 取文件扩展名 / 文件名
来源：http://jnn.chenjidiqi.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tvd.zhongyouzk.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yms.pengpengdd.cyou

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yyu.pycfn.com

TS:   path.extname("a.txt")
来源：http://byr.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tjr.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kmt.havefunace.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://isg.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fwd.tianlin.xyz

[F11] 复制与移动文件
来源：http://xww.feifeiyinyue.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wts.cashguo.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kuq.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eis.yj202588.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eya.jqgfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bth.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uim.fktsv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jya.guannengcc.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kpj.snrcjt.cn

[F12] CSV 读写
来源：http://blu.316326.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zpa.jlsjyb.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://geh.zhiwuduotai.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kis.hcnkem.com

TS:   // 同上
来源：http://qqh.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vyy.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fmt.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gpp.ctjpmb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://tqy.shuidangran.top

================================================================================
来源：http://pxa.chenjidiqi.icu

G. 面向对象
来源：http://prv.hesvh.cn

================================================================================
来源：http://mmy.jinqigufen.top

[G01] 定义类
来源：http://eqo.xylfe.cn

Py:   class User: pass
来源：http://wbc.zhengqikj.top

PHP:  class User {}
来源：http://gwk.tanke756.top

JS:   class User {}
来源：http://tvv.fzhhl.top

TS:   class User { name: string = ""; }
来源：http://dte.fzhhl.top

Java: class User {}
来源：http://ahw.wangdashe.top

Go:   type User struct { Name string }
来源：http://bci.havefunace.top

Ruby: class User; end
来源：http://dng.birdmap.top

C#:   class User {}
来源：http://rmq.0kj1m.cn

[G02] 构造函数
来源：http://pby.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://jcl.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://chw.hammf.cn

JS:   constructor(name) { this.name = name; }
来源：http://zsa.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://crw.dianchejie.cn

Java: User(String name) { this.name = name; }
来源：http://iyx.kuanghao11.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kns.shangyingyoupin.top

Ruby: def initialize(name); @name = name; end
来源：http://xcs.nwbrower.top

C#:   public User(string name) { Name = name; }
来源：http://gga.c1oappe.top

[G03] 实例属性
来源：http://qad.epnwcf.com

Py:   self.name = "x"
来源：http://eyu.daria6918.cn

PHP:  public string $name = "x";
来源：http://bcd.yangfankeji.com

JS:   this.name = "x";
来源：http://cnp.fzhhl.top

TS:   name: string = "x";
来源：http://adj.zhongyouzk.top

Java: private String name;
来源：http://hpr.zhiwuduotai.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nhs.sjlbkw.cn

Ruby: @name = "x"
来源：http://raa.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://mrj.cucudq.cn

[G04] 定义方法
来源：http://jod.jinyuanbaomall.cn

Py:   def greet(self): return self.name
来源：http://uer.52xcode.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://twt.nwbrower.top

JS:   greet() { return this.name; }
来源：http://ekr.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://fca.ybcxt.top

Java: String greet() { return name; }
来源：http://xbg.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://vmx.hammf.cn

Ruby: def greet; @name; end
来源：http://dzq.9152youxi.cn

C#:   public string Greet() => Name;
来源：http://mra.bjfxy.top

[G05] 继承
来源：http://tuc.quarkkingdee.top

Py:   class Admin(User): pass
来源：http://bry.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://wgk.gzhubu.top

JS:   class Admin extends User {}
来源：http://hji.0kj1m.cn

TS:   class Admin extends User {}
来源：http://fcd.9152youxi.cn

Java: class Admin extends User {}
来源：http://mfe.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hcm.316326.xyz

Ruby: class Admin < User; end
来源：http://vqe.fehbvm.com

C#:   class Admin : User {}
来源：http://ydz.redwolf501.top

[G06] 重写方法
来源：http://agg.aibaodan.cn

Py:   def greet(self): return "admin"
来源：http://bqy.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://hye.bjfxy.top

JS:   greet() { return "admin"; }
来源：http://qjp.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://vqg.meibo888.top

Java: @Override String greet() { return "admin"; }
来源：http://ysd.sufxvd.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jca.yvedp.cn

Ruby: def greet; "admin"; end
来源：http://lxv.iojbl.cn

C#:   public override string Greet() => "admin";
来源：http://vjp.hnxiangtu.top

[G07] 调用父类方法
来源：http://dji.yj20258.top

Py:   super().greet()
来源：http://ygy.fehbvm.com

PHP:  parent::greet();
来源：http://jwc.cdnleiting.top

JS:   super.greet();
来源：http://dms.nanxinkj.top

TS:   super.greet();
来源：http://zjh.sufxvd.cn

Java: super.greet();
来源：http://abc.shzxlz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uae.yongpay.top

Ruby: super
来源：http://ieg.ctjpmb.com

C#:   base.Greet();
来源：http://idw.zhoulong.xyz

[G08] 静态方法与属性
来源：http://mni.xuetiantiany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xbw.ivvv.top

PHP:  public static function f() {}
来源：http://mai.jinqigfzy.top

JS:   static f() {}
来源：http://ale.jianghu66.top

TS:   static f(): void {}
来源：http://xtq.hnxiangtu.top

Java: static void f() {}
来源：http://aym.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bdw.shangyingyoupin.top

Ruby: def self.f; end
来源：http://fqh.zhijiandao.cn

C#:   public static void F() {}
来源：http://zyx.ctjpmb.com

[G09] 接口 / 抽象类
来源：http://ibh.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://wsb.xuanzx.com

PHP:  interface Shape { public function area(): float; }
来源：http://gll.fanxiaobao.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://ptw.yfazqb.com

TS:   interface Shape { area(): number; }
来源：http://ldg.yuxming.cn

Java: interface Shape { double area(); }
来源：http://nke.pycfn.com

Go:   type Shape interface { Area() float64 }
来源：http://rub.shanyushiyangtech.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uqm.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://uhh.kuanghao11.cn

[G10] 访问控制
来源：http://hhn.yvedp.cn

Py:   约定 _protected / __private（不强制）
来源：http://vrj.316326.xyz

PHP:  public / protected / private
来源：http://qnx.jqgfzy.top

JS:   #private 字段；其余公开
来源：http://myu.snrcjt.cn

TS:   public / protected / private
来源：http://pxc.zhengqikj.top

Java: public / protected / private / 默认包级
来源：http://kfe.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mzk.shzxlz.cn

Ruby: public / protected / private
来源：http://ybx.hnxiangtu.top

C#:   public / protected / private / internal
来源：http://loq.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://phk.fehbvm.com

Py:   @property 与 @x.setter
来源：http://rbk.ehwqpu.com

PHP:  public function getName(): string { return $this->name; }
来源：http://xtx.haohaochexian.top

JS:   get name() { return this._name; }
来源：http://lmw.cucudq.cn

TS:   get name(): string { return this._name; }
来源：http://phl.jianghu66.top

Java: public String getName() { return name; }
来源：http://kgh.hcnkem.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://qrl.daxiang520.top

Ruby: attr_accessor :name
来源：http://kgw.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://rgd.pengpengdd.cyou

[G12] 对象转字符串
来源：http://mko.jianghu66.top

Py:   def __str__(self): return self.name
来源：http://yth.jqgufenzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://htm.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://rnq.sjlbkw.cn

TS:   toString(): string { return this.name; }
来源：http://fgb.yuanzhike.top

Java: @Override public String toString() { return name; }
来源：http://xae.haohaochexian.top

Go:   func (u User) String() string { return u.Name }
来源：http://peb.bjfxy.top

Ruby: def to_s; @name; end
来源：http://grr.gzhubu.top

C#:   public override string ToString() => Name;
来源：http://tsa.ctjpmb.com

[G13] 判断对象类型
来源：http://ple.epnwcf.com

Py:   isinstance(u, User)
来源：http://nnv.fktsv.cn

PHP:  $u instanceof User
来源：http://pnr.epnwcf.com

JS:   u instanceof User
来源：http://rav.hongshengwenyu.top

TS:   u instanceof User
来源：http://xjy.haohaochexian.top

Java: u instanceof User
来源：http://lrj.yj202588.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fne.yuanzhike.top

Ruby: u.is_a?(User)
来源：http://ffq.ydjk.org.cn

C#:   u is User
来源：http://mho.ivvv.top

[G14] 数据类 / record
来源：http://pqd.tarul.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://law.jinqigufen.top

PHP:  // 用 readonly 属性模拟
来源：http://gvf.quarkkingdee.top

JS:   // 无内置：普通类或对象字面量
来源：http://lxq.jinqigfzy.top

TS:   type User = { name: string; age: number };
来源：http://wui.fktsv.cn

Java: record User(String name, int age) {}
来源：http://oie.vehdjk.com

Go:   type User struct { Name string; Age int }
来源：http://hij.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rnz.0kj1m.cn

C#:   record User(string Name, int Age);
来源：http://ilx.xuanzx.com

[G15] 枚举
来源：http://ncu.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rqj.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tiy.0kj1m.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bnv.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rac.dashuyun.cn

Java: enum Color { RED, GREEN }
来源：http://ovd.0kj1m.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cbx.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://wju.bjfxy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tdi.redwolf501.top

[G16] 对象转数组 / 字典
来源：http://vwp.jqgfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wxb.sufxvd.cn

PHP:  get_object_vars($obj);
来源：http://qsc.tarul.cn

JS:   Object.entries(obj)
来源：http://ijm.hongshengwenyu.top

TS:   Object.entries(obj)
来源：http://vsm.9152youxi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://arj.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vom.sjlbkw.cn

Ruby: obj.instance_variables
来源：http://fnw.hysaishi.cn

C#:   // 用反射或 System.Text.Json
来源：http://uht.tanke756.top

================================================================================
来源：http://rki.hammf.cn

H. 异常与错误处理
来源：http://qeg.hammf.cn

================================================================================
来源：http://cxn.gogol.net.cn

[H01] try / catch 基础
来源：http://zsa.epnwcf.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gem.xuetiantiany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wpb.aizwys.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rpa.sufxvd.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gxn.yj20258888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pnz.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xjh.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sex.chenzaomai.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rhw.ivvv.top

[H02] finally / ensure 收尾
来源：http://bux.hammf.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pzt.zhijiandao.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://arl.0kj1m.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qxx.nanxinkj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ykz.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://rjt.shuidangran.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://elm.dianchejie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ute.zhijiandao.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nau.c1oappe.top

[H03] 主动抛出异常
来源：http://exw.sweek.top

Py:   raise ValueError("错误信息")
来源：http://nnm.guowangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rul.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://lwg.fzhhl.top

TS:   throw new Error("错误信息");
来源：http://ozt.sysykeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ztn.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://siq.andypj.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://brv.yueranfly.top

C#:   throw new ArgumentException("错误信息");
来源：http://rih.hnqzz.top

[H04] 自定义异常类型
来源：http://mgk.hesvh.cn

Py:   class MyError(Exception): pass
来源：http://msf.cqqwz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nsg.snrcjt.cn

JS:   class MyError extends Error {}
来源：http://xfk.tarul.cn

TS:   class MyError extends Error {}
来源：http://rpb.xuetiantiany.cn

Java: class MyException extends RuntimeException {}
来源：http://pkb.hammf.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wjh.jyoumei.cn

Ruby: class MyError < StandardError; end
来源：http://ggp.gaohongyu789.top

C#:   class MyException : Exception {}
来源：http://jbu.tanke756.top

[H05] 捕获特定类型
来源：http://qnb.sxryk.cn

Py:   except ValueError as e:
来源：http://fru.smart0.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xcy.aizwys.cn

JS:   if (e instanceof TypeError) {}
来源：http://dqh.yfazqb.com

TS:   if (e instanceof TypeError) {}
来源：http://lot.haohaochexian.top

Java: catch (IOException | SQLException e) {}
来源：http://fna.zhengqikj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kjh.hysaishi.cn

Ruby: rescue ArgumentError => e
来源：http://rkh.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xoy.fktsv.cn

[H06] 可选值 / 空值安全访问
来源：http://aqs.fzhhl.top

Py:   value = d.get("k") or default
来源：http://zxz.tianlin.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://mgy.hesvh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://exn.shanyushiyangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://kbn.vqdsnc.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://brf.c1oappe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hbw.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://fib.epnwcf.com

C#:   obj?.A?.B ?? default
来源：http://ugz.kuanghao11.cn

[H07] 断言
来源：http://daj.yj20258.top

Py:   assert x > 0, "必须为正"
来源：http://okq.daria6918.cn

PHP:  assert($x > 0);
来源：http://hho.52xcode.cn

JS:   console.assert(x > 0);
来源：http://hto.redwolf501.top

TS:   console.assert(x > 0);
来源：http://tvn.chenjidiqi.icu

Java: assert x > 0 : "必须为正";
来源：http://jba.ehwqpu.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mej.gzhubu.top

Ruby: raise "必须为正" unless x > 0
来源：http://bwe.cheryme.top

C#:   Debug.Assert(x > 0);
来源：http://zcf.0kj1m.cn

[H08] 获取错误信息与堆栈
来源：http://bnx.c1oappe.top

Py:   str(e);  traceback.format_exc()
来源：http://eng.zhaomingkeji.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kyk.meibo888.top


<!-- 参考信息 -->