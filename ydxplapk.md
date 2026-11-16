代发 wailian999

Ruby: File.delete("a.txt")
来源：http://jcc.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://msv.fktsv.cn

[F07] 创建目录（含多级）
来源：http://dzi.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vyv.jlsjyb.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yzc.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yuz.andypj.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://erm.cheryme.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://djb.dianchejie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zqi.meibo888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nlf.yongpay.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yqg.fktsv.cn

[F08] 遍历目录
来源：http://ook.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mnr.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hjr.yueranfly.top

JS:   fs.readdirSync("dir")
来源：http://rdm.vehdjk.com

TS:   fs.readdirSync("dir")
来源：http://foq.jinqigufen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mwj.aizwys.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sst.shuidangran.top

Ruby: Dir.children("dir")
来源：http://syt.cdnleiting.top

C#:   Directory.GetFiles("dir")
来源：http://oli.sjlbkw.cn

[F09] 获取文件大小
来源：http://yql.birdmap.top

Py:   os.path.getsize("a.txt")
来源：http://caj.ydzc1.top

PHP:  filesize("a.txt");
来源：http://esp.fzhhl.top

JS:   fs.statSync("a.txt").size
来源：http://bwe.meibo888.top

TS:   fs.statSync("a.txt").size
来源：http://pga.zhijiandao.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dpf.zdbjq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zuw.yuxming.cn

Ruby: File.size("a.txt")
来源：http://rkg.aibaodan.cn

C#:   new FileInfo("a.txt").Length
来源：http://gqe.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://yii.aibaodan.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sia.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qxo.cheryme.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gds.sjlbkw.cn

TS:   path.extname("a.txt")
来源：http://enb.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vcq.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lrx.daria6918.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lrv.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wlv.jinqigfzy.top

[F11] 复制与移动文件
来源：http://ffa.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qzm.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pre.yonumen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aww.daria6918.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jzq.nanxuanxn.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ejz.xylfe.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jay.chenjidiqi.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wgd.jinyuanbaomall.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vti.ehwqpu.com

[F12] CSV 读写
来源：http://yeu.jlsjyb.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ths.daxiang520.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rtd.birdmap.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://niv.kuanghao11.cn

TS:   // 同上
来源：http://aew.tianlin.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oyk.jqgfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rfu.yj20258.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ypo.9152youxi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rus.mhx1999.top

================================================================================
来源：http://oba.fehbvm.com

G. 面向对象
来源：http://jle.chenzaomai.com

================================================================================
来源：http://rqk.fehbvm.com

[G01] 定义类
来源：http://jsu.zhengqikj.top

Py:   class User: pass
来源：http://ind.gzhubu.top

PHP:  class User {}
来源：http://djn.pengpengdd.cyou

JS:   class User {}
来源：http://mns.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://mqg.wangshuangyany.cn

Java: class User {}
来源：http://kzn.tarul.cn

Go:   type User struct { Name string }
来源：http://rlj.yongpay.top

Ruby: class User; end
来源：http://lwn.zdbjq.cn

C#:   class User {}
来源：http://jzz.yuxming.cn

[G02] 构造函数
来源：http://jfp.xuetiantiany.cn

Py:   def __init__(self, name): self.name = name
来源：http://nrg.meibo888.top

PHP:  public function __construct(public string $name) {}
来源：http://tlz.hnqzz.top

JS:   constructor(name) { this.name = name; }
来源：http://zrf.fehbvm.com

TS:   constructor(public name: string) {}
来源：http://bub.hcnkem.com

Java: User(String name) { this.name = name; }
来源：http://qcv.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zcn.bjfxy.top

Ruby: def initialize(name); @name = name; end
来源：http://wnw.wangdashe.top

C#:   public User(string name) { Name = name; }
来源：http://juw.hesvh.cn

[G03] 实例属性
来源：http://vld.haohaochexian.top

Py:   self.name = "x"
来源：http://pxv.fanxiaobao.xyz

PHP:  public string $name = "x";
来源：http://ttm.tarul.cn

JS:   this.name = "x";
来源：http://onu.fktsv.cn

TS:   name: string = "x";
来源：http://jsm.jinqigfzy.top

Java: private String name;
来源：http://lgb.smart0.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://joa.ydjk.org.cn

Ruby: @name = "x"
来源：http://opa.hnqzz.top

C#:   public string Name { get; set; } = "x";
来源：http://xbf.xziqi.cn

[G04] 定义方法
来源：http://xxh.jianghu66.top

Py:   def greet(self): return self.name
来源：http://iyc.hcnkem.com

PHP:  public function greet(): string { return $this->name; }
来源：http://wrc.jyoumei.cn

JS:   greet() { return this.name; }
来源：http://ukt.cdnleiting.top

TS:   greet(): string { return this.name; }
来源：http://njo.c1oappe.top

Java: String greet() { return name; }
来源：http://sma.xingfuxueyuan.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://wzo.epnwcf.com

Ruby: def greet; @name; end
来源：http://uig.jqgufenzy.top

C#:   public string Greet() => Name;
来源：http://hip.fktsv.cn

[G05] 继承
来源：http://ibu.nanxuanxn.top

Py:   class Admin(User): pass
来源：http://hfz.vehdjk.com

PHP:  class Admin extends User {}
来源：http://btl.jqgufenzy.top

JS:   class Admin extends User {}
来源：http://xcu.birdmap.top

TS:   class Admin extends User {}
来源：http://rfs.jinqigfzy.top

Java: class Admin extends User {}
来源：http://kcr.shangyingyoupin.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zxm.0kj1m.cn

Ruby: class Admin < User; end
来源：http://wny.svipenyu.cn

C#:   class Admin : User {}
来源：http://zcj.xinyue.icu

[G06] 重写方法
来源：http://jzu.hesvh.cn

Py:   def greet(self): return "admin"
来源：http://zwm.gogol.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://anz.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://wjm.meibo888.top

TS:   greet(): string { return "admin"; }
来源：http://rae.bbcook.cn

Java: @Override String greet() { return "admin"; }
来源：http://cup.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://syc.cheryme.top

Ruby: def greet; "admin"; end
来源：http://bvh.sjlbkw.cn

C#:   public override string Greet() => "admin";
来源：http://zbi.meibo888.top

[G07] 调用父类方法
来源：http://mcw.ybcxt.top

Py:   super().greet()
来源：http://eex.andypj.xyz

PHP:  parent::greet();
来源：http://xla.chenzaomai.com

JS:   super.greet();
来源：http://vqc.epnwcf.com

TS:   super.greet();
来源：http://eqk.sysykeji.top

Java: super.greet();
来源：http://hck.zhixingplan.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bhg.zhaomingkeji.xyz

Ruby: super
来源：http://pqx.daria6918.cn

C#:   base.Greet();
来源：http://xlo.sufxvd.cn

[G08] 静态方法与属性
来源：http://ruv.wangdashe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mad.gaohongyu789.top

PHP:  public static function f() {}
来源：http://otn.bbcook.cn

JS:   static f() {}
来源：http://nnx.hnxiangtu.top

TS:   static f(): void {}
来源：http://wfd.jqgufenzy.top

Java: static void f() {}
来源：http://uan.52xcode.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eim.xziqi.cn

Ruby: def self.f; end
来源：http://cws.hesvh.cn

C#:   public static void F() {}
来源：http://tku.ybcxt.top

[G09] 接口 / 抽象类
来源：http://bev.xingfuxueyuan.xyz

Py:   from abc import ABC, abstractmethod
来源：http://xmr.bbcook.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ixt.yuanzhike.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xub.hongshengwenyu.top

TS:   interface Shape { area(): number; }
来源：http://orr.nanxinkj.top

Java: interface Shape { double area(); }
来源：http://qzd.smart0.xyz

Go:   type Shape interface { Area() float64 }
来源：http://mdj.cashguo.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vzf.dashuyun.cn

C#:   interface IShape { double Area(); }
来源：http://mwk.feifeiyinyue.top

[G10] 访问控制
来源：http://rac.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://ghl.jqgfzy.top

PHP:  public / protected / private
来源：http://qvx.quarkkingdee.top

JS:   #private 字段；其余公开
来源：http://pty.meibo888.top

TS:   public / protected / private
来源：http://xuc.zhixingplan.top

Java: public / protected / private / 默认包级
来源：http://zyn.vehdjk.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://kac.pengpengdd.cyou

Ruby: public / protected / private
来源：http://anj.snrcjt.cn

C#:   public / protected / private / internal
来源：http://hdf.hongshengwenyu.top

[G11] getter / setter
来源：http://pzy.sufxvd.cn

Py:   @property 与 @x.setter
来源：http://grs.svipenyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yjw.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://fqx.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://urd.jinyuanbaomall.cn

Java: public String getName() { return name; }
来源：http://twy.smart0.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://kew.redwolf501.top

Ruby: attr_accessor :name
来源：http://aen.yj20258888.top

C#:   public string Name { get; set; }
来源：http://bzn.hywenlv.cn

[G12] 对象转字符串
来源：http://uxx.52xcode.cn

Py:   def __str__(self): return self.name
来源：http://vma.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://uca.guowangkeji.top

JS:   toString() { return this.name; }
来源：http://rcx.cucudq.cn

TS:   toString(): string { return this.name; }
来源：http://dcl.yuanzhike.top

Java: @Override public String toString() { return name; }
来源：http://dvf.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://ctm.hywenlv.cn

Ruby: def to_s; @name; end
来源：http://rqa.zdbjq.cn

C#:   public override string ToString() => Name;
来源：http://gze.zdqjudy.top

[G13] 判断对象类型
来源：http://atf.shangyingyoupin.top

Py:   isinstance(u, User)
来源：http://gou.hfpthk.cn

PHP:  $u instanceof User
来源：http://nhg.chenjidiqi.icu

JS:   u instanceof User
来源：http://kfk.pycfn.com

TS:   u instanceof User
来源：http://kxo.xziqi.cn

Java: u instanceof User
来源：http://vih.aizwys.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fql.epnwcf.com

Ruby: u.is_a?(User)
来源：http://war.hywenlv.cn

C#:   u is User
来源：http://kay.epnwcf.com

[G14] 数据类 / record
来源：http://xgn.tianlin.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sht.yj20258.top

PHP:  // 用 readonly 属性模拟
来源：http://btq.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://oib.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://wxy.redwolf501.top

Java: record User(String name, int age) {}
来源：http://axj.0kj1m.cn

Go:   type User struct { Name string; Age int }
来源：http://rrt.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://swv.yanxiufei.cn

C#:   record User(string Name, int Age);
来源：http://lfj.ybcxt.top

[G15] 枚举
来源：http://gce.hnxiangtu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bkg.yj202588.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://blh.sjlbkw.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sik.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pzl.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://frw.mhx1999.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://min.yuxming.cn

Ruby: Color = %i[red green].freeze
来源：http://kpt.shzxlz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cds.52xcode.cn

[G16] 对象转数组 / 字典
来源：http://lgb.fehbvm.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fsf.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://sqg.jyoumei.cn

JS:   Object.entries(obj)
来源：http://xwg.316326.xyz

TS:   Object.entries(obj)
来源：http://vjs.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ttv.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gya.epnwcf.com

Ruby: obj.instance_variables
来源：http://swy.jlsjyb.cn

C#:   // 用反射或 System.Text.Json
来源：http://tok.tanke756.top

================================================================================
来源：http://uqr.xinyue.icu

H. 异常与错误处理
来源：http://wqj.yanxiufei.cn

================================================================================
来源：http://trp.hnqzz.top

[H01] try / catch 基础
来源：http://zrm.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zjf.yongpay.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kwh.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gnn.aibaodan.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ywj.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://djf.cdnleiting.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://umj.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lwe.redwolf501.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tre.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://foo.c1oappe.top

Py:   try: f()⏎finally: cleanup()
来源：http://mdi.iojbl.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ivw.hnxiangtu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://msg.zdqjudy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xmy.ydjk.org.cn

Java: try { f(); } finally { cleanup(); }
来源：http://suw.cqqwz.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wht.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://vqk.sweek.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://euu.tianlin.xyz

[H03] 主动抛出异常
来源：http://ygw.hnxiangtu.top

Py:   raise ValueError("错误信息")
来源：http://mej.yonumen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qaa.52xcode.cn

JS:   throw new Error("错误信息");
来源：http://dhr.gogol.net.cn

TS:   throw new Error("错误信息");
来源：http://cbc.zhoulong.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://erj.smart0.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://enp.uphjek.com

Ruby: raise ArgumentError, "错误信息"
来源：http://ovp.svipenyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ipx.yanxiufei.cn

[H04] 自定义异常类型
来源：http://vaj.jiagoushi.top

Py:   class MyError(Exception): pass
来源：http://xha.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://wca.hnqzz.top

JS:   class MyError extends Error {}
来源：http://iqu.xuetiantiany.cn

TS:   class MyError extends Error {}
来源：http://big.shanyushiyangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://ljl.smart0.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://asg.jianghu66.top

Ruby: class MyError < StandardError; end
来源：http://xmp.jianghu66.top

C#:   class MyException : Exception {}
来源：http://rrb.shzxlz.cn

[H05] 捕获特定类型
来源：http://eie.yanxiufei.cn

Py:   except ValueError as e:
来源：http://jhw.guannengcc.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ffw.epnwcf.com

JS:   if (e instanceof TypeError) {}
来源：http://scz.gotoacloud.top

TS:   if (e instanceof TypeError) {}
来源：http://amo.chenlongwang.top

Java: catch (IOException | SQLException e) {}
来源：http://igv.guannengcc.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kwq.yangfankeji.com

Ruby: rescue ArgumentError => e
来源：http://ghg.gogol.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hig.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://jqz.yfazqb.com

Py:   value = d.get("k") or default
来源：http://jxf.shangyingyoupin.top

PHP:  $v = $d["k"] ?? null;
来源：http://vcp.daxiang520.top

JS:   obj?.a?.b;  d ?? default
来源：http://jbg.chenzaomai.com

TS:   obj?.a?.b;  d ?? default
来源：http://fdh.nanxuanxn.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yfs.hfpthk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ode.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://flc.shanyushiyangtech.top

C#:   obj?.A?.B ?? default
来源：http://zpd.wangshuangyany.cn

[H07] 断言
来源：http://pml.tianlin.xyz

Py:   assert x > 0, "必须为正"
来源：http://eeb.xinyue.icu

PHP:  assert($x > 0);
来源：http://hxe.ppjwa.cn

JS:   console.assert(x > 0);
来源：http://ckt.iojbl.cn

TS:   console.assert(x > 0);
来源：http://ygz.fzhhl.top

Java: assert x > 0 : "必须为正";
来源：http://iuj.fehbvm.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ezr.yj20258.top

Ruby: raise "必须为正" unless x > 0
来源：http://ybb.shanyushiyangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://osb.hcnkem.com

[H08] 获取错误信息与堆栈
来源：http://rko.ybcxt.top

Py:   str(e);  traceback.format_exc()
来源：http://oqx.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xxn.9152youxi.cn

JS:   e.message;  e.stack
来源：http://elh.mhx1999.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://aad.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jzi.cheryme.top

Go:   err.Error()
来源：http://onk.yanxiufei.cn

Ruby: e.message;  e.backtrace
来源：http://hiz.tanke756.top

C#:   e.Message;  e.StackTrace
来源：http://ndv.bbcook.cn

[H09] 带错误码的异常
来源：http://iur.tianlin.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tsb.guannengcc.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://plf.ydzc1.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qvn.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lij.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gxu.tanke756.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mfl.daxiang520.top

Ruby: raise MyError.new("fail", 500)
来源：http://gtx.zhengqikj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rxx.yfazqb.com

[H10] 资源自动释放
来源：http://jdw.hcnkem.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://zcy.gotoacloud.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ljf.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tbz.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rgj.yongpay.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hhd.mhx1999.top

Go:   defer f.Close()
来源：http://anr.birdmap.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uhx.xziqi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tjg.yangfankeji.com

================================================================================
来源：http://dfo.iojbl.cn

I. 正则表达式
来源：http://ayw.dashuyun.cn

================================================================================
来源：http://zhx.gaohongyu789.top

[I01] 判断是否匹配
来源：http://ixn.jqgfzy.top


<!-- 参考信息 -->