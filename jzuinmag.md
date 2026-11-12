代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://swe.gotoacloud.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gzk.aibaodan.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ike.xziqi.cn

[F08] 遍历目录
来源：http://gtl.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hzv.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ygj.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://pwl.shangyingyoupin.top

TS:   fs.readdirSync("dir")
来源：http://zod.shzxlz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cxu.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://twt.vqdsnc.cn

Ruby: Dir.children("dir")
来源：http://lwl.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://aur.cucudq.cn

[F09] 获取文件大小
来源：http://wnm.aizwys.cn

Py:   os.path.getsize("a.txt")
来源：http://mkp.hywenlv.cn

PHP:  filesize("a.txt");
来源：http://aks.fehbvm.com

JS:   fs.statSync("a.txt").size
来源：http://bno.xinyue.icu

TS:   fs.statSync("a.txt").size
来源：http://thm.ydzc1.top

Java: Files.size(Path.of("a.txt"))
来源：http://mtc.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rlz.nanxinkj.top

Ruby: File.size("a.txt")
来源：http://dsg.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://cdg.zhiwuduotai.top

[F10] 取文件扩展名 / 文件名
来源：http://ics.sxryk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jhn.jyoumei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qey.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fxd.bbcook.cn

TS:   path.extname("a.txt")
来源：http://xcl.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dqb.nanxinkj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ydq.yj202588.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dcd.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jbm.fanxiaobao.xyz

[F11] 复制与移动文件
来源：http://nha.pengpengdd.cyou

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vwx.fzhhl.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mff.yuxming.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ktv.zhaomingkeji.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://orl.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dlq.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vxl.nanxuanxn.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://keq.jqgufenzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nhd.xingfuxueyuan.xyz

[F12] CSV 读写
来源：http://tih.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cum.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rhv.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tbx.sjlbkw.cn

TS:   // 同上
来源：http://qes.jinqigfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qht.haohaochexian.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://npz.xinyue.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://scn.jinghuilouyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wnq.zhongyouzk.top

================================================================================
来源：http://wku.yj20258888.top

G. 面向对象
来源：http://mud.fanxiaobao.xyz

================================================================================
来源：http://jpf.hongshengwenyu.top

[G01] 定义类
来源：http://bar.yangfankeji.com

Py:   class User: pass
来源：http://vdi.fehbvm.com

PHP:  class User {}
来源：http://zfz.ydjk.org.cn

JS:   class User {}
来源：http://tsy.zdqjudy.top

TS:   class User { name: string = ""; }
来源：http://lez.zhijiandao.cn

Java: class User {}
来源：http://jhj.fzhhl.top

Go:   type User struct { Name string }
来源：http://trd.xuetiantiany.cn

Ruby: class User; end
来源：http://uck.wangdashe.top

C#:   class User {}
来源：http://xbq.nanxuanxn.top

[G02] 构造函数
来源：http://vmc.zhengqikj.top

Py:   def __init__(self, name): self.name = name
来源：http://kxx.wangdashe.top

PHP:  public function __construct(public string $name) {}
来源：http://azj.hesvh.cn

JS:   constructor(name) { this.name = name; }
来源：http://lxp.yuxming.cn

TS:   constructor(public name: string) {}
来源：http://kww.zhongyouzk.top

Java: User(String name) { this.name = name; }
来源：http://rni.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hgn.jianghu66.top

Ruby: def initialize(name); @name = name; end
来源：http://iwn.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://vgx.yueranfly.top

[G03] 实例属性
来源：http://kje.wangdashe.top

Py:   self.name = "x"
来源：http://oil.ybcxt.top

PHP:  public string $name = "x";
来源：http://imv.hesvh.cn

JS:   this.name = "x";
来源：http://dwe.cheryme.top

TS:   name: string = "x";
来源：http://fum.yonumen.top

Java: private String name;
来源：http://alp.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gro.yanxiufei.cn

Ruby: @name = "x"
来源：http://dfr.hammf.cn

C#:   public string Name { get; set; } = "x";
来源：http://wbm.redwolf501.top

[G04] 定义方法
来源：http://eul.wangshuangyany.cn

Py:   def greet(self): return self.name
来源：http://xmz.shuidangran.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pft.meibo888.top

JS:   greet() { return this.name; }
来源：http://jxg.cashguo.top

TS:   greet(): string { return this.name; }
来源：http://lwc.yj202588.top

Java: String greet() { return name; }
来源：http://kty.nanxuanxn.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://oyn.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://iih.cucudq.cn

C#:   public string Greet() => Name;
来源：http://aho.xingfuxueyuan.xyz

[G05] 继承
来源：http://wqp.yj20258888.top

Py:   class Admin(User): pass
来源：http://exb.yuxming.cn

PHP:  class Admin extends User {}
来源：http://zim.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://juk.gaohongyu789.top

TS:   class Admin extends User {}
来源：http://isq.xinyue.icu

Java: class Admin extends User {}
来源：http://zrj.yj20258888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qye.yangfankeji.com

Ruby: class Admin < User; end
来源：http://zrd.cashguo.top

C#:   class Admin : User {}
来源：http://amu.yangfankeji.com

[G06] 重写方法
来源：http://cey.cheryme.top

Py:   def greet(self): return "admin"
来源：http://opq.c1oappe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jnb.fktsv.cn

JS:   greet() { return "admin"; }
来源：http://ywx.nwbrower.top

TS:   greet(): string { return "admin"; }
来源：http://nip.xylfe.cn

Java: @Override String greet() { return "admin"; }
来源：http://knu.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jcw.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://vcf.ctjpmb.com

C#:   public override string Greet() => "admin";
来源：http://vws.tian-w.cn

[G07] 调用父类方法
来源：http://ylb.yueranfly.top

Py:   super().greet()
来源：http://zvb.xuanzx.com

PHP:  parent::greet();
来源：http://qyd.pengpengdd.cyou

JS:   super.greet();
来源：http://aim.yuxming.cn

TS:   super.greet();
来源：http://woo.jinyuanbaomall.cn

Java: super.greet();
来源：http://afg.daria6918.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xug.snrcjt.cn

Ruby: super
来源：http://fig.shanyushiyangkeji.top

C#:   base.Greet();
来源：http://lkw.yongpay.top

[G08] 静态方法与属性
来源：http://wtx.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ovn.epnwcf.com

PHP:  public static function f() {}
来源：http://vla.fengsongda.top

JS:   static f() {}
来源：http://tan.ybcxt.top

TS:   static f(): void {}
来源：http://tvp.yj20258.top

Java: static void f() {}
来源：http://crm.xuetiantiany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://psc.zdbjq.cn

Ruby: def self.f; end
来源：http://soy.yuxming.cn

C#:   public static void F() {}
来源：http://nsv.dianchejie.cn

[G09] 接口 / 抽象类
来源：http://bvf.pycfn.com

Py:   from abc import ABC, abstractmethod
来源：http://dto.zdbjq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jzb.cdnleiting.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fdx.zhaomingkeji.xyz

TS:   interface Shape { area(): number; }
来源：http://kma.xziqi.cn

Java: interface Shape { double area(); }
来源：http://hyc.xziqi.cn

Go:   type Shape interface { Area() float64 }
来源：http://kwz.chenjidiqi.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nud.zhixingplan.top

C#:   interface IShape { double Area(); }
来源：http://zqh.zhixingplan.top

[G10] 访问控制
来源：http://pen.bbcook.cn

Py:   约定 _protected / __private（不强制）
来源：http://cdp.sxryk.cn

PHP:  public / protected / private
来源：http://gfi.hfpthk.cn

JS:   #private 字段；其余公开
来源：http://cki.daxiang520.top

TS:   public / protected / private
来源：http://fab.316326.xyz

Java: public / protected / private / 默认包级
来源：http://mmn.52xcode.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kzr.jqgfzy.top

Ruby: public / protected / private
来源：http://wbx.yuanzhike.top

C#:   public / protected / private / internal
来源：http://idd.mhx1999.top

[G11] getter / setter
来源：http://dog.yj202588.top

Py:   @property 与 @x.setter
来源：http://mva.yangfankeji.com

PHP:  public function getName(): string { return $this->name; }
来源：http://udg.yj20258888.top

JS:   get name() { return this._name; }
来源：http://tre.cheryme.top

TS:   get name(): string { return this._name; }
来源：http://ocp.uphjek.com

Java: public String getName() { return name; }
来源：http://xeo.xylfe.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tee.sufxvd.cn

Ruby: attr_accessor :name
来源：http://yye.hfpthk.cn

C#:   public string Name { get; set; }
来源：http://juf.tian-w.cn

[G12] 对象转字符串
来源：http://wqe.uphjek.com

Py:   def __str__(self): return self.name
来源：http://ixc.yonumen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wlo.yvedp.cn

JS:   toString() { return this.name; }
来源：http://cdq.daxiang520.top

TS:   toString(): string { return this.name; }
来源：http://bdf.mhx1999.top

Java: @Override public String toString() { return name; }
来源：http://ivp.dianchejie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gmd.ctjpmb.com

Ruby: def to_s; @name; end
来源：http://mqr.fehbvm.com

C#:   public override string ToString() => Name;
来源：http://kqp.zhaomingkeji.xyz

[G13] 判断对象类型
来源：http://iev.yj20258.top

Py:   isinstance(u, User)
来源：http://qjk.bjfxy.top

PHP:  $u instanceof User
来源：http://pmx.zdbjq.cn

JS:   u instanceof User
来源：http://tyf.yuanzhike.top

TS:   u instanceof User
来源：http://him.shangyingyoupin.top

Java: u instanceof User
来源：http://djz.52xcode.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dzv.yueranfly.top

Ruby: u.is_a?(User)
来源：http://gxa.redwolf501.top

C#:   u is User
来源：http://zhk.aibaodan.cn

[G14] 数据类 / record
来源：http://xjm.nanxinkj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aci.hongshengwenyu.top

PHP:  // 用 readonly 属性模拟
来源：http://xsn.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zlu.hysaishi.cn

TS:   type User = { name: string; age: number };
来源：http://dlx.chenlongwang.top

Java: record User(String name, int age) {}
来源：http://grd.yuxming.cn

Go:   type User struct { Name string; Age int }
来源：http://svs.jqgufenzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vxh.cucudq.cn

C#:   record User(string Name, int Age);
来源：http://pcq.vehdjk.com

[G15] 枚举
来源：http://lox.jinghuilouyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bjt.jianghu66.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mou.cucudq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zxh.sxryk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jdq.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://jpu.xylfe.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nyq.guowangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://ibs.vqdsnc.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://naf.zhoulong.xyz

[G16] 对象转数组 / 字典
来源：http://opw.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ugk.yongpay.top

PHP:  get_object_vars($obj);
来源：http://ydi.fehbvm.com

JS:   Object.entries(obj)
来源：http://vyk.zycfv.cn

TS:   Object.entries(obj)
来源：http://yzj.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lba.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pti.sufxvd.cn

Ruby: obj.instance_variables
来源：http://nkk.xinyue.icu

C#:   // 用反射或 System.Text.Json
来源：http://fqq.quarkkingdee.top

================================================================================
来源：http://efg.iojbl.cn

H. 异常与错误处理
来源：http://sfp.birdmap.top

================================================================================
来源：http://qov.yuanzhike.top

[H01] try / catch 基础
来源：http://qre.dashuyun.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kaa.gotoacloud.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jsq.nwbrower.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mou.dashuyun.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jpt.fehbvm.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oos.xuanzx.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gbc.nanxuanxn.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://knh.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://loc.zhongyouzk.top

[H02] finally / ensure 收尾
来源：http://bed.pengpengdd.cyou

Py:   try: f()⏎finally: cleanup()
来源：http://loc.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lcj.yj202588.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qie.52xcode.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qae.tianlin.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://hhg.nanxuanxn.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://csf.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pso.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://azy.guowangkeji.top

[H03] 主动抛出异常
来源：http://mdl.dianchejie.cn

Py:   raise ValueError("错误信息")
来源：http://pgq.pengpengdd.cyou

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vkm.xuetiantiany.cn

JS:   throw new Error("错误信息");
来源：http://xgj.yj20258.top

TS:   throw new Error("错误信息");
来源：http://opa.hnqzz.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hvs.shuidangran.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kdf.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wnt.c1oappe.top

C#:   throw new ArgumentException("错误信息");
来源：http://qie.zycfv.cn

[H04] 自定义异常类型
来源：http://grj.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://dos.hywenlv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qhp.fanxiaobao.xyz

JS:   class MyError extends Error {}
来源：http://jbf.sweek.top

TS:   class MyError extends Error {}
来源：http://liw.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://hlj.52xcode.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ida.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://brd.aizwys.cn

C#:   class MyException : Exception {}
来源：http://puj.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://pkm.cucudq.cn

Py:   except ValueError as e:
来源：http://itf.jqgufenzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iex.cheryme.top

JS:   if (e instanceof TypeError) {}
来源：http://ahf.birdmap.top

TS:   if (e instanceof TypeError) {}
来源：http://mco.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://uph.guannengcc.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sjv.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://cqg.sufxvd.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dwo.zhengqikj.top

[H06] 可选值 / 空值安全访问
来源：http://rup.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://zsc.snrcjt.cn

PHP:  $v = $d["k"] ?? null;
来源：http://unh.jqgufenzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://jqy.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://hdp.gotoacloud.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://idi.ppjwa.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://blm.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://ktg.yueranfly.top

C#:   obj?.A?.B ?? default
来源：http://dxn.hnxiangtu.top

[H07] 断言
来源：http://pvh.tarul.cn

Py:   assert x > 0, "必须为正"
来源：http://qxz.haohaochexian.top

PHP:  assert($x > 0);
来源：http://agn.zhengqikj.top

JS:   console.assert(x > 0);
来源：http://ykl.guannengcc.top

TS:   console.assert(x > 0);
来源：http://hus.ppjwa.cn

Java: assert x > 0 : "必须为正";
来源：http://wjp.gaohongyu789.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mru.hcnkem.com

Ruby: raise "必须为正" unless x > 0
来源：http://fxv.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://zkz.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://nxa.jinqigfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://xiy.ppjwa.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qho.52xcode.cn

JS:   e.message;  e.stack
来源：http://cio.hnxiangtu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xke.havefunace.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vhr.ydzc1.top

Go:   err.Error()
来源：http://edm.fktsv.cn

Ruby: e.message;  e.backtrace
来源：http://kki.yueranfly.top

C#:   e.Message;  e.StackTrace
来源：http://fas.andypj.xyz

[H09] 带错误码的异常
来源：http://kns.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mvg.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mva.xziqi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tud.shangyingyoupin.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fjq.pycfn.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tnc.yuanzhike.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lkm.fanxiaobao.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://pwi.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qbr.haohaochexian.top

[H10] 资源自动释放
来源：http://mim.meibo888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lic.kuanghao11.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ctd.wangshuangyany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rlk.redwolf501.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sal.chenjidiqi.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://snc.zhixingplan.top

Go:   defer f.Close()
来源：http://aot.yueranfly.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ahe.sufxvd.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rda.c1oappe.top

================================================================================
来源：http://hym.dianchejie.cn

I. 正则表达式
来源：http://bfg.bbcook.cn

================================================================================
来源：http://pnr.wangdashe.top

[I01] 判断是否匹配
来源：http://yew.birdmap.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sej.zhengqikj.top

PHP:  preg_match('/\d+/', $s);
来源：http://phf.nwbrower.top

JS:   /\d+/.test(s)
来源：http://gji.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://epp.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xks.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zlh.wangshuangyany.cn

Ruby: s.match?(/\d+/)
来源：http://szn.shangyingyoupin.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://erv.uphjek.com


<!-- 参考信息 -->