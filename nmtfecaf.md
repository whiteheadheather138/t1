代发 wailian999

Ruby: File.delete("a.txt")
来源：http://xmw.yueranfly.top

C#:   File.Delete("a.txt");
来源：http://xpr.zdqjudy.top

[F07] 创建目录（含多级）
来源：http://ekt.sjlbkw.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oje.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yud.daria6918.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mje.jiagoushi.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fzy.jqgufenzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rwd.316326.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cvu.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iyv.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nwl.zycfv.cn

[F08] 遍历目录
来源：http://fzm.gotoacloud.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://swq.sysykeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eec.iojbl.cn

JS:   fs.readdirSync("dir")
来源：http://rdo.zhiwuduotai.top

TS:   fs.readdirSync("dir")
来源：http://njw.fengsongda.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hpd.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jxf.yueranfly.top

Ruby: Dir.children("dir")
来源：http://chn.wangdashe.top

C#:   Directory.GetFiles("dir")
来源：http://cfy.epnwcf.com

[F09] 获取文件大小
来源：http://bte.yueranfly.top

Py:   os.path.getsize("a.txt")
来源：http://usm.fengsongda.top

PHP:  filesize("a.txt");
来源：http://idz.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://ebt.dashuyun.cn

TS:   fs.statSync("a.txt").size
来源：http://qhx.jianghu66.top

Java: Files.size(Path.of("a.txt"))
来源：http://fpx.kuanghao11.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gnv.hcnkem.com

Ruby: File.size("a.txt")
来源：http://opk.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://xsf.snrcjt.cn

[F10] 取文件扩展名 / 文件名
来源：http://njt.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hwn.iojbl.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jpo.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jba.bbcook.cn

TS:   path.extname("a.txt")
来源：http://jgd.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gio.nanxinkj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fxs.epnwcf.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xcu.dashuyun.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rww.shangyingyoupin.top

[F11] 复制与移动文件
来源：http://cxw.epnwcf.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://igg.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nvo.pycfn.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mta.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ybv.xziqi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://psu.ivvv.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lhg.tian-w.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ont.ppjwa.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://irk.jinghuilouyu.cn

[F12] CSV 读写
来源：http://kdn.shanyushiyangtech.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wmh.ydzc1.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xjs.daxiang520.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ivn.snrcjt.cn

TS:   // 同上
来源：http://jps.shzxlz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://twf.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cxg.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lgv.cqqwz.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dql.yonumen.top

================================================================================
来源：http://hbt.ppjwa.cn

G. 面向对象
来源：http://bsp.yj202588.top

================================================================================
来源：http://rtn.jinghuilouyu.cn

[G01] 定义类
来源：http://apz.fengsongda.top

Py:   class User: pass
来源：http://usf.sjlbkw.cn

PHP:  class User {}
来源：http://cdd.aibaodan.cn

JS:   class User {}
来源：http://vqm.chenjidiqi.icu

TS:   class User { name: string = ""; }
来源：http://avg.fzhhl.top

Java: class User {}
来源：http://zqq.nanxinkj.top

Go:   type User struct { Name string }
来源：http://kab.feifeiyinyue.top

Ruby: class User; end
来源：http://fqw.hywenlv.cn

C#:   class User {}
来源：http://bxm.jinghuilouyu.cn

[G02] 构造函数
来源：http://fub.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://jhb.hesvh.cn

PHP:  public function __construct(public string $name) {}
来源：http://hit.fzhhl.top

JS:   constructor(name) { this.name = name; }
来源：http://upm.fengsongda.top

TS:   constructor(public name: string) {}
来源：http://gey.fehbvm.com

Java: User(String name) { this.name = name; }
来源：http://kvt.zdqjudy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://avm.zhoulong.xyz

Ruby: def initialize(name); @name = name; end
来源：http://cse.jlsjyb.cn

C#:   public User(string name) { Name = name; }
来源：http://bnt.ppjwa.cn

[G03] 实例属性
来源：http://yqb.yj202588.top

Py:   self.name = "x"
来源：http://ate.kuanghao11.cn

PHP:  public string $name = "x";
来源：http://xzi.sweek.top

JS:   this.name = "x";
来源：http://oml.meibo888.top

TS:   name: string = "x";
来源：http://xux.zhengqikj.top

Java: private String name;
来源：http://jnc.aizwys.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nsm.ctjpmb.com

Ruby: @name = "x"
来源：http://hdu.yanxiufei.cn

C#:   public string Name { get; set; } = "x";
来源：http://pfr.chenzaomai.com

[G04] 定义方法
来源：http://oyt.yvedp.cn

Py:   def greet(self): return self.name
来源：http://hks.xinyue.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://djn.zhongyouzk.top

JS:   greet() { return this.name; }
来源：http://ypy.bbcook.cn

TS:   greet(): string { return this.name; }
来源：http://fqt.jqgufenzy.top

Java: String greet() { return name; }
来源：http://zcd.hywenlv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vid.zhijiandao.cn

Ruby: def greet; @name; end
来源：http://rkx.yvedp.cn

C#:   public string Greet() => Name;
来源：http://bkq.sxryk.cn

[G05] 继承
来源：http://mww.xingfuxueyuan.xyz

Py:   class Admin(User): pass
来源：http://yzv.ivvv.top

PHP:  class Admin extends User {}
来源：http://pqy.fktsv.cn

JS:   class Admin extends User {}
来源：http://tbz.9152youxi.cn

TS:   class Admin extends User {}
来源：http://mpe.cqqwz.cn

Java: class Admin extends User {}
来源：http://hcu.guowangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mfk.dashuyun.cn

Ruby: class Admin < User; end
来源：http://vrv.zycfv.cn

C#:   class Admin : User {}
来源：http://ado.hywenlv.cn

[G06] 重写方法
来源：http://nag.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://qua.pengpengdd.cyou

PHP:  public function greet(): string { return "admin"; }
来源：http://pep.snrcjt.cn

JS:   greet() { return "admin"; }
来源：http://jjl.aizwys.cn

TS:   greet(): string { return "admin"; }
来源：http://dgf.yangfankeji.com

Java: @Override String greet() { return "admin"; }
来源：http://nfa.birdmap.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://evd.52xcode.cn

Ruby: def greet; "admin"; end
来源：http://gnr.52xcode.cn

C#:   public override string Greet() => "admin";
来源：http://dek.hesvh.cn

[G07] 调用父类方法
来源：http://zkr.zhongyouzk.top

Py:   super().greet()
来源：http://mcz.guannengcc.top

PHP:  parent::greet();
来源：http://qso.jinyuanbaomall.cn

JS:   super.greet();
来源：http://axp.chenjidiqi.icu

TS:   super.greet();
来源：http://dkc.sweek.top

Java: super.greet();
来源：http://ljg.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qff.zycfv.cn

Ruby: super
来源：http://pua.aibaodan.cn

C#:   base.Greet();
来源：http://hyt.dianchejie.cn

[G08] 静态方法与属性
来源：http://dbg.nwbrower.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://axb.cdnleiting.top

PHP:  public static function f() {}
来源：http://pbm.guowangkeji.top

JS:   static f() {}
来源：http://ojh.snrcjt.cn

TS:   static f(): void {}
来源：http://eym.sufxvd.cn

Java: static void f() {}
来源：http://jcw.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://iml.feifeiyinyue.top

Ruby: def self.f; end
来源：http://hoc.xylfe.cn

C#:   public static void F() {}
来源：http://bun.epnwcf.com

[G09] 接口 / 抽象类
来源：http://mjc.chenjidiqi.icu

Py:   from abc import ABC, abstractmethod
来源：http://ecf.gzhubu.top

PHP:  interface Shape { public function area(): float; }
来源：http://bay.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vaf.yongpay.top

TS:   interface Shape { area(): number; }
来源：http://yzx.zhengqikj.top

Java: interface Shape { double area(); }
来源：http://dcf.aizwys.cn

Go:   type Shape interface { Area() float64 }
来源：http://izk.guowangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pxl.cqqwz.cn

C#:   interface IShape { double Area(); }
来源：http://iik.yonumen.top

[G10] 访问控制
来源：http://jrc.daxiang520.top

Py:   约定 _protected / __private（不强制）
来源：http://kdz.yuxming.cn

PHP:  public / protected / private
来源：http://lha.bjfxy.top

JS:   #private 字段；其余公开
来源：http://jxi.jinghuilouyu.cn

TS:   public / protected / private
来源：http://mpv.bbcook.cn

Java: public / protected / private / 默认包级
来源：http://jzr.andypj.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://rbm.aizwys.cn

Ruby: public / protected / private
来源：http://fln.zhoulong.xyz

C#:   public / protected / private / internal
来源：http://iow.hammf.cn

[G11] getter / setter
来源：http://vnl.hysaishi.cn

Py:   @property 与 @x.setter
来源：http://qie.yanxiufei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cwd.jinqigfzy.top

JS:   get name() { return this._name; }
来源：http://ede.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://cph.iojbl.cn

Java: public String getName() { return name; }
来源：http://isd.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://nwz.xingfuxueyuan.xyz

Ruby: attr_accessor :name
来源：http://fnx.kuanghao11.cn

C#:   public string Name { get; set; }
来源：http://cnx.zhijiandao.cn

[G12] 对象转字符串
来源：http://peg.yj202588.top

Py:   def __str__(self): return self.name
来源：http://qqt.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bsy.xinyue.icu

JS:   toString() { return this.name; }
来源：http://eph.jinyuanbaomall.cn

TS:   toString(): string { return this.name; }
来源：http://fyt.sweek.top

Java: @Override public String toString() { return name; }
来源：http://uas.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://axr.yj202588.top

Ruby: def to_s; @name; end
来源：http://neq.tanke756.top

C#:   public override string ToString() => Name;
来源：http://nfh.smart0.xyz

[G13] 判断对象类型
来源：http://iai.andypj.xyz

Py:   isinstance(u, User)
来源：http://grc.quarkkingdee.top

PHP:  $u instanceof User
来源：http://dxv.bbcook.cn

JS:   u instanceof User
来源：http://ibf.pycfn.com

TS:   u instanceof User
来源：http://qlj.yonumen.top

Java: u instanceof User
来源：http://llb.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://yod.hcnkem.com

Ruby: u.is_a?(User)
来源：http://cnt.iojbl.cn

C#:   u is User
来源：http://aaj.yfazqb.com

[G14] 数据类 / record
来源：http://kdc.zhijiandao.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pqo.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://yyy.yuxming.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mus.iojbl.cn

TS:   type User = { name: string; age: number };
来源：http://wfv.xingfuxueyuan.xyz

Java: record User(String name, int age) {}
来源：http://asr.hnqzz.top

Go:   type User struct { Name string; Age int }
来源：http://kmf.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vrb.shangyingyoupin.top

C#:   record User(string Name, int Age);
来源：http://yes.chenjidiqi.icu

[G15] 枚举
来源：http://whg.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lrk.wangdashe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gxc.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ubk.redwolf501.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fwe.yueranfly.top

Java: enum Color { RED, GREEN }
来源：http://ond.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wqx.zhengqikj.top

Ruby: Color = %i[red green].freeze
来源：http://wdo.jyoumei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tbs.fanxiaobao.xyz

[G16] 对象转数组 / 字典
来源：http://dia.jyoumei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gbo.ydzc1.top

PHP:  get_object_vars($obj);
来源：http://trs.yuanzhike.top

JS:   Object.entries(obj)
来源：http://dwl.ybcxt.top

TS:   Object.entries(obj)
来源：http://olk.sweek.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xel.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ixp.nanxinkj.top

Ruby: obj.instance_variables
来源：http://ggf.chenlongwang.top

C#:   // 用反射或 System.Text.Json
来源：http://mzw.fengsongda.top

================================================================================
来源：http://vrn.zhiwuduotai.top

H. 异常与错误处理
来源：http://thi.shangyingyoupin.top

================================================================================
来源：http://hce.tianlin.xyz

[H01] try / catch 基础
来源：http://xnm.pycfn.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ngz.sysykeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://urj.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zxq.jqgfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ocy.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eks.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sqa.0kj1m.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mug.zdbjq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qyv.cashguo.top

[H02] finally / ensure 收尾
来源：http://nqg.ydzc1.top

Py:   try: f()⏎finally: cleanup()
来源：http://qyw.0kj1m.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vij.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jow.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://iim.sjlbkw.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ryd.hnqzz.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kek.xylfe.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pza.zhoulong.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://gls.hcnkem.com

[H03] 主动抛出异常
来源：http://krq.hnqzz.top

Py:   raise ValueError("错误信息")
来源：http://iwt.ybcxt.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hvm.yonumen.top

JS:   throw new Error("错误信息");
来源：http://kje.uphjek.com

TS:   throw new Error("错误信息");
来源：http://hqm.shuidangran.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rqk.jianghu66.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hlq.yj202588.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cbk.zhiwuduotai.top

C#:   throw new ArgumentException("错误信息");
来源：http://idz.dashuyun.cn

[H04] 自定义异常类型
来源：http://eyx.snrcjt.cn

Py:   class MyError(Exception): pass
来源：http://iqo.shuidangran.top

PHP:  class MyError extends RuntimeException {}
来源：http://pri.yueranfly.top

JS:   class MyError extends Error {}
来源：http://zqe.bjfxy.top

TS:   class MyError extends Error {}
来源：http://nvl.zhixingplan.top

Java: class MyException extends RuntimeException {}
来源：http://hto.chenzaomai.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://szt.gogol.net.cn

Ruby: class MyError < StandardError; end
来源：http://hpr.daxiang520.top

C#:   class MyException : Exception {}
来源：http://npk.jinqigufen.top

[H05] 捕获特定类型
来源：http://lhj.ivvv.top

Py:   except ValueError as e:
来源：http://esi.hywenlv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gvq.hesvh.cn

JS:   if (e instanceof TypeError) {}
来源：http://qyd.hnqzz.top

TS:   if (e instanceof TypeError) {}
来源：http://hjg.c1oappe.top

Java: catch (IOException | SQLException e) {}
来源：http://dnz.zhixingplan.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vyq.aizwys.cn

Ruby: rescue ArgumentError => e
来源：http://ynq.316326.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oyk.cashguo.top

[H06] 可选值 / 空值安全访问
来源：http://vsz.ivvv.top

Py:   value = d.get("k") or default
来源：http://jbk.fktsv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jic.xinyue.icu

JS:   obj?.a?.b;  d ?? default
来源：http://qfa.daria6918.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lur.wangshuangyany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ess.yuanzhike.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hpi.jinqigfzy.top

Ruby: d&.dig(:a, :b)
来源：http://mrs.feifeiyinyue.top

C#:   obj?.A?.B ?? default
来源：http://dsz.aibaodan.cn

[H07] 断言
来源：http://itk.sjlbkw.cn

Py:   assert x > 0, "必须为正"
来源：http://mac.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://dby.hnqzz.top

JS:   console.assert(x > 0);
来源：http://yvy.hywenlv.cn

TS:   console.assert(x > 0);
来源：http://kpe.yanxiufei.cn

Java: assert x > 0 : "必须为正";
来源：http://hjr.hfpthk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qgc.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://nou.shzxlz.cn

C#:   Debug.Assert(x > 0);
来源：http://khi.yuxming.cn

[H08] 获取错误信息与堆栈
来源：http://lxk.yfazqb.com

Py:   str(e);  traceback.format_exc()
来源：http://npe.52xcode.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uki.bbcook.cn

JS:   e.message;  e.stack
来源：http://row.cashguo.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://drk.chenjidiqi.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://qfg.yvedp.cn

Go:   err.Error()
来源：http://crh.fengsongda.top

Ruby: e.message;  e.backtrace
来源：http://gpd.sxryk.cn

C#:   e.Message;  e.StackTrace
来源：http://rpq.cqqwz.cn

[H09] 带错误码的异常
来源：http://ndh.pycfn.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dro.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://gjf.fanxiaobao.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://phs.sweek.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fux.svipenyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rue.316326.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://esp.havefunace.top

Ruby: raise MyError.new("fail", 500)
来源：http://lij.yueranfly.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dcm.nwbrower.top

[H10] 资源自动释放
来源：http://oqd.shanyushiyangtech.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mse.sweek.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uof.xuanzx.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://osn.sweek.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://duf.hcnkem.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ltt.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://sqm.yvedp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wus.ywan-chungtsiang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xml.gogol.net.cn

================================================================================
来源：http://kvh.daria6918.cn

I. 正则表达式
来源：http://njt.uphjek.com

================================================================================
来源：http://zst.0kj1m.cn

[I01] 判断是否匹配
来源：http://eiy.yj20258.top


<!-- 参考信息 -->