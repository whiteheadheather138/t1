代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://uhv.fengsongda.top

TS:   fs.unlinkSync("a.txt")
来源：http://lcw.jinqigfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jkq.tarul.cn

Go:   os.Remove("a.txt")
来源：http://tqc.zhengqikj.top

Ruby: File.delete("a.txt")
来源：http://hzy.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://pyp.jinqigfzy.top

[F07] 创建目录（含多级）
来源：http://whg.svipenyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fxe.hfpthk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nep.zhiwuduotai.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zos.jinghuilouyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ziy.cheryme.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://keo.zdbjq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ixh.bjfxy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yea.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pps.jinghuilouyu.cn

[F08] 遍历目录
来源：http://mnu.ivvv.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://clt.hnqzz.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ofc.hongshengwenyu.top

JS:   fs.readdirSync("dir")
来源：http://qdw.zhaomingkeji.xyz

TS:   fs.readdirSync("dir")
来源：http://xax.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aha.jinqigufen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vec.fanxiaobao.xyz

Ruby: Dir.children("dir")
来源：http://ilg.birdmap.top

C#:   Directory.GetFiles("dir")
来源：http://dob.yanxiufei.cn

[F09] 获取文件大小
来源：http://cwj.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://xjh.fanxiaobao.xyz

PHP:  filesize("a.txt");
来源：http://bwh.vehdjk.com

JS:   fs.statSync("a.txt").size
来源：http://ssn.jqgfzy.top

TS:   fs.statSync("a.txt").size
来源：http://sby.svipenyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fdz.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hax.zdbjq.cn

Ruby: File.size("a.txt")
来源：http://ild.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://gnk.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://hzt.chenlongwang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nob.zhoulong.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zlx.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ocz.cdnleiting.top

TS:   path.extname("a.txt")
来源：http://nqk.hysaishi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pyo.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ebg.xylfe.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qzo.andypj.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jxx.chenlongwang.top

[F11] 复制与移动文件
来源：http://nuu.shuidangran.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vsu.zdbjq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cmd.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vcf.vehdjk.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eto.zycfv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dfy.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://efg.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://amb.ywan-chungtsiang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://diy.redwolf501.top

[F12] CSV 读写
来源：http://nsb.fktsv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hqq.nwbrower.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dnr.dianchejie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kum.ydzc1.top

TS:   // 同上
来源：http://zgs.yueranfly.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hsl.zycfv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://peq.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tkb.hywenlv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bwn.dianchejie.cn

================================================================================
来源：http://iee.fanxiaobao.xyz

G. 面向对象
来源：http://ets.yangfankeji.com

================================================================================
来源：http://voe.dianchejie.cn

[G01] 定义类
来源：http://sdh.daxiang520.top

Py:   class User: pass
来源：http://shs.smart0.xyz

PHP:  class User {}
来源：http://hvo.jinqigfzy.top

JS:   class User {}
来源：http://kjv.zhiwuduotai.top

TS:   class User { name: string = ""; }
来源：http://kiy.gotoacloud.top

Java: class User {}
来源：http://fak.zhongyouzk.top

Go:   type User struct { Name string }
来源：http://ztj.snrcjt.cn

Ruby: class User; end
来源：http://gli.zhongyouzk.top

C#:   class User {}
来源：http://uyq.sufxvd.cn

[G02] 构造函数
来源：http://gqn.quarkkingdee.top

Py:   def __init__(self, name): self.name = name
来源：http://hbt.redwolf501.top

PHP:  public function __construct(public string $name) {}
来源：http://pay.jlsjyb.cn

JS:   constructor(name) { this.name = name; }
来源：http://kes.yangfankeji.com

TS:   constructor(public name: string) {}
来源：http://chr.shuidangran.top

Java: User(String name) { this.name = name; }
来源：http://uxt.xuanzx.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xao.c1oappe.top

Ruby: def initialize(name); @name = name; end
来源：http://usv.0kj1m.cn

C#:   public User(string name) { Name = name; }
来源：http://qip.ehwqpu.com

[G03] 实例属性
来源：http://ogy.uphjek.com

Py:   self.name = "x"
来源：http://poi.vehdjk.com

PHP:  public string $name = "x";
来源：http://ahs.andypj.xyz

JS:   this.name = "x";
来源：http://dea.hammf.cn

TS:   name: string = "x";
来源：http://ccw.hesvh.cn

Java: private String name;
来源：http://vqx.zhijiandao.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://txk.xinyue.icu

Ruby: @name = "x"
来源：http://xep.ydjk.org.cn

C#:   public string Name { get; set; } = "x";
来源：http://qqf.aibaodan.cn

[G04] 定义方法
来源：http://ygb.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://iwm.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ifj.cucudq.cn

JS:   greet() { return this.name; }
来源：http://epd.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://ugr.chenzaomai.com

Java: String greet() { return name; }
来源：http://hlb.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mxz.tarul.cn

Ruby: def greet; @name; end
来源：http://yqv.hongshengwenyu.top

C#:   public string Greet() => Name;
来源：http://mzk.daria6918.cn

[G05] 继承
来源：http://exs.fktsv.cn

Py:   class Admin(User): pass
来源：http://adc.chenlongwang.top

PHP:  class Admin extends User {}
来源：http://fed.wangdashe.top

JS:   class Admin extends User {}
来源：http://yqa.dianchejie.cn

TS:   class Admin extends User {}
来源：http://ucx.zhixingplan.top

Java: class Admin extends User {}
来源：http://bxf.tian-w.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dnk.sweek.top

Ruby: class Admin < User; end
来源：http://yhy.nwbrower.top

C#:   class Admin : User {}
来源：http://tal.vehdjk.com

[G06] 重写方法
来源：http://tyb.ctjpmb.com

Py:   def greet(self): return "admin"
来源：http://zkh.zdbjq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vqg.ctjpmb.com

JS:   greet() { return "admin"; }
来源：http://gyy.9152youxi.cn

TS:   greet(): string { return "admin"; }
来源：http://ipg.ydjk.org.cn

Java: @Override String greet() { return "admin"; }
来源：http://qsy.fzhhl.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://byd.yangfankeji.com

Ruby: def greet; "admin"; end
来源：http://sct.ppjwa.cn

C#:   public override string Greet() => "admin";
来源：http://joc.tianlin.xyz

[G07] 调用父类方法
来源：http://ymu.iojbl.cn

Py:   super().greet()
来源：http://kxz.jinyuanbaomall.cn

PHP:  parent::greet();
来源：http://das.mhx1999.top

JS:   super.greet();
来源：http://uab.ppjwa.cn

TS:   super.greet();
来源：http://tya.sjlbkw.cn

Java: super.greet();
来源：http://kwl.nanxinkj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://svi.daxiang520.top

Ruby: super
来源：http://aok.hcnkem.com

C#:   base.Greet();
来源：http://wgx.yangfankeji.com

[G08] 静态方法与属性
来源：http://bob.fzhhl.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lyd.sysykeji.top

PHP:  public static function f() {}
来源：http://arl.gotoacloud.top

JS:   static f() {}
来源：http://med.sxryk.cn

TS:   static f(): void {}
来源：http://jeb.fktsv.cn

Java: static void f() {}
来源：http://zxm.haohaochexian.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hss.9152youxi.cn

Ruby: def self.f; end
来源：http://gxq.zhiwuduotai.top

C#:   public static void F() {}
来源：http://ilg.xinyue.icu

[G09] 接口 / 抽象类
来源：http://gyc.bjfxy.top

Py:   from abc import ABC, abstractmethod
来源：http://glu.uphjek.com

PHP:  interface Shape { public function area(): float; }
来源：http://waw.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zhs.vqdsnc.cn

TS:   interface Shape { area(): number; }
来源：http://tfz.zhijiandao.cn

Java: interface Shape { double area(); }
来源：http://rrq.ivvv.top

Go:   type Shape interface { Area() float64 }
来源：http://gxg.quarkkingdee.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hki.xuanzx.com

C#:   interface IShape { double Area(); }
来源：http://ybb.shanyushiyangkeji.top

[G10] 访问控制
来源：http://jpi.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://wdd.ctjpmb.com

PHP:  public / protected / private
来源：http://kwd.zycfv.cn

JS:   #private 字段；其余公开
来源：http://rtk.yueranfly.top

TS:   public / protected / private
来源：http://ext.bjfxy.top

Java: public / protected / private / 默认包级
来源：http://vjp.feifeiyinyue.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hqa.kuanghao11.cn

Ruby: public / protected / private
来源：http://aca.ppjwa.cn

C#:   public / protected / private / internal
来源：http://iig.yj20258888.top

[G11] getter / setter
来源：http://bql.epnwcf.com

Py:   @property 与 @x.setter
来源：http://uhs.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wjm.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://kvo.haohaochexian.top

TS:   get name(): string { return this._name; }
来源：http://zlz.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://wok.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://asf.yj20258888.top

Ruby: attr_accessor :name
来源：http://seg.cqqwz.cn

C#:   public string Name { get; set; }
来源：http://vrd.tanke756.top

[G12] 对象转字符串
来源：http://hmz.shanyushiyangtech.top

Py:   def __str__(self): return self.name
来源：http://vkb.yj202588.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pha.yongpay.top

JS:   toString() { return this.name; }
来源：http://dag.mhx1999.top

TS:   toString(): string { return this.name; }
来源：http://kxp.gzhubu.top

Java: @Override public String toString() { return name; }
来源：http://elt.yj20258888.top

Go:   func (u User) String() string { return u.Name }
来源：http://jha.xinyue.icu

Ruby: def to_s; @name; end
来源：http://xts.ehwqpu.com

C#:   public override string ToString() => Name;
来源：http://aic.zycfv.cn

[G13] 判断对象类型
来源：http://imz.9152youxi.cn

Py:   isinstance(u, User)
来源：http://gor.yuxming.cn

PHP:  $u instanceof User
来源：http://dbk.dashuyun.cn

JS:   u instanceof User
来源：http://ijr.aibaodan.cn

TS:   u instanceof User
来源：http://ugh.sysykeji.top

Java: u instanceof User
来源：http://baz.cheryme.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jgr.gotoacloud.top

Ruby: u.is_a?(User)
来源：http://ard.fengsongda.top

C#:   u is User
来源：http://jvy.tarul.cn

[G14] 数据类 / record
来源：http://hbf.ppjwa.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qku.yongpay.top

PHP:  // 用 readonly 属性模拟
来源：http://gth.cheryme.top

JS:   // 无内置：普通类或对象字面量
来源：http://zgm.xziqi.cn

TS:   type User = { name: string; age: number };
来源：http://znz.tian-w.cn

Java: record User(String name, int age) {}
来源：http://rnt.mhx1999.top

Go:   type User struct { Name string; Age int }
来源：http://erq.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lds.xingfuxueyuan.xyz

C#:   record User(string Name, int Age);
来源：http://jon.dianchejie.cn

[G15] 枚举
来源：http://lwp.yueranfly.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zjh.guannengcc.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vnm.jiagoushi.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://koi.jinqigufen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gmw.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://tta.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vkr.bjfxy.top

Ruby: Color = %i[red green].freeze
来源：http://ucs.pengpengdd.cyou

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oxx.ybcxt.top

[G16] 对象转数组 / 字典
来源：http://xcw.yj20258888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dkd.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://xxp.zhixingplan.top

JS:   Object.entries(obj)
来源：http://smi.vqdsnc.cn

TS:   Object.entries(obj)
来源：http://saf.epnwcf.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ton.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qti.yongpay.top

Ruby: obj.instance_variables
来源：http://qko.zhongyouzk.top

C#:   // 用反射或 System.Text.Json
来源：http://ink.aibaodan.cn

================================================================================
来源：http://caf.xingfuxueyuan.xyz

H. 异常与错误处理
来源：http://nrv.bbcook.cn

================================================================================
来源：http://lkj.aizwys.cn

[H01] try / catch 基础
来源：http://veu.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://glj.fzhhl.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://suy.0kj1m.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fyy.guannengcc.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nor.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qnb.yuxming.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fll.c1oappe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mgz.fanxiaobao.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jbo.dianchejie.cn

[H02] finally / ensure 收尾
来源：http://pkv.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://hrc.fehbvm.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://dho.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://tnl.kuanghao11.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gha.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fnp.jqgfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wso.pengpengdd.cyou

Ruby: begin; f; ensure; cleanup; end
来源：http://yzz.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xyk.shuidangran.top

[H03] 主动抛出异常
来源：http://jqx.hywenlv.cn

Py:   raise ValueError("错误信息")
来源：http://tzy.ivvv.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yrd.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://ilt.aizwys.cn

TS:   throw new Error("错误信息");
来源：http://hgo.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nty.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://afm.hywenlv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rzm.daria6918.cn

C#:   throw new ArgumentException("错误信息");
来源：http://iia.shzxlz.cn

[H04] 自定义异常类型
来源：http://hlz.fehbvm.com

Py:   class MyError(Exception): pass
来源：http://eiv.yj202588.top

PHP:  class MyError extends RuntimeException {}
来源：http://trt.hongshengwenyu.top

JS:   class MyError extends Error {}
来源：http://fen.gzhubu.top

TS:   class MyError extends Error {}
来源：http://sne.svipenyu.cn

Java: class MyException extends RuntimeException {}
来源：http://fuf.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bzf.jyoumei.cn

Ruby: class MyError < StandardError; end
来源：http://yqs.ydzc1.top

C#:   class MyException : Exception {}
来源：http://uug.yongpay.top

[H05] 捕获特定类型
来源：http://mjq.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://pel.daxiang520.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ohe.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://qkp.daxiang520.top

TS:   if (e instanceof TypeError) {}
来源：http://sze.yj202588.top

Java: catch (IOException | SQLException e) {}
来源：http://onj.uphjek.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://azq.xuetiantiany.cn

Ruby: rescue ArgumentError => e
来源：http://clo.bjfxy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iwz.smart0.xyz

[H06] 可选值 / 空值安全访问
来源：http://psu.aizwys.cn

Py:   value = d.get("k") or default
来源：http://xes.hnqzz.top

PHP:  $v = $d["k"] ?? null;
来源：http://mku.fktsv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ocm.hysaishi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ngk.cdnleiting.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://izb.iojbl.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lrv.birdmap.top

Ruby: d&.dig(:a, :b)
来源：http://kud.chenlongwang.top

C#:   obj?.A?.B ?? default
来源：http://dtw.wangshuangyany.cn

[H07] 断言
来源：http://qah.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://yle.wangdashe.top

PHP:  assert($x > 0);
来源：http://fyx.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://uvv.jqgfzy.top

TS:   console.assert(x > 0);
来源：http://mto.chenjidiqi.icu

Java: assert x > 0 : "必须为正";
来源：http://mdt.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://knz.hammf.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yhx.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://hhw.pengpengdd.cyou

[H08] 获取错误信息与堆栈
来源：http://kkp.shanyushiyangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://hlr.kuanghao11.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tzj.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://xpf.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zrw.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://xhs.zhongyouzk.top

Go:   err.Error()
来源：http://hxk.ehwqpu.com

Ruby: e.message;  e.backtrace
来源：http://xhp.havefunace.top

C#:   e.Message;  e.StackTrace
来源：http://mwx.sufxvd.cn

[H09] 带错误码的异常
来源：http://omi.andypj.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rps.uphjek.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://ley.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zjz.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ksp.shanyushiyangtech.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kgq.gogol.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qkk.hongshengwenyu.top

Ruby: raise MyError.new("fail", 500)
来源：http://dbw.quarkkingdee.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yky.aizwys.cn

[H10] 资源自动释放
来源：http://fhd.jiagoushi.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gmq.dashuyun.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ynu.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uma.yongpay.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cad.wangshuangyany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fgg.snrcjt.cn

Go:   defer f.Close()
来源：http://trp.hesvh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vcn.aizwys.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://afy.zhengqikj.top


<!-- 参考信息 -->