代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://xma.zhoulong.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://jvb.daxiang520.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zpa.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://hcr.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://kfz.cqqwz.cn

[F06] 删除文件
来源：http://cjl.tanke756.top

Py:   os.remove("a.txt")
来源：http://nvh.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://lpt.yanxiufei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://web.tian-w.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bly.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://olv.sjlbkw.cn

Go:   os.Remove("a.txt")
来源：http://iyb.haohaochexian.top

Ruby: File.delete("a.txt")
来源：http://qcf.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://mcb.zhongyouzk.top

[F07] 创建目录（含多级）
来源：http://nce.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fjp.wangdashe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hmh.0kj1m.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tep.fehbvm.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cnd.bbcook.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bsf.yuanzhike.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oyc.hcnkem.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wda.zhixingplan.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://czw.yangfankeji.com

[F08] 遍历目录
来源：http://axa.daria6918.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pmd.yangfankeji.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gar.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://lal.gzhubu.top

TS:   fs.readdirSync("dir")
来源：http://cid.jyoumei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ebp.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://are.shuidangran.top

Ruby: Dir.children("dir")
来源：http://spp.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://tsk.gzhubu.top

[F09] 获取文件大小
来源：http://pjw.snrcjt.cn

Py:   os.path.getsize("a.txt")
来源：http://tyz.bbcook.cn

PHP:  filesize("a.txt");
来源：http://jba.snrcjt.cn

JS:   fs.statSync("a.txt").size
来源：http://deu.daria6918.cn

TS:   fs.statSync("a.txt").size
来源：http://orn.zhengqikj.top

Java: Files.size(Path.of("a.txt"))
来源：http://pzh.0kj1m.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bxr.fktsv.cn

Ruby: File.size("a.txt")
来源：http://lui.birdmap.top

C#:   new FileInfo("a.txt").Length
来源：http://pyf.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://jcy.zhijiandao.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gul.cashguo.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://atl.cheryme.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zcf.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://iwg.wangshuangyany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cgx.sxryk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://whb.pycfn.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yyg.tianlin.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lfu.hywenlv.cn

[F11] 复制与移动文件
来源：http://lwu.vehdjk.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vdp.cheryme.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ncz.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gxv.zdbjq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://awd.9152youxi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hdb.shzxlz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fyk.ehwqpu.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zpi.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kzi.jyoumei.cn

[F12] CSV 读写
来源：http://imu.feifeiyinyue.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sns.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qpd.gaohongyu789.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yak.hcnkem.com

TS:   // 同上
来源：http://rul.gotoacloud.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xke.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xog.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://was.aizwys.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pwj.aibaodan.cn

================================================================================
来源：http://nan.gotoacloud.top

G. 面向对象
来源：http://nio.chenlongwang.top

================================================================================
来源：http://cmp.tarul.cn

[G01] 定义类
来源：http://lag.sweek.top

Py:   class User: pass
来源：http://pey.gotoacloud.top

PHP:  class User {}
来源：http://xsw.pengpengdd.cyou

JS:   class User {}
来源：http://mws.feifeiyinyue.top

TS:   class User { name: string = ""; }
来源：http://wfm.xinyue.icu

Java: class User {}
来源：http://bkd.hnqzz.top

Go:   type User struct { Name string }
来源：http://ran.hnxiangtu.top

Ruby: class User; end
来源：http://bhw.zhixingplan.top

C#:   class User {}
来源：http://ltb.mhx1999.top

[G02] 构造函数
来源：http://dyw.zhijiandao.cn

Py:   def __init__(self, name): self.name = name
来源：http://bwb.cashguo.top

PHP:  public function __construct(public string $name) {}
来源：http://kzi.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://fod.svipenyu.cn

TS:   constructor(public name: string) {}
来源：http://yzm.bbcook.cn

Java: User(String name) { this.name = name; }
来源：http://vtk.wangshuangyany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://emp.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://fci.hnxiangtu.top

C#:   public User(string name) { Name = name; }
来源：http://kpx.gotoacloud.top

[G03] 实例属性
来源：http://cuo.yuxming.cn

Py:   self.name = "x"
来源：http://bpv.aizwys.cn

PHP:  public string $name = "x";
来源：http://lts.cheryme.top

JS:   this.name = "x";
来源：http://tgw.hfpthk.cn

TS:   name: string = "x";
来源：http://jvq.yuxming.cn

Java: private String name;
来源：http://wqf.pycfn.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zmk.zdbjq.cn

Ruby: @name = "x"
来源：http://exb.jqgfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://wlz.hfpthk.cn

[G04] 定义方法
来源：http://ypy.gzhubu.top

Py:   def greet(self): return self.name
来源：http://kho.snrcjt.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hxm.jinyuanbaomall.cn

JS:   greet() { return this.name; }
来源：http://rdw.zhaomingkeji.xyz

TS:   greet(): string { return this.name; }
来源：http://faa.guowangkeji.top

Java: String greet() { return name; }
来源：http://cqh.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://fwb.sufxvd.cn

Ruby: def greet; @name; end
来源：http://myl.jianghu66.top

C#:   public string Greet() => Name;
来源：http://bug.yfazqb.com

[G05] 继承
来源：http://rgc.birdmap.top

Py:   class Admin(User): pass
来源：http://gjo.tarul.cn

PHP:  class Admin extends User {}
来源：http://ctm.yongpay.top

JS:   class Admin extends User {}
来源：http://wej.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://rrk.jlsjyb.cn

Java: class Admin extends User {}
来源：http://kox.sweek.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pyw.yuxming.cn

Ruby: class Admin < User; end
来源：http://sgo.cucudq.cn

C#:   class Admin : User {}
来源：http://znd.0kj1m.cn

[G06] 重写方法
来源：http://wui.52xcode.cn

Py:   def greet(self): return "admin"
来源：http://epw.shuidangran.top

PHP:  public function greet(): string { return "admin"; }
来源：http://sxg.cheryme.top

JS:   greet() { return "admin"; }
来源：http://igp.ywan-chungtsiang.top

TS:   greet(): string { return "admin"; }
来源：http://xwq.smart0.xyz

Java: @Override String greet() { return "admin"; }
来源：http://amb.xingfuxueyuan.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pxx.cucudq.cn

Ruby: def greet; "admin"; end
来源：http://ill.yueranfly.top

C#:   public override string Greet() => "admin";
来源：http://kem.ivvv.top

[G07] 调用父类方法
来源：http://lww.sweek.top

Py:   super().greet()
来源：http://diw.birdmap.top

PHP:  parent::greet();
来源：http://kix.zhengqikj.top

JS:   super.greet();
来源：http://ten.cheryme.top

TS:   super.greet();
来源：http://ruy.jianghu66.top

Java: super.greet();
来源：http://dyd.sjlbkw.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cxy.mhx1999.top

Ruby: super
来源：http://nxv.andypj.xyz

C#:   base.Greet();
来源：http://gxd.xinyue.icu

[G08] 静态方法与属性
来源：http://cim.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mog.xziqi.cn

PHP:  public static function f() {}
来源：http://lhw.c1oappe.top

JS:   static f() {}
来源：http://fxx.ywan-chungtsiang.top

TS:   static f(): void {}
来源：http://cki.yongpay.top

Java: static void f() {}
来源：http://cda.andypj.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://hsk.cashguo.top

Ruby: def self.f; end
来源：http://tcz.yuanzhike.top

C#:   public static void F() {}
来源：http://ljl.hcnkem.com

[G09] 接口 / 抽象类
来源：http://ukp.ydzc1.top

Py:   from abc import ABC, abstractmethod
来源：http://kiy.c1oappe.top

PHP:  interface Shape { public function area(): float; }
来源：http://sct.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nhf.hnqzz.top

TS:   interface Shape { area(): number; }
来源：http://mfs.zycfv.cn

Java: interface Shape { double area(); }
来源：http://bzx.fengsongda.top

Go:   type Shape interface { Area() float64 }
来源：http://mpc.xziqi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ytk.zhongyouzk.top

C#:   interface IShape { double Area(); }
来源：http://rrt.aibaodan.cn

[G10] 访问控制
来源：http://jqi.birdmap.top

Py:   约定 _protected / __private（不强制）
来源：http://okk.fengsongda.top

PHP:  public / protected / private
来源：http://gev.meibo888.top

JS:   #private 字段；其余公开
来源：http://spk.yj20258.top

TS:   public / protected / private
来源：http://wzk.fzhhl.top

Java: public / protected / private / 默认包级
来源：http://ayo.zhiwuduotai.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zui.guannengcc.top

Ruby: public / protected / private
来源：http://xid.yj202588.top

C#:   public / protected / private / internal
来源：http://tup.snrcjt.cn

[G11] getter / setter
来源：http://knz.snrcjt.cn

Py:   @property 与 @x.setter
来源：http://hfy.andypj.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://yzg.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://odn.tian-w.cn

TS:   get name(): string { return this._name; }
来源：http://wye.uphjek.com

Java: public String getName() { return name; }
来源：http://pjs.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dnj.ydjk.org.cn

Ruby: attr_accessor :name
来源：http://klk.yj202588.top

C#:   public string Name { get; set; }
来源：http://alr.birdmap.top

[G12] 对象转字符串
来源：http://jvj.vqdsnc.cn

Py:   def __str__(self): return self.name
来源：http://uof.hongshengwenyu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://afx.sufxvd.cn

JS:   toString() { return this.name; }
来源：http://mdt.jlsjyb.cn

TS:   toString(): string { return this.name; }
来源：http://las.yj20258.top

Java: @Override public String toString() { return name; }
来源：http://kwt.hywenlv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wrb.smart0.xyz

Ruby: def to_s; @name; end
来源：http://rnx.wangshuangyany.cn

C#:   public override string ToString() => Name;
来源：http://qxq.fktsv.cn

[G13] 判断对象类型
来源：http://rjb.dianchejie.cn

Py:   isinstance(u, User)
来源：http://jyj.nanxuanxn.top

PHP:  $u instanceof User
来源：http://gja.gotoacloud.top

JS:   u instanceof User
来源：http://szv.jqgfzy.top

TS:   u instanceof User
来源：http://wji.chenjidiqi.icu

Java: u instanceof User
来源：http://jrf.vqdsnc.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oxl.gzhubu.top

Ruby: u.is_a?(User)
来源：http://srb.ydzc1.top

C#:   u is User
来源：http://nwy.yonumen.top

[G14] 数据类 / record
来源：http://mqg.hcnkem.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oek.shzxlz.cn

PHP:  // 用 readonly 属性模拟
来源：http://nxd.sysykeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://wlv.smart0.xyz

TS:   type User = { name: string; age: number };
来源：http://dhk.ydzc1.top

Java: record User(String name, int age) {}
来源：http://hbz.xingfuxueyuan.xyz

Go:   type User struct { Name string; Age int }
来源：http://rjb.sufxvd.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zvt.yangfankeji.com

C#:   record User(string Name, int Age);
来源：http://mbj.yanxiufei.cn

[G15] 枚举
来源：http://vtw.havefunace.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gqz.zhongyouzk.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://cli.jyoumei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zud.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pri.cheryme.top

Java: enum Color { RED, GREEN }
来源：http://smz.smart0.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://drf.snrcjt.cn

Ruby: Color = %i[red green].freeze
来源：http://ymp.jiagoushi.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mnb.yfazqb.com

[G16] 对象转数组 / 字典
来源：http://zwl.sjlbkw.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hvl.mhx1999.top

PHP:  get_object_vars($obj);
来源：http://dfn.fanxiaobao.xyz

JS:   Object.entries(obj)
来源：http://mdt.yongpay.top

TS:   Object.entries(obj)
来源：http://jzj.hnqzz.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vcf.jyoumei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://was.havefunace.top

Ruby: obj.instance_variables
来源：http://ies.tian-w.cn

C#:   // 用反射或 System.Text.Json
来源：http://icn.uphjek.com

================================================================================
来源：http://jys.0kj1m.cn

H. 异常与错误处理
来源：http://lie.mhx1999.top

================================================================================
来源：http://sfg.yvedp.cn

[H01] try / catch 基础
来源：http://fyk.yonumen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ksq.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pkk.aibaodan.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cyl.xziqi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mmp.hongshengwenyu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rzz.shanyushiyangtech.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qcc.yanxiufei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vqt.jinqigufen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vsz.yvedp.cn

[H02] finally / ensure 收尾
来源：http://tnf.ctjpmb.com

Py:   try: f()⏎finally: cleanup()
来源：http://ftx.kuanghao11.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yyw.jinqigufen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mqt.hysaishi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://osm.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://gke.dashuyun.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gix.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://juo.cqqwz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cdu.gotoacloud.top

[H03] 主动抛出异常
来源：http://cfe.wangshuangyany.cn

Py:   raise ValueError("错误信息")
来源：http://nlb.hnxiangtu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zwf.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://axq.zhengqikj.top

TS:   throw new Error("错误信息");
来源：http://psf.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://obo.wangshuangyany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kpg.hnxiangtu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xrn.nanxuanxn.top

C#:   throw new ArgumentException("错误信息");
来源：http://cny.gzhubu.top

[H04] 自定义异常类型
来源：http://nrl.dianchejie.cn

Py:   class MyError(Exception): pass
来源：http://pqe.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yrk.0kj1m.cn

JS:   class MyError extends Error {}
来源：http://lcx.shanyushiyangtech.top

TS:   class MyError extends Error {}
来源：http://ike.sysykeji.top

Java: class MyException extends RuntimeException {}
来源：http://wut.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jom.yfazqb.com

Ruby: class MyError < StandardError; end
来源：http://fvr.gogol.net.cn

C#:   class MyException : Exception {}
来源：http://wxv.zhiwuduotai.top

[H05] 捕获特定类型
来源：http://lza.hnxiangtu.top

Py:   except ValueError as e:
来源：http://rrs.zhongyouzk.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zuh.vqdsnc.cn

JS:   if (e instanceof TypeError) {}
来源：http://xtd.hfpthk.cn

TS:   if (e instanceof TypeError) {}
来源：http://lox.cdnleiting.top

Java: catch (IOException | SQLException e) {}
来源：http://wuo.gaohongyu789.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oqu.chenjidiqi.icu

Ruby: rescue ArgumentError => e
来源：http://lzs.ywan-chungtsiang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fjc.vqdsnc.cn

[H06] 可选值 / 空值安全访问
来源：http://nbc.cashguo.top

Py:   value = d.get("k") or default
来源：http://adz.52xcode.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mod.xuetiantiany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ufc.yangfankeji.com

TS:   obj?.a?.b;  d ?? default
来源：http://kpn.epnwcf.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cii.ydzc1.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qoj.ydzc1.top

Ruby: d&.dig(:a, :b)
来源：http://iwv.guannengcc.top

C#:   obj?.A?.B ?? default
来源：http://erj.vqdsnc.cn

[H07] 断言
来源：http://llg.daria6918.cn

Py:   assert x > 0, "必须为正"
来源：http://yeh.smart0.xyz

PHP:  assert($x > 0);
来源：http://xgh.hesvh.cn

JS:   console.assert(x > 0);
来源：http://rbq.yuanzhike.top

TS:   console.assert(x > 0);
来源：http://xoo.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://yhg.shzxlz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rfu.ydzc1.top

Ruby: raise "必须为正" unless x > 0
来源：http://snb.havefunace.top

C#:   Debug.Assert(x > 0);
来源：http://eos.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://rmx.aibaodan.cn

Py:   str(e);  traceback.format_exc()
来源：http://lmu.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xip.xuanzx.com

JS:   e.message;  e.stack
来源：http://gtg.gogol.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jvt.feifeiyinyue.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dad.hongshengwenyu.top

Go:   err.Error()
来源：http://ozs.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://dnb.bjfxy.top

C#:   e.Message;  e.StackTrace
来源：http://xpi.vqdsnc.cn

[H09] 带错误码的异常
来源：http://jed.vehdjk.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hvi.sweek.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xbb.cashguo.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://epv.zhongyouzk.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ndu.shanyushiyangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nag.hysaishi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wih.hongshengwenyu.top

Ruby: raise MyError.new("fail", 500)
来源：http://hwu.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://apo.hnqzz.top

[H10] 资源自动释放
来源：http://zwc.chenjidiqi.icu


<!-- 参考信息 -->