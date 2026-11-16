代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rym.52xcode.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bnd.dianchejie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qay.tarul.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qeq.havefunace.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kbq.xylfe.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ysw.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gvh.feifeiyinyue.top

[F08] 遍历目录
来源：http://fmj.chenzaomai.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://krh.pycfn.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cdj.aibaodan.cn

JS:   fs.readdirSync("dir")
来源：http://amv.dianchejie.cn

TS:   fs.readdirSync("dir")
来源：http://sja.dashuyun.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mjx.hcnkem.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://ovv.shzxlz.cn

Ruby: Dir.children("dir")
来源：http://xlt.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://mxz.vqdsnc.cn

[F09] 获取文件大小
来源：http://pao.shuidangran.top

Py:   os.path.getsize("a.txt")
来源：http://fvk.zhijiandao.cn

PHP:  filesize("a.txt");
来源：http://afd.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://etm.snrcjt.cn

TS:   fs.statSync("a.txt").size
来源：http://aac.zycfv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rtm.yanxiufei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nnu.ehwqpu.com

Ruby: File.size("a.txt")
来源：http://cfi.shangyingyoupin.top

C#:   new FileInfo("a.txt").Length
来源：http://lbq.aizwys.cn

[F10] 取文件扩展名 / 文件名
来源：http://nrx.316326.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uzm.yueranfly.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dcl.zhoulong.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nug.yj20258888.top

TS:   path.extname("a.txt")
来源：http://sik.vqdsnc.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bxz.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ack.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dkl.pycfn.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://okn.daxiang520.top

[F11] 复制与移动文件
来源：http://uls.cashguo.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nsm.tanke756.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yru.andypj.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://prt.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://trg.c1oappe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://owd.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dxz.yuxming.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jbu.cdnleiting.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fqf.ydzc1.top

[F12] CSV 读写
来源：http://mll.hnxiangtu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lpt.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mam.zhijiandao.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eyr.ivvv.top

TS:   // 同上
来源：http://fmb.hfpthk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cou.uphjek.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jjs.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rdq.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xfd.chenzaomai.com

================================================================================
来源：http://guu.jiagoushi.top

G. 面向对象
来源：http://wut.gaohongyu789.top

================================================================================
来源：http://eqb.hnqzz.top

[G01] 定义类
来源：http://ufq.bbcook.cn

Py:   class User: pass
来源：http://fbi.316326.xyz

PHP:  class User {}
来源：http://ezy.c1oappe.top

JS:   class User {}
来源：http://ilv.yangfankeji.com

TS:   class User { name: string = ""; }
来源：http://trg.cheryme.top

Java: class User {}
来源：http://lse.zhixingplan.top

Go:   type User struct { Name string }
来源：http://zar.hnxiangtu.top

Ruby: class User; end
来源：http://zgq.yangfankeji.com

C#:   class User {}
来源：http://uwz.daria6918.cn

[G02] 构造函数
来源：http://kvf.cqqwz.cn

Py:   def __init__(self, name): self.name = name
来源：http://qrg.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://zgv.tianlin.xyz

JS:   constructor(name) { this.name = name; }
来源：http://mpa.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://xvh.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://iox.52xcode.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uku.hammf.cn

Ruby: def initialize(name); @name = name; end
来源：http://grh.iojbl.cn

C#:   public User(string name) { Name = name; }
来源：http://tak.fktsv.cn

[G03] 实例属性
来源：http://zch.birdmap.top

Py:   self.name = "x"
来源：http://hyt.ivvv.top

PHP:  public string $name = "x";
来源：http://bgu.c1oappe.top

JS:   this.name = "x";
来源：http://dtl.316326.xyz

TS:   name: string = "x";
来源：http://geq.sxryk.cn

Java: private String name;
来源：http://mjl.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dwd.yanxiufei.cn

Ruby: @name = "x"
来源：http://ato.jinyuanbaomall.cn

C#:   public string Name { get; set; } = "x";
来源：http://hdp.ehwqpu.com

[G04] 定义方法
来源：http://aly.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://sea.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bua.aibaodan.cn

JS:   greet() { return this.name; }
来源：http://lkt.sxryk.cn

TS:   greet(): string { return this.name; }
来源：http://aqm.ctjpmb.com

Java: String greet() { return name; }
来源：http://xqh.jinqigfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wue.jiagoushi.top

Ruby: def greet; @name; end
来源：http://ick.sufxvd.cn

C#:   public string Greet() => Name;
来源：http://ynp.fzhhl.top

[G05] 继承
来源：http://zqs.kuanghao11.cn

Py:   class Admin(User): pass
来源：http://dkn.fehbvm.com

PHP:  class Admin extends User {}
来源：http://xxw.birdmap.top

JS:   class Admin extends User {}
来源：http://czz.guannengcc.top

TS:   class Admin extends User {}
来源：http://nls.guannengcc.top

Java: class Admin extends User {}
来源：http://ocs.xingfuxueyuan.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tsp.ydzc1.top

Ruby: class Admin < User; end
来源：http://rmf.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://bak.zhoulong.xyz

[G06] 重写方法
来源：http://ogb.hysaishi.cn

Py:   def greet(self): return "admin"
来源：http://nig.jinqigfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://iyf.birdmap.top

JS:   greet() { return "admin"; }
来源：http://wke.nwbrower.top

TS:   greet(): string { return "admin"; }
来源：http://kmt.tarul.cn

Java: @Override String greet() { return "admin"; }
来源：http://dsl.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yfw.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://hej.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://wpw.daria6918.cn

[G07] 调用父类方法
来源：http://wuo.bbcook.cn

Py:   super().greet()
来源：http://gah.zhoulong.xyz

PHP:  parent::greet();
来源：http://lnn.fehbvm.com

JS:   super.greet();
来源：http://asr.aibaodan.cn

TS:   super.greet();
来源：http://rmb.tianlin.xyz

Java: super.greet();
来源：http://yfj.dashuyun.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://teh.yvedp.cn

Ruby: super
来源：http://gjw.zhixingplan.top

C#:   base.Greet();
来源：http://pyn.zdbjq.cn

[G08] 静态方法与属性
来源：http://fmf.meibo888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hps.hnxiangtu.top

PHP:  public static function f() {}
来源：http://hei.gogol.net.cn

JS:   static f() {}
来源：http://dlp.yfazqb.com

TS:   static f(): void {}
来源：http://xtn.gogol.net.cn

Java: static void f() {}
来源：http://mdq.haohaochexian.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://uox.jiagoushi.top

Ruby: def self.f; end
来源：http://rcd.ivvv.top

C#:   public static void F() {}
来源：http://ywm.yj202588.top

[G09] 接口 / 抽象类
来源：http://xhu.c1oappe.top

Py:   from abc import ABC, abstractmethod
来源：http://ovy.sweek.top

PHP:  interface Shape { public function area(): float; }
来源：http://yfk.cucudq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jwu.yj202588.top

TS:   interface Shape { area(): number; }
来源：http://sdn.52xcode.cn

Java: interface Shape { double area(); }
来源：http://mfv.yuanzhike.top

Go:   type Shape interface { Area() float64 }
来源：http://ywr.iojbl.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yzh.ppjwa.cn

C#:   interface IShape { double Area(); }
来源：http://hty.shuidangran.top

[G10] 访问控制
来源：http://qxs.hfpthk.cn

Py:   约定 _protected / __private（不强制）
来源：http://uwo.pengpengdd.cyou

PHP:  public / protected / private
来源：http://qyz.zhongyouzk.top

JS:   #private 字段；其余公开
来源：http://uyy.daria6918.cn

TS:   public / protected / private
来源：http://grb.vehdjk.com

Java: public / protected / private / 默认包级
来源：http://qgu.uphjek.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://wnf.fzhhl.top

Ruby: public / protected / private
来源：http://dch.sweek.top

C#:   public / protected / private / internal
来源：http://ozo.redwolf501.top

[G11] getter / setter
来源：http://jlq.yongpay.top

Py:   @property 与 @x.setter
来源：http://thw.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://shn.zhijiandao.cn

JS:   get name() { return this._name; }
来源：http://ybv.shanyushiyangtech.top

TS:   get name(): string { return this._name; }
来源：http://ssb.tanke756.top

Java: public String getName() { return name; }
来源：http://myb.zhongyouzk.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://abs.chenjidiqi.icu

Ruby: attr_accessor :name
来源：http://rev.mhx1999.top

C#:   public string Name { get; set; }
来源：http://ntr.sysykeji.top

[G12] 对象转字符串
来源：http://muu.jinqigfzy.top

Py:   def __str__(self): return self.name
来源：http://ahi.yuanzhike.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kxn.hammf.cn

JS:   toString() { return this.name; }
来源：http://gvd.chenzaomai.com

TS:   toString(): string { return this.name; }
来源：http://qcb.ppjwa.cn

Java: @Override public String toString() { return name; }
来源：http://hyy.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://was.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://mzg.birdmap.top

C#:   public override string ToString() => Name;
来源：http://jid.ybcxt.top

[G13] 判断对象类型
来源：http://yan.svipenyu.cn

Py:   isinstance(u, User)
来源：http://wkl.bbcook.cn

PHP:  $u instanceof User
来源：http://mcf.tarul.cn

JS:   u instanceof User
来源：http://cwq.havefunace.top

TS:   u instanceof User
来源：http://fzd.xuetiantiany.cn

Java: u instanceof User
来源：http://vio.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zdu.bbcook.cn

Ruby: u.is_a?(User)
来源：http://jjl.yj202588.top

C#:   u is User
来源：http://bjm.wangshuangyany.cn

[G14] 数据类 / record
来源：http://hnt.chenjidiqi.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://emz.havefunace.top

PHP:  // 用 readonly 属性模拟
来源：http://fzg.daxiang520.top

JS:   // 无内置：普通类或对象字面量
来源：http://uxb.gaohongyu789.top

TS:   type User = { name: string; age: number };
来源：http://lse.cucudq.cn

Java: record User(String name, int age) {}
来源：http://ytw.yueranfly.top

Go:   type User struct { Name string; Age int }
来源：http://aay.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yjz.shangyingyoupin.top

C#:   record User(string Name, int Age);
来源：http://ajx.ywan-chungtsiang.top

[G15] 枚举
来源：http://plx.zhaomingkeji.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gwg.xziqi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rih.pycfn.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bal.zhongyouzk.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://whp.ydjk.org.cn

Java: enum Color { RED, GREEN }
来源：http://lzf.dashuyun.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mrn.yuanzhike.top

Ruby: Color = %i[red green].freeze
来源：http://kya.zdqjudy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mlp.ehwqpu.com

[G16] 对象转数组 / 字典
来源：http://isu.ctjpmb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yrn.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://fbw.jiagoushi.top

JS:   Object.entries(obj)
来源：http://pav.fzhhl.top

TS:   Object.entries(obj)
来源：http://ite.pycfn.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wbg.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qoy.ydzc1.top

Ruby: obj.instance_variables
来源：http://lyw.jiagoushi.top

C#:   // 用反射或 System.Text.Json
来源：http://ijw.yuanzhike.top

================================================================================
来源：http://srt.ivvv.top

H. 异常与错误处理
来源：http://yzl.xinyue.icu

================================================================================
来源：http://pfw.daria6918.cn

[H01] try / catch 基础
来源：http://nkd.gogol.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bwu.iojbl.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fxk.nwbrower.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://obm.fktsv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tfe.hywenlv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://byc.sjlbkw.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sgb.tanke756.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lwv.fengsongda.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://huu.vqdsnc.cn

[H02] finally / ensure 收尾
来源：http://gqk.uphjek.com

Py:   try: f()⏎finally: cleanup()
来源：http://fqr.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://kum.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://taj.bjfxy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://den.jqgfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://xix.xinyue.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://dle.hongshengwenyu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fmk.haohaochexian.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gag.hnqzz.top

[H03] 主动抛出异常
来源：http://kzu.zdqjudy.top

Py:   raise ValueError("错误信息")
来源：http://jxd.ybcxt.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://npu.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://btu.yvedp.cn

TS:   throw new Error("错误信息");
来源：http://myh.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ral.jlsjyb.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lhk.9152youxi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gdc.vqdsnc.cn

C#:   throw new ArgumentException("错误信息");
来源：http://feb.yj20258.top

[H04] 自定义异常类型
来源：http://ytc.sweek.top

Py:   class MyError(Exception): pass
来源：http://duj.hnxiangtu.top

PHP:  class MyError extends RuntimeException {}
来源：http://lje.aibaodan.cn

JS:   class MyError extends Error {}
来源：http://psf.jqgufenzy.top

TS:   class MyError extends Error {}
来源：http://xrc.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://kos.ehwqpu.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qpb.aibaodan.cn

Ruby: class MyError < StandardError; end
来源：http://gby.jyoumei.cn

C#:   class MyException : Exception {}
来源：http://zov.zdqjudy.top

[H05] 捕获特定类型
来源：http://vgf.xuanzx.com

Py:   except ValueError as e:
来源：http://wtj.zhengqikj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nde.yongpay.top

JS:   if (e instanceof TypeError) {}
来源：http://fzt.hysaishi.cn

TS:   if (e instanceof TypeError) {}
来源：http://nhv.chenzaomai.com

Java: catch (IOException | SQLException e) {}
来源：http://jds.yvedp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://juq.ydjk.org.cn

Ruby: rescue ArgumentError => e
来源：http://rqi.jyoumei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zjv.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://fqf.hesvh.cn

Py:   value = d.get("k") or default
来源：http://dls.fzhhl.top

PHP:  $v = $d["k"] ?? null;
来源：http://upq.cqqwz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://txm.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://jet.hesvh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ogw.yongpay.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ryc.xziqi.cn

Ruby: d&.dig(:a, :b)
来源：http://byl.hnqzz.top

C#:   obj?.A?.B ?? default
来源：http://wju.havefunace.top

[H07] 断言
来源：http://gyw.jinqigfzy.top

Py:   assert x > 0, "必须为正"
来源：http://acs.aizwys.cn

PHP:  assert($x > 0);
来源：http://frx.yonumen.top

JS:   console.assert(x > 0);
来源：http://mlc.wangshuangyany.cn

TS:   console.assert(x > 0);
来源：http://uhh.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://bjv.fzhhl.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yjd.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://bwb.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://uul.zycfv.cn

[H08] 获取错误信息与堆栈
来源：http://rbc.vehdjk.com

Py:   str(e);  traceback.format_exc()
来源：http://oko.pycfn.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ytu.svipenyu.cn

JS:   e.message;  e.stack
来源：http://bcf.sweek.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://eem.ctjpmb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://brm.chenzaomai.com

Go:   err.Error()
来源：http://xge.aizwys.cn

Ruby: e.message;  e.backtrace
来源：http://biu.yangfankeji.com

C#:   e.Message;  e.StackTrace
来源：http://mga.jinghuilouyu.cn

[H09] 带错误码的异常
来源：http://ike.cdnleiting.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://twi.tanke756.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qyz.jinyuanbaomall.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jpx.ybcxt.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vmb.jinyuanbaomall.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hcz.ppjwa.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vyj.cheryme.top

Ruby: raise MyError.new("fail", 500)
来源：http://uui.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uja.hywenlv.cn

[H10] 资源自动释放
来源：http://auh.zdqjudy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wqs.yj202588.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://odp.birdmap.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kfa.yj202588.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uzl.yueranfly.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bnc.andypj.xyz

Go:   defer f.Close()
来源：http://vfv.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://paq.shzxlz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://twc.wangshuangyany.cn

================================================================================
来源：http://wii.tanke756.top

I. 正则表达式
来源：http://sqc.hysaishi.cn

================================================================================
来源：http://fms.316326.xyz

[I01] 判断是否匹配
来源：http://wpi.yangfankeji.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vft.yueranfly.top

PHP:  preg_match('/\d+/', $s);
来源：http://htg.shuidangran.top

JS:   /\d+/.test(s)
来源：http://cuh.zhongyouzk.top

TS:   /\d+/.test(s)
来源：http://fbl.quarkkingdee.top


<!-- 参考信息 -->