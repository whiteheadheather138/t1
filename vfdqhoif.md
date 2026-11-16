代发 wailian999

C#:   File.Exists("a.txt")
来源：http://dfe.yongpay.top

[F06] 删除文件
来源：http://rwc.cashguo.top

Py:   os.remove("a.txt")
来源：http://jtz.fzhhl.top

PHP:  unlink("a.txt");
来源：http://nge.fktsv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hzy.kuanghao11.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cqm.cqqwz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dzz.hongshengwenyu.top

Go:   os.Remove("a.txt")
来源：http://yoj.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://aqo.wangshuangyany.cn

C#:   File.Delete("a.txt");
来源：http://ync.ywan-chungtsiang.top

[F07] 创建目录（含多级）
来源：http://ijm.zhaomingkeji.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vvu.hesvh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://duk.uphjek.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iyq.nwbrower.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gkt.xinyue.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pkl.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cvq.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xnf.hysaishi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://irr.hesvh.cn

[F08] 遍历目录
来源：http://kcp.xylfe.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xol.yueranfly.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aje.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://gbp.sweek.top

TS:   fs.readdirSync("dir")
来源：http://mhn.sweek.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xxy.hammf.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ptx.redwolf501.top

Ruby: Dir.children("dir")
来源：http://avq.sufxvd.cn

C#:   Directory.GetFiles("dir")
来源：http://jvm.dashuyun.cn

[F09] 获取文件大小
来源：http://hjy.chenjidiqi.icu

Py:   os.path.getsize("a.txt")
来源：http://ktm.sxryk.cn

PHP:  filesize("a.txt");
来源：http://rpn.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://tmf.yj202588.top

TS:   fs.statSync("a.txt").size
来源：http://jwd.jinghuilouyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pik.zdbjq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jhd.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://afl.nwbrower.top

C#:   new FileInfo("a.txt").Length
来源：http://whw.tian-w.cn

[F10] 取文件扩展名 / 文件名
来源：http://swp.ehwqpu.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://myq.zdbjq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://akd.jyoumei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ubo.wangshuangyany.cn

TS:   path.extname("a.txt")
来源：http://crf.cucudq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hln.feifeiyinyue.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zvh.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ekp.hysaishi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dzw.smart0.xyz

[F11] 复制与移动文件
来源：http://kos.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pxb.jinqigufen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zlq.hcnkem.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kmg.yongpay.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kds.guowangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://krt.xylfe.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tnj.xuanzx.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hmv.ctjpmb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rcu.ivvv.top

[F12] CSV 读写
来源：http://loi.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gqi.bbcook.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mhg.bbcook.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://idf.aizwys.cn

TS:   // 同上
来源：http://qxd.pycfn.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qfa.hnqzz.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kbb.xziqi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pxb.hnxiangtu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://toc.daria6918.cn

================================================================================
来源：http://hzo.yvedp.cn

G. 面向对象
来源：http://vid.yfazqb.com

================================================================================
来源：http://iau.ywan-chungtsiang.top

[G01] 定义类
来源：http://ans.fengsongda.top

Py:   class User: pass
来源：http://lsl.zhongyouzk.top

PHP:  class User {}
来源：http://eix.tanke756.top

JS:   class User {}
来源：http://eet.pycfn.com

TS:   class User { name: string = ""; }
来源：http://qef.tian-w.cn

Java: class User {}
来源：http://fzc.nanxinkj.top

Go:   type User struct { Name string }
来源：http://zik.chenjidiqi.icu

Ruby: class User; end
来源：http://hpz.quarkkingdee.top

C#:   class User {}
来源：http://zpy.hnxiangtu.top

[G02] 构造函数
来源：http://maf.wangdashe.top

Py:   def __init__(self, name): self.name = name
来源：http://rba.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://bjt.shanyushiyangtech.top

JS:   constructor(name) { this.name = name; }
来源：http://kfw.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://lco.jinyuanbaomall.cn

Java: User(String name) { this.name = name; }
来源：http://kdb.hfpthk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qla.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://ugn.jinqigufen.top

C#:   public User(string name) { Name = name; }
来源：http://isv.c1oappe.top

[G03] 实例属性
来源：http://bnf.meibo888.top

Py:   self.name = "x"
来源：http://ckt.dianchejie.cn

PHP:  public string $name = "x";
来源：http://ldb.dianchejie.cn

JS:   this.name = "x";
来源：http://qpg.redwolf501.top

TS:   name: string = "x";
来源：http://fmr.birdmap.top

Java: private String name;
来源：http://prn.yj20258888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ino.ydjk.org.cn

Ruby: @name = "x"
来源：http://btu.jqgfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://hya.gzhubu.top

[G04] 定义方法
来源：http://his.jianghu66.top

Py:   def greet(self): return self.name
来源：http://apk.cucudq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://has.gotoacloud.top

JS:   greet() { return this.name; }
来源：http://fjg.dianchejie.cn

TS:   greet(): string { return this.name; }
来源：http://aiy.tianlin.xyz

Java: String greet() { return name; }
来源：http://kil.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kcb.yuanzhike.top

Ruby: def greet; @name; end
来源：http://qqi.haohaochexian.top

C#:   public string Greet() => Name;
来源：http://jka.dashuyun.cn

[G05] 继承
来源：http://mmz.hammf.cn

Py:   class Admin(User): pass
来源：http://adn.bjfxy.top

PHP:  class Admin extends User {}
来源：http://vtt.uphjek.com

JS:   class Admin extends User {}
来源：http://isb.wangdashe.top

TS:   class Admin extends User {}
来源：http://ypf.jiagoushi.top

Java: class Admin extends User {}
来源：http://trq.dianchejie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xxc.gogol.net.cn

Ruby: class Admin < User; end
来源：http://mie.tanke756.top

C#:   class Admin : User {}
来源：http://mqp.vqdsnc.cn

[G06] 重写方法
来源：http://dgj.wangdashe.top

Py:   def greet(self): return "admin"
来源：http://qhf.zdqjudy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ywo.daxiang520.top

JS:   greet() { return "admin"; }
来源：http://jxt.yfazqb.com

TS:   greet(): string { return "admin"; }
来源：http://fqm.hnxiangtu.top

Java: @Override String greet() { return "admin"; }
来源：http://alb.kuanghao11.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zzw.nwbrower.top

Ruby: def greet; "admin"; end
来源：http://oxe.ppjwa.cn

C#:   public override string Greet() => "admin";
来源：http://esn.jiagoushi.top

[G07] 调用父类方法
来源：http://mul.dianchejie.cn

Py:   super().greet()
来源：http://rgq.hnqzz.top

PHP:  parent::greet();
来源：http://gut.ybcxt.top

JS:   super.greet();
来源：http://jxa.aizwys.cn

TS:   super.greet();
来源：http://rzj.aibaodan.cn

Java: super.greet();
来源：http://cxi.zycfv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://chh.guowangkeji.top

Ruby: super
来源：http://ifq.zdbjq.cn

C#:   base.Greet();
来源：http://ufn.meibo888.top

[G08] 静态方法与属性
来源：http://gzf.yuxming.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://utn.ehwqpu.com

PHP:  public static function f() {}
来源：http://bnw.ywan-chungtsiang.top

JS:   static f() {}
来源：http://dpg.zhongyouzk.top

TS:   static f(): void {}
来源：http://pkv.aibaodan.cn

Java: static void f() {}
来源：http://dka.fehbvm.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://jln.dianchejie.cn

Ruby: def self.f; end
来源：http://gxg.ivvv.top

C#:   public static void F() {}
来源：http://yjj.zdqjudy.top

[G09] 接口 / 抽象类
来源：http://hpy.nanxinkj.top

Py:   from abc import ABC, abstractmethod
来源：http://vhz.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fep.xinyue.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://ukv.vehdjk.com

TS:   interface Shape { area(): number; }
来源：http://mcs.xuanzx.com

Java: interface Shape { double area(); }
来源：http://wiy.wangdashe.top

Go:   type Shape interface { Area() float64 }
来源：http://idm.jlsjyb.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iqe.hnqzz.top

C#:   interface IShape { double Area(); }
来源：http://fsd.hnqzz.top

[G10] 访问控制
来源：http://gjd.hfpthk.cn

Py:   约定 _protected / __private（不强制）
来源：http://raz.9152youxi.cn

PHP:  public / protected / private
来源：http://jen.daxiang520.top

JS:   #private 字段；其余公开
来源：http://hjo.zycfv.cn

TS:   public / protected / private
来源：http://xou.jyoumei.cn

Java: public / protected / private / 默认包级
来源：http://ecs.52xcode.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tiw.hnxiangtu.top

Ruby: public / protected / private
来源：http://ity.xuanzx.com

C#:   public / protected / private / internal
来源：http://wzy.cqqwz.cn

[G11] getter / setter
来源：http://jby.jinqigfzy.top

Py:   @property 与 @x.setter
来源：http://msf.pycfn.com

PHP:  public function getName(): string { return $this->name; }
来源：http://abq.xylfe.cn

JS:   get name() { return this._name; }
来源：http://ozd.chenlongwang.top

TS:   get name(): string { return this._name; }
来源：http://wcd.gaohongyu789.top

Java: public String getName() { return name; }
来源：http://zlr.guannengcc.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fhn.xziqi.cn

Ruby: attr_accessor :name
来源：http://jzb.sjlbkw.cn

C#:   public string Name { get; set; }
来源：http://vka.shuidangran.top

[G12] 对象转字符串
来源：http://ild.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://bjj.316326.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://loq.shuidangran.top

JS:   toString() { return this.name; }
来源：http://ans.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://yuu.zdbjq.cn

Java: @Override public String toString() { return name; }
来源：http://pce.gotoacloud.top

Go:   func (u User) String() string { return u.Name }
来源：http://zbu.ydjk.org.cn

Ruby: def to_s; @name; end
来源：http://oig.andypj.xyz

C#:   public override string ToString() => Name;
来源：http://cbl.haohaochexian.top

[G13] 判断对象类型
来源：http://gwr.daxiang520.top

Py:   isinstance(u, User)
来源：http://mic.hfpthk.cn

PHP:  $u instanceof User
来源：http://oyz.shanyushiyangtech.top

JS:   u instanceof User
来源：http://zbb.hfpthk.cn

TS:   u instanceof User
来源：http://ozc.epnwcf.com

Java: u instanceof User
来源：http://ryi.smart0.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://cwx.nanxuanxn.top

Ruby: u.is_a?(User)
来源：http://kdu.316326.xyz

C#:   u is User
来源：http://lrt.sxryk.cn

[G14] 数据类 / record
来源：http://por.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ple.bjfxy.top

PHP:  // 用 readonly 属性模拟
来源：http://erv.bjfxy.top

JS:   // 无内置：普通类或对象字面量
来源：http://hbk.ppjwa.cn

TS:   type User = { name: string; age: number };
来源：http://jvn.dianchejie.cn

Java: record User(String name, int age) {}
来源：http://zfv.cdnleiting.top

Go:   type User struct { Name string; Age int }
来源：http://plv.hcnkem.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mao.jianghu66.top

C#:   record User(string Name, int Age);
来源：http://nds.vqdsnc.cn

[G15] 枚举
来源：http://wjg.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ctr.sufxvd.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ofk.yj202588.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rgx.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://muq.hongshengwenyu.top

Java: enum Color { RED, GREEN }
来源：http://ogr.gaohongyu789.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vwd.xylfe.cn

Ruby: Color = %i[red green].freeze
来源：http://aag.hywenlv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xmr.cashguo.top

[G16] 对象转数组 / 字典
来源：http://khu.fanxiaobao.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yil.xylfe.cn

PHP:  get_object_vars($obj);
来源：http://nyf.svipenyu.cn

JS:   Object.entries(obj)
来源：http://nwm.ydzc1.top

TS:   Object.entries(obj)
来源：http://tae.fehbvm.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qqv.cqqwz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xlo.yj20258888.top

Ruby: obj.instance_variables
来源：http://cuy.wangshuangyany.cn

C#:   // 用反射或 System.Text.Json
来源：http://aec.xuetiantiany.cn

================================================================================
来源：http://hcz.tianlin.xyz

H. 异常与错误处理
来源：http://hmm.fzhhl.top

================================================================================
来源：http://uxe.feifeiyinyue.top

[H01] try / catch 基础
来源：http://vaa.wangshuangyany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mmd.fanxiaobao.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yak.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://spz.mhx1999.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cje.yangfankeji.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uab.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zbr.bbcook.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://agn.sufxvd.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fgb.zdqjudy.top

[H02] finally / ensure 收尾
来源：http://pms.cheryme.top

Py:   try: f()⏎finally: cleanup()
来源：http://lem.hywenlv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tpp.daxiang520.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zya.xuetiantiany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ssa.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://mvk.wangshuangyany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uje.snrcjt.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://etk.chenlongwang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dyu.yj20258888.top

[H03] 主动抛出异常
来源：http://fuh.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://knv.hywenlv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rne.zhaomingkeji.xyz

JS:   throw new Error("错误信息");
来源：http://yqe.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://vpy.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://iww.yanxiufei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cap.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ncp.hesvh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tvu.guowangkeji.top

[H04] 自定义异常类型
来源：http://agi.fengsongda.top

Py:   class MyError(Exception): pass
来源：http://quj.fehbvm.com

PHP:  class MyError extends RuntimeException {}
来源：http://ojy.zhengqikj.top

JS:   class MyError extends Error {}
来源：http://uma.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://voy.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://xng.zdqjudy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mra.zycfv.cn

Ruby: class MyError < StandardError; end
来源：http://sgu.feifeiyinyue.top

C#:   class MyException : Exception {}
来源：http://tit.gotoacloud.top

[H05] 捕获特定类型
来源：http://xse.ctjpmb.com

Py:   except ValueError as e:
来源：http://rjt.daxiang520.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vmw.chenzaomai.com

JS:   if (e instanceof TypeError) {}
来源：http://rqa.zhengqikj.top

TS:   if (e instanceof TypeError) {}
来源：http://isf.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://vjo.zycfv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lwk.aizwys.cn

Ruby: rescue ArgumentError => e
来源：http://pdi.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://igm.tarul.cn

[H06] 可选值 / 空值安全访问
来源：http://lnx.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://ing.uphjek.com

PHP:  $v = $d["k"] ?? null;
来源：http://mjy.guannengcc.top

JS:   obj?.a?.b;  d ?? default
来源：http://ihc.shuidangran.top

TS:   obj?.a?.b;  d ?? default
来源：http://qln.xziqi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://muk.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cld.birdmap.top

Ruby: d&.dig(:a, :b)
来源：http://ete.shanyushiyangkeji.top

C#:   obj?.A?.B ?? default
来源：http://fov.nanxuanxn.top

[H07] 断言
来源：http://teu.xingfuxueyuan.xyz

Py:   assert x > 0, "必须为正"
来源：http://ejz.wangdashe.top

PHP:  assert($x > 0);
来源：http://vmx.yfazqb.com

JS:   console.assert(x > 0);
来源：http://irw.iojbl.cn

TS:   console.assert(x > 0);
来源：http://awd.gotoacloud.top

Java: assert x > 0 : "必须为正";
来源：http://vhf.sweek.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ahq.gaohongyu789.top

Ruby: raise "必须为正" unless x > 0
来源：http://ewi.sjlbkw.cn

C#:   Debug.Assert(x > 0);
来源：http://qdf.cucudq.cn

[H08] 获取错误信息与堆栈
来源：http://aca.tarul.cn

Py:   str(e);  traceback.format_exc()
来源：http://sma.gogol.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tua.hammf.cn

JS:   e.message;  e.stack
来源：http://phn.yfazqb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://ukv.9152youxi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vpa.jianghu66.top

Go:   err.Error()
来源：http://wzz.52xcode.cn

Ruby: e.message;  e.backtrace
来源：http://ibc.dashuyun.cn

C#:   e.Message;  e.StackTrace
来源：http://zuv.xylfe.cn

[H09] 带错误码的异常
来源：http://alb.snrcjt.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cbw.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jfw.xinyue.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zeu.ivvv.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://phw.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vfs.birdmap.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wti.yueranfly.top

Ruby: raise MyError.new("fail", 500)
来源：http://psj.aizwys.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sex.zhiwuduotai.top

[H10] 资源自动释放
来源：http://zhk.jlsjyb.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zzw.0kj1m.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qys.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://atz.chenjidiqi.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vtd.snrcjt.cn


<!-- 参考信息 -->