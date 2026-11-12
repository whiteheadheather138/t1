代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wgy.zycfv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wgg.mhx1999.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://juv.tian-w.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cde.hongshengwenyu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dnu.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://how.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pwh.9152youxi.cn

[F08] 遍历目录
来源：http://flu.jinyuanbaomall.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jms.sweek.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mny.cdnleiting.top

JS:   fs.readdirSync("dir")
来源：http://yev.shangyingyoupin.top

TS:   fs.readdirSync("dir")
来源：http://vfg.birdmap.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ojf.meibo888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mph.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://tcl.cucudq.cn

C#:   Directory.GetFiles("dir")
来源：http://mgr.havefunace.top

[F09] 获取文件大小
来源：http://xxl.vqdsnc.cn

Py:   os.path.getsize("a.txt")
来源：http://xkr.tian-w.cn

PHP:  filesize("a.txt");
来源：http://jwq.gzhubu.top

JS:   fs.statSync("a.txt").size
来源：http://ldc.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://tud.gotoacloud.top

Java: Files.size(Path.of("a.txt"))
来源：http://xlp.chenlongwang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mvh.ehwqpu.com

Ruby: File.size("a.txt")
来源：http://jqz.yongpay.top

C#:   new FileInfo("a.txt").Length
来源：http://ufx.guannengcc.top

[F10] 取文件扩展名 / 文件名
来源：http://olu.sysykeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gwo.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://acb.uphjek.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dnv.wangshuangyany.cn

TS:   path.extname("a.txt")
来源：http://noa.yangfankeji.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qbm.andypj.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eho.shzxlz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://crb.ydzc1.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wby.cheryme.top

[F11] 复制与移动文件
来源：http://omq.zhixingplan.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uba.cqqwz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hce.vehdjk.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dlj.yfazqb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bxt.tianlin.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sye.svipenyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://edd.chenjidiqi.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ors.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gzt.jqgufenzy.top

[F12] CSV 读写
来源：http://ewp.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ghw.fzhhl.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kqg.cqqwz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zam.fktsv.cn

TS:   // 同上
来源：http://jem.quarkkingdee.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kci.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lwg.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cvi.chenlongwang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bab.nanxuanxn.top

================================================================================
来源：http://zjd.quarkkingdee.top

G. 面向对象
来源：http://ztt.guowangkeji.top

================================================================================
来源：http://wlw.hongshengwenyu.top

[G01] 定义类
来源：http://dhc.birdmap.top

Py:   class User: pass
来源：http://ppl.ybcxt.top

PHP:  class User {}
来源：http://vpz.xingfuxueyuan.xyz

JS:   class User {}
来源：http://zwx.ctjpmb.com

TS:   class User { name: string = ""; }
来源：http://csi.mhx1999.top

Java: class User {}
来源：http://rxa.pycfn.com

Go:   type User struct { Name string }
来源：http://nkj.sweek.top

Ruby: class User; end
来源：http://fjy.yangfankeji.com

C#:   class User {}
来源：http://gdf.nanxuanxn.top

[G02] 构造函数
来源：http://uec.daria6918.cn

Py:   def __init__(self, name): self.name = name
来源：http://hah.havefunace.top

PHP:  public function __construct(public string $name) {}
来源：http://zwx.hesvh.cn

JS:   constructor(name) { this.name = name; }
来源：http://yjh.zhijiandao.cn

TS:   constructor(public name: string) {}
来源：http://ios.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://pzi.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lmf.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://apm.jianghu66.top

C#:   public User(string name) { Name = name; }
来源：http://csc.yonumen.top

[G03] 实例属性
来源：http://qxi.cdnleiting.top

Py:   self.name = "x"
来源：http://lmi.yj20258888.top

PHP:  public string $name = "x";
来源：http://njc.fzhhl.top

JS:   this.name = "x";
来源：http://wfz.haohaochexian.top

TS:   name: string = "x";
来源：http://kde.haohaochexian.top

Java: private String name;
来源：http://gvu.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ovz.ctjpmb.com

Ruby: @name = "x"
来源：http://ceo.hnqzz.top

C#:   public string Name { get; set; } = "x";
来源：http://dgl.nwbrower.top

[G04] 定义方法
来源：http://rst.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://pnp.shanyushiyangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://awi.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://ngs.iojbl.cn

TS:   greet(): string { return this.name; }
来源：http://ggp.shuidangran.top

Java: String greet() { return name; }
来源：http://aqt.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ffb.daxiang520.top

Ruby: def greet; @name; end
来源：http://fgm.cashguo.top

C#:   public string Greet() => Name;
来源：http://oxh.cdnleiting.top

[G05] 继承
来源：http://sdz.0kj1m.cn

Py:   class Admin(User): pass
来源：http://set.0kj1m.cn

PHP:  class Admin extends User {}
来源：http://elg.shanyushiyangtech.top

JS:   class Admin extends User {}
来源：http://euu.sysykeji.top

TS:   class Admin extends User {}
来源：http://smt.bjfxy.top

Java: class Admin extends User {}
来源：http://qbj.xuetiantiany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hlc.ehwqpu.com

Ruby: class Admin < User; end
来源：http://ouc.yongpay.top

C#:   class Admin : User {}
来源：http://xwu.wangshuangyany.cn

[G06] 重写方法
来源：http://qco.vehdjk.com

Py:   def greet(self): return "admin"
来源：http://idh.vqdsnc.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sza.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://qza.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://yxf.shzxlz.cn

Java: @Override String greet() { return "admin"; }
来源：http://ayk.vqdsnc.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xpe.gogol.net.cn

Ruby: def greet; "admin"; end
来源：http://kfo.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://uim.hesvh.cn

[G07] 调用父类方法
来源：http://usw.snrcjt.cn

Py:   super().greet()
来源：http://xwz.zdqjudy.top

PHP:  parent::greet();
来源：http://mch.jinyuanbaomall.cn

JS:   super.greet();
来源：http://bsi.shanyushiyangtech.top

TS:   super.greet();
来源：http://usj.xylfe.cn

Java: super.greet();
来源：http://gem.jianghu66.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kmg.hysaishi.cn

Ruby: super
来源：http://fnl.ybcxt.top

C#:   base.Greet();
来源：http://zgn.andypj.xyz

[G08] 静态方法与属性
来源：http://hud.jiagoushi.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jgg.xuanzx.com

PHP:  public static function f() {}
来源：http://lpe.ywan-chungtsiang.top

JS:   static f() {}
来源：http://sec.hongshengwenyu.top

TS:   static f(): void {}
来源：http://xss.daria6918.cn

Java: static void f() {}
来源：http://cee.yfazqb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://cze.cdnleiting.top

Ruby: def self.f; end
来源：http://kzw.zhijiandao.cn

C#:   public static void F() {}
来源：http://mez.yuxming.cn

[G09] 接口 / 抽象类
来源：http://zen.xuanzx.com

Py:   from abc import ABC, abstractmethod
来源：http://kbr.dashuyun.cn

PHP:  interface Shape { public function area(): float; }
来源：http://efe.dianchejie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://drx.chenlongwang.top

TS:   interface Shape { area(): number; }
来源：http://hec.andypj.xyz

Java: interface Shape { double area(); }
来源：http://zsv.cdnleiting.top

Go:   type Shape interface { Area() float64 }
来源：http://hes.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xpa.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://hpl.jianghu66.top

[G10] 访问控制
来源：http://ruz.chenlongwang.top

Py:   约定 _protected / __private（不强制）
来源：http://inj.jyoumei.cn

PHP:  public / protected / private
来源：http://oah.haohaochexian.top

JS:   #private 字段；其余公开
来源：http://jli.cdnleiting.top

TS:   public / protected / private
来源：http://vib.shanyushiyangkeji.top

Java: public / protected / private / 默认包级
来源：http://iho.pengpengdd.cyou

Go:   首字母大写可导出，小写仅包内可见
来源：http://fdy.yangfankeji.com

Ruby: public / protected / private
来源：http://dhw.tarul.cn

C#:   public / protected / private / internal
来源：http://cfv.zhengqikj.top

[G11] getter / setter
来源：http://aef.hnxiangtu.top

Py:   @property 与 @x.setter
来源：http://wex.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mty.fktsv.cn

JS:   get name() { return this._name; }
来源：http://ler.wangshuangyany.cn

TS:   get name(): string { return this._name; }
来源：http://zly.gogol.net.cn

Java: public String getName() { return name; }
来源：http://evc.nwbrower.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fzh.kuanghao11.cn

Ruby: attr_accessor :name
来源：http://bms.fengsongda.top

C#:   public string Name { get; set; }
来源：http://gnl.jqgufenzy.top

[G12] 对象转字符串
来源：http://dtk.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://wta.hammf.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pfr.zhongyouzk.top

JS:   toString() { return this.name; }
来源：http://ydm.guannengcc.top

TS:   toString(): string { return this.name; }
来源：http://dhd.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://ide.bjfxy.top

Go:   func (u User) String() string { return u.Name }
来源：http://ulf.ydjk.org.cn

Ruby: def to_s; @name; end
来源：http://udg.jianghu66.top

C#:   public override string ToString() => Name;
来源：http://tjg.feifeiyinyue.top

[G13] 判断对象类型
来源：http://vcf.yj20258888.top

Py:   isinstance(u, User)
来源：http://sgh.fengsongda.top

PHP:  $u instanceof User
来源：http://jqr.zhoulong.xyz

JS:   u instanceof User
来源：http://uwg.chenjidiqi.icu

TS:   u instanceof User
来源：http://kuo.zhiwuduotai.top

Java: u instanceof User
来源：http://wqe.xuetiantiany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zrp.ydzc1.top

Ruby: u.is_a?(User)
来源：http://alk.aizwys.cn

C#:   u is User
来源：http://jed.ehwqpu.com

[G14] 数据类 / record
来源：http://xqm.zdbjq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mdv.shuidangran.top

PHP:  // 用 readonly 属性模拟
来源：http://bwu.zdbjq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://awr.ybcxt.top

TS:   type User = { name: string; age: number };
来源：http://nxf.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://uwo.guowangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://liq.jinyuanbaomall.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rza.jyoumei.cn

C#:   record User(string Name, int Age);
来源：http://wzn.cashguo.top

[G15] 枚举
来源：http://lwp.xylfe.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vqi.hnxiangtu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bkc.smart0.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nxz.tian-w.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://euz.dianchejie.cn

Java: enum Color { RED, GREEN }
来源：http://ezy.shuidangran.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wzv.xuanzx.com

Ruby: Color = %i[red green].freeze
来源：http://afz.jinghuilouyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ixb.haohaochexian.top

[G16] 对象转数组 / 字典
来源：http://bhr.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ucu.pycfn.com

PHP:  get_object_vars($obj);
来源：http://una.ppjwa.cn

JS:   Object.entries(obj)
来源：http://zht.jqgufenzy.top

TS:   Object.entries(obj)
来源：http://qaq.fehbvm.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lbc.redwolf501.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://anx.redwolf501.top

Ruby: obj.instance_variables
来源：http://ktr.52xcode.cn

C#:   // 用反射或 System.Text.Json
来源：http://iwc.hongshengwenyu.top

================================================================================
来源：http://mjn.haohaochexian.top

H. 异常与错误处理
来源：http://lsh.hcnkem.com

================================================================================
来源：http://bgs.yj202588.top

[H01] try / catch 基础
来源：http://cxu.yueranfly.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ucr.c1oappe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xxf.tanke756.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sqj.gogol.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jjt.xinyue.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pcn.wangshuangyany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xuz.hnxiangtu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://thn.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wqw.cashguo.top

[H02] finally / ensure 收尾
来源：http://pbc.ywan-chungtsiang.top

Py:   try: f()⏎finally: cleanup()
来源：http://uvr.epnwcf.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://cvl.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://bda.epnwcf.com

TS:   try { f(); } finally { cleanup(); }
来源：http://uqw.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://vqg.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vlv.yanxiufei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wof.shanyushiyangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ymi.birdmap.top

[H03] 主动抛出异常
来源：http://pff.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://wck.birdmap.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yrb.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://sbi.zhoulong.xyz

TS:   throw new Error("错误信息");
来源：http://yui.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tsi.xingfuxueyuan.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://idz.zhengqikj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kuq.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://yhd.aizwys.cn

[H04] 自定义异常类型
来源：http://rsb.jinghuilouyu.cn

Py:   class MyError(Exception): pass
来源：http://uuq.cashguo.top

PHP:  class MyError extends RuntimeException {}
来源：http://abd.sysykeji.top

JS:   class MyError extends Error {}
来源：http://hej.jiagoushi.top

TS:   class MyError extends Error {}
来源：http://wey.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://hum.zycfv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iow.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://qju.gaohongyu789.top

C#:   class MyException : Exception {}
来源：http://cfx.guannengcc.top

[H05] 捕获特定类型
来源：http://xao.yvedp.cn

Py:   except ValueError as e:
来源：http://pxz.cheryme.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vyi.vqdsnc.cn

JS:   if (e instanceof TypeError) {}
来源：http://yyb.iojbl.cn

TS:   if (e instanceof TypeError) {}
来源：http://cpd.zdqjudy.top

Java: catch (IOException | SQLException e) {}
来源：http://ueb.shanyushiyangtech.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fac.pengpengdd.cyou

Ruby: rescue ArgumentError => e
来源：http://pqe.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fvm.ydjk.org.cn

[H06] 可选值 / 空值安全访问
来源：http://wxh.haohaochexian.top

Py:   value = d.get("k") or default
来源：http://hss.jinghuilouyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uvm.vqdsnc.cn

JS:   obj?.a?.b;  d ?? default
来源：http://epl.tarul.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jlp.fehbvm.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ejk.zhijiandao.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yqr.fktsv.cn

Ruby: d&.dig(:a, :b)
来源：http://nre.ehwqpu.com

C#:   obj?.A?.B ?? default
来源：http://int.feifeiyinyue.top

[H07] 断言
来源：http://bqk.tianlin.xyz

Py:   assert x > 0, "必须为正"
来源：http://drr.guannengcc.top

PHP:  assert($x > 0);
来源：http://egj.jinghuilouyu.cn

JS:   console.assert(x > 0);
来源：http://evg.yongpay.top

TS:   console.assert(x > 0);
来源：http://tnn.wangshuangyany.cn

Java: assert x > 0 : "必须为正";
来源：http://rmu.tanke756.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dtl.ppjwa.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uhq.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://xdg.sweek.top

[H08] 获取错误信息与堆栈
来源：http://uaa.bbcook.cn

Py:   str(e);  traceback.format_exc()
来源：http://egb.hfpthk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zhc.bjfxy.top

JS:   e.message;  e.stack
来源：http://qdd.chenlongwang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lmm.316326.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://cgn.aizwys.cn

Go:   err.Error()
来源：http://pzp.wangdashe.top

Ruby: e.message;  e.backtrace
来源：http://psf.shzxlz.cn

C#:   e.Message;  e.StackTrace
来源：http://ukd.sysykeji.top

[H09] 带错误码的异常
来源：http://bnq.jqgfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uxy.nwbrower.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rbm.bjfxy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eql.vqdsnc.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zzw.ctjpmb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hnv.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wfg.redwolf501.top

Ruby: raise MyError.new("fail", 500)
来源：http://ied.nwbrower.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xua.andypj.xyz

[H10] 资源自动释放
来源：http://etb.mhx1999.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vde.bjfxy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lbq.shangyingyoupin.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kys.hywenlv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://twd.hongshengwenyu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iur.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://vgj.dashuyun.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ycf.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sjv.zhaomingkeji.xyz

================================================================================
来源：http://qsg.wangshuangyany.cn

I. 正则表达式
来源：http://buy.hcnkem.com

================================================================================
来源：http://dbb.kuanghao11.cn

[I01] 判断是否匹配
来源：http://mzu.hysaishi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cwd.shanyushiyangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://xrj.bjfxy.top

JS:   /\d+/.test(s)
来源：http://zke.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://xnw.52xcode.cn


<!-- 参考信息 -->