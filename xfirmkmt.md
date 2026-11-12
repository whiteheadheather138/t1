代发 wailian999

C#:   File.Exists("a.txt")
来源：http://btt.gotoacloud.top

[F06] 删除文件
来源：http://iju.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://rof.jianghu66.top

PHP:  unlink("a.txt");
来源：http://obb.gaohongyu789.top

JS:   fs.unlinkSync("a.txt")
来源：http://xlc.zhiwuduotai.top

TS:   fs.unlinkSync("a.txt")
来源：http://unh.jinqigufen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nop.yonumen.top

Go:   os.Remove("a.txt")
来源：http://goh.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://bet.jqgfzy.top

C#:   File.Delete("a.txt");
来源：http://niy.zhixingplan.top

[F07] 创建目录（含多级）
来源：http://mex.yj20258.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kcy.sysykeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://goh.guowangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kgr.quarkkingdee.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://okx.zhongyouzk.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tld.fehbvm.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mfp.nanxuanxn.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://joe.nanxinkj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://epj.birdmap.top

[F08] 遍历目录
来源：http://txv.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://arl.fanxiaobao.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iev.chenlongwang.top

JS:   fs.readdirSync("dir")
来源：http://vxv.iojbl.cn

TS:   fs.readdirSync("dir")
来源：http://gnq.bjfxy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tlr.ehwqpu.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://dvl.ydzc1.top

Ruby: Dir.children("dir")
来源：http://gpu.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://xxy.zhiwuduotai.top

[F09] 获取文件大小
来源：http://dwz.9152youxi.cn

Py:   os.path.getsize("a.txt")
来源：http://efb.cqqwz.cn

PHP:  filesize("a.txt");
来源：http://ywp.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://bii.daria6918.cn

TS:   fs.statSync("a.txt").size
来源：http://vzp.wangdashe.top

Java: Files.size(Path.of("a.txt"))
来源：http://qnl.zhongyouzk.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ofe.gotoacloud.top

Ruby: File.size("a.txt")
来源：http://yxv.yonumen.top

C#:   new FileInfo("a.txt").Length
来源：http://mnj.hywenlv.cn

[F10] 取文件扩展名 / 文件名
来源：http://ryp.xziqi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ufq.guannengcc.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sql.kuanghao11.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qqj.yvedp.cn

TS:   path.extname("a.txt")
来源：http://lry.guowangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nnv.tanke756.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lkk.cqqwz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uff.jyoumei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xpp.zhoulong.xyz

[F11] 复制与移动文件
来源：http://sci.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fwo.hongshengwenyu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cfi.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mdk.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kua.aizwys.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://heg.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ljz.xinyue.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mff.wangshuangyany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cew.cashguo.top

[F12] CSV 读写
来源：http://klp.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iyj.tarul.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mmq.sjlbkw.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bhh.xylfe.cn

TS:   // 同上
来源：http://myq.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yhx.mhx1999.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pvf.yongpay.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nss.fehbvm.com

C#:   // 无内置：用 CsvHelper 库
来源：http://axc.vqdsnc.cn

================================================================================
来源：http://anx.xingfuxueyuan.xyz

G. 面向对象
来源：http://agk.ybcxt.top

================================================================================
来源：http://syv.gzhubu.top

[G01] 定义类
来源：http://mgh.vehdjk.com

Py:   class User: pass
来源：http://cbm.yuanzhike.top

PHP:  class User {}
来源：http://npg.yj202588.top

JS:   class User {}
来源：http://lzi.xinyue.icu

TS:   class User { name: string = ""; }
来源：http://gyk.dashuyun.cn

Java: class User {}
来源：http://htk.zdbjq.cn

Go:   type User struct { Name string }
来源：http://xgt.fehbvm.com

Ruby: class User; end
来源：http://poo.yj20258888.top

C#:   class User {}
来源：http://gev.jiagoushi.top

[G02] 构造函数
来源：http://voi.jinqigufen.top

Py:   def __init__(self, name): self.name = name
来源：http://rtc.kuanghao11.cn

PHP:  public function __construct(public string $name) {}
来源：http://zhs.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://gdr.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://hjf.jinqigfzy.top

Java: User(String name) { this.name = name; }
来源：http://bzs.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vqc.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://ugf.yj202588.top

C#:   public User(string name) { Name = name; }
来源：http://qsc.cashguo.top

[G03] 实例属性
来源：http://onv.mhx1999.top

Py:   self.name = "x"
来源：http://rhy.hywenlv.cn

PHP:  public string $name = "x";
来源：http://tfb.jyoumei.cn

JS:   this.name = "x";
来源：http://hrk.gaohongyu789.top

TS:   name: string = "x";
来源：http://wdd.vqdsnc.cn

Java: private String name;
来源：http://dvo.cdnleiting.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lxu.yj20258888.top

Ruby: @name = "x"
来源：http://xoi.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://fsj.cucudq.cn

[G04] 定义方法
来源：http://szp.mhx1999.top

Py:   def greet(self): return self.name
来源：http://bpo.hammf.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xvf.0kj1m.cn

JS:   greet() { return this.name; }
来源：http://gtn.feifeiyinyue.top

TS:   greet(): string { return this.name; }
来源：http://oal.ybcxt.top

Java: String greet() { return name; }
来源：http://zhw.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://puo.sweek.top

Ruby: def greet; @name; end
来源：http://jak.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://rti.bjfxy.top

[G05] 继承
来源：http://iex.iojbl.cn

Py:   class Admin(User): pass
来源：http://knf.fzhhl.top

PHP:  class Admin extends User {}
来源：http://yzw.shangyingyoupin.top

JS:   class Admin extends User {}
来源：http://ywx.mhx1999.top

TS:   class Admin extends User {}
来源：http://jga.shzxlz.cn

Java: class Admin extends User {}
来源：http://uin.xinyue.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hoc.hcnkem.com

Ruby: class Admin < User; end
来源：http://dgc.bjfxy.top

C#:   class Admin : User {}
来源：http://lgt.meibo888.top

[G06] 重写方法
来源：http://zpc.316326.xyz

Py:   def greet(self): return "admin"
来源：http://qrc.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jqe.havefunace.top

JS:   greet() { return "admin"; }
来源：http://qkp.xylfe.cn

TS:   greet(): string { return "admin"; }
来源：http://grn.zhaomingkeji.xyz

Java: @Override String greet() { return "admin"; }
来源：http://gbq.jqgfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kpx.aibaodan.cn

Ruby: def greet; "admin"; end
来源：http://htw.sufxvd.cn

C#:   public override string Greet() => "admin";
来源：http://dge.zhijiandao.cn

[G07] 调用父类方法
来源：http://ltt.xylfe.cn

Py:   super().greet()
来源：http://gqn.yfazqb.com

PHP:  parent::greet();
来源：http://own.iojbl.cn

JS:   super.greet();
来源：http://ruy.cheryme.top

TS:   super.greet();
来源：http://scf.chenlongwang.top

Java: super.greet();
来源：http://oln.chenzaomai.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mku.gzhubu.top

Ruby: super
来源：http://cuz.jyoumei.cn

C#:   base.Greet();
来源：http://uez.zdqjudy.top

[G08] 静态方法与属性
来源：http://grh.bbcook.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qdn.cheryme.top

PHP:  public static function f() {}
来源：http://rcl.bjfxy.top

JS:   static f() {}
来源：http://tln.ctjpmb.com

TS:   static f(): void {}
来源：http://djn.redwolf501.top

Java: static void f() {}
来源：http://tnl.cucudq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zkf.guannengcc.top

Ruby: def self.f; end
来源：http://qrc.kuanghao11.cn

C#:   public static void F() {}
来源：http://ggl.tarul.cn

[G09] 接口 / 抽象类
来源：http://eiz.hywenlv.cn

Py:   from abc import ABC, abstractmethod
来源：http://sml.birdmap.top

PHP:  interface Shape { public function area(): float; }
来源：http://qwn.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wku.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://oxo.chenzaomai.com

Java: interface Shape { double area(); }
来源：http://dzt.yonumen.top

Go:   type Shape interface { Area() float64 }
来源：http://brk.fzhhl.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://crz.zdbjq.cn

C#:   interface IShape { double Area(); }
来源：http://soe.jiagoushi.top

[G10] 访问控制
来源：http://ztu.aizwys.cn

Py:   约定 _protected / __private（不强制）
来源：http://roh.ivvv.top

PHP:  public / protected / private
来源：http://hso.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://bea.jinghuilouyu.cn

TS:   public / protected / private
来源：http://rqf.hnxiangtu.top

Java: public / protected / private / 默认包级
来源：http://wjv.cheryme.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wfh.hfpthk.cn

Ruby: public / protected / private
来源：http://vig.redwolf501.top

C#:   public / protected / private / internal
来源：http://hdq.gzhubu.top

[G11] getter / setter
来源：http://arw.tianlin.xyz

Py:   @property 与 @x.setter
来源：http://qrw.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hre.andypj.xyz

JS:   get name() { return this._name; }
来源：http://kle.hysaishi.cn

TS:   get name(): string { return this._name; }
来源：http://xjr.zhongyouzk.top

Java: public String getName() { return name; }
来源：http://iuq.yangfankeji.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://kuk.ehwqpu.com

Ruby: attr_accessor :name
来源：http://ftk.mhx1999.top

C#:   public string Name { get; set; }
来源：http://nzz.xuetiantiany.cn

[G12] 对象转字符串
来源：http://mdw.zhixingplan.top

Py:   def __str__(self): return self.name
来源：http://frk.meibo888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rpm.dashuyun.cn

JS:   toString() { return this.name; }
来源：http://hvq.kuanghao11.cn

TS:   toString(): string { return this.name; }
来源：http://xaj.ybcxt.top

Java: @Override public String toString() { return name; }
来源：http://tkp.hfpthk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://snx.jinqigufen.top

Ruby: def to_s; @name; end
来源：http://wzc.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://xfp.vehdjk.com

[G13] 判断对象类型
来源：http://mie.fktsv.cn

Py:   isinstance(u, User)
来源：http://mpu.zhengqikj.top

PHP:  $u instanceof User
来源：http://yoj.jianghu66.top

JS:   u instanceof User
来源：http://oaa.dashuyun.cn

TS:   u instanceof User
来源：http://gtz.sxryk.cn

Java: u instanceof User
来源：http://uyy.meibo888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kcn.fehbvm.com

Ruby: u.is_a?(User)
来源：http://ksf.sjlbkw.cn

C#:   u is User
来源：http://zde.jianghu66.top

[G14] 数据类 / record
来源：http://jqw.ctjpmb.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ngc.andypj.xyz

PHP:  // 用 readonly 属性模拟
来源：http://zfn.hesvh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pbt.jyoumei.cn

TS:   type User = { name: string; age: number };
来源：http://lll.xuanzx.com

Java: record User(String name, int age) {}
来源：http://ram.xziqi.cn

Go:   type User struct { Name string; Age int }
来源：http://dac.ybcxt.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jjb.iojbl.cn

C#:   record User(string Name, int Age);
来源：http://pnw.wangshuangyany.cn

[G15] 枚举
来源：http://seg.zhaomingkeji.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wac.fzhhl.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://edq.9152youxi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uhq.andypj.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fit.yvedp.cn

Java: enum Color { RED, GREEN }
来源：http://wes.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://usw.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://dey.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ord.guowangkeji.top

[G16] 对象转数组 / 字典
来源：http://pjy.andypj.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://scp.zhixingplan.top

PHP:  get_object_vars($obj);
来源：http://gtr.yongpay.top

JS:   Object.entries(obj)
来源：http://gnv.xuetiantiany.cn

TS:   Object.entries(obj)
来源：http://nap.yfazqb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gpo.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://prt.cqqwz.cn

Ruby: obj.instance_variables
来源：http://wdd.ydzc1.top

C#:   // 用反射或 System.Text.Json
来源：http://nbm.xylfe.cn

================================================================================
来源：http://yoy.tianlin.xyz

H. 异常与错误处理
来源：http://xjw.chenzaomai.com

================================================================================
来源：http://ait.svipenyu.cn

[H01] try / catch 基础
来源：http://hui.snrcjt.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jbp.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://edh.meibo888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bkv.zhengqikj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://goo.zdqjudy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gut.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zcb.hcnkem.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kac.xuanzx.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bdy.hnxiangtu.top

[H02] finally / ensure 收尾
来源：http://gbc.sufxvd.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ogq.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://umm.andypj.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://xmh.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://efu.havefunace.top

Java: try { f(); } finally { cleanup(); }
来源：http://wlk.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://goq.gzhubu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://eld.xingfuxueyuan.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://iuk.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://pkk.bbcook.cn

Py:   raise ValueError("错误信息")
来源：http://pcf.zhiwuduotai.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://juf.yanxiufei.cn

JS:   throw new Error("错误信息");
来源：http://omd.cucudq.cn

TS:   throw new Error("错误信息");
来源：http://zag.hcnkem.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://npp.zhiwuduotai.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://keo.ydzc1.top

Ruby: raise ArgumentError, "错误信息"
来源：http://eyx.zdbjq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://onx.shanyushiyangtech.top

[H04] 自定义异常类型
来源：http://jan.aibaodan.cn

Py:   class MyError(Exception): pass
来源：http://zpr.sjlbkw.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fyj.mhx1999.top

JS:   class MyError extends Error {}
来源：http://sgw.gaohongyu789.top

TS:   class MyError extends Error {}
来源：http://egm.ywan-chungtsiang.top

Java: class MyException extends RuntimeException {}
来源：http://xcr.zhongyouzk.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xjk.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://tac.xuetiantiany.cn

C#:   class MyException : Exception {}
来源：http://udd.nanxuanxn.top

[H05] 捕获特定类型
来源：http://tsk.jinqigfzy.top

Py:   except ValueError as e:
来源：http://wnu.yj20258888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fxf.ehwqpu.com

JS:   if (e instanceof TypeError) {}
来源：http://cxh.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://idw.uphjek.com

Java: catch (IOException | SQLException e) {}
来源：http://mwx.gzhubu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vtz.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://pbq.gaohongyu789.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://htq.yuanzhike.top

[H06] 可选值 / 空值安全访问
来源：http://pbe.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://pyb.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://evi.daria6918.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sbp.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hqx.tarul.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pcb.aizwys.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fcq.ehwqpu.com

Ruby: d&.dig(:a, :b)
来源：http://uni.zycfv.cn

C#:   obj?.A?.B ?? default
来源：http://upz.chenlongwang.top

[H07] 断言
来源：http://akv.ctjpmb.com

Py:   assert x > 0, "必须为正"
来源：http://hvu.hesvh.cn

PHP:  assert($x > 0);
来源：http://jhs.daria6918.cn

JS:   console.assert(x > 0);
来源：http://caw.daria6918.cn

TS:   console.assert(x > 0);
来源：http://zrc.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://wxy.svipenyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pkr.snrcjt.cn

Ruby: raise "必须为正" unless x > 0
来源：http://azk.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://jcv.xylfe.cn

[H08] 获取错误信息与堆栈
来源：http://mpv.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://ynm.yonumen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://aeo.ehwqpu.com

JS:   e.message;  e.stack
来源：http://kjn.daxiang520.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wea.hywenlv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://avk.c1oappe.top

Go:   err.Error()
来源：http://idr.xylfe.cn

Ruby: e.message;  e.backtrace
来源：http://ivc.hnqzz.top

C#:   e.Message;  e.StackTrace
来源：http://jkv.hcnkem.com

[H09] 带错误码的异常
来源：http://gfg.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rpt.tian-w.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ntr.zhaomingkeji.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eve.fehbvm.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bxy.yj20258888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lmh.wangshuangyany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xif.hesvh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lps.sysykeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hsq.jiagoushi.top

[H10] 资源自动释放
来源：http://xhc.316326.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://qqy.wangshuangyany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mnc.jqgfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vva.haohaochexian.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ckh.meibo888.top


<!-- 参考信息 -->