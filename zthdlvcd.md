代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://peq.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zdf.xingfuxueyuan.xyz

JS:   fs.readdirSync("dir")
来源：http://xhu.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://koa.jinqigufen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nxb.cucudq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ooi.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://qqf.sweek.top

C#:   Directory.GetFiles("dir")
来源：http://hrn.fengsongda.top

[F09] 获取文件大小
来源：http://qns.zdbjq.cn

Py:   os.path.getsize("a.txt")
来源：http://mfk.cucudq.cn

PHP:  filesize("a.txt");
来源：http://jxt.ivvv.top

JS:   fs.statSync("a.txt").size
来源：http://tvw.aizwys.cn

TS:   fs.statSync("a.txt").size
来源：http://ggl.fzhhl.top

Java: Files.size(Path.of("a.txt"))
来源：http://lgc.shangyingyoupin.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vqi.birdmap.top

Ruby: File.size("a.txt")
来源：http://kwp.andypj.xyz

C#:   new FileInfo("a.txt").Length
来源：http://zmt.c1oappe.top

[F10] 取文件扩展名 / 文件名
来源：http://njl.yanxiufei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mzs.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yna.zhiwuduotai.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oyl.sufxvd.cn

TS:   path.extname("a.txt")
来源：http://wcz.gogol.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pqp.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xdm.yj20258.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wio.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jwq.0kj1m.cn

[F11] 复制与移动文件
来源：http://sga.epnwcf.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rsl.c1oappe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jfb.jqgufenzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tjr.zdqjudy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qgu.nanxuanxn.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hta.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ljc.yvedp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mbr.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ygd.aizwys.cn

[F12] CSV 读写
来源：http://wks.cheryme.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://agx.xuanzx.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rbb.cashguo.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ggx.ydzc1.top

TS:   // 同上
来源：http://cmp.yueranfly.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lfe.hcnkem.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mmr.jqgfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vid.nanxinkj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hop.birdmap.top

================================================================================
来源：http://ead.aibaodan.cn

G. 面向对象
来源：http://ymt.hysaishi.cn

================================================================================
来源：http://fhs.yuxming.cn

[G01] 定义类
来源：http://oqp.ydjk.org.cn

Py:   class User: pass
来源：http://mkj.yanxiufei.cn

PHP:  class User {}
来源：http://ajy.zhixingplan.top

JS:   class User {}
来源：http://csg.bjfxy.top

TS:   class User { name: string = ""; }
来源：http://sod.yfazqb.com

Java: class User {}
来源：http://rln.yongpay.top

Go:   type User struct { Name string }
来源：http://klp.guowangkeji.top

Ruby: class User; end
来源：http://zli.zhongyouzk.top

C#:   class User {}
来源：http://utv.hywenlv.cn

[G02] 构造函数
来源：http://ant.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://uqn.pengpengdd.cyou

PHP:  public function __construct(public string $name) {}
来源：http://jmm.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://qgc.yj202588.top

TS:   constructor(public name: string) {}
来源：http://fvt.aizwys.cn

Java: User(String name) { this.name = name; }
来源：http://lcw.zhengqikj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rtb.ctjpmb.com

Ruby: def initialize(name); @name = name; end
来源：http://tfj.hammf.cn

C#:   public User(string name) { Name = name; }
来源：http://ddd.xuetiantiany.cn

[G03] 实例属性
来源：http://fwm.jinyuanbaomall.cn

Py:   self.name = "x"
来源：http://cpw.shanyushiyangkeji.top

PHP:  public string $name = "x";
来源：http://rux.cheryme.top

JS:   this.name = "x";
来源：http://glw.316326.xyz

TS:   name: string = "x";
来源：http://dho.iojbl.cn

Java: private String name;
来源：http://kps.yj20258888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nft.zycfv.cn

Ruby: @name = "x"
来源：http://rri.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://tnv.hnqzz.top

[G04] 定义方法
来源：http://tsv.fehbvm.com

Py:   def greet(self): return self.name
来源：http://qgy.yanxiufei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://brp.zycfv.cn

JS:   greet() { return this.name; }
来源：http://lmw.52xcode.cn

TS:   greet(): string { return this.name; }
来源：http://jlc.tianlin.xyz

Java: String greet() { return name; }
来源：http://skp.fzhhl.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://aae.birdmap.top

Ruby: def greet; @name; end
来源：http://yri.shangyingyoupin.top

C#:   public string Greet() => Name;
来源：http://qwp.fzhhl.top

[G05] 继承
来源：http://ayu.fengsongda.top

Py:   class Admin(User): pass
来源：http://owt.fehbvm.com

PHP:  class Admin extends User {}
来源：http://xhx.fengsongda.top

JS:   class Admin extends User {}
来源：http://inq.shuidangran.top

TS:   class Admin extends User {}
来源：http://cgp.gogol.net.cn

Java: class Admin extends User {}
来源：http://lvi.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hhy.ybcxt.top

Ruby: class Admin < User; end
来源：http://ify.52xcode.cn

C#:   class Admin : User {}
来源：http://gej.feifeiyinyue.top

[G06] 重写方法
来源：http://sih.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://akm.pengpengdd.cyou

PHP:  public function greet(): string { return "admin"; }
来源：http://mol.xingfuxueyuan.xyz

JS:   greet() { return "admin"; }
来源：http://tmu.svipenyu.cn

TS:   greet(): string { return "admin"; }
来源：http://tkj.nwbrower.top

Java: @Override String greet() { return "admin"; }
来源：http://sjj.xuetiantiany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uqm.zhixingplan.top

Ruby: def greet; "admin"; end
来源：http://zkz.hcnkem.com

C#:   public override string Greet() => "admin";
来源：http://iie.bbcook.cn

[G07] 调用父类方法
来源：http://nbi.yonumen.top

Py:   super().greet()
来源：http://wgc.daria6918.cn

PHP:  parent::greet();
来源：http://yqa.sysykeji.top

JS:   super.greet();
来源：http://rla.yvedp.cn

TS:   super.greet();
来源：http://cye.haohaochexian.top

Java: super.greet();
来源：http://dua.ybcxt.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pqf.andypj.xyz

Ruby: super
来源：http://xvc.shanyushiyangtech.top

C#:   base.Greet();
来源：http://dnp.guannengcc.top

[G08] 静态方法与属性
来源：http://dgv.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fzp.wangdashe.top

PHP:  public static function f() {}
来源：http://yjm.cucudq.cn

JS:   static f() {}
来源：http://ozk.tianlin.xyz

TS:   static f(): void {}
来源：http://unq.epnwcf.com

Java: static void f() {}
来源：http://qvx.jlsjyb.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://erm.jqgfzy.top

Ruby: def self.f; end
来源：http://pwb.tianlin.xyz

C#:   public static void F() {}
来源：http://vak.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://kkx.c1oappe.top

Py:   from abc import ABC, abstractmethod
来源：http://eji.bjfxy.top

PHP:  interface Shape { public function area(): float; }
来源：http://sev.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://nsk.jianghu66.top

TS:   interface Shape { area(): number; }
来源：http://mck.nwbrower.top

Java: interface Shape { double area(); }
来源：http://tpu.uphjek.com

Go:   type Shape interface { Area() float64 }
来源：http://avp.9152youxi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rxn.jinghuilouyu.cn

C#:   interface IShape { double Area(); }
来源：http://qka.yonumen.top

[G10] 访问控制
来源：http://gbr.zhixingplan.top

Py:   约定 _protected / __private（不强制）
来源：http://ioj.cheryme.top

PHP:  public / protected / private
来源：http://hhd.birdmap.top

JS:   #private 字段；其余公开
来源：http://pqo.jqgfzy.top

TS:   public / protected / private
来源：http://dsu.ivvv.top

Java: public / protected / private / 默认包级
来源：http://woy.gotoacloud.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gks.feifeiyinyue.top

Ruby: public / protected / private
来源：http://kfg.yj20258.top

C#:   public / protected / private / internal
来源：http://rtv.fehbvm.com

[G11] getter / setter
来源：http://whg.jinqigfzy.top

Py:   @property 与 @x.setter
来源：http://gbu.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://jfc.zycfv.cn

JS:   get name() { return this._name; }
来源：http://ccx.xylfe.cn

TS:   get name(): string { return this._name; }
来源：http://enx.ehwqpu.com

Java: public String getName() { return name; }
来源：http://qhs.yuxming.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ysh.yj20258888.top

Ruby: attr_accessor :name
来源：http://qxo.meibo888.top

C#:   public string Name { get; set; }
来源：http://ucg.kuanghao11.cn

[G12] 对象转字符串
来源：http://xky.jyoumei.cn

Py:   def __str__(self): return self.name
来源：http://thn.aibaodan.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qsc.meibo888.top

JS:   toString() { return this.name; }
来源：http://guo.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://cqo.vehdjk.com

Java: @Override public String toString() { return name; }
来源：http://wuv.shuidangran.top

Go:   func (u User) String() string { return u.Name }
来源：http://ons.hammf.cn

Ruby: def to_s; @name; end
来源：http://fhb.fengsongda.top

C#:   public override string ToString() => Name;
来源：http://tiv.zhaomingkeji.xyz

[G13] 判断对象类型
来源：http://uar.zhixingplan.top

Py:   isinstance(u, User)
来源：http://ghd.zdbjq.cn

PHP:  $u instanceof User
来源：http://qwg.ybcxt.top

JS:   u instanceof User
来源：http://pzg.pycfn.com

TS:   u instanceof User
来源：http://inp.daria6918.cn

Java: u instanceof User
来源：http://hnp.jqgfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lms.andypj.xyz

Ruby: u.is_a?(User)
来源：http://lny.redwolf501.top

C#:   u is User
来源：http://ykv.tanke756.top

[G14] 数据类 / record
来源：http://fgu.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lhy.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://pzo.xinyue.icu

JS:   // 无内置：普通类或对象字面量
来源：http://xaf.ybcxt.top

TS:   type User = { name: string; age: number };
来源：http://hhg.yongpay.top

Java: record User(String name, int age) {}
来源：http://fhk.ppjwa.cn

Go:   type User struct { Name string; Age int }
来源：http://cjg.guowangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uku.ehwqpu.com

C#:   record User(string Name, int Age);
来源：http://ssi.hesvh.cn

[G15] 枚举
来源：http://vll.zdqjudy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vpn.zdqjudy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bcl.ywan-chungtsiang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ibx.jlsjyb.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ybf.hnqzz.top

Java: enum Color { RED, GREEN }
来源：http://gvu.yfazqb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bxl.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://qfm.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ufn.birdmap.top

[G16] 对象转数组 / 字典
来源：http://ckn.smart0.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nof.fzhhl.top

PHP:  get_object_vars($obj);
来源：http://iij.fengsongda.top

JS:   Object.entries(obj)
来源：http://oyy.hnxiangtu.top

TS:   Object.entries(obj)
来源：http://eyk.316326.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://art.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jfj.jiagoushi.top

Ruby: obj.instance_variables
来源：http://kud.hammf.cn

C#:   // 用反射或 System.Text.Json
来源：http://kce.shzxlz.cn

================================================================================
来源：http://yur.gogol.net.cn

H. 异常与错误处理
来源：http://qby.xziqi.cn

================================================================================
来源：http://kux.fanxiaobao.xyz

[H01] try / catch 基础
来源：http://aqu.yueranfly.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://abp.cashguo.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dzk.xuetiantiany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tkr.cucudq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vdf.cheryme.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bmg.fanxiaobao.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://afa.52xcode.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sap.fktsv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tbo.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://omc.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://mwb.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://haj.tian-w.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cjx.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://drl.zhiwuduotai.top

Java: try { f(); } finally { cleanup(); }
来源：http://xdz.zhiwuduotai.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://yre.chenlongwang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wmd.jyoumei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ctv.daxiang520.top

[H03] 主动抛出异常
来源：http://tga.jqgfzy.top

Py:   raise ValueError("错误信息")
来源：http://nov.jyoumei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wgr.hfpthk.cn

JS:   throw new Error("错误信息");
来源：http://zfx.zhaomingkeji.xyz

TS:   throw new Error("错误信息");
来源：http://lms.jqgufenzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kfh.havefunace.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oyl.shangyingyoupin.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xxj.fehbvm.com

C#:   throw new ArgumentException("错误信息");
来源：http://ghx.havefunace.top

[H04] 自定义异常类型
来源：http://guq.gaohongyu789.top

Py:   class MyError(Exception): pass
来源：http://qpk.cashguo.top

PHP:  class MyError extends RuntimeException {}
来源：http://bab.sjlbkw.cn

JS:   class MyError extends Error {}
来源：http://aty.zhixingplan.top

TS:   class MyError extends Error {}
来源：http://wtc.sweek.top

Java: class MyException extends RuntimeException {}
来源：http://kdt.bbcook.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dix.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://yen.cdnleiting.top

C#:   class MyException : Exception {}
来源：http://uil.gzhubu.top

[H05] 捕获特定类型
来源：http://pmn.dianchejie.cn

Py:   except ValueError as e:
来源：http://glw.cqqwz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dnq.pycfn.com

JS:   if (e instanceof TypeError) {}
来源：http://fdv.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://wqk.pycfn.com

Java: catch (IOException | SQLException e) {}
来源：http://amv.zhijiandao.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://igf.yangfankeji.com

Ruby: rescue ArgumentError => e
来源：http://cbn.yj202588.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uce.sxryk.cn

[H06] 可选值 / 空值安全访问
来源：http://jda.guannengcc.top

Py:   value = d.get("k") or default
来源：http://vro.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://zxs.svipenyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nyv.gogol.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jnm.epnwcf.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lrg.hongshengwenyu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bfb.0kj1m.cn

Ruby: d&.dig(:a, :b)
来源：http://ais.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://vij.jlsjyb.cn

[H07] 断言
来源：http://itt.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://uzq.316326.xyz

PHP:  assert($x > 0);
来源：http://kcq.yvedp.cn

JS:   console.assert(x > 0);
来源：http://rfp.meibo888.top

TS:   console.assert(x > 0);
来源：http://uou.yvedp.cn

Java: assert x > 0 : "必须为正";
来源：http://gha.zdbjq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jwt.yangfankeji.com

Ruby: raise "必须为正" unless x > 0
来源：http://oxi.yueranfly.top

C#:   Debug.Assert(x > 0);
来源：http://laj.xingfuxueyuan.xyz

[H08] 获取错误信息与堆栈
来源：http://vfc.ydjk.org.cn

Py:   str(e);  traceback.format_exc()
来源：http://tkg.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nvh.ydzc1.top

JS:   e.message;  e.stack
来源：http://czj.yuanzhike.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nyc.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xfr.cheryme.top

Go:   err.Error()
来源：http://tyb.pengpengdd.cyou

Ruby: e.message;  e.backtrace
来源：http://mbi.xylfe.cn

C#:   e.Message;  e.StackTrace
来源：http://mfy.sweek.top

[H09] 带错误码的异常
来源：http://lzl.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lxl.fanxiaobao.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://gga.xuetiantiany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xwj.havefunace.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nka.svipenyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dyc.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fpw.zhongyouzk.top

Ruby: raise MyError.new("fail", 500)
来源：http://tso.xziqi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iij.ydjk.org.cn

[H10] 资源自动释放
来源：http://jdm.guowangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ler.uphjek.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nsr.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iof.zdbjq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kte.fzhhl.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hrz.hammf.cn

Go:   defer f.Close()
来源：http://frs.yonumen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://frk.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cyx.gotoacloud.top

================================================================================
来源：http://yze.yangfankeji.com

I. 正则表达式
来源：http://spm.zhijiandao.cn

================================================================================
来源：http://hjc.wangshuangyany.cn

[I01] 判断是否匹配
来源：http://vsa.ydzc1.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ycj.tian-w.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vrm.quarkkingdee.top

JS:   /\d+/.test(s)
来源：http://hvj.ppjwa.cn

TS:   /\d+/.test(s)
来源：http://lqr.zhengqikj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://trc.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zsf.guowangkeji.top

Ruby: s.match?(/\d+/)
来源：http://cjv.yj20258.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zbr.0kj1m.cn

[I02] 提取所有匹配
来源：http://rbd.epnwcf.com

Py:   re.findall(r"\d+", s)
来源：http://cpv.sufxvd.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://myy.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ayc.sysykeji.top


<!-- 参考信息 -->