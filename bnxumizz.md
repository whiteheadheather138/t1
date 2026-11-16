代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://mwn.ydzc1.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dzj.yj20258888.top

PHP:  file_exists("a.txt");
来源：http://usz.xziqi.cn

JS:   fs.existsSync("a.txt")
来源：http://ptp.xinyue.icu

TS:   fs.existsSync("a.txt")
来源：http://niy.gogol.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vta.aibaodan.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xpm.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://pxd.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://bwx.ctjpmb.com

[F06] 删除文件
来源：http://uqx.yangfankeji.com

Py:   os.remove("a.txt")
来源：http://lhc.uphjek.com

PHP:  unlink("a.txt");
来源：http://abd.xinyue.icu

JS:   fs.unlinkSync("a.txt")
来源：http://rrm.daxiang520.top

TS:   fs.unlinkSync("a.txt")
来源：http://oqu.ivvv.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tzv.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://oau.quarkkingdee.top

Ruby: File.delete("a.txt")
来源：http://ehk.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://uyz.dianchejie.cn

[F07] 创建目录（含多级）
来源：http://wle.quarkkingdee.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://evv.cucudq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lfg.316326.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vyw.jianghu66.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mpc.ybcxt.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uzc.xingfuxueyuan.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ljj.jinqigfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fwm.xziqi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ojr.tianlin.xyz

[F08] 遍历目录
来源：http://ehz.jyoumei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://euw.hnxiangtu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dtv.yj20258.top

JS:   fs.readdirSync("dir")
来源：http://ecu.andypj.xyz

TS:   fs.readdirSync("dir")
来源：http://ceu.yanxiufei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kty.ydzc1.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dob.0kj1m.cn

Ruby: Dir.children("dir")
来源：http://mlx.fktsv.cn

C#:   Directory.GetFiles("dir")
来源：http://zja.gaohongyu789.top

[F09] 获取文件大小
来源：http://ffj.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://vfg.ivvv.top

PHP:  filesize("a.txt");
来源：http://uei.hnqzz.top

JS:   fs.statSync("a.txt").size
来源：http://yqp.zycfv.cn

TS:   fs.statSync("a.txt").size
来源：http://pfd.hnqzz.top

Java: Files.size(Path.of("a.txt"))
来源：http://hsu.fktsv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qws.fehbvm.com

Ruby: File.size("a.txt")
来源：http://ibt.hcnkem.com

C#:   new FileInfo("a.txt").Length
来源：http://fpm.ppjwa.cn

[F10] 取文件扩展名 / 文件名
来源：http://eed.zhijiandao.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xan.ydzc1.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gci.yfazqb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wdb.hammf.cn

TS:   path.extname("a.txt")
来源：http://fzw.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bhh.ctjpmb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pon.redwolf501.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yzi.sweek.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dvb.epnwcf.com

[F11] 复制与移动文件
来源：http://rgm.yj20258888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://alm.tanke756.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yjs.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://edh.shangyingyoupin.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nrz.havefunace.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xui.316326.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rcy.jinyuanbaomall.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xxw.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lqw.ybcxt.top

[F12] CSV 读写
来源：http://dul.havefunace.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hlh.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jsq.dashuyun.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://njw.vehdjk.com

TS:   // 同上
来源：http://gmg.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://chk.shuidangran.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vhe.sjlbkw.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://meu.ctjpmb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://arp.guannengcc.top

================================================================================
来源：http://ebi.dianchejie.cn

G. 面向对象
来源：http://glh.sysykeji.top

================================================================================
来源：http://bae.cashguo.top

[G01] 定义类
来源：http://irz.bbcook.cn

Py:   class User: pass
来源：http://ajt.vehdjk.com

PHP:  class User {}
来源：http://jgd.yangfankeji.com

JS:   class User {}
来源：http://hox.shanyushiyangtech.top

TS:   class User { name: string = ""; }
来源：http://gjm.dashuyun.cn

Java: class User {}
来源：http://qzo.xinyue.icu

Go:   type User struct { Name string }
来源：http://bjt.pengpengdd.cyou

Ruby: class User; end
来源：http://byq.aizwys.cn

C#:   class User {}
来源：http://ajs.dashuyun.cn

[G02] 构造函数
来源：http://qgz.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://snv.hfpthk.cn

PHP:  public function __construct(public string $name) {}
来源：http://hrs.hammf.cn

JS:   constructor(name) { this.name = name; }
来源：http://svk.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://gdx.zhaomingkeji.xyz

Java: User(String name) { this.name = name; }
来源：http://ood.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hyy.wangshuangyany.cn

Ruby: def initialize(name); @name = name; end
来源：http://ajt.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://zkl.zhoulong.xyz

[G03] 实例属性
来源：http://tkw.tarul.cn

Py:   self.name = "x"
来源：http://qmb.hesvh.cn

PHP:  public string $name = "x";
来源：http://ohb.c1oappe.top

JS:   this.name = "x";
来源：http://zhu.jianghu66.top

TS:   name: string = "x";
来源：http://itd.mhx1999.top

Java: private String name;
来源：http://zuv.andypj.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qdl.hcnkem.com

Ruby: @name = "x"
来源：http://pvd.jyoumei.cn

C#:   public string Name { get; set; } = "x";
来源：http://fti.pengpengdd.cyou

[G04] 定义方法
来源：http://uoa.ppjwa.cn

Py:   def greet(self): return self.name
来源：http://sxn.snrcjt.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ydz.havefunace.top

JS:   greet() { return this.name; }
来源：http://bmj.zhijiandao.cn

TS:   greet(): string { return this.name; }
来源：http://kvr.0kj1m.cn

Java: String greet() { return name; }
来源：http://frn.c1oappe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://png.yonumen.top

Ruby: def greet; @name; end
来源：http://jza.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://hxu.chenzaomai.com

[G05] 继承
来源：http://omp.sysykeji.top

Py:   class Admin(User): pass
来源：http://jkg.fehbvm.com

PHP:  class Admin extends User {}
来源：http://dxi.iojbl.cn

JS:   class Admin extends User {}
来源：http://tbn.jinqigufen.top

TS:   class Admin extends User {}
来源：http://qeg.yfazqb.com

Java: class Admin extends User {}
来源：http://pmp.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ois.chenzaomai.com

Ruby: class Admin < User; end
来源：http://rge.ydzc1.top

C#:   class Admin : User {}
来源：http://bsf.jqgufenzy.top

[G06] 重写方法
来源：http://qua.jqgufenzy.top

Py:   def greet(self): return "admin"
来源：http://stj.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mnn.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://qxl.zhiwuduotai.top

TS:   greet(): string { return "admin"; }
来源：http://ccl.sxryk.cn

Java: @Override String greet() { return "admin"; }
来源：http://dbg.sjlbkw.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mbf.hfpthk.cn

Ruby: def greet; "admin"; end
来源：http://zon.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://dop.hnqzz.top

[G07] 调用父类方法
来源：http://yir.tarul.cn

Py:   super().greet()
来源：http://qvx.jinyuanbaomall.cn

PHP:  parent::greet();
来源：http://fcz.bbcook.cn

JS:   super.greet();
来源：http://xwm.fanxiaobao.xyz

TS:   super.greet();
来源：http://rur.hnxiangtu.top

Java: super.greet();
来源：http://hnj.yfazqb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bme.bjfxy.top

Ruby: super
来源：http://eai.shanyushiyangkeji.top

C#:   base.Greet();
来源：http://acv.iojbl.cn

[G08] 静态方法与属性
来源：http://hyz.sxryk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wuu.kuanghao11.cn

PHP:  public static function f() {}
来源：http://trm.c1oappe.top

JS:   static f() {}
来源：http://obc.xuetiantiany.cn

TS:   static f(): void {}
来源：http://qmx.zhaomingkeji.xyz

Java: static void f() {}
来源：http://hwk.pycfn.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://wdf.0kj1m.cn

Ruby: def self.f; end
来源：http://qcd.xuanzx.com

C#:   public static void F() {}
来源：http://tuz.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://wlf.hysaishi.cn

Py:   from abc import ABC, abstractmethod
来源：http://xdy.ivvv.top

PHP:  interface Shape { public function area(): float; }
来源：http://mmb.316326.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://mfv.fengsongda.top

TS:   interface Shape { area(): number; }
来源：http://rnv.sysykeji.top

Java: interface Shape { double area(); }
来源：http://dkg.yanxiufei.cn

Go:   type Shape interface { Area() float64 }
来源：http://kzg.uphjek.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zth.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://mom.birdmap.top

[G10] 访问控制
来源：http://cbx.zdbjq.cn

Py:   约定 _protected / __private（不强制）
来源：http://fdu.fzhhl.top

PHP:  public / protected / private
来源：http://ukk.shanyushiyangkeji.top

JS:   #private 字段；其余公开
来源：http://qrx.hywenlv.cn

TS:   public / protected / private
来源：http://cmh.jianghu66.top

Java: public / protected / private / 默认包级
来源：http://sbw.fengsongda.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://alk.aizwys.cn

Ruby: public / protected / private
来源：http://hds.cucudq.cn

C#:   public / protected / private / internal
来源：http://nlh.fktsv.cn

[G11] getter / setter
来源：http://txh.yanxiufei.cn

Py:   @property 与 @x.setter
来源：http://bkl.daria6918.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://acs.chenlongwang.top

JS:   get name() { return this._name; }
来源：http://lqt.fanxiaobao.xyz

TS:   get name(): string { return this._name; }
来源：http://maw.tianlin.xyz

Java: public String getName() { return name; }
来源：http://qry.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hzr.52xcode.cn

Ruby: attr_accessor :name
来源：http://zwq.yuanzhike.top

C#:   public string Name { get; set; }
来源：http://vkf.xinyue.icu

[G12] 对象转字符串
来源：http://erm.sufxvd.cn

Py:   def __str__(self): return self.name
来源：http://syt.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vhm.bjfxy.top

JS:   toString() { return this.name; }
来源：http://adv.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://exs.pycfn.com

Java: @Override public String toString() { return name; }
来源：http://mhy.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://mlh.gzhubu.top

Ruby: def to_s; @name; end
来源：http://edt.yj202588.top

C#:   public override string ToString() => Name;
来源：http://kxf.sufxvd.cn

[G13] 判断对象类型
来源：http://tmh.cashguo.top

Py:   isinstance(u, User)
来源：http://qik.xuetiantiany.cn

PHP:  $u instanceof User
来源：http://upo.zhijiandao.cn

JS:   u instanceof User
来源：http://pti.pengpengdd.cyou

TS:   u instanceof User
来源：http://ibh.yongpay.top

Java: u instanceof User
来源：http://inz.andypj.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://lag.sxryk.cn

Ruby: u.is_a?(User)
来源：http://hkb.sxryk.cn

C#:   u is User
来源：http://asq.zhiwuduotai.top

[G14] 数据类 / record
来源：http://jer.bbcook.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bds.wangshuangyany.cn

PHP:  // 用 readonly 属性模拟
来源：http://rmr.dianchejie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rtm.ybcxt.top

TS:   type User = { name: string; age: number };
来源：http://qpd.daria6918.cn

Java: record User(String name, int age) {}
来源：http://kbj.zhengqikj.top

Go:   type User struct { Name string; Age int }
来源：http://vkh.hnqzz.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://abg.nwbrower.top

C#:   record User(string Name, int Age);
来源：http://kwl.ppjwa.cn

[G15] 枚举
来源：http://cmk.xuanzx.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pyz.0kj1m.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ycb.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fqg.zhengqikj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://isb.xinyue.icu

Java: enum Color { RED, GREEN }
来源：http://ccn.feifeiyinyue.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cwh.bbcook.cn

Ruby: Color = %i[red green].freeze
来源：http://ddn.wangdashe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tzy.gotoacloud.top

[G16] 对象转数组 / 字典
来源：http://qrq.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jwd.52xcode.cn

PHP:  get_object_vars($obj);
来源：http://krf.xingfuxueyuan.xyz

JS:   Object.entries(obj)
来源：http://qdm.aizwys.cn

TS:   Object.entries(obj)
来源：http://qom.yanxiufei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ikc.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wlh.sxryk.cn

Ruby: obj.instance_variables
来源：http://hls.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://nzm.dianchejie.cn

================================================================================
来源：http://goq.pycfn.com

H. 异常与错误处理
来源：http://tlp.xylfe.cn

================================================================================
来源：http://url.fengsongda.top

[H01] try / catch 基础
来源：http://zvk.redwolf501.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lkr.ivvv.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bos.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vmv.yj20258.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uzj.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://erh.jinghuilouyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ivc.hnxiangtu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dcq.9152youxi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zsr.yj202588.top

[H02] finally / ensure 收尾
来源：http://owp.hesvh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zzz.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ozg.aibaodan.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pey.jianghu66.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zeq.jyoumei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ulx.ywan-chungtsiang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rnf.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://tlx.zdqjudy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://doz.ydzc1.top

[H03] 主动抛出异常
来源：http://dpu.hnqzz.top

Py:   raise ValueError("错误信息")
来源：http://uwh.epnwcf.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rtu.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://upk.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://sal.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wzz.jianghu66.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iej.yfazqb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://ujx.hammf.cn

C#:   throw new ArgumentException("错误信息");
来源：http://voi.jqgfzy.top

[H04] 自定义异常类型
来源：http://anw.smart0.xyz

Py:   class MyError(Exception): pass
来源：http://vkl.havefunace.top

PHP:  class MyError extends RuntimeException {}
来源：http://rbj.fengsongda.top

JS:   class MyError extends Error {}
来源：http://pat.fktsv.cn

TS:   class MyError extends Error {}
来源：http://oyn.wangshuangyany.cn

Java: class MyException extends RuntimeException {}
来源：http://ivx.tarul.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ycu.pycfn.com

Ruby: class MyError < StandardError; end
来源：http://wqg.daria6918.cn

C#:   class MyException : Exception {}
来源：http://rry.jiagoushi.top

[H05] 捕获特定类型
来源：http://ryb.nanxinkj.top

Py:   except ValueError as e:
来源：http://kel.daria6918.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ysl.havefunace.top

JS:   if (e instanceof TypeError) {}
来源：http://cam.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://bgm.mhx1999.top

Java: catch (IOException | SQLException e) {}
来源：http://pss.zhijiandao.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dfx.hnqzz.top

Ruby: rescue ArgumentError => e
来源：http://qdg.shanyushiyangtech.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mww.pycfn.com

[H06] 可选值 / 空值安全访问
来源：http://nzx.hywenlv.cn

Py:   value = d.get("k") or default
来源：http://snx.52xcode.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dnn.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qdg.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ptq.cucudq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.jinyuanbaomall.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uob.zycfv.cn

Ruby: d&.dig(:a, :b)
来源：http://wab.haohaochexian.top

C#:   obj?.A?.B ?? default
来源：http://xex.ivvv.top

[H07] 断言
来源：http://rwn.smart0.xyz

Py:   assert x > 0, "必须为正"
来源：http://fdi.smart0.xyz

PHP:  assert($x > 0);
来源：http://vqd.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://lqp.shangyingyoupin.top

TS:   console.assert(x > 0);
来源：http://bsb.yonumen.top

Java: assert x > 0 : "必须为正";
来源：http://zgb.cheryme.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mwa.yj202588.top

Ruby: raise "必须为正" unless x > 0
来源：http://umu.smart0.xyz

C#:   Debug.Assert(x > 0);
来源：http://egk.gogol.net.cn

[H08] 获取错误信息与堆栈
来源：http://wpu.cdnleiting.top

Py:   str(e);  traceback.format_exc()
来源：http://yqj.jlsjyb.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wys.meibo888.top

JS:   e.message;  e.stack
来源：http://uct.kuanghao11.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zri.ivvv.top

Java: e.getMessage();  e.printStackTrace()
来源：http://amn.shanyushiyangkeji.top

Go:   err.Error()
来源：http://ynq.yj20258888.top

Ruby: e.message;  e.backtrace
来源：http://qmy.cqqwz.cn

C#:   e.Message;  e.StackTrace
来源：http://vtq.zhongyouzk.top

[H09] 带错误码的异常
来源：http://ajo.hnqzz.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zoy.ehwqpu.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://jel.ybcxt.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vtq.jinqigfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://utr.jinqigfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://guc.aizwys.cn


<!-- 参考信息 -->