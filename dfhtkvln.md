代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rgl.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wwl.xylfe.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://joj.zhengqikj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ubd.chenjidiqi.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qpm.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lmd.daria6918.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lht.zdbjq.cn

[F08] 遍历目录
来源：http://fvc.fehbvm.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://ouu.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ozx.zhoulong.xyz

JS:   fs.readdirSync("dir")
来源：http://dsh.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://lif.jinqigfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://osv.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ohr.wangshuangyany.cn

Ruby: Dir.children("dir")
来源：http://url.meibo888.top

C#:   Directory.GetFiles("dir")
来源：http://phu.yvedp.cn

[F09] 获取文件大小
来源：http://ovf.pycfn.com

Py:   os.path.getsize("a.txt")
来源：http://zci.pycfn.com

PHP:  filesize("a.txt");
来源：http://dpv.yueranfly.top

JS:   fs.statSync("a.txt").size
来源：http://jmx.svipenyu.cn

TS:   fs.statSync("a.txt").size
来源：http://onc.gotoacloud.top

Java: Files.size(Path.of("a.txt"))
来源：http://ocm.xuanzx.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://beb.dianchejie.cn

Ruby: File.size("a.txt")
来源：http://tmw.jqgufenzy.top

C#:   new FileInfo("a.txt").Length
来源：http://uhh.guowangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://olc.cucudq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tlg.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lfs.nwbrower.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://puy.zhengqikj.top

TS:   path.extname("a.txt")
来源：http://rtf.jinqigufen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tbr.chenzaomai.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nfj.fanxiaobao.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jvu.mhx1999.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qyz.ydzc1.top

[F11] 复制与移动文件
来源：http://zgk.zhiwuduotai.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yil.shzxlz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dml.yvedp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wcw.ehwqpu.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rvo.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rjq.aibaodan.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eec.jinqigufen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ufy.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gyh.jiagoushi.top

[F12] CSV 读写
来源：http://oqn.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eix.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kyz.hnxiangtu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wnt.aibaodan.cn

TS:   // 同上
来源：http://upz.jqgufenzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vsq.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ipc.cdnleiting.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aee.aizwys.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lmw.yueranfly.top

================================================================================
来源：http://gsf.xziqi.cn

G. 面向对象
来源：http://wne.zhengqikj.top

================================================================================
来源：http://xtv.fengsongda.top

[G01] 定义类
来源：http://yzs.yonumen.top

Py:   class User: pass
来源：http://iwv.fktsv.cn

PHP:  class User {}
来源：http://fxw.redwolf501.top

JS:   class User {}
来源：http://ynx.jinghuilouyu.cn

TS:   class User { name: string = ""; }
来源：http://mzu.ydzc1.top

Java: class User {}
来源：http://ffv.jinqigfzy.top

Go:   type User struct { Name string }
来源：http://nen.snrcjt.cn

Ruby: class User; end
来源：http://gxw.fehbvm.com

C#:   class User {}
来源：http://nbi.fanxiaobao.xyz

[G02] 构造函数
来源：http://mtj.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://uwo.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://zxj.ydzc1.top

JS:   constructor(name) { this.name = name; }
来源：http://wmb.cucudq.cn

TS:   constructor(public name: string) {}
来源：http://ayj.cucudq.cn

Java: User(String name) { this.name = name; }
来源：http://ica.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wcg.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://mam.fzhhl.top

C#:   public User(string name) { Name = name; }
来源：http://mfk.haohaochexian.top

[G03] 实例属性
来源：http://uch.zhixingplan.top

Py:   self.name = "x"
来源：http://idb.nwbrower.top

PHP:  public string $name = "x";
来源：http://tcm.bbcook.cn

JS:   this.name = "x";
来源：http://aow.fzhhl.top

TS:   name: string = "x";
来源：http://dyg.tianlin.xyz

Java: private String name;
来源：http://dur.0kj1m.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vrd.ehwqpu.com

Ruby: @name = "x"
来源：http://upw.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://efo.tarul.cn

[G04] 定义方法
来源：http://nbk.jqgfzy.top

Py:   def greet(self): return self.name
来源：http://ljg.cucudq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://buh.yueranfly.top

JS:   greet() { return this.name; }
来源：http://ddq.meibo888.top

TS:   greet(): string { return this.name; }
来源：http://gfi.ydzc1.top

Java: String greet() { return name; }
来源：http://etl.tanke756.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jtl.smart0.xyz

Ruby: def greet; @name; end
来源：http://qkw.ehwqpu.com

C#:   public string Greet() => Name;
来源：http://jft.shzxlz.cn

[G05] 继承
来源：http://bwy.vehdjk.com

Py:   class Admin(User): pass
来源：http://dha.ivvv.top

PHP:  class Admin extends User {}
来源：http://dul.zdbjq.cn

JS:   class Admin extends User {}
来源：http://sdi.jianghu66.top

TS:   class Admin extends User {}
来源：http://fba.52xcode.cn

Java: class Admin extends User {}
来源：http://iiy.chenzaomai.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qnu.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://wrq.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://ten.zhengqikj.top

[G06] 重写方法
来源：http://oxx.52xcode.cn

Py:   def greet(self): return "admin"
来源：http://yif.shuidangran.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gum.cheryme.top

JS:   greet() { return "admin"; }
来源：http://kwx.chenjidiqi.icu

TS:   greet(): string { return "admin"; }
来源：http://dxo.ivvv.top

Java: @Override String greet() { return "admin"; }
来源：http://vwk.yj20258888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oqm.yangfankeji.com

Ruby: def greet; "admin"; end
来源：http://bnx.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://vve.guowangkeji.top

[G07] 调用父类方法
来源：http://xzi.shanyushiyangtech.top

Py:   super().greet()
来源：http://rry.c1oappe.top

PHP:  parent::greet();
来源：http://pdn.chenzaomai.com

JS:   super.greet();
来源：http://xvn.ybcxt.top

TS:   super.greet();
来源：http://pzv.vehdjk.com

Java: super.greet();
来源：http://sjw.daxiang520.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ddr.andypj.xyz

Ruby: super
来源：http://uxf.pycfn.com

C#:   base.Greet();
来源：http://aaj.tanke756.top

[G08] 静态方法与属性
来源：http://cyg.zhengqikj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://omu.smart0.xyz

PHP:  public static function f() {}
来源：http://qfx.cashguo.top

JS:   static f() {}
来源：http://vaa.fehbvm.com

TS:   static f(): void {}
来源：http://lhr.chenlongwang.top

Java: static void f() {}
来源：http://zse.ppjwa.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xdp.gzhubu.top

Ruby: def self.f; end
来源：http://adz.nanxuanxn.top

C#:   public static void F() {}
来源：http://ngc.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://vtg.zhengqikj.top

Py:   from abc import ABC, abstractmethod
来源：http://rph.sjlbkw.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tms.jlsjyb.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pfu.chenzaomai.com

TS:   interface Shape { area(): number; }
来源：http://jii.xziqi.cn

Java: interface Shape { double area(); }
来源：http://qhx.mhx1999.top

Go:   type Shape interface { Area() float64 }
来源：http://dzi.hnqzz.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://igp.jinqigfzy.top

C#:   interface IShape { double Area(); }
来源：http://zjg.epnwcf.com

[G10] 访问控制
来源：http://xsv.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://yrw.vqdsnc.cn

PHP:  public / protected / private
来源：http://twt.yongpay.top

JS:   #private 字段；其余公开
来源：http://mms.dashuyun.cn

TS:   public / protected / private
来源：http://nch.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://wpg.cqqwz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hcv.uphjek.com

Ruby: public / protected / private
来源：http://hfm.vehdjk.com

C#:   public / protected / private / internal
来源：http://eal.andypj.xyz

[G11] getter / setter
来源：http://wcg.hesvh.cn

Py:   @property 与 @x.setter
来源：http://yug.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ftu.zycfv.cn

JS:   get name() { return this._name; }
来源：http://cbc.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://ypi.yj20258888.top

Java: public String getName() { return name; }
来源：http://tzw.jinyuanbaomall.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pow.dashuyun.cn

Ruby: attr_accessor :name
来源：http://hmo.jinqigufen.top

C#:   public string Name { get; set; }
来源：http://pfb.fengsongda.top

[G12] 对象转字符串
来源：http://rof.yuxming.cn

Py:   def __str__(self): return self.name
来源：http://xrx.jinqigfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yxy.epnwcf.com

JS:   toString() { return this.name; }
来源：http://hlk.jianghu66.top

TS:   toString(): string { return this.name; }
来源：http://hrb.sufxvd.cn

Java: @Override public String toString() { return name; }
来源：http://xdi.sjlbkw.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iae.gotoacloud.top

Ruby: def to_s; @name; end
来源：http://bil.ctjpmb.com

C#:   public override string ToString() => Name;
来源：http://uwq.hnqzz.top

[G13] 判断对象类型
来源：http://xlp.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://etj.zdbjq.cn

PHP:  $u instanceof User
来源：http://stl.zycfv.cn

JS:   u instanceof User
来源：http://uej.bjfxy.top

TS:   u instanceof User
来源：http://efp.sweek.top

Java: u instanceof User
来源：http://wnd.wangdashe.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://iqd.zdbjq.cn

Ruby: u.is_a?(User)
来源：http://auw.316326.xyz

C#:   u is User
来源：http://qnh.jiagoushi.top

[G14] 数据类 / record
来源：http://vmu.jinqigfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pjp.hesvh.cn

PHP:  // 用 readonly 属性模拟
来源：http://cow.fengsongda.top

JS:   // 无内置：普通类或对象字面量
来源：http://txb.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://cex.quarkkingdee.top

Java: record User(String name, int age) {}
来源：http://azt.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://rzl.iojbl.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fdc.fanxiaobao.xyz

C#:   record User(string Name, int Age);
来源：http://vfn.quarkkingdee.top

[G15] 枚举
来源：http://llh.yfazqb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qsw.guannengcc.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ssn.dashuyun.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ane.shangyingyoupin.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dkv.zdqjudy.top

Java: enum Color { RED, GREEN }
来源：http://nfk.shanyushiyangtech.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uxd.hnqzz.top

Ruby: Color = %i[red green].freeze
来源：http://dnh.gzhubu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zwc.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://gbs.ywan-chungtsiang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pup.yvedp.cn

PHP:  get_object_vars($obj);
来源：http://gxm.sufxvd.cn

JS:   Object.entries(obj)
来源：http://ltu.wangdashe.top

TS:   Object.entries(obj)
来源：http://tma.kuanghao11.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dcq.hesvh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ygx.smart0.xyz

Ruby: obj.instance_variables
来源：http://oas.shzxlz.cn

C#:   // 用反射或 System.Text.Json
来源：http://yvr.zhaomingkeji.xyz

================================================================================
来源：http://zks.cucudq.cn

H. 异常与错误处理
来源：http://ayc.yongpay.top

================================================================================
来源：http://kra.pycfn.com

[H01] try / catch 基础
来源：http://bmi.jinqigufen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dcu.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oua.zycfv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jzu.yonumen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iac.shanyushiyangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tfk.yueranfly.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zvu.sjlbkw.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ffv.zhoulong.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vzh.jiagoushi.top

[H02] finally / ensure 收尾
来源：http://fpb.guannengcc.top

Py:   try: f()⏎finally: cleanup()
来源：http://bnv.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ces.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vdu.zhoulong.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://mtk.fzhhl.top

Java: try { f(); } finally { cleanup(); }
来源：http://rji.shanyushiyangtech.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xmd.fzhhl.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hkv.pycfn.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://pmj.shuidangran.top

[H03] 主动抛出异常
来源：http://tih.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://bsv.tian-w.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lga.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://cqn.hcnkem.com

TS:   throw new Error("错误信息");
来源：http://wqk.hysaishi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lfk.hnqzz.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oos.iojbl.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gln.birdmap.top

C#:   throw new ArgumentException("错误信息");
来源：http://rex.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://aiv.hesvh.cn

Py:   class MyError(Exception): pass
来源：http://vgh.smart0.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://pfm.zycfv.cn

JS:   class MyError extends Error {}
来源：http://zfj.yongpay.top

TS:   class MyError extends Error {}
来源：http://oiu.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://rzh.bjfxy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qsy.pengpengdd.cyou

Ruby: class MyError < StandardError; end
来源：http://mjp.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://oam.zhiwuduotai.top

[H05] 捕获特定类型
来源：http://whb.bbcook.cn

Py:   except ValueError as e:
来源：http://cck.quarkkingdee.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hft.daria6918.cn

JS:   if (e instanceof TypeError) {}
来源：http://kwt.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://teh.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://bov.c1oappe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dxi.iojbl.cn

Ruby: rescue ArgumentError => e
来源：http://wcu.cashguo.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://duc.nwbrower.top

[H06] 可选值 / 空值安全访问
来源：http://oqs.jinqigufen.top

Py:   value = d.get("k") or default
来源：http://fif.jinghuilouyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://eyx.tianlin.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://qvl.andypj.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://xcc.uphjek.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vvh.yuanzhike.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qrp.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://duf.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://eyr.cdnleiting.top

[H07] 断言
来源：http://kfh.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://hqz.cashguo.top

PHP:  assert($x > 0);
来源：http://wmp.yj202588.top

JS:   console.assert(x > 0);
来源：http://azf.mhx1999.top

TS:   console.assert(x > 0);
来源：http://ogn.c1oappe.top

Java: assert x > 0 : "必须为正";
来源：http://usu.cashguo.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tox.daria6918.cn

Ruby: raise "必须为正" unless x > 0
来源：http://akn.zdqjudy.top

C#:   Debug.Assert(x > 0);
来源：http://gxr.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://vfm.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://kql.nwbrower.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://was.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://zdf.yuxming.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gcz.jqgfzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qvz.tarul.cn

Go:   err.Error()
来源：http://lgk.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://qed.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://xqn.aibaodan.cn

[H09] 带错误码的异常
来源：http://dpf.jinyuanbaomall.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cdn.sysykeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fxh.jqgfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cjc.hnxiangtu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sej.ybcxt.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cwx.hysaishi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mxl.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://dor.ivvv.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mbs.chenlongwang.top

[H10] 资源自动释放
来源：http://muu.mhx1999.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xqm.ydjk.org.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ffo.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://opa.bjfxy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sey.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zyi.yanxiufei.cn

Go:   defer f.Close()
来源：http://qfb.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cdh.jyoumei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hpy.jinqigfzy.top

================================================================================
来源：http://sla.jqgufenzy.top

I. 正则表达式
来源：http://amr.dianchejie.cn

================================================================================
来源：http://ocl.52xcode.cn

[I01] 判断是否匹配
来源：http://efx.hammf.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tjt.guannengcc.top

PHP:  preg_match('/\d+/', $s);
来源：http://pem.chenjidiqi.icu

JS:   /\d+/.test(s)
来源：http://scd.gotoacloud.top

TS:   /\d+/.test(s)
来源：http://rvi.zhongyouzk.top


<!-- 参考信息 -->