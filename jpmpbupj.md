代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bsc.jinyuanbaomall.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xxz.bbcook.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pkb.vqdsnc.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pnp.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lpu.xylfe.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fxn.cdnleiting.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hwf.fzhhl.top

[F08] 遍历目录
来源：http://zeg.iojbl.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ngd.ybcxt.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ywq.cheryme.top

JS:   fs.readdirSync("dir")
来源：http://qoq.aibaodan.cn

TS:   fs.readdirSync("dir")
来源：http://omr.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qnr.ydjk.org.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://utc.hywenlv.cn

Ruby: Dir.children("dir")
来源：http://hsi.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://xzv.cheryme.top

[F09] 获取文件大小
来源：http://bka.jiagoushi.top

Py:   os.path.getsize("a.txt")
来源：http://wqe.ivvv.top

PHP:  filesize("a.txt");
来源：http://yeh.zhiwuduotai.top

JS:   fs.statSync("a.txt").size
来源：http://tca.shzxlz.cn

TS:   fs.statSync("a.txt").size
来源：http://utb.tarul.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mms.guannengcc.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kiy.hesvh.cn

Ruby: File.size("a.txt")
来源：http://lob.gzhubu.top

C#:   new FileInfo("a.txt").Length
来源：http://vio.zhiwuduotai.top

[F10] 取文件扩展名 / 文件名
来源：http://skg.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://huw.sufxvd.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rfi.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zoj.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://yti.redwolf501.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ntx.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hzo.kuanghao11.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cgs.xylfe.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gzk.zhijiandao.cn

[F11] 复制与移动文件
来源：http://ffy.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tbj.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sjd.sxryk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cjl.52xcode.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dyr.wangshuangyany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kjj.cdnleiting.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uib.yangfankeji.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hev.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gce.daxiang520.top

[F12] CSV 读写
来源：http://slb.zhaomingkeji.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ceu.chenlongwang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nls.zhengqikj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tit.zhijiandao.cn

TS:   // 同上
来源：http://lnm.shanyushiyangtech.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bii.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://obh.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xom.xylfe.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uwg.daria6918.cn

================================================================================
来源：http://izo.wangdashe.top

G. 面向对象
来源：http://bmx.chenlongwang.top

================================================================================
来源：http://ywa.fanxiaobao.xyz

[G01] 定义类
来源：http://tsr.jinghuilouyu.cn

Py:   class User: pass
来源：http://tha.zhongyouzk.top

PHP:  class User {}
来源：http://ofx.vqdsnc.cn

JS:   class User {}
来源：http://dsy.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://mov.jiagoushi.top

Java: class User {}
来源：http://ncn.shangyingyoupin.top

Go:   type User struct { Name string }
来源：http://nlu.shanyushiyangtech.top

Ruby: class User; end
来源：http://kuw.0kj1m.cn

C#:   class User {}
来源：http://pze.316326.xyz

[G02] 构造函数
来源：http://yfs.yanxiufei.cn

Py:   def __init__(self, name): self.name = name
来源：http://izg.fzhhl.top

PHP:  public function __construct(public string $name) {}
来源：http://bcv.andypj.xyz

JS:   constructor(name) { this.name = name; }
来源：http://mrt.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://ynw.shangyingyoupin.top

Java: User(String name) { this.name = name; }
来源：http://dux.gogol.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bda.bjfxy.top

Ruby: def initialize(name); @name = name; end
来源：http://quk.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://syo.epnwcf.com

[G03] 实例属性
来源：http://qbi.hywenlv.cn

Py:   self.name = "x"
来源：http://zib.yvedp.cn

PHP:  public string $name = "x";
来源：http://aze.chenjidiqi.icu

JS:   this.name = "x";
来源：http://ydq.mhx1999.top

TS:   name: string = "x";
来源：http://uab.zdqjudy.top

Java: private String name;
来源：http://fin.jinqigufen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bab.xuanzx.com

Ruby: @name = "x"
来源：http://vzd.chenlongwang.top

C#:   public string Name { get; set; } = "x";
来源：http://odn.aizwys.cn

[G04] 定义方法
来源：http://ljd.hnqzz.top

Py:   def greet(self): return self.name
来源：http://vhn.dianchejie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://poi.fanxiaobao.xyz

JS:   greet() { return this.name; }
来源：http://onz.hcnkem.com

TS:   greet(): string { return this.name; }
来源：http://cbi.ywan-chungtsiang.top

Java: String greet() { return name; }
来源：http://iyv.ydjk.org.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bcj.yfazqb.com

Ruby: def greet; @name; end
来源：http://dvc.zhoulong.xyz

C#:   public string Greet() => Name;
来源：http://nzg.quarkkingdee.top

[G05] 继承
来源：http://qqe.ivvv.top

Py:   class Admin(User): pass
来源：http://vau.daria6918.cn

PHP:  class Admin extends User {}
来源：http://wfv.aizwys.cn

JS:   class Admin extends User {}
来源：http://xae.fktsv.cn

TS:   class Admin extends User {}
来源：http://ghj.jyoumei.cn

Java: class Admin extends User {}
来源：http://oev.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tfn.cucudq.cn

Ruby: class Admin < User; end
来源：http://hjm.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://qgs.kuanghao11.cn

[G06] 重写方法
来源：http://vcg.yonumen.top

Py:   def greet(self): return "admin"
来源：http://lnv.xziqi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mjv.sxryk.cn

JS:   greet() { return "admin"; }
来源：http://vjh.vqdsnc.cn

TS:   greet(): string { return "admin"; }
来源：http://mjl.0kj1m.cn

Java: @Override String greet() { return "admin"; }
来源：http://jee.tanke756.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ion.xylfe.cn

Ruby: def greet; "admin"; end
来源：http://sdr.xuetiantiany.cn

C#:   public override string Greet() => "admin";
来源：http://hrn.aibaodan.cn

[G07] 调用父类方法
来源：http://yur.zhaomingkeji.xyz

Py:   super().greet()
来源：http://rva.xuanzx.com

PHP:  parent::greet();
来源：http://vva.daxiang520.top

JS:   super.greet();
来源：http://wpy.tian-w.cn

TS:   super.greet();
来源：http://amr.uphjek.com

Java: super.greet();
来源：http://yot.zhijiandao.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uod.wangdashe.top

Ruby: super
来源：http://ibc.fanxiaobao.xyz

C#:   base.Greet();
来源：http://smr.316326.xyz

[G08] 静态方法与属性
来源：http://sqh.jianghu66.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://syz.tanke756.top

PHP:  public static function f() {}
来源：http://jxp.yuxming.cn

JS:   static f() {}
来源：http://cll.zdqjudy.top

TS:   static f(): void {}
来源：http://uyn.yuxming.cn

Java: static void f() {}
来源：http://dmj.jqgufenzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hkw.shangyingyoupin.top

Ruby: def self.f; end
来源：http://oeq.andypj.xyz

C#:   public static void F() {}
来源：http://tuc.yuxming.cn

[G09] 接口 / 抽象类
来源：http://atm.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://gnx.andypj.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://erv.aizwys.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rcb.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://jcn.jlsjyb.cn

Java: interface Shape { double area(); }
来源：http://rpq.nanxinkj.top

Go:   type Shape interface { Area() float64 }
来源：http://wpt.fktsv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kxu.chenjidiqi.icu

C#:   interface IShape { double Area(); }
来源：http://qex.yfazqb.com

[G10] 访问控制
来源：http://url.sufxvd.cn

Py:   约定 _protected / __private（不强制）
来源：http://rac.jlsjyb.cn

PHP:  public / protected / private
来源：http://zvt.aibaodan.cn

JS:   #private 字段；其余公开
来源：http://tva.chenlongwang.top

TS:   public / protected / private
来源：http://qvs.aibaodan.cn

Java: public / protected / private / 默认包级
来源：http://gxp.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fuo.sweek.top

Ruby: public / protected / private
来源：http://yfe.svipenyu.cn

C#:   public / protected / private / internal
来源：http://rxn.mhx1999.top

[G11] getter / setter
来源：http://shq.quarkkingdee.top

Py:   @property 与 @x.setter
来源：http://oni.andypj.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://wcz.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://onq.dianchejie.cn

TS:   get name(): string { return this._name; }
来源：http://hjy.c1oappe.top

Java: public String getName() { return name; }
来源：http://pem.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://yva.hfpthk.cn

Ruby: attr_accessor :name
来源：http://wql.tarul.cn

C#:   public string Name { get; set; }
来源：http://pky.smart0.xyz

[G12] 对象转字符串
来源：http://umi.0kj1m.cn

Py:   def __str__(self): return self.name
来源：http://weo.yfazqb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://rmf.yanxiufei.cn

JS:   toString() { return this.name; }
来源：http://zrg.zhiwuduotai.top

TS:   toString(): string { return this.name; }
来源：http://ayh.zycfv.cn

Java: @Override public String toString() { return name; }
来源：http://igq.sjlbkw.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iol.shuidangran.top

Ruby: def to_s; @name; end
来源：http://sjh.dashuyun.cn

C#:   public override string ToString() => Name;
来源：http://ucf.quarkkingdee.top

[G13] 判断对象类型
来源：http://ssq.birdmap.top

Py:   isinstance(u, User)
来源：http://wey.aizwys.cn

PHP:  $u instanceof User
来源：http://tva.smart0.xyz

JS:   u instanceof User
来源：http://qpj.snrcjt.cn

TS:   u instanceof User
来源：http://klo.jinyuanbaomall.cn

Java: u instanceof User
来源：http://arv.tarul.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jak.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://fpr.guowangkeji.top

C#:   u is User
来源：http://cuh.yangfankeji.com

[G14] 数据类 / record
来源：http://ynq.yj202588.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ids.hesvh.cn

PHP:  // 用 readonly 属性模拟
来源：http://ehy.xinyue.icu

JS:   // 无内置：普通类或对象字面量
来源：http://opt.jinqigfzy.top

TS:   type User = { name: string; age: number };
来源：http://bxi.gotoacloud.top

Java: record User(String name, int age) {}
来源：http://aar.zhongyouzk.top

Go:   type User struct { Name string; Age int }
来源：http://ana.cashguo.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uhi.guannengcc.top

C#:   record User(string Name, int Age);
来源：http://kye.yj20258888.top

[G15] 枚举
来源：http://eol.aibaodan.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bsu.jinghuilouyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bsl.c1oappe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qyp.xylfe.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mhp.quarkkingdee.top

Java: enum Color { RED, GREEN }
来源：http://dqf.daria6918.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rcb.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://rfm.ctjpmb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zac.fzhhl.top

[G16] 对象转数组 / 字典
来源：http://zaa.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jyb.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://wmf.yuxming.cn

JS:   Object.entries(obj)
来源：http://ebi.uphjek.com

TS:   Object.entries(obj)
来源：http://fyz.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lsa.hywenlv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yru.dianchejie.cn

Ruby: obj.instance_variables
来源：http://rkq.yueranfly.top

C#:   // 用反射或 System.Text.Json
来源：http://fko.zdbjq.cn

================================================================================
来源：http://cqv.xylfe.cn

H. 异常与错误处理
来源：http://zal.hammf.cn

================================================================================
来源：http://mgi.gzhubu.top

[H01] try / catch 基础
来源：http://gxo.tanke756.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tse.sysykeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rrn.316326.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://loo.jyoumei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pba.jinyuanbaomall.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kgr.hongshengwenyu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pes.0kj1m.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kmn.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://etl.epnwcf.com

[H02] finally / ensure 收尾
来源：http://uuv.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jne.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uii.xuetiantiany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vkc.jlsjyb.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vrq.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://mhn.jiagoushi.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://yoh.9152youxi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://aza.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nlz.nanxinkj.top

[H03] 主动抛出异常
来源：http://uwx.jqgfzy.top

Py:   raise ValueError("错误信息")
来源：http://mhu.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://inw.sjlbkw.cn

JS:   throw new Error("错误信息");
来源：http://cqt.meibo888.top

TS:   throw new Error("错误信息");
来源：http://ity.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ugc.chenzaomai.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wzt.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hho.9152youxi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pyh.andypj.xyz

[H04] 自定义异常类型
来源：http://prh.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://hgy.ehwqpu.com

PHP:  class MyError extends RuntimeException {}
来源：http://loc.vqdsnc.cn

JS:   class MyError extends Error {}
来源：http://cht.guannengcc.top

TS:   class MyError extends Error {}
来源：http://qpr.jianghu66.top

Java: class MyException extends RuntimeException {}
来源：http://dau.52xcode.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sog.jqgfzy.top

Ruby: class MyError < StandardError; end
来源：http://ayz.fengsongda.top

C#:   class MyException : Exception {}
来源：http://zgz.hongshengwenyu.top

[H05] 捕获特定类型
来源：http://ndi.pengpengdd.cyou

Py:   except ValueError as e:
来源：http://tjo.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://moo.jqgufenzy.top

JS:   if (e instanceof TypeError) {}
来源：http://qgz.gaohongyu789.top

TS:   if (e instanceof TypeError) {}
来源：http://xbr.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://kzx.hfpthk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wmu.kuanghao11.cn

Ruby: rescue ArgumentError => e
来源：http://fpd.c1oappe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sbt.jiagoushi.top

[H06] 可选值 / 空值安全访问
来源：http://ggc.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://gvp.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://dpk.jyoumei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qzd.hammf.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tbc.fanxiaobao.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rpt.cdnleiting.top

Go:   if v, ok := m["k"]; ok { }
来源：http://knz.birdmap.top

Ruby: d&.dig(:a, :b)
来源：http://ezo.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://mgo.cqqwz.cn

[H07] 断言
来源：http://lys.ivvv.top

Py:   assert x > 0, "必须为正"
来源：http://mlk.ppjwa.cn

PHP:  assert($x > 0);
来源：http://amd.zdbjq.cn

JS:   console.assert(x > 0);
来源：http://wae.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://cng.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://fih.cdnleiting.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tnb.hcnkem.com

Ruby: raise "必须为正" unless x > 0
来源：http://ohg.zhengqikj.top

C#:   Debug.Assert(x > 0);
来源：http://bki.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://gvq.daria6918.cn

Py:   str(e);  traceback.format_exc()
来源：http://xxq.tianlin.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xxp.jqgufenzy.top

JS:   e.message;  e.stack
来源：http://ccx.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sch.xylfe.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nmm.vqdsnc.cn

Go:   err.Error()
来源：http://iek.aibaodan.cn

Ruby: e.message;  e.backtrace
来源：http://svi.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://vbt.zhiwuduotai.top

[H09] 带错误码的异常
来源：http://ued.jqgufenzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jmo.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xmy.ctjpmb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gnz.tanke756.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cda.gogol.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sxu.yvedp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bfx.shangyingyoupin.top

Ruby: raise MyError.new("fail", 500)
来源：http://oue.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://rqu.mhx1999.top

[H10] 资源自动释放
来源：http://ifg.feifeiyinyue.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://drf.aizwys.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kfg.pycfn.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://avw.quarkkingdee.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mdh.yuanzhike.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kgk.zycfv.cn

Go:   defer f.Close()
来源：http://gqc.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xsf.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qoc.guowangkeji.top

================================================================================
来源：http://jbc.sjlbkw.cn

I. 正则表达式
来源：http://xjd.yonumen.top

================================================================================
来源：http://cqu.ybcxt.top

[I01] 判断是否匹配
来源：http://qyw.daria6918.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bcz.zhengqikj.top

PHP:  preg_match('/\d+/', $s);
来源：http://qkb.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://hjp.jinghuilouyu.cn

TS:   /\d+/.test(s)
来源：http://dxt.daxiang520.top


<!-- 参考信息 -->