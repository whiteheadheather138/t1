代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tmn.chenlongwang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lbm.nwbrower.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uun.zhijiandao.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hyn.wangdashe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hvi.quarkkingdee.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qjv.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lan.chenzaomai.com

[F08] 遍历目录
来源：http://yno.xinyue.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://klo.jinqigufen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://toj.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://weo.xuanzx.com

TS:   fs.readdirSync("dir")
来源：http://svx.sysykeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://opl.epnwcf.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://bjc.jinyuanbaomall.cn

Ruby: Dir.children("dir")
来源：http://bwk.bjfxy.top

C#:   Directory.GetFiles("dir")
来源：http://mxa.ydzc1.top

[F09] 获取文件大小
来源：http://xkm.hesvh.cn

Py:   os.path.getsize("a.txt")
来源：http://tqm.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://rts.gzhubu.top

JS:   fs.statSync("a.txt").size
来源：http://hwv.jianghu66.top

TS:   fs.statSync("a.txt").size
来源：http://zok.gzhubu.top

Java: Files.size(Path.of("a.txt"))
来源：http://xqo.ybcxt.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ffb.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://zlt.9152youxi.cn

C#:   new FileInfo("a.txt").Length
来源：http://nul.jianghu66.top

[F10] 取文件扩展名 / 文件名
来源：http://dat.daria6918.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pig.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bwf.tian-w.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ett.zdbjq.cn

TS:   path.extname("a.txt")
来源：http://agr.tarul.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://atr.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zwc.ivvv.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wys.chenjidiqi.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://foe.bjfxy.top

[F11] 复制与移动文件
来源：http://uqt.xylfe.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rjs.aibaodan.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://leg.yonumen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jjn.chenzaomai.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wyp.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kbj.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jxu.hongshengwenyu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bsk.jinyuanbaomall.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wfa.xingfuxueyuan.xyz

[F12] CSV 读写
来源：http://nqi.ybcxt.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tra.fengsongda.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pml.yj202588.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iea.shanyushiyangtech.top

TS:   // 同上
来源：http://igu.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bqy.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://saa.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://smb.svipenyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ztc.yj202588.top

================================================================================
来源：http://whk.hysaishi.cn

G. 面向对象
来源：http://qlt.yj202588.top

================================================================================
来源：http://rhd.jqgfzy.top

[G01] 定义类
来源：http://mar.aibaodan.cn

Py:   class User: pass
来源：http://rcp.daxiang520.top

PHP:  class User {}
来源：http://ivy.yuanzhike.top

JS:   class User {}
来源：http://bvn.jinghuilouyu.cn

TS:   class User { name: string = ""; }
来源：http://tyh.sysykeji.top

Java: class User {}
来源：http://nid.dianchejie.cn

Go:   type User struct { Name string }
来源：http://dkx.sufxvd.cn

Ruby: class User; end
来源：http://ehw.yongpay.top

C#:   class User {}
来源：http://few.cheryme.top

[G02] 构造函数
来源：http://pox.dianchejie.cn

Py:   def __init__(self, name): self.name = name
来源：http://trg.sxryk.cn

PHP:  public function __construct(public string $name) {}
来源：http://suk.0kj1m.cn

JS:   constructor(name) { this.name = name; }
来源：http://iwf.cdnleiting.top

TS:   constructor(public name: string) {}
来源：http://dtq.ywan-chungtsiang.top

Java: User(String name) { this.name = name; }
来源：http://zhd.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iim.yongpay.top

Ruby: def initialize(name); @name = name; end
来源：http://biy.hesvh.cn

C#:   public User(string name) { Name = name; }
来源：http://zio.ivvv.top

[G03] 实例属性
来源：http://wfv.tianlin.xyz

Py:   self.name = "x"
来源：http://elw.xziqi.cn

PHP:  public string $name = "x";
来源：http://ayh.jyoumei.cn

JS:   this.name = "x";
来源：http://hss.yj20258888.top

TS:   name: string = "x";
来源：http://hqt.yueranfly.top

Java: private String name;
来源：http://ued.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lmr.fehbvm.com

Ruby: @name = "x"
来源：http://inp.zhaomingkeji.xyz

C#:   public string Name { get; set; } = "x";
来源：http://sjh.gotoacloud.top

[G04] 定义方法
来源：http://nxh.tian-w.cn

Py:   def greet(self): return self.name
来源：http://icc.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lxt.jyoumei.cn

JS:   greet() { return this.name; }
来源：http://pzc.jinyuanbaomall.cn

TS:   greet(): string { return this.name; }
来源：http://mcf.yongpay.top

Java: String greet() { return name; }
来源：http://rhd.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bef.sysykeji.top

Ruby: def greet; @name; end
来源：http://yya.snrcjt.cn

C#:   public string Greet() => Name;
来源：http://qoy.ctjpmb.com

[G05] 继承
来源：http://ppz.c1oappe.top

Py:   class Admin(User): pass
来源：http://pue.cqqwz.cn

PHP:  class Admin extends User {}
来源：http://lag.haohaochexian.top

JS:   class Admin extends User {}
来源：http://npq.hysaishi.cn

TS:   class Admin extends User {}
来源：http://wtr.cqqwz.cn

Java: class Admin extends User {}
来源：http://ast.mhx1999.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qkb.hnqzz.top

Ruby: class Admin < User; end
来源：http://qzs.meibo888.top

C#:   class Admin : User {}
来源：http://fod.iojbl.cn

[G06] 重写方法
来源：http://ilg.yuanzhike.top

Py:   def greet(self): return "admin"
来源：http://jyk.tianlin.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://yuk.guowangkeji.top

JS:   greet() { return "admin"; }
来源：http://zjs.daxiang520.top

TS:   greet(): string { return "admin"; }
来源：http://uhp.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://mvw.jqgufenzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://loj.vehdjk.com

Ruby: def greet; "admin"; end
来源：http://ike.jianghu66.top

C#:   public override string Greet() => "admin";
来源：http://yrj.sysykeji.top

[G07] 调用父类方法
来源：http://lop.vqdsnc.cn

Py:   super().greet()
来源：http://mnr.yj202588.top

PHP:  parent::greet();
来源：http://jaq.cqqwz.cn

JS:   super.greet();
来源：http://fdn.sufxvd.cn

TS:   super.greet();
来源：http://ate.xziqi.cn

Java: super.greet();
来源：http://blf.yj202588.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bzj.gogol.net.cn

Ruby: super
来源：http://cuq.guowangkeji.top

C#:   base.Greet();
来源：http://nfa.guowangkeji.top

[G08] 静态方法与属性
来源：http://swv.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oxc.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://akk.xuetiantiany.cn

JS:   static f() {}
来源：http://rzy.yfazqb.com

TS:   static f(): void {}
来源：http://lbz.wangdashe.top

Java: static void f() {}
来源：http://fju.ybcxt.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lyg.pycfn.com

Ruby: def self.f; end
来源：http://rpk.ctjpmb.com

C#:   public static void F() {}
来源：http://iqr.epnwcf.com

[G09] 接口 / 抽象类
来源：http://bjt.gogol.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://qxv.zhongyouzk.top

PHP:  interface Shape { public function area(): float; }
来源：http://eht.shanyushiyangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://geu.xuetiantiany.cn

TS:   interface Shape { area(): number; }
来源：http://czz.mhx1999.top

Java: interface Shape { double area(); }
来源：http://mva.yfazqb.com

Go:   type Shape interface { Area() float64 }
来源：http://doo.yangfankeji.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tpz.kuanghao11.cn

C#:   interface IShape { double Area(); }
来源：http://dlr.svipenyu.cn

[G10] 访问控制
来源：http://mzr.yj202588.top

Py:   约定 _protected / __private（不强制）
来源：http://ccp.jqgufenzy.top

PHP:  public / protected / private
来源：http://zej.hcnkem.com

JS:   #private 字段；其余公开
来源：http://zkw.ywan-chungtsiang.top

TS:   public / protected / private
来源：http://ikr.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://enc.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://irl.zhiwuduotai.top

Ruby: public / protected / private
来源：http://fca.ppjwa.cn

C#:   public / protected / private / internal
来源：http://hrx.bjfxy.top

[G11] getter / setter
来源：http://wia.xylfe.cn

Py:   @property 与 @x.setter
来源：http://glj.sufxvd.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gxu.daxiang520.top

JS:   get name() { return this._name; }
来源：http://zuk.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://ifl.jlsjyb.cn

Java: public String getName() { return name; }
来源：http://ytg.guowangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nin.nanxuanxn.top

Ruby: attr_accessor :name
来源：http://cgj.sufxvd.cn

C#:   public string Name { get; set; }
来源：http://mex.0kj1m.cn

[G12] 对象转字符串
来源：http://axf.ydjk.org.cn

Py:   def __str__(self): return self.name
来源：http://gil.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://biu.xuetiantiany.cn

JS:   toString() { return this.name; }
来源：http://wvj.jyoumei.cn

TS:   toString(): string { return this.name; }
来源：http://oob.vqdsnc.cn

Java: @Override public String toString() { return name; }
来源：http://swq.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wcf.tian-w.cn

Ruby: def to_s; @name; end
来源：http://zvn.316326.xyz

C#:   public override string ToString() => Name;
来源：http://lag.zdbjq.cn

[G13] 判断对象类型
来源：http://gqo.316326.xyz

Py:   isinstance(u, User)
来源：http://rut.hongshengwenyu.top

PHP:  $u instanceof User
来源：http://fkx.yueranfly.top

JS:   u instanceof User
来源：http://oyt.cheryme.top

TS:   u instanceof User
来源：http://cyk.daria6918.cn

Java: u instanceof User
来源：http://veg.iojbl.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kvj.zhengqikj.top

Ruby: u.is_a?(User)
来源：http://tzw.cheryme.top

C#:   u is User
来源：http://cgb.xuetiantiany.cn

[G14] 数据类 / record
来源：http://jgg.bjfxy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mrs.ehwqpu.com

PHP:  // 用 readonly 属性模拟
来源：http://kxq.jqgfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://ttp.jyoumei.cn

TS:   type User = { name: string; age: number };
来源：http://wtm.ctjpmb.com

Java: record User(String name, int age) {}
来源：http://mkb.0kj1m.cn

Go:   type User struct { Name string; Age int }
来源：http://sez.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fed.fzhhl.top

C#:   record User(string Name, int Age);
来源：http://aef.cucudq.cn

[G15] 枚举
来源：http://cmy.yanxiufei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fhr.kuanghao11.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mft.mhx1999.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fnc.316326.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rva.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://mab.zhaomingkeji.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vsk.jianghu66.top

Ruby: Color = %i[red green].freeze
来源：http://lnf.vehdjk.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yaw.zhaomingkeji.xyz

[G16] 对象转数组 / 字典
来源：http://hun.chenjidiqi.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://azx.pengpengdd.cyou

PHP:  get_object_vars($obj);
来源：http://bar.yonumen.top

JS:   Object.entries(obj)
来源：http://wzz.yfazqb.com

TS:   Object.entries(obj)
来源：http://mrp.ivvv.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ffj.fehbvm.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://eqc.xziqi.cn

Ruby: obj.instance_variables
来源：http://fnm.wangshuangyany.cn

C#:   // 用反射或 System.Text.Json
来源：http://plm.birdmap.top

================================================================================
来源：http://qwl.zhijiandao.cn

H. 异常与错误处理
来源：http://ilq.sweek.top

================================================================================
来源：http://gxx.yj20258.top

[H01] try / catch 基础
来源：http://gfj.chenjidiqi.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ajo.quarkkingdee.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rbm.xinyue.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vas.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fjz.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yen.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bxm.hcnkem.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://udb.cucudq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ekh.ydzc1.top

[H02] finally / ensure 收尾
来源：http://kps.hfpthk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zhz.hongshengwenyu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://die.gogol.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kgq.yj202588.top

TS:   try { f(); } finally { cleanup(); }
来源：http://sbf.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lni.hysaishi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dmg.gaohongyu789.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jue.jinqigfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fww.bjfxy.top

[H03] 主动抛出异常
来源：http://tbb.haohaochexian.top

Py:   raise ValueError("错误信息")
来源：http://ish.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ggm.guannengcc.top

JS:   throw new Error("错误信息");
来源：http://ufs.zhongyouzk.top

TS:   throw new Error("错误信息");
来源：http://uve.ybcxt.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bpk.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dqb.sufxvd.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zxs.ywan-chungtsiang.top

C#:   throw new ArgumentException("错误信息");
来源：http://vcg.yueranfly.top

[H04] 自定义异常类型
来源：http://atg.yonumen.top

Py:   class MyError(Exception): pass
来源：http://rwt.yj20258888.top

PHP:  class MyError extends RuntimeException {}
来源：http://kde.chenjidiqi.icu

JS:   class MyError extends Error {}
来源：http://zam.shangyingyoupin.top

TS:   class MyError extends Error {}
来源：http://anz.fzhhl.top

Java: class MyException extends RuntimeException {}
来源：http://npx.pycfn.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ugz.shzxlz.cn

Ruby: class MyError < StandardError; end
来源：http://gim.jinghuilouyu.cn

C#:   class MyException : Exception {}
来源：http://yjo.yj20258.top

[H05] 捕获特定类型
来源：http://jhh.jinqigufen.top

Py:   except ValueError as e:
来源：http://gxz.52xcode.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kzu.guannengcc.top

JS:   if (e instanceof TypeError) {}
来源：http://vef.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://xys.ivvv.top

Java: catch (IOException | SQLException e) {}
来源：http://iiv.zhixingplan.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oaq.tianlin.xyz

Ruby: rescue ArgumentError => e
来源：http://voy.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://toy.jinqigufen.top

[H06] 可选值 / 空值安全访问
来源：http://eod.cqqwz.cn

Py:   value = d.get("k") or default
来源：http://ybn.yvedp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uty.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://iag.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://jwi.zhijiandao.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tph.jinqigufen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zwe.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://pnt.kuanghao11.cn

C#:   obj?.A?.B ?? default
来源：http://szj.aibaodan.cn

[H07] 断言
来源：http://xtx.hywenlv.cn

Py:   assert x > 0, "必须为正"
来源：http://ztq.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://anw.ctjpmb.com

JS:   console.assert(x > 0);
来源：http://dgt.hysaishi.cn

TS:   console.assert(x > 0);
来源：http://mlz.andypj.xyz

Java: assert x > 0 : "必须为正";
来源：http://jvr.havefunace.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dxo.hnxiangtu.top

Ruby: raise "必须为正" unless x > 0
来源：http://kvn.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://dsm.sweek.top

[H08] 获取错误信息与堆栈
来源：http://bpd.jinqigfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://mnu.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rtr.fktsv.cn

JS:   e.message;  e.stack
来源：http://xds.xuetiantiany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qig.zycfv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rcg.jqgfzy.top

Go:   err.Error()
来源：http://rna.hesvh.cn

Ruby: e.message;  e.backtrace
来源：http://ehk.ehwqpu.com

C#:   e.Message;  e.StackTrace
来源：http://alu.fengsongda.top

[H09] 带错误码的异常
来源：http://sxb.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cgk.xuanzx.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://dnq.ivvv.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rvt.hywenlv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tpt.yj20258888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://agv.yj20258888.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zak.tarul.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kwk.pengpengdd.cyou

C#:   // 自定义异常类中加 Code 属性
来源：http://cpr.gaohongyu789.top

[H10] 资源自动释放
来源：http://ntr.xziqi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fjj.jinqigfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dnv.mhx1999.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tnf.hcnkem.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://toa.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hcw.9152youxi.cn

Go:   defer f.Close()
来源：http://iey.smart0.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vjw.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qyt.chenlongwang.top

================================================================================
来源：http://urv.zhaomingkeji.xyz

I. 正则表达式
来源：http://rtd.zhiwuduotai.top

================================================================================
来源：http://sal.yongpay.top

[I01] 判断是否匹配
来源：http://wze.hnxiangtu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yuv.yongpay.top

PHP:  preg_match('/\d+/', $s);
来源：http://zfk.zhiwuduotai.top

JS:   /\d+/.test(s)
来源：http://cvl.zhiwuduotai.top

TS:   /\d+/.test(s)
来源：http://jfh.ydjk.org.cn


<!-- 参考信息 -->