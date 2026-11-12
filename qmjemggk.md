代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://mco.tanke756.top

TS:   fs.unlinkSync("a.txt")
来源：http://trv.vehdjk.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://abi.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://nrw.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://ovs.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://kqz.jinqigfzy.top

[F07] 创建目录（含多级）
来源：http://nsq.jinqigfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rrr.tanke756.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jsy.nwbrower.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jrv.sysykeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ndq.ivvv.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xoc.snrcjt.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nze.xziqi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tsf.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xai.feifeiyinyue.top

[F08] 遍历目录
来源：http://uho.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hvh.chenlongwang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dqv.zhiwuduotai.top

JS:   fs.readdirSync("dir")
来源：http://ynp.yangfankeji.com

TS:   fs.readdirSync("dir")
来源：http://gxd.xinyue.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://poa.sweek.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zfd.hammf.cn

Ruby: Dir.children("dir")
来源：http://rwp.xinyue.icu

C#:   Directory.GetFiles("dir")
来源：http://vpj.yfazqb.com

[F09] 获取文件大小
来源：http://akn.wangdashe.top

Py:   os.path.getsize("a.txt")
来源：http://hkc.daxiang520.top

PHP:  filesize("a.txt");
来源：http://nhk.fzhhl.top

JS:   fs.statSync("a.txt").size
来源：http://kic.c1oappe.top

TS:   fs.statSync("a.txt").size
来源：http://kdj.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://saj.hesvh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vih.shangyingyoupin.top

Ruby: File.size("a.txt")
来源：http://ttl.cucudq.cn

C#:   new FileInfo("a.txt").Length
来源：http://nll.hesvh.cn

[F10] 取文件扩展名 / 文件名
来源：http://hwz.fanxiaobao.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oru.nanxinkj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vwe.yongpay.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uag.tanke756.top

TS:   path.extname("a.txt")
来源：http://vwe.sjlbkw.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://alq.guannengcc.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vak.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tnt.daria6918.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vpl.yuxming.cn

[F11] 复制与移动文件
来源：http://rkr.cqqwz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://byr.xinyue.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wkz.pycfn.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vry.iojbl.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gcs.zhiwuduotai.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ujl.9152youxi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tmy.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lto.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://svq.yvedp.cn

[F12] CSV 读写
来源：http://rnb.gotoacloud.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kyk.fktsv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aly.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xlc.smart0.xyz

TS:   // 同上
来源：http://woq.fzhhl.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lgf.dashuyun.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://syl.316326.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://umm.52xcode.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ajp.chenlongwang.top

================================================================================
来源：http://nno.feifeiyinyue.top

G. 面向对象
来源：http://yeo.jqgufenzy.top

================================================================================
来源：http://evo.nwbrower.top

[G01] 定义类
来源：http://ioc.52xcode.cn

Py:   class User: pass
来源：http://enr.aizwys.cn

PHP:  class User {}
来源：http://rtn.vqdsnc.cn

JS:   class User {}
来源：http://lqi.shzxlz.cn

TS:   class User { name: string = ""; }
来源：http://eca.chenlongwang.top

Java: class User {}
来源：http://nyo.iojbl.cn

Go:   type User struct { Name string }
来源：http://ebl.yj20258.top

Ruby: class User; end
来源：http://qoe.yvedp.cn

C#:   class User {}
来源：http://daj.snrcjt.cn

[G02] 构造函数
来源：http://sqa.yj20258888.top

Py:   def __init__(self, name): self.name = name
来源：http://vst.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://csx.fanxiaobao.xyz

JS:   constructor(name) { this.name = name; }
来源：http://ahq.fanxiaobao.xyz

TS:   constructor(public name: string) {}
来源：http://mcp.yvedp.cn

Java: User(String name) { this.name = name; }
来源：http://psy.hnqzz.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aho.aibaodan.cn

Ruby: def initialize(name); @name = name; end
来源：http://gik.birdmap.top

C#:   public User(string name) { Name = name; }
来源：http://vvw.xylfe.cn

[G03] 实例属性
来源：http://zjh.yfazqb.com

Py:   self.name = "x"
来源：http://hgr.sufxvd.cn

PHP:  public string $name = "x";
来源：http://txr.fanxiaobao.xyz

JS:   this.name = "x";
来源：http://yiq.zhengqikj.top

TS:   name: string = "x";
来源：http://mtc.yangfankeji.com

Java: private String name;
来源：http://iln.ywan-chungtsiang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jal.xylfe.cn

Ruby: @name = "x"
来源：http://xww.hfpthk.cn

C#:   public string Name { get; set; } = "x";
来源：http://ltb.shanyushiyangkeji.top

[G04] 定义方法
来源：http://frd.andypj.xyz

Py:   def greet(self): return self.name
来源：http://qup.zhixingplan.top

PHP:  public function greet(): string { return $this->name; }
来源：http://npp.hnqzz.top

JS:   greet() { return this.name; }
来源：http://ebn.0kj1m.cn

TS:   greet(): string { return this.name; }
来源：http://kad.0kj1m.cn

Java: String greet() { return name; }
来源：http://ina.sysykeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://spt.cucudq.cn

Ruby: def greet; @name; end
来源：http://xgu.jlsjyb.cn

C#:   public string Greet() => Name;
来源：http://ehf.jqgfzy.top

[G05] 继承
来源：http://gce.sxryk.cn

Py:   class Admin(User): pass
来源：http://rmn.epnwcf.com

PHP:  class Admin extends User {}
来源：http://qgq.zdbjq.cn

JS:   class Admin extends User {}
来源：http://iyw.uphjek.com

TS:   class Admin extends User {}
来源：http://ohd.ybcxt.top

Java: class Admin extends User {}
来源：http://zyk.jianghu66.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jmv.nanxinkj.top

Ruby: class Admin < User; end
来源：http://itt.vehdjk.com

C#:   class Admin : User {}
来源：http://ymq.hcnkem.com

[G06] 重写方法
来源：http://ymq.haohaochexian.top

Py:   def greet(self): return "admin"
来源：http://rds.yfazqb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://pcd.zdbjq.cn

JS:   greet() { return "admin"; }
来源：http://yde.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://nei.tian-w.cn

Java: @Override String greet() { return "admin"; }
来源：http://kps.tianlin.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tbc.aizwys.cn

Ruby: def greet; "admin"; end
来源：http://omh.jqgfzy.top

C#:   public override string Greet() => "admin";
来源：http://xot.guowangkeji.top

[G07] 调用父类方法
来源：http://dyp.fengsongda.top

Py:   super().greet()
来源：http://kfe.shanyushiyangtech.top

PHP:  parent::greet();
来源：http://yqs.zhixingplan.top

JS:   super.greet();
来源：http://wnj.yanxiufei.cn

TS:   super.greet();
来源：http://nho.sjlbkw.cn

Java: super.greet();
来源：http://zjs.nanxuanxn.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lii.chenjidiqi.icu

Ruby: super
来源：http://gpq.gotoacloud.top

C#:   base.Greet();
来源：http://asl.52xcode.cn

[G08] 静态方法与属性
来源：http://wke.hywenlv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jnt.zhongyouzk.top

PHP:  public static function f() {}
来源：http://rvy.yvedp.cn

JS:   static f() {}
来源：http://fah.zhiwuduotai.top

TS:   static f(): void {}
来源：http://sgh.meibo888.top

Java: static void f() {}
来源：http://dqy.52xcode.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mor.pycfn.com

Ruby: def self.f; end
来源：http://cut.feifeiyinyue.top

C#:   public static void F() {}
来源：http://siz.zycfv.cn

[G09] 接口 / 抽象类
来源：http://fem.tanke756.top

Py:   from abc import ABC, abstractmethod
来源：http://jud.52xcode.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iyr.fanxiaobao.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://iqf.zhoulong.xyz

TS:   interface Shape { area(): number; }
来源：http://ley.fktsv.cn

Java: interface Shape { double area(); }
来源：http://rrl.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://deh.jianghu66.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://seq.ydjk.org.cn

C#:   interface IShape { double Area(); }
来源：http://bhi.gogol.net.cn

[G10] 访问控制
来源：http://ykd.gzhubu.top

Py:   约定 _protected / __private（不强制）
来源：http://yxq.pycfn.com

PHP:  public / protected / private
来源：http://bje.yueranfly.top

JS:   #private 字段；其余公开
来源：http://viu.fktsv.cn

TS:   public / protected / private
来源：http://ugo.zycfv.cn

Java: public / protected / private / 默认包级
来源：http://mak.hesvh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vhw.gogol.net.cn

Ruby: public / protected / private
来源：http://srs.jinqigfzy.top

C#:   public / protected / private / internal
来源：http://ewr.shanyushiyangtech.top

[G11] getter / setter
来源：http://xxq.feifeiyinyue.top

Py:   @property 与 @x.setter
来源：http://bvm.gaohongyu789.top

PHP:  public function getName(): string { return $this->name; }
来源：http://quh.fanxiaobao.xyz

JS:   get name() { return this._name; }
来源：http://kqx.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://ivx.fehbvm.com

Java: public String getName() { return name; }
来源：http://nmo.zhiwuduotai.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ipn.dianchejie.cn

Ruby: attr_accessor :name
来源：http://mja.jqgufenzy.top

C#:   public string Name { get; set; }
来源：http://ews.zhijiandao.cn

[G12] 对象转字符串
来源：http://naj.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://cva.daxiang520.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://isq.bjfxy.top

JS:   toString() { return this.name; }
来源：http://kqd.yueranfly.top

TS:   toString(): string { return this.name; }
来源：http://byn.wangdashe.top

Java: @Override public String toString() { return name; }
来源：http://fsa.andypj.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://psb.yanxiufei.cn

Ruby: def to_s; @name; end
来源：http://glb.wangshuangyany.cn

C#:   public override string ToString() => Name;
来源：http://ahq.bbcook.cn

[G13] 判断对象类型
来源：http://atr.aizwys.cn

Py:   isinstance(u, User)
来源：http://sxg.jqgfzy.top

PHP:  $u instanceof User
来源：http://nrb.aizwys.cn

JS:   u instanceof User
来源：http://qpd.ydzc1.top

TS:   u instanceof User
来源：http://spq.yj202588.top

Java: u instanceof User
来源：http://pcc.yuanzhike.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hcz.sweek.top

Ruby: u.is_a?(User)
来源：http://mge.haohaochexian.top

C#:   u is User
来源：http://rsc.guowangkeji.top

[G14] 数据类 / record
来源：http://nrf.fktsv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kyk.zhaomingkeji.xyz

PHP:  // 用 readonly 属性模拟
来源：http://quu.yj20258888.top

JS:   // 无内置：普通类或对象字面量
来源：http://bib.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://nxu.dashuyun.cn

Java: record User(String name, int age) {}
来源：http://btx.xylfe.cn

Go:   type User struct { Name string; Age int }
来源：http://ssh.hnqzz.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ofg.zdbjq.cn

C#:   record User(string Name, int Age);
来源：http://pgo.xinyue.icu

[G15] 枚举
来源：http://vlg.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://twb.daria6918.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xbb.smart0.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://geg.yueranfly.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kak.yangfankeji.com

Java: enum Color { RED, GREEN }
来源：http://lfk.xziqi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jeh.redwolf501.top

Ruby: Color = %i[red green].freeze
来源：http://osg.cheryme.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zmb.guannengcc.top

[G16] 对象转数组 / 字典
来源：http://yzb.daxiang520.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dyh.zhixingplan.top

PHP:  get_object_vars($obj);
来源：http://tvb.hongshengwenyu.top

JS:   Object.entries(obj)
来源：http://hyp.ywan-chungtsiang.top

TS:   Object.entries(obj)
来源：http://utc.zhongyouzk.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://okh.jlsjyb.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://esr.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://vqp.sysykeji.top

C#:   // 用反射或 System.Text.Json
来源：http://ynv.nwbrower.top

================================================================================
来源：http://hbi.gotoacloud.top

H. 异常与错误处理
来源：http://qvz.hammf.cn

================================================================================
来源：http://gey.ivvv.top

[H01] try / catch 基础
来源：http://fmf.shzxlz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nqx.ydjk.org.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bgq.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fae.sysykeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hqa.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qro.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hju.yfazqb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vwv.vehdjk.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wxp.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://wgz.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://ycw.chenzaomai.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://efl.zhixingplan.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jys.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ykj.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dmt.uphjek.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://jim.shanyushiyangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ohv.quarkkingdee.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mvf.zhoulong.xyz

[H03] 主动抛出异常
来源：http://nzp.fzhhl.top

Py:   raise ValueError("错误信息")
来源：http://mgi.cheryme.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://syo.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://ygd.zhaomingkeji.xyz

TS:   throw new Error("错误信息");
来源：http://oja.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://whn.iojbl.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rwx.nwbrower.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qdy.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://szt.wangdashe.top

[H04] 自定义异常类型
来源：http://kne.feifeiyinyue.top

Py:   class MyError(Exception): pass
来源：http://bce.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xbe.epnwcf.com

JS:   class MyError extends Error {}
来源：http://cei.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://dyv.jinqigufen.top

Java: class MyException extends RuntimeException {}
来源：http://pih.snrcjt.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://leq.yvedp.cn

Ruby: class MyError < StandardError; end
来源：http://cha.jiagoushi.top

C#:   class MyException : Exception {}
来源：http://fhd.jianghu66.top

[H05] 捕获特定类型
来源：http://ohg.yanxiufei.cn

Py:   except ValueError as e:
来源：http://jvx.ydzc1.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rxb.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://cie.pengpengdd.cyou

TS:   if (e instanceof TypeError) {}
来源：http://kfr.yj20258.top

Java: catch (IOException | SQLException e) {}
来源：http://qcu.aizwys.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mdt.fanxiaobao.xyz

Ruby: rescue ArgumentError => e
来源：http://hum.hongshengwenyu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aqd.birdmap.top

[H06] 可选值 / 空值安全访问
来源：http://rzb.xziqi.cn

Py:   value = d.get("k") or default
来源：http://kpj.redwolf501.top

PHP:  $v = $d["k"] ?? null;
来源：http://sgn.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://flg.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://jpn.dianchejie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qwq.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://lvt.gotoacloud.top

Ruby: d&.dig(:a, :b)
来源：http://sft.redwolf501.top

C#:   obj?.A?.B ?? default
来源：http://dxa.ehwqpu.com

[H07] 断言
来源：http://lyg.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://blx.jinqigfzy.top

PHP:  assert($x > 0);
来源：http://syc.yanxiufei.cn

JS:   console.assert(x > 0);
来源：http://ngi.chenjidiqi.icu

TS:   console.assert(x > 0);
来源：http://nuf.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://amt.tanke756.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eab.ehwqpu.com

Ruby: raise "必须为正" unless x > 0
来源：http://lyk.havefunace.top

C#:   Debug.Assert(x > 0);
来源：http://ecc.jyoumei.cn

[H08] 获取错误信息与堆栈
来源：http://ove.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://ntv.ydjk.org.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lle.zhengqikj.top

JS:   e.message;  e.stack
来源：http://rei.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lkt.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nwy.yueranfly.top

Go:   err.Error()
来源：http://ojt.9152youxi.cn

Ruby: e.message;  e.backtrace
来源：http://qdh.wangdashe.top

C#:   e.Message;  e.StackTrace
来源：http://omz.yongpay.top

[H09] 带错误码的异常
来源：http://cix.hnqzz.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ckz.nwbrower.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nfj.xinyue.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cyi.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://atv.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yct.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ahq.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oli.vqdsnc.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lst.yangfankeji.com

[H10] 资源自动释放
来源：http://nlx.ywan-chungtsiang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://aqy.fengsongda.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qek.kuanghao11.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qyx.chenlongwang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jmq.gotoacloud.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zth.jinqigufen.top

Go:   defer f.Close()
来源：http://nru.cucudq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aij.smart0.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kms.yonumen.top


<!-- 参考信息 -->