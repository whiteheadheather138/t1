代发 wailian999

C#:   File.Exists("a.txt")
来源：http://cuc.ehwqpu.com

[F06] 删除文件
来源：http://mow.hesvh.cn

Py:   os.remove("a.txt")
来源：http://ocs.zhongyouzk.top

PHP:  unlink("a.txt");
来源：http://agk.gaohongyu789.top

JS:   fs.unlinkSync("a.txt")
来源：http://krj.kuanghao11.cn

TS:   fs.unlinkSync("a.txt")
来源：http://otx.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cwi.chenlongwang.top

Go:   os.Remove("a.txt")
来源：http://jcx.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://yfv.zhengqikj.top

C#:   File.Delete("a.txt");
来源：http://cdo.yj202588.top

[F07] 创建目录（含多级）
来源：http://pks.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pus.cashguo.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xhp.52xcode.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://exh.ehwqpu.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ydz.andypj.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gcb.ydjk.org.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dgy.xuetiantiany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hel.meibo888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hbi.ydzc1.top

[F08] 遍历目录
来源：http://gef.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://raj.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://muh.cucudq.cn

JS:   fs.readdirSync("dir")
来源：http://vlo.jinyuanbaomall.cn

TS:   fs.readdirSync("dir")
来源：http://smu.yongpay.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wgi.jiagoushi.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xhv.c1oappe.top

Ruby: Dir.children("dir")
来源：http://kgb.hysaishi.cn

C#:   Directory.GetFiles("dir")
来源：http://vsv.gzhubu.top

[F09] 获取文件大小
来源：http://hnn.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://kbj.hnqzz.top

PHP:  filesize("a.txt");
来源：http://sxu.uphjek.com

JS:   fs.statSync("a.txt").size
来源：http://fur.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://kni.daxiang520.top

Java: Files.size(Path.of("a.txt"))
来源：http://xau.fanxiaobao.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nvp.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://god.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://yws.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://pwt.yuanzhike.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://thz.yj20258.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pwi.jinqigfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dhy.bbcook.cn

TS:   path.extname("a.txt")
来源：http://ayd.jinqigufen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ibs.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tqy.epnwcf.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pwn.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vyg.xuetiantiany.cn

[F11] 复制与移动文件
来源：http://kmm.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fbu.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://duu.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sqe.jinghuilouyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://umb.chenjidiqi.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yej.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nvv.nanxinkj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jdc.vqdsnc.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wew.9152youxi.cn

[F12] CSV 读写
来源：http://mvt.svipenyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ycf.hysaishi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dgo.yj202588.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yyg.kuanghao11.cn

TS:   // 同上
来源：http://med.hysaishi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://msv.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gvt.hysaishi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ywt.zhixingplan.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ewp.yueranfly.top

================================================================================
来源：http://dwm.aizwys.cn

G. 面向对象
来源：http://jdj.jianghu66.top

================================================================================
来源：http://ger.yj20258.top

[G01] 定义类
来源：http://qyq.guannengcc.top

Py:   class User: pass
来源：http://fdj.jianghu66.top

PHP:  class User {}
来源：http://ysp.tanke756.top

JS:   class User {}
来源：http://fpn.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://hzn.hammf.cn

Java: class User {}
来源：http://nox.tarul.cn

Go:   type User struct { Name string }
来源：http://pxg.cdnleiting.top

Ruby: class User; end
来源：http://qvk.hammf.cn

C#:   class User {}
来源：http://gia.yongpay.top

[G02] 构造函数
来源：http://kcl.52xcode.cn

Py:   def __init__(self, name): self.name = name
来源：http://lih.yongpay.top

PHP:  public function __construct(public string $name) {}
来源：http://wof.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://vow.pengpengdd.cyou

TS:   constructor(public name: string) {}
来源：http://jst.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://qne.gogol.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wvd.tanke756.top

Ruby: def initialize(name); @name = name; end
来源：http://zey.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://fvv.9152youxi.cn

[G03] 实例属性
来源：http://gow.meibo888.top

Py:   self.name = "x"
来源：http://pol.smart0.xyz

PHP:  public string $name = "x";
来源：http://sgf.haohaochexian.top

JS:   this.name = "x";
来源：http://tph.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://uga.ivvv.top

Java: private String name;
来源：http://uwg.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vgf.shangyingyoupin.top

Ruby: @name = "x"
来源：http://big.guowangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://evd.c1oappe.top

[G04] 定义方法
来源：http://fzu.gogol.net.cn

Py:   def greet(self): return self.name
来源：http://slz.zdqjudy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hac.xziqi.cn

JS:   greet() { return this.name; }
来源：http://zyg.bbcook.cn

TS:   greet(): string { return this.name; }
来源：http://yzc.smart0.xyz

Java: String greet() { return name; }
来源：http://tco.hongshengwenyu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://evv.yuanzhike.top

Ruby: def greet; @name; end
来源：http://tza.jyoumei.cn

C#:   public string Greet() => Name;
来源：http://utj.ctjpmb.com

[G05] 继承
来源：http://dkc.jlsjyb.cn

Py:   class Admin(User): pass
来源：http://ffq.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://ptc.pengpengdd.cyou

JS:   class Admin extends User {}
来源：http://eox.zycfv.cn

TS:   class Admin extends User {}
来源：http://qho.yuxming.cn

Java: class Admin extends User {}
来源：http://dgt.0kj1m.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tbs.jinqigfzy.top

Ruby: class Admin < User; end
来源：http://rad.sysykeji.top

C#:   class Admin : User {}
来源：http://ynv.shuidangran.top

[G06] 重写方法
来源：http://gae.fanxiaobao.xyz

Py:   def greet(self): return "admin"
来源：http://phq.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://diz.nanxinkj.top

JS:   greet() { return "admin"; }
来源：http://pnf.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://uqu.chenlongwang.top

Java: @Override String greet() { return "admin"; }
来源：http://ugo.yj20258888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://btk.fzhhl.top

Ruby: def greet; "admin"; end
来源：http://uye.yangfankeji.com

C#:   public override string Greet() => "admin";
来源：http://fxv.jqgfzy.top

[G07] 调用父类方法
来源：http://ybb.c1oappe.top

Py:   super().greet()
来源：http://lfq.cheryme.top

PHP:  parent::greet();
来源：http://lpo.hcnkem.com

JS:   super.greet();
来源：http://cgy.tian-w.cn

TS:   super.greet();
来源：http://vfy.pengpengdd.cyou

Java: super.greet();
来源：http://jtg.svipenyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://syl.wangdashe.top

Ruby: super
来源：http://nlg.aibaodan.cn

C#:   base.Greet();
来源：http://pfp.hywenlv.cn

[G08] 静态方法与属性
来源：http://gmj.jinyuanbaomall.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bxy.smart0.xyz

PHP:  public static function f() {}
来源：http://yyw.tianlin.xyz

JS:   static f() {}
来源：http://wbf.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://kyn.chenzaomai.com

Java: static void f() {}
来源：http://nzw.sweek.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nzv.hfpthk.cn

Ruby: def self.f; end
来源：http://tan.hfpthk.cn

C#:   public static void F() {}
来源：http://nfo.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://xoy.bjfxy.top

Py:   from abc import ABC, abstractmethod
来源：http://jec.vehdjk.com

PHP:  interface Shape { public function area(): float; }
来源：http://riv.snrcjt.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cnb.jiagoushi.top

TS:   interface Shape { area(): number; }
来源：http://yxx.ywan-chungtsiang.top

Java: interface Shape { double area(); }
来源：http://peu.fengsongda.top

Go:   type Shape interface { Area() float64 }
来源：http://euz.bjfxy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eea.pycfn.com

C#:   interface IShape { double Area(); }
来源：http://xba.hfpthk.cn

[G10] 访问控制
来源：http://smu.xinyue.icu

Py:   约定 _protected / __private（不强制）
来源：http://eqb.iojbl.cn

PHP:  public / protected / private
来源：http://tur.daria6918.cn

JS:   #private 字段；其余公开
来源：http://toc.xziqi.cn

TS:   public / protected / private
来源：http://iiy.yuxming.cn

Java: public / protected / private / 默认包级
来源：http://pju.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qtw.yj202588.top

Ruby: public / protected / private
来源：http://fgm.chenlongwang.top

C#:   public / protected / private / internal
来源：http://ttw.yueranfly.top

[G11] getter / setter
来源：http://mba.yonumen.top

Py:   @property 与 @x.setter
来源：http://hgu.shanyushiyangtech.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ofg.smart0.xyz

JS:   get name() { return this._name; }
来源：http://zqc.yj20258.top

TS:   get name(): string { return this._name; }
来源：http://rmr.daxiang520.top

Java: public String getName() { return name; }
来源：http://dob.yj20258888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dnv.hammf.cn

Ruby: attr_accessor :name
来源：http://kli.bbcook.cn

C#:   public string Name { get; set; }
来源：http://dxx.andypj.xyz

[G12] 对象转字符串
来源：http://yrt.316326.xyz

Py:   def __str__(self): return self.name
来源：http://xtv.hesvh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hhe.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://xvj.jyoumei.cn

TS:   toString(): string { return this.name; }
来源：http://dhz.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://ylf.0kj1m.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xzv.zhixingplan.top

Ruby: def to_s; @name; end
来源：http://byj.svipenyu.cn

C#:   public override string ToString() => Name;
来源：http://ylq.xziqi.cn

[G13] 判断对象类型
来源：http://lfr.hnxiangtu.top

Py:   isinstance(u, User)
来源：http://lzr.sweek.top

PHP:  $u instanceof User
来源：http://tto.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://qma.hysaishi.cn

TS:   u instanceof User
来源：http://bou.xylfe.cn

Java: u instanceof User
来源：http://gva.ctjpmb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://fuh.gzhubu.top

Ruby: u.is_a?(User)
来源：http://cfx.snrcjt.cn

C#:   u is User
来源：http://emq.cashguo.top

[G14] 数据类 / record
来源：http://rqp.tarul.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pyf.aibaodan.cn

PHP:  // 用 readonly 属性模拟
来源：http://bwh.cqqwz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fyk.yj20258.top

TS:   type User = { name: string; age: number };
来源：http://sjj.vehdjk.com

Java: record User(String name, int age) {}
来源：http://ezo.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://wnr.redwolf501.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ogr.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://wzq.nanxinkj.top

[G15] 枚举
来源：http://xks.zhijiandao.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hiq.wangshuangyany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://prc.shuidangran.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zup.xylfe.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ozs.svipenyu.cn

Java: enum Color { RED, GREEN }
来源：http://qyk.wangshuangyany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nci.cqqwz.cn

Ruby: Color = %i[red green].freeze
来源：http://ees.ehwqpu.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zva.dashuyun.cn

[G16] 对象转数组 / 字典
来源：http://clf.52xcode.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ilr.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://umn.svipenyu.cn

JS:   Object.entries(obj)
来源：http://vuh.yuanzhike.top

TS:   Object.entries(obj)
来源：http://mvj.gaohongyu789.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bxe.c1oappe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pwx.fanxiaobao.xyz

Ruby: obj.instance_variables
来源：http://nxl.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://gab.andypj.xyz

================================================================================
来源：http://hnk.bjfxy.top

H. 异常与错误处理
来源：http://ber.hfpthk.cn

================================================================================
来源：http://lho.pengpengdd.cyou

[H01] try / catch 基础
来源：http://yak.jqgfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yvy.yfazqb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mxr.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://slt.yueranfly.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://szc.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iha.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ffa.9152youxi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vqa.zhoulong.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cuk.bbcook.cn

[H02] finally / ensure 收尾
来源：http://mad.nanxinkj.top

Py:   try: f()⏎finally: cleanup()
来源：http://wmc.gogol.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fzg.yuanzhike.top

JS:   try { f(); } finally { cleanup(); }
来源：http://yaf.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gvt.ydjk.org.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jlb.yvedp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lef.hongshengwenyu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tsl.jiagoushi.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://erc.fzhhl.top

[H03] 主动抛出异常
来源：http://pju.ydjk.org.cn

Py:   raise ValueError("错误信息")
来源：http://fyz.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ghx.ivvv.top

JS:   throw new Error("错误信息");
来源：http://pke.sjlbkw.cn

TS:   throw new Error("错误信息");
来源：http://git.shuidangran.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qvv.smart0.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ftb.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hql.zycfv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://keq.yj20258888.top

[H04] 自定义异常类型
来源：http://tnw.jlsjyb.cn

Py:   class MyError(Exception): pass
来源：http://fan.hnxiangtu.top

PHP:  class MyError extends RuntimeException {}
来源：http://jxz.wangdashe.top

JS:   class MyError extends Error {}
来源：http://ccx.hysaishi.cn

TS:   class MyError extends Error {}
来源：http://yqi.yj202588.top

Java: class MyException extends RuntimeException {}
来源：http://syt.sjlbkw.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nqt.hnqzz.top

Ruby: class MyError < StandardError; end
来源：http://jly.zdqjudy.top

C#:   class MyException : Exception {}
来源：http://wdy.cheryme.top

[H05] 捕获特定类型
来源：http://jed.tanke756.top

Py:   except ValueError as e:
来源：http://eyf.guowangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mex.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://osp.9152youxi.cn

TS:   if (e instanceof TypeError) {}
来源：http://nmw.sweek.top

Java: catch (IOException | SQLException e) {}
来源：http://jvn.hfpthk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yum.cucudq.cn

Ruby: rescue ArgumentError => e
来源：http://roo.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cjv.dashuyun.cn

[H06] 可选值 / 空值安全访问
来源：http://yrm.jinyuanbaomall.cn

Py:   value = d.get("k") or default
来源：http://pqr.jlsjyb.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tyf.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://pvu.bjfxy.top

TS:   obj?.a?.b;  d ?? default
来源：http://vso.daria6918.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fhx.epnwcf.com

Go:   if v, ok := m["k"]; ok { }
来源：http://thz.pengpengdd.cyou

Ruby: d&.dig(:a, :b)
来源：http://kid.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://kaw.snrcjt.cn

[H07] 断言
来源：http://zwn.xingfuxueyuan.xyz

Py:   assert x > 0, "必须为正"
来源：http://ytz.hesvh.cn

PHP:  assert($x > 0);
来源：http://wsz.epnwcf.com

JS:   console.assert(x > 0);
来源：http://ejh.yj202588.top

TS:   console.assert(x > 0);
来源：http://igo.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://eop.shanyushiyangtech.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xlx.dashuyun.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wjr.yangfankeji.com

C#:   Debug.Assert(x > 0);
来源：http://xbq.pengpengdd.cyou

[H08] 获取错误信息与堆栈
来源：http://dip.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://nbw.ywan-chungtsiang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://klh.hnqzz.top

JS:   e.message;  e.stack
来源：http://coz.daxiang520.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dzd.guannengcc.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qmj.epnwcf.com

Go:   err.Error()
来源：http://plg.gzhubu.top

Ruby: e.message;  e.backtrace
来源：http://ksz.sjlbkw.cn

C#:   e.Message;  e.StackTrace
来源：http://xsu.sjlbkw.cn

[H09] 带错误码的异常
来源：http://ljd.fanxiaobao.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nyl.chenlongwang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://esk.gaohongyu789.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rug.tianlin.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ygl.redwolf501.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wpy.jinqigfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ayf.jinqigfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://out.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://keh.shanyushiyangkeji.top

[H10] 资源自动释放
来源：http://qes.nwbrower.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://buk.ywan-chungtsiang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gdw.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yte.sjlbkw.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qfp.meibo888.top


<!-- 参考信息 -->