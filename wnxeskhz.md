代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tdr.pengpengdd.cyou

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uyt.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iek.meibo888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wgo.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tre.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://drm.uphjek.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zop.jlsjyb.cn

[F08] 遍历目录
来源：http://ykm.wangshuangyany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://grj.redwolf501.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uwl.hongshengwenyu.top

JS:   fs.readdirSync("dir")
来源：http://dat.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://zus.hnqzz.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pnc.vqdsnc.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kqp.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://gsu.hysaishi.cn

C#:   Directory.GetFiles("dir")
来源：http://zky.bbcook.cn

[F09] 获取文件大小
来源：http://mpt.nanxinkj.top

Py:   os.path.getsize("a.txt")
来源：http://erd.xuetiantiany.cn

PHP:  filesize("a.txt");
来源：http://cim.cucudq.cn

JS:   fs.statSync("a.txt").size
来源：http://udz.meibo888.top

TS:   fs.statSync("a.txt").size
来源：http://dwn.hongshengwenyu.top

Java: Files.size(Path.of("a.txt"))
来源：http://nju.yj20258.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nwf.yfazqb.com

Ruby: File.size("a.txt")
来源：http://qed.hnqzz.top

C#:   new FileInfo("a.txt").Length
来源：http://iru.guowangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://ypb.jqgfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dzd.tanke756.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qkz.birdmap.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rgp.fehbvm.com

TS:   path.extname("a.txt")
来源：http://ure.chenjidiqi.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bfx.bbcook.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pgc.c1oappe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qei.yvedp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sxm.tanke756.top

[F11] 复制与移动文件
来源：http://uje.yj20258888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://prp.yanxiufei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wgx.hywenlv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nuj.guowangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mwc.xziqi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dif.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ypu.gaohongyu789.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yfp.meibo888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://epj.yongpay.top

[F12] CSV 读写
来源：http://dfb.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hsb.yuanzhike.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zhv.pycfn.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nuf.jlsjyb.cn

TS:   // 同上
来源：http://gvh.sjlbkw.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://htf.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kiz.fktsv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xke.yangfankeji.com

C#:   // 无内置：用 CsvHelper 库
来源：http://jok.hysaishi.cn

================================================================================
来源：http://kgn.yueranfly.top

G. 面向对象
来源：http://tjr.shangyingyoupin.top

================================================================================
来源：http://vrz.fehbvm.com

[G01] 定义类
来源：http://lse.hfpthk.cn

Py:   class User: pass
来源：http://hel.wangdashe.top

PHP:  class User {}
来源：http://tlr.nanxinkj.top

JS:   class User {}
来源：http://sok.sweek.top

TS:   class User { name: string = ""; }
来源：http://xso.redwolf501.top

Java: class User {}
来源：http://jsj.sweek.top

Go:   type User struct { Name string }
来源：http://yha.zhongyouzk.top

Ruby: class User; end
来源：http://xgp.wangdashe.top

C#:   class User {}
来源：http://agr.jinyuanbaomall.cn

[G02] 构造函数
来源：http://kgb.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://msq.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://jnm.ywan-chungtsiang.top

JS:   constructor(name) { this.name = name; }
来源：http://qpz.mhx1999.top

TS:   constructor(public name: string) {}
来源：http://cog.redwolf501.top

Java: User(String name) { this.name = name; }
来源：http://lfr.ctjpmb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://suz.havefunace.top

Ruby: def initialize(name); @name = name; end
来源：http://efq.sweek.top

C#:   public User(string name) { Name = name; }
来源：http://quv.yj202588.top

[G03] 实例属性
来源：http://zvi.cdnleiting.top

Py:   self.name = "x"
来源：http://kqs.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://une.bjfxy.top

JS:   this.name = "x";
来源：http://laj.jiagoushi.top

TS:   name: string = "x";
来源：http://pws.smart0.xyz

Java: private String name;
来源：http://clx.hnqzz.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tms.hesvh.cn

Ruby: @name = "x"
来源：http://rhw.jinqigfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://ctp.cheryme.top

[G04] 定义方法
来源：http://avt.nwbrower.top

Py:   def greet(self): return self.name
来源：http://wvx.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://irj.ivvv.top

JS:   greet() { return this.name; }
来源：http://kmk.xuanzx.com

TS:   greet(): string { return this.name; }
来源：http://znk.nanxuanxn.top

Java: String greet() { return name; }
来源：http://fhe.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://yvg.jyoumei.cn

Ruby: def greet; @name; end
来源：http://qus.zhoulong.xyz

C#:   public string Greet() => Name;
来源：http://vpe.vehdjk.com

[G05] 继承
来源：http://wwd.bjfxy.top

Py:   class Admin(User): pass
来源：http://qua.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://vbs.fzhhl.top

JS:   class Admin extends User {}
来源：http://tfg.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://hwy.ybcxt.top

Java: class Admin extends User {}
来源：http://kxl.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ddn.guowangkeji.top

Ruby: class Admin < User; end
来源：http://gli.aibaodan.cn

C#:   class Admin : User {}
来源：http://ouw.chenjidiqi.icu

[G06] 重写方法
来源：http://uad.svipenyu.cn

Py:   def greet(self): return "admin"
来源：http://bfn.yj20258888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dzc.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://xjt.chenlongwang.top

TS:   greet(): string { return "admin"; }
来源：http://eks.fktsv.cn

Java: @Override String greet() { return "admin"; }
来源：http://lgo.fanxiaobao.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yyr.jiagoushi.top

Ruby: def greet; "admin"; end
来源：http://qxg.xingfuxueyuan.xyz

C#:   public override string Greet() => "admin";
来源：http://ntv.xziqi.cn

[G07] 调用父类方法
来源：http://zyw.tianlin.xyz

Py:   super().greet()
来源：http://gxn.jlsjyb.cn

PHP:  parent::greet();
来源：http://rwv.quarkkingdee.top

JS:   super.greet();
来源：http://dpe.yuxming.cn

TS:   super.greet();
来源：http://opx.svipenyu.cn

Java: super.greet();
来源：http://wks.chenzaomai.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lxw.hnxiangtu.top

Ruby: super
来源：http://puo.hfpthk.cn

C#:   base.Greet();
来源：http://lrp.havefunace.top

[G08] 静态方法与属性
来源：http://dpu.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wdt.shanyushiyangkeji.top

PHP:  public static function f() {}
来源：http://xwj.chenjidiqi.icu

JS:   static f() {}
来源：http://myy.haohaochexian.top

TS:   static f(): void {}
来源：http://qxr.aizwys.cn

Java: static void f() {}
来源：http://unc.vqdsnc.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zaf.guowangkeji.top

Ruby: def self.f; end
来源：http://nza.bbcook.cn

C#:   public static void F() {}
来源：http://vao.xinyue.icu

[G09] 接口 / 抽象类
来源：http://ohs.uphjek.com

Py:   from abc import ABC, abstractmethod
来源：http://lwq.chenlongwang.top

PHP:  interface Shape { public function area(): float; }
来源：http://avu.gaohongyu789.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yqs.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://jzh.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://qwl.ydzc1.top

Go:   type Shape interface { Area() float64 }
来源：http://ucn.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wvi.zycfv.cn

C#:   interface IShape { double Area(); }
来源：http://plr.ppjwa.cn

[G10] 访问控制
来源：http://ddj.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://ljt.ehwqpu.com

PHP:  public / protected / private
来源：http://fot.daxiang520.top

JS:   #private 字段；其余公开
来源：http://syj.pycfn.com

TS:   public / protected / private
来源：http://isw.zhengqikj.top

Java: public / protected / private / 默认包级
来源：http://yaf.shuidangran.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://maw.hnqzz.top

Ruby: public / protected / private
来源：http://uhx.yuanzhike.top

C#:   public / protected / private / internal
来源：http://pfr.jinqigfzy.top

[G11] getter / setter
来源：http://mdf.wangdashe.top

Py:   @property 与 @x.setter
来源：http://dvp.gzhubu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://med.shanyushiyangtech.top

JS:   get name() { return this._name; }
来源：http://atl.zdqjudy.top

TS:   get name(): string { return this._name; }
来源：http://pra.yj20258888.top

Java: public String getName() { return name; }
来源：http://xta.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://iqw.havefunace.top

Ruby: attr_accessor :name
来源：http://otx.aizwys.cn

C#:   public string Name { get; set; }
来源：http://rlm.cucudq.cn

[G12] 对象转字符串
来源：http://cpv.tanke756.top

Py:   def __str__(self): return self.name
来源：http://mnw.jlsjyb.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mnk.jlsjyb.cn

JS:   toString() { return this.name; }
来源：http://kul.tian-w.cn

TS:   toString(): string { return this.name; }
来源：http://cpo.yongpay.top

Java: @Override public String toString() { return name; }
来源：http://eug.jyoumei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://poh.jianghu66.top

Ruby: def to_s; @name; end
来源：http://qbc.aibaodan.cn

C#:   public override string ToString() => Name;
来源：http://vkm.nanxuanxn.top

[G13] 判断对象类型
来源：http://any.shanyushiyangkeji.top

Py:   isinstance(u, User)
来源：http://uny.ybcxt.top

PHP:  $u instanceof User
来源：http://ima.smart0.xyz

JS:   u instanceof User
来源：http://isd.9152youxi.cn

TS:   u instanceof User
来源：http://zcc.vqdsnc.cn

Java: u instanceof User
来源：http://flu.jianghu66.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ajp.xylfe.cn

Ruby: u.is_a?(User)
来源：http://gtk.shanyushiyangkeji.top

C#:   u is User
来源：http://yuz.iojbl.cn

[G14] 数据类 / record
来源：http://ebp.yj202588.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wwf.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://vrq.fehbvm.com

JS:   // 无内置：普通类或对象字面量
来源：http://qwv.zhongyouzk.top

TS:   type User = { name: string; age: number };
来源：http://lmd.c1oappe.top

Java: record User(String name, int age) {}
来源：http://uaj.snrcjt.cn

Go:   type User struct { Name string; Age int }
来源：http://nti.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hvg.hammf.cn

C#:   record User(string Name, int Age);
来源：http://yaf.fzhhl.top

[G15] 枚举
来源：http://kvg.hfpthk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://acx.zhijiandao.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pqh.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://elf.shanyushiyangtech.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mgn.xuanzx.com

Java: enum Color { RED, GREEN }
来源：http://zks.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fwa.jinqigufen.top

Ruby: Color = %i[red green].freeze
来源：http://xbm.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zyh.jinqigfzy.top

[G16] 对象转数组 / 字典
来源：http://hbu.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vfl.chenjidiqi.icu

PHP:  get_object_vars($obj);
来源：http://jeb.pycfn.com

JS:   Object.entries(obj)
来源：http://kfr.zycfv.cn

TS:   Object.entries(obj)
来源：http://hgt.hnqzz.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gfb.jinyuanbaomall.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yer.yongpay.top

Ruby: obj.instance_variables
来源：http://ecj.zhoulong.xyz

C#:   // 用反射或 System.Text.Json
来源：http://ryi.birdmap.top

================================================================================
来源：http://hjt.daria6918.cn

H. 异常与错误处理
来源：http://iir.ppjwa.cn

================================================================================
来源：http://lyn.ctjpmb.com

[H01] try / catch 基础
来源：http://vuu.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cmk.xinyue.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://azg.ctjpmb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nps.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tvw.zdqjudy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lpr.vehdjk.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uid.yj20258888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vhc.cucudq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pyf.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://smr.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hmz.yonumen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rye.cheryme.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jwt.gzhubu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ssa.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://kaj.kuanghao11.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pdy.jlsjyb.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lwz.sufxvd.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://luy.xylfe.cn

[H03] 主动抛出异常
来源：http://rbu.yongpay.top

Py:   raise ValueError("错误信息")
来源：http://lqn.yanxiufei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pxg.feifeiyinyue.top

JS:   throw new Error("错误信息");
来源：http://sbj.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://ked.fktsv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://oac.guowangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uzh.yongpay.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rjh.xylfe.cn

C#:   throw new ArgumentException("错误信息");
来源：http://led.sxryk.cn

[H04] 自定义异常类型
来源：http://hhs.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://lmp.xingfuxueyuan.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://gyd.jyoumei.cn

JS:   class MyError extends Error {}
来源：http://tff.cashguo.top

TS:   class MyError extends Error {}
来源：http://nbg.fktsv.cn

Java: class MyException extends RuntimeException {}
来源：http://hyh.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ixj.ywan-chungtsiang.top

Ruby: class MyError < StandardError; end
来源：http://aiu.vehdjk.com

C#:   class MyException : Exception {}
来源：http://wzc.meibo888.top

[H05] 捕获特定类型
来源：http://ynd.zhiwuduotai.top

Py:   except ValueError as e:
来源：http://naz.vehdjk.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xni.epnwcf.com

JS:   if (e instanceof TypeError) {}
来源：http://omr.zdbjq.cn

TS:   if (e instanceof TypeError) {}
来源：http://yud.yfazqb.com

Java: catch (IOException | SQLException e) {}
来源：http://beg.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qju.epnwcf.com

Ruby: rescue ArgumentError => e
来源：http://een.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nlx.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://xka.ctjpmb.com

Py:   value = d.get("k") or default
来源：http://pgd.ydjk.org.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sux.svipenyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bqd.quarkkingdee.top

TS:   obj?.a?.b;  d ?? default
来源：http://qtj.yanxiufei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qby.ivvv.top

Go:   if v, ok := m["k"]; ok { }
来源：http://iov.nwbrower.top

Ruby: d&.dig(:a, :b)
来源：http://cot.9152youxi.cn

C#:   obj?.A?.B ?? default
来源：http://abj.tianlin.xyz

[H07] 断言
来源：http://qgq.cqqwz.cn

Py:   assert x > 0, "必须为正"
来源：http://eaw.snrcjt.cn

PHP:  assert($x > 0);
来源：http://vxr.aibaodan.cn

JS:   console.assert(x > 0);
来源：http://xuq.bjfxy.top

TS:   console.assert(x > 0);
来源：http://xfs.yj202588.top

Java: assert x > 0 : "必须为正";
来源：http://geo.nanxuanxn.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tib.kuanghao11.cn

Ruby: raise "必须为正" unless x > 0
来源：http://boj.dashuyun.cn

C#:   Debug.Assert(x > 0);
来源：http://dkn.shanyushiyangkeji.top

[H08] 获取错误信息与堆栈
来源：http://lux.havefunace.top

Py:   str(e);  traceback.format_exc()
来源：http://rrb.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eho.zdbjq.cn

JS:   e.message;  e.stack
来源：http://kju.jinyuanbaomall.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ihu.fktsv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xiw.jqgufenzy.top

Go:   err.Error()
来源：http://bui.xylfe.cn

Ruby: e.message;  e.backtrace
来源：http://dwb.sxryk.cn

C#:   e.Message;  e.StackTrace
来源：http://cwv.yueranfly.top

[H09] 带错误码的异常
来源：http://odh.jinqigfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kbz.hcnkem.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://jvf.yanxiufei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zjo.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ura.aibaodan.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ssh.xziqi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dmf.tianlin.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://mbx.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://vvw.zhiwuduotai.top

[H10] 资源自动释放
来源：http://mgx.havefunace.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://sim.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dur.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zps.jiagoushi.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cug.yj20258.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zrn.gogol.net.cn

Go:   defer f.Close()
来源：http://rrk.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wkr.zycfv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hld.yj20258.top

================================================================================
来源：http://pvc.hywenlv.cn

I. 正则表达式
来源：http://unx.jinqigfzy.top

================================================================================
来源：http://cyi.fktsv.cn

[I01] 判断是否匹配
来源：http://tls.c1oappe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jtj.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://svj.ybcxt.top

JS:   /\d+/.test(s)
来源：http://eel.uphjek.com

TS:   /\d+/.test(s)
来源：http://dwr.hywenlv.cn


<!-- 参考信息 -->