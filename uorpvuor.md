代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xel.zdbjq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kxd.haohaochexian.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qce.jiagoushi.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://enm.0kj1m.cn

[F05] 判断文件或目录是否存在
来源：http://evx.c1oappe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://agu.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://qmy.havefunace.top

JS:   fs.existsSync("a.txt")
来源：http://cot.nwbrower.top

TS:   fs.existsSync("a.txt")
来源：http://ezo.yanxiufei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cpx.tianlin.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tpx.aibaodan.cn

Ruby: File.exist?("a.txt")
来源：http://ubf.jlsjyb.cn

C#:   File.Exists("a.txt")
来源：http://oti.aizwys.cn

[F06] 删除文件
来源：http://wul.snrcjt.cn

Py:   os.remove("a.txt")
来源：http://qzj.hywenlv.cn

PHP:  unlink("a.txt");
来源：http://dec.epnwcf.com

JS:   fs.unlinkSync("a.txt")
来源：http://psx.tanke756.top

TS:   fs.unlinkSync("a.txt")
来源：http://qrk.meibo888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zrt.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://loa.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://mdq.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://kmt.jianghu66.top

[F07] 创建目录（含多级）
来源：http://blm.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xuq.hammf.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kcg.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rlw.bbcook.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://guv.chenjidiqi.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ihk.haohaochexian.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bjw.nanxuanxn.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aqt.nwbrower.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eij.ctjpmb.com

[F08] 遍历目录
来源：http://znn.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://qfa.iojbl.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aeo.sxryk.cn

JS:   fs.readdirSync("dir")
来源：http://fcs.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://tqr.epnwcf.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://voj.tianlin.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://ajx.zdbjq.cn

Ruby: Dir.children("dir")
来源：http://jcw.sxryk.cn

C#:   Directory.GetFiles("dir")
来源：http://kkk.316326.xyz

[F09] 获取文件大小
来源：http://aqj.sysykeji.top

Py:   os.path.getsize("a.txt")
来源：http://qxv.nanxinkj.top

PHP:  filesize("a.txt");
来源：http://dwm.xuanzx.com

JS:   fs.statSync("a.txt").size
来源：http://wej.dashuyun.cn

TS:   fs.statSync("a.txt").size
来源：http://rao.redwolf501.top

Java: Files.size(Path.of("a.txt"))
来源：http://zgj.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vks.hfpthk.cn

Ruby: File.size("a.txt")
来源：http://dxd.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://lfm.sxryk.cn

[F10] 取文件扩展名 / 文件名
来源：http://vgb.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kmc.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gfw.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hzv.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://pek.yj20258.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yfz.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yga.yangfankeji.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aof.tianlin.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ctb.redwolf501.top

[F11] 复制与移动文件
来源：http://sng.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ydr.ivvv.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oxq.shuidangran.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aua.hesvh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yyx.fktsv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zfl.chenlongwang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lzr.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://alv.cheryme.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oox.zhongyouzk.top

[F12] CSV 读写
来源：http://jeu.shangyingyoupin.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oup.fengsongda.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gau.bbcook.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hol.shangyingyoupin.top

TS:   // 同上
来源：http://pqj.guowangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://otp.jinqigufen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bxq.fzhhl.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://haj.ivvv.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zde.zhoulong.xyz

================================================================================
来源：http://psg.jlsjyb.cn

G. 面向对象
来源：http://wfu.iojbl.cn

================================================================================
来源：http://sjb.tian-w.cn

[G01] 定义类
来源：http://gde.vehdjk.com

Py:   class User: pass
来源：http://xxv.redwolf501.top

PHP:  class User {}
来源：http://sru.ctjpmb.com

JS:   class User {}
来源：http://hfw.yuanzhike.top

TS:   class User { name: string = ""; }
来源：http://dcd.xuetiantiany.cn

Java: class User {}
来源：http://jla.aizwys.cn

Go:   type User struct { Name string }
来源：http://ddd.hysaishi.cn

Ruby: class User; end
来源：http://psx.zdbjq.cn

C#:   class User {}
来源：http://axp.xuetiantiany.cn

[G02] 构造函数
来源：http://glj.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://hll.52xcode.cn

PHP:  public function __construct(public string $name) {}
来源：http://aem.shanyushiyangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://aco.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://sxr.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://ejg.epnwcf.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lyc.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://fze.vqdsnc.cn

C#:   public User(string name) { Name = name; }
来源：http://wri.tarul.cn

[G03] 实例属性
来源：http://cjp.yj20258888.top

Py:   self.name = "x"
来源：http://rry.pycfn.com

PHP:  public string $name = "x";
来源：http://acj.jiagoushi.top

JS:   this.name = "x";
来源：http://vti.cucudq.cn

TS:   name: string = "x";
来源：http://uwq.hnxiangtu.top

Java: private String name;
来源：http://fxu.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ptl.sweek.top

Ruby: @name = "x"
来源：http://gsh.zhongyouzk.top

C#:   public string Name { get; set; } = "x";
来源：http://olk.yj20258.top

[G04] 定义方法
来源：http://ixt.hesvh.cn

Py:   def greet(self): return self.name
来源：http://cjt.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jvi.yfazqb.com

JS:   greet() { return this.name; }
来源：http://gsb.fktsv.cn

TS:   greet(): string { return this.name; }
来源：http://pqd.snrcjt.cn

Java: String greet() { return name; }
来源：http://gex.svipenyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ptd.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://hog.hongshengwenyu.top

C#:   public string Greet() => Name;
来源：http://wft.tarul.cn

[G05] 继承
来源：http://yvc.zhixingplan.top

Py:   class Admin(User): pass
来源：http://eze.fzhhl.top

PHP:  class Admin extends User {}
来源：http://mhe.fanxiaobao.xyz

JS:   class Admin extends User {}
来源：http://ssg.guannengcc.top

TS:   class Admin extends User {}
来源：http://qlx.wangdashe.top

Java: class Admin extends User {}
来源：http://eyl.meibo888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hyh.gaohongyu789.top

Ruby: class Admin < User; end
来源：http://wua.cdnleiting.top

C#:   class Admin : User {}
来源：http://ycv.guowangkeji.top

[G06] 重写方法
来源：http://gbo.yonumen.top

Py:   def greet(self): return "admin"
来源：http://nmw.zhongyouzk.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xbk.fktsv.cn

JS:   greet() { return "admin"; }
来源：http://vva.vqdsnc.cn

TS:   greet(): string { return "admin"; }
来源：http://zdc.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://diq.daria6918.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fwq.ywan-chungtsiang.top

Ruby: def greet; "admin"; end
来源：http://moo.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://zmo.hysaishi.cn

[G07] 调用父类方法
来源：http://sjd.sxryk.cn

Py:   super().greet()
来源：http://jzd.jiagoushi.top

PHP:  parent::greet();
来源：http://vro.sweek.top

JS:   super.greet();
来源：http://ckc.sufxvd.cn

TS:   super.greet();
来源：http://lfs.uphjek.com

Java: super.greet();
来源：http://kzv.nanxuanxn.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ocz.yfazqb.com

Ruby: super
来源：http://jjv.yueranfly.top

C#:   base.Greet();
来源：http://zml.aibaodan.cn

[G08] 静态方法与属性
来源：http://vct.shanyushiyangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bas.xziqi.cn

PHP:  public static function f() {}
来源：http://mmz.cashguo.top

JS:   static f() {}
来源：http://gmp.yonumen.top

TS:   static f(): void {}
来源：http://twu.meibo888.top

Java: static void f() {}
来源：http://scq.jqgufenzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rug.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://sos.epnwcf.com

C#:   public static void F() {}
来源：http://rpo.yj20258888.top

[G09] 接口 / 抽象类
来源：http://zie.daxiang520.top

Py:   from abc import ABC, abstractmethod
来源：http://arm.zhongyouzk.top

PHP:  interface Shape { public function area(): float; }
来源：http://ngd.nanxinkj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hdu.yueranfly.top

TS:   interface Shape { area(): number; }
来源：http://nvf.birdmap.top

Java: interface Shape { double area(); }
来源：http://jhd.xingfuxueyuan.xyz

Go:   type Shape interface { Area() float64 }
来源：http://foy.shanyushiyangtech.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xuh.9152youxi.cn

C#:   interface IShape { double Area(); }
来源：http://jle.haohaochexian.top

[G10] 访问控制
来源：http://rdl.hysaishi.cn

Py:   约定 _protected / __private（不强制）
来源：http://alt.cucudq.cn

PHP:  public / protected / private
来源：http://otp.xuanzx.com

JS:   #private 字段；其余公开
来源：http://pfh.vehdjk.com

TS:   public / protected / private
来源：http://xlm.chenzaomai.com

Java: public / protected / private / 默认包级
来源：http://frz.quarkkingdee.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wku.jinghuilouyu.cn

Ruby: public / protected / private
来源：http://ihx.quarkkingdee.top

C#:   public / protected / private / internal
来源：http://ulk.yongpay.top

[G11] getter / setter
来源：http://jhi.vehdjk.com

Py:   @property 与 @x.setter
来源：http://whj.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tiz.nanxuanxn.top

JS:   get name() { return this._name; }
来源：http://xux.tanke756.top

TS:   get name(): string { return this._name; }
来源：http://pdh.0kj1m.cn

Java: public String getName() { return name; }
来源：http://nsm.guowangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ljl.hesvh.cn

Ruby: attr_accessor :name
来源：http://dvt.epnwcf.com

C#:   public string Name { get; set; }
来源：http://lqi.pycfn.com

[G12] 对象转字符串
来源：http://vxx.bjfxy.top

Py:   def __str__(self): return self.name
来源：http://eks.daria6918.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tlr.sxryk.cn

JS:   toString() { return this.name; }
来源：http://rps.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://gsm.guannengcc.top

Java: @Override public String toString() { return name; }
来源：http://umk.shangyingyoupin.top

Go:   func (u User) String() string { return u.Name }
来源：http://lyy.yanxiufei.cn

Ruby: def to_s; @name; end
来源：http://ydb.zhiwuduotai.top

C#:   public override string ToString() => Name;
来源：http://jtt.fanxiaobao.xyz

[G13] 判断对象类型
来源：http://ymr.ehwqpu.com

Py:   isinstance(u, User)
来源：http://oar.xingfuxueyuan.xyz

PHP:  $u instanceof User
来源：http://enq.feifeiyinyue.top

JS:   u instanceof User
来源：http://xdj.0kj1m.cn

TS:   u instanceof User
来源：http://iil.hysaishi.cn

Java: u instanceof User
来源：http://wpk.shanyushiyangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pws.yfazqb.com

Ruby: u.is_a?(User)
来源：http://fbe.svipenyu.cn

C#:   u is User
来源：http://oiz.xuanzx.com

[G14] 数据类 / record
来源：http://van.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qql.52xcode.cn

PHP:  // 用 readonly 属性模拟
来源：http://yzh.yueranfly.top

JS:   // 无内置：普通类或对象字面量
来源：http://vpf.yj202588.top

TS:   type User = { name: string; age: number };
来源：http://jqb.hfpthk.cn

Java: record User(String name, int age) {}
来源：http://bib.cdnleiting.top

Go:   type User struct { Name string; Age int }
来源：http://xhi.xinyue.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://crx.haohaochexian.top

C#:   record User(string Name, int Age);
来源：http://gzh.fengsongda.top

[G15] 枚举
来源：http://mug.316326.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ugu.cucudq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hza.9152youxi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cmy.yueranfly.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mvx.shanyushiyangkeji.top

Java: enum Color { RED, GREEN }
来源：http://zzn.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fhv.meibo888.top

Ruby: Color = %i[red green].freeze
来源：http://wvd.xinyue.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://daf.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://qux.mhx1999.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rgk.fzhhl.top

PHP:  get_object_vars($obj);
来源：http://mmc.bbcook.cn

JS:   Object.entries(obj)
来源：http://els.gotoacloud.top

TS:   Object.entries(obj)
来源：http://sos.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://byn.yj20258888.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zdj.ydzc1.top

Ruby: obj.instance_variables
来源：http://yis.epnwcf.com

C#:   // 用反射或 System.Text.Json
来源：http://txz.vehdjk.com

================================================================================
来源：http://qmd.xingfuxueyuan.xyz

H. 异常与错误处理
来源：http://iij.hongshengwenyu.top

================================================================================
来源：http://xfu.shzxlz.cn

[H01] try / catch 基础
来源：http://xzj.fzhhl.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gaa.daxiang520.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wgh.ivvv.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zsp.hfpthk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ibm.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ebq.xuanzx.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tll.zhengqikj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nsd.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qhr.hcnkem.com

[H02] finally / ensure 收尾
来源：http://zeh.shuidangran.top

Py:   try: f()⏎finally: cleanup()
来源：http://ngv.shanyushiyangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gkg.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pvl.kuanghao11.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mhf.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wey.ivvv.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wpo.jinqigufen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pez.yvedp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://btk.quarkkingdee.top

[H03] 主动抛出异常
来源：http://qju.nanxinkj.top

Py:   raise ValueError("错误信息")
来源：http://bcw.jinqigfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jcv.feifeiyinyue.top

JS:   throw new Error("错误信息");
来源：http://gza.jinqigufen.top

TS:   throw new Error("错误信息");
来源：http://gvm.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lki.zhiwuduotai.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iwl.jqgufenzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kql.aibaodan.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vnx.zhijiandao.cn

[H04] 自定义异常类型
来源：http://tkc.zhoulong.xyz

Py:   class MyError(Exception): pass
来源：http://ubk.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ozk.xylfe.cn

JS:   class MyError extends Error {}
来源：http://rbr.52xcode.cn

TS:   class MyError extends Error {}
来源：http://tik.c1oappe.top

Java: class MyException extends RuntimeException {}
来源：http://vbf.daxiang520.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://brm.jlsjyb.cn

Ruby: class MyError < StandardError; end
来源：http://ira.sysykeji.top

C#:   class MyException : Exception {}
来源：http://hie.yuxming.cn

[H05] 捕获特定类型
来源：http://znv.sysykeji.top

Py:   except ValueError as e:
来源：http://csl.xingfuxueyuan.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lrc.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://iif.yj202588.top

TS:   if (e instanceof TypeError) {}
来源：http://maj.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://zyi.ehwqpu.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tzc.sjlbkw.cn

Ruby: rescue ArgumentError => e
来源：http://zjm.zhongyouzk.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ftu.tian-w.cn

[H06] 可选值 / 空值安全访问
来源：http://zup.uphjek.com

Py:   value = d.get("k") or default
来源：http://ogy.316326.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://whc.c1oappe.top

JS:   obj?.a?.b;  d ?? default
来源：http://xof.jqgufenzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://ydc.pycfn.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rss.zhengqikj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://krb.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://avx.cashguo.top

C#:   obj?.A?.B ?? default
来源：http://btz.fehbvm.com

[H07] 断言
来源：http://buu.gzhubu.top

Py:   assert x > 0, "必须为正"
来源：http://vii.yj202588.top

PHP:  assert($x > 0);
来源：http://kwo.fehbvm.com

JS:   console.assert(x > 0);
来源：http://uet.sysykeji.top

TS:   console.assert(x > 0);
来源：http://kyd.feifeiyinyue.top

Java: assert x > 0 : "必须为正";
来源：http://hrr.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eva.bjfxy.top

Ruby: raise "必须为正" unless x > 0
来源：http://wtq.0kj1m.cn

C#:   Debug.Assert(x > 0);
来源：http://rxb.daxiang520.top

[H08] 获取错误信息与堆栈
来源：http://cjt.hfpthk.cn

Py:   str(e);  traceback.format_exc()
来源：http://hsp.yangfankeji.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fpw.jlsjyb.cn

JS:   e.message;  e.stack
来源：http://lof.fzhhl.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kwm.zhiwuduotai.top

Java: e.getMessage();  e.printStackTrace()
来源：http://myd.gotoacloud.top

Go:   err.Error()
来源：http://oax.vqdsnc.cn

Ruby: e.message;  e.backtrace
来源：http://eej.hammf.cn

C#:   e.Message;  e.StackTrace
来源：http://nbi.redwolf501.top

[H09] 带错误码的异常
来源：http://sko.guannengcc.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ohc.nwbrower.top


<!-- 参考信息 -->