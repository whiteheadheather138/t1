代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://yzg.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://kxc.gzhubu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fdc.fzhhl.top

Go:   os.Remove("a.txt")
来源：http://vco.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://fof.aibaodan.cn

C#:   File.Delete("a.txt");
来源：http://yaa.jianghu66.top

[F07] 创建目录（含多级）
来源：http://rpu.nwbrower.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lre.andypj.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iat.guowangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mex.52xcode.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://enr.daxiang520.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vhd.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zxr.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://alh.jianghu66.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pyx.yangfankeji.com

[F08] 遍历目录
来源：http://xnv.yfazqb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://poj.zhiwuduotai.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vwm.tarul.cn

JS:   fs.readdirSync("dir")
来源：http://foj.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://qwm.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zvg.dianchejie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ldh.jqgufenzy.top

Ruby: Dir.children("dir")
来源：http://eox.xinyue.icu

C#:   Directory.GetFiles("dir")
来源：http://uah.sweek.top

[F09] 获取文件大小
来源：http://yjs.daria6918.cn

Py:   os.path.getsize("a.txt")
来源：http://elr.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://ipi.dashuyun.cn

JS:   fs.statSync("a.txt").size
来源：http://bpz.feifeiyinyue.top

TS:   fs.statSync("a.txt").size
来源：http://toy.xingfuxueyuan.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://piz.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cyo.andypj.xyz

Ruby: File.size("a.txt")
来源：http://klw.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://yuc.xingfuxueyuan.xyz

[F10] 取文件扩展名 / 文件名
来源：http://byc.cdnleiting.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dux.shanyushiyangtech.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rae.sjlbkw.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pya.fengsongda.top

TS:   path.extname("a.txt")
来源：http://rvz.wangshuangyany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mvg.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dyl.haohaochexian.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qgg.tarul.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hys.nanxinkj.top

[F11] 复制与移动文件
来源：http://xry.jqgfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sbp.jinqigufen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qgn.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zff.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uja.snrcjt.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hrw.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lcx.dianchejie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lqq.jqgfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zaa.meibo888.top

[F12] CSV 读写
来源：http://xvp.zhongyouzk.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xoa.sysykeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iob.daria6918.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bsw.kuanghao11.cn

TS:   // 同上
来源：http://lbf.sysykeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vbj.yangfankeji.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://edj.gzhubu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://azz.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xhk.c1oappe.top

================================================================================
来源：http://yge.smart0.xyz

G. 面向对象
来源：http://zzv.jqgufenzy.top

================================================================================
来源：http://rww.chenlongwang.top

[G01] 定义类
来源：http://wkz.redwolf501.top

Py:   class User: pass
来源：http://klx.ybcxt.top

PHP:  class User {}
来源：http://qvp.sysykeji.top

JS:   class User {}
来源：http://rvy.tanke756.top

TS:   class User { name: string = ""; }
来源：http://cbu.guannengcc.top

Java: class User {}
来源：http://rjh.sysykeji.top

Go:   type User struct { Name string }
来源：http://jtr.yangfankeji.com

Ruby: class User; end
来源：http://cqp.smart0.xyz

C#:   class User {}
来源：http://rly.hnqzz.top

[G02] 构造函数
来源：http://joc.bjfxy.top

Py:   def __init__(self, name): self.name = name
来源：http://wzv.fehbvm.com

PHP:  public function __construct(public string $name) {}
来源：http://qjk.9152youxi.cn

JS:   constructor(name) { this.name = name; }
来源：http://bul.fktsv.cn

TS:   constructor(public name: string) {}
来源：http://cdb.xuetiantiany.cn

Java: User(String name) { this.name = name; }
来源：http://ggc.tarul.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dbg.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://kgb.kuanghao11.cn

C#:   public User(string name) { Name = name; }
来源：http://djo.yj20258.top

[G03] 实例属性
来源：http://wus.nanxuanxn.top

Py:   self.name = "x"
来源：http://dfn.fzhhl.top

PHP:  public string $name = "x";
来源：http://xti.svipenyu.cn

JS:   this.name = "x";
来源：http://pdj.nanxuanxn.top

TS:   name: string = "x";
来源：http://afg.yueranfly.top

Java: private String name;
来源：http://ypr.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ebh.yongpay.top

Ruby: @name = "x"
来源：http://hlu.jlsjyb.cn

C#:   public string Name { get; set; } = "x";
来源：http://off.cdnleiting.top

[G04] 定义方法
来源：http://emw.shanyushiyangtech.top

Py:   def greet(self): return self.name
来源：http://zxo.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lta.zdqjudy.top

JS:   greet() { return this.name; }
来源：http://brg.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://zui.tian-w.cn

Java: String greet() { return name; }
来源：http://gnu.hnqzz.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bxa.jqgfzy.top

Ruby: def greet; @name; end
来源：http://frd.yuanzhike.top

C#:   public string Greet() => Name;
来源：http://dne.hfpthk.cn

[G05] 继承
来源：http://mpr.sjlbkw.cn

Py:   class Admin(User): pass
来源：http://izz.xinyue.icu

PHP:  class Admin extends User {}
来源：http://gef.xylfe.cn

JS:   class Admin extends User {}
来源：http://mvv.shanyushiyangkeji.top

TS:   class Admin extends User {}
来源：http://fwp.aibaodan.cn

Java: class Admin extends User {}
来源：http://vvs.havefunace.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hlb.yvedp.cn

Ruby: class Admin < User; end
来源：http://hhi.yongpay.top

C#:   class Admin : User {}
来源：http://zxm.hywenlv.cn

[G06] 重写方法
来源：http://nie.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://gts.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://xaf.yanxiufei.cn

JS:   greet() { return "admin"; }
来源：http://cme.gaohongyu789.top

TS:   greet(): string { return "admin"; }
来源：http://lri.bjfxy.top

Java: @Override String greet() { return "admin"; }
来源：http://bqi.yueranfly.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hob.jianghu66.top

Ruby: def greet; "admin"; end
来源：http://cdk.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://ebl.epnwcf.com

[G07] 调用父类方法
来源：http://ril.yuxming.cn

Py:   super().greet()
来源：http://jes.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://mir.sjlbkw.cn

JS:   super.greet();
来源：http://gdz.yuxming.cn

TS:   super.greet();
来源：http://uxz.svipenyu.cn

Java: super.greet();
来源：http://anx.snrcjt.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ncx.hysaishi.cn

Ruby: super
来源：http://cdg.ctjpmb.com

C#:   base.Greet();
来源：http://msp.jqgfzy.top

[G08] 静态方法与属性
来源：http://pmp.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xca.shangyingyoupin.top

PHP:  public static function f() {}
来源：http://cvz.chenzaomai.com

JS:   static f() {}
来源：http://gwy.jinqigufen.top

TS:   static f(): void {}
来源：http://ccs.yangfankeji.com

Java: static void f() {}
来源：http://tev.yfazqb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://pfl.shzxlz.cn

Ruby: def self.f; end
来源：http://saq.smart0.xyz

C#:   public static void F() {}
来源：http://tnt.xuanzx.com

[G09] 接口 / 抽象类
来源：http://msl.mhx1999.top

Py:   from abc import ABC, abstractmethod
来源：http://msf.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xzf.dianchejie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wek.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://qhl.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://ejv.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://nwt.gotoacloud.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wqx.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://iaf.yuanzhike.top

[G10] 访问控制
来源：http://pxi.xinyue.icu

Py:   约定 _protected / __private（不强制）
来源：http://fce.yuxming.cn

PHP:  public / protected / private
来源：http://ggq.cucudq.cn

JS:   #private 字段；其余公开
来源：http://zvk.xuetiantiany.cn

TS:   public / protected / private
来源：http://ihd.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://ite.pengpengdd.cyou

Go:   首字母大写可导出，小写仅包内可见
来源：http://oze.chenzaomai.com

Ruby: public / protected / private
来源：http://ecv.yfazqb.com

C#:   public / protected / private / internal
来源：http://zty.zhaomingkeji.xyz

[G11] getter / setter
来源：http://zkq.hnxiangtu.top

Py:   @property 与 @x.setter
来源：http://rch.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ggs.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://vsm.quarkkingdee.top

TS:   get name(): string { return this._name; }
来源：http://lzi.yonumen.top

Java: public String getName() { return name; }
来源：http://toc.pycfn.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://dlm.jinqigfzy.top

Ruby: attr_accessor :name
来源：http://llb.hnqzz.top

C#:   public string Name { get; set; }
来源：http://zxr.kuanghao11.cn

[G12] 对象转字符串
来源：http://nsy.sjlbkw.cn

Py:   def __str__(self): return self.name
来源：http://kah.yuxming.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vjx.hcnkem.com

JS:   toString() { return this.name; }
来源：http://xyd.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://rff.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://xhm.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://irj.havefunace.top

Ruby: def to_s; @name; end
来源：http://yps.gotoacloud.top

C#:   public override string ToString() => Name;
来源：http://dmz.jyoumei.cn

[G13] 判断对象类型
来源：http://kfq.yvedp.cn

Py:   isinstance(u, User)
来源：http://rak.pycfn.com

PHP:  $u instanceof User
来源：http://fem.jlsjyb.cn

JS:   u instanceof User
来源：http://eov.ydjk.org.cn

TS:   u instanceof User
来源：http://jek.jinqigufen.top

Java: u instanceof User
来源：http://ipo.hysaishi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cbv.tarul.cn

Ruby: u.is_a?(User)
来源：http://qyz.xylfe.cn

C#:   u is User
来源：http://ckc.mhx1999.top

[G14] 数据类 / record
来源：http://dnh.havefunace.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ina.gaohongyu789.top

PHP:  // 用 readonly 属性模拟
来源：http://zws.jqgfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://uci.havefunace.top

TS:   type User = { name: string; age: number };
来源：http://hfr.cdnleiting.top

Java: record User(String name, int age) {}
来源：http://ssq.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://amw.jlsjyb.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://agq.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://rtz.daria6918.cn

[G15] 枚举
来源：http://kzk.jinqigfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://szt.yj20258888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nsz.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yla.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lzi.quarkkingdee.top

Java: enum Color { RED, GREEN }
来源：http://wma.hnqzz.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ntj.redwolf501.top

Ruby: Color = %i[red green].freeze
来源：http://jjf.guannengcc.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wrf.sweek.top

[G16] 对象转数组 / 字典
来源：http://dvn.shangyingyoupin.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tae.tanke756.top

PHP:  get_object_vars($obj);
来源：http://cfg.redwolf501.top

JS:   Object.entries(obj)
来源：http://shs.c1oappe.top

TS:   Object.entries(obj)
来源：http://wsj.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jsi.hnqzz.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bey.ybcxt.top

Ruby: obj.instance_variables
来源：http://ify.fktsv.cn

C#:   // 用反射或 System.Text.Json
来源：http://jwd.9152youxi.cn

================================================================================
来源：http://meu.jianghu66.top

H. 异常与错误处理
来源：http://uzf.shzxlz.cn

================================================================================
来源：http://ddm.cashguo.top

[H01] try / catch 基础
来源：http://zut.guannengcc.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iet.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://twk.cqqwz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bkr.cashguo.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gef.wangdashe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qlb.aibaodan.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rbn.andypj.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nzd.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nut.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://hkr.cheryme.top

Py:   try: f()⏎finally: cleanup()
来源：http://xvs.yj202588.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rvj.ydjk.org.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xno.nwbrower.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dkg.ydzc1.top

Java: try { f(); } finally { cleanup(); }
来源：http://rrx.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://euu.yueranfly.top

Ruby: begin; f; ensure; cleanup; end
来源：http://soe.9152youxi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ofz.wangshuangyany.cn

[H03] 主动抛出异常
来源：http://wjc.snrcjt.cn

Py:   raise ValueError("错误信息")
来源：http://roh.yueranfly.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eyp.gzhubu.top

JS:   throw new Error("错误信息");
来源：http://nuk.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://qyl.ydjk.org.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tcz.xziqi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ftp.xinyue.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://ohu.jianghu66.top

C#:   throw new ArgumentException("错误信息");
来源：http://aei.wangdashe.top

[H04] 自定义异常类型
来源：http://vda.zhaomingkeji.xyz

Py:   class MyError(Exception): pass
来源：http://tou.shzxlz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hjo.nanxuanxn.top

JS:   class MyError extends Error {}
来源：http://xeg.xuetiantiany.cn

TS:   class MyError extends Error {}
来源：http://giu.316326.xyz

Java: class MyException extends RuntimeException {}
来源：http://mng.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iaw.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://edy.gogol.net.cn

C#:   class MyException : Exception {}
来源：http://lob.yvedp.cn

[H05] 捕获特定类型
来源：http://hnt.chenlongwang.top

Py:   except ValueError as e:
来源：http://nir.bbcook.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zcd.guowangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://wba.feifeiyinyue.top

TS:   if (e instanceof TypeError) {}
来源：http://hfy.shanyushiyangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://tzw.ivvv.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jyu.xziqi.cn

Ruby: rescue ArgumentError => e
来源：http://vey.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cjz.daria6918.cn

[H06] 可选值 / 空值安全访问
来源：http://kig.xuanzx.com

Py:   value = d.get("k") or default
来源：http://pmw.cashguo.top

PHP:  $v = $d["k"] ?? null;
来源：http://vbs.yanxiufei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pdj.redwolf501.top

TS:   obj?.a?.b;  d ?? default
来源：http://pny.iojbl.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cyz.ehwqpu.com

Go:   if v, ok := m["k"]; ok { }
来源：http://dyf.mhx1999.top

Ruby: d&.dig(:a, :b)
来源：http://mli.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://uaj.tianlin.xyz

[H07] 断言
来源：http://ove.ppjwa.cn

Py:   assert x > 0, "必须为正"
来源：http://zxx.quarkkingdee.top

PHP:  assert($x > 0);
来源：http://nmk.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://div.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://jjv.quarkkingdee.top

Java: assert x > 0 : "必须为正";
来源：http://ire.zycfv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ahl.shangyingyoupin.top

Ruby: raise "必须为正" unless x > 0
来源：http://nob.tian-w.cn

C#:   Debug.Assert(x > 0);
来源：http://qnj.jiagoushi.top

[H08] 获取错误信息与堆栈
来源：http://uhb.cashguo.top

Py:   str(e);  traceback.format_exc()
来源：http://czu.epnwcf.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rjs.zdbjq.cn

JS:   e.message;  e.stack
来源：http://ssn.haohaochexian.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bgx.cucudq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uti.daxiang520.top

Go:   err.Error()
来源：http://vbc.sjlbkw.cn

Ruby: e.message;  e.backtrace
来源：http://zuk.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://qva.c1oappe.top

[H09] 带错误码的异常
来源：http://mmn.epnwcf.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://brq.haohaochexian.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vky.guowangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lvx.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ymz.yuanzhike.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rxx.guowangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wbq.yongpay.top

Ruby: raise MyError.new("fail", 500)
来源：http://rhr.quarkkingdee.top

C#:   // 自定义异常类中加 Code 属性
来源：http://omb.pycfn.com

[H10] 资源自动释放
来源：http://fun.0kj1m.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://htl.yvedp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pgu.wangshuangyany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://afs.jlsjyb.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dtp.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cdo.yvedp.cn

Go:   defer f.Close()
来源：http://kcj.vehdjk.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bzg.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nxd.mhx1999.top


<!-- 参考信息 -->