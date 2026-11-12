代发 wailian999

C#:   File.Exists("a.txt")
来源：http://ghb.chenzaomai.com

[F06] 删除文件
来源：http://oan.fengsongda.top

Py:   os.remove("a.txt")
来源：http://tvo.dianchejie.cn

PHP:  unlink("a.txt");
来源：http://mln.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://yev.kuanghao11.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xtv.yj202588.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jnn.daria6918.cn

Go:   os.Remove("a.txt")
来源：http://kbc.hnqzz.top

Ruby: File.delete("a.txt")
来源：http://fbw.pengpengdd.cyou

C#:   File.Delete("a.txt");
来源：http://fmi.yvedp.cn

[F07] 创建目录（含多级）
来源：http://jqp.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qai.cashguo.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uhs.zhiwuduotai.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://idn.cheryme.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bmu.vqdsnc.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jov.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zko.ydzc1.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://euo.yj20258.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vnh.hcnkem.com

[F08] 遍历目录
来源：http://djk.havefunace.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kxf.daxiang520.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oar.yuanzhike.top

JS:   fs.readdirSync("dir")
来源：http://yxp.cheryme.top

TS:   fs.readdirSync("dir")
来源：http://rxi.ctjpmb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mkg.jqgufenzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jgg.hywenlv.cn

Ruby: Dir.children("dir")
来源：http://nqg.cashguo.top

C#:   Directory.GetFiles("dir")
来源：http://oxr.ivvv.top

[F09] 获取文件大小
来源：http://wuq.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://aca.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://pbt.daria6918.cn

JS:   fs.statSync("a.txt").size
来源：http://dhr.sjlbkw.cn

TS:   fs.statSync("a.txt").size
来源：http://tzo.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kzy.zycfv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vof.andypj.xyz

Ruby: File.size("a.txt")
来源：http://dgf.316326.xyz

C#:   new FileInfo("a.txt").Length
来源：http://pcy.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://vxo.zycfv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fgc.zhixingplan.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qur.gaohongyu789.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vfk.nanxinkj.top

TS:   path.extname("a.txt")
来源：http://eca.jqgfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qyg.xingfuxueyuan.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kqa.tarul.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bbf.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pxp.quarkkingdee.top

[F11] 复制与移动文件
来源：http://hfs.guannengcc.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lpn.smart0.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jyi.zycfv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vlm.xuetiantiany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cbb.nanxuanxn.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fbn.smart0.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dvs.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://obw.chenlongwang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://urx.ydjk.org.cn

[F12] CSV 读写
来源：http://eah.52xcode.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kaz.52xcode.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://byg.xylfe.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uva.ppjwa.cn

TS:   // 同上
来源：http://sav.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ili.ydjk.org.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wmo.hammf.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rmh.gaohongyu789.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tej.yfazqb.com

================================================================================
来源：http://utg.cheryme.top

G. 面向对象
来源：http://dhx.gzhubu.top

================================================================================
来源：http://agb.jianghu66.top

[G01] 定义类
来源：http://ztp.yueranfly.top

Py:   class User: pass
来源：http://afs.gaohongyu789.top

PHP:  class User {}
来源：http://zsv.smart0.xyz

JS:   class User {}
来源：http://mjs.andypj.xyz

TS:   class User { name: string = ""; }
来源：http://gzc.xingfuxueyuan.xyz

Java: class User {}
来源：http://zwf.jyoumei.cn

Go:   type User struct { Name string }
来源：http://irs.yangfankeji.com

Ruby: class User; end
来源：http://tvh.yj20258.top

C#:   class User {}
来源：http://dvu.ivvv.top

[G02] 构造函数
来源：http://wnn.ybcxt.top

Py:   def __init__(self, name): self.name = name
来源：http://ycb.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://ulx.pycfn.com

JS:   constructor(name) { this.name = name; }
来源：http://zji.ehwqpu.com

TS:   constructor(public name: string) {}
来源：http://gcd.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://rih.cqqwz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sxn.hnxiangtu.top

Ruby: def initialize(name); @name = name; end
来源：http://khb.hfpthk.cn

C#:   public User(string name) { Name = name; }
来源：http://tel.dianchejie.cn

[G03] 实例属性
来源：http://yty.meibo888.top

Py:   self.name = "x"
来源：http://lln.xinyue.icu

PHP:  public string $name = "x";
来源：http://gav.gzhubu.top

JS:   this.name = "x";
来源：http://zvq.zhiwuduotai.top

TS:   name: string = "x";
来源：http://klj.feifeiyinyue.top

Java: private String name;
来源：http://osd.316326.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ksx.aibaodan.cn

Ruby: @name = "x"
来源：http://uhr.jqgfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://jtx.hfpthk.cn

[G04] 定义方法
来源：http://vnb.daria6918.cn

Py:   def greet(self): return self.name
来源：http://ybk.dashuyun.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uhl.xylfe.cn

JS:   greet() { return this.name; }
来源：http://nxv.kuanghao11.cn

TS:   greet(): string { return this.name; }
来源：http://fwr.shanyushiyangtech.top

Java: String greet() { return name; }
来源：http://lgo.nwbrower.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://txq.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://sgd.birdmap.top

C#:   public string Greet() => Name;
来源：http://dxw.ppjwa.cn

[G05] 继承
来源：http://ync.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://pxo.uphjek.com

PHP:  class Admin extends User {}
来源：http://cig.chenjidiqi.icu

JS:   class Admin extends User {}
来源：http://xca.fehbvm.com

TS:   class Admin extends User {}
来源：http://gvg.shuidangran.top

Java: class Admin extends User {}
来源：http://ezg.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zrh.gaohongyu789.top

Ruby: class Admin < User; end
来源：http://any.daria6918.cn

C#:   class Admin : User {}
来源：http://oyy.ywan-chungtsiang.top

[G06] 重写方法
来源：http://zhv.ivvv.top

Py:   def greet(self): return "admin"
来源：http://pgr.gzhubu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fki.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://kjz.bbcook.cn

TS:   greet(): string { return "admin"; }
来源：http://tnz.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://wzj.hcnkem.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tjx.tanke756.top

Ruby: def greet; "admin"; end
来源：http://hrp.jqgfzy.top

C#:   public override string Greet() => "admin";
来源：http://dys.chenjidiqi.icu

[G07] 调用父类方法
来源：http://amc.ydjk.org.cn

Py:   super().greet()
来源：http://sak.zhoulong.xyz

PHP:  parent::greet();
来源：http://ijh.guannengcc.top

JS:   super.greet();
来源：http://obb.9152youxi.cn

TS:   super.greet();
来源：http://vmk.9152youxi.cn

Java: super.greet();
来源：http://dhn.nanxinkj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fdx.ywan-chungtsiang.top

Ruby: super
来源：http://hxv.epnwcf.com

C#:   base.Greet();
来源：http://uwi.52xcode.cn

[G08] 静态方法与属性
来源：http://qqj.kuanghao11.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dfm.hywenlv.cn

PHP:  public static function f() {}
来源：http://rbn.zhongyouzk.top

JS:   static f() {}
来源：http://lfg.tarul.cn

TS:   static f(): void {}
来源：http://mmn.yj20258.top

Java: static void f() {}
来源：http://qmq.wangshuangyany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://klb.zycfv.cn

Ruby: def self.f; end
来源：http://tow.sjlbkw.cn

C#:   public static void F() {}
来源：http://lwj.yanxiufei.cn

[G09] 接口 / 抽象类
来源：http://jbg.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://kpy.chenzaomai.com

PHP:  interface Shape { public function area(): float; }
来源：http://xtf.gaohongyu789.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qen.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://oxx.jlsjyb.cn

Java: interface Shape { double area(); }
来源：http://god.316326.xyz

Go:   type Shape interface { Area() float64 }
来源：http://fda.hammf.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ext.fanxiaobao.xyz

C#:   interface IShape { double Area(); }
来源：http://egc.smart0.xyz

[G10] 访问控制
来源：http://fcb.yj20258888.top

Py:   约定 _protected / __private（不强制）
来源：http://ijg.sjlbkw.cn

PHP:  public / protected / private
来源：http://mvo.cqqwz.cn

JS:   #private 字段；其余公开
来源：http://otk.sysykeji.top

TS:   public / protected / private
来源：http://jhs.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://vps.jyoumei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bqz.zhaomingkeji.xyz

Ruby: public / protected / private
来源：http://ymo.shangyingyoupin.top

C#:   public / protected / private / internal
来源：http://tux.hnxiangtu.top

[G11] getter / setter
来源：http://ctc.yueranfly.top

Py:   @property 与 @x.setter
来源：http://rnj.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tze.fktsv.cn

JS:   get name() { return this._name; }
来源：http://pzf.haohaochexian.top

TS:   get name(): string { return this._name; }
来源：http://lcl.xuanzx.com

Java: public String getName() { return name; }
来源：http://zqx.shanyushiyangtech.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ajj.quarkkingdee.top

Ruby: attr_accessor :name
来源：http://dzz.9152youxi.cn

C#:   public string Name { get; set; }
来源：http://zyf.0kj1m.cn

[G12] 对象转字符串
来源：http://wjn.zhoulong.xyz

Py:   def __str__(self): return self.name
来源：http://sxj.9152youxi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ntv.chenzaomai.com

JS:   toString() { return this.name; }
来源：http://qcv.redwolf501.top

TS:   toString(): string { return this.name; }
来源：http://kyb.ehwqpu.com

Java: @Override public String toString() { return name; }
来源：http://jqz.dashuyun.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tax.sysykeji.top

Ruby: def to_s; @name; end
来源：http://ngp.andypj.xyz

C#:   public override string ToString() => Name;
来源：http://jhh.xziqi.cn

[G13] 判断对象类型
来源：http://eay.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://xuq.guowangkeji.top

PHP:  $u instanceof User
来源：http://rxw.zhengqikj.top

JS:   u instanceof User
来源：http://nww.hesvh.cn

TS:   u instanceof User
来源：http://kwg.sweek.top

Java: u instanceof User
来源：http://gih.yuxming.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mdf.jqgfzy.top

Ruby: u.is_a?(User)
来源：http://ysr.xziqi.cn

C#:   u is User
来源：http://rpu.316326.xyz

[G14] 数据类 / record
来源：http://vmb.ydjk.org.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xgy.ywan-chungtsiang.top

PHP:  // 用 readonly 属性模拟
来源：http://gwl.daxiang520.top

JS:   // 无内置：普通类或对象字面量
来源：http://zpn.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://cnh.0kj1m.cn

Java: record User(String name, int age) {}
来源：http://wvx.gzhubu.top

Go:   type User struct { Name string; Age int }
来源：http://jst.ehwqpu.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fqn.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://rpc.fanxiaobao.xyz

[G15] 枚举
来源：http://szr.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ayo.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mws.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ylb.fzhhl.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wbt.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://cud.havefunace.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ebk.yonumen.top

Ruby: Color = %i[red green].freeze
来源：http://rtp.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://awx.zhiwuduotai.top

[G16] 对象转数组 / 字典
来源：http://ykp.yuxming.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ujj.xinyue.icu

PHP:  get_object_vars($obj);
来源：http://erj.zycfv.cn

JS:   Object.entries(obj)
来源：http://dgq.jqgufenzy.top

TS:   Object.entries(obj)
来源：http://qfo.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zyc.aizwys.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wnk.snrcjt.cn

Ruby: obj.instance_variables
来源：http://dnl.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://dyt.kuanghao11.cn

================================================================================
来源：http://kpc.hcnkem.com

H. 异常与错误处理
来源：http://wdi.hongshengwenyu.top

================================================================================
来源：http://wft.ybcxt.top

[H01] try / catch 基础
来源：http://zea.ywan-chungtsiang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mgb.hnqzz.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sjc.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nvq.fengsongda.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vhi.yuanzhike.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jfr.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xyr.quarkkingdee.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bwl.hesvh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xth.tarul.cn

[H02] finally / ensure 收尾
来源：http://pdc.daxiang520.top

Py:   try: f()⏎finally: cleanup()
来源：http://rtg.yanxiufei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ttr.yuxming.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bip.ppjwa.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vpw.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://ukj.hywenlv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ysu.ydjk.org.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pyo.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://byn.ywan-chungtsiang.top

[H03] 主动抛出异常
来源：http://rpo.hnqzz.top

Py:   raise ValueError("错误信息")
来源：http://auv.c1oappe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wxh.gogol.net.cn

JS:   throw new Error("错误信息");
来源：http://bmb.shzxlz.cn

TS:   throw new Error("错误信息");
来源：http://krm.shzxlz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fqr.vehdjk.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ctt.9152youxi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kjs.guowangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://ljt.ydjk.org.cn

[H04] 自定义异常类型
来源：http://vbr.shzxlz.cn

Py:   class MyError(Exception): pass
来源：http://kxv.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://snj.chenjidiqi.icu

JS:   class MyError extends Error {}
来源：http://gop.shzxlz.cn

TS:   class MyError extends Error {}
来源：http://rjk.c1oappe.top

Java: class MyException extends RuntimeException {}
来源：http://ubh.tarul.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kwq.zhixingplan.top

Ruby: class MyError < StandardError; end
来源：http://pfg.yj20258888.top

C#:   class MyException : Exception {}
来源：http://qon.fengsongda.top

[H05] 捕获特定类型
来源：http://jfy.gzhubu.top

Py:   except ValueError as e:
来源：http://tgo.andypj.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://chu.jinqigufen.top

JS:   if (e instanceof TypeError) {}
来源：http://vmx.bjfxy.top

TS:   if (e instanceof TypeError) {}
来源：http://pvh.fktsv.cn

Java: catch (IOException | SQLException e) {}
来源：http://khy.daxiang520.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zgz.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://wzg.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cxf.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://eew.yanxiufei.cn

Py:   value = d.get("k") or default
来源：http://ufx.hnqzz.top

PHP:  $v = $d["k"] ?? null;
来源：http://alo.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://ons.9152youxi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jrz.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rqk.yfazqb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://jkm.gaohongyu789.top

Ruby: d&.dig(:a, :b)
来源：http://nch.shanyushiyangkeji.top

C#:   obj?.A?.B ?? default
来源：http://pvi.ywan-chungtsiang.top

[H07] 断言
来源：http://xdg.ywan-chungtsiang.top

Py:   assert x > 0, "必须为正"
来源：http://gms.zhijiandao.cn

PHP:  assert($x > 0);
来源：http://nqm.yj202588.top

JS:   console.assert(x > 0);
来源：http://fij.shuidangran.top

TS:   console.assert(x > 0);
来源：http://syk.chenjidiqi.icu

Java: assert x > 0 : "必须为正";
来源：http://pbl.gogol.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vgx.0kj1m.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sxk.hfpthk.cn

C#:   Debug.Assert(x > 0);
来源：http://cyp.nwbrower.top

[H08] 获取错误信息与堆栈
来源：http://jxq.quarkkingdee.top

Py:   str(e);  traceback.format_exc()
来源：http://iwe.chenlongwang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://igt.dianchejie.cn

JS:   e.message;  e.stack
来源：http://tnl.jlsjyb.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xhw.guowangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qsz.316326.xyz

Go:   err.Error()
来源：http://hnd.yangfankeji.com

Ruby: e.message;  e.backtrace
来源：http://jxk.haohaochexian.top

C#:   e.Message;  e.StackTrace
来源：http://shf.sweek.top

[H09] 带错误码的异常
来源：http://ddp.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eth.epnwcf.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://jhj.hammf.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bss.yj20258.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cza.zdqjudy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kdw.ybcxt.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vkg.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://luh.ehwqpu.com

C#:   // 自定义异常类中加 Code 属性
来源：http://vvt.jinyuanbaomall.cn

[H10] 资源自动释放
来源：http://sme.zhengqikj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://uib.ydjk.org.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yey.zhixingplan.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ndz.dashuyun.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ccz.pengpengdd.cyou


<!-- 参考信息 -->