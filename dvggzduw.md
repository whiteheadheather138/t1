代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://gna.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mhl.hnxiangtu.top

PHP:  file_exists("a.txt");
来源：http://nxy.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://koa.sxryk.cn

TS:   fs.existsSync("a.txt")
来源：http://uvq.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ees.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sky.andypj.xyz

Ruby: File.exist?("a.txt")
来源：http://pfv.yuxming.cn

C#:   File.Exists("a.txt")
来源：http://pkr.tianlin.xyz

[F06] 删除文件
来源：http://mcr.vehdjk.com

Py:   os.remove("a.txt")
来源：http://qfm.dianchejie.cn

PHP:  unlink("a.txt");
来源：http://yvt.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://rfv.hfpthk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dif.hesvh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mwz.zhongyouzk.top

Go:   os.Remove("a.txt")
来源：http://onn.zhoulong.xyz

Ruby: File.delete("a.txt")
来源：http://tqm.xziqi.cn

C#:   File.Delete("a.txt");
来源：http://rxk.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://uiy.havefunace.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xac.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xvk.hongshengwenyu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lfh.zhiwuduotai.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sgv.jlsjyb.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vxm.zhixingplan.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://csp.chenzaomai.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://smu.xylfe.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zag.dashuyun.cn

[F08] 遍历目录
来源：http://veq.cashguo.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://oup.pengpengdd.cyou

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lte.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://wxa.sweek.top

TS:   fs.readdirSync("dir")
来源：http://rhd.yuanzhike.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mpt.vehdjk.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://cvk.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://wte.chenjidiqi.icu

C#:   Directory.GetFiles("dir")
来源：http://iij.bjfxy.top

[F09] 获取文件大小
来源：http://ftj.aizwys.cn

Py:   os.path.getsize("a.txt")
来源：http://anw.birdmap.top

PHP:  filesize("a.txt");
来源：http://jvt.zhoulong.xyz

JS:   fs.statSync("a.txt").size
来源：http://wav.yangfankeji.com

TS:   fs.statSync("a.txt").size
来源：http://nxi.ywan-chungtsiang.top

Java: Files.size(Path.of("a.txt"))
来源：http://wrw.c1oappe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jwd.fengsongda.top

Ruby: File.size("a.txt")
来源：http://bco.yueranfly.top

C#:   new FileInfo("a.txt").Length
来源：http://hzf.chenlongwang.top

[F10] 取文件扩展名 / 文件名
来源：http://ztz.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hct.birdmap.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://noy.jyoumei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ktl.wangshuangyany.cn

TS:   path.extname("a.txt")
来源：http://rqe.yongpay.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lsb.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xro.jinqigufen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nyn.bbcook.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://auq.shanyushiyangtech.top

[F11] 复制与移动文件
来源：http://pyn.shzxlz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iir.ydzc1.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xkz.guannengcc.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eji.nwbrower.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://twv.cucudq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jxf.nanxinkj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hka.iojbl.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lul.iojbl.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pmk.shangyingyoupin.top

[F12] CSV 读写
来源：http://sfv.9152youxi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cmj.nanxuanxn.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://asd.shangyingyoupin.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zum.jianghu66.top

TS:   // 同上
来源：http://oom.xingfuxueyuan.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kcq.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oqm.ybcxt.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mfv.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xlx.zdbjq.cn

================================================================================
来源：http://fyb.uphjek.com

G. 面向对象
来源：http://bco.sjlbkw.cn

================================================================================
来源：http://tpk.jqgufenzy.top

[G01] 定义类
来源：http://tkv.mhx1999.top

Py:   class User: pass
来源：http://cxr.jqgufenzy.top

PHP:  class User {}
来源：http://oed.yfazqb.com

JS:   class User {}
来源：http://imu.sxryk.cn

TS:   class User { name: string = ""; }
来源：http://vmp.kuanghao11.cn

Java: class User {}
来源：http://nol.xziqi.cn

Go:   type User struct { Name string }
来源：http://foi.ydzc1.top

Ruby: class User; end
来源：http://jjz.kuanghao11.cn

C#:   class User {}
来源：http://iqq.ivvv.top

[G02] 构造函数
来源：http://fsj.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://iac.wangdashe.top

PHP:  public function __construct(public string $name) {}
来源：http://qdo.jinqigufen.top

JS:   constructor(name) { this.name = name; }
来源：http://vwe.fanxiaobao.xyz

TS:   constructor(public name: string) {}
来源：http://uov.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://ufo.tian-w.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://urh.yvedp.cn

Ruby: def initialize(name); @name = name; end
来源：http://run.mhx1999.top

C#:   public User(string name) { Name = name; }
来源：http://log.cheryme.top

[G03] 实例属性
来源：http://chc.xinyue.icu

Py:   self.name = "x"
来源：http://ync.yj20258.top

PHP:  public string $name = "x";
来源：http://lse.ywan-chungtsiang.top

JS:   this.name = "x";
来源：http://jhd.yj20258888.top

TS:   name: string = "x";
来源：http://fgi.hesvh.cn

Java: private String name;
来源：http://iyz.ydzc1.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qxe.ywan-chungtsiang.top

Ruby: @name = "x"
来源：http://kza.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://mry.hongshengwenyu.top

[G04] 定义方法
来源：http://ixi.sxryk.cn

Py:   def greet(self): return self.name
来源：http://iwd.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yhm.jyoumei.cn

JS:   greet() { return this.name; }
来源：http://ujb.kuanghao11.cn

TS:   greet(): string { return this.name; }
来源：http://ajg.jinqigfzy.top

Java: String greet() { return name; }
来源：http://bud.chenjidiqi.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://rcv.fzhhl.top

Ruby: def greet; @name; end
来源：http://doj.chenzaomai.com

C#:   public string Greet() => Name;
来源：http://xgd.nwbrower.top

[G05] 继承
来源：http://bpj.xuanzx.com

Py:   class Admin(User): pass
来源：http://hsh.bbcook.cn

PHP:  class Admin extends User {}
来源：http://ybo.fanxiaobao.xyz

JS:   class Admin extends User {}
来源：http://erp.aizwys.cn

TS:   class Admin extends User {}
来源：http://nix.aizwys.cn

Java: class Admin extends User {}
来源：http://epd.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yrd.hnxiangtu.top

Ruby: class Admin < User; end
来源：http://hix.chenjidiqi.icu

C#:   class Admin : User {}
来源：http://obh.haohaochexian.top

[G06] 重写方法
来源：http://kwc.hammf.cn

Py:   def greet(self): return "admin"
来源：http://gni.ydzc1.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hsr.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://sbt.vehdjk.com

TS:   greet(): string { return "admin"; }
来源：http://acm.bbcook.cn

Java: @Override String greet() { return "admin"; }
来源：http://mjk.uphjek.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mxg.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://brd.hongshengwenyu.top

C#:   public override string Greet() => "admin";
来源：http://qvn.shanyushiyangkeji.top

[G07] 调用父类方法
来源：http://bao.dianchejie.cn

Py:   super().greet()
来源：http://nhv.meibo888.top

PHP:  parent::greet();
来源：http://lfa.chenlongwang.top

JS:   super.greet();
来源：http://oau.jyoumei.cn

TS:   super.greet();
来源：http://nop.zdqjudy.top

Java: super.greet();
来源：http://osv.ivvv.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jvy.jinqigufen.top

Ruby: super
来源：http://ppm.jinghuilouyu.cn

C#:   base.Greet();
来源：http://qpr.zhengqikj.top

[G08] 静态方法与属性
来源：http://fpc.snrcjt.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fgl.fanxiaobao.xyz

PHP:  public static function f() {}
来源：http://plf.fehbvm.com

JS:   static f() {}
来源：http://iqg.yvedp.cn

TS:   static f(): void {}
来源：http://hys.shangyingyoupin.top

Java: static void f() {}
来源：http://dxa.quarkkingdee.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://uyr.haohaochexian.top

Ruby: def self.f; end
来源：http://uak.hammf.cn

C#:   public static void F() {}
来源：http://yuk.xingfuxueyuan.xyz

[G09] 接口 / 抽象类
来源：http://qzg.aibaodan.cn

Py:   from abc import ABC, abstractmethod
来源：http://cvw.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://ntb.yfazqb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://aau.chenzaomai.com

TS:   interface Shape { area(): number; }
来源：http://rxf.sweek.top

Java: interface Shape { double area(); }
来源：http://yld.yuxming.cn

Go:   type Shape interface { Area() float64 }
来源：http://xth.sysykeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ayk.aibaodan.cn

C#:   interface IShape { double Area(); }
来源：http://kyh.hammf.cn

[G10] 访问控制
来源：http://cov.mhx1999.top

Py:   约定 _protected / __private（不强制）
来源：http://yrx.bbcook.cn

PHP:  public / protected / private
来源：http://lox.daxiang520.top

JS:   #private 字段；其余公开
来源：http://gno.yfazqb.com

TS:   public / protected / private
来源：http://hdn.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://dmn.jinyuanbaomall.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dwl.yuanzhike.top

Ruby: public / protected / private
来源：http://gjo.chenzaomai.com

C#:   public / protected / private / internal
来源：http://wrx.yueranfly.top

[G11] getter / setter
来源：http://szq.9152youxi.cn

Py:   @property 与 @x.setter
来源：http://igo.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ecs.tarul.cn

JS:   get name() { return this._name; }
来源：http://vdr.meibo888.top

TS:   get name(): string { return this._name; }
来源：http://ptg.yongpay.top

Java: public String getName() { return name; }
来源：http://qho.aizwys.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tyb.vqdsnc.cn

Ruby: attr_accessor :name
来源：http://giz.aizwys.cn

C#:   public string Name { get; set; }
来源：http://qke.xuetiantiany.cn

[G12] 对象转字符串
来源：http://hzq.meibo888.top

Py:   def __str__(self): return self.name
来源：http://ddl.svipenyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://oon.guowangkeji.top

JS:   toString() { return this.name; }
来源：http://eiv.dianchejie.cn

TS:   toString(): string { return this.name; }
来源：http://aez.zhoulong.xyz

Java: @Override public String toString() { return name; }
来源：http://lfw.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ccy.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://ked.fktsv.cn

C#:   public override string ToString() => Name;
来源：http://eao.xinyue.icu

[G13] 判断对象类型
来源：http://xjj.bbcook.cn

Py:   isinstance(u, User)
来源：http://tqn.sysykeji.top

PHP:  $u instanceof User
来源：http://mlj.yuxming.cn

JS:   u instanceof User
来源：http://jdc.jinghuilouyu.cn

TS:   u instanceof User
来源：http://ggi.zhoulong.xyz

Java: u instanceof User
来源：http://jyb.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://txr.ctjpmb.com

Ruby: u.is_a?(User)
来源：http://ltc.c1oappe.top

C#:   u is User
来源：http://btl.tian-w.cn

[G14] 数据类 / record
来源：http://zbe.zhiwuduotai.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zdy.andypj.xyz

PHP:  // 用 readonly 属性模拟
来源：http://oyx.ehwqpu.com

JS:   // 无内置：普通类或对象字面量
来源：http://zyg.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://xwy.jqgfzy.top

Java: record User(String name, int age) {}
来源：http://nof.xziqi.cn

Go:   type User struct { Name string; Age int }
来源：http://zdt.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ejl.yuanzhike.top

C#:   record User(string Name, int Age);
来源：http://blj.cheryme.top

[G15] 枚举
来源：http://nji.chenlongwang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ipv.yueranfly.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lfi.vqdsnc.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dtz.sjlbkw.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zld.shangyingyoupin.top

Java: enum Color { RED, GREEN }
来源：http://vyf.shanyushiyangtech.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mkq.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://yhw.gzhubu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ssc.fanxiaobao.xyz

[G16] 对象转数组 / 字典
来源：http://beu.cqqwz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://buc.sweek.top

PHP:  get_object_vars($obj);
来源：http://zso.yangfankeji.com

JS:   Object.entries(obj)
来源：http://eby.hammf.cn

TS:   Object.entries(obj)
来源：http://cqp.zhongyouzk.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fzz.gzhubu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://eas.gogol.net.cn

Ruby: obj.instance_variables
来源：http://eud.ppjwa.cn

C#:   // 用反射或 System.Text.Json
来源：http://zom.tanke756.top

================================================================================
来源：http://tkj.zdbjq.cn

H. 异常与错误处理
来源：http://fxc.fzhhl.top

================================================================================
来源：http://qix.aizwys.cn

[H01] try / catch 基础
来源：http://zvh.cqqwz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tdl.hammf.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tss.haohaochexian.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jwm.cqqwz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iyn.hnxiangtu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dyu.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sdz.meibo888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cqk.jinqigufen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hgd.epnwcf.com

[H02] finally / ensure 收尾
来源：http://hfz.yongpay.top

Py:   try: f()⏎finally: cleanup()
来源：http://dvh.ehwqpu.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://pws.316326.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://rvb.yfazqb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://dcz.jlsjyb.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vat.ivvv.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pza.9152youxi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gti.wangshuangyany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tpw.hfpthk.cn

[H03] 主动抛出异常
来源：http://zeq.yangfankeji.com

Py:   raise ValueError("错误信息")
来源：http://ajq.daxiang520.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ujb.fktsv.cn

JS:   throw new Error("错误信息");
来源：http://wxg.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://lzx.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kfh.wangdashe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ylw.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wnz.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://rlg.quarkkingdee.top

[H04] 自定义异常类型
来源：http://sfc.jiagoushi.top

Py:   class MyError(Exception): pass
来源：http://qvt.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://qsz.haohaochexian.top

JS:   class MyError extends Error {}
来源：http://zzu.haohaochexian.top

TS:   class MyError extends Error {}
来源：http://vti.feifeiyinyue.top

Java: class MyException extends RuntimeException {}
来源：http://ejd.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nxq.ppjwa.cn

Ruby: class MyError < StandardError; end
来源：http://fbu.svipenyu.cn

C#:   class MyException : Exception {}
来源：http://all.chenlongwang.top

[H05] 捕获特定类型
来源：http://xak.quarkkingdee.top

Py:   except ValueError as e:
来源：http://smj.52xcode.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ktb.yj202588.top

JS:   if (e instanceof TypeError) {}
来源：http://zlb.zhengqikj.top

TS:   if (e instanceof TypeError) {}
来源：http://zsj.zhaomingkeji.xyz

Java: catch (IOException | SQLException e) {}
来源：http://efx.xylfe.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xvf.feifeiyinyue.top

Ruby: rescue ArgumentError => e
来源：http://uct.yuanzhike.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://idx.meibo888.top

[H06] 可选值 / 空值安全访问
来源：http://yil.yj202588.top

Py:   value = d.get("k") or default
来源：http://xnx.fehbvm.com

PHP:  $v = $d["k"] ?? null;
来源：http://igp.feifeiyinyue.top

JS:   obj?.a?.b;  d ?? default
来源：http://gkl.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ubi.jinqigufen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mut.xinyue.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://xvr.hywenlv.cn

Ruby: d&.dig(:a, :b)
来源：http://cyw.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://llt.9152youxi.cn

[H07] 断言
来源：http://egk.sxryk.cn

Py:   assert x > 0, "必须为正"
来源：http://usm.yfazqb.com

PHP:  assert($x > 0);
来源：http://age.jqgufenzy.top

JS:   console.assert(x > 0);
来源：http://iph.chenjidiqi.icu

TS:   console.assert(x > 0);
来源：http://zpo.birdmap.top

Java: assert x > 0 : "必须为正";
来源：http://ioo.aizwys.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nag.hnqzz.top

Ruby: raise "必须为正" unless x > 0
来源：http://trt.feifeiyinyue.top

C#:   Debug.Assert(x > 0);
来源：http://imt.wangdashe.top

[H08] 获取错误信息与堆栈
来源：http://iwg.yuanzhike.top

Py:   str(e);  traceback.format_exc()
来源：http://thc.epnwcf.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://esz.cashguo.top

JS:   e.message;  e.stack
来源：http://rjb.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qaq.fktsv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wxb.hongshengwenyu.top

Go:   err.Error()
来源：http://rzw.xuanzx.com

Ruby: e.message;  e.backtrace
来源：http://fnr.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://qkg.zhaomingkeji.xyz

[H09] 带错误码的异常
来源：http://mme.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://amk.jyoumei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qiw.ivvv.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mzp.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ooz.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://opm.nanxuanxn.top


<!-- 参考信息 -->