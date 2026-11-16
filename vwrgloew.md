代发 wailian999

C#:   File.Exists("a.txt")
来源：http://bhu.zdqjudy.top

[F06] 删除文件
来源：http://sld.fengsongda.top

Py:   os.remove("a.txt")
来源：http://pvm.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://hqo.hesvh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pjg.c1oappe.top

TS:   fs.unlinkSync("a.txt")
来源：http://ugi.hcnkem.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ndf.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://dds.pycfn.com

Ruby: File.delete("a.txt")
来源：http://qgk.guowangkeji.top

C#:   File.Delete("a.txt");
来源：http://xcb.feifeiyinyue.top

[F07] 创建目录（含多级）
来源：http://dtn.haohaochexian.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tgd.havefunace.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ygb.cdnleiting.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sez.yongpay.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hab.cdnleiting.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bmw.9152youxi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yfd.zhoulong.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dxa.chenzaomai.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iip.sweek.top

[F08] 遍历目录
来源：http://svj.cdnleiting.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qby.fanxiaobao.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://val.wangdashe.top

JS:   fs.readdirSync("dir")
来源：http://vdx.wangshuangyany.cn

TS:   fs.readdirSync("dir")
来源：http://xkf.xingfuxueyuan.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gxj.jianghu66.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cgy.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://hkd.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://oto.gotoacloud.top

[F09] 获取文件大小
来源：http://lve.yueranfly.top

Py:   os.path.getsize("a.txt")
来源：http://vuv.zhongyouzk.top

PHP:  filesize("a.txt");
来源：http://nxf.epnwcf.com

JS:   fs.statSync("a.txt").size
来源：http://bof.svipenyu.cn

TS:   fs.statSync("a.txt").size
来源：http://hjw.vehdjk.com

Java: Files.size(Path.of("a.txt"))
来源：http://kdm.sufxvd.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jmk.316326.xyz

Ruby: File.size("a.txt")
来源：http://uku.birdmap.top

C#:   new FileInfo("a.txt").Length
来源：http://neu.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://wcb.smart0.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wdc.ydzc1.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lbq.fzhhl.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gwe.aibaodan.cn

TS:   path.extname("a.txt")
来源：http://ozh.yueranfly.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ubf.tarul.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wxw.sjlbkw.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mij.shanyushiyangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://igz.yanxiufei.cn

[F11] 复制与移动文件
来源：http://jad.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jlu.ydjk.org.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://snq.ctjpmb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iii.tarul.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hnz.uphjek.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xbe.hnqzz.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qoz.bjfxy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ryo.ydjk.org.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xlf.nanxinkj.top

[F12] CSV 读写
来源：http://kcq.aizwys.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gph.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fnc.316326.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dqz.yvedp.cn

TS:   // 同上
来源：http://inu.hongshengwenyu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://awm.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oif.hfpthk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rrz.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://vrt.gzhubu.top

================================================================================
来源：http://oeb.ppjwa.cn

G. 面向对象
来源：http://lwz.ctjpmb.com

================================================================================
来源：http://evl.ivvv.top

[G01] 定义类
来源：http://ydc.redwolf501.top

Py:   class User: pass
来源：http://les.hcnkem.com

PHP:  class User {}
来源：http://tyl.jinyuanbaomall.cn

JS:   class User {}
来源：http://ncc.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://jxq.zhixingplan.top

Java: class User {}
来源：http://ojp.jinqigufen.top

Go:   type User struct { Name string }
来源：http://ymm.vehdjk.com

Ruby: class User; end
来源：http://xjj.smart0.xyz

C#:   class User {}
来源：http://xum.shzxlz.cn

[G02] 构造函数
来源：http://pof.zycfv.cn

Py:   def __init__(self, name): self.name = name
来源：http://plu.zhixingplan.top

PHP:  public function __construct(public string $name) {}
来源：http://vfo.ydzc1.top

JS:   constructor(name) { this.name = name; }
来源：http://jai.xuanzx.com

TS:   constructor(public name: string) {}
来源：http://zau.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://kjs.ywan-chungtsiang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zgg.jyoumei.cn

Ruby: def initialize(name); @name = name; end
来源：http://fct.wangdashe.top

C#:   public User(string name) { Name = name; }
来源：http://lra.sysykeji.top

[G03] 实例属性
来源：http://hnt.shuidangran.top

Py:   self.name = "x"
来源：http://rcj.yvedp.cn

PHP:  public string $name = "x";
来源：http://bna.pengpengdd.cyou

JS:   this.name = "x";
来源：http://zsm.kuanghao11.cn

TS:   name: string = "x";
来源：http://kaj.guannengcc.top

Java: private String name;
来源：http://dal.bbcook.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hzd.ywan-chungtsiang.top

Ruby: @name = "x"
来源：http://amv.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://wuv.hysaishi.cn

[G04] 定义方法
来源：http://tna.chenzaomai.com

Py:   def greet(self): return self.name
来源：http://ljb.shuidangran.top

PHP:  public function greet(): string { return $this->name; }
来源：http://djm.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://lek.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://msg.guannengcc.top

Java: String greet() { return name; }
来源：http://omq.shuidangran.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://otl.316326.xyz

Ruby: def greet; @name; end
来源：http://bxc.xinyue.icu

C#:   public string Greet() => Name;
来源：http://auc.yuxming.cn

[G05] 继承
来源：http://qqw.smart0.xyz

Py:   class Admin(User): pass
来源：http://axg.chenlongwang.top

PHP:  class Admin extends User {}
来源：http://ygi.gotoacloud.top

JS:   class Admin extends User {}
来源：http://mwb.ydzc1.top

TS:   class Admin extends User {}
来源：http://jxr.birdmap.top

Java: class Admin extends User {}
来源：http://rvi.jyoumei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qhf.0kj1m.cn

Ruby: class Admin < User; end
来源：http://wnc.jlsjyb.cn

C#:   class Admin : User {}
来源：http://qmu.yj20258.top

[G06] 重写方法
来源：http://zjz.ydzc1.top

Py:   def greet(self): return "admin"
来源：http://ehp.ydzc1.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ctq.ivvv.top

JS:   greet() { return "admin"; }
来源：http://xni.nanxuanxn.top

TS:   greet(): string { return "admin"; }
来源：http://qby.guannengcc.top

Java: @Override String greet() { return "admin"; }
来源：http://yxy.yfazqb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bti.nwbrower.top

Ruby: def greet; "admin"; end
来源：http://nwe.ydjk.org.cn

C#:   public override string Greet() => "admin";
来源：http://mnb.sweek.top

[G07] 调用父类方法
来源：http://xmp.yuanzhike.top

Py:   super().greet()
来源：http://wcr.iojbl.cn

PHP:  parent::greet();
来源：http://xyd.aibaodan.cn

JS:   super.greet();
来源：http://byu.hfpthk.cn

TS:   super.greet();
来源：http://rjj.cheryme.top

Java: super.greet();
来源：http://oby.zdqjudy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bwm.zhoulong.xyz

Ruby: super
来源：http://vmq.kuanghao11.cn

C#:   base.Greet();
来源：http://yzk.ppjwa.cn

[G08] 静态方法与属性
来源：http://rsi.yfazqb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xfx.ywan-chungtsiang.top

PHP:  public static function f() {}
来源：http://qei.daxiang520.top

JS:   static f() {}
来源：http://thp.shzxlz.cn

TS:   static f(): void {}
来源：http://onx.jinqigufen.top

Java: static void f() {}
来源：http://uxl.shanyushiyangtech.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ibz.nwbrower.top

Ruby: def self.f; end
来源：http://jwe.zdbjq.cn

C#:   public static void F() {}
来源：http://fxv.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://vta.fehbvm.com

Py:   from abc import ABC, abstractmethod
来源：http://ctb.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://skd.ehwqpu.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://qzq.chenjidiqi.icu

TS:   interface Shape { area(): number; }
来源：http://dwu.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://zvs.yfazqb.com

Go:   type Shape interface { Area() float64 }
来源：http://vwz.fzhhl.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pvp.ctjpmb.com

C#:   interface IShape { double Area(); }
来源：http://mzj.kuanghao11.cn

[G10] 访问控制
来源：http://iwc.sufxvd.cn

Py:   约定 _protected / __private（不强制）
来源：http://wcs.ydzc1.top

PHP:  public / protected / private
来源：http://qlu.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://gri.gotoacloud.top

TS:   public / protected / private
来源：http://kfe.svipenyu.cn

Java: public / protected / private / 默认包级
来源：http://egj.ppjwa.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://exh.jinghuilouyu.cn

Ruby: public / protected / private
来源：http://tti.sysykeji.top

C#:   public / protected / private / internal
来源：http://ewc.sufxvd.cn

[G11] getter / setter
来源：http://iiw.kuanghao11.cn

Py:   @property 与 @x.setter
来源：http://tuk.9152youxi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nxx.andypj.xyz

JS:   get name() { return this._name; }
来源：http://oqb.tian-w.cn

TS:   get name(): string { return this._name; }
来源：http://fgf.tanke756.top

Java: public String getName() { return name; }
来源：http://ytm.hcnkem.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://gcs.bjfxy.top

Ruby: attr_accessor :name
来源：http://crh.ydjk.org.cn

C#:   public string Name { get; set; }
来源：http://ulw.shanyushiyangkeji.top

[G12] 对象转字符串
来源：http://hdm.aizwys.cn

Py:   def __str__(self): return self.name
来源：http://qxz.jinqigfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bgz.birdmap.top

JS:   toString() { return this.name; }
来源：http://tgr.dashuyun.cn

TS:   toString(): string { return this.name; }
来源：http://gbm.wangdashe.top

Java: @Override public String toString() { return name; }
来源：http://wjx.tarul.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wox.gaohongyu789.top

Ruby: def to_s; @name; end
来源：http://zzx.fengsongda.top

C#:   public override string ToString() => Name;
来源：http://bgr.epnwcf.com

[G13] 判断对象类型
来源：http://qhd.yonumen.top

Py:   isinstance(u, User)
来源：http://jgm.svipenyu.cn

PHP:  $u instanceof User
来源：http://zmp.bjfxy.top

JS:   u instanceof User
来源：http://lug.ybcxt.top

TS:   u instanceof User
来源：http://xxz.yangfankeji.com

Java: u instanceof User
来源：http://axy.epnwcf.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://ssf.guowangkeji.top

Ruby: u.is_a?(User)
来源：http://apu.fengsongda.top

C#:   u is User
来源：http://vky.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://vtd.cqqwz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gxh.hfpthk.cn

PHP:  // 用 readonly 属性模拟
来源：http://ppj.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://wco.ivvv.top

TS:   type User = { name: string; age: number };
来源：http://bie.gzhubu.top

Java: record User(String name, int age) {}
来源：http://cqn.daria6918.cn

Go:   type User struct { Name string; Age int }
来源：http://asm.guannengcc.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fbo.hfpthk.cn

C#:   record User(string Name, int Age);
来源：http://njl.jinqigufen.top

[G15] 枚举
来源：http://gql.hesvh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aoo.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ryp.zycfv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xpk.havefunace.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ahy.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://nrm.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xbl.tian-w.cn

Ruby: Color = %i[red green].freeze
来源：http://jho.wangdashe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xmq.daxiang520.top

[G16] 对象转数组 / 字典
来源：http://qdf.chenjidiqi.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jtf.pycfn.com

PHP:  get_object_vars($obj);
来源：http://vmd.jqgfzy.top

JS:   Object.entries(obj)
来源：http://qik.shanyushiyangkeji.top

TS:   Object.entries(obj)
来源：http://buy.jinqigfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pqw.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ejf.ybcxt.top

Ruby: obj.instance_variables
来源：http://wol.vehdjk.com

C#:   // 用反射或 System.Text.Json
来源：http://ikz.ydzc1.top

================================================================================
来源：http://lfi.jqgfzy.top

H. 异常与错误处理
来源：http://ivb.ivvv.top

================================================================================
来源：http://ejd.jinyuanbaomall.cn

[H01] try / catch 基础
来源：http://dem.zhijiandao.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dmk.tanke756.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wys.gzhubu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rvh.shanyushiyangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pjf.cqqwz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dww.gzhubu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ogf.gogol.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lrv.xuetiantiany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://akv.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://ach.dashuyun.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ojo.jqgufenzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cwq.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rgk.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qjd.zhaomingkeji.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://xqz.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nwq.sweek.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zfo.meibo888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dzp.wangdashe.top

[H03] 主动抛出异常
来源：http://mzf.hcnkem.com

Py:   raise ValueError("错误信息")
来源：http://nur.hfpthk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kfi.cashguo.top

JS:   throw new Error("错误信息");
来源：http://qlb.cqqwz.cn

TS:   throw new Error("错误信息");
来源：http://tlc.cqqwz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ifn.aibaodan.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rpx.zdbjq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ruz.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://epx.hysaishi.cn

[H04] 自定义异常类型
来源：http://vwx.fehbvm.com

Py:   class MyError(Exception): pass
来源：http://pdx.shanyushiyangtech.top

PHP:  class MyError extends RuntimeException {}
来源：http://mkf.xinyue.icu

JS:   class MyError extends Error {}
来源：http://lag.52xcode.cn

TS:   class MyError extends Error {}
来源：http://szx.jinqigfzy.top

Java: class MyException extends RuntimeException {}
来源：http://zmy.nwbrower.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cxb.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://jfx.xuanzx.com

C#:   class MyException : Exception {}
来源：http://vwe.nwbrower.top

[H05] 捕获特定类型
来源：http://xdt.chenzaomai.com

Py:   except ValueError as e:
来源：http://vax.wangshuangyany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xxo.sjlbkw.cn

JS:   if (e instanceof TypeError) {}
来源：http://spl.yanxiufei.cn

TS:   if (e instanceof TypeError) {}
来源：http://ffp.jqgufenzy.top

Java: catch (IOException | SQLException e) {}
来源：http://pls.tianlin.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://adb.quarkkingdee.top

Ruby: rescue ArgumentError => e
来源：http://jwt.hnqzz.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://grr.zhoulong.xyz

[H06] 可选值 / 空值安全访问
来源：http://mti.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://foj.0kj1m.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bzm.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://ioy.ivvv.top

TS:   obj?.a?.b;  d ?? default
来源：http://sfx.yj202588.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xpo.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eaf.zhongyouzk.top

Ruby: d&.dig(:a, :b)
来源：http://bmq.yueranfly.top

C#:   obj?.A?.B ?? default
来源：http://pax.quarkkingdee.top

[H07] 断言
来源：http://pou.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://tor.nwbrower.top

PHP:  assert($x > 0);
来源：http://reg.jinghuilouyu.cn

JS:   console.assert(x > 0);
来源：http://rim.ybcxt.top

TS:   console.assert(x > 0);
来源：http://srg.9152youxi.cn

Java: assert x > 0 : "必须为正";
来源：http://aku.pycfn.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eur.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xvc.wangshuangyany.cn

C#:   Debug.Assert(x > 0);
来源：http://nlf.guowangkeji.top

[H08] 获取错误信息与堆栈
来源：http://zji.zhongyouzk.top

Py:   str(e);  traceback.format_exc()
来源：http://hkq.yangfankeji.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vzc.0kj1m.cn

JS:   e.message;  e.stack
来源：http://kdr.nanxinkj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tlj.jinghuilouyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yvq.hammf.cn

Go:   err.Error()
来源：http://tyc.yueranfly.top

Ruby: e.message;  e.backtrace
来源：http://uvv.zhoulong.xyz

C#:   e.Message;  e.StackTrace
来源：http://goh.bjfxy.top

[H09] 带错误码的异常
来源：http://fmi.tian-w.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cby.xinyue.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://lsq.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://egx.smart0.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://abo.guowangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xns.shuidangran.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sxo.cucudq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vgn.zhaomingkeji.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://vqa.yj20258888.top

[H10] 资源自动释放
来源：http://dxn.fengsongda.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wlv.yanxiufei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tze.shuidangran.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zrg.xuanzx.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://roy.fengsongda.top


<!-- 参考信息 -->