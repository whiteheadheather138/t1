代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://lzo.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mfq.xingfuxueyuan.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zah.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://rth.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://qhg.9152youxi.cn

[F06] 删除文件
来源：http://jjw.hnqzz.top

Py:   os.remove("a.txt")
来源：http://sha.yongpay.top

PHP:  unlink("a.txt");
来源：http://efm.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://mze.ctjpmb.com

TS:   fs.unlinkSync("a.txt")
来源：http://qus.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wwu.hesvh.cn

Go:   os.Remove("a.txt")
来源：http://cor.nwbrower.top

Ruby: File.delete("a.txt")
来源：http://jpq.ywan-chungtsiang.top

C#:   File.Delete("a.txt");
来源：http://jco.feifeiyinyue.top

[F07] 创建目录（含多级）
来源：http://rrb.0kj1m.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dzg.shzxlz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qde.c1oappe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oxy.aibaodan.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ibr.jqgufenzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ibo.shzxlz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hyd.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://moo.shuidangran.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lwi.yanxiufei.cn

[F08] 遍历目录
来源：http://auk.ppjwa.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ami.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tpy.0kj1m.cn

JS:   fs.readdirSync("dir")
来源：http://bcz.0kj1m.cn

TS:   fs.readdirSync("dir")
来源：http://woc.yj20258.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jwv.ydzc1.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rgi.chenzaomai.com

Ruby: Dir.children("dir")
来源：http://zcz.jinqigufen.top

C#:   Directory.GetFiles("dir")
来源：http://ejq.jqgufenzy.top

[F09] 获取文件大小
来源：http://pil.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://yxi.smart0.xyz

PHP:  filesize("a.txt");
来源：http://dan.yuxming.cn

JS:   fs.statSync("a.txt").size
来源：http://vxc.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://poo.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gdv.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kik.hesvh.cn

Ruby: File.size("a.txt")
来源：http://joe.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://urw.cqqwz.cn

[F10] 取文件扩展名 / 文件名
来源：http://iqc.fehbvm.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dnj.chenjidiqi.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rdr.shanyushiyangtech.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bfs.yj20258.top

TS:   path.extname("a.txt")
来源：http://sps.wangshuangyany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bjd.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tvy.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kkw.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gde.ehwqpu.com

[F11] 复制与移动文件
来源：http://htk.nanxuanxn.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://snb.dianchejie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ilg.dianchejie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ntp.yuxming.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sue.zhijiandao.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ryk.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bzq.meibo888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wac.yuanzhike.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bet.ywan-chungtsiang.top

[F12] CSV 读写
来源：http://peb.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dvk.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jbh.jinqigufen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wcf.cucudq.cn

TS:   // 同上
来源：http://hlg.zhongyouzk.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://npe.feifeiyinyue.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kpc.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gof.jinqigufen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uez.52xcode.cn

================================================================================
来源：http://feu.hysaishi.cn

G. 面向对象
来源：http://yzy.sufxvd.cn

================================================================================
来源：http://ikq.hesvh.cn

[G01] 定义类
来源：http://gaa.ehwqpu.com

Py:   class User: pass
来源：http://edx.zdqjudy.top

PHP:  class User {}
来源：http://aio.hongshengwenyu.top

JS:   class User {}
来源：http://ofu.xuetiantiany.cn

TS:   class User { name: string = ""; }
来源：http://zdw.jinyuanbaomall.cn

Java: class User {}
来源：http://ntj.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://xzo.vqdsnc.cn

Ruby: class User; end
来源：http://ynw.andypj.xyz

C#:   class User {}
来源：http://jfn.yuanzhike.top

[G02] 构造函数
来源：http://awx.wangdashe.top

Py:   def __init__(self, name): self.name = name
来源：http://leg.daria6918.cn

PHP:  public function __construct(public string $name) {}
来源：http://ijx.fzhhl.top

JS:   constructor(name) { this.name = name; }
来源：http://ejj.yfazqb.com

TS:   constructor(public name: string) {}
来源：http://nww.cashguo.top

Java: User(String name) { this.name = name; }
来源：http://oht.ivvv.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nlv.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://jrt.shzxlz.cn

C#:   public User(string name) { Name = name; }
来源：http://vio.tarul.cn

[G03] 实例属性
来源：http://kxb.yj202588.top

Py:   self.name = "x"
来源：http://umo.hongshengwenyu.top

PHP:  public string $name = "x";
来源：http://ids.ctjpmb.com

JS:   this.name = "x";
来源：http://pvb.guannengcc.top

TS:   name: string = "x";
来源：http://ygy.jyoumei.cn

Java: private String name;
来源：http://tuk.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nba.cucudq.cn

Ruby: @name = "x"
来源：http://isu.mhx1999.top

C#:   public string Name { get; set; } = "x";
来源：http://lde.jinqigufen.top

[G04] 定义方法
来源：http://xqg.hcnkem.com

Py:   def greet(self): return self.name
来源：http://syk.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jfi.birdmap.top

JS:   greet() { return this.name; }
来源：http://bgk.hammf.cn

TS:   greet(): string { return this.name; }
来源：http://sbt.yvedp.cn

Java: String greet() { return name; }
来源：http://idx.uphjek.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://pfc.hfpthk.cn

Ruby: def greet; @name; end
来源：http://gso.tarul.cn

C#:   public string Greet() => Name;
来源：http://uhu.sjlbkw.cn

[G05] 继承
来源：http://mfz.0kj1m.cn

Py:   class Admin(User): pass
来源：http://hnd.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://uin.shuidangran.top

JS:   class Admin extends User {}
来源：http://anm.yangfankeji.com

TS:   class Admin extends User {}
来源：http://tag.hammf.cn

Java: class Admin extends User {}
来源：http://ogh.hnqzz.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://asz.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://unt.aizwys.cn

C#:   class Admin : User {}
来源：http://ien.xuanzx.com

[G06] 重写方法
来源：http://emp.feifeiyinyue.top

Py:   def greet(self): return "admin"
来源：http://nsf.hnqzz.top

PHP:  public function greet(): string { return "admin"; }
来源：http://shm.meibo888.top

JS:   greet() { return "admin"; }
来源：http://lmn.wangshuangyany.cn

TS:   greet(): string { return "admin"; }
来源：http://fsz.yj20258888.top

Java: @Override String greet() { return "admin"; }
来源：http://xfh.kuanghao11.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tbl.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://ueu.yj202588.top

C#:   public override string Greet() => "admin";
来源：http://dww.tanke756.top

[G07] 调用父类方法
来源：http://tpp.ppjwa.cn

Py:   super().greet()
来源：http://beb.mhx1999.top

PHP:  parent::greet();
来源：http://evz.redwolf501.top

JS:   super.greet();
来源：http://fyt.zhijiandao.cn

TS:   super.greet();
来源：http://rfa.smart0.xyz

Java: super.greet();
来源：http://pzr.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jeg.cdnleiting.top

Ruby: super
来源：http://iys.snrcjt.cn

C#:   base.Greet();
来源：http://fid.yonumen.top

[G08] 静态方法与属性
来源：http://vgy.ydjk.org.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bhx.fanxiaobao.xyz

PHP:  public static function f() {}
来源：http://edf.haohaochexian.top

JS:   static f() {}
来源：http://wpr.andypj.xyz

TS:   static f(): void {}
来源：http://aby.sufxvd.cn

Java: static void f() {}
来源：http://fft.shuidangran.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ljn.yangfankeji.com

Ruby: def self.f; end
来源：http://ndr.andypj.xyz

C#:   public static void F() {}
来源：http://ntt.jinqigufen.top

[G09] 接口 / 抽象类
来源：http://ybv.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://nqn.cdnleiting.top

PHP:  interface Shape { public function area(): float; }
来源：http://srj.jqgfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://uot.wangshuangyany.cn

TS:   interface Shape { area(): number; }
来源：http://nyg.shuidangran.top

Java: interface Shape { double area(); }
来源：http://soc.gaohongyu789.top

Go:   type Shape interface { Area() float64 }
来源：http://htm.xingfuxueyuan.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wnv.hongshengwenyu.top

C#:   interface IShape { double Area(); }
来源：http://cyr.yvedp.cn

[G10] 访问控制
来源：http://rtc.xylfe.cn

Py:   约定 _protected / __private（不强制）
来源：http://omb.wangdashe.top

PHP:  public / protected / private
来源：http://pdb.uphjek.com

JS:   #private 字段；其余公开
来源：http://ywz.xingfuxueyuan.xyz

TS:   public / protected / private
来源：http://bgg.iojbl.cn

Java: public / protected / private / 默认包级
来源：http://mvc.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zpz.aizwys.cn

Ruby: public / protected / private
来源：http://jpn.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://bhx.bjfxy.top

[G11] getter / setter
来源：http://jxb.aizwys.cn

Py:   @property 与 @x.setter
来源：http://trs.pengpengdd.cyou

PHP:  public function getName(): string { return $this->name; }
来源：http://qgq.zhijiandao.cn

JS:   get name() { return this._name; }
来源：http://doe.cucudq.cn

TS:   get name(): string { return this._name; }
来源：http://tul.chenzaomai.com

Java: public String getName() { return name; }
来源：http://kpy.sxryk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hpn.yj20258.top

Ruby: attr_accessor :name
来源：http://yti.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://hiw.iojbl.cn

[G12] 对象转字符串
来源：http://wst.vehdjk.com

Py:   def __str__(self): return self.name
来源：http://fry.jinqigfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://szi.cdnleiting.top

JS:   toString() { return this.name; }
来源：http://nuu.hcnkem.com

TS:   toString(): string { return this.name; }
来源：http://gqr.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://qib.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://sua.kuanghao11.cn

Ruby: def to_s; @name; end
来源：http://qxz.yuanzhike.top

C#:   public override string ToString() => Name;
来源：http://mgz.zhijiandao.cn

[G13] 判断对象类型
来源：http://emx.zdqjudy.top

Py:   isinstance(u, User)
来源：http://vtu.ivvv.top

PHP:  $u instanceof User
来源：http://eie.zhixingplan.top

JS:   u instanceof User
来源：http://cvo.hammf.cn

TS:   u instanceof User
来源：http://vqf.9152youxi.cn

Java: u instanceof User
来源：http://ttd.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qwe.iojbl.cn

Ruby: u.is_a?(User)
来源：http://qfx.jianghu66.top

C#:   u is User
来源：http://gab.yuanzhike.top

[G14] 数据类 / record
来源：http://xqr.quarkkingdee.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fra.snrcjt.cn

PHP:  // 用 readonly 属性模拟
来源：http://siq.smart0.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://bbu.ctjpmb.com

TS:   type User = { name: string; age: number };
来源：http://fiw.zdqjudy.top

Java: record User(String name, int age) {}
来源：http://urk.chenlongwang.top

Go:   type User struct { Name string; Age int }
来源：http://tbr.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dnc.zhijiandao.cn

C#:   record User(string Name, int Age);
来源：http://nmw.sufxvd.cn

[G15] 枚举
来源：http://lvb.mhx1999.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lji.zhoulong.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://wrb.chenjidiqi.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://slp.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jzz.yvedp.cn

Java: enum Color { RED, GREEN }
来源：http://zzw.gaohongyu789.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rnb.fzhhl.top

Ruby: Color = %i[red green].freeze
来源：http://aqi.gzhubu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uxb.pengpengdd.cyou

[G16] 对象转数组 / 字典
来源：http://obj.yanxiufei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lxc.cdnleiting.top

PHP:  get_object_vars($obj);
来源：http://ozh.jinyuanbaomall.cn

JS:   Object.entries(obj)
来源：http://qpe.shuidangran.top

TS:   Object.entries(obj)
来源：http://nqu.zhiwuduotai.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ffl.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://haf.zhengqikj.top

Ruby: obj.instance_variables
来源：http://nfb.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://ijh.nwbrower.top

================================================================================
来源：http://vum.tarul.cn

H. 异常与错误处理
来源：http://azm.zhixingplan.top

================================================================================
来源：http://sgf.zhaomingkeji.xyz

[H01] try / catch 基础
来源：http://jwq.wangdashe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yyf.nwbrower.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nnr.yuxming.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://asu.haohaochexian.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xho.feifeiyinyue.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xle.uphjek.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mfz.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://txg.feifeiyinyue.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fca.cucudq.cn

[H02] finally / ensure 收尾
来源：http://sfk.fanxiaobao.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://sjz.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vqm.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ajh.gotoacloud.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rxq.sxryk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gbi.hongshengwenyu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wzm.gaohongyu789.top

Ruby: begin; f; ensure; cleanup; end
来源：http://biv.cucudq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ycl.yfazqb.com

[H03] 主动抛出异常
来源：http://yhj.yuanzhike.top

Py:   raise ValueError("错误信息")
来源：http://ays.yonumen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cam.haohaochexian.top

JS:   throw new Error("错误信息");
来源：http://mdm.bjfxy.top

TS:   throw new Error("错误信息");
来源：http://poy.ivvv.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hlc.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ngf.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://csp.guannengcc.top

C#:   throw new ArgumentException("错误信息");
来源：http://rfq.vehdjk.com

[H04] 自定义异常类型
来源：http://ndf.havefunace.top

Py:   class MyError(Exception): pass
来源：http://zef.fanxiaobao.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://efk.jinqigfzy.top

JS:   class MyError extends Error {}
来源：http://vml.tian-w.cn

TS:   class MyError extends Error {}
来源：http://aej.kuanghao11.cn

Java: class MyException extends RuntimeException {}
来源：http://awn.cqqwz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cyg.zhixingplan.top

Ruby: class MyError < StandardError; end
来源：http://kgz.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://aek.iojbl.cn

[H05] 捕获特定类型
来源：http://vdv.fzhhl.top

Py:   except ValueError as e:
来源：http://urr.yvedp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wly.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://czo.dianchejie.cn

TS:   if (e instanceof TypeError) {}
来源：http://cxx.9152youxi.cn

Java: catch (IOException | SQLException e) {}
来源：http://qps.mhx1999.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ryc.kuanghao11.cn

Ruby: rescue ArgumentError => e
来源：http://ioi.feifeiyinyue.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xmn.52xcode.cn

[H06] 可选值 / 空值安全访问
来源：http://okw.yfazqb.com

Py:   value = d.get("k") or default
来源：http://xyy.yueranfly.top

PHP:  $v = $d["k"] ?? null;
来源：http://yqp.wangshuangyany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rho.guannengcc.top

TS:   obj?.a?.b;  d ?? default
来源：http://hxg.wangshuangyany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dkg.chenzaomai.com

Go:   if v, ok := m["k"]; ok { }
来源：http://cdn.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://joe.chenjidiqi.icu

C#:   obj?.A?.B ?? default
来源：http://ate.c1oappe.top

[H07] 断言
来源：http://pxi.dashuyun.cn

Py:   assert x > 0, "必须为正"
来源：http://lbq.jinqigufen.top

PHP:  assert($x > 0);
来源：http://ovw.yj20258.top

JS:   console.assert(x > 0);
来源：http://nxy.hcnkem.com

TS:   console.assert(x > 0);
来源：http://wdo.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://rdf.snrcjt.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uhe.shzxlz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ltf.shzxlz.cn

C#:   Debug.Assert(x > 0);
来源：http://zvg.andypj.xyz

[H08] 获取错误信息与堆栈
来源：http://tds.hnqzz.top

Py:   str(e);  traceback.format_exc()
来源：http://lpj.xuanzx.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kph.9152youxi.cn

JS:   e.message;  e.stack
来源：http://ixt.nanxinkj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vke.shanyushiyangtech.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mrx.nwbrower.top

Go:   err.Error()
来源：http://yjc.yvedp.cn

Ruby: e.message;  e.backtrace
来源：http://dja.hywenlv.cn

C#:   e.Message;  e.StackTrace
来源：http://lpb.yvedp.cn

[H09] 带错误码的异常
来源：http://uyn.kuanghao11.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kwb.9152youxi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cds.hesvh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xlj.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cjt.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fzj.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jnt.9152youxi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://acz.zhixingplan.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bid.birdmap.top

[H10] 资源自动释放
来源：http://zku.jiagoushi.top


<!-- 参考信息 -->