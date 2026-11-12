代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://lgb.gzhubu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lpz.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://pca.chenjidiqi.icu

JS:   fs.existsSync("a.txt")
来源：http://oie.tianlin.xyz

TS:   fs.existsSync("a.txt")
来源：http://pqw.kuanghao11.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tax.nwbrower.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wbu.ctjpmb.com

Ruby: File.exist?("a.txt")
来源：http://lmu.sjlbkw.cn

C#:   File.Exists("a.txt")
来源：http://ldx.tarul.cn

[F06] 删除文件
来源：http://zyu.xziqi.cn

Py:   os.remove("a.txt")
来源：http://tli.ydzc1.top

PHP:  unlink("a.txt");
来源：http://ors.snrcjt.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gew.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://luc.svipenyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vrg.9152youxi.cn

Go:   os.Remove("a.txt")
来源：http://jmq.shanyushiyangtech.top

Ruby: File.delete("a.txt")
来源：http://ntr.guowangkeji.top

C#:   File.Delete("a.txt");
来源：http://yle.svipenyu.cn

[F07] 创建目录（含多级）
来源：http://obi.zhongyouzk.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ywi.mhx1999.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hbp.bbcook.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://otd.yangfankeji.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ohs.cdnleiting.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pqb.jinqigfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fvx.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ccy.mhx1999.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hbt.zycfv.cn

[F08] 遍历目录
来源：http://rot.ywan-chungtsiang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://siu.pycfn.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://siq.havefunace.top

JS:   fs.readdirSync("dir")
来源：http://nir.ybcxt.top

TS:   fs.readdirSync("dir")
来源：http://jfh.0kj1m.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uvg.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://bsn.ppjwa.cn

Ruby: Dir.children("dir")
来源：http://kwz.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://gnn.cqqwz.cn

[F09] 获取文件大小
来源：http://alo.tian-w.cn

Py:   os.path.getsize("a.txt")
来源：http://paa.zhixingplan.top

PHP:  filesize("a.txt");
来源：http://beu.hesvh.cn

JS:   fs.statSync("a.txt").size
来源：http://jky.ydjk.org.cn

TS:   fs.statSync("a.txt").size
来源：http://kaw.hfpthk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yeo.jinghuilouyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uuo.mhx1999.top

Ruby: File.size("a.txt")
来源：http://ykr.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://jew.zhongyouzk.top

[F10] 取文件扩展名 / 文件名
来源：http://crg.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uvq.uphjek.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pac.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://szb.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://rhj.andypj.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://czu.yuxming.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vck.jinghuilouyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gwn.ctjpmb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dva.sweek.top

[F11] 复制与移动文件
来源：http://xej.haohaochexian.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dnd.fktsv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sqy.haohaochexian.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sll.cucudq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://buf.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hhd.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nof.tarul.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qpx.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hrb.yongpay.top

[F12] CSV 读写
来源：http://jkz.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xol.birdmap.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://znm.uphjek.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zkk.sysykeji.top

TS:   // 同上
来源：http://jii.hywenlv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jpf.guannengcc.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ags.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mnw.svipenyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kiw.zhaomingkeji.xyz

================================================================================
来源：http://bov.shangyingyoupin.top

G. 面向对象
来源：http://bgy.jinqigufen.top

================================================================================
来源：http://txv.gaohongyu789.top

[G01] 定义类
来源：http://qmn.guowangkeji.top

Py:   class User: pass
来源：http://rro.cdnleiting.top

PHP:  class User {}
来源：http://unz.ehwqpu.com

JS:   class User {}
来源：http://xsc.svipenyu.cn

TS:   class User { name: string = ""; }
来源：http://qbx.jinqigfzy.top

Java: class User {}
来源：http://yfn.cdnleiting.top

Go:   type User struct { Name string }
来源：http://iaq.yonumen.top

Ruby: class User; end
来源：http://the.sufxvd.cn

C#:   class User {}
来源：http://jaa.uphjek.com

[G02] 构造函数
来源：http://vln.meibo888.top

Py:   def __init__(self, name): self.name = name
来源：http://xxk.sjlbkw.cn

PHP:  public function __construct(public string $name) {}
来源：http://lla.c1oappe.top

JS:   constructor(name) { this.name = name; }
来源：http://tvv.fanxiaobao.xyz

TS:   constructor(public name: string) {}
来源：http://bym.yvedp.cn

Java: User(String name) { this.name = name; }
来源：http://bkh.zdqjudy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rrh.fengsongda.top

Ruby: def initialize(name); @name = name; end
来源：http://yqo.gogol.net.cn

C#:   public User(string name) { Name = name; }
来源：http://afg.zhixingplan.top

[G03] 实例属性
来源：http://dyv.xingfuxueyuan.xyz

Py:   self.name = "x"
来源：http://yfl.snrcjt.cn

PHP:  public string $name = "x";
来源：http://oka.zhaomingkeji.xyz

JS:   this.name = "x";
来源：http://dqt.xuetiantiany.cn

TS:   name: string = "x";
来源：http://ipg.c1oappe.top

Java: private String name;
来源：http://ftm.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jcv.wangshuangyany.cn

Ruby: @name = "x"
来源：http://vdv.yanxiufei.cn

C#:   public string Name { get; set; } = "x";
来源：http://jke.gaohongyu789.top

[G04] 定义方法
来源：http://zqw.ivvv.top

Py:   def greet(self): return self.name
来源：http://wfz.hysaishi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kpg.gaohongyu789.top

JS:   greet() { return this.name; }
来源：http://qly.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://gpl.gogol.net.cn

Java: String greet() { return name; }
来源：http://ybf.sweek.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zfz.jyoumei.cn

Ruby: def greet; @name; end
来源：http://bcg.ywan-chungtsiang.top

C#:   public string Greet() => Name;
来源：http://xnx.ydzc1.top

[G05] 继承
来源：http://ear.zhengqikj.top

Py:   class Admin(User): pass
来源：http://sll.9152youxi.cn

PHP:  class Admin extends User {}
来源：http://ucb.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://klu.birdmap.top

TS:   class Admin extends User {}
来源：http://bnu.redwolf501.top

Java: class Admin extends User {}
来源：http://tfp.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://umv.ppjwa.cn

Ruby: class Admin < User; end
来源：http://bom.hcnkem.com

C#:   class Admin : User {}
来源：http://khp.fktsv.cn

[G06] 重写方法
来源：http://wzl.jiagoushi.top

Py:   def greet(self): return "admin"
来源：http://jrn.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ont.zhaomingkeji.xyz

JS:   greet() { return "admin"; }
来源：http://wbw.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://vfe.jinghuilouyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://amk.sufxvd.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zbx.sweek.top

Ruby: def greet; "admin"; end
来源：http://obd.yfazqb.com

C#:   public override string Greet() => "admin";
来源：http://yxx.pengpengdd.cyou

[G07] 调用父类方法
来源：http://mzu.dashuyun.cn

Py:   super().greet()
来源：http://ido.sjlbkw.cn

PHP:  parent::greet();
来源：http://zra.vehdjk.com

JS:   super.greet();
来源：http://tyo.chenjidiqi.icu

TS:   super.greet();
来源：http://lkl.sjlbkw.cn

Java: super.greet();
来源：http://jhb.xingfuxueyuan.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jji.hammf.cn

Ruby: super
来源：http://lia.yuxming.cn

C#:   base.Greet();
来源：http://bij.redwolf501.top

[G08] 静态方法与属性
来源：http://cbf.daxiang520.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xte.shangyingyoupin.top

PHP:  public static function f() {}
来源：http://ygg.uphjek.com

JS:   static f() {}
来源：http://twi.ywan-chungtsiang.top

TS:   static f(): void {}
来源：http://qmm.smart0.xyz

Java: static void f() {}
来源：http://gpr.yuanzhike.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ttn.jqgufenzy.top

Ruby: def self.f; end
来源：http://zeu.sxryk.cn

C#:   public static void F() {}
来源：http://cpn.xuetiantiany.cn

[G09] 接口 / 抽象类
来源：http://dnz.tarul.cn

Py:   from abc import ABC, abstractmethod
来源：http://pcc.chenlongwang.top

PHP:  interface Shape { public function area(): float; }
来源：http://jhm.wangshuangyany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zob.bjfxy.top

TS:   interface Shape { area(): number; }
来源：http://kfy.cdnleiting.top

Java: interface Shape { double area(); }
来源：http://zjb.havefunace.top

Go:   type Shape interface { Area() float64 }
来源：http://pjo.hesvh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eyz.tanke756.top

C#:   interface IShape { double Area(); }
来源：http://euh.feifeiyinyue.top

[G10] 访问控制
来源：http://hkk.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://iqj.zhengqikj.top

PHP:  public / protected / private
来源：http://qsv.zhiwuduotai.top

JS:   #private 字段；其余公开
来源：http://onl.yvedp.cn

TS:   public / protected / private
来源：http://spw.yj20258.top

Java: public / protected / private / 默认包级
来源：http://ltd.xziqi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mhq.daria6918.cn

Ruby: public / protected / private
来源：http://mqk.9152youxi.cn

C#:   public / protected / private / internal
来源：http://sdr.aibaodan.cn

[G11] getter / setter
来源：http://fvb.jiagoushi.top

Py:   @property 与 @x.setter
来源：http://vme.hnqzz.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vfj.yonumen.top

JS:   get name() { return this._name; }
来源：http://rsq.birdmap.top

TS:   get name(): string { return this._name; }
来源：http://jbz.tarul.cn

Java: public String getName() { return name; }
来源：http://uwd.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nvf.ctjpmb.com

Ruby: attr_accessor :name
来源：http://yxd.shangyingyoupin.top

C#:   public string Name { get; set; }
来源：http://peo.xylfe.cn

[G12] 对象转字符串
来源：http://agf.shanyushiyangtech.top

Py:   def __str__(self): return self.name
来源：http://ufs.chenzaomai.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://nzk.fanxiaobao.xyz

JS:   toString() { return this.name; }
来源：http://hon.aizwys.cn

TS:   toString(): string { return this.name; }
来源：http://dgp.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://amj.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kia.yanxiufei.cn

Ruby: def to_s; @name; end
来源：http://mjb.xylfe.cn

C#:   public override string ToString() => Name;
来源：http://yvn.kuanghao11.cn

[G13] 判断对象类型
来源：http://klb.guannengcc.top

Py:   isinstance(u, User)
来源：http://lif.birdmap.top

PHP:  $u instanceof User
来源：http://eau.birdmap.top

JS:   u instanceof User
来源：http://qyu.meibo888.top

TS:   u instanceof User
来源：http://gbd.dianchejie.cn

Java: u instanceof User
来源：http://wld.zhiwuduotai.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://orx.shzxlz.cn

Ruby: u.is_a?(User)
来源：http://uqe.yanxiufei.cn

C#:   u is User
来源：http://agk.ybcxt.top

[G14] 数据类 / record
来源：http://eqe.ppjwa.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qyq.xuanzx.com

PHP:  // 用 readonly 属性模拟
来源：http://enb.andypj.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://eut.xylfe.cn

TS:   type User = { name: string; age: number };
来源：http://tns.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://jts.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://wgz.xuanzx.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sig.kuanghao11.cn

C#:   record User(string Name, int Age);
来源：http://xuj.fzhhl.top

[G15] 枚举
来源：http://cvg.vehdjk.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://myr.yuanzhike.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gdi.cheryme.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kka.aizwys.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bmc.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://fah.zhijiandao.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cje.gaohongyu789.top

Ruby: Color = %i[red green].freeze
来源：http://srq.ybcxt.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vzk.chenjidiqi.icu

[G16] 对象转数组 / 字典
来源：http://cbw.yongpay.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vkp.smart0.xyz

PHP:  get_object_vars($obj);
来源：http://opa.pycfn.com

JS:   Object.entries(obj)
来源：http://lqv.jinqigufen.top

TS:   Object.entries(obj)
来源：http://hzo.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jdz.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://emq.fengsongda.top

Ruby: obj.instance_variables
来源：http://nwi.feifeiyinyue.top

C#:   // 用反射或 System.Text.Json
来源：http://bsr.daria6918.cn

================================================================================
来源：http://uhg.cqqwz.cn

H. 异常与错误处理
来源：http://bdq.jqgufenzy.top

================================================================================
来源：http://oyh.tianlin.xyz

[H01] try / catch 基础
来源：http://vgl.fehbvm.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ais.hammf.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gfb.yangfankeji.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vqr.tian-w.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xnu.ywan-chungtsiang.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jjy.chenzaomai.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://urd.andypj.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zqv.chenjidiqi.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://akz.tanke756.top

[H02] finally / ensure 收尾
来源：http://nam.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://ihb.uphjek.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://tcv.guowangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ivj.hesvh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://txb.vqdsnc.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oqo.zhengqikj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kxb.jlsjyb.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://obx.jianghu66.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://csu.shzxlz.cn

[H03] 主动抛出异常
来源：http://xxc.zycfv.cn

Py:   raise ValueError("错误信息")
来源：http://uin.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jwt.snrcjt.cn

JS:   throw new Error("错误信息");
来源：http://nsa.tarul.cn

TS:   throw new Error("错误信息");
来源：http://zwt.aibaodan.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://saq.svipenyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fdc.havefunace.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nsc.sysykeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://svr.chenzaomai.com

[H04] 自定义异常类型
来源：http://kra.zhoulong.xyz

Py:   class MyError(Exception): pass
来源：http://kri.fzhhl.top

PHP:  class MyError extends RuntimeException {}
来源：http://tow.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://mtz.shanyushiyangtech.top

TS:   class MyError extends Error {}
来源：http://sum.jlsjyb.cn

Java: class MyException extends RuntimeException {}
来源：http://nnw.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nyh.chenzaomai.com

Ruby: class MyError < StandardError; end
来源：http://sbc.hesvh.cn

C#:   class MyException : Exception {}
来源：http://zrm.yj20258888.top

[H05] 捕获特定类型
来源：http://dis.yvedp.cn

Py:   except ValueError as e:
来源：http://pov.9152youxi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wfh.havefunace.top

JS:   if (e instanceof TypeError) {}
来源：http://awg.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://run.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://nkz.fzhhl.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lxc.xuetiantiany.cn

Ruby: rescue ArgumentError => e
来源：http://qgx.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mhh.sjlbkw.cn

[H06] 可选值 / 空值安全访问
来源：http://zdq.gaohongyu789.top

Py:   value = d.get("k") or default
来源：http://iwt.guannengcc.top

PHP:  $v = $d["k"] ?? null;
来源：http://ysh.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://ini.fengsongda.top

TS:   obj?.a?.b;  d ?? default
来源：http://yjk.aibaodan.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eip.jyoumei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fhy.ydzc1.top

Ruby: d&.dig(:a, :b)
来源：http://gpp.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://kel.jinyuanbaomall.cn

[H07] 断言
来源：http://ejt.yvedp.cn

Py:   assert x > 0, "必须为正"
来源：http://grw.cucudq.cn

PHP:  assert($x > 0);
来源：http://fix.chenjidiqi.icu

JS:   console.assert(x > 0);
来源：http://bzd.wangdashe.top

TS:   console.assert(x > 0);
来源：http://mkt.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://rrt.nwbrower.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zfy.shanyushiyangtech.top

Ruby: raise "必须为正" unless x > 0
来源：http://nwd.daria6918.cn

C#:   Debug.Assert(x > 0);
来源：http://lli.cqqwz.cn

[H08] 获取错误信息与堆栈
来源：http://ase.nwbrower.top

Py:   str(e);  traceback.format_exc()
来源：http://agw.redwolf501.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xyk.hammf.cn

JS:   e.message;  e.stack
来源：http://jfr.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xaw.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xzq.nanxinkj.top

Go:   err.Error()
来源：http://bon.svipenyu.cn

Ruby: e.message;  e.backtrace
来源：http://zjz.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://kew.yvedp.cn

[H09] 带错误码的异常
来源：http://vzb.gaohongyu789.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yno.ywan-chungtsiang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xlc.ehwqpu.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dbf.316326.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fdp.xylfe.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ykk.sxryk.cn


<!-- 参考信息 -->