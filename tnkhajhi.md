代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ifl.meibo888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zwb.sjlbkw.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wqi.nanxuanxn.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dbs.xinyue.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wbo.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tym.yj202588.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uvm.shzxlz.cn

[F08] 遍历目录
来源：http://mfj.wangshuangyany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tfy.316326.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pzl.yueranfly.top

JS:   fs.readdirSync("dir")
来源：http://xgk.aibaodan.cn

TS:   fs.readdirSync("dir")
来源：http://zek.yongpay.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vxw.snrcjt.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ayk.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://ppr.gogol.net.cn

C#:   Directory.GetFiles("dir")
来源：http://lrh.daxiang520.top

[F09] 获取文件大小
来源：http://sww.xingfuxueyuan.xyz

Py:   os.path.getsize("a.txt")
来源：http://jvt.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://asp.sufxvd.cn

JS:   fs.statSync("a.txt").size
来源：http://vqs.iojbl.cn

TS:   fs.statSync("a.txt").size
来源：http://lmi.cdnleiting.top

Java: Files.size(Path.of("a.txt"))
来源：http://dim.pycfn.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://iyj.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://dum.fktsv.cn

C#:   new FileInfo("a.txt").Length
来源：http://cpw.shanyushiyangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://wgd.fzhhl.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://plz.jlsjyb.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wau.sufxvd.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uxh.ppjwa.cn

TS:   path.extname("a.txt")
来源：http://vja.jinyuanbaomall.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kgp.sjlbkw.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vwg.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hmp.havefunace.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zfo.hcnkem.com

[F11] 复制与移动文件
来源：http://xsf.bjfxy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bvw.jinqigfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cla.ctjpmb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://csm.jinghuilouyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gai.zhoulong.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cmd.hfpthk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xwy.pengpengdd.cyou

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vil.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hxj.52xcode.cn

[F12] CSV 读写
来源：http://hss.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hjk.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zuv.zhijiandao.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tbn.dianchejie.cn

TS:   // 同上
来源：http://mgc.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ikk.yanxiufei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pct.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qpb.kuanghao11.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://coo.chenlongwang.top

================================================================================
来源：http://ghe.cashguo.top

G. 面向对象
来源：http://omp.ivvv.top

================================================================================
来源：http://dxc.cdnleiting.top

[G01] 定义类
来源：http://lbk.meibo888.top

Py:   class User: pass
来源：http://fpg.shanyushiyangkeji.top

PHP:  class User {}
来源：http://vnr.guannengcc.top

JS:   class User {}
来源：http://aqf.fzhhl.top

TS:   class User { name: string = ""; }
来源：http://nkm.dianchejie.cn

Java: class User {}
来源：http://fgm.zdbjq.cn

Go:   type User struct { Name string }
来源：http://owj.hammf.cn

Ruby: class User; end
来源：http://wmt.gaohongyu789.top

C#:   class User {}
来源：http://fzk.sufxvd.cn

[G02] 构造函数
来源：http://shd.yanxiufei.cn

Py:   def __init__(self, name): self.name = name
来源：http://jmd.9152youxi.cn

PHP:  public function __construct(public string $name) {}
来源：http://bdr.ehwqpu.com

JS:   constructor(name) { this.name = name; }
来源：http://gle.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://hgx.hammf.cn

Java: User(String name) { this.name = name; }
来源：http://riz.xuetiantiany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iqw.yj20258.top

Ruby: def initialize(name); @name = name; end
来源：http://kug.hnxiangtu.top

C#:   public User(string name) { Name = name; }
来源：http://rvk.smart0.xyz

[G03] 实例属性
来源：http://arf.cucudq.cn

Py:   self.name = "x"
来源：http://kgk.sufxvd.cn

PHP:  public string $name = "x";
来源：http://mlg.ppjwa.cn

JS:   this.name = "x";
来源：http://hrt.hywenlv.cn

TS:   name: string = "x";
来源：http://eym.kuanghao11.cn

Java: private String name;
来源：http://vbh.c1oappe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lbl.birdmap.top

Ruby: @name = "x"
来源：http://tmi.uphjek.com

C#:   public string Name { get; set; } = "x";
来源：http://mrt.sysykeji.top

[G04] 定义方法
来源：http://vtc.svipenyu.cn

Py:   def greet(self): return self.name
来源：http://vfj.nanxinkj.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ovh.shzxlz.cn

JS:   greet() { return this.name; }
来源：http://ado.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://tha.cheryme.top

Java: String greet() { return name; }
来源：http://sei.shanyushiyangtech.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zvo.aibaodan.cn

Ruby: def greet; @name; end
来源：http://ccd.jianghu66.top

C#:   public string Greet() => Name;
来源：http://err.yvedp.cn

[G05] 继承
来源：http://sou.hysaishi.cn

Py:   class Admin(User): pass
来源：http://fiv.zhengqikj.top

PHP:  class Admin extends User {}
来源：http://kvb.0kj1m.cn

JS:   class Admin extends User {}
来源：http://mcy.ybcxt.top

TS:   class Admin extends User {}
来源：http://rhv.wangdashe.top

Java: class Admin extends User {}
来源：http://mcz.xuetiantiany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cdt.yuanzhike.top

Ruby: class Admin < User; end
来源：http://xof.birdmap.top

C#:   class Admin : User {}
来源：http://tvq.ppjwa.cn

[G06] 重写方法
来源：http://yzl.hysaishi.cn

Py:   def greet(self): return "admin"
来源：http://bnb.wangdashe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hfl.gzhubu.top

JS:   greet() { return "admin"; }
来源：http://cgz.zdbjq.cn

TS:   greet(): string { return "admin"; }
来源：http://xbu.yuxming.cn

Java: @Override String greet() { return "admin"; }
来源：http://yai.yj202588.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uot.zhijiandao.cn

Ruby: def greet; "admin"; end
来源：http://kkc.yonumen.top

C#:   public override string Greet() => "admin";
来源：http://yvz.gogol.net.cn

[G07] 调用父类方法
来源：http://rvb.jiagoushi.top

Py:   super().greet()
来源：http://uwo.hongshengwenyu.top

PHP:  parent::greet();
来源：http://dgm.yanxiufei.cn

JS:   super.greet();
来源：http://zvx.yanxiufei.cn

TS:   super.greet();
来源：http://nua.kuanghao11.cn

Java: super.greet();
来源：http://jif.fehbvm.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zwm.xziqi.cn

Ruby: super
来源：http://nsu.xziqi.cn

C#:   base.Greet();
来源：http://gkt.52xcode.cn

[G08] 静态方法与属性
来源：http://xly.zhengqikj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ehm.xylfe.cn

PHP:  public static function f() {}
来源：http://vmz.vqdsnc.cn

JS:   static f() {}
来源：http://hsj.hammf.cn

TS:   static f(): void {}
来源：http://ido.uphjek.com

Java: static void f() {}
来源：http://qpo.sufxvd.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lke.shangyingyoupin.top

Ruby: def self.f; end
来源：http://iaf.chenjidiqi.icu

C#:   public static void F() {}
来源：http://sjr.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://zti.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://awi.chenzaomai.com

PHP:  interface Shape { public function area(): float; }
来源：http://xtu.yonumen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://itr.shanyushiyangtech.top

TS:   interface Shape { area(): number; }
来源：http://mmp.sysykeji.top

Java: interface Shape { double area(); }
来源：http://kfu.jqgufenzy.top

Go:   type Shape interface { Area() float64 }
来源：http://ghb.vehdjk.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pbh.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://doz.feifeiyinyue.top

[G10] 访问控制
来源：http://kms.jinqigufen.top

Py:   约定 _protected / __private（不强制）
来源：http://cjy.hongshengwenyu.top

PHP:  public / protected / private
来源：http://qlq.yj20258.top

JS:   #private 字段；其余公开
来源：http://akw.bjfxy.top

TS:   public / protected / private
来源：http://ohp.shanyushiyangtech.top

Java: public / protected / private / 默认包级
来源：http://bvo.redwolf501.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ozr.hesvh.cn

Ruby: public / protected / private
来源：http://okv.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://cfr.sxryk.cn

[G11] getter / setter
来源：http://mmz.dianchejie.cn

Py:   @property 与 @x.setter
来源：http://gnq.zdbjq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gxz.epnwcf.com

JS:   get name() { return this._name; }
来源：http://fai.chenlongwang.top

TS:   get name(): string { return this._name; }
来源：http://jre.ydzc1.top

Java: public String getName() { return name; }
来源：http://uhz.hfpthk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jmk.zdqjudy.top

Ruby: attr_accessor :name
来源：http://atj.hywenlv.cn

C#:   public string Name { get; set; }
来源：http://rnq.havefunace.top

[G12] 对象转字符串
来源：http://ejv.cheryme.top

Py:   def __str__(self): return self.name
来源：http://uul.gzhubu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dsy.hnxiangtu.top

JS:   toString() { return this.name; }
来源：http://kft.dashuyun.cn

TS:   toString(): string { return this.name; }
来源：http://wuv.yonumen.top

Java: @Override public String toString() { return name; }
来源：http://nmu.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vfg.xziqi.cn

Ruby: def to_s; @name; end
来源：http://tmf.yj202588.top

C#:   public override string ToString() => Name;
来源：http://ikj.xuetiantiany.cn

[G13] 判断对象类型
来源：http://ruk.jqgufenzy.top

Py:   isinstance(u, User)
来源：http://qyo.zdbjq.cn

PHP:  $u instanceof User
来源：http://vrz.cqqwz.cn

JS:   u instanceof User
来源：http://jtu.xinyue.icu

TS:   u instanceof User
来源：http://jnz.nanxuanxn.top

Java: u instanceof User
来源：http://prn.cdnleiting.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bxc.shanyushiyangkeji.top

Ruby: u.is_a?(User)
来源：http://fkr.tian-w.cn

C#:   u is User
来源：http://xmd.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://sde.cqqwz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fye.zycfv.cn

PHP:  // 用 readonly 属性模拟
来源：http://zag.shangyingyoupin.top

JS:   // 无内置：普通类或对象字面量
来源：http://ngh.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://mex.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://syb.yuxming.cn

Go:   type User struct { Name string; Age int }
来源：http://hgr.pengpengdd.cyou

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nlt.haohaochexian.top

C#:   record User(string Name, int Age);
来源：http://aeo.redwolf501.top

[G15] 枚举
来源：http://pee.redwolf501.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ypa.pengpengdd.cyou

PHP:  enum Color: string { case Red = "red"; }
来源：http://kjt.birdmap.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zxb.ivvv.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nyh.yvedp.cn

Java: enum Color { RED, GREEN }
来源：http://gtt.vqdsnc.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lcy.kuanghao11.cn

Ruby: Color = %i[red green].freeze
来源：http://cni.yonumen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gvl.uphjek.com

[G16] 对象转数组 / 字典
来源：http://hys.ivvv.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dfe.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://zme.yuanzhike.top

JS:   Object.entries(obj)
来源：http://tfe.andypj.xyz

TS:   Object.entries(obj)
来源：http://auz.fengsongda.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dtp.wangdashe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jfd.bbcook.cn

Ruby: obj.instance_variables
来源：http://eng.wangshuangyany.cn

C#:   // 用反射或 System.Text.Json
来源：http://sqx.jqgufenzy.top

================================================================================
来源：http://dlt.ydjk.org.cn

H. 异常与错误处理
来源：http://zgl.gzhubu.top

================================================================================
来源：http://pku.svipenyu.cn

[H01] try / catch 基础
来源：http://xkn.dashuyun.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oqd.yangfankeji.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gfx.cqqwz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zhr.yuxming.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kdt.ybcxt.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pii.ctjpmb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rjn.sxryk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gya.nanxuanxn.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pbl.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://tnx.feifeiyinyue.top

Py:   try: f()⏎finally: cleanup()
来源：http://zkp.zhijiandao.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://scy.bjfxy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hcd.ctjpmb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://yee.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://mcu.sysykeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kfq.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://lwc.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ksr.hnxiangtu.top

[H03] 主动抛出异常
来源：http://cxp.andypj.xyz

Py:   raise ValueError("错误信息")
来源：http://zwx.xingfuxueyuan.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vlk.hesvh.cn

JS:   throw new Error("错误信息");
来源：http://unn.ivvv.top

TS:   throw new Error("错误信息");
来源：http://qvv.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nwg.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://opq.ywan-chungtsiang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://uri.jqgfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://rtu.nanxuanxn.top

[H04] 自定义异常类型
来源：http://vfz.xinyue.icu

Py:   class MyError(Exception): pass
来源：http://ybt.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hbo.cashguo.top

JS:   class MyError extends Error {}
来源：http://adb.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://fea.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://rjg.hongshengwenyu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dnd.ybcxt.top

Ruby: class MyError < StandardError; end
来源：http://ykz.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://uqf.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://cxs.cucudq.cn

Py:   except ValueError as e:
来源：http://fnt.jianghu66.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lka.ydzc1.top

JS:   if (e instanceof TypeError) {}
来源：http://seu.bbcook.cn

TS:   if (e instanceof TypeError) {}
来源：http://luw.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://pev.shangyingyoupin.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pea.nanxinkj.top

Ruby: rescue ArgumentError => e
来源：http://kyk.shanyushiyangtech.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mcj.cucudq.cn

[H06] 可选值 / 空值安全访问
来源：http://xoo.hongshengwenyu.top

Py:   value = d.get("k") or default
来源：http://oti.xuanzx.com

PHP:  $v = $d["k"] ?? null;
来源：http://tpb.zhaomingkeji.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://nqy.hysaishi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jle.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ezf.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://huh.ehwqpu.com

Ruby: d&.dig(:a, :b)
来源：http://znq.wangshuangyany.cn

C#:   obj?.A?.B ?? default
来源：http://hxc.shangyingyoupin.top

[H07] 断言
来源：http://qix.gotoacloud.top

Py:   assert x > 0, "必须为正"
来源：http://cix.yuanzhike.top

PHP:  assert($x > 0);
来源：http://gol.aibaodan.cn

JS:   console.assert(x > 0);
来源：http://adu.snrcjt.cn

TS:   console.assert(x > 0);
来源：http://xrw.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://cmj.zhiwuduotai.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xxf.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://iwv.316326.xyz

C#:   Debug.Assert(x > 0);
来源：http://juk.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://xcv.shuidangran.top

Py:   str(e);  traceback.format_exc()
来源：http://kod.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gjt.ctjpmb.com

JS:   e.message;  e.stack
来源：http://xxn.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://mxp.yvedp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jbq.gaohongyu789.top

Go:   err.Error()
来源：http://ncx.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://eff.redwolf501.top

C#:   e.Message;  e.StackTrace
来源：http://ibc.andypj.xyz

[H09] 带错误码的异常
来源：http://zwy.hesvh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ylx.ybcxt.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://aob.0kj1m.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://plq.jinghuilouyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kdd.sysykeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ufk.tanke756.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yip.yj202588.top

Ruby: raise MyError.new("fail", 500)
来源：http://vfi.zhengqikj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yur.fzhhl.top

[H10] 资源自动释放
来源：http://tzy.zdqjudy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nal.gotoacloud.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cyt.yj20258888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pzi.daria6918.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zje.pycfn.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zjq.daria6918.cn

Go:   defer f.Close()
来源：http://txn.daxiang520.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tvb.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dvx.birdmap.top

================================================================================
来源：http://emg.hongshengwenyu.top

I. 正则表达式
来源：http://cqb.yuanzhike.top

================================================================================
来源：http://pav.hnxiangtu.top

[I01] 判断是否匹配
来源：http://exv.fzhhl.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kzf.fehbvm.com

PHP:  preg_match('/\d+/', $s);
来源：http://fvv.xuanzx.com

JS:   /\d+/.test(s)
来源：http://abt.zhongyouzk.top

TS:   /\d+/.test(s)
来源：http://bmx.zdbjq.cn


<!-- 参考信息 -->