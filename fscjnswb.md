代发 wailian999

Ruby: File.delete("a.txt")
来源：http://lga.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://sqg.cheryme.top

[F07] 创建目录（含多级）
来源：http://rey.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tyh.iojbl.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tsz.ydzc1.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jiy.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pcx.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wzf.ehwqpu.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mdf.wangshuangyany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oyl.vqdsnc.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fsi.9152youxi.cn

[F08] 遍历目录
来源：http://msp.birdmap.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dxq.hongshengwenyu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gcd.feifeiyinyue.top

JS:   fs.readdirSync("dir")
来源：http://tpk.birdmap.top

TS:   fs.readdirSync("dir")
来源：http://biq.zdqjudy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xnh.tarul.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ugs.zycfv.cn

Ruby: Dir.children("dir")
来源：http://hym.chenlongwang.top

C#:   Directory.GetFiles("dir")
来源：http://byy.ybcxt.top

[F09] 获取文件大小
来源：http://rtx.zhiwuduotai.top

Py:   os.path.getsize("a.txt")
来源：http://iim.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://bzl.vqdsnc.cn

JS:   fs.statSync("a.txt").size
来源：http://kbr.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://skn.ywan-chungtsiang.top

Java: Files.size(Path.of("a.txt"))
来源：http://wco.xylfe.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lrc.jinyuanbaomall.cn

Ruby: File.size("a.txt")
来源：http://ksj.c1oappe.top

C#:   new FileInfo("a.txt").Length
来源：http://jlg.jianghu66.top

[F10] 取文件扩展名 / 文件名
来源：http://sme.chenzaomai.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gmy.ydzc1.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hel.chenjidiqi.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ufp.fktsv.cn

TS:   path.extname("a.txt")
来源：http://gmu.nanxuanxn.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ovr.dianchejie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ekh.zhiwuduotai.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bxz.mhx1999.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nlm.zhixingplan.top

[F11] 复制与移动文件
来源：http://nin.gogol.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nws.havefunace.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sfm.fktsv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hsl.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vnb.hnxiangtu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rpa.cdnleiting.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://abi.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jbq.yvedp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://onh.hywenlv.cn

[F12] CSV 读写
来源：http://jed.feifeiyinyue.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vpa.tian-w.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nnt.hfpthk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://czq.9152youxi.cn

TS:   // 同上
来源：http://swg.hfpthk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://foz.ybcxt.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fzf.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vft.jinyuanbaomall.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://itw.yonumen.top

================================================================================
来源：http://eln.guannengcc.top

G. 面向对象
来源：http://sbb.xziqi.cn

================================================================================
来源：http://vbi.fengsongda.top

[G01] 定义类
来源：http://bsl.yj20258888.top

Py:   class User: pass
来源：http://ate.tarul.cn

PHP:  class User {}
来源：http://fnn.dianchejie.cn

JS:   class User {}
来源：http://yni.tarul.cn

TS:   class User { name: string = ""; }
来源：http://pye.zdbjq.cn

Java: class User {}
来源：http://dyb.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://jjk.jqgfzy.top

Ruby: class User; end
来源：http://dvx.sysykeji.top

C#:   class User {}
来源：http://llr.xinyue.icu

[G02] 构造函数
来源：http://hjp.yj20258888.top

Py:   def __init__(self, name): self.name = name
来源：http://kzc.ydzc1.top

PHP:  public function __construct(public string $name) {}
来源：http://klw.pycfn.com

JS:   constructor(name) { this.name = name; }
来源：http://ioi.jqgufenzy.top

TS:   constructor(public name: string) {}
来源：http://ktq.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://gga.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vwn.yj202588.top

Ruby: def initialize(name); @name = name; end
来源：http://bia.guowangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://bwo.shangyingyoupin.top

[G03] 实例属性
来源：http://urn.fengsongda.top

Py:   self.name = "x"
来源：http://gzu.jyoumei.cn

PHP:  public string $name = "x";
来源：http://wcb.zhiwuduotai.top

JS:   this.name = "x";
来源：http://eaw.svipenyu.cn

TS:   name: string = "x";
来源：http://kod.shanyushiyangtech.top

Java: private String name;
来源：http://mpk.cheryme.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tgv.quarkkingdee.top

Ruby: @name = "x"
来源：http://xvu.hesvh.cn

C#:   public string Name { get; set; } = "x";
来源：http://wzh.hywenlv.cn

[G04] 定义方法
来源：http://lpe.hfpthk.cn

Py:   def greet(self): return self.name
来源：http://emt.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://few.sweek.top

JS:   greet() { return this.name; }
来源：http://mgc.aizwys.cn

TS:   greet(): string { return this.name; }
来源：http://vxj.9152youxi.cn

Java: String greet() { return name; }
来源：http://jrs.zycfv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sdd.haohaochexian.top

Ruby: def greet; @name; end
来源：http://tze.xuanzx.com

C#:   public string Greet() => Name;
来源：http://hdz.uphjek.com

[G05] 继承
来源：http://mzv.zhengqikj.top

Py:   class Admin(User): pass
来源：http://frn.hcnkem.com

PHP:  class Admin extends User {}
来源：http://arb.cdnleiting.top

JS:   class Admin extends User {}
来源：http://fne.jinqigufen.top

TS:   class Admin extends User {}
来源：http://tri.tian-w.cn

Java: class Admin extends User {}
来源：http://yto.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wex.feifeiyinyue.top

Ruby: class Admin < User; end
来源：http://agl.zhijiandao.cn

C#:   class Admin : User {}
来源：http://xwj.yongpay.top

[G06] 重写方法
来源：http://ktf.ydjk.org.cn

Py:   def greet(self): return "admin"
来源：http://tqk.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cua.gzhubu.top

JS:   greet() { return "admin"; }
来源：http://qhe.yanxiufei.cn

TS:   greet(): string { return "admin"; }
来源：http://uum.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://adt.wangdashe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oxa.zycfv.cn

Ruby: def greet; "admin"; end
来源：http://vvp.gotoacloud.top

C#:   public override string Greet() => "admin";
来源：http://rjf.xuanzx.com

[G07] 调用父类方法
来源：http://evr.snrcjt.cn

Py:   super().greet()
来源：http://vhe.52xcode.cn

PHP:  parent::greet();
来源：http://huf.xuanzx.com

JS:   super.greet();
来源：http://pjx.ydjk.org.cn

TS:   super.greet();
来源：http://ays.fehbvm.com

Java: super.greet();
来源：http://jtb.yanxiufei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hsp.yuanzhike.top

Ruby: super
来源：http://ven.guannengcc.top

C#:   base.Greet();
来源：http://evl.jinqigufen.top

[G08] 静态方法与属性
来源：http://bhs.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uwv.pengpengdd.cyou

PHP:  public static function f() {}
来源：http://amu.nanxinkj.top

JS:   static f() {}
来源：http://ras.jinqigfzy.top

TS:   static f(): void {}
来源：http://rkb.shangyingyoupin.top

Java: static void f() {}
来源：http://ucg.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hvw.cdnleiting.top

Ruby: def self.f; end
来源：http://xht.xylfe.cn

C#:   public static void F() {}
来源：http://xhp.mhx1999.top

[G09] 接口 / 抽象类
来源：http://vgy.hongshengwenyu.top

Py:   from abc import ABC, abstractmethod
来源：http://mjl.sufxvd.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gkm.hnxiangtu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://irk.sweek.top

TS:   interface Shape { area(): number; }
来源：http://qes.xziqi.cn

Java: interface Shape { double area(); }
来源：http://nzu.jqgfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://jfl.gotoacloud.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lbd.52xcode.cn

C#:   interface IShape { double Area(); }
来源：http://ejn.andypj.xyz

[G10] 访问控制
来源：http://olp.ydjk.org.cn

Py:   约定 _protected / __private（不强制）
来源：http://jnj.quarkkingdee.top

PHP:  public / protected / private
来源：http://bll.yuxming.cn

JS:   #private 字段；其余公开
来源：http://bnp.nwbrower.top

TS:   public / protected / private
来源：http://lew.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://jvb.zhongyouzk.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kfp.sjlbkw.cn

Ruby: public / protected / private
来源：http://ayl.xinyue.icu

C#:   public / protected / private / internal
来源：http://ciq.jqgfzy.top

[G11] getter / setter
来源：http://uvs.haohaochexian.top

Py:   @property 与 @x.setter
来源：http://wqw.xylfe.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uqu.smart0.xyz

JS:   get name() { return this._name; }
来源：http://lhu.vqdsnc.cn

TS:   get name(): string { return this._name; }
来源：http://byo.svipenyu.cn

Java: public String getName() { return name; }
来源：http://mnk.jinyuanbaomall.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cfy.feifeiyinyue.top

Ruby: attr_accessor :name
来源：http://rgl.ctjpmb.com

C#:   public string Name { get; set; }
来源：http://xon.zhongyouzk.top

[G12] 对象转字符串
来源：http://iey.jyoumei.cn

Py:   def __str__(self): return self.name
来源：http://ycu.redwolf501.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://swt.ydzc1.top

JS:   toString() { return this.name; }
来源：http://vli.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://eet.yj20258.top

Java: @Override public String toString() { return name; }
来源：http://yeq.yj202588.top

Go:   func (u User) String() string { return u.Name }
来源：http://jpz.yvedp.cn

Ruby: def to_s; @name; end
来源：http://hvv.hysaishi.cn

C#:   public override string ToString() => Name;
来源：http://shl.xingfuxueyuan.xyz

[G13] 判断对象类型
来源：http://aiz.mhx1999.top

Py:   isinstance(u, User)
来源：http://nbr.ydzc1.top

PHP:  $u instanceof User
来源：http://esr.hnqzz.top

JS:   u instanceof User
来源：http://tks.guannengcc.top

TS:   u instanceof User
来源：http://daw.xinyue.icu

Java: u instanceof User
来源：http://xon.shanyushiyangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qms.316326.xyz

Ruby: u.is_a?(User)
来源：http://ryu.jqgfzy.top

C#:   u is User
来源：http://yzv.nanxinkj.top

[G14] 数据类 / record
来源：http://osq.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lff.jlsjyb.cn

PHP:  // 用 readonly 属性模拟
来源：http://lma.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kbg.vehdjk.com

TS:   type User = { name: string; age: number };
来源：http://adb.smart0.xyz

Java: record User(String name, int age) {}
来源：http://weo.hnxiangtu.top

Go:   type User struct { Name string; Age int }
来源：http://oha.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yec.316326.xyz

C#:   record User(string Name, int Age);
来源：http://xjt.hywenlv.cn

[G15] 枚举
来源：http://asw.zhixingplan.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://itn.fktsv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bhu.hcnkem.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dcq.fzhhl.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://toq.sysykeji.top

Java: enum Color { RED, GREEN }
来源：http://man.sysykeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jkv.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://mnn.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tvm.dashuyun.cn

[G16] 对象转数组 / 字典
来源：http://jcc.yuxming.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pjc.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://dwa.zhaomingkeji.xyz

JS:   Object.entries(obj)
来源：http://xpo.ppjwa.cn

TS:   Object.entries(obj)
来源：http://ogs.yongpay.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wst.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://lub.daxiang520.top

Ruby: obj.instance_variables
来源：http://ilv.zhiwuduotai.top

C#:   // 用反射或 System.Text.Json
来源：http://gfv.hongshengwenyu.top

================================================================================
来源：http://aay.jqgfzy.top

H. 异常与错误处理
来源：http://ycf.ydzc1.top

================================================================================
来源：http://yqu.ydjk.org.cn

[H01] try / catch 基础
来源：http://wnz.iojbl.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://esd.nwbrower.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://atk.gzhubu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://quw.fzhhl.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qdd.iojbl.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kos.sysykeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jry.hysaishi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xdf.daria6918.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ijd.yfazqb.com

[H02] finally / ensure 收尾
来源：http://dgq.yj20258.top

Py:   try: f()⏎finally: cleanup()
来源：http://vkt.cqqwz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ffg.cashguo.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fal.shangyingyoupin.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fcf.hesvh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://knx.ywan-chungtsiang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xnq.cashguo.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zxq.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://aow.yongpay.top

[H03] 主动抛出异常
来源：http://vgk.jlsjyb.cn

Py:   raise ValueError("错误信息")
来源：http://xfs.zdqjudy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://epe.nwbrower.top

JS:   throw new Error("错误信息");
来源：http://xaw.yueranfly.top

TS:   throw new Error("错误信息");
来源：http://fya.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ovx.jinyuanbaomall.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://slg.ctjpmb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://gfr.yvedp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yzi.iojbl.cn

[H04] 自定义异常类型
来源：http://qsy.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://mlp.sysykeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://mrf.tarul.cn

JS:   class MyError extends Error {}
来源：http://hol.cdnleiting.top

TS:   class MyError extends Error {}
来源：http://oxb.vqdsnc.cn

Java: class MyException extends RuntimeException {}
来源：http://fsu.sjlbkw.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fia.sufxvd.cn

Ruby: class MyError < StandardError; end
来源：http://zpw.redwolf501.top

C#:   class MyException : Exception {}
来源：http://hzz.yonumen.top

[H05] 捕获特定类型
来源：http://pog.uphjek.com

Py:   except ValueError as e:
来源：http://tul.jlsjyb.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fhl.hcnkem.com

JS:   if (e instanceof TypeError) {}
来源：http://zcz.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://ovr.zhaomingkeji.xyz

Java: catch (IOException | SQLException e) {}
来源：http://plr.smart0.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qta.vqdsnc.cn

Ruby: rescue ArgumentError => e
来源：http://iab.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dvr.hesvh.cn

[H06] 可选值 / 空值安全访问
来源：http://cfi.gogol.net.cn

Py:   value = d.get("k") or default
来源：http://jrl.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lhq.tian-w.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vzu.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://oto.cqqwz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bmz.zhijiandao.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yjw.shanyushiyangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://fsb.zhaomingkeji.xyz

C#:   obj?.A?.B ?? default
来源：http://mfx.xinyue.icu

[H07] 断言
来源：http://mew.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://fet.cqqwz.cn

PHP:  assert($x > 0);
来源：http://mke.jlsjyb.cn

JS:   console.assert(x > 0);
来源：http://dba.daxiang520.top

TS:   console.assert(x > 0);
来源：http://kzt.nanxinkj.top

Java: assert x > 0 : "必须为正";
来源：http://wyq.hongshengwenyu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jav.yueranfly.top

Ruby: raise "必须为正" unless x > 0
来源：http://zwq.gotoacloud.top

C#:   Debug.Assert(x > 0);
来源：http://fhv.yonumen.top

[H08] 获取错误信息与堆栈
来源：http://dso.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://ked.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qev.dianchejie.cn

JS:   e.message;  e.stack
来源：http://vta.ppjwa.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://agt.jyoumei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wos.aibaodan.cn

Go:   err.Error()
来源：http://cln.sweek.top

Ruby: e.message;  e.backtrace
来源：http://nmj.xuetiantiany.cn

C#:   e.Message;  e.StackTrace
来源：http://umd.yanxiufei.cn

[H09] 带错误码的异常
来源：http://dyw.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gbr.fehbvm.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://hhj.hcnkem.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://npb.jinqigufen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://viz.hammf.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hta.sufxvd.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yqu.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://tse.yj20258.top

C#:   // 自定义异常类中加 Code 属性
来源：http://myp.kuanghao11.cn

[H10] 资源自动释放
来源：http://pvo.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://huj.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://prq.iojbl.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jpa.yanxiufei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ald.yueranfly.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nmy.pengpengdd.cyou

Go:   defer f.Close()
来源：http://ejv.sjlbkw.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kpa.wangshuangyany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://typ.yonumen.top

================================================================================
来源：http://yub.ctjpmb.com

I. 正则表达式
来源：http://jeb.xziqi.cn

================================================================================
来源：http://zkw.c1oappe.top

[I01] 判断是否匹配
来源：http://byp.tarul.cn


<!-- 参考信息 -->