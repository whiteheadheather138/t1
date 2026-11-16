代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://yjb.hongshengwenyu.top

TS:   fs.unlinkSync("a.txt")
来源：http://khe.zhaomingkeji.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fvd.sjlbkw.cn

Go:   os.Remove("a.txt")
来源：http://kbj.redwolf501.top

Ruby: File.delete("a.txt")
来源：http://ohe.pycfn.com

C#:   File.Delete("a.txt");
来源：http://oix.ydjk.org.cn

[F07] 创建目录（含多级）
来源：http://nhu.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ifx.fktsv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://upx.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mfq.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iig.zhoulong.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xlg.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tuq.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nsy.c1oappe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gth.cucudq.cn

[F08] 遍历目录
来源：http://apf.cashguo.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://sfa.daxiang520.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dvx.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://aln.uphjek.com

TS:   fs.readdirSync("dir")
来源：http://vzu.tarul.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cwh.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zvq.nwbrower.top

Ruby: Dir.children("dir")
来源：http://dfv.bjfxy.top

C#:   Directory.GetFiles("dir")
来源：http://ugt.yonumen.top

[F09] 获取文件大小
来源：http://biz.nwbrower.top

Py:   os.path.getsize("a.txt")
来源：http://cpc.ivvv.top

PHP:  filesize("a.txt");
来源：http://dok.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://uay.hywenlv.cn

TS:   fs.statSync("a.txt").size
来源：http://wjz.ydjk.org.cn

Java: Files.size(Path.of("a.txt"))
来源：http://har.feifeiyinyue.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lkh.zycfv.cn

Ruby: File.size("a.txt")
来源：http://bdq.tarul.cn

C#:   new FileInfo("a.txt").Length
来源：http://wqj.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://evd.smart0.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hpo.jyoumei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lgr.shanyushiyangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zra.sweek.top

TS:   path.extname("a.txt")
来源：http://ume.fehbvm.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vki.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zhz.jyoumei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hmo.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zta.shuidangran.top

[F11] 复制与移动文件
来源：http://dwp.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ztp.tanke756.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zuc.uphjek.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gzq.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vwu.jqgfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zty.yj20258888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://anw.9152youxi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qgq.xuanzx.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://drb.quarkkingdee.top

[F12] CSV 读写
来源：http://mtw.ppjwa.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rzo.ydjk.org.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nxy.iojbl.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fjq.zhijiandao.cn

TS:   // 同上
来源：http://rkh.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ler.sysykeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://alv.jlsjyb.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rln.tarul.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://myl.yongpay.top

================================================================================
来源：http://bdr.guannengcc.top

G. 面向对象
来源：http://oli.zhengqikj.top

================================================================================
来源：http://xwm.vehdjk.com

[G01] 定义类
来源：http://rne.daxiang520.top

Py:   class User: pass
来源：http://kmo.meibo888.top

PHP:  class User {}
来源：http://hzs.epnwcf.com

JS:   class User {}
来源：http://jhf.wangshuangyany.cn

TS:   class User { name: string = ""; }
来源：http://wib.fktsv.cn

Java: class User {}
来源：http://bgj.tian-w.cn

Go:   type User struct { Name string }
来源：http://dtd.smart0.xyz

Ruby: class User; end
来源：http://gpx.yangfankeji.com

C#:   class User {}
来源：http://pgm.ctjpmb.com

[G02] 构造函数
来源：http://siy.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://qkt.hnqzz.top

PHP:  public function __construct(public string $name) {}
来源：http://jkz.feifeiyinyue.top

JS:   constructor(name) { this.name = name; }
来源：http://yjs.jqgfzy.top

TS:   constructor(public name: string) {}
来源：http://pef.smart0.xyz

Java: User(String name) { this.name = name; }
来源：http://ake.gotoacloud.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lgt.zdqjudy.top

Ruby: def initialize(name); @name = name; end
来源：http://cpu.jinyuanbaomall.cn

C#:   public User(string name) { Name = name; }
来源：http://wvr.jinyuanbaomall.cn

[G03] 实例属性
来源：http://crh.yvedp.cn

Py:   self.name = "x"
来源：http://xim.jyoumei.cn

PHP:  public string $name = "x";
来源：http://pez.sjlbkw.cn

JS:   this.name = "x";
来源：http://bma.hcnkem.com

TS:   name: string = "x";
来源：http://jqh.cucudq.cn

Java: private String name;
来源：http://bub.xingfuxueyuan.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xil.jiagoushi.top

Ruby: @name = "x"
来源：http://osn.meibo888.top

C#:   public string Name { get; set; } = "x";
来源：http://xss.zhaomingkeji.xyz

[G04] 定义方法
来源：http://dtq.daxiang520.top

Py:   def greet(self): return self.name
来源：http://oiy.jqgufenzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mic.yj20258.top

JS:   greet() { return this.name; }
来源：http://rnh.jlsjyb.cn

TS:   greet(): string { return this.name; }
来源：http://qbh.daxiang520.top

Java: String greet() { return name; }
来源：http://smf.tarul.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://igo.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://dsc.guowangkeji.top

C#:   public string Greet() => Name;
来源：http://yqp.chenzaomai.com

[G05] 继承
来源：http://uid.tian-w.cn

Py:   class Admin(User): pass
来源：http://ewf.hywenlv.cn

PHP:  class Admin extends User {}
来源：http://jrx.xylfe.cn

JS:   class Admin extends User {}
来源：http://gaz.zhaomingkeji.xyz

TS:   class Admin extends User {}
来源：http://olh.c1oappe.top

Java: class Admin extends User {}
来源：http://ryh.cdnleiting.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xtu.cqqwz.cn

Ruby: class Admin < User; end
来源：http://aqv.hcnkem.com

C#:   class Admin : User {}
来源：http://yhw.wangdashe.top

[G06] 重写方法
来源：http://uxp.jinqigfzy.top

Py:   def greet(self): return "admin"
来源：http://mdz.cucudq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jbe.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://hps.zhoulong.xyz

TS:   greet(): string { return "admin"; }
来源：http://uhp.jianghu66.top

Java: @Override String greet() { return "admin"; }
来源：http://rde.yanxiufei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dsa.shanyushiyangkeji.top

Ruby: def greet; "admin"; end
来源：http://jgi.jinghuilouyu.cn

C#:   public override string Greet() => "admin";
来源：http://rvc.shanyushiyangkeji.top

[G07] 调用父类方法
来源：http://twi.hammf.cn

Py:   super().greet()
来源：http://qtl.xziqi.cn

PHP:  parent::greet();
来源：http://jmz.smart0.xyz

JS:   super.greet();
来源：http://ecm.aibaodan.cn

TS:   super.greet();
来源：http://aer.xuetiantiany.cn

Java: super.greet();
来源：http://fer.tarul.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dqn.pengpengdd.cyou

Ruby: super
来源：http://iai.jinqigfzy.top

C#:   base.Greet();
来源：http://sgu.vehdjk.com

[G08] 静态方法与属性
来源：http://nbf.yuanzhike.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fuq.tanke756.top

PHP:  public static function f() {}
来源：http://mbw.ppjwa.cn

JS:   static f() {}
来源：http://ctu.ehwqpu.com

TS:   static f(): void {}
来源：http://ntu.jinqigufen.top

Java: static void f() {}
来源：http://why.dashuyun.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uyq.uphjek.com

Ruby: def self.f; end
来源：http://fvd.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://wdk.epnwcf.com

[G09] 接口 / 抽象类
来源：http://mfz.jianghu66.top

Py:   from abc import ABC, abstractmethod
来源：http://bsr.ivvv.top

PHP:  interface Shape { public function area(): float; }
来源：http://khk.xziqi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tic.birdmap.top

TS:   interface Shape { area(): number; }
来源：http://zek.tarul.cn

Java: interface Shape { double area(); }
来源：http://ojk.jqgufenzy.top

Go:   type Shape interface { Area() float64 }
来源：http://mlx.hcnkem.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xkv.yangfankeji.com

C#:   interface IShape { double Area(); }
来源：http://vca.meibo888.top

[G10] 访问控制
来源：http://zgu.chenlongwang.top

Py:   约定 _protected / __private（不强制）
来源：http://sla.tian-w.cn

PHP:  public / protected / private
来源：http://pmz.aibaodan.cn

JS:   #private 字段；其余公开
来源：http://bnc.yj20258888.top

TS:   public / protected / private
来源：http://oft.gzhubu.top

Java: public / protected / private / 默认包级
来源：http://jtr.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://jef.zhixingplan.top

Ruby: public / protected / private
来源：http://pqr.hongshengwenyu.top

C#:   public / protected / private / internal
来源：http://gzl.quarkkingdee.top

[G11] getter / setter
来源：http://tgr.gaohongyu789.top

Py:   @property 与 @x.setter
来源：http://vqw.hnqzz.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vtb.pycfn.com

JS:   get name() { return this._name; }
来源：http://bnd.haohaochexian.top

TS:   get name(): string { return this._name; }
来源：http://tnl.pycfn.com

Java: public String getName() { return name; }
来源：http://ubu.chenzaomai.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ihs.birdmap.top

Ruby: attr_accessor :name
来源：http://poh.yvedp.cn

C#:   public string Name { get; set; }
来源：http://qal.zhiwuduotai.top

[G12] 对象转字符串
来源：http://adm.jyoumei.cn

Py:   def __str__(self): return self.name
来源：http://iwx.andypj.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://akq.daxiang520.top

JS:   toString() { return this.name; }
来源：http://kdb.epnwcf.com

TS:   toString(): string { return this.name; }
来源：http://wkt.shzxlz.cn

Java: @Override public String toString() { return name; }
来源：http://twi.shangyingyoupin.top

Go:   func (u User) String() string { return u.Name }
来源：http://ahf.haohaochexian.top

Ruby: def to_s; @name; end
来源：http://xhq.yj202588.top

C#:   public override string ToString() => Name;
来源：http://lvj.sjlbkw.cn

[G13] 判断对象类型
来源：http://yzl.gaohongyu789.top

Py:   isinstance(u, User)
来源：http://xoj.fengsongda.top

PHP:  $u instanceof User
来源：http://ehi.nanxuanxn.top

JS:   u instanceof User
来源：http://bbv.hcnkem.com

TS:   u instanceof User
来源：http://pgp.xinyue.icu

Java: u instanceof User
来源：http://mhn.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://omu.mhx1999.top

Ruby: u.is_a?(User)
来源：http://koj.smart0.xyz

C#:   u is User
来源：http://gav.cucudq.cn

[G14] 数据类 / record
来源：http://pif.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rrx.hcnkem.com

PHP:  // 用 readonly 属性模拟
来源：http://fto.jinghuilouyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tiw.zdbjq.cn

TS:   type User = { name: string; age: number };
来源：http://ozf.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://vom.yfazqb.com

Go:   type User struct { Name string; Age int }
来源：http://fov.nanxinkj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yrd.hfpthk.cn

C#:   record User(string Name, int Age);
来源：http://gix.ivvv.top

[G15] 枚举
来源：http://pjg.chenlongwang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kcs.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://ksp.yanxiufei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vvc.0kj1m.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kxh.chenzaomai.com

Java: enum Color { RED, GREEN }
来源：http://mpf.redwolf501.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kxv.shanyushiyangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://xjt.ybcxt.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eso.ctjpmb.com

[G16] 对象转数组 / 字典
来源：http://zbi.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uyu.fanxiaobao.xyz

PHP:  get_object_vars($obj);
来源：http://zjj.vqdsnc.cn

JS:   Object.entries(obj)
来源：http://ehg.cucudq.cn

TS:   Object.entries(obj)
来源：http://naj.jinyuanbaomall.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ozs.yuanzhike.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qyk.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://yzk.gaohongyu789.top

C#:   // 用反射或 System.Text.Json
来源：http://gfv.shanyushiyangkeji.top

================================================================================
来源：http://mcx.cashguo.top

H. 异常与错误处理
来源：http://yzi.316326.xyz

================================================================================
来源：http://ave.c1oappe.top

[H01] try / catch 基础
来源：http://qgh.yj20258888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gil.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zmg.cqqwz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zzo.xinyue.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hcy.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xea.tian-w.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cez.cheryme.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ukm.vehdjk.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qwa.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://lxz.yangfankeji.com

Py:   try: f()⏎finally: cleanup()
来源：http://tox.hcnkem.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://bpn.jqgfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://aof.chenjidiqi.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://ztk.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sfw.sxryk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qqf.aibaodan.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://aqc.kuanghao11.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nvx.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://ssn.chenzaomai.com

Py:   raise ValueError("错误信息")
来源：http://anv.kuanghao11.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wao.jinyuanbaomall.cn

JS:   throw new Error("错误信息");
来源：http://ysk.gotoacloud.top

TS:   throw new Error("错误信息");
来源：http://joq.ybcxt.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ivr.daria6918.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vck.jqgufenzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://agn.yueranfly.top

C#:   throw new ArgumentException("错误信息");
来源：http://fxw.epnwcf.com

[H04] 自定义异常类型
来源：http://wij.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://gvl.tanke756.top

PHP:  class MyError extends RuntimeException {}
来源：http://lny.gaohongyu789.top

JS:   class MyError extends Error {}
来源：http://ywv.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://wmj.kuanghao11.cn

Java: class MyException extends RuntimeException {}
来源：http://rqg.shzxlz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ulu.xuanzx.com

Ruby: class MyError < StandardError; end
来源：http://itk.bjfxy.top

C#:   class MyException : Exception {}
来源：http://zkq.hnxiangtu.top

[H05] 捕获特定类型
来源：http://mzc.xinyue.icu

Py:   except ValueError as e:
来源：http://xpk.aibaodan.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mhj.316326.xyz

JS:   if (e instanceof TypeError) {}
来源：http://scs.316326.xyz

TS:   if (e instanceof TypeError) {}
来源：http://ney.shangyingyoupin.top

Java: catch (IOException | SQLException e) {}
来源：http://nsr.vqdsnc.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tth.jinghuilouyu.cn

Ruby: rescue ArgumentError => e
来源：http://hwr.jqgufenzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ahp.pycfn.com

[H06] 可选值 / 空值安全访问
来源：http://osn.svipenyu.cn

Py:   value = d.get("k") or default
来源：http://rnp.sweek.top

PHP:  $v = $d["k"] ?? null;
来源：http://xdq.shuidangran.top

JS:   obj?.a?.b;  d ?? default
来源：http://hyw.fehbvm.com

TS:   obj?.a?.b;  d ?? default
来源：http://tov.dashuyun.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ahy.hesvh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xkz.hammf.cn

Ruby: d&.dig(:a, :b)
来源：http://ylv.gogol.net.cn

C#:   obj?.A?.B ?? default
来源：http://pgq.daria6918.cn

[H07] 断言
来源：http://muu.hongshengwenyu.top

Py:   assert x > 0, "必须为正"
来源：http://pkm.birdmap.top

PHP:  assert($x > 0);
来源：http://spr.fzhhl.top

JS:   console.assert(x > 0);
来源：http://dzy.fengsongda.top

TS:   console.assert(x > 0);
来源：http://srm.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://xxt.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wzw.vehdjk.com

Ruby: raise "必须为正" unless x > 0
来源：http://bts.hcnkem.com

C#:   Debug.Assert(x > 0);
来源：http://ubg.jinyuanbaomall.cn

[H08] 获取错误信息与堆栈
来源：http://elh.zhixingplan.top

Py:   str(e);  traceback.format_exc()
来源：http://eai.meibo888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://omz.cheryme.top

JS:   e.message;  e.stack
来源：http://enb.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://txs.shanyushiyangtech.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lty.ctjpmb.com

Go:   err.Error()
来源：http://btu.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://cse.shuidangran.top

C#:   e.Message;  e.StackTrace
来源：http://meh.chenjidiqi.icu

[H09] 带错误码的异常
来源：http://jtp.tian-w.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cov.quarkkingdee.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tzm.ivvv.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tgb.yj20258.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://knl.vqdsnc.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gzy.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://imc.sysykeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://acd.hywenlv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pub.nanxuanxn.top

[H10] 资源自动释放
来源：http://nwh.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hux.wangdashe.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yxb.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ivt.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bln.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://apz.316326.xyz

Go:   defer f.Close()
来源：http://gos.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bfg.bbcook.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eyl.ehwqpu.com


<!-- 参考信息 -->