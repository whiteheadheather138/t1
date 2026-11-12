代发 wailian999

Ruby: File.delete("a.txt")
来源：http://mxo.yonumen.top

C#:   File.Delete("a.txt");
来源：http://nko.andypj.xyz

[F07] 创建目录（含多级）
来源：http://qaq.zdbjq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sxg.wangshuangyany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ldq.fktsv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gcx.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vlk.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eyy.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://exz.svipenyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://isg.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ypk.shangyingyoupin.top

[F08] 遍历目录
来源：http://ufd.zdqjudy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jgd.shangyingyoupin.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dca.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://dfh.ppjwa.cn

TS:   fs.readdirSync("dir")
来源：http://gox.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://reg.hysaishi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jnx.yanxiufei.cn

Ruby: Dir.children("dir")
来源：http://sor.chenlongwang.top

C#:   Directory.GetFiles("dir")
来源：http://qem.iojbl.cn

[F09] 获取文件大小
来源：http://iap.sjlbkw.cn

Py:   os.path.getsize("a.txt")
来源：http://nib.sxryk.cn

PHP:  filesize("a.txt");
来源：http://ygi.chenlongwang.top

JS:   fs.statSync("a.txt").size
来源：http://vic.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://pvr.gaohongyu789.top

Java: Files.size(Path.of("a.txt"))
来源：http://rpk.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pra.fzhhl.top

Ruby: File.size("a.txt")
来源：http://zoi.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://ttd.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://cyc.52xcode.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hts.wangshuangyany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xiu.yvedp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lxa.vqdsnc.cn

TS:   path.extname("a.txt")
来源：http://qrh.yj20258.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rdv.hywenlv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fyr.tanke756.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kjd.nanxinkj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://msa.9152youxi.cn

[F11] 复制与移动文件
来源：http://xem.chenjidiqi.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kre.wangdashe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iqw.yj202588.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pkv.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iqg.svipenyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rjj.cdnleiting.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hqf.xinyue.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://amk.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fur.hnqzz.top

[F12] CSV 读写
来源：http://hix.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://btj.chenlongwang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ymp.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ihy.nanxinkj.top

TS:   // 同上
来源：http://kpx.zhoulong.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pjn.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fla.svipenyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ero.hnxiangtu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mgd.bjfxy.top

================================================================================
来源：http://kxn.cqqwz.cn

G. 面向对象
来源：http://snn.zhiwuduotai.top

================================================================================
来源：http://ckq.wangshuangyany.cn

[G01] 定义类
来源：http://fcy.cheryme.top

Py:   class User: pass
来源：http://oly.316326.xyz

PHP:  class User {}
来源：http://pmk.meibo888.top

JS:   class User {}
来源：http://efu.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://qmk.zhoulong.xyz

Java: class User {}
来源：http://ueb.fktsv.cn

Go:   type User struct { Name string }
来源：http://pwq.hnqzz.top

Ruby: class User; end
来源：http://zzb.ivvv.top

C#:   class User {}
来源：http://geb.ppjwa.cn

[G02] 构造函数
来源：http://wds.redwolf501.top

Py:   def __init__(self, name): self.name = name
来源：http://urv.jqgufenzy.top

PHP:  public function __construct(public string $name) {}
来源：http://hnd.fengsongda.top

JS:   constructor(name) { this.name = name; }
来源：http://qex.yvedp.cn

TS:   constructor(public name: string) {}
来源：http://eyx.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://tha.havefunace.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hsk.guowangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://ato.jinqigufen.top

C#:   public User(string name) { Name = name; }
来源：http://wss.bjfxy.top

[G03] 实例属性
来源：http://kyi.kuanghao11.cn

Py:   self.name = "x"
来源：http://qzw.yuxming.cn

PHP:  public string $name = "x";
来源：http://hxa.zhengqikj.top

JS:   this.name = "x";
来源：http://xxp.uphjek.com

TS:   name: string = "x";
来源：http://cpe.shanyushiyangtech.top

Java: private String name;
来源：http://kva.jqgfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kui.zhixingplan.top

Ruby: @name = "x"
来源：http://tci.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://akk.9152youxi.cn

[G04] 定义方法
来源：http://wjp.daria6918.cn

Py:   def greet(self): return self.name
来源：http://tyb.aibaodan.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hde.pengpengdd.cyou

JS:   greet() { return this.name; }
来源：http://fng.jianghu66.top

TS:   greet(): string { return this.name; }
来源：http://wjj.zdbjq.cn

Java: String greet() { return name; }
来源：http://msm.vqdsnc.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qzv.hnqzz.top

Ruby: def greet; @name; end
来源：http://pbp.uphjek.com

C#:   public string Greet() => Name;
来源：http://isl.quarkkingdee.top

[G05] 继承
来源：http://yho.yanxiufei.cn

Py:   class Admin(User): pass
来源：http://qoh.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://ehx.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://gul.zhaomingkeji.xyz

TS:   class Admin extends User {}
来源：http://nfd.wangdashe.top

Java: class Admin extends User {}
来源：http://nna.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ngj.aizwys.cn

Ruby: class Admin < User; end
来源：http://fus.guannengcc.top

C#:   class Admin : User {}
来源：http://cyd.zhiwuduotai.top

[G06] 重写方法
来源：http://gfe.yangfankeji.com

Py:   def greet(self): return "admin"
来源：http://hxb.zhijiandao.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kyk.zhoulong.xyz

JS:   greet() { return "admin"; }
来源：http://gsf.pycfn.com

TS:   greet(): string { return "admin"; }
来源：http://awp.hcnkem.com

Java: @Override String greet() { return "admin"; }
来源：http://kob.jinqigufen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tfo.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://utg.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://zdd.yueranfly.top

[G07] 调用父类方法
来源：http://whn.yanxiufei.cn

Py:   super().greet()
来源：http://vxj.hfpthk.cn

PHP:  parent::greet();
来源：http://htu.vqdsnc.cn

JS:   super.greet();
来源：http://lcm.shzxlz.cn

TS:   super.greet();
来源：http://tbe.zhongyouzk.top

Java: super.greet();
来源：http://avn.ppjwa.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kzs.uphjek.com

Ruby: super
来源：http://hle.chenjidiqi.icu

C#:   base.Greet();
来源：http://nxu.c1oappe.top

[G08] 静态方法与属性
来源：http://lyw.jinqigfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pcj.guannengcc.top

PHP:  public static function f() {}
来源：http://kzu.hesvh.cn

JS:   static f() {}
来源：http://ept.cqqwz.cn

TS:   static f(): void {}
来源：http://aev.gotoacloud.top

Java: static void f() {}
来源：http://qve.yongpay.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gny.jyoumei.cn

Ruby: def self.f; end
来源：http://jam.ydzc1.top

C#:   public static void F() {}
来源：http://djr.tianlin.xyz

[G09] 接口 / 抽象类
来源：http://vyu.zycfv.cn

Py:   from abc import ABC, abstractmethod
来源：http://ryc.cucudq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vat.aizwys.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fqa.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://rno.nanxinkj.top

Java: interface Shape { double area(); }
来源：http://vgw.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://vba.xingfuxueyuan.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uhy.jqgufenzy.top

C#:   interface IShape { double Area(); }
来源：http://hln.ehwqpu.com

[G10] 访问控制
来源：http://dfw.chenlongwang.top

Py:   约定 _protected / __private（不强制）
来源：http://zny.jlsjyb.cn

PHP:  public / protected / private
来源：http://hut.sjlbkw.cn

JS:   #private 字段；其余公开
来源：http://qpo.gaohongyu789.top

TS:   public / protected / private
来源：http://lcd.shanyushiyangtech.top

Java: public / protected / private / 默认包级
来源：http://jxj.fktsv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://frh.ydjk.org.cn

Ruby: public / protected / private
来源：http://tvk.smart0.xyz

C#:   public / protected / private / internal
来源：http://wtv.yj20258.top

[G11] getter / setter
来源：http://nqy.tanke756.top

Py:   @property 与 @x.setter
来源：http://pzd.shuidangran.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yhm.iojbl.cn

JS:   get name() { return this._name; }
来源：http://qte.svipenyu.cn

TS:   get name(): string { return this._name; }
来源：http://nve.zdqjudy.top

Java: public String getName() { return name; }
来源：http://prc.cheryme.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lbx.sweek.top

Ruby: attr_accessor :name
来源：http://ygf.fktsv.cn

C#:   public string Name { get; set; }
来源：http://old.ydzc1.top

[G12] 对象转字符串
来源：http://ymd.zhijiandao.cn

Py:   def __str__(self): return self.name
来源：http://ezp.fanxiaobao.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://ewi.gzhubu.top

JS:   toString() { return this.name; }
来源：http://ypx.jianghu66.top

TS:   toString(): string { return this.name; }
来源：http://cjb.shanyushiyangkeji.top

Java: @Override public String toString() { return name; }
来源：http://wff.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://ovf.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://epj.pycfn.com

C#:   public override string ToString() => Name;
来源：http://wqr.fengsongda.top

[G13] 判断对象类型
来源：http://hoz.gotoacloud.top

Py:   isinstance(u, User)
来源：http://rao.hfpthk.cn

PHP:  $u instanceof User
来源：http://bqu.chenlongwang.top

JS:   u instanceof User
来源：http://nmq.zhixingplan.top

TS:   u instanceof User
来源：http://fvh.zhoulong.xyz

Java: u instanceof User
来源：http://fhr.zdqjudy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://phg.havefunace.top

Ruby: u.is_a?(User)
来源：http://pig.sxryk.cn

C#:   u is User
来源：http://vtz.fanxiaobao.xyz

[G14] 数据类 / record
来源：http://viz.zhongyouzk.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ogh.wangdashe.top

PHP:  // 用 readonly 属性模拟
来源：http://idx.shuidangran.top

JS:   // 无内置：普通类或对象字面量
来源：http://eec.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://kyu.nwbrower.top

Java: record User(String name, int age) {}
来源：http://irb.sjlbkw.cn

Go:   type User struct { Name string; Age int }
来源：http://fss.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://thj.cqqwz.cn

C#:   record User(string Name, int Age);
来源：http://kuq.zhongyouzk.top

[G15] 枚举
来源：http://rxj.zhaomingkeji.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ltp.xuanzx.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://ulz.hesvh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jzp.yj202588.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sar.aibaodan.cn

Java: enum Color { RED, GREEN }
来源：http://ere.guannengcc.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ppp.cqqwz.cn

Ruby: Color = %i[red green].freeze
来源：http://rqb.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qwx.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://sxf.zhiwuduotai.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sew.bbcook.cn

PHP:  get_object_vars($obj);
来源：http://spt.yueranfly.top

JS:   Object.entries(obj)
来源：http://yac.hongshengwenyu.top

TS:   Object.entries(obj)
来源：http://per.ivvv.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bmy.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://hju.wangdashe.top

Ruby: obj.instance_variables
来源：http://jsv.shzxlz.cn

C#:   // 用反射或 System.Text.Json
来源：http://lja.wangshuangyany.cn

================================================================================
来源：http://wja.jlsjyb.cn

H. 异常与错误处理
来源：http://fsl.yangfankeji.com

================================================================================
来源：http://cjj.hammf.cn

[H01] try / catch 基础
来源：http://koq.pengpengdd.cyou

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uwx.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://thp.chenzaomai.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qvf.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://znp.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xrr.yueranfly.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://edl.zdbjq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bjb.svipenyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vkv.jiagoushi.top

[H02] finally / ensure 收尾
来源：http://dcg.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://amw.sufxvd.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mht.shanyushiyangtech.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wzs.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://spr.quarkkingdee.top

Java: try { f(); } finally { cleanup(); }
来源：http://qot.fengsongda.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rhg.zhiwuduotai.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ond.shuidangran.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jfo.jiagoushi.top

[H03] 主动抛出异常
来源：http://jre.jqgufenzy.top

Py:   raise ValueError("错误信息")
来源：http://adl.hfpthk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qnj.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://mlg.nanxuanxn.top

TS:   throw new Error("错误信息");
来源：http://ete.xingfuxueyuan.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://bqi.nanxinkj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ikk.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cru.xylfe.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wit.hcnkem.com

[H04] 自定义异常类型
来源：http://lvx.guannengcc.top

Py:   class MyError(Exception): pass
来源：http://una.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sop.zhixingplan.top

JS:   class MyError extends Error {}
来源：http://spy.shzxlz.cn

TS:   class MyError extends Error {}
来源：http://dxv.jianghu66.top

Java: class MyException extends RuntimeException {}
来源：http://jcp.pengpengdd.cyou

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cip.shzxlz.cn

Ruby: class MyError < StandardError; end
来源：http://yzv.xylfe.cn

C#:   class MyException : Exception {}
来源：http://oxc.tian-w.cn

[H05] 捕获特定类型
来源：http://igk.sxryk.cn

Py:   except ValueError as e:
来源：http://zom.cashguo.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aqd.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://apu.yanxiufei.cn

TS:   if (e instanceof TypeError) {}
来源：http://ywo.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://yku.daxiang520.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fbz.guowangkeji.top

Ruby: rescue ArgumentError => e
来源：http://ajq.tian-w.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rul.yj20258888.top

[H06] 可选值 / 空值安全访问
来源：http://wlj.gaohongyu789.top

Py:   value = d.get("k") or default
来源：http://puh.shanyushiyangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://lum.ybcxt.top

JS:   obj?.a?.b;  d ?? default
来源：http://ddr.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://bcr.yueranfly.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vnu.jinqigfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hqr.hfpthk.cn

Ruby: d&.dig(:a, :b)
来源：http://oey.fehbvm.com

C#:   obj?.A?.B ?? default
来源：http://ypk.gaohongyu789.top

[H07] 断言
来源：http://mrf.zhengqikj.top

Py:   assert x > 0, "必须为正"
来源：http://nwl.zhijiandao.cn

PHP:  assert($x > 0);
来源：http://ont.yonumen.top

JS:   console.assert(x > 0);
来源：http://njt.mhx1999.top

TS:   console.assert(x > 0);
来源：http://nhs.yueranfly.top

Java: assert x > 0 : "必须为正";
来源：http://lwv.hnxiangtu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oos.sysykeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://kmy.hesvh.cn

C#:   Debug.Assert(x > 0);
来源：http://dqj.nanxuanxn.top

[H08] 获取错误信息与堆栈
来源：http://hzw.zhiwuduotai.top

Py:   str(e);  traceback.format_exc()
来源：http://yhr.yuanzhike.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bbo.tianlin.xyz

JS:   e.message;  e.stack
来源：http://htd.nwbrower.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jup.zhiwuduotai.top

Java: e.getMessage();  e.printStackTrace()
来源：http://svv.birdmap.top

Go:   err.Error()
来源：http://hww.pycfn.com

Ruby: e.message;  e.backtrace
来源：http://shs.yongpay.top

C#:   e.Message;  e.StackTrace
来源：http://vgd.shuidangran.top

[H09] 带错误码的异常
来源：http://ewo.hfpthk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sny.fehbvm.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://omn.cucudq.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zed.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hnn.yj20258888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bff.yj202588.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://evv.tianlin.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://hpu.wangshuangyany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nax.andypj.xyz

[H10] 资源自动释放
来源：http://lwn.cucudq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vtv.jlsjyb.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vwb.meibo888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jfa.ywan-chungtsiang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://exc.havefunace.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://odf.mhx1999.top

Go:   defer f.Close()
来源：http://juu.jianghu66.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ndy.jianghu66.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vdi.jqgfzy.top

================================================================================
来源：http://wdo.jianghu66.top

I. 正则表达式
来源：http://dlq.jinqigfzy.top

================================================================================
来源：http://sws.zycfv.cn

[I01] 判断是否匹配
来源：http://giy.ydjk.org.cn


<!-- 参考信息 -->