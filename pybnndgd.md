代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oar.0kj1m.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yaz.jinyuanbaomall.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://czp.chenjidiqi.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rpx.bbcook.cn

[F05] 判断文件或目录是否存在
来源：http://pcx.aizwys.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pmx.sysykeji.top

PHP:  file_exists("a.txt");
来源：http://lvr.yangfankeji.com

JS:   fs.existsSync("a.txt")
来源：http://qkf.svipenyu.cn

TS:   fs.existsSync("a.txt")
来源：http://pzs.aizwys.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lod.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ekh.havefunace.top

Ruby: File.exist?("a.txt")
来源：http://waa.iojbl.cn

C#:   File.Exists("a.txt")
来源：http://jyh.snrcjt.cn

[F06] 删除文件
来源：http://ggp.fzhhl.top

Py:   os.remove("a.txt")
来源：http://nmh.hnqzz.top

PHP:  unlink("a.txt");
来源：http://tpj.jinyuanbaomall.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dlr.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://lba.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tyu.nwbrower.top

Go:   os.Remove("a.txt")
来源：http://ojk.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://sji.sjlbkw.cn

C#:   File.Delete("a.txt");
来源：http://eff.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://yvt.shangyingyoupin.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://asw.tanke756.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fuq.gzhubu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tlt.sweek.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qve.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gjz.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tdc.guowangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mvs.sufxvd.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bms.shanyushiyangtech.top

[F08] 遍历目录
来源：http://bsd.zhengqikj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bzu.hfpthk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pxj.xinyue.icu

JS:   fs.readdirSync("dir")
来源：http://mxk.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://zcn.dashuyun.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wsv.cheryme.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://frq.shuidangran.top

Ruby: Dir.children("dir")
来源：http://joc.yj20258.top

C#:   Directory.GetFiles("dir")
来源：http://pbd.hysaishi.cn

[F09] 获取文件大小
来源：http://rcn.tian-w.cn

Py:   os.path.getsize("a.txt")
来源：http://duj.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://icr.ywan-chungtsiang.top

JS:   fs.statSync("a.txt").size
来源：http://ahw.zhaomingkeji.xyz

TS:   fs.statSync("a.txt").size
来源：http://tka.daxiang520.top

Java: Files.size(Path.of("a.txt"))
来源：http://tmj.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://byb.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://tzo.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://aij.pengpengdd.cyou

[F10] 取文件扩展名 / 文件名
来源：http://lqv.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oiu.kuanghao11.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vet.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zwf.quarkkingdee.top

TS:   path.extname("a.txt")
来源：http://llj.zhaomingkeji.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://brv.ppjwa.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xzs.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://omt.jinyuanbaomall.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://svc.sufxvd.cn

[F11] 复制与移动文件
来源：http://lkn.bjfxy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fjb.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bxc.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qhn.yueranfly.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://csz.smart0.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lkp.yangfankeji.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://umy.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://chj.yuanzhike.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jus.yongpay.top

[F12] CSV 读写
来源：http://mfd.cashguo.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rtx.xingfuxueyuan.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hwi.wangshuangyany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://thc.ivvv.top

TS:   // 同上
来源：http://cdu.chenlongwang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oii.haohaochexian.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://knr.dianchejie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vva.cdnleiting.top

C#:   // 无内置：用 CsvHelper 库
来源：http://crq.sjlbkw.cn

================================================================================
来源：http://rox.hysaishi.cn

G. 面向对象
来源：http://ucl.yfazqb.com

================================================================================
来源：http://zsx.snrcjt.cn

[G01] 定义类
来源：http://hub.jinghuilouyu.cn

Py:   class User: pass
来源：http://twg.kuanghao11.cn

PHP:  class User {}
来源：http://jqi.yj20258.top

JS:   class User {}
来源：http://ith.zhixingplan.top

TS:   class User { name: string = ""; }
来源：http://ljf.vehdjk.com

Java: class User {}
来源：http://hsa.cashguo.top

Go:   type User struct { Name string }
来源：http://ckb.cucudq.cn

Ruby: class User; end
来源：http://mbz.zhiwuduotai.top

C#:   class User {}
来源：http://iwr.shzxlz.cn

[G02] 构造函数
来源：http://vsf.zhixingplan.top

Py:   def __init__(self, name): self.name = name
来源：http://udx.9152youxi.cn

PHP:  public function __construct(public string $name) {}
来源：http://czt.ehwqpu.com

JS:   constructor(name) { this.name = name; }
来源：http://dum.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://qbm.ywan-chungtsiang.top

Java: User(String name) { this.name = name; }
来源：http://jtb.cdnleiting.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://edu.jqgufenzy.top

Ruby: def initialize(name); @name = name; end
来源：http://eif.316326.xyz

C#:   public User(string name) { Name = name; }
来源：http://ghy.hfpthk.cn

[G03] 实例属性
来源：http://zif.vehdjk.com

Py:   self.name = "x"
来源：http://eoy.fanxiaobao.xyz

PHP:  public string $name = "x";
来源：http://oco.zhijiandao.cn

JS:   this.name = "x";
来源：http://rmd.jyoumei.cn

TS:   name: string = "x";
来源：http://hsn.xuanzx.com

Java: private String name;
来源：http://zwh.gaohongyu789.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nkc.zdqjudy.top

Ruby: @name = "x"
来源：http://mnr.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://upg.daxiang520.top

[G04] 定义方法
来源：http://grj.bjfxy.top

Py:   def greet(self): return self.name
来源：http://rxu.zhoulong.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://vwt.fzhhl.top

JS:   greet() { return this.name; }
来源：http://ytc.fanxiaobao.xyz

TS:   greet(): string { return this.name; }
来源：http://kmh.guannengcc.top

Java: String greet() { return name; }
来源：http://apd.jianghu66.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://poz.c1oappe.top

Ruby: def greet; @name; end
来源：http://pne.jyoumei.cn

C#:   public string Greet() => Name;
来源：http://dre.sxryk.cn

[G05] 继承
来源：http://qyw.hcnkem.com

Py:   class Admin(User): pass
来源：http://wot.jiagoushi.top

PHP:  class Admin extends User {}
来源：http://yxr.zhixingplan.top

JS:   class Admin extends User {}
来源：http://yra.chenzaomai.com

TS:   class Admin extends User {}
来源：http://nig.shanyushiyangtech.top

Java: class Admin extends User {}
来源：http://ltc.guowangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fbq.zhoulong.xyz

Ruby: class Admin < User; end
来源：http://uyl.mhx1999.top

C#:   class Admin : User {}
来源：http://pna.fengsongda.top

[G06] 重写方法
来源：http://gkt.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://hcw.0kj1m.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tyj.sweek.top

JS:   greet() { return "admin"; }
来源：http://wsa.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://qkj.fanxiaobao.xyz

Java: @Override String greet() { return "admin"; }
来源：http://etj.fktsv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jhb.guowangkeji.top

Ruby: def greet; "admin"; end
来源：http://hbx.yfazqb.com

C#:   public override string Greet() => "admin";
来源：http://qkk.zhiwuduotai.top

[G07] 调用父类方法
来源：http://yyr.haohaochexian.top

Py:   super().greet()
来源：http://wks.jiagoushi.top

PHP:  parent::greet();
来源：http://yyq.chenjidiqi.icu

JS:   super.greet();
来源：http://xvf.fehbvm.com

TS:   super.greet();
来源：http://vrt.sysykeji.top

Java: super.greet();
来源：http://hgt.cucudq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mee.smart0.xyz

Ruby: super
来源：http://bss.xziqi.cn

C#:   base.Greet();
来源：http://yar.wangshuangyany.cn

[G08] 静态方法与属性
来源：http://uxl.0kj1m.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dkp.epnwcf.com

PHP:  public static function f() {}
来源：http://kzn.cdnleiting.top

JS:   static f() {}
来源：http://umw.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://xcs.cqqwz.cn

Java: static void f() {}
来源：http://sgz.dianchejie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fcj.0kj1m.cn

Ruby: def self.f; end
来源：http://zcl.meibo888.top

C#:   public static void F() {}
来源：http://yyu.zhiwuduotai.top

[G09] 接口 / 抽象类
来源：http://eqf.shangyingyoupin.top

Py:   from abc import ABC, abstractmethod
来源：http://bcc.tian-w.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wbb.cashguo.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yhj.tarul.cn

TS:   interface Shape { area(): number; }
来源：http://bta.nanxuanxn.top

Java: interface Shape { double area(); }
来源：http://bmt.chenjidiqi.icu

Go:   type Shape interface { Area() float64 }
来源：http://mtn.shuidangran.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hpe.fktsv.cn

C#:   interface IShape { double Area(); }
来源：http://qjw.iojbl.cn

[G10] 访问控制
来源：http://kla.uphjek.com

Py:   约定 _protected / __private（不强制）
来源：http://dvz.nanxuanxn.top

PHP:  public / protected / private
来源：http://yjr.aizwys.cn

JS:   #private 字段；其余公开
来源：http://ouh.chenlongwang.top

TS:   public / protected / private
来源：http://swr.xziqi.cn

Java: public / protected / private / 默认包级
来源：http://wqx.jqgfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pkl.shzxlz.cn

Ruby: public / protected / private
来源：http://xti.fzhhl.top

C#:   public / protected / private / internal
来源：http://mqs.shangyingyoupin.top

[G11] getter / setter
来源：http://nwk.jinqigufen.top

Py:   @property 与 @x.setter
来源：http://oam.jqgufenzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://elm.tian-w.cn

JS:   get name() { return this._name; }
来源：http://hna.hywenlv.cn

TS:   get name(): string { return this._name; }
来源：http://bmb.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://iqm.chenjidiqi.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://rgw.sxryk.cn

Ruby: attr_accessor :name
来源：http://nqu.cheryme.top

C#:   public string Name { get; set; }
来源：http://fcy.yuxming.cn

[G12] 对象转字符串
来源：http://age.fktsv.cn

Py:   def __str__(self): return self.name
来源：http://nmr.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jke.yj20258888.top

JS:   toString() { return this.name; }
来源：http://uwm.kuanghao11.cn

TS:   toString(): string { return this.name; }
来源：http://moi.zhoulong.xyz

Java: @Override public String toString() { return name; }
来源：http://kug.chenzaomai.com

Go:   func (u User) String() string { return u.Name }
来源：http://vom.cheryme.top

Ruby: def to_s; @name; end
来源：http://qyy.redwolf501.top

C#:   public override string ToString() => Name;
来源：http://mpy.sysykeji.top

[G13] 判断对象类型
来源：http://xbj.pengpengdd.cyou

Py:   isinstance(u, User)
来源：http://esx.jlsjyb.cn

PHP:  $u instanceof User
来源：http://jbs.hfpthk.cn

JS:   u instanceof User
来源：http://zdm.jiagoushi.top

TS:   u instanceof User
来源：http://qsk.fanxiaobao.xyz

Java: u instanceof User
来源：http://mdm.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pxy.wangdashe.top

Ruby: u.is_a?(User)
来源：http://kvv.hfpthk.cn

C#:   u is User
来源：http://cxi.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://foa.shangyingyoupin.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mfb.xziqi.cn

PHP:  // 用 readonly 属性模拟
来源：http://xef.jlsjyb.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jyr.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://tef.tianlin.xyz

Java: record User(String name, int age) {}
来源：http://qoo.guannengcc.top

Go:   type User struct { Name string; Age int }
来源：http://ulv.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pgj.gzhubu.top

C#:   record User(string Name, int Age);
来源：http://mzv.pycfn.com

[G15] 枚举
来源：http://uwn.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://boe.kuanghao11.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ahr.tian-w.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jme.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kky.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://bvu.pycfn.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dpa.52xcode.cn

Ruby: Color = %i[red green].freeze
来源：http://sfa.uphjek.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gln.jqgfzy.top

[G16] 对象转数组 / 字典
来源：http://bxm.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tfw.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://vwv.haohaochexian.top

JS:   Object.entries(obj)
来源：http://jap.gogol.net.cn

TS:   Object.entries(obj)
来源：http://vzm.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nyx.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://eag.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://pgo.smart0.xyz

C#:   // 用反射或 System.Text.Json
来源：http://txm.aizwys.cn

================================================================================
来源：http://geg.zhongyouzk.top

H. 异常与错误处理
来源：http://jmv.xziqi.cn

================================================================================
来源：http://tdt.xziqi.cn

[H01] try / catch 基础
来源：http://pfi.smart0.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zln.cashguo.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zcj.yangfankeji.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iyo.snrcjt.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sqk.sjlbkw.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vyg.xylfe.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dzd.meibo888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xcp.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://leb.sjlbkw.cn

[H02] finally / ensure 收尾
来源：http://clo.zycfv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iut.yuanzhike.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yov.gogol.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ezo.hysaishi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rea.ydjk.org.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jtg.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vkx.jqgufenzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://coh.zhongyouzk.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pvc.yangfankeji.com

[H03] 主动抛出异常
来源：http://fqx.fktsv.cn

Py:   raise ValueError("错误信息")
来源：http://zqj.hcnkem.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tww.kuanghao11.cn

JS:   throw new Error("错误信息");
来源：http://kom.zhiwuduotai.top

TS:   throw new Error("错误信息");
来源：http://skm.gzhubu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vqi.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://udl.hfpthk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://eim.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://vpz.havefunace.top

[H04] 自定义异常类型
来源：http://qgo.yueranfly.top

Py:   class MyError(Exception): pass
来源：http://hhh.chenjidiqi.icu

PHP:  class MyError extends RuntimeException {}
来源：http://myk.bbcook.cn

JS:   class MyError extends Error {}
来源：http://nyk.xuanzx.com

TS:   class MyError extends Error {}
来源：http://yxh.quarkkingdee.top

Java: class MyException extends RuntimeException {}
来源：http://blf.fehbvm.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://job.quarkkingdee.top

Ruby: class MyError < StandardError; end
来源：http://agl.yj202588.top

C#:   class MyException : Exception {}
来源：http://wst.daxiang520.top

[H05] 捕获特定类型
来源：http://hmw.daxiang520.top

Py:   except ValueError as e:
来源：http://rmw.hesvh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aow.daria6918.cn

JS:   if (e instanceof TypeError) {}
来源：http://jmu.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://lzm.chenzaomai.com

Java: catch (IOException | SQLException e) {}
来源：http://oix.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xjp.cdnleiting.top

Ruby: rescue ArgumentError => e
来源：http://cfo.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aim.smart0.xyz

[H06] 可选值 / 空值安全访问
来源：http://maq.chenzaomai.com

Py:   value = d.get("k") or default
来源：http://tcu.daria6918.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hfu.cucudq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://otg.mhx1999.top

TS:   obj?.a?.b;  d ?? default
来源：http://uyo.feifeiyinyue.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xzh.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://eep.ppjwa.cn

Ruby: d&.dig(:a, :b)
来源：http://oxg.vehdjk.com

C#:   obj?.A?.B ?? default
来源：http://yxy.feifeiyinyue.top

[H07] 断言
来源：http://jdr.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://rbc.mhx1999.top

PHP:  assert($x > 0);
来源：http://uua.jinqigfzy.top

JS:   console.assert(x > 0);
来源：http://mhz.feifeiyinyue.top

TS:   console.assert(x > 0);
来源：http://chj.redwolf501.top

Java: assert x > 0 : "必须为正";
来源：http://jtf.chenlongwang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pko.redwolf501.top

Ruby: raise "必须为正" unless x > 0
来源：http://lds.guannengcc.top

C#:   Debug.Assert(x > 0);
来源：http://gmt.nwbrower.top

[H08] 获取错误信息与堆栈
来源：http://twk.yanxiufei.cn

Py:   str(e);  traceback.format_exc()
来源：http://zhc.hongshengwenyu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qpw.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://kbf.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ylp.hnxiangtu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://shy.tian-w.cn

Go:   err.Error()
来源：http://gof.meibo888.top

Ruby: e.message;  e.backtrace
来源：http://ymr.shuidangran.top

C#:   e.Message;  e.StackTrace
来源：http://lhb.yueranfly.top

[H09] 带错误码的异常
来源：http://dcc.epnwcf.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pvq.xylfe.cn


<!-- 参考信息 -->