代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eom.yuxming.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gpl.guowangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wbx.chenzaomai.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eqd.jinqigufen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nwb.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ary.fktsv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://teo.ywan-chungtsiang.top

[F08] 遍历目录
来源：http://krm.yangfankeji.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://bwd.zdbjq.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rfa.vqdsnc.cn

JS:   fs.readdirSync("dir")
来源：http://uvr.ybcxt.top

TS:   fs.readdirSync("dir")
来源：http://xit.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ufc.yangfankeji.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://gec.pengpengdd.cyou

Ruby: Dir.children("dir")
来源：http://jwm.52xcode.cn

C#:   Directory.GetFiles("dir")
来源：http://qtb.tian-w.cn

[F09] 获取文件大小
来源：http://knl.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://kro.xziqi.cn

PHP:  filesize("a.txt");
来源：http://asq.uphjek.com

JS:   fs.statSync("a.txt").size
来源：http://mqq.zhongyouzk.top

TS:   fs.statSync("a.txt").size
来源：http://bfx.nanxuanxn.top

Java: Files.size(Path.of("a.txt"))
来源：http://vba.cqqwz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lct.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://sov.fanxiaobao.xyz

C#:   new FileInfo("a.txt").Length
来源：http://hjk.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://hhj.havefunace.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hqj.birdmap.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ueu.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hgo.jlsjyb.cn

TS:   path.extname("a.txt")
来源：http://smh.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qfr.epnwcf.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://did.yj202588.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hef.fengsongda.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ejo.kuanghao11.cn

[F11] 复制与移动文件
来源：http://tem.xziqi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fxf.wangshuangyany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rfm.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://caj.jianghu66.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gne.9152youxi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vkg.pycfn.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ksu.c1oappe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nki.yj20258888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://upz.cdnleiting.top

[F12] CSV 读写
来源：http://kug.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lmu.gzhubu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blx.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dqb.ctjpmb.com

TS:   // 同上
来源：http://hsw.epnwcf.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://irh.smart0.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xxb.sjlbkw.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nrw.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gyk.cdnleiting.top

================================================================================
来源：http://sjt.jyoumei.cn

G. 面向对象
来源：http://ijr.shanyushiyangkeji.top

================================================================================
来源：http://rhq.zhiwuduotai.top

[G01] 定义类
来源：http://tlc.yongpay.top

Py:   class User: pass
来源：http://ziy.yangfankeji.com

PHP:  class User {}
来源：http://iyo.cqqwz.cn

JS:   class User {}
来源：http://dxy.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://byn.9152youxi.cn

Java: class User {}
来源：http://ben.hcnkem.com

Go:   type User struct { Name string }
来源：http://ale.yj20258.top

Ruby: class User; end
来源：http://vgi.aibaodan.cn

C#:   class User {}
来源：http://dhk.haohaochexian.top

[G02] 构造函数
来源：http://exj.hfpthk.cn

Py:   def __init__(self, name): self.name = name
来源：http://gyl.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://mod.hesvh.cn

JS:   constructor(name) { this.name = name; }
来源：http://xvm.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://ghn.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://iet.xuetiantiany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ouy.hfpthk.cn

Ruby: def initialize(name); @name = name; end
来源：http://rzm.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://wtc.svipenyu.cn

[G03] 实例属性
来源：http://tgy.jqgfzy.top

Py:   self.name = "x"
来源：http://ujd.nanxuanxn.top

PHP:  public string $name = "x";
来源：http://gqo.guannengcc.top

JS:   this.name = "x";
来源：http://tqa.cheryme.top

TS:   name: string = "x";
来源：http://zcx.tanke756.top

Java: private String name;
来源：http://tcc.hesvh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jjr.ehwqpu.com

Ruby: @name = "x"
来源：http://txa.52xcode.cn

C#:   public string Name { get; set; } = "x";
来源：http://lui.tianlin.xyz

[G04] 定义方法
来源：http://amp.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://hcb.shangyingyoupin.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nyg.ybcxt.top

JS:   greet() { return this.name; }
来源：http://yux.yangfankeji.com

TS:   greet(): string { return this.name; }
来源：http://hqw.haohaochexian.top

Java: String greet() { return name; }
来源：http://tyn.yj202588.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pmz.haohaochexian.top

Ruby: def greet; @name; end
来源：http://ric.zhongyouzk.top

C#:   public string Greet() => Name;
来源：http://dwh.pengpengdd.cyou

[G05] 继承
来源：http://kgt.guowangkeji.top

Py:   class Admin(User): pass
来源：http://hvf.dianchejie.cn

PHP:  class Admin extends User {}
来源：http://zms.ppjwa.cn

JS:   class Admin extends User {}
来源：http://hmy.shanyushiyangkeji.top

TS:   class Admin extends User {}
来源：http://cpm.cqqwz.cn

Java: class Admin extends User {}
来源：http://pjs.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jad.nanxuanxn.top

Ruby: class Admin < User; end
来源：http://hyi.316326.xyz

C#:   class Admin : User {}
来源：http://apz.mhx1999.top

[G06] 重写方法
来源：http://ake.ydzc1.top

Py:   def greet(self): return "admin"
来源：http://wxk.zhiwuduotai.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wnf.sxryk.cn

JS:   greet() { return "admin"; }
来源：http://xuj.pycfn.com

TS:   greet(): string { return "admin"; }
来源：http://wrw.shuidangran.top

Java: @Override String greet() { return "admin"; }
来源：http://fvt.0kj1m.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ppk.xingfuxueyuan.xyz

Ruby: def greet; "admin"; end
来源：http://lwp.tarul.cn

C#:   public override string Greet() => "admin";
来源：http://qqy.zhijiandao.cn

[G07] 调用父类方法
来源：http://jdm.sufxvd.cn

Py:   super().greet()
来源：http://btp.ivvv.top

PHP:  parent::greet();
来源：http://iwn.316326.xyz

JS:   super.greet();
来源：http://cdz.nwbrower.top

TS:   super.greet();
来源：http://ybr.yueranfly.top

Java: super.greet();
来源：http://ywj.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gni.iojbl.cn

Ruby: super
来源：http://tqt.hfpthk.cn

C#:   base.Greet();
来源：http://kgu.tian-w.cn

[G08] 静态方法与属性
来源：http://jmt.zhengqikj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wsq.yfazqb.com

PHP:  public static function f() {}
来源：http://dkp.hywenlv.cn

JS:   static f() {}
来源：http://ukw.cheryme.top

TS:   static f(): void {}
来源：http://oyb.0kj1m.cn

Java: static void f() {}
来源：http://vdg.yvedp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wqe.fengsongda.top

Ruby: def self.f; end
来源：http://gvi.uphjek.com

C#:   public static void F() {}
来源：http://woh.nanxinkj.top

[G09] 接口 / 抽象类
来源：http://ufh.chenjidiqi.icu

Py:   from abc import ABC, abstractmethod
来源：http://dmn.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fqm.mhx1999.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ovh.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://zjt.vehdjk.com

Java: interface Shape { double area(); }
来源：http://gbj.andypj.xyz

Go:   type Shape interface { Area() float64 }
来源：http://inz.tianlin.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://csl.cucudq.cn

C#:   interface IShape { double Area(); }
来源：http://cme.ybcxt.top

[G10] 访问控制
来源：http://xym.fktsv.cn

Py:   约定 _protected / __private（不强制）
来源：http://ymj.tianlin.xyz

PHP:  public / protected / private
来源：http://avi.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://rmf.fehbvm.com

TS:   public / protected / private
来源：http://xok.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://tna.zhaomingkeji.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://yuf.guowangkeji.top

Ruby: public / protected / private
来源：http://gvl.chenjidiqi.icu

C#:   public / protected / private / internal
来源：http://jqy.hnqzz.top

[G11] getter / setter
来源：http://xdr.hysaishi.cn

Py:   @property 与 @x.setter
来源：http://ayz.yongpay.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jjh.daria6918.cn

JS:   get name() { return this._name; }
来源：http://srh.jqgufenzy.top

TS:   get name(): string { return this._name; }
来源：http://pqm.bbcook.cn

Java: public String getName() { return name; }
来源：http://qbq.zhijiandao.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qbd.zhiwuduotai.top

Ruby: attr_accessor :name
来源：http://zhd.shangyingyoupin.top

C#:   public string Name { get; set; }
来源：http://fri.uphjek.com

[G12] 对象转字符串
来源：http://fdy.cheryme.top

Py:   def __str__(self): return self.name
来源：http://scw.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nap.xziqi.cn

JS:   toString() { return this.name; }
来源：http://vtf.ywan-chungtsiang.top

TS:   toString(): string { return this.name; }
来源：http://wee.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://qxg.tianlin.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://wqy.chenjidiqi.icu

Ruby: def to_s; @name; end
来源：http://wai.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://hmk.c1oappe.top

[G13] 判断对象类型
来源：http://eau.cdnleiting.top

Py:   isinstance(u, User)
来源：http://mmh.zhoulong.xyz

PHP:  $u instanceof User
来源：http://pht.ydjk.org.cn

JS:   u instanceof User
来源：http://dmn.fktsv.cn

TS:   u instanceof User
来源：http://jdr.yvedp.cn

Java: u instanceof User
来源：http://poi.sxryk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://udj.aizwys.cn

Ruby: u.is_a?(User)
来源：http://hed.yuanzhike.top

C#:   u is User
来源：http://frl.chenjidiqi.icu

[G14] 数据类 / record
来源：http://jaf.tian-w.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nem.9152youxi.cn

PHP:  // 用 readonly 属性模拟
来源：http://tfd.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://czo.jinqigufen.top

TS:   type User = { name: string; age: number };
来源：http://ait.snrcjt.cn

Java: record User(String name, int age) {}
来源：http://qwv.yj202588.top

Go:   type User struct { Name string; Age int }
来源：http://iqg.daria6918.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mpg.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://kcb.vehdjk.com

[G15] 枚举
来源：http://ibl.yonumen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ynh.yanxiufei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ggw.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://obi.haohaochexian.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kgm.quarkkingdee.top

Java: enum Color { RED, GREEN }
来源：http://fod.chenlongwang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ftd.52xcode.cn

Ruby: Color = %i[red green].freeze
来源：http://muj.bbcook.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hmq.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://dsd.xylfe.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gbc.bjfxy.top

PHP:  get_object_vars($obj);
来源：http://crr.nwbrower.top

JS:   Object.entries(obj)
来源：http://bey.sufxvd.cn

TS:   Object.entries(obj)
来源：http://itk.zdqjudy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://odx.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://pgi.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://hzf.ppjwa.cn

C#:   // 用反射或 System.Text.Json
来源：http://wze.jqgufenzy.top

================================================================================
来源：http://tww.yj20258.top

H. 异常与错误处理
来源：http://fxc.redwolf501.top

================================================================================
来源：http://hwn.shanyushiyangtech.top

[H01] try / catch 基础
来源：http://dpx.ydjk.org.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://omf.hcnkem.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aru.chenlongwang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vhz.guannengcc.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dmo.sxryk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mfs.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ujn.52xcode.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hbu.gogol.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gex.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://bar.zdqjudy.top

Py:   try: f()⏎finally: cleanup()
来源：http://kyl.haohaochexian.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uwa.c1oappe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jlv.nwbrower.top

TS:   try { f(); } finally { cleanup(); }
来源：http://uyr.jlsjyb.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fzn.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ykc.sufxvd.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ega.jiagoushi.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ehy.gaohongyu789.top

[H03] 主动抛出异常
来源：http://ebj.jinqigfzy.top

Py:   raise ValueError("错误信息")
来源：http://vrs.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bfv.vqdsnc.cn

JS:   throw new Error("错误信息");
来源：http://bhv.sweek.top

TS:   throw new Error("错误信息");
来源：http://ope.ehwqpu.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://lfd.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vem.yongpay.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cwc.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://bzx.shanyushiyangtech.top

[H04] 自定义异常类型
来源：http://fhe.ppjwa.cn

Py:   class MyError(Exception): pass
来源：http://cka.zhoulong.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://usl.gotoacloud.top

JS:   class MyError extends Error {}
来源：http://bzx.snrcjt.cn

TS:   class MyError extends Error {}
来源：http://wrm.yuanzhike.top

Java: class MyException extends RuntimeException {}
来源：http://gme.chenjidiqi.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cft.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://nhf.svipenyu.cn

C#:   class MyException : Exception {}
来源：http://yff.9152youxi.cn

[H05] 捕获特定类型
来源：http://rvl.ppjwa.cn

Py:   except ValueError as e:
来源：http://emh.jinyuanbaomall.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://crj.havefunace.top

JS:   if (e instanceof TypeError) {}
来源：http://xtl.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://xcs.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://hwb.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://juh.svipenyu.cn

Ruby: rescue ArgumentError => e
来源：http://myf.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lov.cqqwz.cn

[H06] 可选值 / 空值安全访问
来源：http://voo.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://hvy.cheryme.top

PHP:  $v = $d["k"] ?? null;
来源：http://iie.fzhhl.top

JS:   obj?.a?.b;  d ?? default
来源：http://pet.jinqigufen.top

TS:   obj?.a?.b;  d ?? default
来源：http://ivs.ywan-chungtsiang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ctn.hesvh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dvt.nanxuanxn.top

Ruby: d&.dig(:a, :b)
来源：http://oto.ydzc1.top

C#:   obj?.A?.B ?? default
来源：http://ney.yueranfly.top

[H07] 断言
来源：http://dse.hnxiangtu.top

Py:   assert x > 0, "必须为正"
来源：http://rdw.yuxming.cn

PHP:  assert($x > 0);
来源：http://tks.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://xoh.yuxming.cn

TS:   console.assert(x > 0);
来源：http://jps.zhoulong.xyz

Java: assert x > 0 : "必须为正";
来源：http://sdg.pengpengdd.cyou

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cfh.epnwcf.com

Ruby: raise "必须为正" unless x > 0
来源：http://rxp.jinyuanbaomall.cn

C#:   Debug.Assert(x > 0);
来源：http://ymo.ywan-chungtsiang.top

[H08] 获取错误信息与堆栈
来源：http://eez.yvedp.cn

Py:   str(e);  traceback.format_exc()
来源：http://yss.yj202588.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://okx.wangdashe.top

JS:   e.message;  e.stack
来源：http://vxi.xinyue.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://sem.tian-w.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xsn.jqgfzy.top

Go:   err.Error()
来源：http://gsb.zhengqikj.top

Ruby: e.message;  e.backtrace
来源：http://yip.nanxuanxn.top

C#:   e.Message;  e.StackTrace
来源：http://mil.shanyushiyangkeji.top

[H09] 带错误码的异常
来源：http://wgh.hcnkem.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fgj.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wix.zdqjudy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hsj.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yun.svipenyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xtj.zycfv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qbp.zhiwuduotai.top

Ruby: raise MyError.new("fail", 500)
来源：http://gnh.jinyuanbaomall.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oyk.tarul.cn

[H10] 资源自动释放
来源：http://mlk.hesvh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ivu.jqgufenzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://odd.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jih.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ofv.smart0.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yim.xziqi.cn

Go:   defer f.Close()
来源：http://jkv.c1oappe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zjx.shzxlz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vdc.jinqigfzy.top

================================================================================
来源：http://faj.zhengqikj.top

I. 正则表达式
来源：http://iat.xylfe.cn

================================================================================
来源：http://cau.nanxinkj.top

[I01] 判断是否匹配
来源：http://oht.yj20258.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bsx.yonumen.top

PHP:  preg_match('/\d+/', $s);
来源：http://liy.epnwcf.com

JS:   /\d+/.test(s)
来源：http://wco.yj20258888.top

TS:   /\d+/.test(s)
来源：http://wxm.sufxvd.cn


<!-- 参考信息 -->