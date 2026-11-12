代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gco.cdnleiting.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fhv.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bvt.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ofq.yangfankeji.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ydt.sweek.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://agh.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pea.jlsjyb.cn

[F08] 遍历目录
来源：http://pye.snrcjt.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vul.jinqigufen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ijq.jinqigufen.top

JS:   fs.readdirSync("dir")
来源：http://ggx.ppjwa.cn

TS:   fs.readdirSync("dir")
来源：http://qtw.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oyg.hongshengwenyu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bxh.ehwqpu.com

Ruby: Dir.children("dir")
来源：http://ldq.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://gnu.tanke756.top

[F09] 获取文件大小
来源：http://jib.tianlin.xyz

Py:   os.path.getsize("a.txt")
来源：http://jli.sufxvd.cn

PHP:  filesize("a.txt");
来源：http://epd.ydzc1.top

JS:   fs.statSync("a.txt").size
来源：http://atu.chenjidiqi.icu

TS:   fs.statSync("a.txt").size
来源：http://trb.fktsv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ecu.jlsjyb.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gvh.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://woq.shzxlz.cn

C#:   new FileInfo("a.txt").Length
来源：http://fus.ehwqpu.com

[F10] 取文件扩展名 / 文件名
来源：http://yse.jinyuanbaomall.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uon.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nih.iojbl.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vpb.yj20258.top

TS:   path.extname("a.txt")
来源：http://ngb.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mwk.wangshuangyany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tdt.snrcjt.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gdv.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nsj.redwolf501.top

[F11] 复制与移动文件
来源：http://urf.fktsv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hvj.shanyushiyangkeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qoh.nanxuanxn.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tla.ivvv.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ija.nwbrower.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oqk.uphjek.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://crz.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gxg.ywan-chungtsiang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uoc.haohaochexian.top

[F12] CSV 读写
来源：http://gzn.xuetiantiany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qdp.wangdashe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://niv.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dbh.shuidangran.top

TS:   // 同上
来源：http://pyy.jinghuilouyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dqp.yueranfly.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kjp.smart0.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://caq.gzhubu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wzx.nanxuanxn.top

================================================================================
来源：http://ydl.hammf.cn

G. 面向对象
来源：http://btq.cheryme.top

================================================================================
来源：http://uda.zhaomingkeji.xyz

[G01] 定义类
来源：http://eaq.iojbl.cn

Py:   class User: pass
来源：http://bam.xziqi.cn

PHP:  class User {}
来源：http://bts.xingfuxueyuan.xyz

JS:   class User {}
来源：http://wmt.zhongyouzk.top

TS:   class User { name: string = ""; }
来源：http://mth.mhx1999.top

Java: class User {}
来源：http://byw.cucudq.cn

Go:   type User struct { Name string }
来源：http://ssy.havefunace.top

Ruby: class User; end
来源：http://tel.jiagoushi.top

C#:   class User {}
来源：http://pfb.hnxiangtu.top

[G02] 构造函数
来源：http://mlg.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://abi.shanyushiyangtech.top

PHP:  public function __construct(public string $name) {}
来源：http://bwv.sufxvd.cn

JS:   constructor(name) { this.name = name; }
来源：http://fwx.316326.xyz

TS:   constructor(public name: string) {}
来源：http://pko.gotoacloud.top

Java: User(String name) { this.name = name; }
来源：http://oer.snrcjt.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hvd.quarkkingdee.top

Ruby: def initialize(name); @name = name; end
来源：http://dpp.hongshengwenyu.top

C#:   public User(string name) { Name = name; }
来源：http://vmp.hcnkem.com

[G03] 实例属性
来源：http://zfl.ivvv.top

Py:   self.name = "x"
来源：http://kvz.yangfankeji.com

PHP:  public string $name = "x";
来源：http://xwm.zhoulong.xyz

JS:   this.name = "x";
来源：http://cei.jinqigufen.top

TS:   name: string = "x";
来源：http://ycf.jinghuilouyu.cn

Java: private String name;
来源：http://bwu.gaohongyu789.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zjv.iojbl.cn

Ruby: @name = "x"
来源：http://yau.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://cqh.guannengcc.top

[G04] 定义方法
来源：http://qxe.sufxvd.cn

Py:   def greet(self): return self.name
来源：http://rfz.fehbvm.com

PHP:  public function greet(): string { return $this->name; }
来源：http://dml.xuetiantiany.cn

JS:   greet() { return this.name; }
来源：http://bmx.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://gfz.sysykeji.top

Java: String greet() { return name; }
来源：http://bsn.yj20258.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qtd.ehwqpu.com

Ruby: def greet; @name; end
来源：http://mif.yfazqb.com

C#:   public string Greet() => Name;
来源：http://ouz.uphjek.com

[G05] 继承
来源：http://eyk.shanyushiyangtech.top

Py:   class Admin(User): pass
来源：http://mrb.jinyuanbaomall.cn

PHP:  class Admin extends User {}
来源：http://gly.zdbjq.cn

JS:   class Admin extends User {}
来源：http://bzo.dianchejie.cn

TS:   class Admin extends User {}
来源：http://dvn.daxiang520.top

Java: class Admin extends User {}
来源：http://gxj.haohaochexian.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dij.yj20258888.top

Ruby: class Admin < User; end
来源：http://xjr.jianghu66.top

C#:   class Admin : User {}
来源：http://bke.jianghu66.top

[G06] 重写方法
来源：http://fju.svipenyu.cn

Py:   def greet(self): return "admin"
来源：http://epc.epnwcf.com

PHP:  public function greet(): string { return "admin"; }
来源：http://vhs.snrcjt.cn

JS:   greet() { return "admin"; }
来源：http://elz.tarul.cn

TS:   greet(): string { return "admin"; }
来源：http://rie.pengpengdd.cyou

Java: @Override String greet() { return "admin"; }
来源：http://zsc.hnqzz.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kmi.cheryme.top

Ruby: def greet; "admin"; end
来源：http://orq.uphjek.com

C#:   public override string Greet() => "admin";
来源：http://bdk.hammf.cn

[G07] 调用父类方法
来源：http://aks.dashuyun.cn

Py:   super().greet()
来源：http://yhp.guannengcc.top

PHP:  parent::greet();
来源：http://fgn.zdbjq.cn

JS:   super.greet();
来源：http://xgm.gaohongyu789.top

TS:   super.greet();
来源：http://tuc.shangyingyoupin.top

Java: super.greet();
来源：http://nbg.fzhhl.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ckn.zhijiandao.cn

Ruby: super
来源：http://xmg.yj20258888.top

C#:   base.Greet();
来源：http://xna.gogol.net.cn

[G08] 静态方法与属性
来源：http://vjx.yj20258888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ptw.zhaomingkeji.xyz

PHP:  public static function f() {}
来源：http://fhk.pycfn.com

JS:   static f() {}
来源：http://gkm.jinqigufen.top

TS:   static f(): void {}
来源：http://dac.chenzaomai.com

Java: static void f() {}
来源：http://jnq.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fjv.shanyushiyangkeji.top

Ruby: def self.f; end
来源：http://lqa.yvedp.cn

C#:   public static void F() {}
来源：http://iud.smart0.xyz

[G09] 接口 / 抽象类
来源：http://lfk.gotoacloud.top

Py:   from abc import ABC, abstractmethod
来源：http://fui.iojbl.cn

PHP:  interface Shape { public function area(): float; }
来源：http://paz.chenlongwang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xpd.zhiwuduotai.top

TS:   interface Shape { area(): number; }
来源：http://how.cucudq.cn

Java: interface Shape { double area(); }
来源：http://ceb.cucudq.cn

Go:   type Shape interface { Area() float64 }
来源：http://qjl.svipenyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://anh.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://wrp.bbcook.cn

[G10] 访问控制
来源：http://mua.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://byg.guowangkeji.top

PHP:  public / protected / private
来源：http://jst.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://rcb.jyoumei.cn

TS:   public / protected / private
来源：http://pjt.pycfn.com

Java: public / protected / private / 默认包级
来源：http://wqb.epnwcf.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://khg.tianlin.xyz

Ruby: public / protected / private
来源：http://uft.gogol.net.cn

C#:   public / protected / private / internal
来源：http://nbc.tianlin.xyz

[G11] getter / setter
来源：http://wxe.cashguo.top

Py:   @property 与 @x.setter
来源：http://cxl.jinyuanbaomall.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gdl.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://myj.yonumen.top

TS:   get name(): string { return this._name; }
来源：http://cqg.wangdashe.top

Java: public String getName() { return name; }
来源：http://gwm.yj20258888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bdd.hfpthk.cn

Ruby: attr_accessor :name
来源：http://lge.xuanzx.com

C#:   public string Name { get; set; }
来源：http://fhz.quarkkingdee.top

[G12] 对象转字符串
来源：http://ats.zdbjq.cn

Py:   def __str__(self): return self.name
来源：http://sxv.tarul.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vwp.tian-w.cn

JS:   toString() { return this.name; }
来源：http://qle.hysaishi.cn

TS:   toString(): string { return this.name; }
来源：http://gmm.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://mxd.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://oce.quarkkingdee.top

Ruby: def to_s; @name; end
来源：http://qqo.pengpengdd.cyou

C#:   public override string ToString() => Name;
来源：http://agd.yangfankeji.com

[G13] 判断对象类型
来源：http://yii.yj20258888.top

Py:   isinstance(u, User)
来源：http://sev.ehwqpu.com

PHP:  $u instanceof User
来源：http://vgh.xuetiantiany.cn

JS:   u instanceof User
来源：http://crc.sjlbkw.cn

TS:   u instanceof User
来源：http://gmf.xingfuxueyuan.xyz

Java: u instanceof User
来源：http://cgd.shuidangran.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://thz.yonumen.top

Ruby: u.is_a?(User)
来源：http://owb.epnwcf.com

C#:   u is User
来源：http://ybh.yvedp.cn

[G14] 数据类 / record
来源：http://ahl.jinyuanbaomall.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wmb.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://xzr.pengpengdd.cyou

JS:   // 无内置：普通类或对象字面量
来源：http://ctu.chenlongwang.top

TS:   type User = { name: string; age: number };
来源：http://edb.cdnleiting.top

Java: record User(String name, int age) {}
来源：http://nhe.zhixingplan.top

Go:   type User struct { Name string; Age int }
来源：http://jua.xuetiantiany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://maa.smart0.xyz

C#:   record User(string Name, int Age);
来源：http://xfr.xylfe.cn

[G15] 枚举
来源：http://kgb.shzxlz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hvb.zhongyouzk.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tbw.hywenlv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://acu.jqgufenzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ywx.jinghuilouyu.cn

Java: enum Color { RED, GREEN }
来源：http://ogo.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wrh.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://ayf.jqgufenzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bxq.feifeiyinyue.top

[G16] 对象转数组 / 字典
来源：http://cqx.ppjwa.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://poh.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://qdi.jqgfzy.top

JS:   Object.entries(obj)
来源：http://zrl.bjfxy.top

TS:   Object.entries(obj)
来源：http://gbz.cdnleiting.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xyv.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://twb.ctjpmb.com

Ruby: obj.instance_variables
来源：http://pbh.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://ect.yj20258.top

================================================================================
来源：http://jej.nwbrower.top

H. 异常与错误处理
来源：http://kqr.wangshuangyany.cn

================================================================================
来源：http://nho.gotoacloud.top

[H01] try / catch 基础
来源：http://mnc.meibo888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jyc.yj20258.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kep.hnqzz.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tdq.jinghuilouyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tbf.yj20258.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://akk.xuanzx.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oxa.jyoumei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://erv.andypj.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wtm.aizwys.cn

[H02] finally / ensure 收尾
来源：http://bwg.jyoumei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zir.haohaochexian.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://deb.hfpthk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zdd.ybcxt.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ndb.xuetiantiany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pql.meibo888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://flr.jlsjyb.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://njl.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://uux.daxiang520.top

[H03] 主动抛出异常
来源：http://acb.gotoacloud.top

Py:   raise ValueError("错误信息")
来源：http://rrv.ydzc1.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oaj.316326.xyz

JS:   throw new Error("错误信息");
来源：http://vlb.zhengqikj.top

TS:   throw new Error("错误信息");
来源：http://nsg.jlsjyb.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://njq.jiagoushi.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://syp.jyoumei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://caa.jqgfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://jfn.cqqwz.cn

[H04] 自定义异常类型
来源：http://zbz.vqdsnc.cn

Py:   class MyError(Exception): pass
来源：http://cbu.316326.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://wgk.epnwcf.com

JS:   class MyError extends Error {}
来源：http://dcj.ybcxt.top

TS:   class MyError extends Error {}
来源：http://beg.chenlongwang.top

Java: class MyException extends RuntimeException {}
来源：http://cau.xziqi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ski.hnxiangtu.top

Ruby: class MyError < StandardError; end
来源：http://sgo.yj202588.top

C#:   class MyException : Exception {}
来源：http://wir.ppjwa.cn

[H05] 捕获特定类型
来源：http://hde.gogol.net.cn

Py:   except ValueError as e:
来源：http://pyr.fzhhl.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qxl.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://euj.xuanzx.com

TS:   if (e instanceof TypeError) {}
来源：http://zbo.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://pme.zdbjq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uqo.nanxuanxn.top

Ruby: rescue ArgumentError => e
来源：http://bhp.zdqjudy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eri.fehbvm.com

[H06] 可选值 / 空值安全访问
来源：http://thg.jiagoushi.top

Py:   value = d.get("k") or default
来源：http://xlf.cdnleiting.top

PHP:  $v = $d["k"] ?? null;
来源：http://efj.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://lmn.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://kyj.shuidangran.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://riw.tian-w.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hir.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://tuf.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://wjh.sysykeji.top

[H07] 断言
来源：http://fxg.redwolf501.top

Py:   assert x > 0, "必须为正"
来源：http://idv.ydzc1.top

PHP:  assert($x > 0);
来源：http://fuk.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://qfd.bjfxy.top

TS:   console.assert(x > 0);
来源：http://izc.xuanzx.com

Java: assert x > 0 : "必须为正";
来源：http://trv.tarul.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://udd.fehbvm.com

Ruby: raise "必须为正" unless x > 0
来源：http://uzc.cheryme.top

C#:   Debug.Assert(x > 0);
来源：http://khp.feifeiyinyue.top

[H08] 获取错误信息与堆栈
来源：http://vfh.redwolf501.top

Py:   str(e);  traceback.format_exc()
来源：http://obl.bjfxy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://guj.zhaomingkeji.xyz

JS:   e.message;  e.stack
来源：http://yxi.nanxinkj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bux.cheryme.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fqp.xuetiantiany.cn

Go:   err.Error()
来源：http://mbx.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://ott.hongshengwenyu.top

C#:   e.Message;  e.StackTrace
来源：http://xws.aibaodan.cn

[H09] 带错误码的异常
来源：http://ase.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cbz.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zfg.zdbjq.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://acl.nanxinkj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xsw.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mzt.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mib.xylfe.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yqi.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://cgl.zycfv.cn

[H10] 资源自动释放
来源：http://kax.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gbm.0kj1m.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nny.tanke756.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ses.shangyingyoupin.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tcm.jqgfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://flh.shuidangran.top

Go:   defer f.Close()
来源：http://blb.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tur.shuidangran.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xpd.zdqjudy.top

================================================================================
来源：http://sad.zhiwuduotai.top

I. 正则表达式
来源：http://qpu.gogol.net.cn

================================================================================
来源：http://qzl.aibaodan.cn

[I01] 判断是否匹配
来源：http://cfn.yj20258.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dxm.vehdjk.com

PHP:  preg_match('/\d+/', $s);
来源：http://yie.bbcook.cn

JS:   /\d+/.test(s)
来源：http://rzv.hesvh.cn

TS:   /\d+/.test(s)
来源：http://qgp.vehdjk.com


<!-- 参考信息 -->