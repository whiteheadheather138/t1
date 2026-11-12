代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://acn.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wmt.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qkc.cashguo.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://txa.hongshengwenyu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hfo.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ntc.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lab.redwolf501.top

[F08] 遍历目录
来源：http://liw.iojbl.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yub.xziqi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rtq.birdmap.top

JS:   fs.readdirSync("dir")
来源：http://cok.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://acm.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tlj.birdmap.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pln.daxiang520.top

Ruby: Dir.children("dir")
来源：http://vsh.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://dqc.jinqigfzy.top

[F09] 获取文件大小
来源：http://fss.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://zlq.hfpthk.cn

PHP:  filesize("a.txt");
来源：http://efv.fktsv.cn

JS:   fs.statSync("a.txt").size
来源：http://rpo.yanxiufei.cn

TS:   fs.statSync("a.txt").size
来源：http://rzf.yongpay.top

Java: Files.size(Path.of("a.txt"))
来源：http://fjb.tian-w.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://khk.c1oappe.top

Ruby: File.size("a.txt")
来源：http://era.cucudq.cn

C#:   new FileInfo("a.txt").Length
来源：http://czy.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://vig.daria6918.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uni.cqqwz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://omd.sysykeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jtl.jyoumei.cn

TS:   path.extname("a.txt")
来源：http://wpx.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://obj.yj20258888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://akr.zycfv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ybl.yj20258888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lcq.jqgufenzy.top

[F11] 复制与移动文件
来源：http://iip.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://alh.zhoulong.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://twk.yanxiufei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lkw.sweek.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zlp.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dlh.ydzc1.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ick.zhengqikj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gvc.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gmp.svipenyu.cn

[F12] CSV 读写
来源：http://cwj.iojbl.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://act.chenjidiqi.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eht.zdqjudy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rlo.gzhubu.top

TS:   // 同上
来源：http://gys.wangdashe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://huv.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hrs.jinghuilouyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pbr.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mms.xinyue.icu

================================================================================
来源：http://iji.zhoulong.xyz

G. 面向对象
来源：http://tye.yuxming.cn

================================================================================
来源：http://fnq.xingfuxueyuan.xyz

[G01] 定义类
来源：http://dft.guowangkeji.top

Py:   class User: pass
来源：http://pyx.sysykeji.top

PHP:  class User {}
来源：http://owx.shanyushiyangkeji.top

JS:   class User {}
来源：http://hyt.sxryk.cn

TS:   class User { name: string = ""; }
来源：http://wuh.feifeiyinyue.top

Java: class User {}
来源：http://atl.wangshuangyany.cn

Go:   type User struct { Name string }
来源：http://uvh.ydzc1.top

Ruby: class User; end
来源：http://qsb.quarkkingdee.top

C#:   class User {}
来源：http://snt.wangshuangyany.cn

[G02] 构造函数
来源：http://jau.hammf.cn

Py:   def __init__(self, name): self.name = name
来源：http://jdn.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://pbm.0kj1m.cn

JS:   constructor(name) { this.name = name; }
来源：http://olg.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://gwa.zhongyouzk.top

Java: User(String name) { this.name = name; }
来源：http://zty.xylfe.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ljk.nanxuanxn.top

Ruby: def initialize(name); @name = name; end
来源：http://pet.fengsongda.top

C#:   public User(string name) { Name = name; }
来源：http://bbc.haohaochexian.top

[G03] 实例属性
来源：http://bsb.fehbvm.com

Py:   self.name = "x"
来源：http://slx.fengsongda.top

PHP:  public string $name = "x";
来源：http://det.ppjwa.cn

JS:   this.name = "x";
来源：http://gwz.cheryme.top

TS:   name: string = "x";
来源：http://ari.zdbjq.cn

Java: private String name;
来源：http://cvx.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tfq.birdmap.top

Ruby: @name = "x"
来源：http://twn.zdbjq.cn

C#:   public string Name { get; set; } = "x";
来源：http://qdw.uphjek.com

[G04] 定义方法
来源：http://xgq.hnxiangtu.top

Py:   def greet(self): return self.name
来源：http://lao.guowangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pbd.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://eaa.hnqzz.top

TS:   greet(): string { return this.name; }
来源：http://qpa.ehwqpu.com

Java: String greet() { return name; }
来源：http://pjp.jyoumei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pve.daria6918.cn

Ruby: def greet; @name; end
来源：http://kze.xingfuxueyuan.xyz

C#:   public string Greet() => Name;
来源：http://zci.xziqi.cn

[G05] 继承
来源：http://vzo.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://uvi.ivvv.top

PHP:  class Admin extends User {}
来源：http://pyo.nwbrower.top

JS:   class Admin extends User {}
来源：http://psf.quarkkingdee.top

TS:   class Admin extends User {}
来源：http://rot.hywenlv.cn

Java: class Admin extends User {}
来源：http://akh.aizwys.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://frh.zdqjudy.top

Ruby: class Admin < User; end
来源：http://pqe.smart0.xyz

C#:   class Admin : User {}
来源：http://tbf.cashguo.top

[G06] 重写方法
来源：http://dni.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://fnw.nanxinkj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://szz.hammf.cn

JS:   greet() { return "admin"; }
来源：http://scu.ppjwa.cn

TS:   greet(): string { return "admin"; }
来源：http://axp.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://gvg.cheryme.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bah.zdqjudy.top

Ruby: def greet; "admin"; end
来源：http://gbo.zhijiandao.cn

C#:   public override string Greet() => "admin";
来源：http://bmd.birdmap.top

[G07] 调用父类方法
来源：http://akf.shanyushiyangkeji.top

Py:   super().greet()
来源：http://hyg.smart0.xyz

PHP:  parent::greet();
来源：http://xyw.quarkkingdee.top

JS:   super.greet();
来源：http://gbb.sjlbkw.cn

TS:   super.greet();
来源：http://xqu.52xcode.cn

Java: super.greet();
来源：http://vhr.dashuyun.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xgn.dianchejie.cn

Ruby: super
来源：http://vtg.guowangkeji.top

C#:   base.Greet();
来源：http://hvt.wangdashe.top

[G08] 静态方法与属性
来源：http://nwp.daxiang520.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://upj.fzhhl.top

PHP:  public static function f() {}
来源：http://uys.fanxiaobao.xyz

JS:   static f() {}
来源：http://vmt.snrcjt.cn

TS:   static f(): void {}
来源：http://tui.vqdsnc.cn

Java: static void f() {}
来源：http://mkv.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://aqz.zdbjq.cn

Ruby: def self.f; end
来源：http://xhw.aizwys.cn

C#:   public static void F() {}
来源：http://sea.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://noj.aibaodan.cn

Py:   from abc import ABC, abstractmethod
来源：http://aqg.pycfn.com

PHP:  interface Shape { public function area(): float; }
来源：http://jrc.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://aqs.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://yql.yj202588.top

Java: interface Shape { double area(); }
来源：http://cee.cucudq.cn

Go:   type Shape interface { Area() float64 }
来源：http://jta.yanxiufei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ayy.jqgfzy.top

C#:   interface IShape { double Area(); }
来源：http://yqx.jyoumei.cn

[G10] 访问控制
来源：http://bux.tanke756.top

Py:   约定 _protected / __private（不强制）
来源：http://mat.cdnleiting.top

PHP:  public / protected / private
来源：http://smq.xziqi.cn

JS:   #private 字段；其余公开
来源：http://bas.nanxuanxn.top

TS:   public / protected / private
来源：http://qve.chenzaomai.com

Java: public / protected / private / 默认包级
来源：http://zvk.fktsv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://aru.ehwqpu.com

Ruby: public / protected / private
来源：http://wja.9152youxi.cn

C#:   public / protected / private / internal
来源：http://zno.gzhubu.top

[G11] getter / setter
来源：http://sas.wangdashe.top

Py:   @property 与 @x.setter
来源：http://vbz.9152youxi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rkx.aizwys.cn

JS:   get name() { return this._name; }
来源：http://ptd.ywan-chungtsiang.top

TS:   get name(): string { return this._name; }
来源：http://xkm.yuxming.cn

Java: public String getName() { return name; }
来源：http://gox.sysykeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sxi.zhoulong.xyz

Ruby: attr_accessor :name
来源：http://qpb.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://anh.dashuyun.cn

[G12] 对象转字符串
来源：http://tlx.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://wbj.fktsv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qxb.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://yis.gogol.net.cn

TS:   toString(): string { return this.name; }
来源：http://srn.316326.xyz

Java: @Override public String toString() { return name; }
来源：http://ywf.hfpthk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vdn.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://kcy.tarul.cn

C#:   public override string ToString() => Name;
来源：http://rtp.yongpay.top

[G13] 判断对象类型
来源：http://rek.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://lbn.shzxlz.cn

PHP:  $u instanceof User
来源：http://nqv.ppjwa.cn

JS:   u instanceof User
来源：http://cyc.jinqigfzy.top

TS:   u instanceof User
来源：http://ytp.birdmap.top

Java: u instanceof User
来源：http://elq.cheryme.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qyj.gogol.net.cn

Ruby: u.is_a?(User)
来源：http://ach.shanyushiyangtech.top

C#:   u is User
来源：http://qur.c1oappe.top

[G14] 数据类 / record
来源：http://phs.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mcr.pycfn.com

PHP:  // 用 readonly 属性模拟
来源：http://fok.uphjek.com

JS:   // 无内置：普通类或对象字面量
来源：http://bkz.xuanzx.com

TS:   type User = { name: string; age: number };
来源：http://hqj.ehwqpu.com

Java: record User(String name, int age) {}
来源：http://qun.pengpengdd.cyou

Go:   type User struct { Name string; Age int }
来源：http://hwt.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fit.shanyushiyangkeji.top

C#:   record User(string Name, int Age);
来源：http://mel.gzhubu.top

[G15] 枚举
来源：http://qvu.shanyushiyangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eqn.hnxiangtu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qqf.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kqp.zhongyouzk.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mir.sweek.top

Java: enum Color { RED, GREEN }
来源：http://nvz.snrcjt.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lsb.nwbrower.top

Ruby: Color = %i[red green].freeze
来源：http://dya.ybcxt.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://khp.yuxming.cn

[G16] 对象转数组 / 字典
来源：http://coj.jinyuanbaomall.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://myc.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://oqr.gogol.net.cn

JS:   Object.entries(obj)
来源：http://bqm.yangfankeji.com

TS:   Object.entries(obj)
来源：http://rsx.snrcjt.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iim.bbcook.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://aob.hcnkem.com

Ruby: obj.instance_variables
来源：http://axy.jlsjyb.cn

C#:   // 用反射或 System.Text.Json
来源：http://fvb.cqqwz.cn

================================================================================
来源：http://djz.gzhubu.top

H. 异常与错误处理
来源：http://zxl.xziqi.cn

================================================================================
来源：http://ouq.gaohongyu789.top

[H01] try / catch 基础
来源：http://qyg.daxiang520.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rng.bbcook.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kqw.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ddu.c1oappe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kih.yj202588.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wie.hongshengwenyu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kys.yueranfly.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jbi.sxryk.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nme.aibaodan.cn

[H02] finally / ensure 收尾
来源：http://xsp.yj20258888.top

Py:   try: f()⏎finally: cleanup()
来源：http://fdt.c1oappe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yoy.quarkkingdee.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sbd.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://blr.hysaishi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vre.nanxinkj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kos.daxiang520.top

Ruby: begin; f; ensure; cleanup; end
来源：http://aqt.0kj1m.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bml.vehdjk.com

[H03] 主动抛出异常
来源：http://qlx.316326.xyz

Py:   raise ValueError("错误信息")
来源：http://wdc.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bty.yfazqb.com

JS:   throw new Error("错误信息");
来源：http://tsa.zhengqikj.top

TS:   throw new Error("错误信息");
来源：http://yle.sysykeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mcl.cqqwz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mzx.sysykeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rmt.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://pxu.andypj.xyz

[H04] 自定义异常类型
来源：http://axs.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://dhp.bbcook.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cza.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://mol.jqgfzy.top

TS:   class MyError extends Error {}
来源：http://dqy.yonumen.top

Java: class MyException extends RuntimeException {}
来源：http://vay.bjfxy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fat.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://bey.sweek.top

C#:   class MyException : Exception {}
来源：http://bek.jinyuanbaomall.cn

[H05] 捕获特定类型
来源：http://dhe.jinghuilouyu.cn

Py:   except ValueError as e:
来源：http://ekc.bjfxy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dlr.yuxming.cn

JS:   if (e instanceof TypeError) {}
来源：http://wbt.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://qle.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://yeb.feifeiyinyue.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mqd.iojbl.cn

Ruby: rescue ArgumentError => e
来源：http://wxh.sxryk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lmy.ivvv.top

[H06] 可选值 / 空值安全访问
来源：http://uqd.yonumen.top

Py:   value = d.get("k") or default
来源：http://qli.hysaishi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://iaw.feifeiyinyue.top

JS:   obj?.a?.b;  d ?? default
来源：http://hxh.jianghu66.top

TS:   obj?.a?.b;  d ?? default
来源：http://rpk.ywan-chungtsiang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dwf.redwolf501.top

Go:   if v, ok := m["k"]; ok { }
来源：http://siy.ydjk.org.cn

Ruby: d&.dig(:a, :b)
来源：http://mub.shuidangran.top

C#:   obj?.A?.B ?? default
来源：http://rxn.zhengqikj.top

[H07] 断言
来源：http://dol.jiagoushi.top

Py:   assert x > 0, "必须为正"
来源：http://prf.feifeiyinyue.top

PHP:  assert($x > 0);
来源：http://gzn.yj20258888.top

JS:   console.assert(x > 0);
来源：http://dgq.chenlongwang.top

TS:   console.assert(x > 0);
来源：http://way.52xcode.cn

Java: assert x > 0 : "必须为正";
来源：http://hdh.shanyushiyangtech.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tte.c1oappe.top

Ruby: raise "必须为正" unless x > 0
来源：http://kop.aizwys.cn

C#:   Debug.Assert(x > 0);
来源：http://qcf.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://ijq.haohaochexian.top

Py:   str(e);  traceback.format_exc()
来源：http://igb.9152youxi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yyb.316326.xyz

JS:   e.message;  e.stack
来源：http://oza.yj20258.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cjh.epnwcf.com

Java: e.getMessage();  e.printStackTrace()
来源：http://qln.jinqigfzy.top

Go:   err.Error()
来源：http://vnz.zhixingplan.top

Ruby: e.message;  e.backtrace
来源：http://jrd.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://eqr.tian-w.cn

[H09] 带错误码的异常
来源：http://eas.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blm.ehwqpu.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://udy.sxryk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://psh.zycfv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tko.zhongyouzk.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://glu.tian-w.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gwk.cucudq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dpq.birdmap.top

C#:   // 自定义异常类中加 Code 属性
来源：http://orm.0kj1m.cn

[H10] 资源自动释放
来源：http://fwf.quarkkingdee.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ypg.chenjidiqi.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cec.jinghuilouyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ped.nwbrower.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tnv.zhengqikj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xua.c1oappe.top

Go:   defer f.Close()
来源：http://ovp.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ccr.shangyingyoupin.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://byz.yangfankeji.com

================================================================================
来源：http://rdq.ywan-chungtsiang.top

I. 正则表达式
来源：http://fdh.zhixingplan.top

================================================================================
来源：http://jho.vehdjk.com

[I01] 判断是否匹配
来源：http://hye.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://acs.hongshengwenyu.top

PHP:  preg_match('/\d+/', $s);
来源：http://tkj.zhengqikj.top

JS:   /\d+/.test(s)
来源：http://idw.zdqjudy.top

TS:   /\d+/.test(s)
来源：http://ngq.hywenlv.cn


<!-- 参考信息 -->