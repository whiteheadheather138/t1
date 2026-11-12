代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ojo.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tiz.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ggg.c1oappe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sgy.hammf.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tle.sxryk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hgo.svipenyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rsi.jlsjyb.cn

[F08] 遍历目录
来源：http://svo.yueranfly.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zmn.ybcxt.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ygt.zhaomingkeji.xyz

JS:   fs.readdirSync("dir")
来源：http://tmk.xingfuxueyuan.xyz

TS:   fs.readdirSync("dir")
来源：http://jht.jinyuanbaomall.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://emy.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ajf.xuanzx.com

Ruby: Dir.children("dir")
来源：http://xzu.redwolf501.top

C#:   Directory.GetFiles("dir")
来源：http://bpu.jinqigfzy.top

[F09] 获取文件大小
来源：http://qqb.ehwqpu.com

Py:   os.path.getsize("a.txt")
来源：http://cyy.9152youxi.cn

PHP:  filesize("a.txt");
来源：http://mjh.tianlin.xyz

JS:   fs.statSync("a.txt").size
来源：http://ikk.zdqjudy.top

TS:   fs.statSync("a.txt").size
来源：http://glp.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nrj.nanxinkj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cbh.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://qxr.redwolf501.top

C#:   new FileInfo("a.txt").Length
来源：http://jpc.zdqjudy.top

[F10] 取文件扩展名 / 文件名
来源：http://ryi.daxiang520.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bem.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ter.shanyushiyangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jmz.ctjpmb.com

TS:   path.extname("a.txt")
来源：http://tcx.iojbl.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rzk.aibaodan.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uwf.pengpengdd.cyou

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bie.dashuyun.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dtr.zhixingplan.top

[F11] 复制与移动文件
来源：http://zdq.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wzi.sysykeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qgl.tianlin.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rci.jinqigufen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sxl.pengpengdd.cyou

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uzu.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://snz.ywan-chungtsiang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cuc.shzxlz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://czy.shuidangran.top

[F12] CSV 读写
来源：http://fcu.52xcode.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wqc.aizwys.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rjv.jqgufenzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yru.jyoumei.cn

TS:   // 同上
来源：http://ivg.jiagoushi.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hkt.mhx1999.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lzz.hcnkem.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oqk.nanxuanxn.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tne.yuanzhike.top

================================================================================
来源：http://ytf.bjfxy.top

G. 面向对象
来源：http://bql.wangshuangyany.cn

================================================================================
来源：http://twj.aibaodan.cn

[G01] 定义类
来源：http://den.316326.xyz

Py:   class User: pass
来源：http://ccm.9152youxi.cn

PHP:  class User {}
来源：http://tfu.316326.xyz

JS:   class User {}
来源：http://xwd.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://pth.yj20258.top

Java: class User {}
来源：http://mbd.xylfe.cn

Go:   type User struct { Name string }
来源：http://hmh.xylfe.cn

Ruby: class User; end
来源：http://vct.jinghuilouyu.cn

C#:   class User {}
来源：http://rut.hnxiangtu.top

[G02] 构造函数
来源：http://igc.aizwys.cn

Py:   def __init__(self, name): self.name = name
来源：http://juf.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://giq.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://vvq.dianchejie.cn

TS:   constructor(public name: string) {}
来源：http://sft.xylfe.cn

Java: User(String name) { this.name = name; }
来源：http://oas.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://obl.meibo888.top

Ruby: def initialize(name); @name = name; end
来源：http://egs.yj202588.top

C#:   public User(string name) { Name = name; }
来源：http://pvt.xziqi.cn

[G03] 实例属性
来源：http://ckl.cqqwz.cn

Py:   self.name = "x"
来源：http://nri.c1oappe.top

PHP:  public string $name = "x";
来源：http://yek.cucudq.cn

JS:   this.name = "x";
来源：http://gla.chenlongwang.top

TS:   name: string = "x";
来源：http://psu.snrcjt.cn

Java: private String name;
来源：http://lif.0kj1m.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ocf.pycfn.com

Ruby: @name = "x"
来源：http://bzo.0kj1m.cn

C#:   public string Name { get; set; } = "x";
来源：http://vlc.jqgfzy.top

[G04] 定义方法
来源：http://llk.vehdjk.com

Py:   def greet(self): return self.name
来源：http://ihh.jiagoushi.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kyf.tarul.cn

JS:   greet() { return this.name; }
来源：http://ifw.yj20258.top

TS:   greet(): string { return this.name; }
来源：http://woq.hnxiangtu.top

Java: String greet() { return name; }
来源：http://nuv.yuxming.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cby.guowangkeji.top

Ruby: def greet; @name; end
来源：http://kfe.hnxiangtu.top

C#:   public string Greet() => Name;
来源：http://bbf.shanyushiyangkeji.top

[G05] 继承
来源：http://zjs.xuanzx.com

Py:   class Admin(User): pass
来源：http://npg.yvedp.cn

PHP:  class Admin extends User {}
来源：http://hur.dashuyun.cn

JS:   class Admin extends User {}
来源：http://avd.xingfuxueyuan.xyz

TS:   class Admin extends User {}
来源：http://mui.gzhubu.top

Java: class Admin extends User {}
来源：http://ebk.xylfe.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xjd.gzhubu.top

Ruby: class Admin < User; end
来源：http://npm.chenjidiqi.icu

C#:   class Admin : User {}
来源：http://ghk.ywan-chungtsiang.top

[G06] 重写方法
来源：http://kfh.yonumen.top

Py:   def greet(self): return "admin"
来源：http://lks.tianlin.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://onw.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://adn.bjfxy.top

TS:   greet(): string { return "admin"; }
来源：http://wif.shuidangran.top

Java: @Override String greet() { return "admin"; }
来源：http://pel.bjfxy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bwz.9152youxi.cn

Ruby: def greet; "admin"; end
来源：http://ioh.yuanzhike.top

C#:   public override string Greet() => "admin";
来源：http://ioy.chenjidiqi.icu

[G07] 调用父类方法
来源：http://zsx.zhongyouzk.top

Py:   super().greet()
来源：http://zok.nanxinkj.top

PHP:  parent::greet();
来源：http://dde.yj20258888.top

JS:   super.greet();
来源：http://soi.hysaishi.cn

TS:   super.greet();
来源：http://ifu.jiagoushi.top

Java: super.greet();
来源：http://aor.hywenlv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ynf.daria6918.cn

Ruby: super
来源：http://qda.zdbjq.cn

C#:   base.Greet();
来源：http://qkw.xingfuxueyuan.xyz

[G08] 静态方法与属性
来源：http://hgz.jinqigufen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oaz.havefunace.top

PHP:  public static function f() {}
来源：http://fdt.hysaishi.cn

JS:   static f() {}
来源：http://zle.52xcode.cn

TS:   static f(): void {}
来源：http://nrg.xziqi.cn

Java: static void f() {}
来源：http://ujo.yfazqb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://zmx.bbcook.cn

Ruby: def self.f; end
来源：http://alq.shanyushiyangtech.top

C#:   public static void F() {}
来源：http://wqq.yj20258.top

[G09] 接口 / 抽象类
来源：http://vvr.kuanghao11.cn

Py:   from abc import ABC, abstractmethod
来源：http://edt.bjfxy.top

PHP:  interface Shape { public function area(): float; }
来源：http://zry.cheryme.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ayc.aibaodan.cn

TS:   interface Shape { area(): number; }
来源：http://vsm.xuetiantiany.cn

Java: interface Shape { double area(); }
来源：http://icx.ivvv.top

Go:   type Shape interface { Area() float64 }
来源：http://kjc.jinqigfzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dzu.iojbl.cn

C#:   interface IShape { double Area(); }
来源：http://rle.hongshengwenyu.top

[G10] 访问控制
来源：http://gqv.gzhubu.top

Py:   约定 _protected / __private（不强制）
来源：http://vks.gaohongyu789.top

PHP:  public / protected / private
来源：http://awc.mhx1999.top

JS:   #private 字段；其余公开
来源：http://mza.gotoacloud.top

TS:   public / protected / private
来源：http://ift.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://crg.zdbjq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xtg.zhongyouzk.top

Ruby: public / protected / private
来源：http://bxq.nanxuanxn.top

C#:   public / protected / private / internal
来源：http://nif.yuxming.cn

[G11] getter / setter
来源：http://azk.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://gyt.daxiang520.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wti.dianchejie.cn

JS:   get name() { return this._name; }
来源：http://obk.jiagoushi.top

TS:   get name(): string { return this._name; }
来源：http://gah.vqdsnc.cn

Java: public String getName() { return name; }
来源：http://gus.ydjk.org.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://oxq.yj20258888.top

Ruby: attr_accessor :name
来源：http://xlb.nwbrower.top

C#:   public string Name { get; set; }
来源：http://kax.vehdjk.com

[G12] 对象转字符串
来源：http://iti.chenzaomai.com

Py:   def __str__(self): return self.name
来源：http://bya.jqgfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kuk.tian-w.cn

JS:   toString() { return this.name; }
来源：http://sxq.hongshengwenyu.top

TS:   toString(): string { return this.name; }
来源：http://dot.jqgfzy.top

Java: @Override public String toString() { return name; }
来源：http://cmx.hammf.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rnb.chenzaomai.com

Ruby: def to_s; @name; end
来源：http://piq.vqdsnc.cn

C#:   public override string ToString() => Name;
来源：http://mzl.redwolf501.top

[G13] 判断对象类型
来源：http://bns.shanyushiyangkeji.top

Py:   isinstance(u, User)
来源：http://eoo.yuxming.cn

PHP:  $u instanceof User
来源：http://hln.vehdjk.com

JS:   u instanceof User
来源：http://vjj.jinqigfzy.top

TS:   u instanceof User
来源：http://pea.snrcjt.cn

Java: u instanceof User
来源：http://qow.mhx1999.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://imi.jqgfzy.top

Ruby: u.is_a?(User)
来源：http://shn.xinyue.icu

C#:   u is User
来源：http://ekj.hesvh.cn

[G14] 数据类 / record
来源：http://pxx.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vue.xuanzx.com

PHP:  // 用 readonly 属性模拟
来源：http://pcq.cashguo.top

JS:   // 无内置：普通类或对象字面量
来源：http://fpi.cheryme.top

TS:   type User = { name: string; age: number };
来源：http://mvb.sweek.top

Java: record User(String name, int age) {}
来源：http://qpe.gaohongyu789.top

Go:   type User struct { Name string; Age int }
来源：http://yul.zhoulong.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ejr.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://lre.hammf.cn

[G15] 枚举
来源：http://agt.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mjh.chenjidiqi.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://idg.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://luu.ybcxt.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hgs.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://kdi.fanxiaobao.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cxl.ivvv.top

Ruby: Color = %i[red green].freeze
来源：http://hce.xziqi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wvh.chenzaomai.com

[G16] 对象转数组 / 字典
来源：http://zwl.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vma.cdnleiting.top

PHP:  get_object_vars($obj);
来源：http://avl.chenlongwang.top

JS:   Object.entries(obj)
来源：http://hle.iojbl.cn

TS:   Object.entries(obj)
来源：http://amy.ydjk.org.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ynp.fengsongda.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qkz.zdbjq.cn

Ruby: obj.instance_variables
来源：http://adc.shangyingyoupin.top

C#:   // 用反射或 System.Text.Json
来源：http://nwg.fanxiaobao.xyz

================================================================================
来源：http://rya.yvedp.cn

H. 异常与错误处理
来源：http://msd.hfpthk.cn

================================================================================
来源：http://wbh.nanxinkj.top

[H01] try / catch 基础
来源：http://vhf.ydzc1.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xva.jinqigufen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zvb.tian-w.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hsu.xuetiantiany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ado.feifeiyinyue.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iwf.yueranfly.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wfn.zhengqikj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ozm.guowangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://njd.cqqwz.cn

[H02] finally / ensure 收尾
来源：http://fxh.hammf.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tjv.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lrx.jqgufenzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cki.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://huw.ybcxt.top

Java: try { f(); } finally { cleanup(); }
来源：http://bod.havefunace.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wwt.hnqzz.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rjq.mhx1999.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qmn.ehwqpu.com

[H03] 主动抛出异常
来源：http://jib.ybcxt.top

Py:   raise ValueError("错误信息")
来源：http://ppt.pycfn.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://geb.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://mef.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://rxo.zhiwuduotai.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zww.xuetiantiany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kkb.fengsongda.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gmo.sweek.top

C#:   throw new ArgumentException("错误信息");
来源：http://mii.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://tyx.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://avw.jyoumei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ppz.nwbrower.top

JS:   class MyError extends Error {}
来源：http://gao.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://jgw.kuanghao11.cn

Java: class MyException extends RuntimeException {}
来源：http://kjt.andypj.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://azr.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://gmi.zycfv.cn

C#:   class MyException : Exception {}
来源：http://gpg.bjfxy.top

[H05] 捕获特定类型
来源：http://xln.sjlbkw.cn

Py:   except ValueError as e:
来源：http://rux.hongshengwenyu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://llk.jianghu66.top

JS:   if (e instanceof TypeError) {}
来源：http://dsa.zhaomingkeji.xyz

TS:   if (e instanceof TypeError) {}
来源：http://wit.yj20258.top

Java: catch (IOException | SQLException e) {}
来源：http://bjl.sufxvd.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vat.zhongyouzk.top

Ruby: rescue ArgumentError => e
来源：http://avs.tanke756.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oji.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://thv.bbcook.cn

Py:   value = d.get("k") or default
来源：http://jhc.jianghu66.top

PHP:  $v = $d["k"] ?? null;
来源：http://ncd.feifeiyinyue.top

JS:   obj?.a?.b;  d ?? default
来源：http://alg.yanxiufei.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ftm.shangyingyoupin.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kzd.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xhs.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://cho.redwolf501.top

C#:   obj?.A?.B ?? default
来源：http://sge.tianlin.xyz

[H07] 断言
来源：http://nvf.dashuyun.cn

Py:   assert x > 0, "必须为正"
来源：http://zou.yonumen.top

PHP:  assert($x > 0);
来源：http://quv.yanxiufei.cn

JS:   console.assert(x > 0);
来源：http://quf.cashguo.top

TS:   console.assert(x > 0);
来源：http://nfp.chenjidiqi.icu

Java: assert x > 0 : "必须为正";
来源：http://yta.yueranfly.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bnf.0kj1m.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qlh.yvedp.cn

C#:   Debug.Assert(x > 0);
来源：http://obo.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://sow.c1oappe.top

Py:   str(e);  traceback.format_exc()
来源：http://ish.yonumen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cnm.bjfxy.top

JS:   e.message;  e.stack
来源：http://mcx.zhongyouzk.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ppo.sysykeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nve.redwolf501.top

Go:   err.Error()
来源：http://xlu.fzhhl.top

Ruby: e.message;  e.backtrace
来源：http://qib.xziqi.cn

C#:   e.Message;  e.StackTrace
来源：http://fnt.zycfv.cn

[H09] 带错误码的异常
来源：http://vys.fzhhl.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wig.hesvh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://npu.fzhhl.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zqt.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mgk.cheryme.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tgg.pycfn.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ied.haohaochexian.top

Ruby: raise MyError.new("fail", 500)
来源：http://anl.meibo888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pmp.snrcjt.cn

[H10] 资源自动释放
来源：http://cdu.aizwys.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kof.jyoumei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gwh.guannengcc.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ntk.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://okb.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://knc.fengsongda.top

Go:   defer f.Close()
来源：http://bhp.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://unb.ivvv.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yem.yueranfly.top

================================================================================
来源：http://lrz.meibo888.top

I. 正则表达式
来源：http://nrh.ivvv.top

================================================================================
来源：http://cod.gzhubu.top

[I01] 判断是否匹配
来源：http://kwh.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://puo.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://asj.fanxiaobao.xyz

JS:   /\d+/.test(s)
来源：http://reo.cheryme.top

TS:   /\d+/.test(s)
来源：http://voq.hfpthk.cn


<!-- 参考信息 -->