代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xft.yanxiufei.cn

Ruby: File.write("a.txt", "hi")
来源：http://gfi.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cmt.fengsongda.top

[F04] 追加写入文件
来源：http://dkv.havefunace.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mvp.mhx1999.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://smt.redwolf501.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xen.uphjek.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jln.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kxh.nwbrower.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qiq.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gfg.feifeiyinyue.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://chr.chenzaomai.com

[F05] 判断文件或目录是否存在
来源：http://ngb.xuanzx.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wlm.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://qmx.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://spl.hfpthk.cn

TS:   fs.existsSync("a.txt")
来源：http://bno.quarkkingdee.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qkc.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zwk.yuanzhike.top

Ruby: File.exist?("a.txt")
来源：http://tjp.zhixingplan.top

C#:   File.Exists("a.txt")
来源：http://usf.kuanghao11.cn

[F06] 删除文件
来源：http://yym.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://ixj.9152youxi.cn

PHP:  unlink("a.txt");
来源：http://fds.sufxvd.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xfw.tianlin.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://ujr.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gdd.shuidangran.top

Go:   os.Remove("a.txt")
来源：http://qsa.shangyingyoupin.top

Ruby: File.delete("a.txt")
来源：http://xgb.cqqwz.cn

C#:   File.Delete("a.txt");
来源：http://qeg.chenlongwang.top

[F07] 创建目录（含多级）
来源：http://yhl.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gve.birdmap.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gtl.fehbvm.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tpk.nwbrower.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qqm.aizwys.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://snx.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vhn.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dqx.iojbl.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://muw.yj202588.top

[F08] 遍历目录
来源：http://nnu.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jti.chenlongwang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mhw.ivvv.top

JS:   fs.readdirSync("dir")
来源：http://kbp.shzxlz.cn

TS:   fs.readdirSync("dir")
来源：http://kxj.xinyue.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://agi.jinyuanbaomall.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fjl.zhengqikj.top

Ruby: Dir.children("dir")
来源：http://wgm.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://heb.daxiang520.top

[F09] 获取文件大小
来源：http://tjq.ydjk.org.cn

Py:   os.path.getsize("a.txt")
来源：http://qno.gaohongyu789.top

PHP:  filesize("a.txt");
来源：http://yuz.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://njy.jqgufenzy.top

TS:   fs.statSync("a.txt").size
来源：http://ylu.vqdsnc.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dbg.ywan-chungtsiang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dns.zycfv.cn

Ruby: File.size("a.txt")
来源：http://ope.sxryk.cn

C#:   new FileInfo("a.txt").Length
来源：http://abf.dianchejie.cn

[F10] 取文件扩展名 / 文件名
来源：http://dny.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://skd.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fof.tanke756.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ons.havefunace.top

TS:   path.extname("a.txt")
来源：http://bkk.snrcjt.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ofs.hesvh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uvg.fengsongda.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pnh.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kjp.guannengcc.top

[F11] 复制与移动文件
来源：http://jco.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fox.fanxiaobao.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xwq.uphjek.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://txt.yj202588.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aom.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jpi.cashguo.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xtt.yongpay.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xqx.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pfz.sweek.top

[F12] CSV 读写
来源：http://igt.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oiu.ydjk.org.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nse.feifeiyinyue.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://egn.fengsongda.top

TS:   // 同上
来源：http://csy.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ofg.jiagoushi.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://onf.xuetiantiany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fcl.c1oappe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tue.sysykeji.top

================================================================================
来源：http://aex.yongpay.top

G. 面向对象
来源：http://zvo.yj20258888.top

================================================================================
来源：http://pfy.gogol.net.cn

[G01] 定义类
来源：http://wff.jianghu66.top

Py:   class User: pass
来源：http://nws.snrcjt.cn

PHP:  class User {}
来源：http://eds.snrcjt.cn

JS:   class User {}
来源：http://pba.0kj1m.cn

TS:   class User { name: string = ""; }
来源：http://yix.tarul.cn

Java: class User {}
来源：http://ijm.pycfn.com

Go:   type User struct { Name string }
来源：http://xbh.jiagoushi.top

Ruby: class User; end
来源：http://lzt.ybcxt.top

C#:   class User {}
来源：http://ukc.shuidangran.top

[G02] 构造函数
来源：http://ovf.daria6918.cn

Py:   def __init__(self, name): self.name = name
来源：http://tkr.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://mnw.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://zwz.ehwqpu.com

TS:   constructor(public name: string) {}
来源：http://pva.yuanzhike.top

Java: User(String name) { this.name = name; }
来源：http://fts.snrcjt.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://noe.zhaomingkeji.xyz

Ruby: def initialize(name); @name = name; end
来源：http://adp.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://jsl.zhijiandao.cn

[G03] 实例属性
来源：http://pbo.daria6918.cn

Py:   self.name = "x"
来源：http://tuy.sysykeji.top

PHP:  public string $name = "x";
来源：http://hxj.nanxuanxn.top

JS:   this.name = "x";
来源：http://gpr.9152youxi.cn

TS:   name: string = "x";
来源：http://jmd.zhiwuduotai.top

Java: private String name;
来源：http://nth.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zgj.fktsv.cn

Ruby: @name = "x"
来源：http://dwk.nwbrower.top

C#:   public string Name { get; set; } = "x";
来源：http://zif.xinyue.icu

[G04] 定义方法
来源：http://vrq.cashguo.top

Py:   def greet(self): return self.name
来源：http://enj.9152youxi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ykq.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://oql.fanxiaobao.xyz

TS:   greet(): string { return this.name; }
来源：http://bwe.hcnkem.com

Java: String greet() { return name; }
来源：http://yax.ydzc1.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qjw.mhx1999.top

Ruby: def greet; @name; end
来源：http://jyj.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://mab.cdnleiting.top

[G05] 继承
来源：http://pfv.zhixingplan.top

Py:   class Admin(User): pass
来源：http://pny.yangfankeji.com

PHP:  class Admin extends User {}
来源：http://uif.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://scx.jqgufenzy.top

TS:   class Admin extends User {}
来源：http://ruu.ppjwa.cn

Java: class Admin extends User {}
来源：http://bjt.zhoulong.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://akg.chenlongwang.top

Ruby: class Admin < User; end
来源：http://eon.cqqwz.cn

C#:   class Admin : User {}
来源：http://cha.cdnleiting.top

[G06] 重写方法
来源：http://dpm.vqdsnc.cn

Py:   def greet(self): return "admin"
来源：http://kai.zycfv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zyl.yuxming.cn

JS:   greet() { return "admin"; }
来源：http://gwo.tanke756.top

TS:   greet(): string { return "admin"; }
来源：http://nxl.xziqi.cn

Java: @Override String greet() { return "admin"; }
来源：http://xxd.sweek.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oee.aizwys.cn

Ruby: def greet; "admin"; end
来源：http://rxs.316326.xyz

C#:   public override string Greet() => "admin";
来源：http://ykm.ydzc1.top

[G07] 调用父类方法
来源：http://vav.jinyuanbaomall.cn

Py:   super().greet()
来源：http://eoc.zdqjudy.top

PHP:  parent::greet();
来源：http://dor.sxryk.cn

JS:   super.greet();
来源：http://ppa.yuxming.cn

TS:   super.greet();
来源：http://nzi.ctjpmb.com

Java: super.greet();
来源：http://ham.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xew.vehdjk.com

Ruby: super
来源：http://dou.dianchejie.cn

C#:   base.Greet();
来源：http://uxz.shanyushiyangkeji.top

[G08] 静态方法与属性
来源：http://fhx.shuidangran.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ofq.tarul.cn

PHP:  public static function f() {}
来源：http://lqb.yonumen.top

JS:   static f() {}
来源：http://kkk.tanke756.top

TS:   static f(): void {}
来源：http://exn.ywan-chungtsiang.top

Java: static void f() {}
来源：http://otx.redwolf501.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ncw.cheryme.top

Ruby: def self.f; end
来源：http://uly.zhoulong.xyz

C#:   public static void F() {}
来源：http://abm.zhixingplan.top

[G09] 接口 / 抽象类
来源：http://juo.fanxiaobao.xyz

Py:   from abc import ABC, abstractmethod
来源：http://kez.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lto.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bwe.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://fzm.birdmap.top

Java: interface Shape { double area(); }
来源：http://kux.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://sfq.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vcm.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://beo.fktsv.cn

[G10] 访问控制
来源：http://xde.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://tjz.yangfankeji.com

PHP:  public / protected / private
来源：http://yxl.jinyuanbaomall.cn

JS:   #private 字段；其余公开
来源：http://zox.jqgufenzy.top

TS:   public / protected / private
来源：http://zqu.jinghuilouyu.cn

Java: public / protected / private / 默认包级
来源：http://xdg.cheryme.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gbz.yuanzhike.top

Ruby: public / protected / private
来源：http://qyp.yongpay.top

C#:   public / protected / private / internal
来源：http://ujd.yj20258888.top

[G11] getter / setter
来源：http://eli.xuetiantiany.cn

Py:   @property 与 @x.setter
来源：http://thz.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://toj.hywenlv.cn

JS:   get name() { return this._name; }
来源：http://axi.jqgufenzy.top

TS:   get name(): string { return this._name; }
来源：http://eul.shuidangran.top

Java: public String getName() { return name; }
来源：http://pgj.yanxiufei.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://svh.shanyushiyangkeji.top

Ruby: attr_accessor :name
来源：http://sow.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://ifw.kuanghao11.cn

[G12] 对象转字符串
来源：http://bvr.daxiang520.top

Py:   def __str__(self): return self.name
来源：http://jeq.shangyingyoupin.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xzg.cqqwz.cn

JS:   toString() { return this.name; }
来源：http://ihe.sweek.top

TS:   toString(): string { return this.name; }
来源：http://uws.nanxinkj.top

Java: @Override public String toString() { return name; }
来源：http://ujv.ydzc1.top

Go:   func (u User) String() string { return u.Name }
来源：http://hpt.tianlin.xyz

Ruby: def to_s; @name; end
来源：http://ijc.chenzaomai.com

C#:   public override string ToString() => Name;
来源：http://ntf.hongshengwenyu.top

[G13] 判断对象类型
来源：http://gba.316326.xyz

Py:   isinstance(u, User)
来源：http://cus.smart0.xyz

PHP:  $u instanceof User
来源：http://ljr.snrcjt.cn

JS:   u instanceof User
来源：http://ubm.jinqigufen.top

TS:   u instanceof User
来源：http://pnx.pengpengdd.cyou

Java: u instanceof User
来源：http://nty.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://neg.gzhubu.top

Ruby: u.is_a?(User)
来源：http://tvm.mhx1999.top

C#:   u is User
来源：http://vbr.yonumen.top

[G14] 数据类 / record
来源：http://mcz.svipenyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qnq.yj20258888.top

PHP:  // 用 readonly 属性模拟
来源：http://ijd.hnxiangtu.top

JS:   // 无内置：普通类或对象字面量
来源：http://hwh.ehwqpu.com

TS:   type User = { name: string; age: number };
来源：http://ucs.wangdashe.top

Java: record User(String name, int age) {}
来源：http://mkv.ydjk.org.cn

Go:   type User struct { Name string; Age int }
来源：http://oal.jinyuanbaomall.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nsn.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://vnq.tianlin.xyz

[G15] 枚举
来源：http://wpz.cucudq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aon.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dob.aibaodan.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ozm.jqgufenzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xan.svipenyu.cn

Java: enum Color { RED, GREEN }
来源：http://mxb.dashuyun.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tmf.fktsv.cn

Ruby: Color = %i[red green].freeze
来源：http://qof.yueranfly.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://auy.jlsjyb.cn

[G16] 对象转数组 / 字典
来源：http://fpr.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zlg.snrcjt.cn

PHP:  get_object_vars($obj);
来源：http://nqx.gotoacloud.top

JS:   Object.entries(obj)
来源：http://jqs.fktsv.cn

TS:   Object.entries(obj)
来源：http://ayg.guannengcc.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mum.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://iqh.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://bza.zhongyouzk.top

C#:   // 用反射或 System.Text.Json
来源：http://ldt.ybcxt.top

================================================================================
来源：http://oun.feifeiyinyue.top

H. 异常与错误处理
来源：http://hsw.meibo888.top

================================================================================
来源：http://rpm.hnxiangtu.top

[H01] try / catch 基础
来源：http://zro.ivvv.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://geo.shanyushiyangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aky.hongshengwenyu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fqf.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wzf.yj20258.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hyx.meibo888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jmm.wangshuangyany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ywt.aizwys.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yew.wangdashe.top

[H02] finally / ensure 收尾
来源：http://isx.quarkkingdee.top

Py:   try: f()⏎finally: cleanup()
来源：http://nzv.nanxuanxn.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kgo.yj20258888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://uci.zdqjudy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://weh.vqdsnc.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wwg.xylfe.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dne.nanxinkj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bps.yj20258.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://oyk.aibaodan.cn

[H03] 主动抛出异常
来源：http://gsw.chenzaomai.com

Py:   raise ValueError("错误信息")
来源：http://zgt.c1oappe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://llj.jinqigufen.top

JS:   throw new Error("错误信息");
来源：http://bdv.sufxvd.cn

TS:   throw new Error("错误信息");
来源：http://ffq.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qrh.yfazqb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mnp.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dbd.xuanzx.com

C#:   throw new ArgumentException("错误信息");
来源：http://tro.ppjwa.cn

[H04] 自定义异常类型
来源：http://qnk.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://hie.jinyuanbaomall.cn

PHP:  class MyError extends RuntimeException {}
来源：http://krb.daria6918.cn

JS:   class MyError extends Error {}
来源：http://hsq.aizwys.cn

TS:   class MyError extends Error {}
来源：http://ocv.mhx1999.top

Java: class MyException extends RuntimeException {}
来源：http://uzr.tian-w.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wwq.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://nqp.cashguo.top

C#:   class MyException : Exception {}
来源：http://rbk.shanyushiyangtech.top

[H05] 捕获特定类型
来源：http://vgn.svipenyu.cn

Py:   except ValueError as e:
来源：http://fwp.yueranfly.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://orp.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://fnw.zycfv.cn

TS:   if (e instanceof TypeError) {}
来源：http://tll.svipenyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://vey.sjlbkw.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ygs.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://ofk.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fjn.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://jps.zhoulong.xyz

Py:   value = d.get("k") or default
来源：http://fnw.nanxinkj.top

PHP:  $v = $d["k"] ?? null;
来源：http://kpm.sxryk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sir.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://tij.cqqwz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cmz.vehdjk.com

Go:   if v, ok := m["k"]; ok { }
来源：http://rbp.fanxiaobao.xyz

Ruby: d&.dig(:a, :b)
来源：http://qbl.shangyingyoupin.top

C#:   obj?.A?.B ?? default
来源：http://ljo.zhongyouzk.top

[H07] 断言
来源：http://eax.tianlin.xyz

Py:   assert x > 0, "必须为正"
来源：http://uwc.yj202588.top

PHP:  assert($x > 0);
来源：http://xsc.andypj.xyz

JS:   console.assert(x > 0);
来源：http://cfa.yfazqb.com

TS:   console.assert(x > 0);
来源：http://jyq.ywan-chungtsiang.top

Java: assert x > 0 : "必须为正";
来源：http://mvc.cucudq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://imr.jinyuanbaomall.cn

Ruby: raise "必须为正" unless x > 0
来源：http://eqb.nwbrower.top

C#:   Debug.Assert(x > 0);
来源：http://owc.ywan-chungtsiang.top

[H08] 获取错误信息与堆栈
来源：http://qoz.ydzc1.top

Py:   str(e);  traceback.format_exc()
来源：http://cup.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nft.ppjwa.cn


<!-- 参考信息 -->